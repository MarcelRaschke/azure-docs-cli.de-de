---
title: Azure CLI 2.0-Versionshinweise
description: Enthält Informationen zu den aktuellen Updates von Azure CLI 2.0.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 06/01/2018
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 57f13c7d17e2d248132e2e9c49bb0b4994f041f5
ms.sourcegitcommit: 80189ff103c91f8c47ab8ebf586df815fff5dd5d
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/05/2018
ms.locfileid: "34799259"
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="78b41-103">Azure CLI 2.0-Versionshinweise</span><span class="sxs-lookup"><span data-stu-id="78b41-103">Azure CLI 2.0 release notes</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="78b41-104">5. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="78b41-104">June 5, 2018</span></span>

<span data-ttu-id="78b41-105">Version 2.0.34</span><span class="sxs-lookup"><span data-stu-id="78b41-105">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="78b41-106">Core</span><span class="sxs-lookup"><span data-stu-id="78b41-106">Core</span></span>

* <span data-ttu-id="78b41-107">Unterstützung für mandantenübergreifende Ressourcenverweise hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-107">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="78b41-108">Verbesserte Zuverlässigkeit bei Telemetrieuploads</span><span class="sxs-lookup"><span data-stu-id="78b41-108">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="78b41-109">ACR</span><span class="sxs-lookup"><span data-stu-id="78b41-109">ACR</span></span>

* <span data-ttu-id="78b41-110">Unterstützung für VSTS als Remotequellort hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-110">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="78b41-111">Befehl `acr import` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-111">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="78b41-112">AKS</span><span class="sxs-lookup"><span data-stu-id="78b41-112">AKS</span></span>

* <span data-ttu-id="78b41-113">`aks get-credentials` wurde geändert, um die Kube-Konfigurationsdatei mit sichereren Dateisystemberechtigungen zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="78b41-113">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="78b41-114">Batch</span><span class="sxs-lookup"><span data-stu-id="78b41-114">Batch</span></span>

* <span data-ttu-id="78b41-115">Fehler bei der Formatierung der Poollistentabelle behoben [[Problem 4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="78b41-115">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="78b41-116">IoT</span><span class="sxs-lookup"><span data-stu-id="78b41-116">IOT</span></span>

* <span data-ttu-id="78b41-117">Unterstützung für das Erstellen von IoT Hub-Instanzen im Tarif „Basic“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-117">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="78b41-118">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="78b41-118">Network</span></span>

* <span data-ttu-id="78b41-119">`network vnet peering` wurde verbessert.</span><span class="sxs-lookup"><span data-stu-id="78b41-119">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="78b41-120">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="78b41-120">Policy Insights</span></span>

* <span data-ttu-id="78b41-121">Erste Version</span><span class="sxs-lookup"><span data-stu-id="78b41-121">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="78b41-122">ARM</span><span class="sxs-lookup"><span data-stu-id="78b41-122">ARM</span></span>

* <span data-ttu-id="78b41-123">Befehle vom Typ `account management-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-123">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="78b41-124">SQL</span><span class="sxs-lookup"><span data-stu-id="78b41-124">SQL</span></span>

* <span data-ttu-id="78b41-125">Neue Befehle für verwaltete Instanzen hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="78b41-125">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="78b41-126">Neue Befehle für verwaltete Datenbanken hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="78b41-126">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="78b41-127">Speicher</span><span class="sxs-lookup"><span data-stu-id="78b41-127">Storage</span></span>

* <span data-ttu-id="78b41-128">Zusätzliche MimeTypes für JSON und JavaScript hinzugefügt (abzuleiten aus Dateierweiterungen)</span><span class="sxs-lookup"><span data-stu-id="78b41-128">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="78b41-129">VM</span><span class="sxs-lookup"><span data-stu-id="78b41-129">VM</span></span>

* <span data-ttu-id="78b41-130">`vm list-skus` wurde geändert, um feste Spalten zu verwenden und eine Warnung hinzuzufügen, dass `Tier` und `Size` entfernt werden.</span><span class="sxs-lookup"><span data-stu-id="78b41-130">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="78b41-131">Option `--accelerated-networking` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-131">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="78b41-132">`--tags` zu `identity create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-132">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="78b41-133">22. Mai 2018</span><span class="sxs-lookup"><span data-stu-id="78b41-133">May 22, 2018</span></span>

<span data-ttu-id="78b41-134">Version 2.0.33</span><span class="sxs-lookup"><span data-stu-id="78b41-134">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="78b41-135">Core</span><span class="sxs-lookup"><span data-stu-id="78b41-135">Core</span></span>

* <span data-ttu-id="78b41-136">Unterstützung für das Erweitern von `@` in Dateinamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-136">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="78b41-137">ACS</span><span class="sxs-lookup"><span data-stu-id="78b41-137">ACS</span></span>

* <span data-ttu-id="78b41-138">Neue Dev Spaces-Befehle `aks use-dev-spaces` und `aks remove-dev-spaces` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-138">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="78b41-139">Tippfehler in Hilfemeldung korrigiert</span><span class="sxs-lookup"><span data-stu-id="78b41-139">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="78b41-140">AppService</span><span class="sxs-lookup"><span data-stu-id="78b41-140">AppService</span></span>

* <span data-ttu-id="78b41-141">Verbesserte generische Aktualisierungsbefehle</span><span class="sxs-lookup"><span data-stu-id="78b41-141">Improved generic update commands</span></span>
* <span data-ttu-id="78b41-142">Asynchrone Unterstützung für `webapp deployment source config-zip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-142">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="78b41-143">Container</span><span class="sxs-lookup"><span data-stu-id="78b41-143">Container</span></span>

* <span data-ttu-id="78b41-144">Unterstützung für das Exportieren einer Containergruppe im YAML-Format hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-144">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="78b41-145">Unterstützung für die Verwendung einer YAML-Datei zum Erstellen/Aktualisieren einer Containergruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-145">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="78b41-146">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="78b41-146">Extension</span></span>

* <span data-ttu-id="78b41-147">Verbesserte Entfernung von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="78b41-147">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="78b41-148">Interactive</span><span class="sxs-lookup"><span data-stu-id="78b41-148">Interactive</span></span>

* <span data-ttu-id="78b41-149">Protokollierung geändert, um Parser für Abschlüsse zu deaktivieren</span><span class="sxs-lookup"><span data-stu-id="78b41-149">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="78b41-150">Verbesserte Verarbeitung beschädigter Hilfscaches</span><span class="sxs-lookup"><span data-stu-id="78b41-150">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="78b41-151">KeyVault</span><span class="sxs-lookup"><span data-stu-id="78b41-151">KeyVault</span></span>

* <span data-ttu-id="78b41-152">keyvault-Befehle wurden korrigiert, damit sie in Cloud Shell oder auf virtuellen Computern mit Identität verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="78b41-152">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="78b41-153">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="78b41-153">Network</span></span>

* <span data-ttu-id="78b41-154">Problem behoben, aufgrund dessen `network watcher show-topology` nicht mit einem VNET und/oder Subnetznamen verwendet werden konnte ([#6326](https://github.com/Azure/azure-cli/issues/6326))</span><span class="sxs-lookup"><span data-stu-id="78b41-154">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="78b41-155">Problem behoben, aufgrund dessen einige `network watcher`-Befehle fälschlicherweise angaben, dass Network Watcher nicht für bestimmte Regionen aktiviert ist ([#6264](https://github.com/Azure/azure-cli/issues/6264))</span><span class="sxs-lookup"><span data-stu-id="78b41-155">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="78b41-156">SQL</span><span class="sxs-lookup"><span data-stu-id="78b41-156">SQL</span></span>

* <span data-ttu-id="78b41-157">[WICHTIGE ÄNDERUNG] Von den Befehlen `db` und `dw` zurückgegebene Antwortobjekte geändert:</span><span class="sxs-lookup"><span data-stu-id="78b41-157">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="78b41-158">Eigenschaft `serviceLevelObjective` in `currentServiceObjectiveName` umbenannt</span><span class="sxs-lookup"><span data-stu-id="78b41-158">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="78b41-159">Eigenschaften `currentServiceObjectiveId` und `requestedServiceObjectiveId` entfernt</span><span class="sxs-lookup"><span data-stu-id="78b41-159">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span> 
    * <span data-ttu-id="78b41-160">Eigenschaft `maxSizeBytes` geändert (ist nun keine Zeichenfolge mehr, sondern ein Ganzzahlwert)</span><span class="sxs-lookup"><span data-stu-id="78b41-160">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="78b41-161">[WICHTIGE ÄNDERUNG] Die folgenden `db`- und `dw`-Eigenschaften wurden geändert und sind jetzt schreibgeschützt:</span><span class="sxs-lookup"><span data-stu-id="78b41-161">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="78b41-162">`requestedServiceObjectiveName`(Fixierte Verbindung) festgelegt ist(Fixierte Verbindung) festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="78b41-162">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="78b41-163">Verwenden Sie zum Aktualisieren den Parameter `--service-objective`, oder legen Sie die Eigenschaft `sku.name` fest.</span><span class="sxs-lookup"><span data-stu-id="78b41-163">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="78b41-164">`edition`(Fixierte Verbindung) festgelegt ist(Fixierte Verbindung) festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="78b41-164">`edition`.</span></span> <span data-ttu-id="78b41-165">Verwenden Sie zum Aktualisieren den Parameter `--edition`, oder legen Sie die Eigenschaft `sku.tier` fest.</span><span class="sxs-lookup"><span data-stu-id="78b41-165">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="78b41-166">`elasticPoolName`(Fixierte Verbindung) festgelegt ist(Fixierte Verbindung) festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="78b41-166">`elasticPoolName`.</span></span> <span data-ttu-id="78b41-167">Verwenden Sie zum Aktualisieren den Parameter `--elastic-pool`, oder legen Sie die Eigenschaft `elasticPoolId` fest.</span><span class="sxs-lookup"><span data-stu-id="78b41-167">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="78b41-168">[WICHTIGE ÄNDERUNG] Die folgenden `elastic-pool`-Eigenschaften wurden geändert und sind jetzt schreibgeschützt:</span><span class="sxs-lookup"><span data-stu-id="78b41-168">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="78b41-169">`edition`(Fixierte Verbindung) festgelegt ist(Fixierte Verbindung) festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="78b41-169">`edition`.</span></span> <span data-ttu-id="78b41-170">Verwenden Sie zum Aktualisieren den Parameter `--edition`.</span><span class="sxs-lookup"><span data-stu-id="78b41-170">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="78b41-171">`dtu`(Fixierte Verbindung) festgelegt ist(Fixierte Verbindung) festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="78b41-171">`dtu`.</span></span> <span data-ttu-id="78b41-172">Verwenden Sie zum Aktualisieren den Parameter `--capacity`.</span><span class="sxs-lookup"><span data-stu-id="78b41-172">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="78b41-173">`databaseDtuMin`(Fixierte Verbindung) festgelegt ist(Fixierte Verbindung) festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="78b41-173">`databaseDtuMin`.</span></span> <span data-ttu-id="78b41-174">Verwenden Sie zum Aktualisieren den Parameter `--db-min-capacity`.</span><span class="sxs-lookup"><span data-stu-id="78b41-174">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="78b41-175">`databaseDtuMax`(Fixierte Verbindung) festgelegt ist(Fixierte Verbindung) festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="78b41-175">`databaseDtuMax`.</span></span> <span data-ttu-id="78b41-176">Verwenden Sie zum Aktualisieren den Parameter `--db-max-capacity`.</span><span class="sxs-lookup"><span data-stu-id="78b41-176">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="78b41-177">Die Parameter `--family` und `--capacity` wurden zu den `db`-, `dw`- und `elastic-pool`-Befehlen hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="78b41-177">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="78b41-178">Den `db`-, `dw`- und `elastic-pool`-Befehlen wurden Tabellenformatierer hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="78b41-178">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="78b41-179">Speicher</span><span class="sxs-lookup"><span data-stu-id="78b41-179">Storage</span></span>

* <span data-ttu-id="78b41-180">Vervollständigung für das Argument `--account-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-180">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="78b41-181">Problem mit `storage entity query` behoben</span><span class="sxs-lookup"><span data-stu-id="78b41-181">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="78b41-182">VM</span><span class="sxs-lookup"><span data-stu-id="78b41-182">VM</span></span>

* <span data-ttu-id="78b41-183">[WICHTIGE ÄNDERUNG] `--write-accelerator` aus `vm create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="78b41-183">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="78b41-184">Die gleiche Unterstützung kann über `vm update` oder `vm disk attach` erzielt werden.</span><span class="sxs-lookup"><span data-stu-id="78b41-184">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="78b41-185">Erweiterungsimageabgleich in `[vm|vmss] extension` korrigiert</span><span class="sxs-lookup"><span data-stu-id="78b41-185">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="78b41-186">`--boot-diagnostics-storage` zu `vm create` zur Erfassung des Startprotokolls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-186">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="78b41-187">`--license-type` zu `[vm|vmss] update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-187">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="78b41-188">7. Mai 2018</span><span class="sxs-lookup"><span data-stu-id="78b41-188">May 7, 2018</span></span>

<span data-ttu-id="78b41-189">Version 2.0.32</span><span class="sxs-lookup"><span data-stu-id="78b41-189">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="78b41-190">Core</span><span class="sxs-lookup"><span data-stu-id="78b41-190">Core</span></span>

* <span data-ttu-id="78b41-191">Ein Ausnahmefehler wurde behoben, der beim Abrufen von Geheimnissen aus einem Dienstprinzipalkonto mit Zertifikat auftrat.</span><span class="sxs-lookup"><span data-stu-id="78b41-191">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="78b41-192">Eingeschränkte Unterstützung für positionelle Argumente hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-192">Added limited support for positional arguments</span></span>
* <span data-ttu-id="78b41-193">Problem behoben, aufgrund dessen `--query` nicht mit `--ids` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="78b41-193">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="78b41-194">#5591</span><span class="sxs-lookup"><span data-stu-id="78b41-194">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="78b41-195">Pipingszenarien von Befehlen bei Verwendung von `--ids` verbessert</span><span class="sxs-lookup"><span data-stu-id="78b41-195">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="78b41-196">Unterstützt `-o tsv` mit angegebener Abfrage bzw. `-o json` ohne angegeben Abfrage</span><span class="sxs-lookup"><span data-stu-id="78b41-196">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="78b41-197">Befehlsvorschläge bei Fehler hinzugefügt, wenn Befehle Tippfehler enthielten</span><span class="sxs-lookup"><span data-stu-id="78b41-197">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="78b41-198">Fehler bei der Eingabe von `az ''` behandelt</span><span class="sxs-lookup"><span data-stu-id="78b41-198">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="78b41-199">Unterstützung für benutzerdefinierte Ressourcentypen für Befehlsmodule und -erweiterungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-199">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="78b41-200">ACR</span><span class="sxs-lookup"><span data-stu-id="78b41-200">ACR</span></span>

* <span data-ttu-id="78b41-201">ACR Build-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-201">Added ACR Build commands</span></span>
* <span data-ttu-id="78b41-202">Fehlermeldungen vom Typ „Ressource nicht gefunden.“ verbessert</span><span class="sxs-lookup"><span data-stu-id="78b41-202">Improved resource not found error messages</span></span>
* <span data-ttu-id="78b41-203">Höhere Leistung bei der Ressourcenerstellung und optimierte Fehlerbehandlung</span><span class="sxs-lookup"><span data-stu-id="78b41-203">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="78b41-204">ACR-Anmeldung bei nicht standardmäßigen Konsolen und WSL optimiert</span><span class="sxs-lookup"><span data-stu-id="78b41-204">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="78b41-205">Fehlermeldungen zu Repositorybefehlen optimiert</span><span class="sxs-lookup"><span data-stu-id="78b41-205">Improved repository commands error messages</span></span>
* <span data-ttu-id="78b41-206">Tabellenspalten und -reihenfolge aktualisiert</span><span class="sxs-lookup"><span data-stu-id="78b41-206">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="78b41-207">ACS</span><span class="sxs-lookup"><span data-stu-id="78b41-207">ACS</span></span>

* <span data-ttu-id="78b41-208">Warnung hinzugefügt, dass `az aks` eine Vorschauversion des Diensts ist</span><span class="sxs-lookup"><span data-stu-id="78b41-208">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="78b41-209">Berechtigungsproblem in `aks install-connector` behoben, wenn `--aci-resource-group` nicht angegeben wird</span><span class="sxs-lookup"><span data-stu-id="78b41-209">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="78b41-210">AMS</span><span class="sxs-lookup"><span data-stu-id="78b41-210">AMS</span></span>

* <span data-ttu-id="78b41-211">Erste Version: Verwalten von Azure Media Services-Ressourcen</span><span class="sxs-lookup"><span data-stu-id="78b41-211">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="78b41-212">AppService</span><span class="sxs-lookup"><span data-stu-id="78b41-212">Appservice</span></span>

* <span data-ttu-id="78b41-213">Ein Problem in `webapp delete` wurde behoben, das bei Angabe von `--slot` auftrat.</span><span class="sxs-lookup"><span data-stu-id="78b41-213">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="78b41-214">`--runtime-version` aus `webapp auth update` entfernt</span><span class="sxs-lookup"><span data-stu-id="78b41-214">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="78b41-215">Unterstützung für „min\_tls\_version“ und „https2.0“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-215">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="78b41-216">Unterstützung für mehrere Container hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-216">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="78b41-217">Batch AI</span><span class="sxs-lookup"><span data-stu-id="78b41-217">Batch AI</span></span>

* <span data-ttu-id="78b41-218">`batchai create cluster` wurde geändert, um die in der Konfigurationsdatei des Clusters konfigurierte VM-Priorität zu berücksichtigen.</span><span class="sxs-lookup"><span data-stu-id="78b41-218">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="78b41-219">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="78b41-219">Cognitive Services</span></span>

* <span data-ttu-id="78b41-220">Tippfehler im Beispiel für `cognitiveservices account create` korrigiert ([#5603](https://github.com/Azure/azure-cli/issues/5603))</span><span class="sxs-lookup"><span data-stu-id="78b41-220">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="78b41-221">Nutzung</span><span class="sxs-lookup"><span data-stu-id="78b41-221">Consumption</span></span>

* <span data-ttu-id="78b41-222">Neue Befehle für Budget-API hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-222">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="78b41-223">Container</span><span class="sxs-lookup"><span data-stu-id="78b41-223">Container</span></span>

* <span data-ttu-id="78b41-224">`--registry-server` muss nicht mehr für `container create` angegeben werden, wenn ein Registrierungsserver im Imagenamen enthalten ist.</span><span class="sxs-lookup"><span data-stu-id="78b41-224">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="78b41-225">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="78b41-225">Cosmos DB</span></span>

* <span data-ttu-id="78b41-226">VNET-Unterstützung für Azure CLI eingeführt: Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="78b41-226">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="78b41-227">DMS</span><span class="sxs-lookup"><span data-stu-id="78b41-227">DMS</span></span>

* <span data-ttu-id="78b41-228">Erste Version: Die Migration von SQL zu Azure SQL wird nun unterstützt.</span><span class="sxs-lookup"><span data-stu-id="78b41-228">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="78b41-229">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="78b41-229">Extension</span></span>

* <span data-ttu-id="78b41-230">Fehler behoben, aufgrund dessen Erweiterungsmetadaten nicht mehr angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="78b41-230">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="78b41-231">Interactive</span><span class="sxs-lookup"><span data-stu-id="78b41-231">Interactive</span></span>

* <span data-ttu-id="78b41-232">Interaktive Vervollständigung funktioniert nun auch mit positionellen Argumenten.</span><span class="sxs-lookup"><span data-stu-id="78b41-232">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="78b41-233">Benutzerfreundlichere Ausgabe bei der Eingabe von '\'</span><span class="sxs-lookup"><span data-stu-id="78b41-233">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="78b41-234">Abschlüsse für Parameter ohne Hilfe korrigiert</span><span class="sxs-lookup"><span data-stu-id="78b41-234">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="78b41-235">Beschreibungen für Befehlsgruppen korrigiert</span><span class="sxs-lookup"><span data-stu-id="78b41-235">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="78b41-236">Labor</span><span class="sxs-lookup"><span data-stu-id="78b41-236">Lab</span></span>

* <span data-ttu-id="78b41-237">Regressionen aus Knack-Umwandlung korrigiert</span><span class="sxs-lookup"><span data-stu-id="78b41-237">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="78b41-238">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="78b41-238">Network</span></span>

* <span data-ttu-id="78b41-239">[WICHTIGE ÄNDERUNG] Parameter `--ids` entfernt für:</span><span class="sxs-lookup"><span data-stu-id="78b41-239">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span> 
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="78b41-240">Profil</span><span class="sxs-lookup"><span data-stu-id="78b41-240">Profile</span></span>

* <span data-ttu-id="78b41-241">Quellerkennung für `disk create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="78b41-241">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="78b41-242">[WICHTIGE ÄNDERUNG] `--msi-port` und `--identity-port` entfernt, da sie nicht mehr verwendet werden</span><span class="sxs-lookup"><span data-stu-id="78b41-242">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="78b41-243">Tippfehler in kurzer Zusammenfassung für `account get-access-token` korrigiert</span><span class="sxs-lookup"><span data-stu-id="78b41-243">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="78b41-244">Redis</span><span class="sxs-lookup"><span data-stu-id="78b41-244">Redis</span></span>

* <span data-ttu-id="78b41-245">`redis patch-schedule patch-schedule show` wurde durch `redis patch-schedule show` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="78b41-245">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="78b41-246">`redis list-all` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="78b41-246">Deprecated `redis list-all`.</span></span> <span data-ttu-id="78b41-247">Diese Funktion wurde in `redis list` integriert.</span><span class="sxs-lookup"><span data-stu-id="78b41-247">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="78b41-248">`redis import-method` wurde durch `redis import` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="78b41-248">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="78b41-249">Unterstützung für `--ids` zu verschiedenen Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-249">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="78b41-250">Rolle</span><span class="sxs-lookup"><span data-stu-id="78b41-250">Role</span></span>

* <span data-ttu-id="78b41-251">[WICHTIGE ÄNDERUNG] Veralteter Befehl `ad sp reset-credentials` entfernt</span><span class="sxs-lookup"><span data-stu-id="78b41-251">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="78b41-252">Speicher</span><span class="sxs-lookup"><span data-stu-id="78b41-252">Storage</span></span>

* <span data-ttu-id="78b41-253">Zulassen, dass das Ziel-SAS-Token für die Blobkopie auf die Quelle angewendet wird, wenn Quell-SAS und Kontoschlüssel nicht angegeben werden</span><span class="sxs-lookup"><span data-stu-id="78b41-253">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="78b41-254">Verfügbar gemacht: Socket-Timeout für Blobuploads und -downloads</span><span class="sxs-lookup"><span data-stu-id="78b41-254">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="78b41-255">Blobnamen, die mit Pfadtrennzeichen beginnen, als relative Pfade behandeln</span><span class="sxs-lookup"><span data-stu-id="78b41-255">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="78b41-256">Zulassen, dass `storage blob copy --source-sas` mit dem Abfragezeichen „?“ beginnt</span><span class="sxs-lookup"><span data-stu-id="78b41-256">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="78b41-257">`storage entity query --marker` korrigiert, um Liste von Schlüsselwerten zu akzeptieren</span><span class="sxs-lookup"><span data-stu-id="78b41-257">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="78b41-258">VM</span><span class="sxs-lookup"><span data-stu-id="78b41-258">VM</span></span>

* <span data-ttu-id="78b41-259">Ungültige Erkennungslogik für nicht verwalteten Blob-URI korrigiert</span><span class="sxs-lookup"><span data-stu-id="78b41-259">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="78b41-260">Unterstützung für Datenträgerverschlüsselung ohne vom Benutzer bereitgestellte Dienstprinzipale hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-260">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="78b41-261">[WICHTIGE ÄNDERUNG] Verwenden Sie nicht „ManagedIdentityExtension“ des virtuellen Computers für MSI-Unterstützung.</span><span class="sxs-lookup"><span data-stu-id="78b41-261">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="78b41-262">Unterstützung für Entfernungsrichtlinie zu `vmss` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-262">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="78b41-263">[WICHTIGE ÄNDERUNG] `--ids` entfernt aus:</span><span class="sxs-lookup"><span data-stu-id="78b41-263">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="78b41-264">Unterstützung für Schreibbeschleunigung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-264">Added write accelerator support</span></span> 
* <span data-ttu-id="78b41-265">`vmss perform-maintenance` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-265">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="78b41-266">`vm diagnostics set` korrigiert, um zuverlässig den Betriebssystemtyp des virtuellen Computers zu erkennen</span><span class="sxs-lookup"><span data-stu-id="78b41-266">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="78b41-267">`vm resize` geändert, um zu überprüfen, ob die angeforderte Größe von der derzeit festgelegten Größe abweicht, und nur bei einer Änderung eine Aktualisierung auszuführen</span><span class="sxs-lookup"><span data-stu-id="78b41-267">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="78b41-268">10. April 2018</span><span class="sxs-lookup"><span data-stu-id="78b41-268">April 10, 2018</span></span>

<span data-ttu-id="78b41-269">Version 2.0.31</span><span class="sxs-lookup"><span data-stu-id="78b41-269">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="78b41-270">ACR</span><span class="sxs-lookup"><span data-stu-id="78b41-270">ACR</span></span>

* <span data-ttu-id="78b41-271">Verbesserte Fehlerbehandlung für wincred-Fallback</span><span class="sxs-lookup"><span data-stu-id="78b41-271">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="78b41-272">ACS</span><span class="sxs-lookup"><span data-stu-id="78b41-272">ACS</span></span>

* <span data-ttu-id="78b41-273">Gültigkeit von per AKS erstellten SPNs in fünf Jahre geändert</span><span class="sxs-lookup"><span data-stu-id="78b41-273">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="78b41-274">AppService</span><span class="sxs-lookup"><span data-stu-id="78b41-274">Appservice</span></span>

* [WICHTIGE ÄNDERUNG]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="78b41-276">Nicht abgefangene Ausnahme für nicht vorhandene Web-App-Pläne behoben</span><span class="sxs-lookup"><span data-stu-id="78b41-276">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="78b41-277">Batch AI</span><span class="sxs-lookup"><span data-stu-id="78b41-277">BatchAI</span></span>

* <span data-ttu-id="78b41-278">Unterstützung für API 2018-03-01 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-278">Added support for 2018-03-01 API</span></span>

 - <span data-ttu-id="78b41-279">Bereitstellung auf Auftragsebene</span><span class="sxs-lookup"><span data-stu-id="78b41-279">Job level mounting</span></span>
 - <span data-ttu-id="78b41-280">Umgebungsvariablen mit Geheimniswerten</span><span class="sxs-lookup"><span data-stu-id="78b41-280">Environment variables with secret values</span></span>
 - <span data-ttu-id="78b41-281">Einstellungen von Leistungsindikatoren</span><span class="sxs-lookup"><span data-stu-id="78b41-281">Performance counters settings</span></span>
 - <span data-ttu-id="78b41-282">Berichtstellung für auftragsspezifisches Pfadsegment</span><span class="sxs-lookup"><span data-stu-id="78b41-282">Reporting of job specific path segment</span></span>
 - <span data-ttu-id="78b41-283">Unterstützung für Unterordner in Listendateien-API</span><span class="sxs-lookup"><span data-stu-id="78b41-283">Support for subfolders in list files api</span></span>
 - <span data-ttu-id="78b41-284">Berichterstellung zur Nutzung und zu Grenzwerten</span><span class="sxs-lookup"><span data-stu-id="78b41-284">Usage and limits reporting</span></span>
 - <span data-ttu-id="78b41-285">Zulassen der Angabe des Cachetyps für NFS-Server</span><span class="sxs-lookup"><span data-stu-id="78b41-285">Allow to specify caching type for NFS servers</span></span>
 - <span data-ttu-id="78b41-286">Unterstützung für benutzerdefinierte Images</span><span class="sxs-lookup"><span data-stu-id="78b41-286">Support for custom images</span></span>
 - <span data-ttu-id="78b41-287">Unterstützung für pyTorch-Toolkit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-287">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="78b41-288">Befehl `job wait` hinzugefügt, der das Warten auf die Auftragsfertigstellung ermöglicht und den Code für die Auftragsbeendigung meldet</span><span class="sxs-lookup"><span data-stu-id="78b41-288">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="78b41-289">Befehl `usage show` hinzugefügt, mit dem die aktuelle Nutzung von Batch AI-Ressourcen und die Grenzwerte für verschiedene Regionen aufgelistet werden</span><span class="sxs-lookup"><span data-stu-id="78b41-289">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="78b41-290">Nationale Clouds werden unterstützt</span><span class="sxs-lookup"><span data-stu-id="78b41-290">National clouds are supported</span></span>
* <span data-ttu-id="78b41-291">Befehlszeilenargumente für Aufträge hinzugefügt, um das Bereitstellen von Dateisystemen auf Auftragsebene zusätzlich zu Konfigurationsdateien zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="78b41-291">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="78b41-292">Weitere Optionen zum Anpassen von Clustern hinzugefügt – VM-Priorität, Subnetz, anfängliche Knotenanzahl für Cluster mit automatischer Skalierung, Angeben eines benutzerdefinierten Images</span><span class="sxs-lookup"><span data-stu-id="78b41-292">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="78b41-293">Befehlszeilenoption zum Angeben des Cachetyps für NFS mit Verwaltung per Batch AI hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-293">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="78b41-294">Angeben der Bereitstellung von Dateisystemen in Konfigurationsdateien vereinfacht.</span><span class="sxs-lookup"><span data-stu-id="78b41-294">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="78b41-295">Weglassen von Anmeldeinformationen für Azure-Dateifreigaben und Azure-Blobcontainer ist jetzt möglich. Die CLI füllt fehlende Anmeldeinformationen auf, indem der Speicherkontoschlüssel verwendet wird, der über Befehlszeilenparameter oder per Umgebungsvariable angegeben wird, oder der Schlüssel wird über Azure Storage abgefragt (sofern das Speicherkonto zum aktuellen Abonnement gehört).</span><span class="sxs-lookup"><span data-stu-id="78b41-295">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="78b41-296">Der Befehl zum Streamen von Auftragsdateien wird jetzt automatisch abgeschlossen, nachdem der Auftrag beendet ist (Erfolg, Fehler, Beendigung oder Löschung)</span><span class="sxs-lookup"><span data-stu-id="78b41-296">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="78b41-297">Verbesserte `table`-Ausgabe für `show`-Vorgänge</span><span class="sxs-lookup"><span data-stu-id="78b41-297">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="78b41-298">Option `--use-auto-storage` für die Clustererstellung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="78b41-298">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="78b41-299">Diese Option erleichtert die Verwaltung von Speicherkonten und die Bereitstellung von Azure-Dateifreigaben und Azure-Blobcontainern in Clustern.</span><span class="sxs-lookup"><span data-stu-id="78b41-299">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="78b41-300">`--generate-ssh-keys` für `cluster create` und `file-server create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-300">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="78b41-301">Möglichkeit zum Angeben der Knotensetupaufgabe über die Befehlszeile</span><span class="sxs-lookup"><span data-stu-id="78b41-301">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="78b41-302">[WICHTIGE ÄNDERUNG] Befehl `job stream-file` und `job list-files` in die Gruppe `job file` verschoben</span><span class="sxs-lookup"><span data-stu-id="78b41-302">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="78b41-303">[WICHTIGE ÄNDERUNG] `--admin-user-name` im Befehl `file-server create` in `--user-name` umbenannt, um Einheitlichkeit mit dem Befehl `cluster create` zu erzielen</span><span class="sxs-lookup"><span data-stu-id="78b41-303">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="78b41-304">Abrechnung</span><span class="sxs-lookup"><span data-stu-id="78b41-304">Billing</span></span>

* <span data-ttu-id="78b41-305">Registrierungskontobefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-305">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="78b41-306">Nutzung</span><span class="sxs-lookup"><span data-stu-id="78b41-306">Consumption</span></span>

* <span data-ttu-id="78b41-307">Befehle vom Typ `marketplace` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-307">Added `marketplace` commands</span></span>
* <span data-ttu-id="78b41-308">[WICHTIGE ÄNDERUNG] `reservations summaries` in `reservation summary` umbenannt</span><span class="sxs-lookup"><span data-stu-id="78b41-308">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="78b41-309">[WICHTIGE ÄNDERUNG] `reservations details` in `reservation detail` umbenannt</span><span class="sxs-lookup"><span data-stu-id="78b41-309">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="78b41-310">[WICHTIGE ÄNDERUNG] Kurzoptionen `--reservation-order-id` und `--reservation-id` für `reservation`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="78b41-310">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="78b41-311">[WICHTIGE ÄNDERUNG] `--grain`-Kurzoptionen für `reservation summary`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="78b41-311">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="78b41-312">[WICHTIGE ÄNDERUNG] `--include-meter-details`-Kurzoptionen für `pricesheet`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="78b41-312">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="78b41-313">Container</span><span class="sxs-lookup"><span data-stu-id="78b41-313">Container</span></span>

* <span data-ttu-id="78b41-314">Git-Repository-Parameter `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` und `--gitrepo-mount-path` für die Volumebereitstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-314">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="78b41-315">[#5926](https://github.com/Azure/azure-cli/issues/5926) behoben: Fehler bei `az container exec`, wenn „--container-name“ angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="78b41-315">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="78b41-316">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="78b41-316">Extension</span></span>

* <span data-ttu-id="78b41-317">Meldung für Distributionsüberprüfung in Debugebene geändert</span><span class="sxs-lookup"><span data-stu-id="78b41-317">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="78b41-318">Interactive</span><span class="sxs-lookup"><span data-stu-id="78b41-318">Interactive</span></span>

* <span data-ttu-id="78b41-319">Geändert: Verhinderung des Abschlusses bei nicht erkannten Befehlen</span><span class="sxs-lookup"><span data-stu-id="78b41-319">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="78b41-320">Ereignishooks vor und nach der Erstellung der Teilstruktur von Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-320">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="78b41-321">Abschluss für `--ids`-Parameter hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-321">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="78b41-322">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="78b41-322">Network</span></span>

* <span data-ttu-id="78b41-323">[#5936](https://github.com/Azure/azure-cli/issues/5936) behoben: `application-gateway create`-Tags konnten nicht festgelegt werden</span><span class="sxs-lookup"><span data-stu-id="78b41-323">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="78b41-324">Argument `--auth-certs` zum Anfügen von Authentifizierungszertifikaten für `application-gateway http-settings [create|update]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="78b41-324">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="78b41-325">#4910</span><span class="sxs-lookup"><span data-stu-id="78b41-325">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="78b41-326">`ddos-protection`-Befehle zum Erstellen von DDoS-Schutzplänen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-326">Added `ddos-protection` commands to create DDoS protection plans</span></span> 
* <span data-ttu-id="78b41-327">Unterstützung von `--ddos-protection-plan` für `vnet [create|update]` hinzugefügt, um das Zuordnen eines VNET zu einem DDoS-Schutzplan zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="78b41-327">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="78b41-328">Problem mit `--disable-bgp-route-propagation`-Flag in `network route-table [create|update]` behoben</span><span class="sxs-lookup"><span data-stu-id="78b41-328">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="78b41-329">Dummy-Argumente `--public-ip-address-type` und `--subnet-type` für `network lb [create|update]` entfernt</span><span class="sxs-lookup"><span data-stu-id="78b41-329">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="78b41-330">Unterstützung für TXT-Datensätze mit RFC 1035-Escapesequenzen für `network dns zone [import|export]` und `network dns record-set txt add-record` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-330">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="78b41-331">Profil</span><span class="sxs-lookup"><span data-stu-id="78b41-331">Profile</span></span>

* <span data-ttu-id="78b41-332">Unterstützung für klassische Azure-Konten in `account list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-332">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="78b41-333">[WICHTIGE ÄNDERUNG] `--msi` & `--msi-port`-Argumente entfernt</span><span class="sxs-lookup"><span data-stu-id="78b41-333">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="78b41-334">RDBMS</span><span class="sxs-lookup"><span data-stu-id="78b41-334">RDBMS</span></span>

* <span data-ttu-id="78b41-335">Befehl `georestore` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-335">Added `georestore` command</span></span>
* <span data-ttu-id="78b41-336">Speichergrößenbeschränkung aus Befehl `create` entfernt</span><span class="sxs-lookup"><span data-stu-id="78b41-336">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="78b41-337">Ressource</span><span class="sxs-lookup"><span data-stu-id="78b41-337">Resource</span></span>

* <span data-ttu-id="78b41-338">Unterstützung für `--metadata` zu `policy definition create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-338">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="78b41-339">Unterstützung von `--metadata`, `--set`, `--add`, `--remove` für `policy definition update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-339">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="78b41-340">SQL</span><span class="sxs-lookup"><span data-stu-id="78b41-340">SQL</span></span>

* <span data-ttu-id="78b41-341">`sql elastic-pool op list` und `sql elastic-pool op cancel` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-341">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="78b41-342">Speicher</span><span class="sxs-lookup"><span data-stu-id="78b41-342">Storage</span></span>

* <span data-ttu-id="78b41-343">Fehlermeldungen für falsch formatierte Verbindungszeichenfolgen verbessert</span><span class="sxs-lookup"><span data-stu-id="78b41-343">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="78b41-344">VM</span><span class="sxs-lookup"><span data-stu-id="78b41-344">VM</span></span>

* <span data-ttu-id="78b41-345">Unterstützung für die Konfiguration der Plattform-Fehlerdomänenanzahl für `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-345">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="78b41-346">`vmss create` geändert, damit standardmäßig „Standard LB“ für zonales, großes oder per einzelner Platzierungsgruppe deaktiviertes Scale Set festgelegt wird</span><span class="sxs-lookup"><span data-stu-id="78b41-346">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [WICHTIGE ÄNDERUNG]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="78b41-348">Unterstützung für SKU mit öffentlicher IP für `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-348">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="78b41-349">Argumente `--keyvault` und `--resource-group` für `vm secret format` hinzugefügt, um Szenarien zu unterstützen, bei denen der Befehl die Tresor-ID nicht auflösen kann.</span><span class="sxs-lookup"><span data-stu-id="78b41-349">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="78b41-350">#5718</span><span class="sxs-lookup"><span data-stu-id="78b41-350">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="78b41-351">Bessere Fehler für `[vm|vmss create]`, wenn der Standort einer Ressourcengruppe keine Zonenunterstützung aufweist</span><span class="sxs-lookup"><span data-stu-id="78b41-351">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="78b41-352">27. März 2018</span><span class="sxs-lookup"><span data-stu-id="78b41-352">March 27, 2018</span></span>

<span data-ttu-id="78b41-353">Version 2.0.30</span><span class="sxs-lookup"><span data-stu-id="78b41-353">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="78b41-354">Core</span><span class="sxs-lookup"><span data-stu-id="78b41-354">Core</span></span>

* <span data-ttu-id="78b41-355">Anzeigen einer Meldung für Erweiterungen, die in der Hilfe als Vorschauversion gekennzeichnet sind</span><span class="sxs-lookup"><span data-stu-id="78b41-355">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="78b41-356">ACS</span><span class="sxs-lookup"><span data-stu-id="78b41-356">ACS</span></span>

* <span data-ttu-id="78b41-357">Behebung eines Fehlers bei der SSL-Zertifikatprüfung für `aks install-cli` in Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="78b41-357">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="78b41-358">AppService</span><span class="sxs-lookup"><span data-stu-id="78b41-358">Appservice</span></span>

* <span data-ttu-id="78b41-359">Unterstützung nur von HTTPS zu `webapp update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-359">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="78b41-360">Unterstützung für Slots zu `az webapp identity [assign|show]` und `az functionapp identity [assign|show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-360">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="78b41-361">Backup</span><span class="sxs-lookup"><span data-stu-id="78b41-361">Backup</span></span>

* <span data-ttu-id="78b41-362">Neuer Befehl `az backup protection isenabled-for-vm` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="78b41-362">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="78b41-363">Mit diesem Befehl kann überprüft werden, ob ein virtueller Computer von einem beliebigen Tresor im Abonnement gesichert wird.</span><span class="sxs-lookup"><span data-stu-id="78b41-363">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="78b41-364">Azure-Objekt-IDs für Parameter `--resource-group` und `--vault-name` für die folgenden Befehle aktiviert:</span><span class="sxs-lookup"><span data-stu-id="78b41-364">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="78b41-365">`--name`-Parameter wurden geändert, um das Ausgabeformat von `backup ... show`-Befehlen zu akzeptieren.</span><span class="sxs-lookup"><span data-stu-id="78b41-365">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="78b41-366">Container</span><span class="sxs-lookup"><span data-stu-id="78b41-366">Container</span></span>

* <span data-ttu-id="78b41-367">Befehl `container exec` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="78b41-367">Added `container exec` command.</span></span> <span data-ttu-id="78b41-368">Ausführung von Befehlen in einem Container für eine ausgeführte Containergruppe</span><span class="sxs-lookup"><span data-stu-id="78b41-368">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="78b41-369">Zulassen der Tabellenausgabe zum Erstellen und Aktualisieren einer Containergruppe</span><span class="sxs-lookup"><span data-stu-id="78b41-369">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="78b41-370">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="78b41-370">Extension</span></span>

* <span data-ttu-id="78b41-371">Meldung für `extension add` hinzugefügt, wenn sich die Erweiterung in der Vorschauphase befindet</span><span class="sxs-lookup"><span data-stu-id="78b41-371">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="78b41-372">`extension list-available` geändert, um vollständige Erweiterungsdaten mit `--show-details` anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="78b41-372">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="78b41-373">[WICHTIGE ÄNDERUNG] `extension list-available` geändert, um standardmäßig vereinfachte Erweiterungsdaten anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="78b41-373">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="78b41-374">Interactive</span><span class="sxs-lookup"><span data-stu-id="78b41-374">Interactive</span></span>

* <span data-ttu-id="78b41-375">Vervollständigungen wurden geändert und werden jetzt aktiviert, sobald das Laden der Befehlstabelle abgeschlossen ist.</span><span class="sxs-lookup"><span data-stu-id="78b41-375">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="78b41-376">Fehler bei der Verwendung des Parameters `--style` behoben</span><span class="sxs-lookup"><span data-stu-id="78b41-376">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="78b41-377">Interaktiver Lexer nach Befehlstabellensicherung instanziiert (sofern nicht vorhanden)</span><span class="sxs-lookup"><span data-stu-id="78b41-377">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="78b41-378">Verbesserte Unterstützung der Vervollständigung</span><span class="sxs-lookup"><span data-stu-id="78b41-378">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="78b41-379">Labor</span><span class="sxs-lookup"><span data-stu-id="78b41-379">Lab</span></span>

* <span data-ttu-id="78b41-380">Probleme mit Befehl `create environment` behoben</span><span class="sxs-lookup"><span data-stu-id="78b41-380">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="78b41-381">Überwachen</span><span class="sxs-lookup"><span data-stu-id="78b41-381">Monitor</span></span>

* <span data-ttu-id="78b41-382">Unterstützung für `--top`, `--orderby` und `--namespace` zu `metrics list` hinzugefügt ([#5785](https://github.com/Azure/azure-cli/issues/5785))</span><span class="sxs-lookup"><span data-stu-id="78b41-382">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="78b41-383">[#4529](https://github.com/Azure/azure-cli/issues/5785) behoben: `metrics list` akzeptiert eine durch Leerzeichen getrennte Liste von abzurufenden Metriken.</span><span class="sxs-lookup"><span data-stu-id="78b41-383">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="78b41-384">Unterstützung für `--namespace` zu `metrics list-definitions` hinzugefügt ([#5785](https://github.com/Azure/azure-cli/issues/5785))</span><span class="sxs-lookup"><span data-stu-id="78b41-384">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="78b41-385">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="78b41-385">Network</span></span>

* <span data-ttu-id="78b41-386">Unterstützung für private DNS-Zonen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-386">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="78b41-387">Profil</span><span class="sxs-lookup"><span data-stu-id="78b41-387">Profile</span></span>

* <span data-ttu-id="78b41-388">Warnung für `--identity-port` und `--msi-port` zu `login` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-388">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="78b41-389">RDBMS</span><span class="sxs-lookup"><span data-stu-id="78b41-389">RDBMS</span></span>

* <span data-ttu-id="78b41-390">GA-API-Version 2017-12-01 (Geschäftsmodell) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-390">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="78b41-391">Ressource</span><span class="sxs-lookup"><span data-stu-id="78b41-391">Resource</span></span>

* [WICHTIGE ÄNDERUNG]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="78b41-393">Rolle</span><span class="sxs-lookup"><span data-stu-id="78b41-393">Role</span></span>

* <span data-ttu-id="78b41-394">Unterstützung für erforderliche Zugriffskonfigurationen und native Clients zu `az ad app create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-394">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="78b41-395">`rbac`-Befehle geändert, um maximal 1.000 IDs für Objektauflösung zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="78b41-395">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="78b41-396">Befehle zur Verwaltung von Anmeldeinformationen (`ad sp credential [reset|list|delete]`) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-396">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="78b41-397">[WICHTIGE ÄNDERUNG] „properties“ aus `az role assignment [list|show]`-Ausgabe entfernt</span><span class="sxs-lookup"><span data-stu-id="78b41-397">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="78b41-398">Unterstützung für `dataActions`- und `notDataActions`-Berechtigungen zu `role definition` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-398">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="78b41-399">Speicher</span><span class="sxs-lookup"><span data-stu-id="78b41-399">Storage</span></span>

* <span data-ttu-id="78b41-400">Problem beim Hochladen von Dateien mit einer Größe von 195 GB bis 200 GB behoben</span><span class="sxs-lookup"><span data-stu-id="78b41-400">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="78b41-401">[#4049](https://github.com/Azure/azure-cli/issues/4049) behoben: Probleme bei Uploads von Anfügeblobs behoben, die ein Ignorieren der Bedingungsparameter verursachten</span><span class="sxs-lookup"><span data-stu-id="78b41-401">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="78b41-402">VM</span><span class="sxs-lookup"><span data-stu-id="78b41-402">VM</span></span>

* <span data-ttu-id="78b41-403">Warnung für anstehende wichtige Änderungen für Sätze mit mehr als 100 Instanzen zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-403">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="78b41-404">Unterstützung der Zonenresilienz zu `vm [snapshot|image]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-404">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="78b41-405">Datenträgerinstanzansicht geändert, um besseren Verschlüsselungsstatus zu melden</span><span class="sxs-lookup"><span data-stu-id="78b41-405">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="78b41-406">[WICHTIGE ÄNDERUNG] `vm extension delete` geändert, um keine Ausgabe mehr zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="78b41-406">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="78b41-407">13. März 2018</span><span class="sxs-lookup"><span data-stu-id="78b41-407">March 13, 2018</span></span>

<span data-ttu-id="78b41-408">Version 2.0.29</span><span class="sxs-lookup"><span data-stu-id="78b41-408">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="78b41-409">ACR</span><span class="sxs-lookup"><span data-stu-id="78b41-409">ACR</span></span>

* <span data-ttu-id="78b41-410">Unterstützung für den Parameter `--image` zu `repository delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-410">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="78b41-411">Parameter `--manifest` und `--tag` des Befehls `repository delete` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="78b41-411">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="78b41-412">Befehl `repository untag` zum Entfernen eines Tags ohne das Löschen von Daten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-412">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="78b41-413">ACS</span><span class="sxs-lookup"><span data-stu-id="78b41-413">ACS</span></span>

* <span data-ttu-id="78b41-414">Befehl `aks upgrade-connector` zum Aktualisieren eines vorhandenen Connectors hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-414">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="78b41-415">`kubectl`-Konfigurationsdateien zur Verwendung von besser lesbarem YAML im Blockstil geändert</span><span class="sxs-lookup"><span data-stu-id="78b41-415">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="78b41-416">Advisor</span><span class="sxs-lookup"><span data-stu-id="78b41-416">Advisor</span></span>

* <span data-ttu-id="78b41-417">[WICHTIGE ÄNDERUNG] `advisor configuration get` in `advisor configuration list` umbenannt</span><span class="sxs-lookup"><span data-stu-id="78b41-417">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="78b41-418">[WICHTIGE ÄNDERUNG] `advisor configuration set` in `advisor configuration update` umbenannt</span><span class="sxs-lookup"><span data-stu-id="78b41-418">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="78b41-419">[WICHTIGE ÄNDERUNG] `advisor recommendation generate` entfernt</span><span class="sxs-lookup"><span data-stu-id="78b41-419">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span> 
* <span data-ttu-id="78b41-420">Parameter `--refresh` zu `advisor recommendation list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-420">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="78b41-421">Befehl `advisor recommendation show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-421">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="78b41-422">AppService</span><span class="sxs-lookup"><span data-stu-id="78b41-422">Appservice</span></span>

* <span data-ttu-id="78b41-423">`[webapp|functionapp] assign-identity` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="78b41-423">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="78b41-424">Befehle `webapp identity [assign|show]` und `functionapp identity [assign|show]` für verwaltete Identität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-424">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="78b41-425">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="78b41-425">Eventhubs</span></span>

* <span data-ttu-id="78b41-426">Erste Version</span><span class="sxs-lookup"><span data-stu-id="78b41-426">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="78b41-427">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="78b41-427">Extension</span></span>

* <span data-ttu-id="78b41-428">Überprüfung zum Warnen von Benutzern hinzugefügt, wenn sich die verwendete Distribution von der in der Paketquelldatei gespeicherten Distribution unterscheidet, da dies Fehlern führen kann</span><span class="sxs-lookup"><span data-stu-id="78b41-428">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="78b41-429">Interactive</span><span class="sxs-lookup"><span data-stu-id="78b41-429">Interactive</span></span>

* <span data-ttu-id="78b41-430">[#5625](https://github.com/Azure/azure-cli/issues/5625) behoben: Verlauf über verschiedene Sitzungen hinweg beibehalten</span><span class="sxs-lookup"><span data-stu-id="78b41-430">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="78b41-431">[#3016](https://github.com/Azure/azure-cli/issues/3016) behoben: Verlauf nicht aufgezeichnet, obwohl er innerhalb des Bereichs liegt</span><span class="sxs-lookup"><span data-stu-id="78b41-431">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="78b41-432">[#5688](https://github.com/Azure/azure-cli/issues/5688) behoben: Abschlüsse nicht angezeigt, wenn beim Laden der Befehlstabelle Ausnahme auftrat</span><span class="sxs-lookup"><span data-stu-id="78b41-432">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="78b41-433">Statusanzeige für lang ausgeführte Vorgänge korrigiert</span><span class="sxs-lookup"><span data-stu-id="78b41-433">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="78b41-434">Überwachen</span><span class="sxs-lookup"><span data-stu-id="78b41-434">Monitor</span></span>

* <span data-ttu-id="78b41-435">`monitor autoscale-settings`-Befehle als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="78b41-435">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="78b41-436">Befehle vom Typ `monitor autoscale` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-436">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="78b41-437">Befehle vom Typ `monitor autoscale profile` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-437">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="78b41-438">Befehle vom Typ `monitor autoscale rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-438">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="78b41-439">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="78b41-439">Network</span></span>

* <span data-ttu-id="78b41-440">[WICHTIGE ÄNDERUNG] Parameter `--tags` aus `route-filter rule create` entfernt</span><span class="sxs-lookup"><span data-stu-id="78b41-440">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="78b41-441">Einige fehlerhafte Standardwerte für die folgenden Befehle entfernt:</span><span class="sxs-lookup"><span data-stu-id="78b41-441">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="78b41-442">`network watcher connection-monitor`-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-442">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="78b41-443">Parameter `--vnet` und `--subnet` zu `network watcher show-topology` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-443">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="78b41-444">Profil</span><span class="sxs-lookup"><span data-stu-id="78b41-444">Profile</span></span>

* <span data-ttu-id="78b41-445">Parameter `--msi` für `az login` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="78b41-445">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="78b41-446">Parameter `--identity` für `az login` als Ersatz vor `--msi` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-446">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="78b41-447">RDBMS</span><span class="sxs-lookup"><span data-stu-id="78b41-447">RDBMS</span></span>

* <span data-ttu-id="78b41-448">[VORSCHAU] Geändert, sodass die API „2017-12-01-preview“ verwendet wird</span><span class="sxs-lookup"><span data-stu-id="78b41-448">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="78b41-449">Service Bus</span><span class="sxs-lookup"><span data-stu-id="78b41-449">Service Bus</span></span>

* <span data-ttu-id="78b41-450">Erste Version</span><span class="sxs-lookup"><span data-stu-id="78b41-450">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="78b41-451">Speicher</span><span class="sxs-lookup"><span data-stu-id="78b41-451">Storage</span></span>

* <span data-ttu-id="78b41-452">[#4971](https://github.com/Azure/azure-cli/issues/4971) behoben: `storage blob copy` unterstützt jetzt andere Azure-Clouds.</span><span class="sxs-lookup"><span data-stu-id="78b41-452">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="78b41-453">[#5286](https://github.com/Azure/azure-cli/issues/5286) behoben: `storage blob [delete-batch|download-batch|upload-batch]`-Batchbefehle lösen bei Vorbedingungsfehlern keinen Fehler mehr aus.</span><span class="sxs-lookup"><span data-stu-id="78b41-453">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="78b41-454">VM</span><span class="sxs-lookup"><span data-stu-id="78b41-454">VM</span></span>

* <span data-ttu-id="78b41-455">`[vm|vmss] create` unterstützt jetzt das Anfügen nicht verwalteter Datenträger und das Konfigurieren der Zwischenspeicherung.</span><span class="sxs-lookup"><span data-stu-id="78b41-455">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="78b41-456">`[vm|vmss] assign-identity` und `[vm|vmss] remove-identity` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="78b41-456">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="78b41-457">Befehle `vm identity [assign|remove|show]` und `vmss identity [assign|remove|show]` als Ersatz für veraltete Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-457">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="78b41-458">Standardpriorität in `vmss create` auf „Keine“ geändert</span><span class="sxs-lookup"><span data-stu-id="78b41-458">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="78b41-459">27. Februar 2018</span><span class="sxs-lookup"><span data-stu-id="78b41-459">February 27, 2018</span></span>

<span data-ttu-id="78b41-460">Version 2.0.28</span><span class="sxs-lookup"><span data-stu-id="78b41-460">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="78b41-461">Core</span><span class="sxs-lookup"><span data-stu-id="78b41-461">Core</span></span>

* <span data-ttu-id="78b41-462">[5184](https://github.com/Azure/azure-cli/issues/5184) (Problem beim Installieren von Homebrew) behoben</span><span class="sxs-lookup"><span data-stu-id="78b41-462">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="78b41-463">Unterstützung für Erweiterungstelemetrie mit benutzerdefinierten Schlüsseln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-463">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="78b41-464">HTTP-Protokollierung zu `--debug` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-464">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="78b41-465">ACS</span><span class="sxs-lookup"><span data-stu-id="78b41-465">ACS</span></span>

* <span data-ttu-id="78b41-466">Geändert, sodass für `aks install-connector` standardmäßig das Helm-Diagramm `virtual-kubelet-for-aks` verwendet wird</span><span class="sxs-lookup"><span data-stu-id="78b41-466">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="78b41-467">Problem behoben: Unzureichende Berechtigungen für Dienstprinzipale zum Erstellen einer ACI-Containergruppe</span><span class="sxs-lookup"><span data-stu-id="78b41-467">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="78b41-468">Parameter `--aci-container-group`, `--location` und `--image-tag` zu `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-468">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="78b41-469">Veraltungshinweis aus `aks get-versions` entfernt</span><span class="sxs-lookup"><span data-stu-id="78b41-469">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="78b41-470">AppService</span><span class="sxs-lookup"><span data-stu-id="78b41-470">Appservice</span></span>

* <span data-ttu-id="78b41-471">Updates für die neue SDK-Version (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="78b41-471">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="78b41-472">[5538](https://github.com/Azure/azure-cli/issues/5538) behoben: `Free` wurde als ungültige SKU gemeldet.</span><span class="sxs-lookup"><span data-stu-id="78b41-472">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="78b41-473">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="78b41-473">Cognitive Services</span></span>

* <span data-ttu-id="78b41-474">Hinweis beim Erstellen eines neuen Cognitive Services-Kontos aktualisiert</span><span class="sxs-lookup"><span data-stu-id="78b41-474">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="78b41-475">Nutzung</span><span class="sxs-lookup"><span data-stu-id="78b41-475">Consumption</span></span>

* <span data-ttu-id="78b41-476">Neue Befehle für PriceSheet-API hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-476">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="78b41-477">Vorhandene Formate für Nutzungsdetails und Reservierungsdetails aktualisiert</span><span class="sxs-lookup"><span data-stu-id="78b41-477">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="78b41-478">Container</span><span class="sxs-lookup"><span data-stu-id="78b41-478">Container</span></span>

* <span data-ttu-id="78b41-479">Argumente `--secrets` und `--secrets-mount-path` zu `container create` hinzugefügt, um Geheimnisse in ACI verwenden zu können</span><span class="sxs-lookup"><span data-stu-id="78b41-479">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="78b41-480">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="78b41-480">Network</span></span>

* <span data-ttu-id="78b41-481">[5559](https://github.com/Azure/azure-cli/issues/5559) behoben: Fehlender Client in `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="78b41-481">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="78b41-482">Ressource</span><span class="sxs-lookup"><span data-stu-id="78b41-482">Resource</span></span>

* <span data-ttu-id="78b41-483">`group deployment export` geändert, um eine partielle Vorlage und ggf. Fehler anzuzeigen, wenn der Vorgang nicht erfolgreich war</span><span class="sxs-lookup"><span data-stu-id="78b41-483">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="78b41-484">Rolle</span><span class="sxs-lookup"><span data-stu-id="78b41-484">Role</span></span>

* <span data-ttu-id="78b41-485">`role assignment list-changelogs` hinzugefügt, um die Überprüfung von Dienstprinzipalrollen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="78b41-485">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="78b41-486">SQL</span><span class="sxs-lookup"><span data-stu-id="78b41-486">SQL</span></span>

* <span data-ttu-id="78b41-487">Zonenredundanzunterstützung für Datenbanken und Pools für elastische Datenbanken hinzugefügt (bei Erstellung und Aktualisierung)</span><span class="sxs-lookup"><span data-stu-id="78b41-487">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="78b41-488">Speicher</span><span class="sxs-lookup"><span data-stu-id="78b41-488">Storage</span></span>

* <span data-ttu-id="78b41-489">Angabe von Zielpfad/Präfix für `storage blob [upload-batch|download-batch]` ermöglicht</span><span class="sxs-lookup"><span data-stu-id="78b41-489">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="78b41-490">VM</span><span class="sxs-lookup"><span data-stu-id="78b41-490">VM</span></span>

* <span data-ttu-id="78b41-491">Unterstützung für das Anfügen/Trennen von Datenträgern für eine einzelne VMSS-Instanz hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-491">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="78b41-492">13. Februar 2018</span><span class="sxs-lookup"><span data-stu-id="78b41-492">February 13, 2018</span></span>

<span data-ttu-id="78b41-493">Version 2.0.27</span><span class="sxs-lookup"><span data-stu-id="78b41-493">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="78b41-494">Core</span><span class="sxs-lookup"><span data-stu-id="78b41-494">Core</span></span>

* <span data-ttu-id="78b41-495">Authentifizierung für Abonnement-ID und Namen bei der MSI-Anmeldung in Authentifizierung mit Schlüssel geändert</span><span class="sxs-lookup"><span data-stu-id="78b41-495">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="78b41-496">ACS</span><span class="sxs-lookup"><span data-stu-id="78b41-496">ACS</span></span>

* <span data-ttu-id="78b41-497">[WICHTIGE ÄNDERUNG] `aks get-versions` aus Gründen der Genauigkeit in `aks get-upgrades` umbenannt</span><span class="sxs-lookup"><span data-stu-id="78b41-497">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="78b41-498">`aks get-versions` zur Anzeige der verfügbaren Kubernetes-Versionen für `aks create` geändert</span><span class="sxs-lookup"><span data-stu-id="78b41-498">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="78b41-499">Standardwerte von `aks create` in Auswahl der Kubernetes-Version durch den Server geändert</span><span class="sxs-lookup"><span data-stu-id="78b41-499">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="78b41-500">Hilfemeldungen zu dem von AKS generierten Dienstprinzipal aktualisiert</span><span class="sxs-lookup"><span data-stu-id="78b41-500">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="78b41-501">Standardknotengrößen für `aks create` von „Standard\_D1\_v2“ in „Standard\_DS1\_v2“ geändert</span><span class="sxs-lookup"><span data-stu-id="78b41-501">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="78b41-502">Zuverlässigkeit der Suche nach dem Dashboardpod für `az aks browse` verbessert</span><span class="sxs-lookup"><span data-stu-id="78b41-502">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="78b41-503">`aks get-credentials` korrigiert, um Unicode-Fehler beim Laden von Kubernetes-Konfigurationsdateien zu behandeln</span><span class="sxs-lookup"><span data-stu-id="78b41-503">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="78b41-504">Meldung zu `az aks install-cli` hinzugefügt, um das Abrufen von `kubectl` in `$PATH` zu erleichtern</span><span class="sxs-lookup"><span data-stu-id="78b41-504">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="78b41-505">AppService</span><span class="sxs-lookup"><span data-stu-id="78b41-505">Appservice</span></span>

* <span data-ttu-id="78b41-506">Problem behoben, das zu einem Fehler von `webapp [backup|restore]` aufgrund eines Nullverweises führte</span><span class="sxs-lookup"><span data-stu-id="78b41-506">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="78b41-507">Unterstützung für Standard-App Service-Pläne durch `az configure --defaults appserviceplan=my-asp` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-507">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="78b41-508">CDN</span><span class="sxs-lookup"><span data-stu-id="78b41-508">CDN</span></span>

* <span data-ttu-id="78b41-509">Befehle vom Typ `cdn custom-domain [enable-https|disable-https]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-509">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="78b41-510">Container</span><span class="sxs-lookup"><span data-stu-id="78b41-510">Container</span></span>

* <span data-ttu-id="78b41-511">Option `--follow` zu `az container logs` für Streamingprotokolle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-511">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="78b41-512">Befehl `container attach` hinzugefügt, der die lokale Standardausgabe und Fehlerdatenströme an einen Container in einer Containergruppe angefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-512">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="78b41-513">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="78b41-513">CosmosDB</span></span>

* <span data-ttu-id="78b41-514">Unterstützung für Einstellungsfunktionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-514">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="78b41-515">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="78b41-515">Extension</span></span>

* <span data-ttu-id="78b41-516">Unterstützung für den Parameter `--pip-proxy` zu Befehlen vom Typ `az extension [add|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-516">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="78b41-517">Unterstützung für das Argument `--pip-extra-index-urls` zu Befehlen vom Typ `az extension [add|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-517">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="78b41-518">Feedback</span><span class="sxs-lookup"><span data-stu-id="78b41-518">Feedback</span></span>

* <span data-ttu-id="78b41-519">Erweiterungsinformationen zu Telemetriedaten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-519">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="78b41-520">Interactive</span><span class="sxs-lookup"><span data-stu-id="78b41-520">Interactive</span></span>

* <span data-ttu-id="78b41-521">Problem behoben, aufgrund dessen der Benutzer bei Verwendung des interaktiven Modus in Cloud Shell zur Anmeldung aufgefordert wird</span><span class="sxs-lookup"><span data-stu-id="78b41-521">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="78b41-522">Regression mit fehlenden Parametervervollständigungen korrigiert</span><span class="sxs-lookup"><span data-stu-id="78b41-522">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="78b41-523">IoT</span><span class="sxs-lookup"><span data-stu-id="78b41-523">IoT</span></span>

* <span data-ttu-id="78b41-524">Problem behoben, aufgrund dessen `iot dps access policy [create|update]` bei erfolgreicher Ausführung einen Fehler „nicht gefunden“ zurückgibt</span><span class="sxs-lookup"><span data-stu-id="78b41-524">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="78b41-525">Problem behoben, aufgrund dessen `iot dps linked-hub [create|update]` bei erfolgreicher Ausführung einen Fehler „nicht gefunden“ zurückgibt</span><span class="sxs-lookup"><span data-stu-id="78b41-525">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="78b41-526">Unterstützung für `--no-wait` zu `iot dps access policy [create|update]` und `iot dps linked-hub [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-526">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="78b41-527">`iot hub create` geändert, um die Angabe der Anzahl von Partitionen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="78b41-527">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="78b41-528">Überwachen</span><span class="sxs-lookup"><span data-stu-id="78b41-528">Monitor</span></span>

* <span data-ttu-id="78b41-529">Befehl `az monitor log-profiles create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="78b41-529">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="78b41-530">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="78b41-530">Network</span></span>

* <span data-ttu-id="78b41-531">Option `--tags` für folgende Befehle korrigiert:</span><span class="sxs-lookup"><span data-stu-id="78b41-531">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="78b41-532">Profil</span><span class="sxs-lookup"><span data-stu-id="78b41-532">Profile</span></span>

* <span data-ttu-id="78b41-533">`az login` im interaktiven Modus aktiviert</span><span class="sxs-lookup"><span data-stu-id="78b41-533">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="78b41-534">Ressource</span><span class="sxs-lookup"><span data-stu-id="78b41-534">Resource</span></span>

* <span data-ttu-id="78b41-535">`feature show` wieder hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-535">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="78b41-536">Rolle</span><span class="sxs-lookup"><span data-stu-id="78b41-536">Role</span></span>

* <span data-ttu-id="78b41-537">Argument `--available-to-other-tenants` zu `ad app update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-537">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="78b41-538">SQL</span><span class="sxs-lookup"><span data-stu-id="78b41-538">SQL</span></span>

* <span data-ttu-id="78b41-539">Befehle vom Typ `sql server dns-alias` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-539">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="78b41-540">`sql db rename` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-540">Added `sql db rename`</span></span>
* <span data-ttu-id="78b41-541">Unterstützung für das Argument `--ids` für alle SQL-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-541">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="78b41-542">Speicher</span><span class="sxs-lookup"><span data-stu-id="78b41-542">Storage</span></span>

* <span data-ttu-id="78b41-543">Befehle `storage blob service-properties delete-policy` und `storage blob undelete` hinzugefügt, um vorläufiges Löschen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="78b41-543">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="78b41-544">VM</span><span class="sxs-lookup"><span data-stu-id="78b41-544">VM</span></span>

* <span data-ttu-id="78b41-545">Absturz bei unvollständiger Initialisierung der VM-Verschlüsselung behoben</span><span class="sxs-lookup"><span data-stu-id="78b41-545">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="78b41-546">Prinzipal-ID-Ausgabe beim Aktivieren von MSI hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-546">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="78b41-547">`vm boot-diagnostics get-boot-log` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="78b41-547">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="78b41-548">31. Januar 2018</span><span class="sxs-lookup"><span data-stu-id="78b41-548">January 31, 2018</span></span>

<span data-ttu-id="78b41-549">Version 2.0.26</span><span class="sxs-lookup"><span data-stu-id="78b41-549">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="78b41-550">Core</span><span class="sxs-lookup"><span data-stu-id="78b41-550">Core</span></span>

* <span data-ttu-id="78b41-551">Unterstützung für das Abrufen von unformatierten Token im MSI-Kontext hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-551">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="78b41-552">Abrufindikator-Zeichenfolge nach Fertigstellung von LRO für die Windows-Datei „cmd.exe“ entfernt</span><span class="sxs-lookup"><span data-stu-id="78b41-552">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="78b41-553">Warnung hinzugefügt, die angezeigt wird, wenn ein konfigurierter Standardwert in einen Eintrag auf INFO-Ebene geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="78b41-553">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="78b41-554">`--verbose` zum Anzeigen verwenden.</span><span class="sxs-lookup"><span data-stu-id="78b41-554">Use `--verbose` to see</span></span>
* <span data-ttu-id="78b41-555">Statusanzeige für Wait-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-555">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="78b41-556">ACS</span><span class="sxs-lookup"><span data-stu-id="78b41-556">ACS</span></span>

* <span data-ttu-id="78b41-557">Argument `--disable-browser` erläutert</span><span class="sxs-lookup"><span data-stu-id="78b41-557">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="78b41-558">Vervollständigung mit der TAB-TASTE für Argumente vom Typ `--vm-size` verbessert</span><span class="sxs-lookup"><span data-stu-id="78b41-558">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="78b41-559">AppService</span><span class="sxs-lookup"><span data-stu-id="78b41-559">Appservice</span></span>

* <span data-ttu-id="78b41-560">`webapp log [tail|download]` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="78b41-560">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="78b41-561">Überprüfung `kind` für Web-Apps und Funktionen entfernt</span><span class="sxs-lookup"><span data-stu-id="78b41-561">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="78b41-562">CDN</span><span class="sxs-lookup"><span data-stu-id="78b41-562">CDN</span></span>

* <span data-ttu-id="78b41-563">Problem mit fehlendem Client für `cdn custom-domain create` behoben</span><span class="sxs-lookup"><span data-stu-id="78b41-563">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="78b41-564">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="78b41-564">CosmosDB</span></span>

* <span data-ttu-id="78b41-565">Parameterbeschreibung für Failoverrichtlinien korrigiert</span><span class="sxs-lookup"><span data-stu-id="78b41-565">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="78b41-566">Interactive</span><span class="sxs-lookup"><span data-stu-id="78b41-566">Interactive</span></span>

* <span data-ttu-id="78b41-567">Problem behoben, aufgrund dessen Vervollständigungen von Befehlsoptionen nicht mehr angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="78b41-567">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="78b41-568">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="78b41-568">Network</span></span>

* <span data-ttu-id="78b41-569">Schutz für `--cert-password` zu `application-gateway create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-569">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="78b41-570">Problem mit `application-gateway update` behoben, aufgrund dessen `--sku` fälschlicherweise einen Standardwert anwendete</span><span class="sxs-lookup"><span data-stu-id="78b41-570">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="78b41-571">Schutz für `--shared-key` und `--authorization-key` zu `vpn-connection create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-571">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="78b41-572">Problem mit fehlendem Client für `asg create` behoben</span><span class="sxs-lookup"><span data-stu-id="78b41-572">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="78b41-573">Parameter `--file-name / -f` für exportierte Namen zu `dns zone export` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-573">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="78b41-574">Folgende Probleme mit `dns zone export` behoben:</span><span class="sxs-lookup"><span data-stu-id="78b41-574">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="78b41-575">Problem behoben, aufgrund dessen lange TXT-Einträge nicht korrekt exportiert wurden</span><span class="sxs-lookup"><span data-stu-id="78b41-575">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="78b41-576">Problem behoben, aufgrund dessen TXT-Einträge in Anführungszeichen fälschlich ohne Anführungszeichen in Escapezeichen exportiert wurden</span><span class="sxs-lookup"><span data-stu-id="78b41-576">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="78b41-577">Problem behoben, aufgrund dessen bestimmte Datensätze zweimal mit `dns zone import` importiert wurden</span><span class="sxs-lookup"><span data-stu-id="78b41-577">Fixed issue where certain records were imported twice with `dns zone import`</span></span> 
* <span data-ttu-id="78b41-578">Befehle `vnet-gateway root-cert` und `vnet-gateway revoked-cert` wiederhergestellt</span><span class="sxs-lookup"><span data-stu-id="78b41-578">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="78b41-579">Profil</span><span class="sxs-lookup"><span data-stu-id="78b41-579">Profile</span></span>

* <span data-ttu-id="78b41-580">`get-access-token` zur Verwendung auf einer VM mit Identität korrigiert</span><span class="sxs-lookup"><span data-stu-id="78b41-580">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="78b41-581">Ressource</span><span class="sxs-lookup"><span data-stu-id="78b41-581">Resource</span></span>

* <span data-ttu-id="78b41-582">Fehler mit `deployment [create|validate]` korrigiert, aufgrund dessen fälschlich eine Warnung angezeigt wurde, wenn ein Vorlagenfeld „Typ“ Werte in Großbuchstaben enthielt</span><span class="sxs-lookup"><span data-stu-id="78b41-582">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="78b41-583">Speicher</span><span class="sxs-lookup"><span data-stu-id="78b41-583">Storage</span></span>

* <span data-ttu-id="78b41-584">Problem mit der Migration von Storage V1-Konten zu Storage V2 behoben</span><span class="sxs-lookup"><span data-stu-id="78b41-584">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="78b41-585">Statusberichterstellung für alle Upload-/Downloadbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-585">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="78b41-586">Fehler korrigiert, der die Verwendung der arg-Option „-n“ mit `storage account check-name` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="78b41-586">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>  
* <span data-ttu-id="78b41-587">Spalte „Momentaufnahme“ zur Tabellenausgabe für `blob [list|show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-587">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="78b41-588">Fehler mit verschiedenen Parametern korrigiert, die als Int-Typen analysiert werden mussten</span><span class="sxs-lookup"><span data-stu-id="78b41-588">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="78b41-589">VM</span><span class="sxs-lookup"><span data-stu-id="78b41-589">VM</span></span>

* <span data-ttu-id="78b41-590">Befehl `vm image accept-terms` hinzugefügt, um die Erstellung von VMs aus Images mit zusätzlichen Gebühren zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="78b41-590">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="78b41-591">`[vm|vmss create]` korrigiert, um sicherzustellen, dass Befehle unter einem Proxy mit nicht signierten Zertifikaten ausgeführt werden können</span><span class="sxs-lookup"><span data-stu-id="78b41-591">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="78b41-592">[VORSCHAU] Unterstützung für „niedrige“ Priorität zu VMSS hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-592">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="78b41-593">Schutz für `--admin-password` zu `[vm|vmss] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-593">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="78b41-594">17. Januar 2018</span><span class="sxs-lookup"><span data-stu-id="78b41-594">January 17, 2018</span></span>

<span data-ttu-id="78b41-595">Version 2.0.25</span><span class="sxs-lookup"><span data-stu-id="78b41-595">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="78b41-596">ACR</span><span class="sxs-lookup"><span data-stu-id="78b41-596">ACR</span></span>

* <span data-ttu-id="78b41-597">Fallback auf ACR-Anmeldung bei Fehlern mit Windows-Anmeldeinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-597">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="78b41-598">Registrierungsprotokolle aktiviert</span><span class="sxs-lookup"><span data-stu-id="78b41-598">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="78b41-599">ACS</span><span class="sxs-lookup"><span data-stu-id="78b41-599">ACS</span></span>

* <span data-ttu-id="78b41-600">Befehl `get-credentials` korrigiert</span><span class="sxs-lookup"><span data-stu-id="78b41-600">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="78b41-601">SPN-Rollenanforderung entfernt</span><span class="sxs-lookup"><span data-stu-id="78b41-601">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="78b41-602">AppService</span><span class="sxs-lookup"><span data-stu-id="78b41-602">Appservice</span></span>

* <span data-ttu-id="78b41-603">Fehler mit `config ssl upload` behoben, bei dem `hosting_environment_profile` NULL war</span><span class="sxs-lookup"><span data-stu-id="78b41-603">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="78b41-604">Unterstützung benutzerdefinierter URLs zu `browse` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-604">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="78b41-605">Slotunterstützung für `log tail` korrigiert</span><span class="sxs-lookup"><span data-stu-id="78b41-605">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="78b41-606">Backup</span><span class="sxs-lookup"><span data-stu-id="78b41-606">Backup</span></span>

* <span data-ttu-id="78b41-607">Option `--container-name` von `backup item list` geändert (ist jetzt optional)</span><span class="sxs-lookup"><span data-stu-id="78b41-607">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="78b41-608">Speicherkontooptionen zu `backup restore restore-disks` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-608">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="78b41-609">Standortüberprüfung in `backup protection enable-for-vm` korrigiert (Groß-/Kleinschreibung wird jetzt nicht mehr beachtet)</span><span class="sxs-lookup"><span data-stu-id="78b41-609">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="78b41-610">Problem behoben, durch das bei Befehlen mit ungültigem Containernamen ein Fehler auftrat</span><span class="sxs-lookup"><span data-stu-id="78b41-610">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="78b41-611">`backup item list` geändert (Integritätsstatus jetzt standardmäßig enthalten)</span><span class="sxs-lookup"><span data-stu-id="78b41-611">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="78b41-612">Batch</span><span class="sxs-lookup"><span data-stu-id="78b41-612">Batch</span></span>

* <span data-ttu-id="78b41-613">`batch login` geändert, um Authentifizierungsdetails zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="78b41-613">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="78b41-614">Cloud</span><span class="sxs-lookup"><span data-stu-id="78b41-614">Cloud</span></span>

* <span data-ttu-id="78b41-615">Beim Festlegen von `--profile` für eine Cloud werden nun keine Endpunkte mehr benötigt.</span><span class="sxs-lookup"><span data-stu-id="78b41-615">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="78b41-616">Nutzung</span><span class="sxs-lookup"><span data-stu-id="78b41-616">Consumption</span></span>

* <span data-ttu-id="78b41-617">Neue Befehle für Reservierungen hinzugefügt: `consumption reservations summaries` und `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="78b41-617">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="78b41-618">Event Grid</span><span class="sxs-lookup"><span data-stu-id="78b41-618">Event Grid</span></span>

* <span data-ttu-id="78b41-619">[WICHTIGE ÄNDERUNG] Die Befehle vom Typ `az eventgrid topic event-subscription` wurden in `eventgrid event-subscription` verschoben.</span><span class="sxs-lookup"><span data-stu-id="78b41-619">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="78b41-620">[WICHTIGE ÄNDERUNG] Die Befehle vom Typ `az eventgrid resource event-subscription` wurden in `eventgrid event-subscription` verschoben.</span><span class="sxs-lookup"><span data-stu-id="78b41-620">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="78b41-621">[WICHTIGE ÄNDERUNG] Der Befehl `eventgrid event-subscription show-endpoint-url` wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="78b41-621">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="78b41-622">Verwenden Sie stattdessen `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="78b41-622">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="78b41-623">Befehl `eventgrid topic update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-623">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="78b41-624">Befehl `eventgrid event-subscription update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-624">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="78b41-625">Parameter `--ids` für Befehle vom Typ `eventgrid topic` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-625">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="78b41-626">Unterstützung der Vervollständigung mit der TAB-TASTE für Themennamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-626">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="78b41-627">Interactive</span><span class="sxs-lookup"><span data-stu-id="78b41-627">Interactive</span></span>

* <span data-ttu-id="78b41-628">Problem behoben, das dazu führte, dass der interaktive Modus nicht mit Python 2.x verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="78b41-628">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="78b41-629">Fehler beim Start behoben</span><span class="sxs-lookup"><span data-stu-id="78b41-629">Fixed errors on startup</span></span>
* <span data-ttu-id="78b41-630">Problem behoben, das dazu führte, dass einige Befehle nicht im interaktiven Modus ausgeführt werden konnten</span><span class="sxs-lookup"><span data-stu-id="78b41-630">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="78b41-631">IoT</span><span class="sxs-lookup"><span data-stu-id="78b41-631">IoT</span></span>

* <span data-ttu-id="78b41-632">Unterstützung für Gerätebereitstellungsdienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-632">Added support for device provisioning service</span></span>
* <span data-ttu-id="78b41-633">Benachrichtigungen zu veralteten Elementen in Befehlen und in der Befehlshilfe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-633">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="78b41-634">IoT-Überprüfung hinzugefügt, um Benutzer über die IoT-Erweiterung zu informieren</span><span class="sxs-lookup"><span data-stu-id="78b41-634">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="78b41-635">Überwachen</span><span class="sxs-lookup"><span data-stu-id="78b41-635">Monitor</span></span>

* <span data-ttu-id="78b41-636">Unterstützung mehrerer Diagnoseeinstellung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="78b41-636">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="78b41-637">Der Parameter `--name` ist nun für `az monitor diagnostic-settings create` erforderlich.</span><span class="sxs-lookup"><span data-stu-id="78b41-637">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="78b41-638">Befehl `monitor diagnostic-settings categories` zum Abrufen der Diagnoseeinstellungskategorie hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-638">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="78b41-639">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="78b41-639">Network</span></span>

* <span data-ttu-id="78b41-640">Problem behoben, das beim Ändern des aktiven Standbymodus mit `vnet-gateway update` auftrat</span><span class="sxs-lookup"><span data-stu-id="78b41-640">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="78b41-641">Unterstützung für HTTP2 zu `application-gateway [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-641">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="78b41-642">Profil</span><span class="sxs-lookup"><span data-stu-id="78b41-642">Profile</span></span>

* <span data-ttu-id="78b41-643">Unterstützung für die Anmeldung mit durch Benutzer zugewiesenen Identitäten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-643">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="78b41-644">Rolle</span><span class="sxs-lookup"><span data-stu-id="78b41-644">Role</span></span>

* <span data-ttu-id="78b41-645">Argument `--assignee-object-id` zu `role assignment create` hinzugefügt, um Graph-Abfrage zu umgehen</span><span class="sxs-lookup"><span data-stu-id="78b41-645">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="78b41-646">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="78b41-646">Service Fabric</span></span>

* <span data-ttu-id="78b41-647">Ausführliche Fehler zur Überprüfungsantwort bei der Clustererstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-647">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="78b41-648">Problem mit fehlendem Client für verschiedene Befehle behoben</span><span class="sxs-lookup"><span data-stu-id="78b41-648">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="78b41-649">VM</span><span class="sxs-lookup"><span data-stu-id="78b41-649">VM</span></span>

* <span data-ttu-id="78b41-650">[VORSCHAUVERSION] Zonenübergreifende Unterstützung für `vmss`</span><span class="sxs-lookup"><span data-stu-id="78b41-650">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="78b41-651">[WICHTIGE ÄNDERUNG] Standard für Einzelzone (`vmss`) in Standardlastenausgleich geändert</span><span class="sxs-lookup"><span data-stu-id="78b41-651">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="78b41-652">[WICHTIGE ÄNDERUNG] `externalIdentities` in `userAssignedIdentities` geändert für EMSI</span><span class="sxs-lookup"><span data-stu-id="78b41-652">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="78b41-653">[VORSCHAUVERSION] Unterstützung für Austausch des Betriebssystemdatenträgers hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-653">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="78b41-654">Unterstützung der Verwendung von VM-Images aus anderen Abonnements hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-654">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="78b41-655">Argumente `--plan-name`, `--plan-product`, `--plan-promotion-code` und `--plan-publisher` zu `[vm|vmss] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-655">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="78b41-656">Fehlerbedingte Probleme mit `[vm|vmss] create` behoben</span><span class="sxs-lookup"><span data-stu-id="78b41-656">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="78b41-657">Übermäßige Ressourcenverwendung durch `vm image list --all` behoben</span><span class="sxs-lookup"><span data-stu-id="78b41-657">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="78b41-658">19. Dezember 2017</span><span class="sxs-lookup"><span data-stu-id="78b41-658">December 19, 2017</span></span>

<span data-ttu-id="78b41-659">Version 2.0.23</span><span class="sxs-lookup"><span data-stu-id="78b41-659">Version 2.0.23</span></span>

* <span data-ttu-id="78b41-660">Unterstützung für die Anmeldung mit durch Benutzer zugewiesenen Identitäten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-660">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="78b41-661">Container</span><span class="sxs-lookup"><span data-stu-id="78b41-661">Container</span></span>

* <span data-ttu-id="78b41-662">Falsche Reihenfolge der Parameter für Containerprotokolle behoben</span><span class="sxs-lookup"><span data-stu-id="78b41-662">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="78b41-663">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="78b41-663">Network</span></span>

* <span data-ttu-id="78b41-664">Argument `--disable-bgp-route-propagation` zu `route-table [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-664">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="78b41-665">Argument `--ip-tags` zu `public-ip [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-665">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="78b41-666">Speicher</span><span class="sxs-lookup"><span data-stu-id="78b41-666">Storage</span></span>

* <span data-ttu-id="78b41-667">Unterstützung für Storage V2 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-667">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="78b41-668">VM</span><span class="sxs-lookup"><span data-stu-id="78b41-668">VM</span></span>

* <span data-ttu-id="78b41-669">[VORSCHAUVERSION] Unterstützung für durch Benutzer zugewiesene Identitäten für virtuelle Computer und VMSSs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-669">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="78b41-670">5. Dezember 2017</span><span class="sxs-lookup"><span data-stu-id="78b41-670">December 5, 2017</span></span>

<span data-ttu-id="78b41-671">Version 2.0.22</span><span class="sxs-lookup"><span data-stu-id="78b41-671">Version 2.0.22</span></span>

* <span data-ttu-id="78b41-672">`az component`-Befehle wurden entfernt.</span><span class="sxs-lookup"><span data-stu-id="78b41-672">Removed `az component` commands.</span></span> <span data-ttu-id="78b41-673">Verwenden Sie stattdessen `az extension`.</span><span class="sxs-lookup"><span data-stu-id="78b41-673">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="78b41-674">Core</span><span class="sxs-lookup"><span data-stu-id="78b41-674">Core</span></span>
* <span data-ttu-id="78b41-675">Der `AZURE_US_GOV_CLOUD`-Autoritätsendpunkt von AAD wurde von „login.microsoftonline.com“ in „login.microsoftonline.us“ geändert.</span><span class="sxs-lookup"><span data-stu-id="78b41-675">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="78b41-676">Problem behoben, aufgrund dessen Telemetriedaten fortlaufend neu gesendet wurden</span><span class="sxs-lookup"><span data-stu-id="78b41-676">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="78b41-677">ACS</span><span class="sxs-lookup"><span data-stu-id="78b41-677">ACS</span></span>

* <span data-ttu-id="78b41-678">Die Befehle `aks install-connector` und `aks remove-connector` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="78b41-678">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="78b41-679">Verbesserte Fehlerberichterstellung für `acs create`</span><span class="sxs-lookup"><span data-stu-id="78b41-679">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="78b41-680">Feste Verwendung von `aks get-credentials -f` ohne vollqualifizierten Pfad</span><span class="sxs-lookup"><span data-stu-id="78b41-680">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="78b41-681">Advisor</span><span class="sxs-lookup"><span data-stu-id="78b41-681">Advisor</span></span>

* <span data-ttu-id="78b41-682">Erste Version</span><span class="sxs-lookup"><span data-stu-id="78b41-682">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="78b41-683">AppService</span><span class="sxs-lookup"><span data-stu-id="78b41-683">Appservice</span></span>

* <span data-ttu-id="78b41-684">Erstellung feststehender Zertifikatnamen mit `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="78b41-684">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="78b41-685">`webapp [list|show]` und `functionapp [list|show]` wurden verbessert, um die richtigen Apps anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="78b41-685">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="78b41-686">Standardwert für `WEBSITE_NODE_DEFAULT_VERSION` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-686">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="78b41-687">Nutzung</span><span class="sxs-lookup"><span data-stu-id="78b41-687">Consumption</span></span>

* <span data-ttu-id="78b41-688">Unterstützung für API-Version 2017-11-30 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-688">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="78b41-689">Container</span><span class="sxs-lookup"><span data-stu-id="78b41-689">Container</span></span>

* <span data-ttu-id="78b41-690">Feste Regression für Standardports</span><span class="sxs-lookup"><span data-stu-id="78b41-690">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="78b41-691">Überwachen</span><span class="sxs-lookup"><span data-stu-id="78b41-691">Monitor</span></span>

* <span data-ttu-id="78b41-692">Unterstützung mehrerer Dimensionen zu Metrikbefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-692">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="78b41-693">Ressource</span><span class="sxs-lookup"><span data-stu-id="78b41-693">Resource</span></span>

* <span data-ttu-id="78b41-694">Argument `--include-response-body` zu `resource show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-694">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="78b41-695">Rolle</span><span class="sxs-lookup"><span data-stu-id="78b41-695">Role</span></span>

* <span data-ttu-id="78b41-696">Anzeige von Standardzuweisungen für „klassische“ Administratoren zu `role assignment list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-696">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="78b41-697">Unterstützung für das Hinzufügen (anstelle der Überschreibung) von Anmeldeinformationen zu `ad sp reset-credentials` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-697">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="78b41-698">Verbesserte Fehlerberichterstellung für `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="78b41-698">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="78b41-699">SQL</span><span class="sxs-lookup"><span data-stu-id="78b41-699">SQL</span></span>

* <span data-ttu-id="78b41-700">Die Befehle `sql db list-usages` und `sql db show-usage` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="78b41-700">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="78b41-701">Die Befehle `sql server conn-policy show` und `sql server conn-policy update` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="78b41-701">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="78b41-702">VM</span><span class="sxs-lookup"><span data-stu-id="78b41-702">VM</span></span>

* <span data-ttu-id="78b41-703">Zoneninformationen zu `az vm list-skus` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-703">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="78b41-704">14. November 2017</span><span class="sxs-lookup"><span data-stu-id="78b41-704">November 14, 2017</span></span>

<span data-ttu-id="78b41-705">Version 2.0.21</span><span class="sxs-lookup"><span data-stu-id="78b41-705">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="78b41-706">ACR</span><span class="sxs-lookup"><span data-stu-id="78b41-706">ACR</span></span>

* <span data-ttu-id="78b41-707">Unterstützung für das Erstellen von Webhooks in Replikationsregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-707">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="78b41-708">ACS</span><span class="sxs-lookup"><span data-stu-id="78b41-708">ACS</span></span>

* <span data-ttu-id="78b41-709">Formulierung in AKS von „Agent“ in „Knoten“ geändert</span><span class="sxs-lookup"><span data-stu-id="78b41-709">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="78b41-710">Option `--orchestrator-release` für `acs create` als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="78b41-710">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="78b41-711">VM-Standardgröße für AKS in `Standard_D1_v2` geändert</span><span class="sxs-lookup"><span data-stu-id="78b41-711">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="78b41-712">`az aks browse` für Windows korrigiert</span><span class="sxs-lookup"><span data-stu-id="78b41-712">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="78b41-713">`az aks get-credentials` für Windows korrigiert</span><span class="sxs-lookup"><span data-stu-id="78b41-713">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="78b41-714">AppService</span><span class="sxs-lookup"><span data-stu-id="78b41-714">Appservice</span></span>

* <span data-ttu-id="78b41-715">Bereitstellungsquelle `config-zip` für Web-Apps und Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-715">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="78b41-716">Option `--docker-container-logging` zu `az webapp log config` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-716">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="78b41-717">Option `storage` aus dem Parameter `--web-server-logging` von `az webapp log config` entfernt</span><span class="sxs-lookup"><span data-stu-id="78b41-717">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="78b41-718">Fehlermeldungen für `deployment user set` verbessert</span><span class="sxs-lookup"><span data-stu-id="78b41-718">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="78b41-719">Unterstützung für das Erstellen von Linux-Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-719">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="78b41-720">`list-locations` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="78b41-720">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="78b41-721">Batch</span><span class="sxs-lookup"><span data-stu-id="78b41-721">Batch</span></span>

* <span data-ttu-id="78b41-722">Fehler im Poolerstellungsbefehl korrigiert, der bei Verwendung einer Ressourcen-ID mit dem Flag `--image` aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="78b41-722">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="78b41-723">BatchAI</span><span class="sxs-lookup"><span data-stu-id="78b41-723">Batchai</span></span>

* <span data-ttu-id="78b41-724">Kurzoption (`-s`) für `--vm-size` zur Angabe der VM-Größe im Befehl `file-server create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-724">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="78b41-725">Argumente für Speicherkontoname und -schlüssel zum Parameter `cluster create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-725">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="78b41-726">Dokumentation für `job list-files` und `job stream-file` korrigiert</span><span class="sxs-lookup"><span data-stu-id="78b41-726">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="78b41-727">Kurzoption (`-r`) für `--cluster-name` zur Angabe des Clusternamens im Befehl `job create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-727">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="78b41-728">Cloud</span><span class="sxs-lookup"><span data-stu-id="78b41-728">Cloud</span></span>

* <span data-ttu-id="78b41-729">`cloud [register|update]` geändert, um die Registrierung von Clouds ohne erforderliche Endpunkte zu verhindern</span><span class="sxs-lookup"><span data-stu-id="78b41-729">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="78b41-730">Container</span><span class="sxs-lookup"><span data-stu-id="78b41-730">Container</span></span>

* <span data-ttu-id="78b41-731">Unterstützung für das Öffnen mehrerer Ports hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-731">Added support to open multiple ports</span></span>
* <span data-ttu-id="78b41-732">Neustartrichtlinie für Containergruppen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-732">Added container group restart policy</span></span>
* <span data-ttu-id="78b41-733">Unterstützung zum Einbinden einer Azure-Dateifreigabe als Volume hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-733">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="78b41-734">Hilfedokumente aktualisiert</span><span class="sxs-lookup"><span data-stu-id="78b41-734">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="78b41-735">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="78b41-735">Data Lake Analytics</span></span>

* <span data-ttu-id="78b41-736">`[job|account] list` geändert, um präzisere Informationen zu erhalten</span><span class="sxs-lookup"><span data-stu-id="78b41-736">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="78b41-737">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="78b41-737">Data Lake Store</span></span>

* <span data-ttu-id="78b41-738">`account list` geändert, um präzisere Informationen zu erhalten</span><span class="sxs-lookup"><span data-stu-id="78b41-738">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="78b41-739">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="78b41-739">Extension</span></span>

* <span data-ttu-id="78b41-740">`extension list-available` hinzugefügt, um das Auflisten offizieller Microsoft-Erweiterungen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="78b41-740">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="78b41-741">`--name` zu `extension [add|update]` hinzugefügt, um das Installieren von Erweiterungen nach Name zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="78b41-741">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="78b41-742">IoT</span><span class="sxs-lookup"><span data-stu-id="78b41-742">IoT</span></span>

* <span data-ttu-id="78b41-743">Unterstützung für Zertifizierungsstellen (CAs) und Zertifikatketten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-743">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="78b41-744">Überwachen</span><span class="sxs-lookup"><span data-stu-id="78b41-744">Monitor</span></span>

* <span data-ttu-id="78b41-745">Befehle vom Typ `activity-log alert` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-745">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="78b41-746">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="78b41-746">Network</span></span>

* <span data-ttu-id="78b41-747">Unterstützung für CAA-DNS-Einträge hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-747">Added support for CAA DNS records</span></span>
* <span data-ttu-id="78b41-748">Problem behoben, durch das Endpunkte nicht mit `traffic-manager profile update` aktualisiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="78b41-748">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="78b41-749">Problem behoben, durch das `vnet update --dns-servers` je nach VNet-Erstellungsmethode nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="78b41-749">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="78b41-750">Problem behoben, durch das relative DNS-Namen durch `dns zone import` nicht korrekt importiert wurden</span><span class="sxs-lookup"><span data-stu-id="78b41-750">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="78b41-751">Reservations</span><span class="sxs-lookup"><span data-stu-id="78b41-751">Reservations</span></span>

* <span data-ttu-id="78b41-752">Erste Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="78b41-752">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="78b41-753">Ressource</span><span class="sxs-lookup"><span data-stu-id="78b41-753">Resource</span></span>

* <span data-ttu-id="78b41-754">Unterstützung für Ressourcen-IDs zum Parameter `--resource` und Sperren auf Ressourcenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-754">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="78b41-755">SQL</span><span class="sxs-lookup"><span data-stu-id="78b41-755">SQL</span></span>

* <span data-ttu-id="78b41-756">Parameter `--ignore-missing-vnet-service-endpoint` zu `sql server vnet-rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-756">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="78b41-757">Speicher</span><span class="sxs-lookup"><span data-stu-id="78b41-757">Storage</span></span>

* <span data-ttu-id="78b41-758">`storage account create` geändert, sodass die SKU `Standard_RAGRS` als Standard verwendet wird</span><span class="sxs-lookup"><span data-stu-id="78b41-758">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="78b41-759">Fehler im Zusammenhang mit Datei-/Blobnamen korrigiert, die ASCII-fremde Zeichen enthalten</span><span class="sxs-lookup"><span data-stu-id="78b41-759">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="78b41-760">Fehler korrigiert, der die Verwendung von `--source-uri` mit `storage [blob|file] copy start-batch` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="78b41-760">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="78b41-761">Befehle zum Globalisieren und Löschen mehrerer Objekte mit `storage [blob|file] delete-batch` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-761">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="78b41-762">Problem beim Aktivieren von Metriken mit `storage metrics update` behoben</span><span class="sxs-lookup"><span data-stu-id="78b41-762">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="78b41-763">Problem mit Dateien über 200 GB bei Verwendung von `storage blob upload-batch` behoben</span><span class="sxs-lookup"><span data-stu-id="78b41-763">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="78b41-764">Problem behoben, durch das `--bypass` und `--default-action` von `storage account [create|update]` ignoriert wurden</span><span class="sxs-lookup"><span data-stu-id="78b41-764">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="78b41-765">VM</span><span class="sxs-lookup"><span data-stu-id="78b41-765">VM</span></span>

* <span data-ttu-id="78b41-766">Fehler mit `vmss create` korrigiert, der die Verwendung der Größenebene `Basic` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="78b41-766">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="78b41-767">`--plan`-Argumente zu `[vm|vmss] create` für benutzerdefinierte Images mit Abrechnungsinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-767">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="78b41-768">Befehle hinzugefügt: `vm secret `[add|remove|list]</span><span class="sxs-lookup"><span data-stu-id="78b41-768">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="78b41-769">`vm format-secret` in `vm secret format` umbenannt</span><span class="sxs-lookup"><span data-stu-id="78b41-769">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="78b41-770">Argument `--encrypt format` zu `vm encryption enable` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-770">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="78b41-771">24. Oktober 2017</span><span class="sxs-lookup"><span data-stu-id="78b41-771">October 24, 2017</span></span>

<span data-ttu-id="78b41-772">Version 2.0.20</span><span class="sxs-lookup"><span data-stu-id="78b41-772">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="78b41-773">Core</span><span class="sxs-lookup"><span data-stu-id="78b41-773">Core</span></span>

* <span data-ttu-id="78b41-774">Aktualisierung von `2017-03-09-profile` zur Verwendung von Version `2016-01-01` der `MGMT_STORAGE`-API</span><span class="sxs-lookup"><span data-stu-id="78b41-774">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="78b41-775">ACR</span><span class="sxs-lookup"><span data-stu-id="78b41-775">ACR</span></span>

* <span data-ttu-id="78b41-776">Die Ressourcenverwaltung wurde aktualisiert und verweist nun auf die API-Version `2017-10-01`.</span><span class="sxs-lookup"><span data-stu-id="78b41-776">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="78b41-777">SKU „Bring Your Own Storage“ wurde in „Klassisch“ geändert.</span><span class="sxs-lookup"><span data-stu-id="78b41-777">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="78b41-778">Die Registrierungs-SKUs wurden in „Basic“, „Standard“ und „Premium“ umbenannt.</span><span class="sxs-lookup"><span data-stu-id="78b41-778">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="78b41-779">ACS</span><span class="sxs-lookup"><span data-stu-id="78b41-779">ACS</span></span>

* <span data-ttu-id="78b41-780">[VORSCHAUVERSION] Befehle vom Typ `az aks` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-780">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="78b41-781">Problem mit `get-credentials` in Kubernetes behoben</span><span class="sxs-lookup"><span data-stu-id="78b41-781">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="78b41-782">AppService</span><span class="sxs-lookup"><span data-stu-id="78b41-782">Appservice</span></span>

* <span data-ttu-id="78b41-783">Problem behoben, aufgrund dessen heruntergeladene `webapp`-Protokolle unter Umständen ungültig waren</span><span class="sxs-lookup"><span data-stu-id="78b41-783">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="78b41-784">Komponente</span><span class="sxs-lookup"><span data-stu-id="78b41-784">Component</span></span>

* <span data-ttu-id="78b41-785">Deutlichere Meldung zur Einstellung für alle Installer und für Bestätigungsaufforderung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-785">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="78b41-786">Überwachen</span><span class="sxs-lookup"><span data-stu-id="78b41-786">Monitor</span></span>

* <span data-ttu-id="78b41-787">Befehle vom Typ `action-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-787">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="78b41-788">Ressource</span><span class="sxs-lookup"><span data-stu-id="78b41-788">Resource</span></span>

* <span data-ttu-id="78b41-789">Inkompatibilität mit der aktuellen Version der msrest-Abhängigkeit in `group export` behoben</span><span class="sxs-lookup"><span data-stu-id="78b41-789">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="78b41-790">Problem mit `policy assignment create` behoben, sodass der Befehl mit integrierten Richtliniendefinitionen und Richtliniensatzdefinitionen verwendet werden kann</span><span class="sxs-lookup"><span data-stu-id="78b41-790">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="78b41-791">VM</span><span class="sxs-lookup"><span data-stu-id="78b41-791">VM</span></span>

* <span data-ttu-id="78b41-792">Argument `--accelerated-networking` zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-792">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="78b41-793">9. Oktober 2017</span><span class="sxs-lookup"><span data-stu-id="78b41-793">October 9, 2017</span></span>

<span data-ttu-id="78b41-794">Version 2.0.19</span><span class="sxs-lookup"><span data-stu-id="78b41-794">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="78b41-795">Core</span><span class="sxs-lookup"><span data-stu-id="78b41-795">Core</span></span>

* <span data-ttu-id="78b41-796">Verarbeitung von ADFS-Autoritäts-URLs wurde mit einem nachgestellten Schrägstrich zu Azure Stack hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="78b41-796">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="78b41-797">AppService</span><span class="sxs-lookup"><span data-stu-id="78b41-797">Appservice</span></span>

* <span data-ttu-id="78b41-798">Mit dem neuen Befehl `webapp update` wurde ein allgemeines Update hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="78b41-798">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="78b41-799">Batch</span><span class="sxs-lookup"><span data-stu-id="78b41-799">Batch</span></span>

* <span data-ttu-id="78b41-800">Aktualisierung auf Batch SDK 4.0.0</span><span class="sxs-lookup"><span data-stu-id="78b41-800">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="78b41-801">Die Option `--image` von „VirtualMachineConfiguration“ wurde aktualisiert, um zusätzlich zu „publish:offer:sku:version“ ARM-Imageverweise zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="78b41-801">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="78b41-802">Unterstützung für das neue CLI-Erweiterungsmodell für Batch-Erweiterungsbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-802">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="78b41-803">Batch-Unterstützung aus dem Komponentenmodell entfernt</span><span class="sxs-lookup"><span data-stu-id="78b41-803">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="78b41-804">BatchAI</span><span class="sxs-lookup"><span data-stu-id="78b41-804">Batchai</span></span>

* <span data-ttu-id="78b41-805">Erste Version des Batch AI-Moduls</span><span class="sxs-lookup"><span data-stu-id="78b41-805">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="78b41-806">KeyVault</span><span class="sxs-lookup"><span data-stu-id="78b41-806">Keyvault</span></span>

* <span data-ttu-id="78b41-807">Key Vault-Authentifizierungsproblem behoben, das bei Verwendung von ADFS in Azure Stack auftrat.</span><span class="sxs-lookup"><span data-stu-id="78b41-807">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="78b41-808">(#4448)</span><span class="sxs-lookup"><span data-stu-id="78b41-808">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="78b41-809">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="78b41-809">Network</span></span>

* <span data-ttu-id="78b41-810">Das Argument `--server` von `application-gateway address-pool create` ist nun optional, sodass leere Adresspools zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="78b41-810">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="78b41-811">`traffic-manager` wurde aktualisiert, um aktuelle Features zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="78b41-811">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="78b41-812">Ressource</span><span class="sxs-lookup"><span data-stu-id="78b41-812">Resource</span></span>

* <span data-ttu-id="78b41-813">Zusätzliche Unterstützung für `--resource-group/-g`-Optionen für Ressourcengruppennamen zu `group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-813">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="78b41-814">Befehle für `account lock` hinzugefügt, um die Verwendung mit Sperren auf Abonnementebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="78b41-814">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="78b41-815">Befehle für `group lock` hinzugefügt, um die Verwendung mit Sperren auf Gruppenebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="78b41-815">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="78b41-816">Befehle für `resource lock` hinzugefügt, um die Verwendung mit Sperren auf Ressourcenebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="78b41-816">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="78b41-817">Sql</span><span class="sxs-lookup"><span data-stu-id="78b41-817">Sql</span></span>

* <span data-ttu-id="78b41-818">Unterstützung für SQL Transparent Data Encryption (TDE) und TDE für Bring Your Own Key-Szenarien hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-818">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="78b41-819">Der Befehl `db list-deleted` und der Parameter `db restore --deleted-time` wurden hinzugefügt, um die Ermittlung und Wiederherstellung gelöschter Datenbanken zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="78b41-819">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="78b41-820">`db op list` und `db op cancel` wurden hinzugefügt, um das Auflisten und Abbrechen ausgeführter Vorgänge für eine Datenbank zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="78b41-820">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="78b41-821">Speicher</span><span class="sxs-lookup"><span data-stu-id="78b41-821">Storage</span></span>

* <span data-ttu-id="78b41-822">Unterstützung für Momentaufnahme von Dateifreigaben hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-822">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="78b41-823">VM</span><span class="sxs-lookup"><span data-stu-id="78b41-823">Vm</span></span>

* <span data-ttu-id="78b41-824">Korrektur eines Fehlers in `vm show`, bei dem die Verwendung von `-d` in Verbindung mit fehlenden privaten IP-Adressen einen Absturz verursachte</span><span class="sxs-lookup"><span data-stu-id="78b41-824">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="78b41-825">[VORSCHAUVERSION] Unterstützung für paralleles Upgrade zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-825">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="78b41-826">Unterstützung für das Aktualisieren der Verschlüsselungseinstellungen mit `vm encryption enable` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-826">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="78b41-827">Parameter `--os-disk-size-gb` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-827">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="78b41-828">Parameter `--license-type` für Windows zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-828">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="78b41-829">22. September 2017</span><span class="sxs-lookup"><span data-stu-id="78b41-829">September 22, 2017</span></span>

<span data-ttu-id="78b41-830">Version 2.0.18</span><span class="sxs-lookup"><span data-stu-id="78b41-830">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="78b41-831">Ressource</span><span class="sxs-lookup"><span data-stu-id="78b41-831">Resource</span></span>

* <span data-ttu-id="78b41-832">Unterstützung für das Anzeigen integrierter Richtliniendefinitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-832">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="78b41-833">Unterstützungsmodusparameter zum Erstellen von Richtliniendefinitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-833">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="78b41-834">Unterstützung für UI-Definitionen und -Vorlagen zu `managedapp definition create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-834">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="78b41-835">[WICHTIGE ÄNDERUNG] Der Ressourcentyp `managedapp` wurde von `appliances` in `applications` und von `applianceDefinitions` in `applicationDefinitions` geändert.</span><span class="sxs-lookup"><span data-stu-id="78b41-835">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="78b41-836">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="78b41-836">Network</span></span>

* <span data-ttu-id="78b41-837">Unterstützung für Verfügbarkeitszone zu Unterbefehlen `network lb` und `network public-ip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-837">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="78b41-838">Unterstützung für IPv6-Microsoft-Peering zu `express-route` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-838">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="78b41-839">Befehle für Anwendungssicherheitsgruppe `asg` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-839">Added `asg` application security group commands</span></span>
* <span data-ttu-id="78b41-840">Argument `--application-security-groups` zu `nic [create|ip-config create|ip-config update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-840">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="78b41-841">Argumente `--source-asgs` und `--destination-asgs` zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-841">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="78b41-842">Argumente `--ddos-protection` und `--vm-protection` zu `vnet [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-842">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="78b41-843">Befehle vom Typ `network [vnet-gateway|vpn-client|show-url]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-843">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="78b41-844">Speicher</span><span class="sxs-lookup"><span data-stu-id="78b41-844">Storage</span></span>

* <span data-ttu-id="78b41-845">Problem behoben, das nach der Aktualisierung des SDK unter Umständen einen Fehler der `storage account network-rule`-Befehle zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="78b41-845">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="78b41-846">Eventgrid</span><span class="sxs-lookup"><span data-stu-id="78b41-846">Eventgrid</span></span>

* <span data-ttu-id="78b41-847">Azure Event Grid Python SDK für die Verwendung der neueren API-Version „2017-09-15-preview“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="78b41-847">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="78b41-848">SQL</span><span class="sxs-lookup"><span data-stu-id="78b41-848">SQL</span></span>

* <span data-ttu-id="78b41-849">`sql server list`-Argument `--resource-group` geändert, sodass es nun optional ist.</span><span class="sxs-lookup"><span data-stu-id="78b41-849">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="78b41-850">Wird es nicht angegeben, werden alle SQL Server-Instanzen im Abonnement zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="78b41-850">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="78b41-851">Parameter `--no-wait` zu `db [create|copy|restore|update|replica create|create|update]` und `dw [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-851">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="78b41-852">KeyVault</span><span class="sxs-lookup"><span data-stu-id="78b41-852">Keyvault</span></span>

* <span data-ttu-id="78b41-853">Unterstützung für die Keyvault-Befehlsausführung hinter einem Proxy hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-853">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="78b41-854">VM</span><span class="sxs-lookup"><span data-stu-id="78b41-854">VM</span></span>

* <span data-ttu-id="78b41-855">Unterstützung für Verfügbarkeitszone zu `[vm|vmss|disk] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-855">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="78b41-856">Problem behoben, das bei Verwendung von `--app-gateway ID` mit `vmss create` einen Fehler zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="78b41-856">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="78b41-857">Argument `--asgs` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-857">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="78b41-858">Unterstützung für die Ausführung von Befehlen auf virtuellen Computern mit `vm run-command` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-858">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="78b41-859">[VORSCHAU] Unterstützung für VMSS-Datenträgerverschlüsselung mit `vmss encryption` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-859">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="78b41-860">Unterstützung für die Durchführung der Wartung auf virtuellen Computern mit `vm perform-maintenance` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-860">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="78b41-861">ACS</span><span class="sxs-lookup"><span data-stu-id="78b41-861">ACS</span></span>

* <span data-ttu-id="78b41-862">[VORSCHAU] Argument `--orchestrator-release` zu `acs create` für ACS-Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-862">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="78b41-863">AppService</span><span class="sxs-lookup"><span data-stu-id="78b41-863">Appservice</span></span>

* <span data-ttu-id="78b41-864">Neue Möglichkeit zum Aktualisieren und Anzeigen der Authentifizierungseinstellungen mit `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="78b41-864">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="78b41-865">Backup</span><span class="sxs-lookup"><span data-stu-id="78b41-865">Backup</span></span>

* <span data-ttu-id="78b41-866">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="78b41-866">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="78b41-867">11. September 2017</span><span class="sxs-lookup"><span data-stu-id="78b41-867">September 11, 2017</span></span>

<span data-ttu-id="78b41-868">Version 2.0.17</span><span class="sxs-lookup"><span data-stu-id="78b41-868">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="78b41-869">Core</span><span class="sxs-lookup"><span data-stu-id="78b41-869">Core</span></span>

* <span data-ttu-id="78b41-870">Festlegung einer eigenen Korrelations-ID in Telemetrie durch das Befehlsmodul aktiviert</span><span class="sxs-lookup"><span data-stu-id="78b41-870">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="78b41-871">Ein Problem mit der JSON-Sicherungsdatei wurde behoben, das beim Festlegen des Diagnosemodus für Telemetrie auftrat</span><span class="sxs-lookup"><span data-stu-id="78b41-871">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="78b41-872">ACS</span><span class="sxs-lookup"><span data-stu-id="78b41-872">Acs</span></span>

* <span data-ttu-id="78b41-873">Befehl `acs list-locations` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-873">Added `acs list-locations` command</span></span>
* <span data-ttu-id="78b41-874">`ssh-key-file` wird mit dem erwarteten Standardwert versehen.</span><span class="sxs-lookup"><span data-stu-id="78b41-874">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="78b41-875">AppService</span><span class="sxs-lookup"><span data-stu-id="78b41-875">Appservice</span></span>

* <span data-ttu-id="78b41-876">Neue Möglichkeit zum Erstellen einer Web-App in einer anderen Ressourcengruppe als der des aktiven Diensttarifs</span><span class="sxs-lookup"><span data-stu-id="78b41-876">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="78b41-877">CDN</span><span class="sxs-lookup"><span data-stu-id="78b41-877">CDN</span></span>

* <span data-ttu-id="78b41-878">Der Fehler bei `cdn custom-domain create`, dass „CustomDomain“ nicht wiederholbar ist, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="78b41-878">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="78b41-879">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="78b41-879">Extension</span></span>

* <span data-ttu-id="78b41-880">Erste Version</span><span class="sxs-lookup"><span data-stu-id="78b41-880">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="78b41-881">KeyVault</span><span class="sxs-lookup"><span data-stu-id="78b41-881">Keyvault</span></span>

* <span data-ttu-id="78b41-882">Problem behoben, aufgrund dessen bei den Berechtigungen für `keyvault set-policy` die Groß-/Kleinschreibung beachtet werden musste</span><span class="sxs-lookup"><span data-stu-id="78b41-882">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="78b41-883">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="78b41-883">Network</span></span>

* <span data-ttu-id="78b41-884">`vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="78b41-884">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="78b41-885">Das Argument `--private-access-services` wurde für `vnet subnet create/update` in `--service-endpoints` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="78b41-885">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="78b41-886">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-886">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="78b41-887">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-887">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="78b41-888">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-888">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="78b41-889">Ressource</span><span class="sxs-lookup"><span data-stu-id="78b41-889">Resource</span></span>

* <span data-ttu-id="78b41-890">Übergabe von Parameterdefinitionen für Ressourcenrichtlinien in `policy definition create` und `policy definition update` zulassen</span><span class="sxs-lookup"><span data-stu-id="78b41-890">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="78b41-891">Übergabe von Parameterwerten für `policy assignment create` zulassen</span><span class="sxs-lookup"><span data-stu-id="78b41-891">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="78b41-892">Übergabe von JSON-Code oder einer Datei für alle Parameter zulassen</span><span class="sxs-lookup"><span data-stu-id="78b41-892">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="78b41-893">Inkrementierte API-Version</span><span class="sxs-lookup"><span data-stu-id="78b41-893">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="78b41-894">SQL</span><span class="sxs-lookup"><span data-stu-id="78b41-894">SQL</span></span>

* <span data-ttu-id="78b41-895">Befehle vom Typ `sql server vnet-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-895">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="78b41-896">VM</span><span class="sxs-lookup"><span data-stu-id="78b41-896">VM</span></span>

* <span data-ttu-id="78b41-897">Behoben: Zugriff nur zuweisen, wenn `--scope` angegeben wird</span><span class="sxs-lookup"><span data-stu-id="78b41-897">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="78b41-898">Behoben: Gleiche Erweiterungsbenennung wie Portal verwenden</span><span class="sxs-lookup"><span data-stu-id="78b41-898">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="78b41-899">`subscription` aus der Ausgabe von `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="78b41-899">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="78b41-900">Behoben: Speicher-SKU vom Typ `[vm|vmss] create` wird nicht auf Datenträger mit einem Image angewendet.</span><span class="sxs-lookup"><span data-stu-id="78b41-900">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="78b41-901">Behoben: `vm format-secret --secrets` akzeptierte keine durch neue Zeilen getrennte IDs.</span><span class="sxs-lookup"><span data-stu-id="78b41-901">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="78b41-902">31. August 2017</span><span class="sxs-lookup"><span data-stu-id="78b41-902">August 31, 2017</span></span>

<span data-ttu-id="78b41-903">Version 2.0.16</span><span class="sxs-lookup"><span data-stu-id="78b41-903">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="78b41-904">KeyVault</span><span class="sxs-lookup"><span data-stu-id="78b41-904">Keyvault</span></span>

* <span data-ttu-id="78b41-905">Fehler behoben, der beim Versuch auftrat, die Geheimniscodierung mit `secret download` automatisch aufzulösen</span><span class="sxs-lookup"><span data-stu-id="78b41-905">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="78b41-906">Sf</span><span class="sxs-lookup"><span data-stu-id="78b41-906">Sf</span></span>

* <span data-ttu-id="78b41-907">Alle Befehle wurden durch die Service Fabric-Befehlszeilenschnittstelle (sfctl) ersetzt.</span><span class="sxs-lookup"><span data-stu-id="78b41-907">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="78b41-908">Speicher</span><span class="sxs-lookup"><span data-stu-id="78b41-908">Storage</span></span>

* <span data-ttu-id="78b41-909">Problem behoben, aufgrund dessen Speicherkonten nicht in Regionen erstellt werden konnten, die die NetworkACLs-Funktion nicht unterstützen</span><span class="sxs-lookup"><span data-stu-id="78b41-909">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="78b41-910">Festlegen des Inhaltstyps und der Inhaltscodierung während Blob- und Dateiuploads, wenn weder Inhaltstyp noch Inhaltscodierung angegeben sind</span><span class="sxs-lookup"><span data-stu-id="78b41-910">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="78b41-911">28. August 2017</span><span class="sxs-lookup"><span data-stu-id="78b41-911">August 28, 2017</span></span>

<span data-ttu-id="78b41-912">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="78b41-912">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="78b41-913">Befehlszeilenschnittstelle (CLI)</span><span class="sxs-lookup"><span data-stu-id="78b41-913">CLI</span></span>

* <span data-ttu-id="78b41-914">Rechtlichen Hinweis zu `--version` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-914">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="78b41-915">ACS</span><span class="sxs-lookup"><span data-stu-id="78b41-915">ACS</span></span>

* <span data-ttu-id="78b41-916">Vorschauregionen korrigiert</span><span class="sxs-lookup"><span data-stu-id="78b41-916">Corrected preview regions</span></span>
* <span data-ttu-id="78b41-917">Standardmäßiges DNS-Namenspräfix (`dns_name_prefix`) ordnungsgemäß formatiert</span><span class="sxs-lookup"><span data-stu-id="78b41-917">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="78b41-918">ACS-Befehlsausgabe optimiert</span><span class="sxs-lookup"><span data-stu-id="78b41-918">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="78b41-919">AppService</span><span class="sxs-lookup"><span data-stu-id="78b41-919">Appservice</span></span>

* <span data-ttu-id="78b41-920">[WICHTIGE ÄNDERUNG] Inkonsistenzen in der Ausgabe von `az webapp config appsettings [delete|set]` behoben</span><span class="sxs-lookup"><span data-stu-id="78b41-920">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="78b41-921">Neuen Alias (`-i`) für `az webapp config container set --docker-custom-image-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-921">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="78b41-922">`az webapp log show` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="78b41-922">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="78b41-923">Neue Argumente aus `az webapp delete` verfügbar gemacht, um App Service-Plan, Metriken oder DNS-Registrierung beizubehalten</span><span class="sxs-lookup"><span data-stu-id="78b41-923">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="78b41-924">Behoben: Korrekte Erkennung der Sloteinstellungen</span><span class="sxs-lookup"><span data-stu-id="78b41-924">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="78b41-925">IoT</span><span class="sxs-lookup"><span data-stu-id="78b41-925">IoT</span></span>

* <span data-ttu-id="78b41-926">Behoben (3934): Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="78b41-926">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="78b41-927">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="78b41-927">Network</span></span>

* <span data-ttu-id="78b41-928">[WICHTIGE ÄNDERUNG] `vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="78b41-928">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="78b41-929">[WICHTIGE ÄNDERUNG] Option `--private-access-services` für `--service-endpoints` in `vnet subnet [create|update]` umbenannt</span><span class="sxs-lookup"><span data-stu-id="78b41-929">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="78b41-930">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-930">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="78b41-931">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-931">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="78b41-932">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-932">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="78b41-933">Profil</span><span class="sxs-lookup"><span data-stu-id="78b41-933">Profile</span></span>

* <span data-ttu-id="78b41-934">`--msi` und `--msi-port` für die Anmeldung mit der Identität eines virtuellen Computers verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="78b41-934">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="78b41-935">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="78b41-935">Service Fabric</span></span>

* <span data-ttu-id="78b41-936">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="78b41-936">Preview release</span></span>
* <span data-ttu-id="78b41-937">Registrierungsbenutzer-/-kennwortregeln für Befehl vereinfacht</span><span class="sxs-lookup"><span data-stu-id="78b41-937">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="78b41-938">Kennwortanforderung für Benutzer trotz Parameterübergabe behoben</span><span class="sxs-lookup"><span data-stu-id="78b41-938">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="78b41-939">Unterstützung für leere Registrierungsanmeldeinformationen (`registry_cred`) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-939">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="78b41-940">Speicher</span><span class="sxs-lookup"><span data-stu-id="78b41-940">Storage</span></span>

* <span data-ttu-id="78b41-941">Festlegen des Blobtarifs ermöglicht</span><span class="sxs-lookup"><span data-stu-id="78b41-941">Enabled setting blob tier</span></span>
* <span data-ttu-id="78b41-942">Argumente `--bypass` und `--default-action` zur Unterstützung von Diensttunneling zu `storage account [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-942">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="78b41-943">Befehle zum Hinzufügen von VNet-Regeln und IP-basierten Regeln zu `storage account network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-943">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="78b41-944">Dienstverschlüsselung durch vom Kunden verwalteten Schlüssel ermöglicht</span><span class="sxs-lookup"><span data-stu-id="78b41-944">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="78b41-945">[WICHTIGE ÄNDERUNG] Option `--encryption` für Befehl `az storage account create and az storage account update` in `--encryption-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="78b41-945">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="78b41-946">Behoben (4220): `az storage account update encryption` – Syntaxkonflikt</span><span class="sxs-lookup"><span data-stu-id="78b41-946">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="78b41-947">VM</span><span class="sxs-lookup"><span data-stu-id="78b41-947">VM</span></span>

* <span data-ttu-id="78b41-948">Problem behoben, aufgrund dessen bei Verwendung von `--instance-id *` zusätzliche, fehlerhafte Informationen für `vmss get-instance-view` angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="78b41-948">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="78b41-949">Unterstützung für `--lb-sku` zu `vmss create` hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="78b41-949">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="78b41-950">Menschliche Namen aus der Administratornamen-Blacklist für `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="78b41-950">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="78b41-951">Problem behoben, aufgrund dessen `[vm|vmss] create` einen Fehler ausgelöst hat, wenn aus einem Image keine Tarifinformationen extrahiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="78b41-951">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="78b41-952">Absturzproblem beim Erstellen einer VMMS-Skalierungsgruppe mit einem internen Lastenausgleich behoben</span><span class="sxs-lookup"><span data-stu-id="78b41-952">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="78b41-953">Problem behoben, aufgrund dessen das Argument `--no-wait` nicht mit `vm availability-set create` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="78b41-953">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="78b41-954">15. August 2017</span><span class="sxs-lookup"><span data-stu-id="78b41-954">August 15, 2017</span></span>

<span data-ttu-id="78b41-955">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="78b41-955">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="78b41-956">ACS</span><span class="sxs-lookup"><span data-stu-id="78b41-956">ACS</span></span>

* <span data-ttu-id="78b41-957">sshMaster0-Portnummer für Kubernetes korrigiert</span><span class="sxs-lookup"><span data-stu-id="78b41-957">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="78b41-958">AppService</span><span class="sxs-lookup"><span data-stu-id="78b41-958">Appservice</span></span>

* <span data-ttu-id="78b41-959">Ausnahme beim Erstellen einer neuen Git-basierten Linux-Web-App behoben</span><span class="sxs-lookup"><span data-stu-id="78b41-959">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="78b41-960">Event Grid</span><span class="sxs-lookup"><span data-stu-id="78b41-960">Event Grid</span></span>

* <span data-ttu-id="78b41-961">SDK-Abhängigkeiten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-961">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="78b41-962">11. August 2017</span><span class="sxs-lookup"><span data-stu-id="78b41-962">August 11, 2017</span></span>

<span data-ttu-id="78b41-963">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="78b41-963">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="78b41-964">ACS</span><span class="sxs-lookup"><span data-stu-id="78b41-964">ACS</span></span>

* <span data-ttu-id="78b41-965">Weitere Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-965">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="78b41-966">Batch</span><span class="sxs-lookup"><span data-stu-id="78b41-966">Batch</span></span>

* <span data-ttu-id="78b41-967">Auf Batch SDK 3.1.0 und Batch Management SDK 4.1.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="78b41-967">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="78b41-968">Neuen Befehl zum Anzeigen der Aufgabenanzahl eines Auftrags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-968">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="78b41-969">Fehler in der SAS-URL-Verarbeitung der Ressourcendatei behoben</span><span class="sxs-lookup"><span data-stu-id="78b41-969">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="78b41-970">Batch-Kontoendpunkt unterstützt nun optionales Präfix „https://“</span><span class="sxs-lookup"><span data-stu-id="78b41-970">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="78b41-971">Unterstützung für das Hinzufügen von Listen mit mehr als 100 Aufgaben zu einem Auftrag</span><span class="sxs-lookup"><span data-stu-id="78b41-971">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="78b41-972">Debugprotokollierung für das Laden des Erweiterungsbefehlsmoduls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-972">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="78b41-973">Komponente</span><span class="sxs-lookup"><span data-stu-id="78b41-973">Component</span></span>

* <span data-ttu-id="78b41-974">Warnung für veraltete Befehle vom Typ „az component“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-974">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="78b41-975">Container</span><span class="sxs-lookup"><span data-stu-id="78b41-975">Container</span></span>

* <span data-ttu-id="78b41-976">`create`: Problem behoben, aufgrund dessen das Gleichheitszeichen innerhalb einer Umgebungsvariablen nicht zulässig war</span><span class="sxs-lookup"><span data-stu-id="78b41-976">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="78b41-977">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="78b41-977">Data Lake Store</span></span>

* <span data-ttu-id="78b41-978">Fortschrittsüberwachung ermöglicht</span><span class="sxs-lookup"><span data-stu-id="78b41-978">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="78b41-979">Event Grid</span><span class="sxs-lookup"><span data-stu-id="78b41-979">Event Grid</span></span>

* <span data-ttu-id="78b41-980">Erste Version</span><span class="sxs-lookup"><span data-stu-id="78b41-980">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="78b41-981">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="78b41-981">Network</span></span>

* <span data-ttu-id="78b41-982">`lb`: Problem behoben, aufgrund dessen bestimmte Namen untergeordneter Ressourcen bei Auslassung nicht ordnungsgemäß aufgelöst wurden</span><span class="sxs-lookup"><span data-stu-id="78b41-982">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="78b41-983">`application-gateway {subresource} delete`: Problem behoben, aufgrund dessen `--no-wait` nicht berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="78b41-983">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="78b41-984">`application-gateway http-settings update`: Problem behoben, aufgrund dessen `--connection-draining-timeout` nicht deaktiviert werden konnte</span><span class="sxs-lookup"><span data-stu-id="78b41-984">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="78b41-985">Fehler behoben: Unerwartetes Schlüsselwortargument `sa_data_size_kilobyes` bei `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="78b41-985">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="78b41-986">Profil</span><span class="sxs-lookup"><span data-stu-id="78b41-986">Profile</span></span>

* <span data-ttu-id="78b41-987">`account list`: `--refresh` hinzugefügt, um die neuesten Abonnements vom Server zu synchronisieren</span><span class="sxs-lookup"><span data-stu-id="78b41-987">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="78b41-988">Speicher</span><span class="sxs-lookup"><span data-stu-id="78b41-988">Storage</span></span>

* <span data-ttu-id="78b41-989">Aktualisieren des Speicherkontos mit vom System zugewiesener Identität ermöglicht</span><span class="sxs-lookup"><span data-stu-id="78b41-989">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="78b41-990">VM</span><span class="sxs-lookup"><span data-stu-id="78b41-990">VM</span></span>

* <span data-ttu-id="78b41-991">`availability-set`: Fehlerdomänenanzahl bei Konvertierung verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="78b41-991">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="78b41-992">Befehl `list-skus` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="78b41-992">Exposed `list-skus` command</span></span>
* <span data-ttu-id="78b41-993">Unterstützung der Identitätszuweisung ohne Erstellung von Rollenzuweisungen</span><span class="sxs-lookup"><span data-stu-id="78b41-993">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="78b41-994">Anwenden von Speicher-SKU beim Anfügen von Datenträgern</span><span class="sxs-lookup"><span data-stu-id="78b41-994">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="78b41-995">Standardmäßiger Betriebssystemdatenträger-Name und Speicher-SKU bei Verwendung verwalteter Datenträger entfernt</span><span class="sxs-lookup"><span data-stu-id="78b41-995">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="78b41-996">28. Juli 2017</span><span class="sxs-lookup"><span data-stu-id="78b41-996">July 28, 2017</span></span>

<span data-ttu-id="78b41-997">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="78b41-997">Version 2.0.12</span></span>

* <span data-ttu-id="78b41-998">Containerbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-998">Added container commands</span></span>
* <span data-ttu-id="78b41-999">Abrechnungs- und Nutzungsmodule hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-999">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="78b41-1000">Core</span><span class="sxs-lookup"><span data-stu-id="78b41-1000">Core</span></span>

* <span data-ttu-id="78b41-1001">Ausgabe von SDK-Authentifizierungsinformationen für Dienstprinzipale mit Zertifikaten</span><span class="sxs-lookup"><span data-stu-id="78b41-1001">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="78b41-1002">Ausnahmen beim Bereitstellungsfortschritt behoben</span><span class="sxs-lookup"><span data-stu-id="78b41-1002">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="78b41-1003">Verwendung des ARM-Endpunkts aus der aktuellen Cloud für die Erstellung des Abonnementclients</span><span class="sxs-lookup"><span data-stu-id="78b41-1003">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="78b41-1004">Gleichzeitige Verarbeitung der Datei „clouds.config“ verbessert (3636)</span><span class="sxs-lookup"><span data-stu-id="78b41-1004">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="78b41-1005">Aktualisierung der Clientanforderungs-ID für jede Befehlsausführung</span><span class="sxs-lookup"><span data-stu-id="78b41-1005">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="78b41-1006">Erstellung von Abonnementclients mit richtigem SDK-Profil (3635)</span><span class="sxs-lookup"><span data-stu-id="78b41-1006">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="78b41-1007">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="78b41-1007">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="78b41-1008">Unterstützung für Auswahl von Tabellenausgabefeldern über jmespath Abfrage hinzugefügt (3581)</span><span class="sxs-lookup"><span data-stu-id="78b41-1008">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="78b41-1009">Stummschaltung von Analyseargumenten und Anfügeverlauf mit Gesten verbessert (3434)</span><span class="sxs-lookup"><span data-stu-id="78b41-1009">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="78b41-1010">Erstellung von Abonnementclients mit richtigem SDK-Profil</span><span class="sxs-lookup"><span data-stu-id="78b41-1010">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="78b41-1011">Verschiebung aller vorhandenen Erfassungsdateien in den neuesten Ordner</span><span class="sxs-lookup"><span data-stu-id="78b41-1011">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="78b41-1012">Idempotenz für VM-/VMSS-Erstellung behoben (3586)</span><span class="sxs-lookup"><span data-stu-id="78b41-1012">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="78b41-1013">Bei Befehlspfaden wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="78b41-1013">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="78b41-1014">Bei bestimmten booleschen Parametern wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="78b41-1014">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="78b41-1015">Unterstützung der Anmeldung bei lokalem AD FS-Server wie Azure Stack</span><span class="sxs-lookup"><span data-stu-id="78b41-1015">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="78b41-1016">Gleichzeitige Schreibvorgänge in „clouds.config“ behoben (3255)</span><span class="sxs-lookup"><span data-stu-id="78b41-1016">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="78b41-1017">ACR</span><span class="sxs-lookup"><span data-stu-id="78b41-1017">ACR</span></span>

* <span data-ttu-id="78b41-1018">Befehl `show-usage` für verwaltete Registrierungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-1018">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="78b41-1019">Unterstützung der SKU-Aktualisierung für verwaltete Registrierungen</span><span class="sxs-lookup"><span data-stu-id="78b41-1019">Support SKU update for managed registries</span></span>
* <span data-ttu-id="78b41-1020">Verwaltete Registrierungen mit verwalteter SKU hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-1020">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="78b41-1021">Webhooks für verwaltete Registrierungen mit ACR-Webhook-Befehlsmodul hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-1021">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="78b41-1022">AAD-Authentifizierung mit ACR-Anmeldebefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-1022">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="78b41-1023">Löschbefehl für Docker-Repositorys, Manifeste und Tags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-1023">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="78b41-1024">ACS</span><span class="sxs-lookup"><span data-stu-id="78b41-1024">ACS</span></span>

* <span data-ttu-id="78b41-1025">Unterstützung der API-Version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="78b41-1025">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="78b41-1026">AppService</span><span class="sxs-lookup"><span data-stu-id="78b41-1026">Appservice</span></span>

* <span data-ttu-id="78b41-1027">Fehler behoben, aufgrund dessen die Auflistung der Linux-Web-App keine Werte zurückgegeben hat</span><span class="sxs-lookup"><span data-stu-id="78b41-1027">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="78b41-1028">Unterstützung für das Abrufen von Anmeldeinformationen aus dem ACR</span><span class="sxs-lookup"><span data-stu-id="78b41-1028">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="78b41-1029">Entfernung aller Befehle unter `appservice web`</span><span class="sxs-lookup"><span data-stu-id="78b41-1029">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="78b41-1030">Maskierung von Docker-Registrierungskennwörtern aus der Befehlsausgabe (3656)</span><span class="sxs-lookup"><span data-stu-id="78b41-1030">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="78b41-1031">Gewährleistung der fehlerfreien Verwendung des Standardbrowsers unter macOS (3623)</span><span class="sxs-lookup"><span data-stu-id="78b41-1031">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="78b41-1032">Verbesserung des Nutzens von `webapp log tail` und `webapp log download` (3624)</span><span class="sxs-lookup"><span data-stu-id="78b41-1032">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="78b41-1033">Befehl `traffic-routing` zum Konfigurieren des statischen Routings verfügbar gemacht (3566)</span><span class="sxs-lookup"><span data-stu-id="78b41-1033">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="78b41-1034">Zuverlässigkeit beim Konfigurieren der Quellcodeverwaltung verbessert (3245)</span><span class="sxs-lookup"><span data-stu-id="78b41-1034">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="78b41-1035">Nicht unterstütztes Argument `--node-version` aus `webapp config update` für Windows-Web-Apps entfernt.</span><span class="sxs-lookup"><span data-stu-id="78b41-1035">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="78b41-1036">Verwenden Sie stattdessen `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="78b41-1036">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="78b41-1037">Batch</span><span class="sxs-lookup"><span data-stu-id="78b41-1037">Batch</span></span>

* <span data-ttu-id="78b41-1038">Auf Batch SDK 3.0.0 mit Unterstützung virtueller Computer mit niedriger Priorität in Pools aktualisiert</span><span class="sxs-lookup"><span data-stu-id="78b41-1038">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="78b41-1039">`pool create`-Option `--target-dedicated` in `--target-dedicated-nodes` umbenannt</span><span class="sxs-lookup"><span data-stu-id="78b41-1039">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="78b41-1040">`pool create`-Optionen `--target-low-priority-nodes` und `--application-licenses` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-1040">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="78b41-1041">CDN</span><span class="sxs-lookup"><span data-stu-id="78b41-1041">CDN</span></span>

* <span data-ttu-id="78b41-1042">Besser verständliche Fehlermeldung für `cdn endpoint list`, wenn das von `--profile-name` angegebene Profil nicht vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="78b41-1042">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="78b41-1043">Cloud</span><span class="sxs-lookup"><span data-stu-id="78b41-1043">Cloud</span></span>

* <span data-ttu-id="78b41-1044">API-Version des Cloudmetadaten-Endpunkts in das Format JJJJ-MM-TT umgewandelt</span><span class="sxs-lookup"><span data-stu-id="78b41-1044">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="78b41-1045">Katalogendpunkt nicht erforderlich</span><span class="sxs-lookup"><span data-stu-id="78b41-1045">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="78b41-1046">Unterstützung für die Cloudregistrierung nur mit ARM-Endpunkt</span><span class="sxs-lookup"><span data-stu-id="78b41-1046">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="78b41-1047">Option für `cloud set` bereitgestellt, um beim Auswählen der aktuellen Cloud das Profil auswählen zu können</span><span class="sxs-lookup"><span data-stu-id="78b41-1047">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="78b41-1048">`endpoint_vm_image_alias_doc` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="78b41-1048">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="78b41-1049">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="78b41-1049">CosmosDB</span></span>

* <span data-ttu-id="78b41-1050">Möglichkeit zum Erstellen einer Auflistung mit benutzerdefiniertem Partitionsschlüssel behoben</span><span class="sxs-lookup"><span data-stu-id="78b41-1050">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="78b41-1051">Unterstützung für Auflistungs-Standardgültigkeitsdauer hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-1051">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="78b41-1052">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="78b41-1052">Data Lake Analytics</span></span>

* <span data-ttu-id="78b41-1053">Zusätzliche Befehle für Compute-Richtlinienverwaltung unter der Überschrift `dla account compute-policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-1053">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="78b41-1054">`dla job pipeline show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-1054">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="78b41-1055">`dla job recurrence list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-1055">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="78b41-1056">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="78b41-1056">Data Lake Store</span></span>

* <span data-ttu-id="78b41-1057">Unterstützung für vom Benutzer verwaltete Schlüsseltresor-Schlüsselrotation in `dls account update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-1057">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="78b41-1058">Zugrunde liegende SDK-Version des Data Lake Store-Dateisystems aktualisiert, um ein Leistungsproblem zu behandeln</span><span class="sxs-lookup"><span data-stu-id="78b41-1058">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="78b41-1059">Befehl `dls enable-key-vault` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="78b41-1059">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="78b41-1060">Dieser Befehl versucht, eine vom Benutzer angegebene Key Vault-Instanz zur Verschlüsselung der Daten in einem Data Lake Store-Konto zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="78b41-1060">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="78b41-1061">Interaktiv</span><span class="sxs-lookup"><span data-stu-id="78b41-1061">Interactive</span></span>

* <span data-ttu-id="78b41-1062">Startzeit durch Verwendung zwischengespeicherter Befehle verbessert</span><span class="sxs-lookup"><span data-stu-id="78b41-1062">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="78b41-1063">Testabdeckung verbessert</span><span class="sxs-lookup"><span data-stu-id="78b41-1063">Increased test coverage</span></span>
* <span data-ttu-id="78b41-1064">?-Geste erweitert, sodass sie auch in den nächsten Befehl eingefügt wird</span><span class="sxs-lookup"><span data-stu-id="78b41-1064">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="78b41-1065">Interaktive Fehler mit dem Profil „2017-03-09-profile-preview“ behoben (3587)</span><span class="sxs-lookup"><span data-stu-id="78b41-1065">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="78b41-1066">`--version` als Parameter für den interaktiven Modus zugelassen (3645)</span><span class="sxs-lookup"><span data-stu-id="78b41-1066">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="78b41-1067">Beseitigung von Fehlern im interaktiven Modus beim Abschluss von Überprüfungen (3570)</span><span class="sxs-lookup"><span data-stu-id="78b41-1067">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="78b41-1068">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="78b41-1068">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="78b41-1069">Flag `--progress` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-1069">Added `--progress` flag</span></span>
* <span data-ttu-id="78b41-1070">`--debug` und `--verbose` aus Abschlüssen entfernt</span><span class="sxs-lookup"><span data-stu-id="78b41-1070">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="78b41-1071">`interactive` aus Abschlüssen entfernt (3324)</span><span class="sxs-lookup"><span data-stu-id="78b41-1071">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="78b41-1072">IoT</span><span class="sxs-lookup"><span data-stu-id="78b41-1072">IoT</span></span>

* <span data-ttu-id="78b41-1073">Behoben: Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="78b41-1073">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="78b41-1074">(3934)</span><span class="sxs-lookup"><span data-stu-id="78b41-1074">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="78b41-1075">Schlüsseltresor</span><span class="sxs-lookup"><span data-stu-id="78b41-1075">Key vault</span></span>

* <span data-ttu-id="78b41-1076">Befehle für Schlüsseltresor-Wiederherstellungsfeatures hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="78b41-1076">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="78b41-1077">`keyvault`-Unterbefehle: `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="78b41-1077">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="78b41-1078">`keyvault secret`-Unterbefehle: `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="78b41-1078">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="78b41-1079">`keyvault certificate`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="78b41-1079">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="78b41-1080">`keyvault key`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="78b41-1080">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="78b41-1081">Dienstprinzipal-Schlüsseltresorintegration hinzugefügt (3133)</span><span class="sxs-lookup"><span data-stu-id="78b41-1081">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="78b41-1082">Schlüsseltresor-Datenebene auf 0.3.2. aktualisiert</span><span class="sxs-lookup"><span data-stu-id="78b41-1082">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="78b41-1083">(3307)</span><span class="sxs-lookup"><span data-stu-id="78b41-1083">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="78b41-1084">Labor</span><span class="sxs-lookup"><span data-stu-id="78b41-1084">Lab</span></span>

* <span data-ttu-id="78b41-1085">Unterstützung für Übernahme eines beliebigen virtuellen Computers im Labor über `az lab vm claim` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-1085">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="78b41-1086">Tabellenausgabeformatierer für `az lab vm list` und `az lab vm show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-1086">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="78b41-1087">Überwachen</span><span class="sxs-lookup"><span data-stu-id="78b41-1087">Monitor</span></span>

* <span data-ttu-id="78b41-1088">Korrektur für Vorlagendatei mit Befehl `monitor autoscale-settings get-parameters-template` (3349)</span><span class="sxs-lookup"><span data-stu-id="78b41-1088">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="78b41-1089">`monitor alert-rule-incidents list` in `monitor alert list-incidents` umbenannt</span><span class="sxs-lookup"><span data-stu-id="78b41-1089">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="78b41-1090">`monitor alert-rule-incidents show` in `monitor alert show-incident` umbenannt</span><span class="sxs-lookup"><span data-stu-id="78b41-1090">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="78b41-1091">`monitor metric-defintions list` in `monitor metrics list-definitions` umbenannt</span><span class="sxs-lookup"><span data-stu-id="78b41-1091">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="78b41-1092">`monitor alert-rules` in `monitor alert` umbenannt</span><span class="sxs-lookup"><span data-stu-id="78b41-1092">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="78b41-1093">`monitor alert create` geändert:</span><span class="sxs-lookup"><span data-stu-id="78b41-1093">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="78b41-1094">Unterbefehle vom Typ `condition` und `action` akzeptieren keinen JSON-Code mehr.</span><span class="sxs-lookup"><span data-stu-id="78b41-1094">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="78b41-1095">Hinzufügung zahlreicher Parameter zur Vereinfachung der Regelerstellung</span><span class="sxs-lookup"><span data-stu-id="78b41-1095">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="78b41-1096">`location` nicht mehr erforderlich</span><span class="sxs-lookup"><span data-stu-id="78b41-1096">`location` no longer required</span></span>
  * <span data-ttu-id="78b41-1097">Hinzufügung von Namen- und ID-Unterstützung für Ziel</span><span class="sxs-lookup"><span data-stu-id="78b41-1097">Add name and ID support for target</span></span>
  * <span data-ttu-id="78b41-1098">Entfernung von `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="78b41-1098">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="78b41-1099">Umbenennung von `is-enabled` in `enabled` (nicht mehr erforderlich)</span><span class="sxs-lookup"><span data-stu-id="78b41-1099">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="78b41-1100">`description` wird nun abhängig von der angegebenen Bedingung auf einen Standardwert festgelegt.</span><span class="sxs-lookup"><span data-stu-id="78b41-1100">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="78b41-1101">Hinzufügung von Beispielen zur Verdeutlichung des neuen Formats</span><span class="sxs-lookup"><span data-stu-id="78b41-1101">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="78b41-1102">Unterstützung von Namen oder IDs für Befehle vom Typ `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="78b41-1102">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="78b41-1103">Komfortargumente und Beispiele zu `monitor alert rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-1103">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="78b41-1104">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="78b41-1104">Network</span></span>

* <span data-ttu-id="78b41-1105">Befehl `list-private-access-services` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-1105">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="78b41-1106">Argument `--private-access-services` zu `vnet subnet create` und `vnet subnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-1106">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="78b41-1107">Problem behoben, das einen Fehler für `application-gateway redirect-config create` zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="78b41-1107">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="78b41-1108">Problem behoben, aufgrund dessen `application-gateway redirect-config update` nicht mit `--no-wait` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="78b41-1108">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="78b41-1109">Fehler behoben, der bei der Verwendung des Arguments `--servers` mit `application-gateway address-pool create` und `application-gateway address-pool update` aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="78b41-1109">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="78b41-1110">Befehle vom Typ `application-gateway redirect-config` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-1110">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="78b41-1111">Befehle zu `application-gateway ssl-policy` hinzugefügt: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="78b41-1111">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="78b41-1112">Argumente zu `application-gateway ssl-policy set` hinzugefügt: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="78b41-1112">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="78b41-1113">Argumente zu `application-gateway http-settings create` und `application-gateway http-settings update` hinzugefügt: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="78b41-1113">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="78b41-1114">Argumente zu `application-gateway url-path-map create` und `application-gateway url-path-map update` hinzugefügt: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="78b41-1114">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="78b41-1115">Argument `--redirect-config` zu `application-gateway url-path-map rule create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-1115">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="78b41-1116">Unterstützung für `--no-wait` zu `application-gateway url-path-map rule delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-1116">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="78b41-1117">Argumente zu `application-gateway probe create` und `application-gateway probe update` hinzugefügt: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="78b41-1117">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="78b41-1118">Argument `--redirect-config` zu `application-gateway rule create` und `application-gateway rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-1118">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="78b41-1119">Unterstützung für `--accelerated-networking` zu `nic create` und `nic update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-1119">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="78b41-1120">Argument `--internal-dns-name-suffix` von `nic create` entfernt</span><span class="sxs-lookup"><span data-stu-id="78b41-1120">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="78b41-1121">Unterstützung für `--dns-servers` zu `nic update` und `nic create` hinzugefügt: Unterstützung für „--dns-servers“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-1121">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="78b41-1122">Fehler korrigiert, aufgrund dessen `--local-address-prefixes` von `local-gateway create` ignoriert wurde</span><span class="sxs-lookup"><span data-stu-id="78b41-1122">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="78b41-1123">Unterstützung für `--dns-servers` zu `vnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-1123">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="78b41-1124">Fehler beim Erstellen eines Peerings ohne Routenfilterung mit `express-route peering create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="78b41-1124">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="78b41-1125">Fehler korrigiert, aufgrund dessen die Argumente `--provider` und `--bandwidth` nicht mit `express-route update` verwendet werden konnten</span><span class="sxs-lookup"><span data-stu-id="78b41-1125">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="78b41-1126">Fehler mit Standardlogik von `network watcher show-topology` korrigiert</span><span class="sxs-lookup"><span data-stu-id="78b41-1126">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="78b41-1127">Ausgabeformatierung für `network list-usages` verbessert</span><span class="sxs-lookup"><span data-stu-id="78b41-1127">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="78b41-1128">Verwendung der standardmäßigen Front-End-IP-Adresse für `application-gateway http-listener create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="78b41-1128">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="78b41-1129">Verwendung des Standardadresspools, der HTTP-Standardeinstellungen und des HTTP-Standardlisteners für `application-gateway rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="78b41-1129">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="78b41-1130">Verwendung der standardmäßigen Front-End-IP-Adresse und des standardmäßigen Back-End-Pools für `lb rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="78b41-1130">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="78b41-1131">Verwendung der standardmäßigen Front-End-IP-Adresse für `lb inbound-nat-rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="78b41-1131">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="78b41-1132">Profil</span><span class="sxs-lookup"><span data-stu-id="78b41-1132">Profile</span></span>

* <span data-ttu-id="78b41-1133">Unterstützung der Anmeldung innerhalb eines virtuellen Computers mit einer verwalteten Identität</span><span class="sxs-lookup"><span data-stu-id="78b41-1133">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="78b41-1134">Unterstützung der Ausgabe für `account show` im SDK-Authentifizierungsdateiformat</span><span class="sxs-lookup"><span data-stu-id="78b41-1134">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="78b41-1135">Anzeige von Warnungen für veraltete Befehle bei Verwendung von „--expanded-view“</span><span class="sxs-lookup"><span data-stu-id="78b41-1135">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="78b41-1136">Befehl `get-access-token` für die Bereitstellung eines unformatierten AAD-Tokens hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-1136">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="78b41-1137">Unterstützung der Anmeldung mit einem Benutzerkonto ohne zugeordnete Abonnements</span><span class="sxs-lookup"><span data-stu-id="78b41-1137">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="78b41-1138">RDBMS</span><span class="sxs-lookup"><span data-stu-id="78b41-1138">RDBMS</span></span>

* <span data-ttu-id="78b41-1139">Unterstützung der abonnementübergreifenden Auflistung von Servern (3417)</span><span class="sxs-lookup"><span data-stu-id="78b41-1139">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="78b41-1140">Behoben: `%s` wird aufgrund von fehlendem `% server_type` nicht verarbeitet (3393)</span><span class="sxs-lookup"><span data-stu-id="78b41-1140">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="78b41-1141">Dokumentquellenzuordnung behoben und CI-Aufgabe zur Überprüfung hinzugefügt (3361)</span><span class="sxs-lookup"><span data-stu-id="78b41-1141">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="78b41-1142">MySQL- und PostgreSQL-Hilfe korrigiert (3369)</span><span class="sxs-lookup"><span data-stu-id="78b41-1142">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="78b41-1143">Ressource</span><span class="sxs-lookup"><span data-stu-id="78b41-1143">Resource</span></span>

* <span data-ttu-id="78b41-1144">Eingabeaufforderungen bei fehlenden Parametern für `group deployment create` verbessert</span><span class="sxs-lookup"><span data-stu-id="78b41-1144">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="78b41-1145">Analyse der Syntax `--parameters KEY=VALUE` verbessert</span><span class="sxs-lookup"><span data-stu-id="78b41-1145">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="78b41-1146">Probleme behoben, durch die Parameterdateien von `group deployment create` bei Verwendung der Syntax `@<file>` nicht mehr erkannt wurden</span><span class="sxs-lookup"><span data-stu-id="78b41-1146">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="78b41-1147">Unterstützung des Arguments `--ids` für Befehle vom Typ `resource` und `managedapp`</span><span class="sxs-lookup"><span data-stu-id="78b41-1147">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="78b41-1148">Einige Analyse- und Fehlermeldungen korrigiert (3584)</span><span class="sxs-lookup"><span data-stu-id="78b41-1148">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="78b41-1149">Analyse vom Typ `--resource-type` für den Befehl `lock` korrigiert, sodass `<resource-namespace>` und `<resource-type>` akzeptiert werden</span><span class="sxs-lookup"><span data-stu-id="78b41-1149">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="78b41-1150">Parameterüberprüfung für Vorlagenlinkvorlagen hinzugefügt (3629)</span><span class="sxs-lookup"><span data-stu-id="78b41-1150">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="78b41-1151">Unterstützung für die Angabe von Bereitstellungsparametern mit der Syntax `KEY=VALUE` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-1151">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="78b41-1152">Rolle</span><span class="sxs-lookup"><span data-stu-id="78b41-1152">Role</span></span>

* <span data-ttu-id="78b41-1153">Unterstützung der Ausgabe im SDK-Authentifizierungsdateiformat für `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="78b41-1153">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="78b41-1154">Rollenzuweisungen und dazugehörige AAD-Anwendung beim Löschen eines Dienstprinzipals bereinigt (3610)</span><span class="sxs-lookup"><span data-stu-id="78b41-1154">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="78b41-1155">Einbeziehung des Zeitformats in Beschreibungen vom Typ `--start-date` und `--end-date` für `app create`-Argumente</span><span class="sxs-lookup"><span data-stu-id="78b41-1155">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="78b41-1156">Anzeige von Warnungen für veraltete Befehle bei Verwendung von `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="78b41-1156">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="78b41-1157">Schlüsseltresorintegration zu den Befehlen `create-for-rbac` und `reset-credentials` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-1157">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="78b41-1158">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="78b41-1158">Service Fabric</span></span>
* <span data-ttu-id="78b41-1159">Problem behoben, aufgrund dessen große Dateien in Anwendungen beim Hochladen gekürzt wurden (3666)</span><span class="sxs-lookup"><span data-stu-id="78b41-1159">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="78b41-1160">Tests für Service Fabric-Befehle hinzugefügt (3424)</span><span class="sxs-lookup"><span data-stu-id="78b41-1160">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="78b41-1161">Zahlreiche Service Fabric-Befehle korrigiert (3234)</span><span class="sxs-lookup"><span data-stu-id="78b41-1161">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="78b41-1162">SQL</span><span class="sxs-lookup"><span data-stu-id="78b41-1162">SQL</span></span>

* <span data-ttu-id="78b41-1163">Fehlerhaften Parameter `--identity` für `sql server create` entfernt</span><span class="sxs-lookup"><span data-stu-id="78b41-1163">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="78b41-1164">Kennwortwerte aus der Befehlsausgabe von `sql server create` und `sql server update` entfernt</span><span class="sxs-lookup"><span data-stu-id="78b41-1164">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="78b41-1165">Befehle `sql db list-editions` und `sql elastic-pool list-editions` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-1165">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="78b41-1166">Speicher</span><span class="sxs-lookup"><span data-stu-id="78b41-1166">Storage</span></span>

* <span data-ttu-id="78b41-1167">Option `--marker` für die Befehle `storage blob list`, `storage container list` und `storage share list` entfernt (3745)</span><span class="sxs-lookup"><span data-stu-id="78b41-1167">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="78b41-1168">Erstellung eines reinen HTTPS-Speicherkontos ermöglicht</span><span class="sxs-lookup"><span data-stu-id="78b41-1168">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="78b41-1169">Speichermetriken, Protokollierung und CORS-Befehle aktualisiert (3495)</span><span class="sxs-lookup"><span data-stu-id="78b41-1169">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="78b41-1170">Ausnahmemeldung von „cors add“ umformuliert (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="78b41-1170">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="78b41-1171">Generator im Probelaufmodus des Downloadbatchbefehls in eine Liste konvertiert (3592)</span><span class="sxs-lookup"><span data-stu-id="78b41-1171">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="78b41-1172">Problem bei Probelauf des Blobdownloadbatchs behoben (3640) (3592)</span><span class="sxs-lookup"><span data-stu-id="78b41-1172">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="78b41-1173">VM</span><span class="sxs-lookup"><span data-stu-id="78b41-1173">VM</span></span>

* <span data-ttu-id="78b41-1174">Unterstützung der NSG-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="78b41-1174">Support configuring nsg</span></span>
* <span data-ttu-id="78b41-1175">Fehler behoben, aufgrund dessen der DNS-Server nicht ordnungsgemäß konfiguriert wurde</span><span class="sxs-lookup"><span data-stu-id="78b41-1175">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="78b41-1176">Unterstützung verwalteter Dienstidentitäten</span><span class="sxs-lookup"><span data-stu-id="78b41-1176">Support managed service identities</span></span>
* <span data-ttu-id="78b41-1177">Problem behoben, aufgrund dessen `cmss create` mit einem vorhandenen Lastenausgleich `--backend-pool-name` benötigte</span><span class="sxs-lookup"><span data-stu-id="78b41-1177">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="78b41-1178">Festlegung, dass die LUN von mit `vm image create` erstellten Datenträgern mit 0 beginnt</span><span class="sxs-lookup"><span data-stu-id="78b41-1178">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="78b41-1179">10. Mai 2017</span><span class="sxs-lookup"><span data-stu-id="78b41-1179">May 10, 2017</span></span>

<span data-ttu-id="78b41-1180">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="78b41-1180">Version 2.0.6</span></span>

* <span data-ttu-id="78b41-1181">Umbenennen von „documentdb“ in „cosmosdb“</span><span class="sxs-lookup"><span data-stu-id="78b41-1181">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="78b41-1182">Hinzufügen von rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="78b41-1182">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="78b41-1183">Einbeziehen der Data Lake Analytics- und Data Lake Store-Module</span><span class="sxs-lookup"><span data-stu-id="78b41-1183">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="78b41-1184">Einbeziehen des Cognitive Services-Moduls</span><span class="sxs-lookup"><span data-stu-id="78b41-1184">Include Cognitive Services module</span></span>
* <span data-ttu-id="78b41-1185">Einbeziehen des Service Fabric-Moduls</span><span class="sxs-lookup"><span data-stu-id="78b41-1185">Include Service Fabric module</span></span>
* <span data-ttu-id="78b41-1186">Einbeziehen des interaktiven Moduls (Umbenennen von „az-shell“)</span><span class="sxs-lookup"><span data-stu-id="78b41-1186">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="78b41-1187">Hinzufügen von Unterstützung für CDN-Befehle</span><span class="sxs-lookup"><span data-stu-id="78b41-1187">Add support for CDN commands</span></span>
* <span data-ttu-id="78b41-1188">Entfernen des Containermoduls</span><span class="sxs-lookup"><span data-stu-id="78b41-1188">Remove Container module</span></span>
* <span data-ttu-id="78b41-1189">Hinzufügen von „az -v“ als Verknüpfung für „az --version“ ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="78b41-1189">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="78b41-1190">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="78b41-1190">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="78b41-1191">Core</span><span class="sxs-lookup"><span data-stu-id="78b41-1191">Core</span></span>

* <span data-ttu-id="78b41-1192">Core: Erfassen von Ausnahmen, die durch einen nicht registrierten Anbieter verursacht werden, und automatische Registrierung</span><span class="sxs-lookup"><span data-stu-id="78b41-1192">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="78b41-1193">Leistung: Dauerhaftes Speichern des ADAL-Tokencaches im Arbeitsspeicher bis zum Prozessende ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="78b41-1193">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="78b41-1194">Korrigieren der vom hexadezimalen Fingerabdruck -o tsv zurückgegebenen Bytes ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="78b41-1194">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="78b41-1195">Verbessern des Downloads des Schlüsseltresorzertifikats und der AAD-SP-Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="78b41-1195">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="78b41-1196">Hinzufügen des Python-Speicherorts zu „az –version“ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="78b41-1196">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="78b41-1197">Anmeldung: Unterstützung der Anmeldung, wenn keine Abonnements vorhanden sind ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="78b41-1197">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="78b41-1198">Core: Beheben eines Fehlers bei zweimaliger Verwendung eines Dienstprinzipals bei der Anmeldung ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="78b41-1198">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="78b41-1199">Core: Ermöglichen der Konfiguration des Dateipfads von „accessTokens.json“ über eine Umgebungsvariable ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="78b41-1199">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="78b41-1200">Core: Zulassen der Anwendung konfigurierter Standardwerte auf optionale Argumente ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="78b41-1200">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="78b41-1201">Core: Verbesserte Leistung</span><span class="sxs-lookup"><span data-stu-id="78b41-1201">core: Improved performance</span></span>
* <span data-ttu-id="78b41-1202">Core: Zertifikate von benutzerdefinierter Zertifizierungsstelle – Unterstützung für das Festlegen der REQUESTS_CA_BUNDLE-Umgebungsvariablen</span><span class="sxs-lookup"><span data-stu-id="78b41-1202">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="78b41-1203">Core: Cloudkonfiguration – Verwenden des Endpunkts „resource manager“, wenn Endpunkt „management“ nicht festgelegt ist</span><span class="sxs-lookup"><span data-stu-id="78b41-1203">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="78b41-1204">ACS</span><span class="sxs-lookup"><span data-stu-id="78b41-1204">ACS</span></span>

* <span data-ttu-id="78b41-1205">Korrigieren der Master- und Agentanzahl als ganze Zahl statt Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="78b41-1205">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="78b41-1206">Verfügbarmachen von „az acs create --no-wait“ und „az acs wait“ für die asynchrone Erstellung</span><span class="sxs-lookup"><span data-stu-id="78b41-1206">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="78b41-1207">Verfügbarmachen von „az acs create --validate“ für Probelaufüberprüfungen</span><span class="sxs-lookup"><span data-stu-id="78b41-1207">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="78b41-1208">Entfernen von Windows-Profil vor PUT-Aufruf für Skalierungsbefehl ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="78b41-1208">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="78b41-1209">AppService</span><span class="sxs-lookup"><span data-stu-id="78b41-1209">AppService</span></span>

* <span data-ttu-id="78b41-1210">functionapp: Hinzufügen der vollständigen functionapp-Unterstützung, einschließlich Erstellen, Anzeigen, Auflisten, Löschen, Hostname, SSL usw.</span><span class="sxs-lookup"><span data-stu-id="78b41-1210">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="78b41-1211">Hinzufügen von Team Services (vsts) als Continuous Delivery-Option zu „appservice web source-control config“</span><span class="sxs-lookup"><span data-stu-id="78b41-1211">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="78b41-1212">Erstellen von „az webapp“ als Ersatz für „az appservice web“ (für Abwärtskompatibilität bleibt „az appservice web“ für 2 weitere Releases erhalten)</span><span class="sxs-lookup"><span data-stu-id="78b41-1212">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="78b41-1213">Verfügbarmachen von Argumenten zum Konfigurieren von Bereitstellung und Laufzeitstapeln beim Erstellen von Web-Apps</span><span class="sxs-lookup"><span data-stu-id="78b41-1213">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="78b41-1214">Verfügbarmachen von „webapp list-runtimes“</span><span class="sxs-lookup"><span data-stu-id="78b41-1214">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="78b41-1215">Unterstützen der Konfiguration von Verbindungszeichenfolgen ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="78b41-1215">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="78b41-1216">Unterstützen des Slottauschs mit Vorschau</span><span class="sxs-lookup"><span data-stu-id="78b41-1216">support slot swap with preview</span></span>
* <span data-ttu-id="78b41-1217">Beheben von Fehlern in appservice-Befehlen ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="78b41-1217">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="78b41-1218">Verwenden der Ressourcengruppe des App Service-Plans für Zertifizierungsvorgänge ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="78b41-1218">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="78b41-1219">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="78b41-1219">CosmosDB</span></span>

* <span data-ttu-id="78b41-1220">Umbenennen des documentdb-Moduls in cosmosdb</span><span class="sxs-lookup"><span data-stu-id="78b41-1220">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="78b41-1221">Zusätzliche Unterstützung für documentdb-APIs auf Datenebene: Datenbank- und Sammlungsverwaltung</span><span class="sxs-lookup"><span data-stu-id="78b41-1221">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="78b41-1222">Zusätzliche Unterstützung für das Aktivieren des automatischen Failovers für Datenbankkonten</span><span class="sxs-lookup"><span data-stu-id="78b41-1222">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="78b41-1223">Zusätzliche Unterstützung für die neue ConsistentPrefix-Konsistenzrichtlinie</span><span class="sxs-lookup"><span data-stu-id="78b41-1223">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="78b41-1224">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="78b41-1224">Data Lake Analytics</span></span>

* <span data-ttu-id="78b41-1225">Beheben eines Fehlers, bei dem das Filtern von Auftragslisten nach Ergebnis und Status einen Fehler auslöst</span><span class="sxs-lookup"><span data-stu-id="78b41-1225">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="78b41-1226">Hinzufügen von Unterstützung für den neuen Katalogelementtyp „Paket“</span><span class="sxs-lookup"><span data-stu-id="78b41-1226">Add support for new catalog item type: package.</span></span> <span data-ttu-id="78b41-1227">Zugriff über: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="78b41-1227">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="78b41-1228">Ermöglichen der Auflistung folgender Katalogelemente innerhalb einer Datenbank (keine Schemaspezifikation erforderlich):</span><span class="sxs-lookup"><span data-stu-id="78b41-1228">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="78b41-1229">Table</span><span class="sxs-lookup"><span data-stu-id="78b41-1229">Table</span></span>
  * <span data-ttu-id="78b41-1230">Tabellenwertfunktion</span><span class="sxs-lookup"><span data-stu-id="78b41-1230">Table valued function</span></span>
  * <span data-ttu-id="78b41-1231">Sicht</span><span class="sxs-lookup"><span data-stu-id="78b41-1231">View</span></span>
  * <span data-ttu-id="78b41-1232">Tabellenstatistiken.</span><span class="sxs-lookup"><span data-stu-id="78b41-1232">Table Statistics.</span></span> <span data-ttu-id="78b41-1233">Können auch mit einem Schema, jedoch ohne Angabe eines Tabellennamens aufgelistet werden.</span><span class="sxs-lookup"><span data-stu-id="78b41-1233">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="78b41-1234">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="78b41-1234">Data Lake Store</span></span>

* <span data-ttu-id="78b41-1235">Aktualisieren der Version des zugrunde liegenden Dateisystem-SDK, wodurch eine bessere Unterstützung für die Verarbeitung von Drosselungsszenarien auf Serverseite gewährt wird</span><span class="sxs-lookup"><span data-stu-id="78b41-1235">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="78b41-1236">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="78b41-1236">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="78b41-1237">Fehlende Hilfe für Zugriffsanzeige</span><span class="sxs-lookup"><span data-stu-id="78b41-1237">missed help for access show.</span></span> <span data-ttu-id="78b41-1238">hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="78b41-1238">adding it.</span></span> <span data-ttu-id="78b41-1239">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="78b41-1239">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="78b41-1240">Suchen</span><span class="sxs-lookup"><span data-stu-id="78b41-1240">Find</span></span>

* <span data-ttu-id="78b41-1241">Verbessern von Suchergebnissen und Ermöglichen der Versionsverwaltung des Suchindex</span><span class="sxs-lookup"><span data-stu-id="78b41-1241">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="78b41-1242">KeyVault</span><span class="sxs-lookup"><span data-stu-id="78b41-1242">KeyVault</span></span>

* <span data-ttu-id="78b41-1243">BC:`az keyvault certificate download` Ändern von „-e“ von Zeichenfolge oder Binärdatentyp in PEM oder DER zur besseren Darstellung der Optionen</span><span class="sxs-lookup"><span data-stu-id="78b41-1243">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="78b41-1244">BC: Entfernen von „--expires“ und „--not-before“ aus `keyvault certificate create`, da diese Parameter nicht vom Dienst unterstützt werden</span><span class="sxs-lookup"><span data-stu-id="78b41-1244">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="78b41-1245">Hinzufügen des Parameters „--validity“ zu `keyvault certificate create`, um gezielt den Wert in „--policy“ zu überschreiben</span><span class="sxs-lookup"><span data-stu-id="78b41-1245">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="78b41-1246">Beheben des Problems in `keyvault certificate get-default-policy`, bei dem „expires“ und „not_before“ verfügbar gemacht wurden, „validity_in_months“ hingegen nicht</span><span class="sxs-lookup"><span data-stu-id="78b41-1246">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="78b41-1247">Keyvault-Korrektur für den Import von PEM und PFX ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="78b41-1247">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="78b41-1248">Labor</span><span class="sxs-lookup"><span data-stu-id="78b41-1248">Lab</span></span>

* <span data-ttu-id="78b41-1249">Hinzufügen der Befehle „create“, „show“, „delete“ und „list“ für die Laborumgebung</span><span class="sxs-lookup"><span data-stu-id="78b41-1249">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="78b41-1250">Hinzufügen der Befehle „show“ und „list“ zur Anzeige von ARM-Vorlagen im Labor</span><span class="sxs-lookup"><span data-stu-id="78b41-1250">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="78b41-1251">Hinzufügen des Kennzeichens „--environment“ in `az lab vm list`, um virtuelle Computer nach Umgebung im Labor zu filtern</span><span class="sxs-lookup"><span data-stu-id="78b41-1251">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="78b41-1252">Hinzufügen des benutzerfreundlichen Befehls `az lab formula export-artifacts` zum Exportieren des Artefaktgerüsts innerhalb der Formel eines Labors</span><span class="sxs-lookup"><span data-stu-id="78b41-1252">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="78b41-1253">Hinzufügen von Befehlen zum Verwalten von Geheimnissen in einem Labor</span><span class="sxs-lookup"><span data-stu-id="78b41-1253">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="78b41-1254">Überwachen</span><span class="sxs-lookup"><span data-stu-id="78b41-1254">Monitor</span></span>

* <span data-ttu-id="78b41-1255">Programmfehlerbehebung: Modellieren von `--actions` von `az alert-rules create` zum Verarbeiten von JSON-Zeichenfolgen ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="78b41-1255">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="78b41-1256">Programmfehlerbehebung: Beim Erstellen von Diagnoseeinstellungen werden Protokolle/Metriken aus Anzeigebefehlen nicht akzeptiert ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="78b41-1256">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="78b41-1257">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="78b41-1257">Network</span></span>

* <span data-ttu-id="78b41-1258">Hinzufügen des `network watcher test-connectivity`-Befehls</span><span class="sxs-lookup"><span data-stu-id="78b41-1258">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="78b41-1259">Hinzufügen von Unterstützung für den `--filters`-Parameter für `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="78b41-1259">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="78b41-1260">Hinzufügen von Unterstützung für den Application Gateway-Verbindungsausgleich</span><span class="sxs-lookup"><span data-stu-id="78b41-1260">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="78b41-1261">Hinzufügen von Unterstützung für die Konfiguration von Application Gateway-WAF-Regelsätzen</span><span class="sxs-lookup"><span data-stu-id="78b41-1261">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="78b41-1262">Hinzufügen von Unterstützung für ExpressRoute-Routenfilter und -Regeln</span><span class="sxs-lookup"><span data-stu-id="78b41-1262">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="78b41-1263">Hinzufügen von Unterstützung für geografisches TrafficManager-Routing</span><span class="sxs-lookup"><span data-stu-id="78b41-1263">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="78b41-1264">Hinzufügen von Unterstützung für richtlinienbasierte Datenverkehrsselektoren für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="78b41-1264">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="78b41-1265">Hinzufügen von Unterstützung für IPSec-Richtlinien für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="78b41-1265">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="78b41-1266">Korrektur eines Fehlers bei `vpn-connection create` bei Verwendung der Parameter `--no-wait` oder `--validate`</span><span class="sxs-lookup"><span data-stu-id="78b41-1266">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="78b41-1267">Hinzufügen von Unterstützung für Aktiv/Aktiv-VNET-Gateways</span><span class="sxs-lookup"><span data-stu-id="78b41-1267">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="78b41-1268">Entfernen von NULL-Werten aus der Ausgabe von `network vpn-connection list/show`-Befehlen</span><span class="sxs-lookup"><span data-stu-id="78b41-1268">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="78b41-1269">BC: Korrektur eines Fehlers in der Ausgabe von `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="78b41-1269">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="78b41-1270">Korrektur eines Fehlers, bei dem das Argument „--key-length“ von „vpn-connection create“ nicht ordnungsgemäß analysiert wurde</span><span class="sxs-lookup"><span data-stu-id="78b41-1270">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="78b41-1271">Korrektur eines Fehlers in `dns zone import`, bei dem Datensätze nicht ordnungsgemäß importiert wurden</span><span class="sxs-lookup"><span data-stu-id="78b41-1271">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="78b41-1272">Korrektur eines Fehlers, bei dem `traffic-manager endpoint update` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="78b41-1272">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="78b41-1273">Hinzufügen von Network Watcher-Vorschaubefehlen</span><span class="sxs-lookup"><span data-stu-id="78b41-1273">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="78b41-1274">Profil</span><span class="sxs-lookup"><span data-stu-id="78b41-1274">Profile</span></span>

* <span data-ttu-id="78b41-1275">Unterstützung der Anmeldung, wenn keine Abonnements gefunden werden ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="78b41-1275">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="78b41-1276">Unterstützung für kurze Parameternamen in „az account set --subscription“ ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="78b41-1276">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="78b41-1277">Redis</span><span class="sxs-lookup"><span data-stu-id="78b41-1277">Redis</span></span>

* <span data-ttu-id="78b41-1278">Hinzufügen des Updatebefehls, durch den auch die Möglichkeit zum Skalieren für Redis Cache hinzugefügt wird</span><span class="sxs-lookup"><span data-stu-id="78b41-1278">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="78b41-1279">Verwerfen des Befehls „update-settings“</span><span class="sxs-lookup"><span data-stu-id="78b41-1279">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="78b41-1280">Ressource</span><span class="sxs-lookup"><span data-stu-id="78b41-1280">Resource</span></span>

* <span data-ttu-id="78b41-1281">Hinzufügen der Befehle „managedapp“ und „managedapp definition“ ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="78b41-1281">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="78b41-1282">Unterstützung für die „provider operation“-Befehle ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="78b41-1282">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="78b41-1283">Unterstützung für die Erstellung generischer Ressourcen ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="78b41-1283">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="78b41-1284">Korrigieren der Ressourcenanalyse und der API-Versionssuche</span><span class="sxs-lookup"><span data-stu-id="78b41-1284">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="78b41-1285">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="78b41-1285">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="78b41-1286">Hinzufügen von Dokumenten für „az lock update“</span><span class="sxs-lookup"><span data-stu-id="78b41-1286">Add docs for az lock update.</span></span> <span data-ttu-id="78b41-1287">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="78b41-1287">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="78b41-1288">Beenden mit Fehler bei dem Versuch, Ressourcen für eine nicht vorhandene Gruppe aufzulisten</span><span class="sxs-lookup"><span data-stu-id="78b41-1288">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="78b41-1289">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="78b41-1289">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="78b41-1290">[Compute] Beheben von Problemen mit dem Update von VMSS- und VM-Verfügbarkeitsgruppen</span><span class="sxs-lookup"><span data-stu-id="78b41-1290">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="78b41-1291">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="78b41-1291">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="78b41-1292">Korrigieren des Erstellungs- und Löschvorgangs für Sperren, wenn „parent-resource-path“ auf „None“ festgelegt ist ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="78b41-1292">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="78b41-1293">Rolle</span><span class="sxs-lookup"><span data-stu-id="78b41-1293">Role</span></span>

* <span data-ttu-id="78b41-1294">create-for-rbac: Sicherstellen, dass das SP-Enddatum nicht das Ablaufdatum des Zertifikats überschreitet ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="78b41-1294">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="78b41-1295">RBAC: Hinzufügen vollständiger Unterstützung für „ad group“ ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="78b41-1295">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="78b41-1296">Rolle: Beheben von Probleme beim Rollendefinitionsupdate ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="78b41-1296">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="78b41-1297">create-for-rbac: Sicherstellen, dass das angegebene Benutzerkennwort übernommen wird</span><span class="sxs-lookup"><span data-stu-id="78b41-1297">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="78b41-1298">SQL</span><span class="sxs-lookup"><span data-stu-id="78b41-1298">SQL</span></span>

* <span data-ttu-id="78b41-1299">Hinzufügen der Befehle „az sql server list-usages“ und „az sql db list-usages“</span><span class="sxs-lookup"><span data-stu-id="78b41-1299">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="78b41-1300">SQL: Möglichkeit zur direkten Verbindung mit Ressourcenanbieter ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="78b41-1300">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="78b41-1301">Speicher</span><span class="sxs-lookup"><span data-stu-id="78b41-1301">Storage</span></span>

* <span data-ttu-id="78b41-1302">Festlegen des Ressourcengruppenstandorts als Standardstandort für `storage account create`</span><span class="sxs-lookup"><span data-stu-id="78b41-1302">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="78b41-1303">Hinzufügen von Unterstützung für das inkrementelle Kopieren von Blobs</span><span class="sxs-lookup"><span data-stu-id="78b41-1303">Add support for incremental blob copy</span></span>
* <span data-ttu-id="78b41-1304">Hinzufügen von Unterstützung für den Upload umfangreicher Blockblobs</span><span class="sxs-lookup"><span data-stu-id="78b41-1304">Add support for large block blob upload</span></span>
* <span data-ttu-id="78b41-1305">Ändern der Blockgröße auf 100 MB, wenn die hochzuladende Datei größer als 200 GB ist</span><span class="sxs-lookup"><span data-stu-id="78b41-1305">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="78b41-1306">VM</span><span class="sxs-lookup"><span data-stu-id="78b41-1306">VM</span></span>

* <span data-ttu-id="78b41-1307">avail-set: Festlegen der UD- und FD-Domänenanzahl als optional</span><span class="sxs-lookup"><span data-stu-id="78b41-1307">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="78b41-1308">Hinweis zu VM-Befehlen in unabhängigen Clouds: Vermeiden Sie Features im Zusammenhang mit verwalteten Datenträgern, einschließlich der folgenden:</span><span class="sxs-lookup"><span data-stu-id="78b41-1308">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="78b41-1309">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="78b41-1309">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="78b41-1310">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="78b41-1310">az vm/vmss disk</span></span>
  3. <span data-ttu-id="78b41-1311">Verwenden Sie in „az vm/vmss create“ den Befehl „—use-unmanaged-disk“, um verwaltete Datenträger zu vermeiden. Andere Befehle sollten funktionieren.</span><span class="sxs-lookup"><span data-stu-id="78b41-1311">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="78b41-1312">vm/vmss: Verbessern des Warnungstexts beim Generieren von SSH-Schlüsselpaaren</span><span class="sxs-lookup"><span data-stu-id="78b41-1312">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="78b41-1313">vm/vmss: Unterstützen der Erstellung über ein Marketplace-Image, für das Planinformationen erforderlich sind ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="78b41-1313">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="78b41-1314">3. April 2017</span><span class="sxs-lookup"><span data-stu-id="78b41-1314">April 3, 2017</span></span>

<span data-ttu-id="78b41-1315">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="78b41-1315">Version 2.0.2</span></span>

<span data-ttu-id="78b41-1316">In dieser Version wurden die Komponenten ACR, Batch, KeyVault und SQL eingeführt.</span><span class="sxs-lookup"><span data-stu-id="78b41-1316">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="78b41-1317">Core</span><span class="sxs-lookup"><span data-stu-id="78b41-1317">Core</span></span>

* <span data-ttu-id="78b41-1318">Hinzufügen der Module „acr“, „lab“, „monitor“ und „find“ zur Standardliste</span><span class="sxs-lookup"><span data-stu-id="78b41-1318">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="78b41-1319">Anmeldung: Überspringen des fehlerhaften Mandanten ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="78b41-1319">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="78b41-1320">Anmeldung: Festlegen des Standardabonnements auf ein Abonnement mit dem Status „Enabled“ ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="78b41-1320">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="78b41-1321">Hinzufügen von wait-Befehlen und Unterstützung von „--no-wait“ für mehr Befehle ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="78b41-1321">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="78b41-1322">Core: Unterstützen der Anmeldung per Dienstprinzipal mit einem Zertifikat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="78b41-1322">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="78b41-1323">Hinzufügen der Meldung zu fehlenden Vorlagenparametern</span><span class="sxs-lookup"><span data-stu-id="78b41-1323">Add prompting for missing template parameters.</span></span> <span data-ttu-id="78b41-1324">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="78b41-1324">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="78b41-1325">Unterstützen des Festlegens von Standardwerten für häufig verwendete Argumente, z.B. Standardressourcengruppe, Standardweb und Standard-VM</span><span class="sxs-lookup"><span data-stu-id="78b41-1325">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="78b41-1326">Unterstützen der Anmeldung an einem bestimmten Mandanten</span><span class="sxs-lookup"><span data-stu-id="78b41-1326">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="78b41-1327">ACS</span><span class="sxs-lookup"><span data-stu-id="78b41-1327">ACS</span></span>

* <span data-ttu-id="78b41-1328">[ACS] Hinzufügen von Unterstützung für die Konfiguration eines ACS-Standardclusters ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="78b41-1328">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="78b41-1329">Hinzufügen von Unterstützung der Aufforderung zur Kennworteingabe für SSH-Schlüssel</span><span class="sxs-lookup"><span data-stu-id="78b41-1329">Add support for ssh key password prompting.</span></span> <span data-ttu-id="78b41-1330">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="78b41-1330">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="78b41-1331">Hinzufügen von Unterstützung für Windows-Cluster</span><span class="sxs-lookup"><span data-stu-id="78b41-1331">Add support for windows clusters.</span></span> <span data-ttu-id="78b41-1332">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="78b41-1332">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="78b41-1333">Wechseln von der Rolle „Besitzer“ zur Rolle „Mitwirkender“</span><span class="sxs-lookup"><span data-stu-id="78b41-1333">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="78b41-1334">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="78b41-1334">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="78b41-1335">AppService</span><span class="sxs-lookup"><span data-stu-id="78b41-1335">AppService</span></span>

* <span data-ttu-id="78b41-1336">appservice: Unterstützung für das Abrufen der externen IP-Adresse für DNS A-Einträge ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="78b41-1336">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="78b41-1337">appservice: Unterstützung der Bindung von Platzhalterzertifikaten ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="78b41-1337">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="78b41-1338">appservice: Unterstützung von Veröffentlichungsprofilen für Listen ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="78b41-1338">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="78b41-1339">AppService: Auslösen der Synchronisierung der Quellcodeverwaltung nach der Konfiguration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="78b41-1339">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="78b41-1340">DataLake</span><span class="sxs-lookup"><span data-stu-id="78b41-1340">DataLake</span></span>

* <span data-ttu-id="78b41-1341">Erste Version des Data Lake Analytics-Moduls</span><span class="sxs-lookup"><span data-stu-id="78b41-1341">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="78b41-1342">Erste Version des Data Lake Store-Moduls</span><span class="sxs-lookup"><span data-stu-id="78b41-1342">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="78b41-1343">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="78b41-1343">DocuemntDB</span></span>

* <span data-ttu-id="78b41-1344">DocumentDB: Hinzufügen von Unterstützung für das Auflisten von Verbindungszeichenfolgen ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="78b41-1344">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="78b41-1345">VM</span><span class="sxs-lookup"><span data-stu-id="78b41-1345">VM</span></span>

* <span data-ttu-id="78b41-1346">[Compute] Hinzufügen von AppGateway-Unterstützung für Erstellung von VM-Skalierungsgruppen ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="78b41-1346">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="78b41-1347">[VM/VMSS] Verbesserte Unterstützung für die Datenträgerzwischenspeicherung ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="78b41-1347">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="78b41-1348">VM/VMSS: Einbinden der vom Portal verwendeten Logik zur Überprüfung von Anmeldeinformationen ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="78b41-1348">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="78b41-1349">Hinzufügen von wait-Befehlen und Unterstützung für „--no-wait“ ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="78b41-1349">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="78b41-1350">VM-Skalierungsgruppe: Unterstützung von „\*“ zum Auflisten der übergreifenden Instanzansicht für VMs ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="78b41-1350">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="78b41-1351">Hinzufügen – geheime Schlüssel für virtuellen Computer und VM-Skalierungsgruppe ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="78b41-1351">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="78b41-1352">Zulassen der VM-Erstellung mit spezialisierter VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="78b41-1352">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="78b41-1353">27. Februar 2017</span><span class="sxs-lookup"><span data-stu-id="78b41-1353">February 27, 2017</span></span>

<span data-ttu-id="78b41-1354">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="78b41-1354">Version 2.0.0</span></span>

<span data-ttu-id="78b41-1355">Diese Version der Azure CLI 2.0 ist die erste „allgemein verfügbare“ Version. Die allgemeine Verfügbarkeit gilt für die folgenden Befehlsmodule:</span><span class="sxs-lookup"><span data-stu-id="78b41-1355">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="78b41-1356">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="78b41-1356">Container Service (acs)</span></span>
- <span data-ttu-id="78b41-1357">Compute (einschließlich Resource Manager, VM, VM-Skalierungsgruppen, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="78b41-1357">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="78b41-1358">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="78b41-1358">Networking</span></span>
- <span data-ttu-id="78b41-1359">Speicher</span><span class="sxs-lookup"><span data-stu-id="78b41-1359">Storage</span></span>

<span data-ttu-id="78b41-1360">Diese Befehlsmodule können in der Produktion verwendet werden und verfügen über Unterstützung durch eine Standard-SLA von Microsoft. Sie können Anfragen zu Problemen direkt beim Microsoft-Support oder in der [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/) öffnen. Sie haben die Möglichkeit, Fragen in [StackOverflow mit dem Tag „azure-cli“](http://stackoverflow.com/questions/tagged/azure-cli) zu stellen oder sich unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) an das Produktteam zu wenden. Außerdem können Sie über die Befehlszeile mit dem Befehl `az feedback` Feedback senden.</span><span class="sxs-lookup"><span data-stu-id="78b41-1360">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="78b41-1361">Die Befehle in diesen Modulen sind stabil, und es ist nicht zu erwarten, dass sich die Syntax in den anstehenden Veröffentlichungen dieser Version der Azure CLI ändern.</span><span class="sxs-lookup"><span data-stu-id="78b41-1361">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="78b41-1362">Verwenden Sie zum Überprüfen der Version der CLI den Befehl `az --version`. In der Ausgabe werden die Version der CLI selbst (für diese Veröffentlichung 2.0.0), die einzelnen Befehlsmodule und die von Ihnen genutzten Versionen von Python und GCC aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="78b41-1362">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="78b41-1363">Einige Befehlsmodule verfügen über das Postfix „b*n*“ oder „rc*n*“. Diese Befehlsmodule befinden sich noch in der Vorschauphase und werden später die allgemeine Verfügbarkeit erlangen.</span><span class="sxs-lookup"><span data-stu-id="78b41-1363">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="78b41-1364">Außerdem werden jeden Abend Vorschaubuilds der CLI bereitgestellt. Informationen hierzu finden Sie in der [Anleitung zum Abrufen der abendlichen Builds](https://github.com/Azure/azure-cli#nightly-builds) und im Abschnitt zum [Setup für Entwickler und Beitragen von Code](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="78b41-1364">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="78b41-1365">Sie können für die abendlichen Vorschaubuilds wie folgt Probleme melden:</span><span class="sxs-lookup"><span data-stu-id="78b41-1365">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="78b41-1366">Über die [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="78b41-1366">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="78b41-1367">Per Kontaktaufnahme mit dem Produktteam unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="78b41-1367">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="78b41-1368">Senden von Feedback über die Befehlszeile mit dem Befehl `az feedback`</span><span class="sxs-lookup"><span data-stu-id="78b41-1368">Provide feedback from the command line with the `az feedback` command</span></span>


---
title: Versionshinweise für die Azure CLI
description: Enthält Informationen zu den aktuellen Updates der Azure CLI.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 10/09/2018
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 0aec9dce0eda007c71df3693b39c7ec8cc9856cd
ms.sourcegitcommit: 0fc354c24454f5c9c5ff4b7296ad7b18ffdf31b1
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 10/10/2018
ms.locfileid: "48904785"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="4b7f8-103">Versionshinweise für die Azure CLI</span><span class="sxs-lookup"><span data-stu-id="4b7f8-103">Azure CLI release notes</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="4b7f8-104">9. Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="4b7f8-104">October 9, 2018</span></span>

<span data-ttu-id="4b7f8-105">Version 2.0.47</span><span class="sxs-lookup"><span data-stu-id="4b7f8-105">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="4b7f8-106">Core</span><span class="sxs-lookup"><span data-stu-id="4b7f8-106">Core</span></span>
* <span data-ttu-id="4b7f8-107">Verbesserte Fehlerbehandlung für Fehler vom Typ „Ungültige Anforderung“</span><span class="sxs-lookup"><span data-stu-id="4b7f8-107">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="4b7f8-108">ACR</span><span class="sxs-lookup"><span data-stu-id="4b7f8-108">ACR</span></span>
* <span data-ttu-id="4b7f8-109">Unterstützung für ähnliches Tabellenformat wie Helm-Client hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-109">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="4b7f8-110">ACS</span><span class="sxs-lookup"><span data-stu-id="4b7f8-110">ACS</span></span>
* <span data-ttu-id="4b7f8-111">`aks [create|scale] --nodepool-name` zum Konfigurieren des Knotenpoolnamens hinzugefügt, auf 12 Zeichen gekürzt, Standard: nodepool1</span><span class="sxs-lookup"><span data-stu-id="4b7f8-111">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="4b7f8-112">Korrektur, bei der auf „scp“ zurückgegriffen wird, wenn Parimiko nicht funktioniert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-112">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="4b7f8-113">`aks create` geändert, sodass `--aad-tenant-id` nicht mehr erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="4b7f8-113">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="4b7f8-114">Verbesserte Zusammenführung von Kubernetes-Anmeldeinformationen, wenn doppelte Einträge vorhanden sind</span><span class="sxs-lookup"><span data-stu-id="4b7f8-114">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="4b7f8-115">Container</span><span class="sxs-lookup"><span data-stu-id="4b7f8-115">Container</span></span>
* <span data-ttu-id="4b7f8-116">`functionapp create` geändert, sodass das Erstellen eines Linux-Nutzungsplans mit einer bestimmten Runtime unterstützt wird</span><span class="sxs-lookup"><span data-stu-id="4b7f8-116">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="4b7f8-117">[VORSCHAUVERSION] Unterstützung für das Hosten von Web-Apps in Windows-Containern hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-117">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="4b7f8-118">Event Hub</span><span class="sxs-lookup"><span data-stu-id="4b7f8-118">Event Hub</span></span>
* <span data-ttu-id="4b7f8-119">Befehl `eventhub update` korrigiert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-119">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="4b7f8-120">[WICHTIGE ÄNDERUNG] `list`-Befehle geändert, sodass Fehler von Typ „NotFound(404)“ für Ressourcen mit der typische Vorgehensweise behandelt werden, anstatt eine leere Liste anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="4b7f8-120">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="4b7f8-121">Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="4b7f8-121">Extensions</span></span>
* <span data-ttu-id="4b7f8-122">Problem beim Hinzufügen einer Erweiterung behoben, die bereits installiert ist</span><span class="sxs-lookup"><span data-stu-id="4b7f8-122">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="4b7f8-123">HDInsight</span><span class="sxs-lookup"><span data-stu-id="4b7f8-123">HDInsight</span></span>
* <span data-ttu-id="4b7f8-124">Erste Version</span><span class="sxs-lookup"><span data-stu-id="4b7f8-124">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="4b7f8-125">IoT</span><span class="sxs-lookup"><span data-stu-id="4b7f8-125">IoT</span></span>
* <span data-ttu-id="4b7f8-126">Befehl zur Erweiterungsinstallation zu Banner bei der ersten Ausführung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-126">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="4b7f8-127">KeyVault</span><span class="sxs-lookup"><span data-stu-id="4b7f8-127">KeyVault</span></span>
* <span data-ttu-id="4b7f8-128">Geändert, sodass Key Vault-Speicherbefehle auf das aktuelle API-Profil beschränkt sind</span><span class="sxs-lookup"><span data-stu-id="4b7f8-128">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="4b7f8-129">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="4b7f8-129">Network</span></span>
* <span data-ttu-id="4b7f8-130">`network dns zone create` korrigiert: Befehl ist auch erfolgreich, wenn der Benutzer einen Standardspeicherort konfiguriert hat.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-130">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="4b7f8-131">Siehe Nr. 6052</span><span class="sxs-lookup"><span data-stu-id="4b7f8-131">See #6052</span></span>
* <span data-ttu-id="4b7f8-132">`--remote-vnet-id` für `network vnet peering create` eingestellt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-132">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="4b7f8-133">`--remote-vnet` zum `network vnet peering create`-Element hinzugefügt, das einen Namen oder eine ID akzeptiert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-133">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="4b7f8-134">Unterstützung für mehrere Subnetzpräfixe zu `network vnet create` in `--subnet-prefixes` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-134">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="4b7f8-135">Unterstützung für mehrere Subnetzpräfixe zu `network vnet subnet [create|update]` in `--address-prefixes` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-135">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="4b7f8-136">Problem mit `network application-gateway create` behoben, das die Erstellung von Gateways mit der SKU `WAF_v2` oder `Standard_v2` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="4b7f8-136">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="4b7f8-137">`--service-endpoint-policy`-Argument für Benutzerfreundlichkeit zu `network vnet subnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-137">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="4b7f8-138">Rolle</span><span class="sxs-lookup"><span data-stu-id="4b7f8-138">Role</span></span>
* <span data-ttu-id="4b7f8-139">Unterstützung für das Auflisten von Azure AD-App-Besitzern in `ad app owner` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-139">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="4b7f8-140">Unterstützung für das Auflisten von Azure AD-Dienstprinzipalbesitzern in `ad sp owner` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-140">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="4b7f8-141">Geändert, um sicherzustellen, dass die Erstellungs- und Aktualisierungsbefehle für die Rollendefinition Konfigurationen mit mehreren Berechtigungen akzeptieren</span><span class="sxs-lookup"><span data-stu-id="4b7f8-141">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="4b7f8-142">`ad sp create-for-rbac` geändert, um sicherzustellen, dass der Homepage-URI immer „https“ ist</span><span class="sxs-lookup"><span data-stu-id="4b7f8-142">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="4b7f8-143">Service Bus</span><span class="sxs-lookup"><span data-stu-id="4b7f8-143">Service Bus</span></span>
* <span data-ttu-id="4b7f8-144">[WICHTIGE ÄNDERUNG] `list`-Befehle geändert, sodass Fehler von Typ „NotFound(404)“ für Ressourcen mit der typische Vorgehensweise behandelt werden, anstatt eine leere Liste anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="4b7f8-144">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="4b7f8-145">VM</span><span class="sxs-lookup"><span data-stu-id="4b7f8-145">VM</span></span>
* <span data-ttu-id="4b7f8-146">Leeres `accessSas`-Feld in `disk grant-access` korrigiert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-146">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="4b7f8-147">`vmss create` geändert, sodass ein ausreichend großer Front-End-Portbereich zur Verarbeitung von Überbereitstellung reserviert ist</span><span class="sxs-lookup"><span data-stu-id="4b7f8-147">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="4b7f8-148">Aktualisierungsbefehle für `sig` korrigiert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-148">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="4b7f8-149">`--no-wait`-Unterstützung für die Verwaltung von Imageversionen in `sig` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-149">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="4b7f8-150">`vm list-ip-addresses` geändert, sodass die Verfügbarkeitszone von öffentlichen IP-Adressen angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="4b7f8-150">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="4b7f8-151">`[vm|vmss] disk attach` geändert, sodass die Standard-LUN eines Datenträgers standardmäßig auf die erste verfügbare Stelle festgelegt wird</span><span class="sxs-lookup"><span data-stu-id="4b7f8-151">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="4b7f8-152">21. September 2018</span><span class="sxs-lookup"><span data-stu-id="4b7f8-152">September 21, 2018</span></span>

<span data-ttu-id="4b7f8-153">Version 2.0.46</span><span class="sxs-lookup"><span data-stu-id="4b7f8-153">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="4b7f8-154">ACR</span><span class="sxs-lookup"><span data-stu-id="4b7f8-154">ACR</span></span>
* <span data-ttu-id="4b7f8-155">ACR-Aufgabenbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-155">Added ACR Task commands</span></span>
* <span data-ttu-id="4b7f8-156">Befehl für die Schnellausführung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-156">Added quick run command</span></span>
* <span data-ttu-id="4b7f8-157">`build-task`-Befehlsgruppe als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-157">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="4b7f8-158">`helm`-Befehlsgruppe hinzugefügt, um die Verwaltung von Helm-Diagrammen mit ACR zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="4b7f8-158">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="4b7f8-159">Unterstützung für idempotentes Erstellen für die verwaltete Registrierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-159">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="4b7f8-160">Formatfreies Flag für die Anzeige von Buildprotokollen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-160">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="4b7f8-161">ACS</span><span class="sxs-lookup"><span data-stu-id="4b7f8-161">ACS</span></span>
* <span data-ttu-id="4b7f8-162">Befehl `install-connector` zum Festlegen des AKS-Master-FQDN geändert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-162">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="4b7f8-163">Erstellen der Rollenzuweisung für „vnet-subnet-id“ (wenn kein Dienstprinzipal angegeben wurde) und „skip-role-assignment“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-163">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="4b7f8-164">AppService</span><span class="sxs-lookup"><span data-stu-id="4b7f8-164">AppService</span></span>

* <span data-ttu-id="4b7f8-165">Unterstützung für WebJobs-Vorgangsverwaltung hinzugefügt (kontinuierlich/ausgelöst)</span><span class="sxs-lookup"><span data-stu-id="4b7f8-165">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="4b7f8-166">„az webapp config set“ unterstützt die Eigenschaft „--fts-state“; Unterstützung für „az functionapp config set/show“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-166">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="4b7f8-167">Unterstützung für Bring Your Own Storage für Web-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-167">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="4b7f8-168">Unterstützung für das Auflisten und Wiederherstellen gelöschter Web-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-168">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="4b7f8-169">Batch</span><span class="sxs-lookup"><span data-stu-id="4b7f8-169">Batch</span></span>
* <span data-ttu-id="4b7f8-170">Hinzufügen von Aufgaben über `--json-file` geändert, um die AddTaskCollectionParameter-Syntax zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="4b7f8-170">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="4b7f8-171">Dokumentation akzeptierter `--json-file`-Formate aktualisiert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-171">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="4b7f8-172">`--max-tasks-per-node-option` zu `batch pool create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-172">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="4b7f8-173">Verhalten von `batch account` geändert, um das aktuell angemeldete Konto anzuzeigen, wenn keine Optionen angegeben wurden</span><span class="sxs-lookup"><span data-stu-id="4b7f8-173">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="4b7f8-174">Batch AI</span><span class="sxs-lookup"><span data-stu-id="4b7f8-174">Batch AI</span></span> 
* <span data-ttu-id="4b7f8-175">Fehler bei der automatischen Speicherkontoerstellung im Befehl `batchai cluster create` behoben</span><span class="sxs-lookup"><span data-stu-id="4b7f8-175">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="4b7f8-176">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="4b7f8-176">Cognitive Services</span></span>
* <span data-ttu-id="4b7f8-177">Vervollständigung für die Argumente `--sku`, `--kind` und `--location` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-177">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="4b7f8-178">Befehl `cognitiveservices account list-usage` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-178">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="4b7f8-179">Befehl `cognitiveservices account list-kinds` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-179">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="4b7f8-180">Befehl `cognitiveservices account list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-180">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="4b7f8-181">`cognitiveservices list` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-181">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="4b7f8-182">`--name` geändert (ist jetzt optional für `cognitiveservices account list-skus`)</span><span class="sxs-lookup"><span data-stu-id="4b7f8-182">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="4b7f8-183">Container</span><span class="sxs-lookup"><span data-stu-id="4b7f8-183">Container</span></span>
* <span data-ttu-id="4b7f8-184">Möglichkeit zum Neustarten und Beenden einer ausgeführten Containergruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-184">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="4b7f8-185">`--network-profile` zum Übergeben eines Netzwerkprofils hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-185">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="4b7f8-186">`--subnet` und `--vnet_name` hinzugefügt, um das Erstellen von Containergruppen in einem VNET zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="4b7f8-186">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="4b7f8-187">Tabellenausgabe geändert, sodass der Status der Containergruppe angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="4b7f8-187">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="4b7f8-188">Data Lake</span><span class="sxs-lookup"><span data-stu-id="4b7f8-188">Datalake</span></span>
* <span data-ttu-id="4b7f8-189">Befehle für VNET-Regeln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-189">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="4b7f8-190">Interaktive Shell</span><span class="sxs-lookup"><span data-stu-id="4b7f8-190">Interactive Shell</span></span>
* <span data-ttu-id="4b7f8-191">Fehler in Windows behoben, durch den Befehle nicht ordnungsgemäß ausgeführt wurden</span><span class="sxs-lookup"><span data-stu-id="4b7f8-191">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="4b7f8-192">Durch veraltete Objekte verursachtes Problem beim Laden von Befehlen im interaktiven Modus behoben</span><span class="sxs-lookup"><span data-stu-id="4b7f8-192">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="4b7f8-193">IoT</span><span class="sxs-lookup"><span data-stu-id="4b7f8-193">IoT</span></span>
* <span data-ttu-id="4b7f8-194">Routingunterstützung für IoT Hubs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-194">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="4b7f8-195">Key Vault</span><span class="sxs-lookup"><span data-stu-id="4b7f8-195">Key Vault</span></span>
* <span data-ttu-id="4b7f8-196">Key Vault-Schlüsselimport für RSA-Schlüssel korrigiert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-196">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="4b7f8-197">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="4b7f8-197">Network</span></span>
* <span data-ttu-id="4b7f8-198">Befehle vom Typ `network public-ip prefix` hinzugefügt, um Präfixe von öffentlichen IP-Adressen zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="4b7f8-198">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="4b7f8-199">Befehle vom Typ `network service-endpoint` hinzugefügt, um Dienstendpunktrichtlinien-Features zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="4b7f8-199">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="4b7f8-200">Befehle vom Typ `network lb outbound-rule` hinzugefügt, um die Erstellung von Ausgangsregeln für Load Balancer Standard zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="4b7f8-200">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="4b7f8-201">`--public-ip-prefix` zu `network lb frontend-ip create/update` hinzugefügt, um Front-End-IP-Konfigurationen mit Präfixen von öffentlichen IP-Adressen zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="4b7f8-201">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="4b7f8-202">`--enable-tcp-reset` zu `network lb rule/inbound-nat-rule/inbound-nat-pool create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-202">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="4b7f8-203">`--disable-outbound-snat` zu `network lb rule create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-203">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="4b7f8-204">Verwendung von `network watcher flow-log show/configure` mit klassischen NSGs ermöglicht</span><span class="sxs-lookup"><span data-stu-id="4b7f8-204">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="4b7f8-205">Hinzufügen des `network watcher run-configuration-diagnostic`-Befehls</span><span class="sxs-lookup"><span data-stu-id="4b7f8-205">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="4b7f8-206">Befehl `network watcher test-connectivity` korrigiert und Eigenschaften `--method`, `--valid-status-codes` und `--headers` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-206">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="4b7f8-207">`network express-route create/update`: Flag `--allow-global-reach` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-207">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="4b7f8-208">`network vnet subnet create/update`: Unterstützung für `--delegation` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-208">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="4b7f8-209">Befehl `network vnet subnet list-available-delegations` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-209">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="4b7f8-210">`network traffic-manager profile create/update`: Unterstützung für `--interval`, `--timeout` und `--max-failures` für die Überwachungskonfiguration hinzugefügt; Optionen `--monitor-path`, `--monitor-port` und `--monitor-protocol` zugunsten von `--path`, `--port` und `--protocol` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-210">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="4b7f8-211">`network lb frontend-ip create/update`: Logik für das Festlegen der Zuweisungsmethode für private IP-Adressen korrigiert. Bei Angabe einer privaten IP-Adresse ist die Zuweisung statisch. Wird keine private IP-Adresse (oder eine leere Zeichenfolge für die private IP-Adresse) angegeben, erfolgt eine dynamische Zuweisung.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-211">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="4b7f8-212">`dns record-set * create/update`: Unterstützung für `--target-resource` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-212">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="4b7f8-213">Befehle vom Typ `network interface-endpoint` hinzugefügt, um Schnittstellenendpunkt-Objekte abzufragen</span><span class="sxs-lookup"><span data-stu-id="4b7f8-213">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="4b7f8-214">`network profile show/list/delete` für die partielle Verwaltung von Netzwerkprofilen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-214">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="4b7f8-215">Befehle vom Typ `network express-route peering connection` für die Verwaltung von Peeringverbindungen zwischen ExpressRoute-Instanzen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-215">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="4b7f8-216">RDBMS</span><span class="sxs-lookup"><span data-stu-id="4b7f8-216">RDBMS</span></span>
* <span data-ttu-id="4b7f8-217">Unterstützung für den MariaDB-Dienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-217">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="4b7f8-218">Reservierung</span><span class="sxs-lookup"><span data-stu-id="4b7f8-218">Reservation</span></span>
* <span data-ttu-id="4b7f8-219">Cosmos DB im Enumerationstyp für reservierte Ressourcen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-219">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="4b7f8-220">Namenseigenschaft im Patchmodell hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-220">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="4b7f8-221">App-Verwaltung</span><span class="sxs-lookup"><span data-stu-id="4b7f8-221">Manage App</span></span>
* <span data-ttu-id="4b7f8-222">Fehler in `managedapp create --kind MarketPlace` korrigiert, der zum Absturz der Instanzerstellung einer verwalteten Marketplace-App führte</span><span class="sxs-lookup"><span data-stu-id="4b7f8-222">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="4b7f8-223">Befehle vom Typ `feature` geändert, um sie auf unterstützte Profile zu beschränken</span><span class="sxs-lookup"><span data-stu-id="4b7f8-223">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="4b7f8-224">Rolle</span><span class="sxs-lookup"><span data-stu-id="4b7f8-224">Role</span></span>
* <span data-ttu-id="4b7f8-225">Unterstützung für das Auflisten der Gruppenmitgliedschaften des Benutzers hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-225">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="4b7f8-226">SignalR</span><span class="sxs-lookup"><span data-stu-id="4b7f8-226">SignalR</span></span>
* <span data-ttu-id="4b7f8-227">Erste Version</span><span class="sxs-lookup"><span data-stu-id="4b7f8-227">First release</span></span>

### <a name="storage"></a><span data-ttu-id="4b7f8-228">Speicher</span><span class="sxs-lookup"><span data-stu-id="4b7f8-228">Storage</span></span>
* <span data-ttu-id="4b7f8-229">Parameter `--auth-mode login` für die Verwendung der Anmeldeinformationen des Benutzers für die Blob- und Warteschlangenautorisierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-229">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="4b7f8-230">`storage container immutability-policy/legal-hold` für die Verwaltung von unveränderlichem Speicher hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-230">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="4b7f8-231">VM</span><span class="sxs-lookup"><span data-stu-id="4b7f8-231">VM</span></span>
* <span data-ttu-id="4b7f8-232">Problem behoben, das dazu führte, dass die Datei mit dem privaten Schlüssel durch `vm create --generate-ssh-keys` überschrieben wird, wenn die Datei mit dem privaten Schlüssel fehlt (Nr. 4725, 6780)</span><span class="sxs-lookup"><span data-stu-id="4b7f8-232">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="4b7f8-233">Unterstützung für den gemeinsamen Image-Katalog über `az sig` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-233">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="4b7f8-234">28. August 2018</span><span class="sxs-lookup"><span data-stu-id="4b7f8-234">August 28, 2018</span></span>

<span data-ttu-id="4b7f8-235">Version 2.0.45</span><span class="sxs-lookup"><span data-stu-id="4b7f8-235">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="4b7f8-236">Core</span><span class="sxs-lookup"><span data-stu-id="4b7f8-236">Core</span></span>

* <span data-ttu-id="4b7f8-237">Das Problem, aufgrund dessen eine leere Konfigurationsdatei geladen wurde, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-237">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="4b7f8-238">Unterstützung für Profil `2018-03-01-hybrid` für Azure Stack hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-238">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="4b7f8-239">ACR</span><span class="sxs-lookup"><span data-stu-id="4b7f8-239">ACR</span></span>

* <span data-ttu-id="4b7f8-240">Problemumgehung für Laufzeitvorgänge ohne ARM-Anforderungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-240">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="4b7f8-241">Änderung vorgenommen, um im Befehl `build` Versionskontrolldateien (etwa „.git“ und „.gitignore“) standardmäßig aus der TAR-Datei auszuschließen</span><span class="sxs-lookup"><span data-stu-id="4b7f8-241">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="4b7f8-242">ACS</span><span class="sxs-lookup"><span data-stu-id="4b7f8-242">ACS</span></span>

* <span data-ttu-id="4b7f8-243">`aks create` geändert, dass standardmäßig virtuelle Computer vom Typ `Standard_DS2_v2` erstellt werden</span><span class="sxs-lookup"><span data-stu-id="4b7f8-243">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="4b7f8-244">`aks get-credentials` geändert, um nun neue APIs zum Abrufen der Clusteranmeldeinformationen aufzurufen</span><span class="sxs-lookup"><span data-stu-id="4b7f8-244">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="4b7f8-245">AppService</span><span class="sxs-lookup"><span data-stu-id="4b7f8-245">AppService</span></span>

* <span data-ttu-id="4b7f8-246">Unterstützung für CORS in „functionapp“ und „webapp“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-246">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="4b7f8-247">ARM-Tagunterstützung in Erstellungsbefehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-247">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="4b7f8-248">`[webapp|functionapp] identity show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="4b7f8-248">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="4b7f8-249">Backup</span><span class="sxs-lookup"><span data-stu-id="4b7f8-249">Backup</span></span>

* <span data-ttu-id="4b7f8-250">`backup vault backup-properties show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="4b7f8-250">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="4b7f8-251">Botdienst</span><span class="sxs-lookup"><span data-stu-id="4b7f8-251">Bot Service</span></span>

* <span data-ttu-id="4b7f8-252">Anfängliches Release der Botdienst-CLI</span><span class="sxs-lookup"><span data-stu-id="4b7f8-252">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="4b7f8-253">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="4b7f8-253">Cognitive Services</span></span>

* <span data-ttu-id="4b7f8-254">Neuer Parameter `--api-properties,` hinzugefügt, der zum Erstellen einiger Dienste erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="4b7f8-254">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="4b7f8-255">IoT</span><span class="sxs-lookup"><span data-stu-id="4b7f8-255">IoT</span></span>

* <span data-ttu-id="4b7f8-256">Problem mit dem Zuweisen verknüpfter Hubs behoben</span><span class="sxs-lookup"><span data-stu-id="4b7f8-256">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="4b7f8-257">Überwachen</span><span class="sxs-lookup"><span data-stu-id="4b7f8-257">Monitor</span></span>

* <span data-ttu-id="4b7f8-258">`monitor metrics alert`-Befehle für Metrikwarnungen nahezu in Echtzeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-258">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="4b7f8-259">`monitor alert`-Befehle als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-259">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="4b7f8-260">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="4b7f8-260">Network</span></span>

* <span data-ttu-id="4b7f8-261">`network application-gateway ssl-policy predefined show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="4b7f8-261">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="4b7f8-262">Ressource</span><span class="sxs-lookup"><span data-stu-id="4b7f8-262">Resource</span></span>

* <span data-ttu-id="4b7f8-263">`provider operation show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="4b7f8-263">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="4b7f8-264">Speicher</span><span class="sxs-lookup"><span data-stu-id="4b7f8-264">Storage</span></span>

* <span data-ttu-id="4b7f8-265">`storage share policy show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="4b7f8-265">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="4b7f8-266">VM</span><span class="sxs-lookup"><span data-stu-id="4b7f8-266">VM</span></span>

* <span data-ttu-id="4b7f8-267">`vm/vmss identity show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="4b7f8-267">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="4b7f8-268">`--storage-caching` für `vm create` eingestellt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-268">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="4b7f8-269">14. August 2018</span><span class="sxs-lookup"><span data-stu-id="4b7f8-269">Auguest 14, 2018</span></span>

<span data-ttu-id="4b7f8-270">Version 2.0.44</span><span class="sxs-lookup"><span data-stu-id="4b7f8-270">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="4b7f8-271">Core</span><span class="sxs-lookup"><span data-stu-id="4b7f8-271">Core</span></span>

* <span data-ttu-id="4b7f8-272">Numerische Anzeige in `table`-Ausgabe korrigiert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-272">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="4b7f8-273">YAML-Ausgabeformat hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-273">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="4b7f8-274">Telemetrie</span><span class="sxs-lookup"><span data-stu-id="4b7f8-274">Telemetry</span></span>

* <span data-ttu-id="4b7f8-275">Verbesserte Berichterstellung für Telemetriedaten</span><span class="sxs-lookup"><span data-stu-id="4b7f8-275">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="4b7f8-276">ACR</span><span class="sxs-lookup"><span data-stu-id="4b7f8-276">ACR</span></span>

* <span data-ttu-id="4b7f8-277">Befehle vom Typ `content-trust policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-277">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="4b7f8-278">Problem behoben, aufgrund dessen `.dockerignore` nicht richtig verarbeitet wurde</span><span class="sxs-lookup"><span data-stu-id="4b7f8-278">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="4b7f8-279">ACS</span><span class="sxs-lookup"><span data-stu-id="4b7f8-279">ACS</span></span>

* <span data-ttu-id="4b7f8-280">`az acs/aks install-cli` für die Installation in `%USERPROFILE%\.azure-kubectl` unter Windows geändert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-280">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="4b7f8-281">`az aks install-connector` geändert, um zu ermitteln, ob der Cluster über RBAC verfügt, und um den ACI-Connector entsprechend zu konfigurieren</span><span class="sxs-lookup"><span data-stu-id="4b7f8-281">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="4b7f8-282">Geändert in Rollenzuweisung zum Subnetz bei entsprechender Angabe</span><span class="sxs-lookup"><span data-stu-id="4b7f8-282">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="4b7f8-283">Neue Option zum Überspringen der Rollenzuweisung für Subnetz hinzugefügt, wenn dieses angegeben ist</span><span class="sxs-lookup"><span data-stu-id="4b7f8-283">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="4b7f8-284">Geändert, um Rollenzuweisung zum Subnetz zu überspringen, wenn bereits eine Zuweisung vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="4b7f8-284">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="4b7f8-285">AppService</span><span class="sxs-lookup"><span data-stu-id="4b7f8-285">AppService</span></span>

* <span data-ttu-id="4b7f8-286">Fehler behoben, der das Erstellen einer Funktions-App mithilfe von Speicherkonten in externen Ressourcengruppen verhinderte</span><span class="sxs-lookup"><span data-stu-id="4b7f8-286">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="4b7f8-287">Absturz bei ZIP-Bereitstellung behoben</span><span class="sxs-lookup"><span data-stu-id="4b7f8-287">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="4b7f8-288">Batch AI</span><span class="sxs-lookup"><span data-stu-id="4b7f8-288">BatchAI</span></span>

* <span data-ttu-id="4b7f8-289">Protokollierungsausgabe für die automatische Speicherkontoerstellung geändert, sodass nun „Ressourcen*gruppe*“ angegeben wird</span><span class="sxs-lookup"><span data-stu-id="4b7f8-289">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="4b7f8-290">Container</span><span class="sxs-lookup"><span data-stu-id="4b7f8-290">Container</span></span>

* <span data-ttu-id="4b7f8-291">`--secure-environment-variables` zum Übergeben sicherer Umgebungsvariablen an einen Container hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-291">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="4b7f8-292">IoT</span><span class="sxs-lookup"><span data-stu-id="4b7f8-292">IoT</span></span>

* <span data-ttu-id="4b7f8-293">[WICHTIGE ÄNDERUNG] Veraltete Befehle entfernt, die in die IoT-Erweiterung verschoben wurden</span><span class="sxs-lookup"><span data-stu-id="4b7f8-293">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="4b7f8-294">Elemente aktualisiert, um nicht die Domäne `azure-devices.net` anzunehmen</span><span class="sxs-lookup"><span data-stu-id="4b7f8-294">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="4b7f8-295">Iot Central</span><span class="sxs-lookup"><span data-stu-id="4b7f8-295">Iot Central</span></span>

* <span data-ttu-id="4b7f8-296">Erstes Release des IoT Central-Moduls</span><span class="sxs-lookup"><span data-stu-id="4b7f8-296">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="4b7f8-297">KeyVault</span><span class="sxs-lookup"><span data-stu-id="4b7f8-297">KeyVault</span></span>


* <span data-ttu-id="4b7f8-298">Befehle zum Verwalten von Speicherkonten und SAS-Definitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-298">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="4b7f8-299">Befehle für Netzwerkregeln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-299">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="4b7f8-300">Parameter `--id` zu Geheimnis-, Schlüssel- und Zertifikatvorgängen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-300">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="4b7f8-301">Unterstützung für Version mit mehreren APIs zur Schlüsseltresorverwaltung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-301">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="4b7f8-302">Unterstützung für Version mit mehreren APIs zur Schlüsseltresordatenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-302">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="4b7f8-303">Relay</span><span class="sxs-lookup"><span data-stu-id="4b7f8-303">Relay</span></span>

* <span data-ttu-id="4b7f8-304">Erste Version</span><span class="sxs-lookup"><span data-stu-id="4b7f8-304">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="4b7f8-305">Sql</span><span class="sxs-lookup"><span data-stu-id="4b7f8-305">Sql</span></span>

* <span data-ttu-id="4b7f8-306">Befehle vom Typ `sql failover-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-306">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="4b7f8-307">Speicher</span><span class="sxs-lookup"><span data-stu-id="4b7f8-307">Storage</span></span>

* <span data-ttu-id="4b7f8-308">[WICHTIGE ÄNDERUNG] `storage account show-usage` geändert, um Parameter `--location` erforderlich zu machen. Auflistung nach Region</span><span class="sxs-lookup"><span data-stu-id="4b7f8-308">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="4b7f8-309">Parameter `--resource-group` geändert, sodass er für `storage account`-Befehle optional ist</span><span class="sxs-lookup"><span data-stu-id="4b7f8-309">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="4b7f8-310">Warnungen vom Typ „Fehler bei Vorbedingung“ für einzelne Fehler in Batch-Befehlen für eine aggregiert Nachricht entfernt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-310">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="4b7f8-311">`[blob|file] delete-batch`-Befehle geändert, sodass kein Array mit Null-Werten mehr ausgegeben wird</span><span class="sxs-lookup"><span data-stu-id="4b7f8-311">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="4b7f8-312">`blob [download|upload|delete-batch]`-Befehle geändert, um SAS-Token aus Container-URL zu lesen</span><span class="sxs-lookup"><span data-stu-id="4b7f8-312">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="4b7f8-313">VM</span><span class="sxs-lookup"><span data-stu-id="4b7f8-313">VM</span></span>

* <span data-ttu-id="4b7f8-314">Allgemeine Filter zu `vm list-skus` für höhere Benutzerfreundlichkeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-314">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="4b7f8-315">31. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="4b7f8-315">July 31, 2018</span></span>

<span data-ttu-id="4b7f8-316">Version 2.0.43</span><span class="sxs-lookup"><span data-stu-id="4b7f8-316">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="4b7f8-317">ACR</span><span class="sxs-lookup"><span data-stu-id="4b7f8-317">ACR</span></span>

* <span data-ttu-id="4b7f8-318">Flag `--with-secure-properties` zum Befehl `acr build-task show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-318">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="4b7f8-319">Befehl `acr build-task update-build` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-319">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="4b7f8-320">ACS</span><span class="sxs-lookup"><span data-stu-id="4b7f8-320">ACS</span></span>

* <span data-ttu-id="4b7f8-321">Änderung, um 0 (Erfolg) zurückzugeben, wenn `az aks browse` durch Drücken von [STRG+C] beendet wird</span><span class="sxs-lookup"><span data-stu-id="4b7f8-321">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="4b7f8-322">Batch</span><span class="sxs-lookup"><span data-stu-id="4b7f8-322">Batch</span></span>

* <span data-ttu-id="4b7f8-323">Korrektur eines Fehlers bei der Anzeige des AAD-Tokens in Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="4b7f8-323">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="4b7f8-324">Container</span><span class="sxs-lookup"><span data-stu-id="4b7f8-324">Container</span></span>

* <span data-ttu-id="4b7f8-325">Voraussetzung von `--log-analytics-workspace-key` für Name oder ID im festgelegten Abonnement entfernt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-325">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="4b7f8-326">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="4b7f8-326">Network</span></span>

* <span data-ttu-id="4b7f8-327">DNS-Unterstützung zu „2017-03-09-profile“ für Azure Stack hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-327">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="4b7f8-328">Ressource</span><span class="sxs-lookup"><span data-stu-id="4b7f8-328">Resource</span></span>

* <span data-ttu-id="4b7f8-329">`--rollback-on-error` zu `group deployment create` hinzugefügt, um bei einem Fehler eine als funktionierend bekannte Bereitstellung auszuführen</span><span class="sxs-lookup"><span data-stu-id="4b7f8-329">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="4b7f8-330">Problem behoben, aufgrund dessen `--parameters {}` mit `group deployment create` zu einem Fehler führte</span><span class="sxs-lookup"><span data-stu-id="4b7f8-330">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="4b7f8-331">Rolle</span><span class="sxs-lookup"><span data-stu-id="4b7f8-331">Role</span></span>

* <span data-ttu-id="4b7f8-332">Unterstützung für das Stack-Profil „2017-03-09-profile“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-332">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="4b7f8-333">Problem behoben, aufgrund dessen das generische Update von Parametern auf `app update` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="4b7f8-333">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="4b7f8-334">Suchen,</span><span class="sxs-lookup"><span data-stu-id="4b7f8-334">Search</span></span>

* <span data-ttu-id="4b7f8-335">Befehle für Azure Search-Dienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-335">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="4b7f8-336">Service Bus</span><span class="sxs-lookup"><span data-stu-id="4b7f8-336">Service Bus</span></span>

* <span data-ttu-id="4b7f8-337">Migrationsbefehlsgruppe hinzugefügt, um einen Namespace von Service Bus Standard zu Premium zu migrieren</span><span class="sxs-lookup"><span data-stu-id="4b7f8-337">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="4b7f8-338">Neue optionale Eigenschaften zu Service Bus-Warteschlange und -Abonnement hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-338">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="4b7f8-339">`--enable-batched-operations` und `--enable-dead-lettering-on-message-expiration` in `queue`</span><span class="sxs-lookup"><span data-stu-id="4b7f8-339">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="4b7f8-340">`--dead-letter-on-filter-exceptions` in `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="4b7f8-340">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="4b7f8-341">Speicher</span><span class="sxs-lookup"><span data-stu-id="4b7f8-341">Storage</span></span>

* <span data-ttu-id="4b7f8-342">Unterstützung für den Download großer Dateien über eine einzelne Verbindung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-342">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="4b7f8-343">`show`-Befehle konvertiert, bei denen im Falle einer fehlenden Ressource kein Fehler mit dem Exitcode 3 ausgelöst wurde</span><span class="sxs-lookup"><span data-stu-id="4b7f8-343">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="4b7f8-344">VM</span><span class="sxs-lookup"><span data-stu-id="4b7f8-344">VM</span></span>

* <span data-ttu-id="4b7f8-345">Unterstützung zum Auflisten von Verfügbarkeitsgruppen nach Abonnement hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-345">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="4b7f8-346">Unterstützung für `StandardSSD_LRS` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-346">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="4b7f8-347">Unterstützung für Anwendungssicherheitsgruppe beim Erstellen einer VM-Skalierungsgruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-347">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="4b7f8-348">[WICHTIGE ÄNDERUNG] `[vm|vmss] create`, `[vm|vmss] identity assign` und `[vm|vmss] identity remove` wurden geändert, um vom Benutzer zugewiesene Identitäten im Wörterbuchformat auszugeben.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-348">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="4b7f8-349">18. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="4b7f8-349">July 18, 2018</span></span>

<span data-ttu-id="4b7f8-350">Version 2.0.42</span><span class="sxs-lookup"><span data-stu-id="4b7f8-350">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="4b7f8-351">Core</span><span class="sxs-lookup"><span data-stu-id="4b7f8-351">Core</span></span>

* <span data-ttu-id="4b7f8-352">Unterstützung für browserbasierte Anmeldung WSL-Bash-Fenster hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-352">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="4b7f8-353">`--force-string`-Flag für alle generischen Updatebefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-353">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="4b7f8-354">[WICHTIGE ÄNDERUNG] Befehle vom Typ „show“ so geändert, dass die Fehlermeldung protokolliert wird und der Vorgang bei einer fehlenden Ressource mit dem Exitcode 3 fehlschlägt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-354">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="4b7f8-355">ACR</span><span class="sxs-lookup"><span data-stu-id="4b7f8-355">ACR</span></span>

* <span data-ttu-id="4b7f8-356">[WICHTIGE ÄNDERUNG] „--no-push“ in Befehl „acr build“ in reines Flag geändert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-356">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="4b7f8-357">Befehle `show` und `update` unter Gruppe `acr repository` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-357">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="4b7f8-358">`--detail`-Flag für `show-manifests` und `show-tags` hinzugefügt, um ausführlichere Informationen anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="4b7f8-358">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="4b7f8-359">Parameter `--image` zur Unterstützung des Abrufs von Builddetails oder Protokollen anhand eines Images hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-359">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="4b7f8-360">ACS</span><span class="sxs-lookup"><span data-stu-id="4b7f8-360">ACS</span></span>

* <span data-ttu-id="4b7f8-361">`az aks create` so geändert, dass mit Fehler beendet wird, wenn `--max-pods` kleiner als 5 ist</span><span class="sxs-lookup"><span data-stu-id="4b7f8-361">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="4b7f8-362">AppService</span><span class="sxs-lookup"><span data-stu-id="4b7f8-362">AppService</span></span>

* <span data-ttu-id="4b7f8-363">Unterstützung für PremiumV2-SKUs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-363">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="4b7f8-364">Batch</span><span class="sxs-lookup"><span data-stu-id="4b7f8-364">Batch</span></span>

* <span data-ttu-id="4b7f8-365">Korrektur eines Fehlers bei der Verwendung von Anmeldeinformationen im Cloud Shell-Modus</span><span class="sxs-lookup"><span data-stu-id="4b7f8-365">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="4b7f8-366">JSON-Eingabe so geändert, dass Groß-/Kleinschreibung nicht beachtet wird</span><span class="sxs-lookup"><span data-stu-id="4b7f8-366">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="4b7f8-367">Batch AI</span><span class="sxs-lookup"><span data-stu-id="4b7f8-367">Batch AI</span></span>

* <span data-ttu-id="4b7f8-368">Befehl `az batchai job exec` korrigiert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-368">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="4b7f8-369">Container</span><span class="sxs-lookup"><span data-stu-id="4b7f8-369">Container</span></span>

* <span data-ttu-id="4b7f8-370">Anforderung von Benutzername und Kennwort für Nicht-DockerHub-Registrierungen entfernt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-370">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="4b7f8-371">Fehler beim Erstellen von Containergruppen aus YAML-Datei behoben</span><span class="sxs-lookup"><span data-stu-id="4b7f8-371">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="4b7f8-372">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="4b7f8-372">Network</span></span>

* <span data-ttu-id="4b7f8-373">Unterstützung für `--no-wait` zu `network nic [create|update|delete]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-373">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="4b7f8-374">`network nic wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-374">Added `network nic wait`</span></span>
* <span data-ttu-id="4b7f8-375">`--ids`-Argument für `network vnet [subnet|peering] list` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-375">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="4b7f8-376">`--include-default`-Flag hinzugefügt, um Standardsicherheitsregeln in die Ausgabe von `network nsg rule list` aufzunehmen</span><span class="sxs-lookup"><span data-stu-id="4b7f8-376">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="4b7f8-377">Ressource</span><span class="sxs-lookup"><span data-stu-id="4b7f8-377">Resource</span></span>

* <span data-ttu-id="4b7f8-378">Unterstützung für `--no-wait` zu `group deployment delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-378">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="4b7f8-379">Unterstützung für `--no-wait` zu `deployment delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-379">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="4b7f8-380">Befehl `deployment wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-380">Added `deployment wait` command</span></span>
* <span data-ttu-id="4b7f8-381">Problem behoben, aufgrund dessen die `az deployment`-Befehle auf Abonnementebene fälschlicherweise für Profil „2017-03-09-profile“ angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="4b7f8-381">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="4b7f8-382">SQL</span><span class="sxs-lookup"><span data-stu-id="4b7f8-382">SQL</span></span>

* <span data-ttu-id="4b7f8-383">Fehler „Der angegebene Ressourcengruppenname ... entsprach nicht dem Namen in der URL“ beim Angeben des Namens des Pools für elastische Datenbanken für `sql db copy`-und `sql db replica create`-Befehle behoben</span><span class="sxs-lookup"><span data-stu-id="4b7f8-383">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="4b7f8-384">Konfigurieren des Standard-SQL Servers durch Ausführen von `az configure --defaults sql-server=<name>` zulässig</span><span class="sxs-lookup"><span data-stu-id="4b7f8-384">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="4b7f8-385">Tabellenformatierer für Befehle `sql server`, `sql server firewall-rule`, `sql list-usages` und `sql show-usage` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-385">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="4b7f8-386">Speicher</span><span class="sxs-lookup"><span data-stu-id="4b7f8-386">Storage</span></span>

* <span data-ttu-id="4b7f8-387">`pageRanges`-Eigenschaft zu `storage blob show`-Ausgabe hinzugefügt, die für Seitenblobs ausgefüllt wird</span><span class="sxs-lookup"><span data-stu-id="4b7f8-387">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="4b7f8-388">VM</span><span class="sxs-lookup"><span data-stu-id="4b7f8-388">VM</span></span>

* <span data-ttu-id="4b7f8-389">[WICHTIGE ÄNDERUNG] `vmss create` so geändert, dass `Standard_DS1_v2` als standardmäßige Instanzgröße verwendet wird</span><span class="sxs-lookup"><span data-stu-id="4b7f8-389">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="4b7f8-390">Unterstützung für `--no-wait` zu `vm extension [set|delete]` und `vmss extension [set|delete]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-390">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="4b7f8-391">`vm extension wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-391">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="4b7f8-392">3. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="4b7f8-392">July 3, 2018</span></span>

<span data-ttu-id="4b7f8-393">Version 2.0.41</span><span class="sxs-lookup"><span data-stu-id="4b7f8-393">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="4b7f8-394">AKS</span><span class="sxs-lookup"><span data-stu-id="4b7f8-394">AKS</span></span>

* <span data-ttu-id="4b7f8-395">Überwachung geändert, sodass Abonnement-ID verwendet wird</span><span class="sxs-lookup"><span data-stu-id="4b7f8-395">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="4b7f8-396">3. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="4b7f8-396">July 3, 2018</span></span>

<span data-ttu-id="4b7f8-397">Version 2.0.40</span><span class="sxs-lookup"><span data-stu-id="4b7f8-397">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="4b7f8-398">Core</span><span class="sxs-lookup"><span data-stu-id="4b7f8-398">Core</span></span>

* <span data-ttu-id="4b7f8-399">Neuer Autorisierungscode-Flow für interaktive Anmeldung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-399">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="4b7f8-400">ACR</span><span class="sxs-lookup"><span data-stu-id="4b7f8-400">ACR</span></span>

* <span data-ttu-id="4b7f8-401">Abruf-Buildstatus hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-401">Added polling build status</span></span>
* <span data-ttu-id="4b7f8-402">Unterstützung für Enumerationswerte ohne Berücksichtigung von Groß-/Kleinschreibung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-402">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="4b7f8-403">Parameter `--top` und `--orderby` für `show-manifests` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-403">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="4b7f8-404">ACS</span><span class="sxs-lookup"><span data-stu-id="4b7f8-404">ACS</span></span>

* <span data-ttu-id="4b7f8-405">[WICHTIGE ÄNDERUNG] Standardmäßiges Aktivieren der rollenbasierten Zugriffssteuerung für Kubernetes</span><span class="sxs-lookup"><span data-stu-id="4b7f8-405">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="4b7f8-406">Argument `--disable-rbac` hinzugefügt und `--enable-rbac` als veraltet festgelegt, da es nun der Standard ist</span><span class="sxs-lookup"><span data-stu-id="4b7f8-406">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="4b7f8-407">Optionen für Befehl `aks browse` wurden aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-407">Updated options for `aks browse` command.</span></span> <span data-ttu-id="4b7f8-408">Unterstützung für `--listen-port` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-408">Added `--listen-port` support</span></span>
* <span data-ttu-id="4b7f8-409">Standardmäßiges Helm-Diagrammpaket für Befehl `aks install-connector` wurde aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-409">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="4b7f8-410">Verwenden von „virtual-kubelet-for-aks-latest.tgz“</span><span class="sxs-lookup"><span data-stu-id="4b7f8-410">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="4b7f8-411">Befehle `aks enable-addons` und `aks disable-addons` zum Aktualisieren eines vorhandenen Clusters hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-411">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="4b7f8-412">AppService</span><span class="sxs-lookup"><span data-stu-id="4b7f8-412">AppService</span></span>

* <span data-ttu-id="4b7f8-413">Unterstützung für das Deaktivieren der Identität über `webapp identity remove` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-413">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="4b7f8-414">`preview`-Tag für Identitätsfunktion entfernt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-414">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="4b7f8-415">Backup</span><span class="sxs-lookup"><span data-stu-id="4b7f8-415">Backup</span></span>

* <span data-ttu-id="4b7f8-416">Moduldefinition aktualisiert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-416">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="4b7f8-417">Batch AI</span><span class="sxs-lookup"><span data-stu-id="4b7f8-417">BatchAI</span></span>

* <span data-ttu-id="4b7f8-418">Tabellenausgabe für Befehle `batchai cluster node list` und `batchai job node list` korrigiert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-418">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="4b7f8-419">Cloud</span><span class="sxs-lookup"><span data-stu-id="4b7f8-419">Cloud</span></span>

* <span data-ttu-id="4b7f8-420">Serversuffix `acr login` zu Cloudkonfiguration hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-420">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="4b7f8-421">Container</span><span class="sxs-lookup"><span data-stu-id="4b7f8-421">Container</span></span>

* <span data-ttu-id="4b7f8-422">`container create` zu Standard für Vorgang mit langer Ausführungsdauer geändert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-422">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="4b7f8-423">Log Analytics-Parameter `--log-analytics-workspace` und `--log-analytics-workspace-key` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-423">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="4b7f8-424">Parameter `--protocol` zum Festlegen des zu verwendenden Netzwerkprotokolls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-424">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="4b7f8-425">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="4b7f8-425">Extension</span></span>

* <span data-ttu-id="4b7f8-426">`extension list-available` geändert, sodass nur mit der CLI-Version kompatible Erweiterungen angezeigt werden</span><span class="sxs-lookup"><span data-stu-id="4b7f8-426">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="4b7f8-427">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="4b7f8-427">Network</span></span>

* <span data-ttu-id="4b7f8-428">Problem behoben, aufgrund dessen bei Datensatztypen die Groß-/Kleinschreibung beachtet werden musste ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="4b7f8-428">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="4b7f8-429">Rdbms</span><span class="sxs-lookup"><span data-stu-id="4b7f8-429">Rdbms</span></span>

* <span data-ttu-id="4b7f8-430">Befehle vom Typ `[postgres|myql] server vnet-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-430">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="4b7f8-431">Ressource</span><span class="sxs-lookup"><span data-stu-id="4b7f8-431">Resource</span></span>

* <span data-ttu-id="4b7f8-432">Neue Vorgangsgruppe `deployment` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-432">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="4b7f8-433">VM</span><span class="sxs-lookup"><span data-stu-id="4b7f8-433">VM</span></span>

* <span data-ttu-id="4b7f8-434">Unterstützung für das Entfernen der vom System zugewiesenen Identität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-434">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="4b7f8-435">25. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="4b7f8-435">June 25, 2018</span></span>

<span data-ttu-id="4b7f8-436">Version 2.0.39</span><span class="sxs-lookup"><span data-stu-id="4b7f8-436">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="4b7f8-437">Befehlszeilenschnittstelle (CLI)</span><span class="sxs-lookup"><span data-stu-id="4b7f8-437">CLI</span></span>

* <span data-ttu-id="4b7f8-438">Dateieinschränkung in MSI-Installer aktualisiert, um Problem mit der Erweiterungsinstallation zu beheben</span><span class="sxs-lookup"><span data-stu-id="4b7f8-438">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="4b7f8-439">19. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="4b7f8-439">June 19, 2018</span></span>

<span data-ttu-id="4b7f8-440">Version 2.0.38</span><span class="sxs-lookup"><span data-stu-id="4b7f8-440">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="4b7f8-441">Core</span><span class="sxs-lookup"><span data-stu-id="4b7f8-441">Core</span></span>

* <span data-ttu-id="4b7f8-442">Globale Unterstützung für `--subscription` zu den meisten Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-442">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="4b7f8-443">ACR</span><span class="sxs-lookup"><span data-stu-id="4b7f8-443">ACR</span></span>

* <span data-ttu-id="4b7f8-444">`azure-storage-blob` als Abhängigkeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-444">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="4b7f8-445">CPU-Standardkonfiguration für `acr build-task create` geändert, sodass zwei Kerne verwendet werden</span><span class="sxs-lookup"><span data-stu-id="4b7f8-445">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="4b7f8-446">ACS</span><span class="sxs-lookup"><span data-stu-id="4b7f8-446">ACS</span></span>

* <span data-ttu-id="4b7f8-447">Optionen des Befehls `aks use-dev-spaces` wurden aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-447">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="4b7f8-448">Unterstützung für `--update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-448">Added `--update` support</span></span>
* <span data-ttu-id="4b7f8-449">`aks get-credentials --admin` geändert, sodass der Benutzerkontext in `$HOME/.kube/config` ersetzt wird</span><span class="sxs-lookup"><span data-stu-id="4b7f8-449">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="4b7f8-450">Schreibgeschützte `nodeResourceGroup`-Eigenschaft in verwalteten Clustern verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="4b7f8-450">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="4b7f8-451">Befehlsfehler `acs browse` korrigiert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-451">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="4b7f8-452">`--connector-name` für `aks install-connector`, `aks upgrade-connector` und `aks remove-connector` als optional festgelegt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-452">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="4b7f8-453">Neue Azure Container Instances-Regionen für `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-453">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="4b7f8-454">Normalisierter Speicherort im Helm-Versionsnamen und Knotenname zu `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-454">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="4b7f8-455">AppService</span><span class="sxs-lookup"><span data-stu-id="4b7f8-455">AppService</span></span>

* <span data-ttu-id="4b7f8-456">Unterstützung für neuere Versionen von „urllib“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-456">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="4b7f8-457">Unterstützung der Verwendung eines App Service-Plans aus externen Ressourcengruppen zu `functionapp create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-457">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="4b7f8-458">Batch</span><span class="sxs-lookup"><span data-stu-id="4b7f8-458">Batch</span></span>

* <span data-ttu-id="4b7f8-459">`azure-batch-extensions`-Abhängigkeit entfernt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-459">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="4b7f8-460">Batch AI</span><span class="sxs-lookup"><span data-stu-id="4b7f8-460">Batch AI</span></span>

* <span data-ttu-id="4b7f8-461">Unterstützung für Arbeitsbereiche wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-461">Added support for workspaces.</span></span> <span data-ttu-id="4b7f8-462">Arbeitsbereiche ermöglichen das Zusammenfassen von Clustern, Dateiservern und Experimenten in Gruppen ohne Beschränkung der Anzahl von Ressourcen, die erstellt werden können.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-462">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="4b7f8-463">Unterstützung für Experimente wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-463">Added support for experiments.</span></span> <span data-ttu-id="4b7f8-464">Experimente ermöglichen das Zusammenfassen von Aufträgen in Sammlungen ohne Beschränkung der Anzahl von erstellten Aufträgen.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-464">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="4b7f8-465">Unterstützung für das Konfigurieren von `/dev/shm` für Aufträge hinzugefügt, die in einem Docker-Container ausgeführt werden</span><span class="sxs-lookup"><span data-stu-id="4b7f8-465">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="4b7f8-466">Die Befehle `batchai cluster node exec` und `batchai job node exec` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-466">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="4b7f8-467">Diese Befehle ermöglichen die Ausführung aller Befehle direkt auf Knoten und bieten Funktionen zur Portweiterleitung.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-467">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="4b7f8-468">Unterstützung für `--ids` zu `batchai`-Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-468">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="4b7f8-469">[WICHTIGE ÄNDERUNG] Alle Cluster und Dateiserver müssen unter Arbeitsbereichen erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-469">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="4b7f8-470">[WICHTIGE ÄNDERUNG] Aufträge müssen unter Experimenten erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-470">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="4b7f8-471">[WICHTIGE ÄNDERUNG] `--nfs-resource-group` wurde aus den Befehlen `cluster create` und `job create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-471">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="4b7f8-472">Geben Sie zum Bereitstellen eines NFS, das einem anderen Arbeitsbereich/einer anderen Ressourcengruppe angehört, die ARM-ID des Dateiservers über die Option `--nfs` an.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-472">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="4b7f8-473">[WICHTIGE ÄNDERUNG] `--cluster-resource-group` wurde aus dem Befehl `job create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-473">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="4b7f8-474">Geben Sie zum Übermitteln eines Auftrags, der einem anderen Arbeitsbereich/einer anderen Ressourcengruppe angehört, die ARM-ID des Clusters über die Option `--cluster` an.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-474">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="4b7f8-475">[WICHTIGE ÄNDERUNG] Attribut `location` wurde aus Aufträgen, Clustern und Dateiservern entfernt.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-475">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="4b7f8-476">„Location“ ist jetzt ein Attribut eines Arbeitsbereichs.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-476">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="4b7f8-477">[WICHTIGE ÄNDERUNG] `--location` wurde aus den Befehlen `job create`, `cluster create` und `file-server create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-477">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="4b7f8-478">[WICHTIGE ÄNDERUNG] Namen von Kurzoptionen wurden geändert, um die Schnittstelle konsistenter zu machen:</span><span class="sxs-lookup"><span data-stu-id="4b7f8-478">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
 - <span data-ttu-id="4b7f8-479">[`--config`, `-c`] in [`--config-file`, `-f`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-479">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
 - <span data-ttu-id="4b7f8-480">[`--cluster`, `-r`] in [`--cluster`, `-c`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-480">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
 - <span data-ttu-id="4b7f8-481">[`--cluster`, `-n`] in [`--cluster`, `-c`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-481">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
 - <span data-ttu-id="4b7f8-482">[`--job`, `-n`] in [`--job`, `-j`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-482">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="4b7f8-483">Karten</span><span class="sxs-lookup"><span data-stu-id="4b7f8-483">Maps</span></span>

* <span data-ttu-id="4b7f8-484">[WICHTIGE ÄNDERUNG] `maps account create` wurde so geändert, dass Nutzungsbedingungen entweder durch interaktive Eingabeaufforderung oder `--accept-tos`-Flag akzeptiert werden müssen.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-484">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="4b7f8-485">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="4b7f8-485">Network</span></span>

* <span data-ttu-id="4b7f8-486">Unterstützung für `https` zu `network lb probe create` hinzugefügt ([#6571](https://github.com/Azure/azure-cli/issues/6571))</span><span class="sxs-lookup"><span data-stu-id="4b7f8-486">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="4b7f8-487">Problem behoben, aufgrund dessen die Groß-/Kleinschreibung von `--endpoint-status` berücksichtigt wurde.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-487">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="4b7f8-488">#6502</span><span class="sxs-lookup"><span data-stu-id="4b7f8-488">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="4b7f8-489">Reservations</span><span class="sxs-lookup"><span data-stu-id="4b7f8-489">Reservations</span></span>

* <span data-ttu-id="4b7f8-490">[WICHTIGE ÄNDERUNG] Erforderlicher Parameter `ReservedResourceType` zu `reservations catalog show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-490">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="4b7f8-491">Parameter `Location` zu `reservations catalog show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-491">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="4b7f8-492">[WICHTIGE ÄNDERUNG] `kind` aus `ReservationProperties` entfernt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-492">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="4b7f8-493">[WICHTIGE ÄNDERUNG] `capabilities` wurde in `Catalog` in `sku_properties` umbenannt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-493">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="4b7f8-494">[WICHTIGE ÄNDERUNG] Eigenschaften `size` und `tier` aus `Catalog` entfernt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-494">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="4b7f8-495">Parameter `InstanceFlexibility` zu `reservations reservation update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-495">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="4b7f8-496">Rolle</span><span class="sxs-lookup"><span data-stu-id="4b7f8-496">Role</span></span>

* <span data-ttu-id="4b7f8-497">Fehlerbehandlung verbessert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-497">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="4b7f8-498">SQL</span><span class="sxs-lookup"><span data-stu-id="4b7f8-498">SQL</span></span>

* <span data-ttu-id="4b7f8-499">Verwirrender Fehler behoben, der beim Ausführen von `az sql db list-editions` für einen Ort auftrat, der für Ihr Abonnement nicht verfügbar ist</span><span class="sxs-lookup"><span data-stu-id="4b7f8-499">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="4b7f8-500">Speicher</span><span class="sxs-lookup"><span data-stu-id="4b7f8-500">Storage</span></span>

* <span data-ttu-id="4b7f8-501">Lesbarkeit der Tabellenausgabe für `storage blob download` verbessert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-501">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="4b7f8-502">VM</span><span class="sxs-lookup"><span data-stu-id="4b7f8-502">VM</span></span>

* <span data-ttu-id="4b7f8-503">Verbesserte Einschränkung der VM-Größenüberprüfung für Unterstützung von beschleunigten Netzwerken in `vm create`</span><span class="sxs-lookup"><span data-stu-id="4b7f8-503">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="4b7f8-504">Warnung für `vmss create` hinzugefügt, dass die VM-Standardgröße von `Standard_D1_v2` auf `Standard_DS1_v2` umgestellt wird</span><span class="sxs-lookup"><span data-stu-id="4b7f8-504">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="4b7f8-505">`--force-update` zu `[vm|vmss] extension set` hinzugefügt, um die Erweiterung auch dann zu aktualisieren, wenn die Konfiguration nicht geändert wurde</span><span class="sxs-lookup"><span data-stu-id="4b7f8-505">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="4b7f8-506">13. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="4b7f8-506">June 13, 2018</span></span>

<span data-ttu-id="4b7f8-507">Version 2.0.37</span><span class="sxs-lookup"><span data-stu-id="4b7f8-507">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="4b7f8-508">Core</span><span class="sxs-lookup"><span data-stu-id="4b7f8-508">Core</span></span>

* <span data-ttu-id="4b7f8-509">Verbesserte interaktive Telemetrie</span><span class="sxs-lookup"><span data-stu-id="4b7f8-509">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="4b7f8-510">13. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="4b7f8-510">June 13, 2018</span></span>

<span data-ttu-id="4b7f8-511">Version 2.0.36</span><span class="sxs-lookup"><span data-stu-id="4b7f8-511">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="4b7f8-512">AKS</span><span class="sxs-lookup"><span data-stu-id="4b7f8-512">AKS</span></span>

* <span data-ttu-id="4b7f8-513">Zusätzliche erweiterte Netzwerkoptionen zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-513">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="4b7f8-514">Argumente zu `aks create` zum Aktivieren der Überwachung und HTTP-Routing hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-514">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="4b7f8-515">Argument `--no-ssh-key` zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-515">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="4b7f8-516">Argument `--enable-rbac` zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-516">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="4b7f8-517">[VORSCHAUVERSION] Unterstützung für Azure Active Directory-Authentifizierung zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-517">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="4b7f8-518">AppService</span><span class="sxs-lookup"><span data-stu-id="4b7f8-518">AppService</span></span>

* <span data-ttu-id="4b7f8-519">Problem mit inkompatiblen urllib-Versionen behoben</span><span class="sxs-lookup"><span data-stu-id="4b7f8-519">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="4b7f8-520">5. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="4b7f8-520">June 5, 2018</span></span>

<span data-ttu-id="4b7f8-521">Version 2.0.35</span><span class="sxs-lookup"><span data-stu-id="4b7f8-521">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="4b7f8-522">Interactive</span><span class="sxs-lookup"><span data-stu-id="4b7f8-522">Interactive</span></span>

* <span data-ttu-id="4b7f8-523">Grenzwerte für die Abhängigkeiten des interaktiven Modus hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-523">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="4b7f8-524">5. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="4b7f8-524">June 5, 2018</span></span>

<span data-ttu-id="4b7f8-525">Version 2.0.34</span><span class="sxs-lookup"><span data-stu-id="4b7f8-525">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="4b7f8-526">Core</span><span class="sxs-lookup"><span data-stu-id="4b7f8-526">Core</span></span>

* <span data-ttu-id="4b7f8-527">Unterstützung für mandantenübergreifende Ressourcenverweise hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-527">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="4b7f8-528">Verbesserte Zuverlässigkeit bei Telemetrieuploads</span><span class="sxs-lookup"><span data-stu-id="4b7f8-528">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="4b7f8-529">ACR</span><span class="sxs-lookup"><span data-stu-id="4b7f8-529">ACR</span></span>

* <span data-ttu-id="4b7f8-530">Unterstützung für VSTS als Remotequellort hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-530">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="4b7f8-531">Befehl `acr import` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-531">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="4b7f8-532">AKS</span><span class="sxs-lookup"><span data-stu-id="4b7f8-532">AKS</span></span>

* <span data-ttu-id="4b7f8-533">`aks get-credentials` wurde geändert, um die Kube-Konfigurationsdatei mit sichereren Dateisystemberechtigungen zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-533">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="4b7f8-534">Batch</span><span class="sxs-lookup"><span data-stu-id="4b7f8-534">Batch</span></span>

* <span data-ttu-id="4b7f8-535">Fehler bei der Formatierung der Poollistentabelle behoben [[Problem 4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="4b7f8-535">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="4b7f8-536">IoT</span><span class="sxs-lookup"><span data-stu-id="4b7f8-536">IOT</span></span>

* <span data-ttu-id="4b7f8-537">Unterstützung für das Erstellen von IoT Hub-Instanzen im Tarif „Basic“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-537">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="4b7f8-538">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="4b7f8-538">Network</span></span>

* <span data-ttu-id="4b7f8-539">`network vnet peering` wurde verbessert.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-539">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="4b7f8-540">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="4b7f8-540">Policy Insights</span></span>

* <span data-ttu-id="4b7f8-541">Erste Version</span><span class="sxs-lookup"><span data-stu-id="4b7f8-541">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="4b7f8-542">ARM</span><span class="sxs-lookup"><span data-stu-id="4b7f8-542">ARM</span></span>

* <span data-ttu-id="4b7f8-543">Befehle vom Typ `account management-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-543">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="4b7f8-544">SQL</span><span class="sxs-lookup"><span data-stu-id="4b7f8-544">SQL</span></span>

* <span data-ttu-id="4b7f8-545">Neue Befehle für verwaltete Instanzen hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="4b7f8-545">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="4b7f8-546">Neue Befehle für verwaltete Datenbanken hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="4b7f8-546">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="4b7f8-547">Speicher</span><span class="sxs-lookup"><span data-stu-id="4b7f8-547">Storage</span></span>

* <span data-ttu-id="4b7f8-548">Zusätzliche MimeTypes für JSON und JavaScript hinzugefügt (abzuleiten aus Dateierweiterungen)</span><span class="sxs-lookup"><span data-stu-id="4b7f8-548">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="4b7f8-549">VM</span><span class="sxs-lookup"><span data-stu-id="4b7f8-549">VM</span></span>

* <span data-ttu-id="4b7f8-550">`vm list-skus` wurde geändert, um feste Spalten zu verwenden und eine Warnung hinzuzufügen, dass `Tier` und `Size` entfernt werden.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-550">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="4b7f8-551">Option `--accelerated-networking` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-551">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="4b7f8-552">`--tags` zu `identity create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-552">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="4b7f8-553">22. Mai 2018</span><span class="sxs-lookup"><span data-stu-id="4b7f8-553">May 22, 2018</span></span>

<span data-ttu-id="4b7f8-554">Version 2.0.33</span><span class="sxs-lookup"><span data-stu-id="4b7f8-554">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="4b7f8-555">Core</span><span class="sxs-lookup"><span data-stu-id="4b7f8-555">Core</span></span>

* <span data-ttu-id="4b7f8-556">Unterstützung für das Erweitern von `@` in Dateinamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-556">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="4b7f8-557">ACS</span><span class="sxs-lookup"><span data-stu-id="4b7f8-557">ACS</span></span>

* <span data-ttu-id="4b7f8-558">Neue Dev Spaces-Befehle `aks use-dev-spaces` und `aks remove-dev-spaces` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-558">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="4b7f8-559">Tippfehler in Hilfemeldung korrigiert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-559">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="4b7f8-560">AppService</span><span class="sxs-lookup"><span data-stu-id="4b7f8-560">AppService</span></span>

* <span data-ttu-id="4b7f8-561">Verbesserte generische Aktualisierungsbefehle</span><span class="sxs-lookup"><span data-stu-id="4b7f8-561">Improved generic update commands</span></span>
* <span data-ttu-id="4b7f8-562">Asynchrone Unterstützung für `webapp deployment source config-zip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-562">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="4b7f8-563">Container</span><span class="sxs-lookup"><span data-stu-id="4b7f8-563">Container</span></span>

* <span data-ttu-id="4b7f8-564">Unterstützung für das Exportieren einer Containergruppe im YAML-Format hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-564">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="4b7f8-565">Unterstützung für die Verwendung einer YAML-Datei zum Erstellen/Aktualisieren einer Containergruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-565">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="4b7f8-566">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="4b7f8-566">Extension</span></span>

* <span data-ttu-id="4b7f8-567">Verbesserte Entfernung von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="4b7f8-567">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="4b7f8-568">Interactive</span><span class="sxs-lookup"><span data-stu-id="4b7f8-568">Interactive</span></span>

* <span data-ttu-id="4b7f8-569">Protokollierung geändert, um Parser für Abschlüsse zu deaktivieren</span><span class="sxs-lookup"><span data-stu-id="4b7f8-569">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="4b7f8-570">Verbesserte Verarbeitung beschädigter Hilfscaches</span><span class="sxs-lookup"><span data-stu-id="4b7f8-570">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="4b7f8-571">KeyVault</span><span class="sxs-lookup"><span data-stu-id="4b7f8-571">KeyVault</span></span>

* <span data-ttu-id="4b7f8-572">keyvault-Befehle wurden korrigiert, damit sie in Cloud Shell oder auf virtuellen Computern mit Identität verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-572">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="4b7f8-573">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="4b7f8-573">Network</span></span>

* <span data-ttu-id="4b7f8-574">Problem behoben, aufgrund dessen `network watcher show-topology` nicht mit einem VNET und/oder Subnetznamen verwendet werden konnte ([#6326](https://github.com/Azure/azure-cli/issues/6326))</span><span class="sxs-lookup"><span data-stu-id="4b7f8-574">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="4b7f8-575">Problem behoben, aufgrund dessen einige `network watcher`-Befehle fälschlicherweise angaben, dass Network Watcher nicht für bestimmte Regionen aktiviert ist ([#6264](https://github.com/Azure/azure-cli/issues/6264))</span><span class="sxs-lookup"><span data-stu-id="4b7f8-575">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="4b7f8-576">SQL</span><span class="sxs-lookup"><span data-stu-id="4b7f8-576">SQL</span></span>

* <span data-ttu-id="4b7f8-577">[WICHTIGE ÄNDERUNG] Von den Befehlen `db` und `dw` zurückgegebene Antwortobjekte geändert:</span><span class="sxs-lookup"><span data-stu-id="4b7f8-577">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="4b7f8-578">Eigenschaft `serviceLevelObjective` in `currentServiceObjectiveName` umbenannt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-578">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="4b7f8-579">Eigenschaften `currentServiceObjectiveId` und `requestedServiceObjectiveId` entfernt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-579">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="4b7f8-580">Eigenschaft `maxSizeBytes` geändert (ist nun keine Zeichenfolge mehr, sondern ein Ganzzahlwert)</span><span class="sxs-lookup"><span data-stu-id="4b7f8-580">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="4b7f8-581">[WICHTIGE ÄNDERUNG] Die folgenden `db`- und `dw`-Eigenschaften wurden geändert und sind jetzt schreibgeschützt:</span><span class="sxs-lookup"><span data-stu-id="4b7f8-581">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="4b7f8-582">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-582">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="4b7f8-583">Verwenden Sie zum Aktualisieren den Parameter `--service-objective`, oder legen Sie die Eigenschaft `sku.name` fest.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-583">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="4b7f8-584">`edition`.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-584">`edition`.</span></span> <span data-ttu-id="4b7f8-585">Verwenden Sie zum Aktualisieren den Parameter `--edition`, oder legen Sie die Eigenschaft `sku.tier` fest.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-585">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="4b7f8-586">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-586">`elasticPoolName`.</span></span> <span data-ttu-id="4b7f8-587">Verwenden Sie zum Aktualisieren den Parameter `--elastic-pool`, oder legen Sie die Eigenschaft `elasticPoolId` fest.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-587">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="4b7f8-588">[WICHTIGE ÄNDERUNG] Die folgenden `elastic-pool`-Eigenschaften wurden geändert und sind jetzt schreibgeschützt:</span><span class="sxs-lookup"><span data-stu-id="4b7f8-588">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="4b7f8-589">`edition`.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-589">`edition`.</span></span> <span data-ttu-id="4b7f8-590">Verwenden Sie zum Aktualisieren den Parameter `--edition`.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-590">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="4b7f8-591">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-591">`dtu`.</span></span> <span data-ttu-id="4b7f8-592">Verwenden Sie zum Aktualisieren den Parameter `--capacity`.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-592">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="4b7f8-593">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-593">`databaseDtuMin`.</span></span> <span data-ttu-id="4b7f8-594">Verwenden Sie zum Aktualisieren den Parameter `--db-min-capacity`.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-594">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="4b7f8-595">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-595">`databaseDtuMax`.</span></span> <span data-ttu-id="4b7f8-596">Verwenden Sie zum Aktualisieren den Parameter `--db-max-capacity`.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-596">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="4b7f8-597">Die Parameter `--family` und `--capacity` wurden zu den `db`-, `dw`- und `elastic-pool`-Befehlen hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-597">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="4b7f8-598">Den `db`-, `dw`- und `elastic-pool`-Befehlen wurden Tabellenformatierer hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-598">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="4b7f8-599">Speicher</span><span class="sxs-lookup"><span data-stu-id="4b7f8-599">Storage</span></span>

* <span data-ttu-id="4b7f8-600">Vervollständigung für das Argument `--account-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-600">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="4b7f8-601">Problem mit `storage entity query` behoben</span><span class="sxs-lookup"><span data-stu-id="4b7f8-601">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="4b7f8-602">VM</span><span class="sxs-lookup"><span data-stu-id="4b7f8-602">VM</span></span>

* <span data-ttu-id="4b7f8-603">[WICHTIGE ÄNDERUNG] `--write-accelerator` aus `vm create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-603">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="4b7f8-604">Die gleiche Unterstützung kann über `vm update` oder `vm disk attach` erzielt werden.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-604">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="4b7f8-605">Erweiterungsimageabgleich in `[vm|vmss] extension` korrigiert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-605">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="4b7f8-606">`--boot-diagnostics-storage` zu `vm create` zur Erfassung des Startprotokolls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-606">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="4b7f8-607">`--license-type` zu `[vm|vmss] update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-607">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="4b7f8-608">7. Mai 2018</span><span class="sxs-lookup"><span data-stu-id="4b7f8-608">May 7, 2018</span></span>

<span data-ttu-id="4b7f8-609">Version 2.0.32</span><span class="sxs-lookup"><span data-stu-id="4b7f8-609">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="4b7f8-610">Core</span><span class="sxs-lookup"><span data-stu-id="4b7f8-610">Core</span></span>

* <span data-ttu-id="4b7f8-611">Ein Ausnahmefehler wurde behoben, der beim Abrufen von Geheimnissen aus einem Dienstprinzipalkonto mit Zertifikat auftrat.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-611">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="4b7f8-612">Eingeschränkte Unterstützung für positionelle Argumente hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-612">Added limited support for positional arguments</span></span>
* <span data-ttu-id="4b7f8-613">Problem behoben, aufgrund dessen `--query` nicht mit `--ids` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="4b7f8-613">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="4b7f8-614">#5591</span><span class="sxs-lookup"><span data-stu-id="4b7f8-614">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="4b7f8-615">Pipingszenarien von Befehlen bei Verwendung von `--ids` verbessert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-615">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="4b7f8-616">Unterstützt `-o tsv` mit angegebener Abfrage bzw. `-o json` ohne angegeben Abfrage</span><span class="sxs-lookup"><span data-stu-id="4b7f8-616">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="4b7f8-617">Befehlsvorschläge bei Fehler hinzugefügt, wenn Befehle Tippfehler enthielten</span><span class="sxs-lookup"><span data-stu-id="4b7f8-617">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="4b7f8-618">Fehler bei der Eingabe von `az ''` behandelt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-618">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="4b7f8-619">Unterstützung für benutzerdefinierte Ressourcentypen für Befehlsmodule und -erweiterungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-619">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="4b7f8-620">ACR</span><span class="sxs-lookup"><span data-stu-id="4b7f8-620">ACR</span></span>

* <span data-ttu-id="4b7f8-621">ACR Build-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-621">Added ACR Build commands</span></span>
* <span data-ttu-id="4b7f8-622">Fehlermeldungen vom Typ „Ressource nicht gefunden.“ verbessert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-622">Improved resource not found error messages</span></span>
* <span data-ttu-id="4b7f8-623">Höhere Leistung bei der Ressourcenerstellung und optimierte Fehlerbehandlung</span><span class="sxs-lookup"><span data-stu-id="4b7f8-623">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="4b7f8-624">ACR-Anmeldung bei nicht standardmäßigen Konsolen und WSL optimiert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-624">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="4b7f8-625">Fehlermeldungen zu Repositorybefehlen optimiert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-625">Improved repository commands error messages</span></span>
* <span data-ttu-id="4b7f8-626">Tabellenspalten und -reihenfolge aktualisiert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-626">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="4b7f8-627">ACS</span><span class="sxs-lookup"><span data-stu-id="4b7f8-627">ACS</span></span>

* <span data-ttu-id="4b7f8-628">Warnung hinzugefügt, dass `az aks` eine Vorschauversion des Diensts ist</span><span class="sxs-lookup"><span data-stu-id="4b7f8-628">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="4b7f8-629">Berechtigungsproblem in `aks install-connector` behoben, wenn `--aci-resource-group` nicht angegeben wird</span><span class="sxs-lookup"><span data-stu-id="4b7f8-629">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="4b7f8-630">AMS</span><span class="sxs-lookup"><span data-stu-id="4b7f8-630">AMS</span></span>

* <span data-ttu-id="4b7f8-631">Erste Version: Verwalten von Azure Media Services-Ressourcen</span><span class="sxs-lookup"><span data-stu-id="4b7f8-631">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="4b7f8-632">AppService</span><span class="sxs-lookup"><span data-stu-id="4b7f8-632">Appservice</span></span>

* <span data-ttu-id="4b7f8-633">Ein Problem in `webapp delete` wurde behoben, das bei Angabe von `--slot` auftrat.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-633">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="4b7f8-634">`--runtime-version` aus `webapp auth update` entfernt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-634">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="4b7f8-635">Unterstützung für „min\_tls\_version“ und „https2.0“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-635">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="4b7f8-636">Unterstützung für mehrere Container hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-636">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="4b7f8-637">Batch AI</span><span class="sxs-lookup"><span data-stu-id="4b7f8-637">Batch AI</span></span>

* <span data-ttu-id="4b7f8-638">`batchai create cluster` wurde geändert, um die in der Konfigurationsdatei des Clusters konfigurierte VM-Priorität zu berücksichtigen.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-638">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="4b7f8-639">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="4b7f8-639">Cognitive Services</span></span>

* <span data-ttu-id="4b7f8-640">Tippfehler im Beispiel für `cognitiveservices account create` korrigiert ([#5603](https://github.com/Azure/azure-cli/issues/5603))</span><span class="sxs-lookup"><span data-stu-id="4b7f8-640">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="4b7f8-641">Nutzung</span><span class="sxs-lookup"><span data-stu-id="4b7f8-641">Consumption</span></span>

* <span data-ttu-id="4b7f8-642">Neue Befehle für Budget-API hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-642">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="4b7f8-643">Container</span><span class="sxs-lookup"><span data-stu-id="4b7f8-643">Container</span></span>

* <span data-ttu-id="4b7f8-644">`--registry-server` muss nicht mehr für `container create` angegeben werden, wenn ein Registrierungsserver im Imagenamen enthalten ist.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-644">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="4b7f8-645">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="4b7f8-645">Cosmos DB</span></span>

* <span data-ttu-id="4b7f8-646">VNET-Unterstützung für Azure CLI eingeführt: Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="4b7f8-646">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="4b7f8-647">DMS</span><span class="sxs-lookup"><span data-stu-id="4b7f8-647">DMS</span></span>

* <span data-ttu-id="4b7f8-648">Erste Version: Die Migration von SQL zu Azure SQL wird nun unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-648">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="4b7f8-649">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="4b7f8-649">Extension</span></span>

* <span data-ttu-id="4b7f8-650">Fehler behoben, aufgrund dessen Erweiterungsmetadaten nicht mehr angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="4b7f8-650">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="4b7f8-651">Interactive</span><span class="sxs-lookup"><span data-stu-id="4b7f8-651">Interactive</span></span>

* <span data-ttu-id="4b7f8-652">Interaktive Vervollständigung funktioniert nun auch mit positionellen Argumenten.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-652">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="4b7f8-653">Benutzerfreundlichere Ausgabe bei der Eingabe von '\'</span><span class="sxs-lookup"><span data-stu-id="4b7f8-653">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="4b7f8-654">Abschlüsse für Parameter ohne Hilfe korrigiert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-654">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="4b7f8-655">Beschreibungen für Befehlsgruppen korrigiert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-655">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="4b7f8-656">Labor</span><span class="sxs-lookup"><span data-stu-id="4b7f8-656">Lab</span></span>

* <span data-ttu-id="4b7f8-657">Regressionen aus Knack-Umwandlung korrigiert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-657">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="4b7f8-658">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="4b7f8-658">Network</span></span>

* <span data-ttu-id="4b7f8-659">[WICHTIGE ÄNDERUNG] Parameter `--ids` entfernt für:</span><span class="sxs-lookup"><span data-stu-id="4b7f8-659">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="4b7f8-660">Profil</span><span class="sxs-lookup"><span data-stu-id="4b7f8-660">Profile</span></span>

* <span data-ttu-id="4b7f8-661">Quellerkennung für `disk create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-661">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="4b7f8-662">[WICHTIGE ÄNDERUNG] `--msi-port` und `--identity-port` entfernt, da sie nicht mehr verwendet werden</span><span class="sxs-lookup"><span data-stu-id="4b7f8-662">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="4b7f8-663">Tippfehler in kurzer Zusammenfassung für `account get-access-token` korrigiert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-663">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="4b7f8-664">Redis</span><span class="sxs-lookup"><span data-stu-id="4b7f8-664">Redis</span></span>

* <span data-ttu-id="4b7f8-665">`redis patch-schedule patch-schedule show` wurde durch `redis patch-schedule show` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-665">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="4b7f8-666">`redis list-all` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-666">Deprecated `redis list-all`.</span></span> <span data-ttu-id="4b7f8-667">Diese Funktion wurde in `redis list` integriert.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-667">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="4b7f8-668">`redis import-method` wurde durch `redis import` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-668">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="4b7f8-669">Unterstützung für `--ids` zu verschiedenen Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-669">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="4b7f8-670">Rolle</span><span class="sxs-lookup"><span data-stu-id="4b7f8-670">Role</span></span>

* <span data-ttu-id="4b7f8-671">[WICHTIGE ÄNDERUNG] Veralteter Befehl `ad sp reset-credentials` entfernt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-671">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="4b7f8-672">Speicher</span><span class="sxs-lookup"><span data-stu-id="4b7f8-672">Storage</span></span>

* <span data-ttu-id="4b7f8-673">Zulassen, dass das Ziel-SAS-Token für die Blobkopie auf die Quelle angewendet wird, wenn Quell-SAS und Kontoschlüssel nicht angegeben werden</span><span class="sxs-lookup"><span data-stu-id="4b7f8-673">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="4b7f8-674">Verfügbar gemacht: Socket-Timeout für Blobuploads und -downloads</span><span class="sxs-lookup"><span data-stu-id="4b7f8-674">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="4b7f8-675">Blobnamen, die mit Pfadtrennzeichen beginnen, als relative Pfade behandeln</span><span class="sxs-lookup"><span data-stu-id="4b7f8-675">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="4b7f8-676">Zulassen, dass `storage blob copy --source-sas` mit dem Abfragezeichen „?“ beginnt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-676">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="4b7f8-677">`storage entity query --marker` korrigiert, um Liste von Schlüsselwerten zu akzeptieren</span><span class="sxs-lookup"><span data-stu-id="4b7f8-677">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="4b7f8-678">VM</span><span class="sxs-lookup"><span data-stu-id="4b7f8-678">VM</span></span>

* <span data-ttu-id="4b7f8-679">Ungültige Erkennungslogik für nicht verwalteten Blob-URI korrigiert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-679">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="4b7f8-680">Unterstützung für Datenträgerverschlüsselung ohne vom Benutzer bereitgestellte Dienstprinzipale hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-680">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="4b7f8-681">[WICHTIGE ÄNDERUNG] Verwenden Sie nicht „ManagedIdentityExtension“ des virtuellen Computers für MSI-Unterstützung.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-681">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="4b7f8-682">Unterstützung für Entfernungsrichtlinie zu `vmss` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-682">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="4b7f8-683">[WICHTIGE ÄNDERUNG] `--ids` entfernt aus:</span><span class="sxs-lookup"><span data-stu-id="4b7f8-683">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="4b7f8-684">Unterstützung für Schreibbeschleunigung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-684">Added write accelerator support</span></span>
* <span data-ttu-id="4b7f8-685">`vmss perform-maintenance` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-685">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="4b7f8-686">`vm diagnostics set` korrigiert, um zuverlässig den Betriebssystemtyp des virtuellen Computers zu erkennen</span><span class="sxs-lookup"><span data-stu-id="4b7f8-686">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="4b7f8-687">`vm resize` geändert, um zu überprüfen, ob die angeforderte Größe von der derzeit festgelegten Größe abweicht, und nur bei einer Änderung eine Aktualisierung auszuführen</span><span class="sxs-lookup"><span data-stu-id="4b7f8-687">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="4b7f8-688">10. April 2018</span><span class="sxs-lookup"><span data-stu-id="4b7f8-688">April 10, 2018</span></span>

<span data-ttu-id="4b7f8-689">Version 2.0.31</span><span class="sxs-lookup"><span data-stu-id="4b7f8-689">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="4b7f8-690">ACR</span><span class="sxs-lookup"><span data-stu-id="4b7f8-690">ACR</span></span>

* <span data-ttu-id="4b7f8-691">Verbesserte Fehlerbehandlung für wincred-Fallback</span><span class="sxs-lookup"><span data-stu-id="4b7f8-691">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="4b7f8-692">ACS</span><span class="sxs-lookup"><span data-stu-id="4b7f8-692">ACS</span></span>

* <span data-ttu-id="4b7f8-693">Gültigkeit von per AKS erstellten SPNs in fünf Jahre geändert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-693">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="4b7f8-694">AppService</span><span class="sxs-lookup"><span data-stu-id="4b7f8-694">Appservice</span></span>

* [WICHTIGE ÄNDERUNG]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="4b7f8-696">Nicht abgefangene Ausnahme für nicht vorhandene Web-App-Pläne behoben</span><span class="sxs-lookup"><span data-stu-id="4b7f8-696">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="4b7f8-697">Batch AI</span><span class="sxs-lookup"><span data-stu-id="4b7f8-697">BatchAI</span></span>

* <span data-ttu-id="4b7f8-698">Unterstützung für API 2018-03-01 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-698">Added support for 2018-03-01 API</span></span>

 - <span data-ttu-id="4b7f8-699">Bereitstellung auf Auftragsebene</span><span class="sxs-lookup"><span data-stu-id="4b7f8-699">Job level mounting</span></span>
 - <span data-ttu-id="4b7f8-700">Umgebungsvariablen mit Geheimniswerten</span><span class="sxs-lookup"><span data-stu-id="4b7f8-700">Environment variables with secret values</span></span>
 - <span data-ttu-id="4b7f8-701">Einstellungen von Leistungsindikatoren</span><span class="sxs-lookup"><span data-stu-id="4b7f8-701">Performance counters settings</span></span>
 - <span data-ttu-id="4b7f8-702">Berichtstellung für auftragsspezifisches Pfadsegment</span><span class="sxs-lookup"><span data-stu-id="4b7f8-702">Reporting of job specific path segment</span></span>
 - <span data-ttu-id="4b7f8-703">Unterstützung für Unterordner in Listendateien-API</span><span class="sxs-lookup"><span data-stu-id="4b7f8-703">Support for subfolders in list files api</span></span>
 - <span data-ttu-id="4b7f8-704">Berichterstellung zur Nutzung und zu Grenzwerten</span><span class="sxs-lookup"><span data-stu-id="4b7f8-704">Usage and limits reporting</span></span>
 - <span data-ttu-id="4b7f8-705">Zulassen der Angabe des Cachetyps für NFS-Server</span><span class="sxs-lookup"><span data-stu-id="4b7f8-705">Allow to specify caching type for NFS servers</span></span>
 - <span data-ttu-id="4b7f8-706">Unterstützung für benutzerdefinierte Images</span><span class="sxs-lookup"><span data-stu-id="4b7f8-706">Support for custom images</span></span>
 - <span data-ttu-id="4b7f8-707">Unterstützung für pyTorch-Toolkit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-707">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="4b7f8-708">Befehl `job wait` hinzugefügt, der das Warten auf die Auftragsfertigstellung ermöglicht und den Code für die Auftragsbeendigung meldet</span><span class="sxs-lookup"><span data-stu-id="4b7f8-708">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="4b7f8-709">Befehl `usage show` hinzugefügt, mit dem die aktuelle Nutzung von Batch AI-Ressourcen und die Grenzwerte für verschiedene Regionen aufgelistet werden</span><span class="sxs-lookup"><span data-stu-id="4b7f8-709">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="4b7f8-710">Nationale Clouds werden unterstützt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-710">National clouds are supported</span></span>
* <span data-ttu-id="4b7f8-711">Befehlszeilenargumente für Aufträge hinzugefügt, um das Bereitstellen von Dateisystemen auf Auftragsebene zusätzlich zu Konfigurationsdateien zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="4b7f8-711">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="4b7f8-712">Weitere Optionen zum Anpassen von Clustern hinzugefügt – VM-Priorität, Subnetz, anfängliche Knotenanzahl für Cluster mit automatischer Skalierung, Angeben eines benutzerdefinierten Images</span><span class="sxs-lookup"><span data-stu-id="4b7f8-712">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="4b7f8-713">Befehlszeilenoption zum Angeben des Cachetyps für NFS mit Verwaltung per Batch AI hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-713">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="4b7f8-714">Angeben der Bereitstellung von Dateisystemen in Konfigurationsdateien vereinfacht.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-714">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="4b7f8-715">Weglassen von Anmeldeinformationen für Azure-Dateifreigaben und Azure-Blobcontainer ist jetzt möglich. Die CLI füllt fehlende Anmeldeinformationen auf, indem der Speicherkontoschlüssel verwendet wird, der über Befehlszeilenparameter oder per Umgebungsvariable angegeben wird, oder der Schlüssel wird über Azure Storage abgefragt (sofern das Speicherkonto zum aktuellen Abonnement gehört).</span><span class="sxs-lookup"><span data-stu-id="4b7f8-715">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="4b7f8-716">Der Befehl zum Streamen von Auftragsdateien wird jetzt automatisch abgeschlossen, nachdem der Auftrag beendet ist (Erfolg, Fehler, Beendigung oder Löschung)</span><span class="sxs-lookup"><span data-stu-id="4b7f8-716">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="4b7f8-717">Verbesserte `table`-Ausgabe für `show`-Vorgänge</span><span class="sxs-lookup"><span data-stu-id="4b7f8-717">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="4b7f8-718">Option `--use-auto-storage` für die Clustererstellung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-718">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="4b7f8-719">Diese Option erleichtert die Verwaltung von Speicherkonten und die Bereitstellung von Azure-Dateifreigaben und Azure-Blobcontainern in Clustern.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-719">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="4b7f8-720">`--generate-ssh-keys` für `cluster create` und `file-server create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-720">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="4b7f8-721">Möglichkeit zum Angeben der Knotensetupaufgabe über die Befehlszeile</span><span class="sxs-lookup"><span data-stu-id="4b7f8-721">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="4b7f8-722">[WICHTIGE ÄNDERUNG] Befehl `job stream-file` und `job list-files` in die Gruppe `job file` verschoben</span><span class="sxs-lookup"><span data-stu-id="4b7f8-722">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="4b7f8-723">[WICHTIGE ÄNDERUNG] `--admin-user-name` im Befehl `file-server create` in `--user-name` umbenannt, um Einheitlichkeit mit dem Befehl `cluster create` zu erzielen</span><span class="sxs-lookup"><span data-stu-id="4b7f8-723">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="4b7f8-724">Abrechnung</span><span class="sxs-lookup"><span data-stu-id="4b7f8-724">Billing</span></span>

* <span data-ttu-id="4b7f8-725">Registrierungskontobefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-725">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="4b7f8-726">Nutzung</span><span class="sxs-lookup"><span data-stu-id="4b7f8-726">Consumption</span></span>

* <span data-ttu-id="4b7f8-727">Befehle vom Typ `marketplace` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-727">Added `marketplace` commands</span></span>
* <span data-ttu-id="4b7f8-728">[WICHTIGE ÄNDERUNG] `reservations summaries` in `reservation summary` umbenannt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-728">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="4b7f8-729">[WICHTIGE ÄNDERUNG] `reservations details` in `reservation detail` umbenannt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-729">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="4b7f8-730">[WICHTIGE ÄNDERUNG] Kurzoptionen `--reservation-order-id` und `--reservation-id` für `reservation`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-730">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="4b7f8-731">[WICHTIGE ÄNDERUNG] `--grain`-Kurzoptionen für `reservation summary`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-731">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="4b7f8-732">[WICHTIGE ÄNDERUNG] `--include-meter-details`-Kurzoptionen für `pricesheet`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-732">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="4b7f8-733">Container</span><span class="sxs-lookup"><span data-stu-id="4b7f8-733">Container</span></span>

* <span data-ttu-id="4b7f8-734">Git-Repository-Parameter `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` und `--gitrepo-mount-path` für die Volumebereitstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-734">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="4b7f8-735">[#5926](https://github.com/Azure/azure-cli/issues/5926) behoben: Fehler bei `az container exec`, wenn „--container-name“ angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="4b7f8-735">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="4b7f8-736">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="4b7f8-736">Extension</span></span>

* <span data-ttu-id="4b7f8-737">Meldung für Distributionsüberprüfung in Debugebene geändert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-737">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="4b7f8-738">Interactive</span><span class="sxs-lookup"><span data-stu-id="4b7f8-738">Interactive</span></span>

* <span data-ttu-id="4b7f8-739">Geändert: Verhinderung des Abschlusses bei nicht erkannten Befehlen</span><span class="sxs-lookup"><span data-stu-id="4b7f8-739">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="4b7f8-740">Ereignishooks vor und nach der Erstellung der Teilstruktur von Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-740">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="4b7f8-741">Abschluss für `--ids`-Parameter hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-741">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="4b7f8-742">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="4b7f8-742">Network</span></span>

* <span data-ttu-id="4b7f8-743">[#5936](https://github.com/Azure/azure-cli/issues/5936) behoben: `application-gateway create`-Tags konnten nicht festgelegt werden</span><span class="sxs-lookup"><span data-stu-id="4b7f8-743">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="4b7f8-744">Argument `--auth-certs` zum Anfügen von Authentifizierungszertifikaten für `application-gateway http-settings [create|update]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-744">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="4b7f8-745">#4910</span><span class="sxs-lookup"><span data-stu-id="4b7f8-745">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="4b7f8-746">`ddos-protection`-Befehle zum Erstellen von DDoS-Schutzplänen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-746">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="4b7f8-747">Unterstützung von `--ddos-protection-plan` für `vnet [create|update]` hinzugefügt, um das Zuordnen eines VNET zu einem DDoS-Schutzplan zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="4b7f8-747">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="4b7f8-748">Problem mit `--disable-bgp-route-propagation`-Flag in `network route-table [create|update]` behoben</span><span class="sxs-lookup"><span data-stu-id="4b7f8-748">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="4b7f8-749">Dummy-Argumente `--public-ip-address-type` und `--subnet-type` für `network lb [create|update]` entfernt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-749">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="4b7f8-750">Unterstützung für TXT-Datensätze mit RFC 1035-Escapesequenzen für `network dns zone [import|export]` und `network dns record-set txt add-record` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-750">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="4b7f8-751">Profil</span><span class="sxs-lookup"><span data-stu-id="4b7f8-751">Profile</span></span>

* <span data-ttu-id="4b7f8-752">Unterstützung für klassische Azure-Konten in `account list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-752">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="4b7f8-753">[WICHTIGE ÄNDERUNG] `--msi` & `--msi-port`-Argumente entfernt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-753">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="4b7f8-754">RDBMS</span><span class="sxs-lookup"><span data-stu-id="4b7f8-754">RDBMS</span></span>

* <span data-ttu-id="4b7f8-755">Befehl `georestore` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-755">Added `georestore` command</span></span>
* <span data-ttu-id="4b7f8-756">Speichergrößenbeschränkung aus Befehl `create` entfernt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-756">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="4b7f8-757">Ressource</span><span class="sxs-lookup"><span data-stu-id="4b7f8-757">Resource</span></span>

* <span data-ttu-id="4b7f8-758">Unterstützung für `--metadata` zu `policy definition create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-758">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="4b7f8-759">Unterstützung von `--metadata`, `--set`, `--add`, `--remove` für `policy definition update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-759">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="4b7f8-760">SQL</span><span class="sxs-lookup"><span data-stu-id="4b7f8-760">SQL</span></span>

* <span data-ttu-id="4b7f8-761">`sql elastic-pool op list` und `sql elastic-pool op cancel` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-761">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="4b7f8-762">Speicher</span><span class="sxs-lookup"><span data-stu-id="4b7f8-762">Storage</span></span>

* <span data-ttu-id="4b7f8-763">Fehlermeldungen für falsch formatierte Verbindungszeichenfolgen verbessert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-763">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="4b7f8-764">VM</span><span class="sxs-lookup"><span data-stu-id="4b7f8-764">VM</span></span>

* <span data-ttu-id="4b7f8-765">Unterstützung für die Konfiguration der Plattform-Fehlerdomänenanzahl für `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-765">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="4b7f8-766">`vmss create` geändert, damit standardmäßig „Standard LB“ für zonales, großes oder per einzelner Platzierungsgruppe deaktiviertes Scale Set festgelegt wird</span><span class="sxs-lookup"><span data-stu-id="4b7f8-766">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [WICHTIGE ÄNDERUNG]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="4b7f8-768">Unterstützung für SKU mit öffentlicher IP für `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-768">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="4b7f8-769">Argumente `--keyvault` und `--resource-group` für `vm secret format` hinzugefügt, um Szenarien zu unterstützen, bei denen der Befehl die Tresor-ID nicht auflösen kann.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-769">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="4b7f8-770">#5718</span><span class="sxs-lookup"><span data-stu-id="4b7f8-770">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="4b7f8-771">Bessere Fehler für `[vm|vmss create]`, wenn der Standort einer Ressourcengruppe keine Zonenunterstützung aufweist</span><span class="sxs-lookup"><span data-stu-id="4b7f8-771">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="4b7f8-772">27. März 2018</span><span class="sxs-lookup"><span data-stu-id="4b7f8-772">March 27, 2018</span></span>

<span data-ttu-id="4b7f8-773">Version 2.0.30</span><span class="sxs-lookup"><span data-stu-id="4b7f8-773">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="4b7f8-774">Core</span><span class="sxs-lookup"><span data-stu-id="4b7f8-774">Core</span></span>

* <span data-ttu-id="4b7f8-775">Anzeigen einer Meldung für Erweiterungen, die in der Hilfe als Vorschauversion gekennzeichnet sind</span><span class="sxs-lookup"><span data-stu-id="4b7f8-775">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="4b7f8-776">ACS</span><span class="sxs-lookup"><span data-stu-id="4b7f8-776">ACS</span></span>

* <span data-ttu-id="4b7f8-777">Behebung eines Fehlers bei der SSL-Zertifikatprüfung für `aks install-cli` in Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="4b7f8-777">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="4b7f8-778">AppService</span><span class="sxs-lookup"><span data-stu-id="4b7f8-778">Appservice</span></span>

* <span data-ttu-id="4b7f8-779">Unterstützung nur von HTTPS zu `webapp update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-779">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="4b7f8-780">Unterstützung für Slots zu `az webapp identity [assign|show]` und `az functionapp identity [assign|show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-780">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="4b7f8-781">Backup</span><span class="sxs-lookup"><span data-stu-id="4b7f8-781">Backup</span></span>

* <span data-ttu-id="4b7f8-782">Neuer Befehl `az backup protection isenabled-for-vm` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-782">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="4b7f8-783">Mit diesem Befehl kann überprüft werden, ob ein virtueller Computer von einem beliebigen Tresor im Abonnement gesichert wird.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-783">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="4b7f8-784">Azure-Objekt-IDs für Parameter `--resource-group` und `--vault-name` für die folgenden Befehle aktiviert:</span><span class="sxs-lookup"><span data-stu-id="4b7f8-784">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="4b7f8-785">`--name`-Parameter wurden geändert, um das Ausgabeformat von `backup ... show`-Befehlen zu akzeptieren.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-785">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="4b7f8-786">Container</span><span class="sxs-lookup"><span data-stu-id="4b7f8-786">Container</span></span>

* <span data-ttu-id="4b7f8-787">Befehl `container exec` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-787">Added `container exec` command.</span></span> <span data-ttu-id="4b7f8-788">Ausführung von Befehlen in einem Container für eine ausgeführte Containergruppe</span><span class="sxs-lookup"><span data-stu-id="4b7f8-788">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="4b7f8-789">Zulassen der Tabellenausgabe zum Erstellen und Aktualisieren einer Containergruppe</span><span class="sxs-lookup"><span data-stu-id="4b7f8-789">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="4b7f8-790">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="4b7f8-790">Extension</span></span>

* <span data-ttu-id="4b7f8-791">Meldung für `extension add` hinzugefügt, wenn sich die Erweiterung in der Vorschauphase befindet</span><span class="sxs-lookup"><span data-stu-id="4b7f8-791">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="4b7f8-792">`extension list-available` geändert, um vollständige Erweiterungsdaten mit `--show-details` anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="4b7f8-792">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="4b7f8-793">[WICHTIGE ÄNDERUNG] `extension list-available` geändert, um standardmäßig vereinfachte Erweiterungsdaten anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="4b7f8-793">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="4b7f8-794">Interactive</span><span class="sxs-lookup"><span data-stu-id="4b7f8-794">Interactive</span></span>

* <span data-ttu-id="4b7f8-795">Vervollständigungen wurden geändert und werden jetzt aktiviert, sobald das Laden der Befehlstabelle abgeschlossen ist.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-795">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="4b7f8-796">Fehler bei der Verwendung des Parameters `--style` behoben</span><span class="sxs-lookup"><span data-stu-id="4b7f8-796">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="4b7f8-797">Interaktiver Lexer nach Befehlstabellensicherung instanziiert (sofern nicht vorhanden)</span><span class="sxs-lookup"><span data-stu-id="4b7f8-797">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="4b7f8-798">Verbesserte Unterstützung der Vervollständigung</span><span class="sxs-lookup"><span data-stu-id="4b7f8-798">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="4b7f8-799">Labor</span><span class="sxs-lookup"><span data-stu-id="4b7f8-799">Lab</span></span>

* <span data-ttu-id="4b7f8-800">Probleme mit Befehl `create environment` behoben</span><span class="sxs-lookup"><span data-stu-id="4b7f8-800">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="4b7f8-801">Überwachen</span><span class="sxs-lookup"><span data-stu-id="4b7f8-801">Monitor</span></span>

* <span data-ttu-id="4b7f8-802">Unterstützung für `--top`, `--orderby` und `--namespace` zu `metrics list` hinzugefügt ([#5785](https://github.com/Azure/azure-cli/issues/5785))</span><span class="sxs-lookup"><span data-stu-id="4b7f8-802">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="4b7f8-803">[#4529](https://github.com/Azure/azure-cli/issues/5785) behoben: `metrics list` akzeptiert eine durch Leerzeichen getrennte Liste von abzurufenden Metriken.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-803">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="4b7f8-804">Unterstützung für `--namespace` zu `metrics list-definitions` hinzugefügt ([#5785](https://github.com/Azure/azure-cli/issues/5785))</span><span class="sxs-lookup"><span data-stu-id="4b7f8-804">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="4b7f8-805">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="4b7f8-805">Network</span></span>

* <span data-ttu-id="4b7f8-806">Unterstützung für private DNS-Zonen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-806">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="4b7f8-807">Profil</span><span class="sxs-lookup"><span data-stu-id="4b7f8-807">Profile</span></span>

* <span data-ttu-id="4b7f8-808">Warnung für `--identity-port` und `--msi-port` zu `login` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-808">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="4b7f8-809">RDBMS</span><span class="sxs-lookup"><span data-stu-id="4b7f8-809">RDBMS</span></span>

* <span data-ttu-id="4b7f8-810">GA-API-Version 2017-12-01 (Geschäftsmodell) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-810">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="4b7f8-811">Ressource</span><span class="sxs-lookup"><span data-stu-id="4b7f8-811">Resource</span></span>

* [WICHTIGE ÄNDERUNG]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="4b7f8-813">Rolle</span><span class="sxs-lookup"><span data-stu-id="4b7f8-813">Role</span></span>

* <span data-ttu-id="4b7f8-814">Unterstützung für erforderliche Zugriffskonfigurationen und native Clients zu `az ad app create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-814">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="4b7f8-815">`rbac`-Befehle geändert, um maximal 1.000 IDs für Objektauflösung zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="4b7f8-815">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="4b7f8-816">Befehle zur Verwaltung von Anmeldeinformationen (`ad sp credential [reset|list|delete]`) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-816">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="4b7f8-817">[WICHTIGE ÄNDERUNG] „properties“ aus `az role assignment [list|show]`-Ausgabe entfernt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-817">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="4b7f8-818">Unterstützung für `dataActions`- und `notDataActions`-Berechtigungen zu `role definition` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-818">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="4b7f8-819">Speicher</span><span class="sxs-lookup"><span data-stu-id="4b7f8-819">Storage</span></span>

* <span data-ttu-id="4b7f8-820">Problem beim Hochladen von Dateien mit einer Größe von 195 GB bis 200 GB behoben</span><span class="sxs-lookup"><span data-stu-id="4b7f8-820">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="4b7f8-821">[#4049](https://github.com/Azure/azure-cli/issues/4049) behoben: Probleme bei Uploads von Anfügeblobs behoben, die ein Ignorieren der Bedingungsparameter verursachten</span><span class="sxs-lookup"><span data-stu-id="4b7f8-821">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="4b7f8-822">VM</span><span class="sxs-lookup"><span data-stu-id="4b7f8-822">VM</span></span>

* <span data-ttu-id="4b7f8-823">Warnung für anstehende wichtige Änderungen für Sätze mit mehr als 100 Instanzen zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-823">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="4b7f8-824">Unterstützung der Zonenresilienz zu `vm [snapshot|image]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-824">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="4b7f8-825">Datenträgerinstanzansicht geändert, um besseren Verschlüsselungsstatus zu melden</span><span class="sxs-lookup"><span data-stu-id="4b7f8-825">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="4b7f8-826">[WICHTIGE ÄNDERUNG] `vm extension delete` geändert, um keine Ausgabe mehr zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="4b7f8-826">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="4b7f8-827">13. März 2018</span><span class="sxs-lookup"><span data-stu-id="4b7f8-827">March 13, 2018</span></span>

<span data-ttu-id="4b7f8-828">Version 2.0.29</span><span class="sxs-lookup"><span data-stu-id="4b7f8-828">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="4b7f8-829">ACR</span><span class="sxs-lookup"><span data-stu-id="4b7f8-829">ACR</span></span>

* <span data-ttu-id="4b7f8-830">Unterstützung für den Parameter `--image` zu `repository delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-830">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="4b7f8-831">Parameter `--manifest` und `--tag` des Befehls `repository delete` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-831">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="4b7f8-832">Befehl `repository untag` zum Entfernen eines Tags ohne das Löschen von Daten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-832">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="4b7f8-833">ACS</span><span class="sxs-lookup"><span data-stu-id="4b7f8-833">ACS</span></span>

* <span data-ttu-id="4b7f8-834">Befehl `aks upgrade-connector` zum Aktualisieren eines vorhandenen Connectors hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-834">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="4b7f8-835">`kubectl`-Konfigurationsdateien zur Verwendung von besser lesbarem YAML im Blockstil geändert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-835">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="4b7f8-836">Advisor</span><span class="sxs-lookup"><span data-stu-id="4b7f8-836">Advisor</span></span>

* <span data-ttu-id="4b7f8-837">[WICHTIGE ÄNDERUNG] `advisor configuration get` in `advisor configuration list` umbenannt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-837">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="4b7f8-838">[WICHTIGE ÄNDERUNG] `advisor configuration set` in `advisor configuration update` umbenannt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-838">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="4b7f8-839">[WICHTIGE ÄNDERUNG] `advisor recommendation generate` entfernt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-839">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="4b7f8-840">Parameter `--refresh` zu `advisor recommendation list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-840">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="4b7f8-841">Befehl `advisor recommendation show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-841">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="4b7f8-842">AppService</span><span class="sxs-lookup"><span data-stu-id="4b7f8-842">Appservice</span></span>

* <span data-ttu-id="4b7f8-843">`[webapp|functionapp] assign-identity` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-843">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="4b7f8-844">Befehle `webapp identity [assign|show]` und `functionapp identity [assign|show]` für verwaltete Identität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-844">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="4b7f8-845">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="4b7f8-845">Eventhubs</span></span>

* <span data-ttu-id="4b7f8-846">Erste Version</span><span class="sxs-lookup"><span data-stu-id="4b7f8-846">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="4b7f8-847">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="4b7f8-847">Extension</span></span>

* <span data-ttu-id="4b7f8-848">Überprüfung zum Warnen von Benutzern hinzugefügt, wenn sich die verwendete Distribution von der in der Paketquelldatei gespeicherten Distribution unterscheidet, da dies Fehlern führen kann</span><span class="sxs-lookup"><span data-stu-id="4b7f8-848">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="4b7f8-849">Interactive</span><span class="sxs-lookup"><span data-stu-id="4b7f8-849">Interactive</span></span>

* <span data-ttu-id="4b7f8-850">[#5625](https://github.com/Azure/azure-cli/issues/5625) behoben: Verlauf über verschiedene Sitzungen hinweg beibehalten</span><span class="sxs-lookup"><span data-stu-id="4b7f8-850">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="4b7f8-851">[#3016](https://github.com/Azure/azure-cli/issues/3016) behoben: Verlauf nicht aufgezeichnet, obwohl er innerhalb des Bereichs liegt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-851">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="4b7f8-852">[#5688](https://github.com/Azure/azure-cli/issues/5688) behoben: Abschlüsse nicht angezeigt, wenn beim Laden der Befehlstabelle Ausnahme auftrat</span><span class="sxs-lookup"><span data-stu-id="4b7f8-852">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="4b7f8-853">Statusanzeige für lang ausgeführte Vorgänge korrigiert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-853">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="4b7f8-854">Überwachen</span><span class="sxs-lookup"><span data-stu-id="4b7f8-854">Monitor</span></span>

* <span data-ttu-id="4b7f8-855">`monitor autoscale-settings`-Befehle als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-855">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="4b7f8-856">Befehle vom Typ `monitor autoscale` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-856">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="4b7f8-857">Befehle vom Typ `monitor autoscale profile` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-857">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="4b7f8-858">Befehle vom Typ `monitor autoscale rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-858">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="4b7f8-859">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="4b7f8-859">Network</span></span>

* <span data-ttu-id="4b7f8-860">[WICHTIGE ÄNDERUNG] Parameter `--tags` aus `route-filter rule create` entfernt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-860">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="4b7f8-861">Einige fehlerhafte Standardwerte für die folgenden Befehle entfernt:</span><span class="sxs-lookup"><span data-stu-id="4b7f8-861">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="4b7f8-862">`network watcher connection-monitor`-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-862">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="4b7f8-863">Parameter `--vnet` und `--subnet` zu `network watcher show-topology` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-863">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="4b7f8-864">Profil</span><span class="sxs-lookup"><span data-stu-id="4b7f8-864">Profile</span></span>

* <span data-ttu-id="4b7f8-865">Parameter `--msi` für `az login` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-865">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="4b7f8-866">Parameter `--identity` für `az login` als Ersatz vor `--msi` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-866">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="4b7f8-867">RDBMS</span><span class="sxs-lookup"><span data-stu-id="4b7f8-867">RDBMS</span></span>

* <span data-ttu-id="4b7f8-868">[VORSCHAU] Geändert, sodass die API „2017-12-01-preview“ verwendet wird</span><span class="sxs-lookup"><span data-stu-id="4b7f8-868">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="4b7f8-869">Service Bus</span><span class="sxs-lookup"><span data-stu-id="4b7f8-869">Service Bus</span></span>

* <span data-ttu-id="4b7f8-870">Erste Version</span><span class="sxs-lookup"><span data-stu-id="4b7f8-870">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="4b7f8-871">Speicher</span><span class="sxs-lookup"><span data-stu-id="4b7f8-871">Storage</span></span>

* <span data-ttu-id="4b7f8-872">[#4971](https://github.com/Azure/azure-cli/issues/4971) behoben: `storage blob copy` unterstützt jetzt andere Azure-Clouds.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-872">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="4b7f8-873">[#5286](https://github.com/Azure/azure-cli/issues/5286) behoben: `storage blob [delete-batch|download-batch|upload-batch]`-Batchbefehle lösen bei Vorbedingungsfehlern keinen Fehler mehr aus.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-873">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="4b7f8-874">VM</span><span class="sxs-lookup"><span data-stu-id="4b7f8-874">VM</span></span>

* <span data-ttu-id="4b7f8-875">`[vm|vmss] create` unterstützt jetzt das Anfügen nicht verwalteter Datenträger und das Konfigurieren der Zwischenspeicherung.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-875">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="4b7f8-876">`[vm|vmss] assign-identity` und `[vm|vmss] remove-identity` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-876">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="4b7f8-877">Befehle `vm identity [assign|remove|show]` und `vmss identity [assign|remove|show]` als Ersatz für veraltete Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-877">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="4b7f8-878">Standardpriorität in `vmss create` auf „Keine“ geändert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-878">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="4b7f8-879">27. Februar 2018</span><span class="sxs-lookup"><span data-stu-id="4b7f8-879">February 27, 2018</span></span>

<span data-ttu-id="4b7f8-880">Version 2.0.28</span><span class="sxs-lookup"><span data-stu-id="4b7f8-880">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="4b7f8-881">Core</span><span class="sxs-lookup"><span data-stu-id="4b7f8-881">Core</span></span>

* <span data-ttu-id="4b7f8-882">[5184](https://github.com/Azure/azure-cli/issues/5184) (Problem beim Installieren von Homebrew) behoben</span><span class="sxs-lookup"><span data-stu-id="4b7f8-882">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="4b7f8-883">Unterstützung für Erweiterungstelemetrie mit benutzerdefinierten Schlüsseln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-883">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="4b7f8-884">HTTP-Protokollierung zu `--debug` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-884">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="4b7f8-885">ACS</span><span class="sxs-lookup"><span data-stu-id="4b7f8-885">ACS</span></span>

* <span data-ttu-id="4b7f8-886">Geändert, sodass für `aks install-connector` standardmäßig das Helm-Diagramm `virtual-kubelet-for-aks` verwendet wird</span><span class="sxs-lookup"><span data-stu-id="4b7f8-886">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="4b7f8-887">Problem behoben: Unzureichende Berechtigungen für Dienstprinzipale zum Erstellen einer ACI-Containergruppe</span><span class="sxs-lookup"><span data-stu-id="4b7f8-887">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="4b7f8-888">Parameter `--aci-container-group`, `--location` und `--image-tag` zu `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-888">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="4b7f8-889">Veraltungshinweis aus `aks get-versions` entfernt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-889">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="4b7f8-890">AppService</span><span class="sxs-lookup"><span data-stu-id="4b7f8-890">Appservice</span></span>

* <span data-ttu-id="4b7f8-891">Updates für die neue SDK-Version (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="4b7f8-891">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="4b7f8-892">[5538](https://github.com/Azure/azure-cli/issues/5538) behoben: `Free` wurde als ungültige SKU gemeldet.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-892">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="4b7f8-893">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="4b7f8-893">Cognitive Services</span></span>

* <span data-ttu-id="4b7f8-894">Hinweis beim Erstellen eines neuen Cognitive Services-Kontos aktualisiert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-894">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="4b7f8-895">Nutzung</span><span class="sxs-lookup"><span data-stu-id="4b7f8-895">Consumption</span></span>

* <span data-ttu-id="4b7f8-896">Neue Befehle für PriceSheet-API hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-896">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="4b7f8-897">Vorhandene Formate für Nutzungsdetails und Reservierungsdetails aktualisiert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-897">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="4b7f8-898">Container</span><span class="sxs-lookup"><span data-stu-id="4b7f8-898">Container</span></span>

* <span data-ttu-id="4b7f8-899">Argumente `--secrets` und `--secrets-mount-path` zu `container create` hinzugefügt, um Geheimnisse in ACI verwenden zu können</span><span class="sxs-lookup"><span data-stu-id="4b7f8-899">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="4b7f8-900">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="4b7f8-900">Network</span></span>

* <span data-ttu-id="4b7f8-901">[5559](https://github.com/Azure/azure-cli/issues/5559) behoben: Fehlender Client in `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="4b7f8-901">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="4b7f8-902">Ressource</span><span class="sxs-lookup"><span data-stu-id="4b7f8-902">Resource</span></span>

* <span data-ttu-id="4b7f8-903">`group deployment export` geändert, um eine partielle Vorlage und ggf. Fehler anzuzeigen, wenn der Vorgang nicht erfolgreich war</span><span class="sxs-lookup"><span data-stu-id="4b7f8-903">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="4b7f8-904">Rolle</span><span class="sxs-lookup"><span data-stu-id="4b7f8-904">Role</span></span>

* <span data-ttu-id="4b7f8-905">`role assignment list-changelogs` hinzugefügt, um die Überprüfung von Dienstprinzipalrollen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="4b7f8-905">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="4b7f8-906">SQL</span><span class="sxs-lookup"><span data-stu-id="4b7f8-906">SQL</span></span>

* <span data-ttu-id="4b7f8-907">Zonenredundanzunterstützung für Datenbanken und Pools für elastische Datenbanken hinzugefügt (bei Erstellung und Aktualisierung)</span><span class="sxs-lookup"><span data-stu-id="4b7f8-907">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="4b7f8-908">Speicher</span><span class="sxs-lookup"><span data-stu-id="4b7f8-908">Storage</span></span>

* <span data-ttu-id="4b7f8-909">Angabe von Zielpfad/Präfix für `storage blob [upload-batch|download-batch]` ermöglicht</span><span class="sxs-lookup"><span data-stu-id="4b7f8-909">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="4b7f8-910">VM</span><span class="sxs-lookup"><span data-stu-id="4b7f8-910">VM</span></span>

* <span data-ttu-id="4b7f8-911">Unterstützung für das Anfügen/Trennen von Datenträgern für eine einzelne VMSS-Instanz hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-911">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="4b7f8-912">13. Februar 2018</span><span class="sxs-lookup"><span data-stu-id="4b7f8-912">February 13, 2018</span></span>

<span data-ttu-id="4b7f8-913">Version 2.0.27</span><span class="sxs-lookup"><span data-stu-id="4b7f8-913">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="4b7f8-914">Core</span><span class="sxs-lookup"><span data-stu-id="4b7f8-914">Core</span></span>

* <span data-ttu-id="4b7f8-915">Authentifizierung für Abonnement-ID und Namen bei der MSI-Anmeldung in Authentifizierung mit Schlüssel geändert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-915">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="4b7f8-916">ACS</span><span class="sxs-lookup"><span data-stu-id="4b7f8-916">ACS</span></span>

* <span data-ttu-id="4b7f8-917">[WICHTIGE ÄNDERUNG] `aks get-versions` aus Gründen der Genauigkeit in `aks get-upgrades` umbenannt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-917">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="4b7f8-918">`aks get-versions` zur Anzeige der verfügbaren Kubernetes-Versionen für `aks create` geändert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-918">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="4b7f8-919">Standardwerte von `aks create` in Auswahl der Kubernetes-Version durch den Server geändert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-919">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="4b7f8-920">Hilfemeldungen zu dem von AKS generierten Dienstprinzipal aktualisiert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-920">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="4b7f8-921">Standardknotengrößen für `aks create` von „Standard\_D1\_v2“ in „Standard\_DS1\_v2“ geändert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-921">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="4b7f8-922">Zuverlässigkeit der Suche nach dem Dashboardpod für `az aks browse` verbessert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-922">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="4b7f8-923">`aks get-credentials` korrigiert, um Unicode-Fehler beim Laden von Kubernetes-Konfigurationsdateien zu behandeln</span><span class="sxs-lookup"><span data-stu-id="4b7f8-923">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="4b7f8-924">Meldung zu `az aks install-cli` hinzugefügt, um das Abrufen von `kubectl` in `$PATH` zu erleichtern</span><span class="sxs-lookup"><span data-stu-id="4b7f8-924">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="4b7f8-925">AppService</span><span class="sxs-lookup"><span data-stu-id="4b7f8-925">Appservice</span></span>

* <span data-ttu-id="4b7f8-926">Problem behoben, das zu einem Fehler von `webapp [backup|restore]` aufgrund eines Nullverweises führte</span><span class="sxs-lookup"><span data-stu-id="4b7f8-926">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="4b7f8-927">Unterstützung für Standard-App Service-Pläne durch `az configure --defaults appserviceplan=my-asp` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-927">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="4b7f8-928">CDN</span><span class="sxs-lookup"><span data-stu-id="4b7f8-928">CDN</span></span>

* <span data-ttu-id="4b7f8-929">Befehle vom Typ `cdn custom-domain [enable-https|disable-https]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-929">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="4b7f8-930">Container</span><span class="sxs-lookup"><span data-stu-id="4b7f8-930">Container</span></span>

* <span data-ttu-id="4b7f8-931">Option `--follow` zu `az container logs` für Streamingprotokolle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-931">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="4b7f8-932">Befehl `container attach` hinzugefügt, der die lokale Standardausgabe und Fehlerdatenströme an einen Container in einer Containergruppe angefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-932">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="4b7f8-933">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="4b7f8-933">CosmosDB</span></span>

* <span data-ttu-id="4b7f8-934">Unterstützung für Einstellungsfunktionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-934">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="4b7f8-935">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="4b7f8-935">Extension</span></span>

* <span data-ttu-id="4b7f8-936">Unterstützung für den Parameter `--pip-proxy` zu Befehlen vom Typ `az extension [add|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-936">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="4b7f8-937">Unterstützung für das Argument `--pip-extra-index-urls` zu Befehlen vom Typ `az extension [add|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-937">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="4b7f8-938">Feedback</span><span class="sxs-lookup"><span data-stu-id="4b7f8-938">Feedback</span></span>

* <span data-ttu-id="4b7f8-939">Erweiterungsinformationen zu Telemetriedaten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-939">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="4b7f8-940">Interactive</span><span class="sxs-lookup"><span data-stu-id="4b7f8-940">Interactive</span></span>

* <span data-ttu-id="4b7f8-941">Problem behoben, aufgrund dessen der Benutzer bei Verwendung des interaktiven Modus in Cloud Shell zur Anmeldung aufgefordert wird</span><span class="sxs-lookup"><span data-stu-id="4b7f8-941">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="4b7f8-942">Regression mit fehlenden Parametervervollständigungen korrigiert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-942">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="4b7f8-943">IoT</span><span class="sxs-lookup"><span data-stu-id="4b7f8-943">IoT</span></span>

* <span data-ttu-id="4b7f8-944">Problem behoben, aufgrund dessen `iot dps access policy [create|update]` bei erfolgreicher Ausführung einen Fehler „nicht gefunden“ zurückgibt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-944">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="4b7f8-945">Problem behoben, aufgrund dessen `iot dps linked-hub [create|update]` bei erfolgreicher Ausführung einen Fehler „nicht gefunden“ zurückgibt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-945">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="4b7f8-946">Unterstützung für `--no-wait` zu `iot dps access policy [create|update]` und `iot dps linked-hub [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-946">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="4b7f8-947">`iot hub create` geändert, um die Angabe der Anzahl von Partitionen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="4b7f8-947">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="4b7f8-948">Überwachen</span><span class="sxs-lookup"><span data-stu-id="4b7f8-948">Monitor</span></span>

* <span data-ttu-id="4b7f8-949">Befehl `az monitor log-profiles create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-949">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="4b7f8-950">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="4b7f8-950">Network</span></span>

* <span data-ttu-id="4b7f8-951">Option `--tags` für folgende Befehle korrigiert:</span><span class="sxs-lookup"><span data-stu-id="4b7f8-951">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="4b7f8-952">Profil</span><span class="sxs-lookup"><span data-stu-id="4b7f8-952">Profile</span></span>

* <span data-ttu-id="4b7f8-953">`az login` im interaktiven Modus aktiviert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-953">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="4b7f8-954">Ressource</span><span class="sxs-lookup"><span data-stu-id="4b7f8-954">Resource</span></span>

* <span data-ttu-id="4b7f8-955">`feature show` wieder hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-955">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="4b7f8-956">Rolle</span><span class="sxs-lookup"><span data-stu-id="4b7f8-956">Role</span></span>

* <span data-ttu-id="4b7f8-957">Argument `--available-to-other-tenants` zu `ad app update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-957">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="4b7f8-958">SQL</span><span class="sxs-lookup"><span data-stu-id="4b7f8-958">SQL</span></span>

* <span data-ttu-id="4b7f8-959">Befehle vom Typ `sql server dns-alias` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-959">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="4b7f8-960">`sql db rename` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-960">Added `sql db rename`</span></span>
* <span data-ttu-id="4b7f8-961">Unterstützung für das Argument `--ids` für alle SQL-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-961">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="4b7f8-962">Speicher</span><span class="sxs-lookup"><span data-stu-id="4b7f8-962">Storage</span></span>

* <span data-ttu-id="4b7f8-963">Befehle `storage blob service-properties delete-policy` und `storage blob undelete` hinzugefügt, um vorläufiges Löschen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="4b7f8-963">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="4b7f8-964">VM</span><span class="sxs-lookup"><span data-stu-id="4b7f8-964">VM</span></span>

* <span data-ttu-id="4b7f8-965">Absturz bei unvollständiger Initialisierung der VM-Verschlüsselung behoben</span><span class="sxs-lookup"><span data-stu-id="4b7f8-965">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="4b7f8-966">Prinzipal-ID-Ausgabe beim Aktivieren von MSI hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-966">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="4b7f8-967">`vm boot-diagnostics get-boot-log` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="4b7f8-967">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="4b7f8-968">31. Januar 2018</span><span class="sxs-lookup"><span data-stu-id="4b7f8-968">January 31, 2018</span></span>

<span data-ttu-id="4b7f8-969">Version 2.0.26</span><span class="sxs-lookup"><span data-stu-id="4b7f8-969">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="4b7f8-970">Core</span><span class="sxs-lookup"><span data-stu-id="4b7f8-970">Core</span></span>

* <span data-ttu-id="4b7f8-971">Unterstützung für das Abrufen von unformatierten Token im MSI-Kontext hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-971">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="4b7f8-972">Abrufindikator-Zeichenfolge nach Fertigstellung von LRO für die Windows-Datei „cmd.exe“ entfernt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-972">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="4b7f8-973">Warnung hinzugefügt, die angezeigt wird, wenn ein konfigurierter Standardwert in einen Eintrag auf INFO-Ebene geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-973">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="4b7f8-974">`--verbose` zum Anzeigen verwenden.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-974">Use `--verbose` to see</span></span>
* <span data-ttu-id="4b7f8-975">Statusanzeige für Wait-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-975">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="4b7f8-976">ACS</span><span class="sxs-lookup"><span data-stu-id="4b7f8-976">ACS</span></span>

* <span data-ttu-id="4b7f8-977">Argument `--disable-browser` erläutert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-977">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="4b7f8-978">Vervollständigung mit der TAB-TASTE für Argumente vom Typ `--vm-size` verbessert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-978">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="4b7f8-979">AppService</span><span class="sxs-lookup"><span data-stu-id="4b7f8-979">Appservice</span></span>

* <span data-ttu-id="4b7f8-980">`webapp log [tail|download]` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="4b7f8-980">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="4b7f8-981">Überprüfung `kind` für Web-Apps und Funktionen entfernt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-981">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="4b7f8-982">CDN</span><span class="sxs-lookup"><span data-stu-id="4b7f8-982">CDN</span></span>

* <span data-ttu-id="4b7f8-983">Problem mit fehlendem Client für `cdn custom-domain create` behoben</span><span class="sxs-lookup"><span data-stu-id="4b7f8-983">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="4b7f8-984">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="4b7f8-984">CosmosDB</span></span>

* <span data-ttu-id="4b7f8-985">Parameterbeschreibung für Failoverrichtlinien korrigiert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-985">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="4b7f8-986">Interactive</span><span class="sxs-lookup"><span data-stu-id="4b7f8-986">Interactive</span></span>

* <span data-ttu-id="4b7f8-987">Problem behoben, aufgrund dessen Vervollständigungen von Befehlsoptionen nicht mehr angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="4b7f8-987">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="4b7f8-988">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="4b7f8-988">Network</span></span>

* <span data-ttu-id="4b7f8-989">Schutz für `--cert-password` zu `application-gateway create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-989">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="4b7f8-990">Problem mit `application-gateway update` behoben, aufgrund dessen `--sku` fälschlicherweise einen Standardwert anwendete</span><span class="sxs-lookup"><span data-stu-id="4b7f8-990">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="4b7f8-991">Schutz für `--shared-key` und `--authorization-key` zu `vpn-connection create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-991">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="4b7f8-992">Problem mit fehlendem Client für `asg create` behoben</span><span class="sxs-lookup"><span data-stu-id="4b7f8-992">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="4b7f8-993">Parameter `--file-name / -f` für exportierte Namen zu `dns zone export` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-993">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="4b7f8-994">Folgende Probleme mit `dns zone export` behoben:</span><span class="sxs-lookup"><span data-stu-id="4b7f8-994">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="4b7f8-995">Problem behoben, aufgrund dessen lange TXT-Einträge nicht korrekt exportiert wurden</span><span class="sxs-lookup"><span data-stu-id="4b7f8-995">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="4b7f8-996">Problem behoben, aufgrund dessen TXT-Einträge in Anführungszeichen fälschlich ohne Anführungszeichen in Escapezeichen exportiert wurden</span><span class="sxs-lookup"><span data-stu-id="4b7f8-996">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="4b7f8-997">Problem behoben, aufgrund dessen bestimmte Datensätze zweimal mit `dns zone import` importiert wurden</span><span class="sxs-lookup"><span data-stu-id="4b7f8-997">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="4b7f8-998">Befehle `vnet-gateway root-cert` und `vnet-gateway revoked-cert` wiederhergestellt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-998">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="4b7f8-999">Profil</span><span class="sxs-lookup"><span data-stu-id="4b7f8-999">Profile</span></span>

* <span data-ttu-id="4b7f8-1000">`get-access-token` zur Verwendung auf einer VM mit Identität korrigiert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1000">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="4b7f8-1001">Ressource</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1001">Resource</span></span>

* <span data-ttu-id="4b7f8-1002">Fehler mit `deployment [create|validate]` korrigiert, aufgrund dessen fälschlich eine Warnung angezeigt wurde, wenn ein Vorlagenfeld „Typ“ Werte in Großbuchstaben enthielt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1002">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="4b7f8-1003">Speicher</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1003">Storage</span></span>

* <span data-ttu-id="4b7f8-1004">Problem mit der Migration von Storage V1-Konten zu Storage V2 behoben</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1004">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="4b7f8-1005">Statusberichterstellung für alle Upload-/Downloadbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1005">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="4b7f8-1006">Fehler korrigiert, der die Verwendung der arg-Option „-n“ mit `storage account check-name` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1006">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="4b7f8-1007">Spalte „Momentaufnahme“ zur Tabellenausgabe für `blob [list|show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1007">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="4b7f8-1008">Fehler mit verschiedenen Parametern korrigiert, die als Int-Typen analysiert werden mussten</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1008">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="4b7f8-1009">VM</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1009">VM</span></span>

* <span data-ttu-id="4b7f8-1010">Befehl `vm image accept-terms` hinzugefügt, um die Erstellung von VMs aus Images mit zusätzlichen Gebühren zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1010">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="4b7f8-1011">`[vm|vmss create]` korrigiert, um sicherzustellen, dass Befehle unter einem Proxy mit nicht signierten Zertifikaten ausgeführt werden können</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1011">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="4b7f8-1012">[VORSCHAU] Unterstützung für „niedrige“ Priorität zu VMSS hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1012">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="4b7f8-1013">Schutz für `--admin-password` zu `[vm|vmss] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1013">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="4b7f8-1014">17. Januar 2018</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1014">January 17, 2018</span></span>

<span data-ttu-id="4b7f8-1015">Version 2.0.25</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1015">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="4b7f8-1016">ACR</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1016">ACR</span></span>

* <span data-ttu-id="4b7f8-1017">Fallback auf ACR-Anmeldung bei Fehlern mit Windows-Anmeldeinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1017">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="4b7f8-1018">Registrierungsprotokolle aktiviert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1018">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="4b7f8-1019">ACS</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1019">ACS</span></span>

* <span data-ttu-id="4b7f8-1020">Befehl `get-credentials` korrigiert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1020">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="4b7f8-1021">SPN-Rollenanforderung entfernt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1021">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="4b7f8-1022">AppService</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1022">Appservice</span></span>

* <span data-ttu-id="4b7f8-1023">Fehler mit `config ssl upload` behoben, bei dem `hosting_environment_profile` NULL war</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1023">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="4b7f8-1024">Unterstützung benutzerdefinierter URLs zu `browse` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1024">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="4b7f8-1025">Slotunterstützung für `log tail` korrigiert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1025">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="4b7f8-1026">Backup</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1026">Backup</span></span>

* <span data-ttu-id="4b7f8-1027">Option `--container-name` von `backup item list` geändert (ist jetzt optional)</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1027">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="4b7f8-1028">Speicherkontooptionen zu `backup restore restore-disks` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1028">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="4b7f8-1029">Standortüberprüfung in `backup protection enable-for-vm` korrigiert (Groß-/Kleinschreibung wird jetzt nicht mehr beachtet)</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1029">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="4b7f8-1030">Problem behoben, durch das bei Befehlen mit ungültigem Containernamen ein Fehler auftrat</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1030">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="4b7f8-1031">`backup item list` geändert (Integritätsstatus jetzt standardmäßig enthalten)</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1031">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="4b7f8-1032">Batch</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1032">Batch</span></span>

* <span data-ttu-id="4b7f8-1033">`batch login` geändert, um Authentifizierungsdetails zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1033">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="4b7f8-1034">Cloud</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1034">Cloud</span></span>

* <span data-ttu-id="4b7f8-1035">Beim Festlegen von `--profile` für eine Cloud werden nun keine Endpunkte mehr benötigt.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1035">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="4b7f8-1036">Nutzung</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1036">Consumption</span></span>

* <span data-ttu-id="4b7f8-1037">Neue Befehle für Reservierungen hinzugefügt: `consumption reservations summaries` und `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1037">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="4b7f8-1038">Event Grid</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1038">Event Grid</span></span>

* <span data-ttu-id="4b7f8-1039">[WICHTIGE ÄNDERUNG] Die Befehle vom Typ `az eventgrid topic event-subscription` wurden in `eventgrid event-subscription` verschoben.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1039">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="4b7f8-1040">[WICHTIGE ÄNDERUNG] Die Befehle vom Typ `az eventgrid resource event-subscription` wurden in `eventgrid event-subscription` verschoben.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1040">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="4b7f8-1041">[WICHTIGE ÄNDERUNG] Der Befehl `eventgrid event-subscription show-endpoint-url` wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1041">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="4b7f8-1042">Verwenden Sie stattdessen `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1042">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="4b7f8-1043">Befehl `eventgrid topic update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1043">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="4b7f8-1044">Befehl `eventgrid event-subscription update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1044">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="4b7f8-1045">Parameter `--ids` für Befehle vom Typ `eventgrid topic` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1045">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="4b7f8-1046">Unterstützung der Vervollständigung mit der TAB-TASTE für Themennamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1046">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="4b7f8-1047">Interactive</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1047">Interactive</span></span>

* <span data-ttu-id="4b7f8-1048">Problem behoben, das dazu führte, dass der interaktive Modus nicht mit Python 2.x verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1048">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="4b7f8-1049">Fehler beim Start behoben</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1049">Fixed errors on startup</span></span>
* <span data-ttu-id="4b7f8-1050">Problem behoben, das dazu führte, dass einige Befehle nicht im interaktiven Modus ausgeführt werden konnten</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1050">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="4b7f8-1051">IoT</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1051">IoT</span></span>

* <span data-ttu-id="4b7f8-1052">Unterstützung für Gerätebereitstellungsdienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1052">Added support for device provisioning service</span></span>
* <span data-ttu-id="4b7f8-1053">Benachrichtigungen zu veralteten Elementen in Befehlen und in der Befehlshilfe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1053">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="4b7f8-1054">IoT-Überprüfung hinzugefügt, um Benutzer über die IoT-Erweiterung zu informieren</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1054">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="4b7f8-1055">Überwachen</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1055">Monitor</span></span>

* <span data-ttu-id="4b7f8-1056">Unterstützung mehrerer Diagnoseeinstellung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1056">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="4b7f8-1057">Der Parameter `--name` ist nun für `az monitor diagnostic-settings create` erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1057">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="4b7f8-1058">Befehl `monitor diagnostic-settings categories` zum Abrufen der Diagnoseeinstellungskategorie hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1058">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="4b7f8-1059">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1059">Network</span></span>

* <span data-ttu-id="4b7f8-1060">Problem behoben, das beim Ändern des aktiven Standbymodus mit `vnet-gateway update` auftrat</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1060">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="4b7f8-1061">Unterstützung für HTTP2 zu `application-gateway [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1061">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="4b7f8-1062">Profil</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1062">Profile</span></span>

* <span data-ttu-id="4b7f8-1063">Unterstützung für die Anmeldung mit durch Benutzer zugewiesenen Identitäten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1063">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="4b7f8-1064">Rolle</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1064">Role</span></span>

* <span data-ttu-id="4b7f8-1065">Argument `--assignee-object-id` zu `role assignment create` hinzugefügt, um Graph-Abfrage zu umgehen</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1065">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="4b7f8-1066">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1066">Service Fabric</span></span>

* <span data-ttu-id="4b7f8-1067">Ausführliche Fehler zur Überprüfungsantwort bei der Clustererstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1067">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="4b7f8-1068">Problem mit fehlendem Client für verschiedene Befehle behoben</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1068">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="4b7f8-1069">VM</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1069">VM</span></span>

* <span data-ttu-id="4b7f8-1070">[VORSCHAUVERSION] Zonenübergreifende Unterstützung für `vmss`</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1070">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="4b7f8-1071">[WICHTIGE ÄNDERUNG] Standard für Einzelzone (`vmss`) in Standardlastenausgleich geändert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1071">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="4b7f8-1072">[WICHTIGE ÄNDERUNG] `externalIdentities` in `userAssignedIdentities` geändert für EMSI</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1072">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="4b7f8-1073">[VORSCHAUVERSION] Unterstützung für Austausch des Betriebssystemdatenträgers hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1073">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="4b7f8-1074">Unterstützung der Verwendung von VM-Images aus anderen Abonnements hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1074">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="4b7f8-1075">Argumente `--plan-name`, `--plan-product`, `--plan-promotion-code` und `--plan-publisher` zu `[vm|vmss] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1075">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="4b7f8-1076">Fehlerbedingte Probleme mit `[vm|vmss] create` behoben</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1076">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="4b7f8-1077">Übermäßige Ressourcenverwendung durch `vm image list --all` behoben</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1077">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="4b7f8-1078">19. Dezember 2017</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1078">December 19, 2017</span></span>

<span data-ttu-id="4b7f8-1079">Version 2.0.23</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1079">Version 2.0.23</span></span>

* <span data-ttu-id="4b7f8-1080">Unterstützung für die Anmeldung mit durch Benutzer zugewiesenen Identitäten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1080">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="4b7f8-1081">Container</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1081">Container</span></span>

* <span data-ttu-id="4b7f8-1082">Falsche Reihenfolge der Parameter für Containerprotokolle behoben</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1082">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="4b7f8-1083">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1083">Network</span></span>

* <span data-ttu-id="4b7f8-1084">Argument `--disable-bgp-route-propagation` zu `route-table [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1084">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="4b7f8-1085">Argument `--ip-tags` zu `public-ip [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1085">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="4b7f8-1086">Speicher</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1086">Storage</span></span>

* <span data-ttu-id="4b7f8-1087">Unterstützung für Storage V2 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1087">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="4b7f8-1088">VM</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1088">VM</span></span>

* <span data-ttu-id="4b7f8-1089">[VORSCHAUVERSION] Unterstützung für durch Benutzer zugewiesene Identitäten für virtuelle Computer und VMSSs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1089">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="4b7f8-1090">5. Dezember 2017</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1090">December 5, 2017</span></span>

<span data-ttu-id="4b7f8-1091">Version 2.0.22</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1091">Version 2.0.22</span></span>

* <span data-ttu-id="4b7f8-1092">`az component`-Befehle wurden entfernt.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1092">Removed `az component` commands.</span></span> <span data-ttu-id="4b7f8-1093">Verwenden Sie stattdessen `az extension`.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1093">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="4b7f8-1094">Core</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1094">Core</span></span>
* <span data-ttu-id="4b7f8-1095">Der `AZURE_US_GOV_CLOUD`-Autoritätsendpunkt von AAD wurde von „login.microsoftonline.com“ in „login.microsoftonline.us“ geändert.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1095">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="4b7f8-1096">Problem behoben, aufgrund dessen Telemetriedaten fortlaufend neu gesendet wurden</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1096">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="4b7f8-1097">ACS</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1097">ACS</span></span>

* <span data-ttu-id="4b7f8-1098">Die Befehle `aks install-connector` und `aks remove-connector` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1098">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="4b7f8-1099">Verbesserte Fehlerberichterstellung für `acs create`</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1099">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="4b7f8-1100">Feste Verwendung von `aks get-credentials -f` ohne vollqualifizierten Pfad</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1100">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="4b7f8-1101">Advisor</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1101">Advisor</span></span>

* <span data-ttu-id="4b7f8-1102">Erste Version</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1102">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="4b7f8-1103">AppService</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1103">Appservice</span></span>

* <span data-ttu-id="4b7f8-1104">Erstellung feststehender Zertifikatnamen mit `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1104">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="4b7f8-1105">`webapp [list|show]` und `functionapp [list|show]` wurden verbessert, um die richtigen Apps anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1105">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="4b7f8-1106">Standardwert für `WEBSITE_NODE_DEFAULT_VERSION` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1106">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="4b7f8-1107">Nutzung</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1107">Consumption</span></span>

* <span data-ttu-id="4b7f8-1108">Unterstützung für API-Version 2017-11-30 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1108">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="4b7f8-1109">Container</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1109">Container</span></span>

* <span data-ttu-id="4b7f8-1110">Feste Regression für Standardports</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1110">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="4b7f8-1111">Überwachen</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1111">Monitor</span></span>

* <span data-ttu-id="4b7f8-1112">Unterstützung mehrerer Dimensionen zu Metrikbefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1112">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="4b7f8-1113">Ressource</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1113">Resource</span></span>

* <span data-ttu-id="4b7f8-1114">Argument `--include-response-body` zu `resource show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1114">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="4b7f8-1115">Rolle</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1115">Role</span></span>

* <span data-ttu-id="4b7f8-1116">Anzeige von Standardzuweisungen für „klassische“ Administratoren zu `role assignment list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1116">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="4b7f8-1117">Unterstützung für das Hinzufügen (anstelle der Überschreibung) von Anmeldeinformationen zu `ad sp reset-credentials` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1117">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="4b7f8-1118">Verbesserte Fehlerberichterstellung für `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1118">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="4b7f8-1119">SQL</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1119">SQL</span></span>

* <span data-ttu-id="4b7f8-1120">Die Befehle `sql db list-usages` und `sql db show-usage` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1120">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="4b7f8-1121">Die Befehle `sql server conn-policy show` und `sql server conn-policy update` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1121">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="4b7f8-1122">VM</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1122">VM</span></span>

* <span data-ttu-id="4b7f8-1123">Zoneninformationen zu `az vm list-skus` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1123">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="4b7f8-1124">14. November 2017</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1124">November 14, 2017</span></span>

<span data-ttu-id="4b7f8-1125">Version 2.0.21</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1125">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="4b7f8-1126">ACR</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1126">ACR</span></span>

* <span data-ttu-id="4b7f8-1127">Unterstützung für das Erstellen von Webhooks in Replikationsregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1127">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="4b7f8-1128">ACS</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1128">ACS</span></span>

* <span data-ttu-id="4b7f8-1129">Formulierung in AKS von „Agent“ in „Knoten“ geändert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1129">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="4b7f8-1130">Option `--orchestrator-release` für `acs create` als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1130">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="4b7f8-1131">VM-Standardgröße für AKS in `Standard_D1_v2` geändert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1131">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="4b7f8-1132">`az aks browse` für Windows korrigiert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1132">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="4b7f8-1133">`az aks get-credentials` für Windows korrigiert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1133">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="4b7f8-1134">AppService</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1134">Appservice</span></span>

* <span data-ttu-id="4b7f8-1135">Bereitstellungsquelle `config-zip` für Web-Apps und Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1135">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="4b7f8-1136">Option `--docker-container-logging` zu `az webapp log config` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1136">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="4b7f8-1137">Option `storage` aus dem Parameter `--web-server-logging` von `az webapp log config` entfernt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1137">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="4b7f8-1138">Fehlermeldungen für `deployment user set` verbessert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1138">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="4b7f8-1139">Unterstützung für das Erstellen von Linux-Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1139">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="4b7f8-1140">`list-locations` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1140">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="4b7f8-1141">Batch</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1141">Batch</span></span>

* <span data-ttu-id="4b7f8-1142">Fehler im Poolerstellungsbefehl korrigiert, der bei Verwendung einer Ressourcen-ID mit dem Flag `--image` aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1142">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="4b7f8-1143">BatchAI</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1143">Batchai</span></span>

* <span data-ttu-id="4b7f8-1144">Kurzoption (`-s`) für `--vm-size` zur Angabe der VM-Größe im Befehl `file-server create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1144">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="4b7f8-1145">Argumente für Speicherkontoname und -schlüssel zum Parameter `cluster create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1145">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="4b7f8-1146">Dokumentation für `job list-files` und `job stream-file` korrigiert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1146">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="4b7f8-1147">Kurzoption (`-r`) für `--cluster-name` zur Angabe des Clusternamens im Befehl `job create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1147">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="4b7f8-1148">Cloud</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1148">Cloud</span></span>

* <span data-ttu-id="4b7f8-1149">`cloud [register|update]` geändert, um die Registrierung von Clouds ohne erforderliche Endpunkte zu verhindern</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1149">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="4b7f8-1150">Container</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1150">Container</span></span>

* <span data-ttu-id="4b7f8-1151">Unterstützung für das Öffnen mehrerer Ports hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1151">Added support to open multiple ports</span></span>
* <span data-ttu-id="4b7f8-1152">Neustartrichtlinie für Containergruppen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1152">Added container group restart policy</span></span>
* <span data-ttu-id="4b7f8-1153">Unterstützung zum Einbinden einer Azure-Dateifreigabe als Volume hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1153">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="4b7f8-1154">Hilfedokumente aktualisiert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1154">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="4b7f8-1155">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1155">Data Lake Analytics</span></span>

* <span data-ttu-id="4b7f8-1156">`[job|account] list` geändert, um präzisere Informationen zu erhalten</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1156">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="4b7f8-1157">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1157">Data Lake Store</span></span>

* <span data-ttu-id="4b7f8-1158">`account list` geändert, um präzisere Informationen zu erhalten</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1158">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="4b7f8-1159">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1159">Extension</span></span>

* <span data-ttu-id="4b7f8-1160">`extension list-available` hinzugefügt, um das Auflisten offizieller Microsoft-Erweiterungen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1160">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="4b7f8-1161">`--name` zu `extension [add|update]` hinzugefügt, um das Installieren von Erweiterungen nach Name zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1161">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="4b7f8-1162">IoT</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1162">IoT</span></span>

* <span data-ttu-id="4b7f8-1163">Unterstützung für Zertifizierungsstellen (CAs) und Zertifikatketten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1163">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="4b7f8-1164">Überwachen</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1164">Monitor</span></span>

* <span data-ttu-id="4b7f8-1165">Befehle vom Typ `activity-log alert` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1165">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="4b7f8-1166">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1166">Network</span></span>

* <span data-ttu-id="4b7f8-1167">Unterstützung für CAA-DNS-Einträge hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1167">Added support for CAA DNS records</span></span>
* <span data-ttu-id="4b7f8-1168">Problem behoben, durch das Endpunkte nicht mit `traffic-manager profile update` aktualisiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1168">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="4b7f8-1169">Problem behoben, durch das `vnet update --dns-servers` je nach VNet-Erstellungsmethode nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1169">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="4b7f8-1170">Problem behoben, durch das relative DNS-Namen durch `dns zone import` nicht korrekt importiert wurden</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1170">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="4b7f8-1171">Reservations</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1171">Reservations</span></span>

* <span data-ttu-id="4b7f8-1172">Erste Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1172">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="4b7f8-1173">Ressource</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1173">Resource</span></span>

* <span data-ttu-id="4b7f8-1174">Unterstützung für Ressourcen-IDs zum Parameter `--resource` und Sperren auf Ressourcenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1174">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="4b7f8-1175">SQL</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1175">SQL</span></span>

* <span data-ttu-id="4b7f8-1176">Parameter `--ignore-missing-vnet-service-endpoint` zu `sql server vnet-rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1176">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="4b7f8-1177">Speicher</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1177">Storage</span></span>

* <span data-ttu-id="4b7f8-1178">`storage account create` geändert, sodass die SKU `Standard_RAGRS` als Standard verwendet wird</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1178">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="4b7f8-1179">Fehler im Zusammenhang mit Datei-/Blobnamen korrigiert, die ASCII-fremde Zeichen enthalten</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1179">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="4b7f8-1180">Fehler korrigiert, der die Verwendung von `--source-uri` mit `storage [blob|file] copy start-batch` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1180">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="4b7f8-1181">Befehle zum Globalisieren und Löschen mehrerer Objekte mit `storage [blob|file] delete-batch` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1181">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="4b7f8-1182">Problem beim Aktivieren von Metriken mit `storage metrics update` behoben</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1182">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="4b7f8-1183">Problem mit Dateien über 200 GB bei Verwendung von `storage blob upload-batch` behoben</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1183">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="4b7f8-1184">Problem behoben, durch das `--bypass` und `--default-action` von `storage account [create|update]` ignoriert wurden</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1184">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="4b7f8-1185">VM</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1185">VM</span></span>

* <span data-ttu-id="4b7f8-1186">Fehler mit `vmss create` korrigiert, der die Verwendung der Größenebene `Basic` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1186">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="4b7f8-1187">`--plan`-Argumente zu `[vm|vmss] create` für benutzerdefinierte Images mit Abrechnungsinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1187">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="4b7f8-1188">Befehle hinzugefügt: `vm secret `[add|remove|list]</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1188">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="4b7f8-1189">`vm format-secret` in `vm secret format` umbenannt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1189">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="4b7f8-1190">Argument `--encrypt format` zu `vm encryption enable` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1190">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="4b7f8-1191">24. Oktober 2017</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1191">October 24, 2017</span></span>

<span data-ttu-id="4b7f8-1192">Version 2.0.20</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1192">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="4b7f8-1193">Core</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1193">Core</span></span>

* <span data-ttu-id="4b7f8-1194">Aktualisierung von `2017-03-09-profile` zur Verwendung von Version `2016-01-01` der `MGMT_STORAGE`-API</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1194">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="4b7f8-1195">ACR</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1195">ACR</span></span>

* <span data-ttu-id="4b7f8-1196">Die Ressourcenverwaltung wurde aktualisiert und verweist nun auf die API-Version `2017-10-01`.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1196">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="4b7f8-1197">SKU „Bring Your Own Storage“ wurde in „Klassisch“ geändert.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1197">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="4b7f8-1198">Die Registrierungs-SKUs wurden in „Basic“, „Standard“ und „Premium“ umbenannt.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1198">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="4b7f8-1199">ACS</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1199">ACS</span></span>

* <span data-ttu-id="4b7f8-1200">[VORSCHAUVERSION] Befehle vom Typ `az aks` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1200">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="4b7f8-1201">Problem mit `get-credentials` in Kubernetes behoben</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1201">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="4b7f8-1202">AppService</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1202">Appservice</span></span>

* <span data-ttu-id="4b7f8-1203">Problem behoben, aufgrund dessen heruntergeladene `webapp`-Protokolle unter Umständen ungültig waren</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1203">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="4b7f8-1204">Komponente</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1204">Component</span></span>

* <span data-ttu-id="4b7f8-1205">Deutlichere Meldung zur Einstellung für alle Installer und für Bestätigungsaufforderung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1205">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="4b7f8-1206">Überwachen</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1206">Monitor</span></span>

* <span data-ttu-id="4b7f8-1207">Befehle vom Typ `action-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1207">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="4b7f8-1208">Ressource</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1208">Resource</span></span>

* <span data-ttu-id="4b7f8-1209">Inkompatibilität mit der aktuellen Version der msrest-Abhängigkeit in `group export` behoben</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1209">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="4b7f8-1210">Problem mit `policy assignment create` behoben, sodass der Befehl mit integrierten Richtliniendefinitionen und Richtliniensatzdefinitionen verwendet werden kann</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1210">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="4b7f8-1211">VM</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1211">VM</span></span>

* <span data-ttu-id="4b7f8-1212">Argument `--accelerated-networking` zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1212">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="4b7f8-1213">9. Oktober 2017</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1213">October 9, 2017</span></span>

<span data-ttu-id="4b7f8-1214">Version 2.0.19</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1214">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="4b7f8-1215">Core</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1215">Core</span></span>

* <span data-ttu-id="4b7f8-1216">Verarbeitung von ADFS-Autoritäts-URLs wurde mit einem nachgestellten Schrägstrich zu Azure Stack hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1216">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="4b7f8-1217">AppService</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1217">Appservice</span></span>

* <span data-ttu-id="4b7f8-1218">Mit dem neuen Befehl `webapp update` wurde ein allgemeines Update hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1218">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="4b7f8-1219">Batch</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1219">Batch</span></span>

* <span data-ttu-id="4b7f8-1220">Aktualisierung auf Batch SDK 4.0.0</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1220">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="4b7f8-1221">Die Option `--image` von „VirtualMachineConfiguration“ wurde aktualisiert, um zusätzlich zu „publish:offer:sku:version“ ARM-Imageverweise zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1221">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="4b7f8-1222">Unterstützung für das neue CLI-Erweiterungsmodell für Batch-Erweiterungsbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1222">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="4b7f8-1223">Batch-Unterstützung aus dem Komponentenmodell entfernt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1223">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="4b7f8-1224">BatchAI</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1224">Batchai</span></span>

* <span data-ttu-id="4b7f8-1225">Erste Version des Batch AI-Moduls</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1225">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="4b7f8-1226">KeyVault</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1226">Keyvault</span></span>

* <span data-ttu-id="4b7f8-1227">Key Vault-Authentifizierungsproblem behoben, das bei Verwendung von ADFS in Azure Stack auftrat.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1227">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="4b7f8-1228">(#4448)</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1228">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="4b7f8-1229">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1229">Network</span></span>

* <span data-ttu-id="4b7f8-1230">Das Argument `--server` von `application-gateway address-pool create` ist nun optional, sodass leere Adresspools zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1230">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="4b7f8-1231">`traffic-manager` wurde aktualisiert, um aktuelle Features zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1231">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="4b7f8-1232">Ressource</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1232">Resource</span></span>

* <span data-ttu-id="4b7f8-1233">Zusätzliche Unterstützung für `--resource-group/-g`-Optionen für Ressourcengruppennamen zu `group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1233">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="4b7f8-1234">Befehle für `account lock` hinzugefügt, um die Verwendung mit Sperren auf Abonnementebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1234">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="4b7f8-1235">Befehle für `group lock` hinzugefügt, um die Verwendung mit Sperren auf Gruppenebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1235">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="4b7f8-1236">Befehle für `resource lock` hinzugefügt, um die Verwendung mit Sperren auf Ressourcenebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1236">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="4b7f8-1237">Sql</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1237">Sql</span></span>

* <span data-ttu-id="4b7f8-1238">Unterstützung für SQL Transparent Data Encryption (TDE) und TDE für Bring Your Own Key-Szenarien hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1238">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="4b7f8-1239">Der Befehl `db list-deleted` und der Parameter `db restore --deleted-time` wurden hinzugefügt, um die Ermittlung und Wiederherstellung gelöschter Datenbanken zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1239">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="4b7f8-1240">`db op list` und `db op cancel` wurden hinzugefügt, um das Auflisten und Abbrechen ausgeführter Vorgänge für eine Datenbank zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1240">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="4b7f8-1241">Speicher</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1241">Storage</span></span>

* <span data-ttu-id="4b7f8-1242">Unterstützung für Momentaufnahme von Dateifreigaben hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1242">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="4b7f8-1243">VM</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1243">Vm</span></span>

* <span data-ttu-id="4b7f8-1244">Korrektur eines Fehlers in `vm show`, bei dem die Verwendung von `-d` in Verbindung mit fehlenden privaten IP-Adressen einen Absturz verursachte</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1244">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="4b7f8-1245">[VORSCHAUVERSION] Unterstützung für paralleles Upgrade zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1245">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="4b7f8-1246">Unterstützung für das Aktualisieren der Verschlüsselungseinstellungen mit `vm encryption enable` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1246">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="4b7f8-1247">Parameter `--os-disk-size-gb` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1247">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="4b7f8-1248">Parameter `--license-type` für Windows zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1248">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="4b7f8-1249">22. September 2017</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1249">September 22, 2017</span></span>

<span data-ttu-id="4b7f8-1250">Version 2.0.18</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1250">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="4b7f8-1251">Ressource</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1251">Resource</span></span>

* <span data-ttu-id="4b7f8-1252">Unterstützung für das Anzeigen integrierter Richtliniendefinitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1252">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="4b7f8-1253">Unterstützungsmodusparameter zum Erstellen von Richtliniendefinitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1253">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="4b7f8-1254">Unterstützung für UI-Definitionen und -Vorlagen zu `managedapp definition create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1254">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="4b7f8-1255">[WICHTIGE ÄNDERUNG] Der Ressourcentyp `managedapp` wurde von `appliances` in `applications` und von `applianceDefinitions` in `applicationDefinitions` geändert.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1255">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="4b7f8-1256">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1256">Network</span></span>

* <span data-ttu-id="4b7f8-1257">Unterstützung für Verfügbarkeitszone zu Unterbefehlen `network lb` und `network public-ip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1257">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="4b7f8-1258">Unterstützung für IPv6-Microsoft-Peering zu `express-route` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1258">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="4b7f8-1259">Befehle für Anwendungssicherheitsgruppe `asg` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1259">Added `asg` application security group commands</span></span>
* <span data-ttu-id="4b7f8-1260">Argument `--application-security-groups` zu `nic [create|ip-config create|ip-config update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1260">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="4b7f8-1261">Argumente `--source-asgs` und `--destination-asgs` zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1261">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="4b7f8-1262">Argumente `--ddos-protection` und `--vm-protection` zu `vnet [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1262">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="4b7f8-1263">Befehle vom Typ `network [vnet-gateway|vpn-client|show-url]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1263">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="4b7f8-1264">Speicher</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1264">Storage</span></span>

* <span data-ttu-id="4b7f8-1265">Problem behoben, das nach der Aktualisierung des SDK unter Umständen einen Fehler der `storage account network-rule`-Befehle zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1265">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="4b7f8-1266">Eventgrid</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1266">Eventgrid</span></span>

* <span data-ttu-id="4b7f8-1267">Azure Event Grid Python SDK für die Verwendung der neueren API-Version „2017-09-15-preview“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1267">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="4b7f8-1268">SQL</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1268">SQL</span></span>

* <span data-ttu-id="4b7f8-1269">`sql server list`-Argument `--resource-group` geändert, sodass es nun optional ist.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1269">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="4b7f8-1270">Wird es nicht angegeben, werden alle SQL Server-Instanzen im Abonnement zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1270">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="4b7f8-1271">Parameter `--no-wait` zu `db [create|copy|restore|update|replica create|create|update]` und `dw [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1271">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="4b7f8-1272">KeyVault</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1272">Keyvault</span></span>

* <span data-ttu-id="4b7f8-1273">Unterstützung für die Keyvault-Befehlsausführung hinter einem Proxy hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1273">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="4b7f8-1274">VM</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1274">VM</span></span>

* <span data-ttu-id="4b7f8-1275">Unterstützung für Verfügbarkeitszone zu `[vm|vmss|disk] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1275">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="4b7f8-1276">Problem behoben, das bei Verwendung von `--app-gateway ID` mit `vmss create` einen Fehler zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1276">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="4b7f8-1277">Argument `--asgs` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1277">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="4b7f8-1278">Unterstützung für die Ausführung von Befehlen auf virtuellen Computern mit `vm run-command` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1278">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="4b7f8-1279">[VORSCHAU] Unterstützung für VMSS-Datenträgerverschlüsselung mit `vmss encryption` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1279">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="4b7f8-1280">Unterstützung für die Durchführung der Wartung auf virtuellen Computern mit `vm perform-maintenance` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1280">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="4b7f8-1281">ACS</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1281">ACS</span></span>

* <span data-ttu-id="4b7f8-1282">[VORSCHAU] Argument `--orchestrator-release` zu `acs create` für ACS-Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1282">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="4b7f8-1283">AppService</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1283">Appservice</span></span>

* <span data-ttu-id="4b7f8-1284">Neue Möglichkeit zum Aktualisieren und Anzeigen der Authentifizierungseinstellungen mit `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1284">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="4b7f8-1285">Backup</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1285">Backup</span></span>

* <span data-ttu-id="4b7f8-1286">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1286">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="4b7f8-1287">11. September 2017</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1287">September 11, 2017</span></span>

<span data-ttu-id="4b7f8-1288">Version 2.0.17</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1288">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="4b7f8-1289">Core</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1289">Core</span></span>

* <span data-ttu-id="4b7f8-1290">Festlegung einer eigenen Korrelations-ID in Telemetrie durch das Befehlsmodul aktiviert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1290">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="4b7f8-1291">Ein Problem mit der JSON-Sicherungsdatei wurde behoben, das beim Festlegen des Diagnosemodus für Telemetrie auftrat</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1291">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="4b7f8-1292">ACS</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1292">Acs</span></span>

* <span data-ttu-id="4b7f8-1293">Befehl `acs list-locations` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1293">Added `acs list-locations` command</span></span>
* <span data-ttu-id="4b7f8-1294">`ssh-key-file` wird mit dem erwarteten Standardwert versehen.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1294">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="4b7f8-1295">AppService</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1295">Appservice</span></span>

* <span data-ttu-id="4b7f8-1296">Neue Möglichkeit zum Erstellen einer Web-App in einer anderen Ressourcengruppe als der des aktiven Diensttarifs</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1296">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="4b7f8-1297">CDN</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1297">CDN</span></span>

* <span data-ttu-id="4b7f8-1298">Der Fehler bei `cdn custom-domain create`, dass „CustomDomain“ nicht wiederholbar ist, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1298">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="4b7f8-1299">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1299">Extension</span></span>

* <span data-ttu-id="4b7f8-1300">Erste Version</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1300">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="4b7f8-1301">KeyVault</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1301">Keyvault</span></span>

* <span data-ttu-id="4b7f8-1302">Problem behoben, aufgrund dessen bei den Berechtigungen für `keyvault set-policy` die Groß-/Kleinschreibung beachtet werden musste</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1302">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="4b7f8-1303">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1303">Network</span></span>

* <span data-ttu-id="4b7f8-1304">`vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1304">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="4b7f8-1305">Das Argument `--private-access-services` wurde für `vnet subnet create/update` in `--service-endpoints` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1305">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="4b7f8-1306">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1306">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="4b7f8-1307">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1307">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="4b7f8-1308">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1308">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="4b7f8-1309">Ressource</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1309">Resource</span></span>

* <span data-ttu-id="4b7f8-1310">Übergabe von Parameterdefinitionen für Ressourcenrichtlinien in `policy definition create` und `policy definition update` zulassen</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1310">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="4b7f8-1311">Übergabe von Parameterwerten für `policy assignment create` zulassen</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1311">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="4b7f8-1312">Übergabe von JSON-Code oder einer Datei für alle Parameter zulassen</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1312">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="4b7f8-1313">Inkrementierte API-Version</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1313">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="4b7f8-1314">SQL</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1314">SQL</span></span>

* <span data-ttu-id="4b7f8-1315">Befehle vom Typ `sql server vnet-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1315">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="4b7f8-1316">VM</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1316">VM</span></span>

* <span data-ttu-id="4b7f8-1317">Behoben: Zugriff nur zuweisen, wenn `--scope` angegeben wird</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1317">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="4b7f8-1318">Behoben: Gleiche Erweiterungsbenennung wie Portal verwenden</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1318">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="4b7f8-1319">`subscription` aus der Ausgabe von `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1319">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="4b7f8-1320">Behoben: Speicher-SKU vom Typ `[vm|vmss] create` wird nicht auf Datenträger mit einem Image angewendet.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1320">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="4b7f8-1321">Behoben: `vm format-secret --secrets` akzeptierte keine durch neue Zeilen getrennte IDs.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1321">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="4b7f8-1322">31. August 2017</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1322">August 31, 2017</span></span>

<span data-ttu-id="4b7f8-1323">Version 2.0.16</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1323">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="4b7f8-1324">KeyVault</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1324">Keyvault</span></span>

* <span data-ttu-id="4b7f8-1325">Fehler behoben, der beim Versuch auftrat, die Geheimniscodierung mit `secret download` automatisch aufzulösen</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1325">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="4b7f8-1326">Sf</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1326">Sf</span></span>

* <span data-ttu-id="4b7f8-1327">Alle Befehle wurden durch die Service Fabric-Befehlszeilenschnittstelle (sfctl) ersetzt.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1327">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="4b7f8-1328">Speicher</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1328">Storage</span></span>

* <span data-ttu-id="4b7f8-1329">Problem behoben, aufgrund dessen Speicherkonten nicht in Regionen erstellt werden konnten, die die NetworkACLs-Funktion nicht unterstützen</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1329">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="4b7f8-1330">Festlegen des Inhaltstyps und der Inhaltscodierung während Blob- und Dateiuploads, wenn weder Inhaltstyp noch Inhaltscodierung angegeben sind</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1330">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="4b7f8-1331">28. August 2017</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1331">August 28, 2017</span></span>

<span data-ttu-id="4b7f8-1332">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1332">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="4b7f8-1333">Befehlszeilenschnittstelle (CLI)</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1333">CLI</span></span>

* <span data-ttu-id="4b7f8-1334">Rechtlichen Hinweis zu `--version` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1334">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="4b7f8-1335">ACS</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1335">ACS</span></span>

* <span data-ttu-id="4b7f8-1336">Vorschauregionen korrigiert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1336">Corrected preview regions</span></span>
* <span data-ttu-id="4b7f8-1337">Standardmäßiges DNS-Namenspräfix (`dns_name_prefix`) ordnungsgemäß formatiert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1337">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="4b7f8-1338">ACS-Befehlsausgabe optimiert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1338">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="4b7f8-1339">AppService</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1339">Appservice</span></span>

* <span data-ttu-id="4b7f8-1340">[WICHTIGE ÄNDERUNG] Inkonsistenzen in der Ausgabe von `az webapp config appsettings [delete|set]` behoben</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1340">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="4b7f8-1341">Neuen Alias (`-i`) für `az webapp config container set --docker-custom-image-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1341">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="4b7f8-1342">`az webapp log show` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1342">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="4b7f8-1343">Neue Argumente aus `az webapp delete` verfügbar gemacht, um App Service-Plan, Metriken oder DNS-Registrierung beizubehalten</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1343">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="4b7f8-1344">Behoben: Korrekte Erkennung der Sloteinstellungen</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1344">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="4b7f8-1345">IoT</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1345">IoT</span></span>

* <span data-ttu-id="4b7f8-1346">Behoben (3934): Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1346">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="4b7f8-1347">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1347">Network</span></span>

* <span data-ttu-id="4b7f8-1348">[WICHTIGE ÄNDERUNG] `vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1348">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="4b7f8-1349">[WICHTIGE ÄNDERUNG] Option `--private-access-services` für `--service-endpoints` in `vnet subnet [create|update]` umbenannt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1349">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="4b7f8-1350">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1350">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="4b7f8-1351">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1351">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="4b7f8-1352">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1352">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="4b7f8-1353">Profil</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1353">Profile</span></span>

* <span data-ttu-id="4b7f8-1354">`--msi` und `--msi-port` für die Anmeldung mit der Identität eines virtuellen Computers verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1354">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="4b7f8-1355">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1355">Service Fabric</span></span>

* <span data-ttu-id="4b7f8-1356">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1356">Preview release</span></span>
* <span data-ttu-id="4b7f8-1357">Registrierungsbenutzer-/-kennwortregeln für Befehl vereinfacht</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1357">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="4b7f8-1358">Kennwortanforderung für Benutzer trotz Parameterübergabe behoben</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1358">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="4b7f8-1359">Unterstützung für leere Registrierungsanmeldeinformationen (`registry_cred`) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1359">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="4b7f8-1360">Speicher</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1360">Storage</span></span>

* <span data-ttu-id="4b7f8-1361">Festlegen des Blobtarifs ermöglicht</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1361">Enabled setting blob tier</span></span>
* <span data-ttu-id="4b7f8-1362">Argumente `--bypass` und `--default-action` zur Unterstützung von Diensttunneling zu `storage account [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1362">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="4b7f8-1363">Befehle zum Hinzufügen von VNet-Regeln und IP-basierten Regeln zu `storage account network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1363">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="4b7f8-1364">Dienstverschlüsselung durch vom Kunden verwalteten Schlüssel ermöglicht</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1364">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="4b7f8-1365">[WICHTIGE ÄNDERUNG] Option `--encryption` für Befehl `az storage account create and az storage account update` in `--encryption-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1365">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="4b7f8-1366">Behoben (4220): `az storage account update encryption` – Syntaxkonflikt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1366">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="4b7f8-1367">VM</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1367">VM</span></span>

* <span data-ttu-id="4b7f8-1368">Problem behoben, aufgrund dessen bei Verwendung von `--instance-id *` zusätzliche, fehlerhafte Informationen für `vmss get-instance-view` angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1368">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="4b7f8-1369">Unterstützung für `--lb-sku` zu `vmss create` hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1369">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="4b7f8-1370">Menschliche Namen aus der Administratornamen-Blacklist für `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1370">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="4b7f8-1371">Problem behoben, aufgrund dessen `[vm|vmss] create` einen Fehler ausgelöst hat, wenn aus einem Image keine Tarifinformationen extrahiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1371">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="4b7f8-1372">Absturzproblem beim Erstellen einer VMMS-Skalierungsgruppe mit einem internen Lastenausgleich behoben</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1372">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="4b7f8-1373">Problem behoben, aufgrund dessen das Argument `--no-wait` nicht mit `vm availability-set create` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1373">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="4b7f8-1374">15. August 2017</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1374">August 15, 2017</span></span>

<span data-ttu-id="4b7f8-1375">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1375">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="4b7f8-1376">ACS</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1376">ACS</span></span>

* <span data-ttu-id="4b7f8-1377">sshMaster0-Portnummer für Kubernetes korrigiert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1377">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="4b7f8-1378">AppService</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1378">Appservice</span></span>

* <span data-ttu-id="4b7f8-1379">Ausnahme beim Erstellen einer neuen Git-basierten Linux-Web-App behoben</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1379">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="4b7f8-1380">Event Grid</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1380">Event Grid</span></span>

* <span data-ttu-id="4b7f8-1381">SDK-Abhängigkeiten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1381">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="4b7f8-1382">11. August 2017</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1382">August 11, 2017</span></span>

<span data-ttu-id="4b7f8-1383">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1383">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="4b7f8-1384">ACS</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1384">ACS</span></span>

* <span data-ttu-id="4b7f8-1385">Weitere Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1385">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="4b7f8-1386">Batch</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1386">Batch</span></span>

* <span data-ttu-id="4b7f8-1387">Auf Batch SDK 3.1.0 und Batch Management SDK 4.1.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1387">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="4b7f8-1388">Neuen Befehl zum Anzeigen der Aufgabenanzahl eines Auftrags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1388">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="4b7f8-1389">Fehler in der SAS-URL-Verarbeitung der Ressourcendatei behoben</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1389">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="4b7f8-1390">Batch-Kontoendpunkt unterstützt nun optionales Präfix „https://“</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1390">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="4b7f8-1391">Unterstützung für das Hinzufügen von Listen mit mehr als 100 Aufgaben zu einem Auftrag</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1391">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="4b7f8-1392">Debugprotokollierung für das Laden des Erweiterungsbefehlsmoduls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1392">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="4b7f8-1393">Komponente</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1393">Component</span></span>

* <span data-ttu-id="4b7f8-1394">Warnung für veraltete Befehle vom Typ „az component“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1394">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="4b7f8-1395">Container</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1395">Container</span></span>

* <span data-ttu-id="4b7f8-1396">`create`: Problem behoben, aufgrund dessen das Gleichheitszeichen innerhalb einer Umgebungsvariablen nicht zulässig war</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1396">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="4b7f8-1397">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1397">Data Lake Store</span></span>

* <span data-ttu-id="4b7f8-1398">Fortschrittsüberwachung ermöglicht</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1398">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="4b7f8-1399">Event Grid</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1399">Event Grid</span></span>

* <span data-ttu-id="4b7f8-1400">Erste Version</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1400">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="4b7f8-1401">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1401">Network</span></span>

* <span data-ttu-id="4b7f8-1402">`lb`: Problem behoben, aufgrund dessen bestimmte Namen untergeordneter Ressourcen bei Auslassung nicht ordnungsgemäß aufgelöst wurden</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1402">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="4b7f8-1403">`application-gateway {subresource} delete`: Problem behoben, aufgrund dessen `--no-wait` nicht berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1403">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="4b7f8-1404">`application-gateway http-settings update`: Problem behoben, aufgrund dessen `--connection-draining-timeout` nicht deaktiviert werden konnte</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1404">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="4b7f8-1405">Fehler behoben: Unerwartetes Schlüsselwortargument `sa_data_size_kilobyes` bei `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1405">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="4b7f8-1406">Profil</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1406">Profile</span></span>

* <span data-ttu-id="4b7f8-1407">`account list`: `--refresh` hinzugefügt, um die neuesten Abonnements vom Server zu synchronisieren</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1407">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="4b7f8-1408">Speicher</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1408">Storage</span></span>

* <span data-ttu-id="4b7f8-1409">Aktualisieren des Speicherkontos mit vom System zugewiesener Identität ermöglicht</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1409">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="4b7f8-1410">VM</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1410">VM</span></span>

* <span data-ttu-id="4b7f8-1411">`availability-set`: Fehlerdomänenanzahl bei Konvertierung verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1411">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="4b7f8-1412">Befehl `list-skus` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1412">Exposed `list-skus` command</span></span>
* <span data-ttu-id="4b7f8-1413">Unterstützung der Identitätszuweisung ohne Erstellung von Rollenzuweisungen</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1413">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="4b7f8-1414">Anwenden von Speicher-SKU beim Anfügen von Datenträgern</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1414">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="4b7f8-1415">Standardmäßiger Betriebssystemdatenträger-Name und Speicher-SKU bei Verwendung verwalteter Datenträger entfernt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1415">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="4b7f8-1416">28. Juli 2017</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1416">July 28, 2017</span></span>

<span data-ttu-id="4b7f8-1417">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1417">Version 2.0.12</span></span>

* <span data-ttu-id="4b7f8-1418">Containerbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1418">Added container commands</span></span>
* <span data-ttu-id="4b7f8-1419">Abrechnungs- und Nutzungsmodule hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1419">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="4b7f8-1420">Core</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1420">Core</span></span>

* <span data-ttu-id="4b7f8-1421">Ausgabe von SDK-Authentifizierungsinformationen für Dienstprinzipale mit Zertifikaten</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1421">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="4b7f8-1422">Ausnahmen beim Bereitstellungsfortschritt behoben</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1422">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="4b7f8-1423">Verwendung des ARM-Endpunkts aus der aktuellen Cloud für die Erstellung des Abonnementclients</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1423">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="4b7f8-1424">Gleichzeitige Verarbeitung der Datei „clouds.config“ verbessert (3636)</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1424">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="4b7f8-1425">Aktualisierung der Clientanforderungs-ID für jede Befehlsausführung</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1425">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="4b7f8-1426">Erstellung von Abonnementclients mit richtigem SDK-Profil (3635)</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1426">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="4b7f8-1427">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1427">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="4b7f8-1428">Unterstützung für Auswahl von Tabellenausgabefeldern über jmespath Abfrage hinzugefügt (3581)</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1428">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="4b7f8-1429">Stummschaltung von Analyseargumenten und Anfügeverlauf mit Gesten verbessert (3434)</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1429">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="4b7f8-1430">Erstellung von Abonnementclients mit richtigem SDK-Profil</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1430">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="4b7f8-1431">Verschiebung aller vorhandenen Erfassungsdateien in den neuesten Ordner</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1431">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="4b7f8-1432">Idempotenz für VM-/VMSS-Erstellung behoben (3586)</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1432">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="4b7f8-1433">Bei Befehlspfaden wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1433">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="4b7f8-1434">Bei bestimmten booleschen Parametern wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1434">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="4b7f8-1435">Unterstützung der Anmeldung bei lokalem AD FS-Server wie Azure Stack</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1435">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="4b7f8-1436">Gleichzeitige Schreibvorgänge in „clouds.config“ behoben (3255)</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1436">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="4b7f8-1437">ACR</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1437">ACR</span></span>

* <span data-ttu-id="4b7f8-1438">Befehl `show-usage` für verwaltete Registrierungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1438">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="4b7f8-1439">Unterstützung der SKU-Aktualisierung für verwaltete Registrierungen</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1439">Support SKU update for managed registries</span></span>
* <span data-ttu-id="4b7f8-1440">Verwaltete Registrierungen mit verwalteter SKU hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1440">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="4b7f8-1441">Webhooks für verwaltete Registrierungen mit ACR-Webhook-Befehlsmodul hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1441">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="4b7f8-1442">AAD-Authentifizierung mit ACR-Anmeldebefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1442">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="4b7f8-1443">Löschbefehl für Docker-Repositorys, Manifeste und Tags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1443">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="4b7f8-1444">ACS</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1444">ACS</span></span>

* <span data-ttu-id="4b7f8-1445">Unterstützung der API-Version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1445">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="4b7f8-1446">AppService</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1446">Appservice</span></span>

* <span data-ttu-id="4b7f8-1447">Fehler behoben, aufgrund dessen die Auflistung der Linux-Web-App keine Werte zurückgegeben hat</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1447">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="4b7f8-1448">Unterstützung für das Abrufen von Anmeldeinformationen aus dem ACR</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1448">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="4b7f8-1449">Entfernung aller Befehle unter `appservice web`</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1449">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="4b7f8-1450">Maskierung von Docker-Registrierungskennwörtern aus der Befehlsausgabe (3656)</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1450">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="4b7f8-1451">Gewährleistung der fehlerfreien Verwendung des Standardbrowsers unter macOS (3623)</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1451">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="4b7f8-1452">Verbesserung des Nutzens von `webapp log tail` und `webapp log download` (3624)</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1452">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="4b7f8-1453">Befehl `traffic-routing` zum Konfigurieren des statischen Routings verfügbar gemacht (3566)</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1453">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="4b7f8-1454">Zuverlässigkeit beim Konfigurieren der Quellcodeverwaltung verbessert (3245)</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1454">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="4b7f8-1455">Nicht unterstütztes Argument `--node-version` aus `webapp config update` für Windows-Web-Apps entfernt.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1455">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="4b7f8-1456">Verwenden Sie stattdessen `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1456">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="4b7f8-1457">Batch</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1457">Batch</span></span>

* <span data-ttu-id="4b7f8-1458">Auf Batch SDK 3.0.0 mit Unterstützung virtueller Computer mit niedriger Priorität in Pools aktualisiert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1458">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="4b7f8-1459">`pool create`-Option `--target-dedicated` in `--target-dedicated-nodes` umbenannt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1459">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="4b7f8-1460">`pool create`-Optionen `--target-low-priority-nodes` und `--application-licenses` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1460">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="4b7f8-1461">CDN</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1461">CDN</span></span>

* <span data-ttu-id="4b7f8-1462">Besser verständliche Fehlermeldung für `cdn endpoint list`, wenn das von `--profile-name` angegebene Profil nicht vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1462">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="4b7f8-1463">Cloud</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1463">Cloud</span></span>

* <span data-ttu-id="4b7f8-1464">API-Version des Cloudmetadaten-Endpunkts in das Format JJJJ-MM-TT umgewandelt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1464">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="4b7f8-1465">Katalogendpunkt nicht erforderlich</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1465">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="4b7f8-1466">Unterstützung für die Cloudregistrierung nur mit ARM-Endpunkt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1466">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="4b7f8-1467">Option für `cloud set` bereitgestellt, um beim Auswählen der aktuellen Cloud das Profil auswählen zu können</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1467">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="4b7f8-1468">`endpoint_vm_image_alias_doc` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1468">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="4b7f8-1469">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1469">CosmosDB</span></span>

* <span data-ttu-id="4b7f8-1470">Möglichkeit zum Erstellen einer Auflistung mit benutzerdefiniertem Partitionsschlüssel behoben</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1470">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="4b7f8-1471">Unterstützung für Auflistungs-Standardgültigkeitsdauer hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1471">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="4b7f8-1472">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1472">Data Lake Analytics</span></span>

* <span data-ttu-id="4b7f8-1473">Zusätzliche Befehle für Compute-Richtlinienverwaltung unter der Überschrift `dla account compute-policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1473">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="4b7f8-1474">`dla job pipeline show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1474">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="4b7f8-1475">`dla job recurrence list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1475">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="4b7f8-1476">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1476">Data Lake Store</span></span>

* <span data-ttu-id="4b7f8-1477">Unterstützung für vom Benutzer verwaltete Schlüsseltresor-Schlüsselrotation in `dls account update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1477">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="4b7f8-1478">Zugrunde liegende SDK-Version des Data Lake Store-Dateisystems aktualisiert, um ein Leistungsproblem zu behandeln</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1478">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="4b7f8-1479">Befehl `dls enable-key-vault` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1479">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="4b7f8-1480">Dieser Befehl versucht, eine vom Benutzer angegebene Key Vault-Instanz zur Verschlüsselung der Daten in einem Data Lake Store-Konto zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1480">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="4b7f8-1481">Interaktiv</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1481">Interactive</span></span>

* <span data-ttu-id="4b7f8-1482">Startzeit durch Verwendung zwischengespeicherter Befehle verbessert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1482">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="4b7f8-1483">Testabdeckung verbessert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1483">Increased test coverage</span></span>
* <span data-ttu-id="4b7f8-1484">?-Geste erweitert, sodass sie auch in den nächsten Befehl eingefügt wird</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1484">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="4b7f8-1485">Interaktive Fehler mit dem Profil „2017-03-09-profile-preview“ behoben (3587)</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1485">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="4b7f8-1486">`--version` als Parameter für den interaktiven Modus zugelassen (3645)</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1486">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="4b7f8-1487">Beseitigung von Fehlern im interaktiven Modus beim Abschluss von Überprüfungen (3570)</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1487">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="4b7f8-1488">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1488">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="4b7f8-1489">Flag `--progress` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1489">Added `--progress` flag</span></span>
* <span data-ttu-id="4b7f8-1490">`--debug` und `--verbose` aus Abschlüssen entfernt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1490">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="4b7f8-1491">`interactive` aus Abschlüssen entfernt (3324)</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1491">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="4b7f8-1492">IoT</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1492">IoT</span></span>

* <span data-ttu-id="4b7f8-1493">Behoben: Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1493">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="4b7f8-1494">(3934)</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1494">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="4b7f8-1495">Schlüsseltresor</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1495">Key vault</span></span>

* <span data-ttu-id="4b7f8-1496">Befehle für Schlüsseltresor-Wiederherstellungsfeatures hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1496">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="4b7f8-1497">`keyvault`-Unterbefehle: `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1497">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="4b7f8-1498">`keyvault secret`-Unterbefehle: `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1498">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="4b7f8-1499">`keyvault certificate`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1499">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="4b7f8-1500">`keyvault key`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1500">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="4b7f8-1501">Dienstprinzipal-Schlüsseltresorintegration hinzugefügt (3133)</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1501">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="4b7f8-1502">Schlüsseltresor-Datenebene auf 0.3.2. aktualisiert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1502">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="4b7f8-1503">(3307)</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1503">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="4b7f8-1504">Labor</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1504">Lab</span></span>

* <span data-ttu-id="4b7f8-1505">Unterstützung für Übernahme eines beliebigen virtuellen Computers im Labor über `az lab vm claim` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1505">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="4b7f8-1506">Tabellenausgabeformatierer für `az lab vm list` und `az lab vm show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1506">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="4b7f8-1507">Überwachen</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1507">Monitor</span></span>

* <span data-ttu-id="4b7f8-1508">Korrektur für Vorlagendatei mit Befehl `monitor autoscale-settings get-parameters-template` (3349)</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1508">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="4b7f8-1509">`monitor alert-rule-incidents list` in `monitor alert list-incidents` umbenannt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1509">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="4b7f8-1510">`monitor alert-rule-incidents show` in `monitor alert show-incident` umbenannt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1510">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="4b7f8-1511">`monitor metric-defintions list` in `monitor metrics list-definitions` umbenannt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1511">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="4b7f8-1512">`monitor alert-rules` in `monitor alert` umbenannt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1512">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="4b7f8-1513">`monitor alert create` geändert:</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1513">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="4b7f8-1514">Unterbefehle vom Typ `condition` und `action` akzeptieren keinen JSON-Code mehr.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1514">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="4b7f8-1515">Hinzufügung zahlreicher Parameter zur Vereinfachung der Regelerstellung</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1515">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="4b7f8-1516">`location` nicht mehr erforderlich</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1516">`location` no longer required</span></span>
  * <span data-ttu-id="4b7f8-1517">Hinzufügung von Namen- und ID-Unterstützung für Ziel</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1517">Add name and ID support for target</span></span>
  * <span data-ttu-id="4b7f8-1518">Entfernung von `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1518">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="4b7f8-1519">Umbenennung von `is-enabled` in `enabled` (nicht mehr erforderlich)</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1519">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="4b7f8-1520">`description` wird nun abhängig von der angegebenen Bedingung auf einen Standardwert festgelegt.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1520">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="4b7f8-1521">Hinzufügung von Beispielen zur Verdeutlichung des neuen Formats</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1521">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="4b7f8-1522">Unterstützung von Namen oder IDs für Befehle vom Typ `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1522">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="4b7f8-1523">Komfortargumente und Beispiele zu `monitor alert rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1523">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="4b7f8-1524">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1524">Network</span></span>

* <span data-ttu-id="4b7f8-1525">Befehl `list-private-access-services` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1525">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="4b7f8-1526">Argument `--private-access-services` zu `vnet subnet create` und `vnet subnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1526">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="4b7f8-1527">Problem behoben, das einen Fehler für `application-gateway redirect-config create` zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1527">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="4b7f8-1528">Problem behoben, aufgrund dessen `application-gateway redirect-config update` nicht mit `--no-wait` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1528">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="4b7f8-1529">Fehler behoben, der bei der Verwendung des Arguments `--servers` mit `application-gateway address-pool create` und `application-gateway address-pool update` aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1529">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="4b7f8-1530">Befehle vom Typ `application-gateway redirect-config` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1530">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="4b7f8-1531">Befehle zu `application-gateway ssl-policy` hinzugefügt: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1531">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="4b7f8-1532">Argumente zu `application-gateway ssl-policy set` hinzugefügt: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1532">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="4b7f8-1533">Argumente zu `application-gateway http-settings create` und `application-gateway http-settings update` hinzugefügt: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1533">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="4b7f8-1534">Argumente zu `application-gateway url-path-map create` und `application-gateway url-path-map update` hinzugefügt: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1534">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="4b7f8-1535">Argument `--redirect-config` zu `application-gateway url-path-map rule create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1535">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="4b7f8-1536">Unterstützung für `--no-wait` zu `application-gateway url-path-map rule delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1536">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="4b7f8-1537">Argumente zu `application-gateway probe create` und `application-gateway probe update` hinzugefügt: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1537">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="4b7f8-1538">Argument `--redirect-config` zu `application-gateway rule create` und `application-gateway rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1538">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="4b7f8-1539">Unterstützung für `--accelerated-networking` zu `nic create` und `nic update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1539">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="4b7f8-1540">Argument `--internal-dns-name-suffix` von `nic create` entfernt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1540">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="4b7f8-1541">Unterstützung für `--dns-servers` zu `nic update` und `nic create` hinzugefügt: Unterstützung für „--dns-servers“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1541">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="4b7f8-1542">Fehler korrigiert, aufgrund dessen `--local-address-prefixes` von `local-gateway create` ignoriert wurde</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1542">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="4b7f8-1543">Unterstützung für `--dns-servers` zu `vnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1543">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="4b7f8-1544">Fehler beim Erstellen eines Peerings ohne Routenfilterung mit `express-route peering create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1544">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="4b7f8-1545">Fehler korrigiert, aufgrund dessen die Argumente `--provider` und `--bandwidth` nicht mit `express-route update` verwendet werden konnten</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1545">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="4b7f8-1546">Fehler mit Standardlogik von `network watcher show-topology` korrigiert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1546">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="4b7f8-1547">Ausgabeformatierung für `network list-usages` verbessert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1547">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="4b7f8-1548">Verwendung der standardmäßigen Front-End-IP-Adresse für `application-gateway http-listener create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1548">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="4b7f8-1549">Verwendung des Standardadresspools, der HTTP-Standardeinstellungen und des HTTP-Standardlisteners für `application-gateway rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1549">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="4b7f8-1550">Verwendung der standardmäßigen Front-End-IP-Adresse und des standardmäßigen Back-End-Pools für `lb rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1550">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="4b7f8-1551">Verwendung der standardmäßigen Front-End-IP-Adresse für `lb inbound-nat-rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1551">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="4b7f8-1552">Profil</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1552">Profile</span></span>

* <span data-ttu-id="4b7f8-1553">Unterstützung der Anmeldung innerhalb eines virtuellen Computers mit einer verwalteten Identität</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1553">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="4b7f8-1554">Unterstützung der Ausgabe für `account show` im SDK-Authentifizierungsdateiformat</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1554">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="4b7f8-1555">Anzeige von Warnungen für veraltete Befehle bei Verwendung von „--expanded-view“</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1555">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="4b7f8-1556">Befehl `get-access-token` für die Bereitstellung eines unformatierten AAD-Tokens hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1556">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="4b7f8-1557">Unterstützung der Anmeldung mit einem Benutzerkonto ohne zugeordnete Abonnements</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1557">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="4b7f8-1558">RDBMS</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1558">RDBMS</span></span>

* <span data-ttu-id="4b7f8-1559">Unterstützung der abonnementübergreifenden Auflistung von Servern (3417)</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1559">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="4b7f8-1560">Behoben: `%s` wird aufgrund von fehlendem `% server_type` nicht verarbeitet (3393)</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1560">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="4b7f8-1561">Dokumentquellenzuordnung behoben und CI-Aufgabe zur Überprüfung hinzugefügt (3361)</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1561">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="4b7f8-1562">MySQL- und PostgreSQL-Hilfe korrigiert (3369)</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1562">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="4b7f8-1563">Ressource</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1563">Resource</span></span>

* <span data-ttu-id="4b7f8-1564">Eingabeaufforderungen bei fehlenden Parametern für `group deployment create` verbessert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1564">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="4b7f8-1565">Analyse der Syntax `--parameters KEY=VALUE` verbessert</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1565">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="4b7f8-1566">Probleme behoben, durch die Parameterdateien von `group deployment create` bei Verwendung der Syntax `@<file>` nicht mehr erkannt wurden</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1566">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="4b7f8-1567">Unterstützung des Arguments `--ids` für Befehle vom Typ `resource` und `managedapp`</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1567">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="4b7f8-1568">Einige Analyse- und Fehlermeldungen korrigiert (3584)</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1568">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="4b7f8-1569">Analyse vom Typ `--resource-type` für den Befehl `lock` korrigiert, sodass `<resource-namespace>` und `<resource-type>` akzeptiert werden</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1569">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="4b7f8-1570">Parameterüberprüfung für Vorlagenlinkvorlagen hinzugefügt (3629)</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1570">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="4b7f8-1571">Unterstützung für die Angabe von Bereitstellungsparametern mit der Syntax `KEY=VALUE` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1571">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="4b7f8-1572">Rolle</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1572">Role</span></span>

* <span data-ttu-id="4b7f8-1573">Unterstützung der Ausgabe im SDK-Authentifizierungsdateiformat für `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1573">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="4b7f8-1574">Rollenzuweisungen und dazugehörige AAD-Anwendung beim Löschen eines Dienstprinzipals bereinigt (3610)</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1574">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="4b7f8-1575">Einbeziehung des Zeitformats in Beschreibungen vom Typ `--start-date` und `--end-date` für `app create`-Argumente</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1575">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="4b7f8-1576">Anzeige von Warnungen für veraltete Befehle bei Verwendung von `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1576">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="4b7f8-1577">Schlüsseltresorintegration zu den Befehlen `create-for-rbac` und `reset-credentials` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1577">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="4b7f8-1578">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1578">Service Fabric</span></span>
* <span data-ttu-id="4b7f8-1579">Problem behoben, aufgrund dessen große Dateien in Anwendungen beim Hochladen gekürzt wurden (3666)</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1579">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="4b7f8-1580">Tests für Service Fabric-Befehle hinzugefügt (3424)</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1580">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="4b7f8-1581">Zahlreiche Service Fabric-Befehle korrigiert (3234)</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1581">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="4b7f8-1582">SQL</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1582">SQL</span></span>

* <span data-ttu-id="4b7f8-1583">Fehlerhaften Parameter `--identity` für `sql server create` entfernt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1583">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="4b7f8-1584">Kennwortwerte aus der Befehlsausgabe von `sql server create` und `sql server update` entfernt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1584">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="4b7f8-1585">Befehle `sql db list-editions` und `sql elastic-pool list-editions` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1585">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="4b7f8-1586">Speicher</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1586">Storage</span></span>

* <span data-ttu-id="4b7f8-1587">Option `--marker` für die Befehle `storage blob list`, `storage container list` und `storage share list` entfernt (3745)</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1587">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="4b7f8-1588">Erstellung eines reinen HTTPS-Speicherkontos ermöglicht</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1588">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="4b7f8-1589">Speichermetriken, Protokollierung und CORS-Befehle aktualisiert (3495)</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1589">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="4b7f8-1590">Ausnahmemeldung von „cors add“ umformuliert (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1590">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="4b7f8-1591">Generator im Probelaufmodus des Downloadbatchbefehls in eine Liste konvertiert (3592)</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1591">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="4b7f8-1592">Problem bei Probelauf des Blobdownloadbatchs behoben (3640) (3592)</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1592">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="4b7f8-1593">VM</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1593">VM</span></span>

* <span data-ttu-id="4b7f8-1594">Unterstützung der NSG-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1594">Support configuring nsg</span></span>
* <span data-ttu-id="4b7f8-1595">Fehler behoben, aufgrund dessen der DNS-Server nicht ordnungsgemäß konfiguriert wurde</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1595">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="4b7f8-1596">Unterstützung verwalteter Dienstidentitäten</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1596">Support managed service identities</span></span>
* <span data-ttu-id="4b7f8-1597">Problem behoben, aufgrund dessen `cmss create` mit einem vorhandenen Lastenausgleich `--backend-pool-name` benötigte</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1597">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="4b7f8-1598">Festlegung, dass die LUN von mit `vm image create` erstellten Datenträgern mit 0 beginnt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1598">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="4b7f8-1599">10. Mai 2017</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1599">May 10, 2017</span></span>

<span data-ttu-id="4b7f8-1600">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1600">Version 2.0.6</span></span>

* <span data-ttu-id="4b7f8-1601">Umbenennen von „documentdb“ in „cosmosdb“</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1601">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="4b7f8-1602">Hinzufügen von rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1602">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="4b7f8-1603">Einbeziehen der Data Lake Analytics- und Data Lake Store-Module</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1603">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="4b7f8-1604">Einbeziehen des Cognitive Services-Moduls</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1604">Include Cognitive Services module</span></span>
* <span data-ttu-id="4b7f8-1605">Einbeziehen des Service Fabric-Moduls</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1605">Include Service Fabric module</span></span>
* <span data-ttu-id="4b7f8-1606">Einbeziehen des interaktiven Moduls (Umbenennen von „az-shell“)</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1606">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="4b7f8-1607">Hinzufügen von Unterstützung für CDN-Befehle</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1607">Add support for CDN commands</span></span>
* <span data-ttu-id="4b7f8-1608">Entfernen des Containermoduls</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1608">Remove Container module</span></span>
* <span data-ttu-id="4b7f8-1609">Hinzufügen von „az -v“ als Verknüpfung für „az --version“ ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1609">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="4b7f8-1610">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1610">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="4b7f8-1611">Core</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1611">Core</span></span>

* <span data-ttu-id="4b7f8-1612">Core: Erfassen von Ausnahmen, die durch einen nicht registrierten Anbieter verursacht werden, und automatische Registrierung</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1612">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="4b7f8-1613">Leistung: Dauerhaftes Speichern des ADAL-Tokencaches im Arbeitsspeicher bis zum Prozessende ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1613">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="4b7f8-1614">Korrigieren der vom hexadezimalen Fingerabdruck -o tsv zurückgegebenen Bytes ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1614">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="4b7f8-1615">Verbessern des Downloads des Schlüsseltresorzertifikats und der AAD-SP-Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1615">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="4b7f8-1616">Hinzufügen des Python-Speicherorts zu „az –version“ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1616">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="4b7f8-1617">Anmeldung: Unterstützung der Anmeldung, wenn keine Abonnements vorhanden sind ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1617">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="4b7f8-1618">Core: Beheben eines Fehlers bei zweimaliger Verwendung eines Dienstprinzipals bei der Anmeldung ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1618">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="4b7f8-1619">Core: Ermöglichen der Konfiguration des Dateipfads von „accessTokens.json“ über eine Umgebungsvariable ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1619">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="4b7f8-1620">Core: Zulassen der Anwendung konfigurierter Standardwerte auf optionale Argumente ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1620">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="4b7f8-1621">Core: Verbesserte Leistung</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1621">core: Improved performance</span></span>
* <span data-ttu-id="4b7f8-1622">Core: Zertifikate von benutzerdefinierter Zertifizierungsstelle – Unterstützung für das Festlegen der REQUESTS_CA_BUNDLE-Umgebungsvariablen</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1622">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="4b7f8-1623">Core: Cloudkonfiguration – Verwenden des Endpunkts „resource manager“, wenn Endpunkt „management“ nicht festgelegt ist</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1623">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="4b7f8-1624">ACS</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1624">ACS</span></span>

* <span data-ttu-id="4b7f8-1625">Korrigieren der Master- und Agentanzahl als ganze Zahl statt Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1625">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="4b7f8-1626">Verfügbarmachen von „az acs create --no-wait“ und „az acs wait“ für die asynchrone Erstellung</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1626">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="4b7f8-1627">Verfügbarmachen von „az acs create --validate“ für Probelaufüberprüfungen</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1627">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="4b7f8-1628">Entfernen von Windows-Profil vor PUT-Aufruf für Skalierungsbefehl ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1628">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="4b7f8-1629">AppService</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1629">AppService</span></span>

* <span data-ttu-id="4b7f8-1630">functionapp: Hinzufügen der vollständigen functionapp-Unterstützung, einschließlich Erstellen, Anzeigen, Auflisten, Löschen, Hostname, SSL usw.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1630">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="4b7f8-1631">Hinzufügen von Team Services (vsts) als Continuous Delivery-Option zu „appservice web source-control config“</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1631">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="4b7f8-1632">Erstellen von „az webapp“ als Ersatz für „az appservice web“ (für Abwärtskompatibilität bleibt „az appservice web“ für 2 weitere Releases erhalten)</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1632">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="4b7f8-1633">Verfügbarmachen von Argumenten zum Konfigurieren von Bereitstellung und Laufzeitstapeln beim Erstellen von Web-Apps</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1633">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="4b7f8-1634">Verfügbarmachen von „webapp list-runtimes“</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1634">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="4b7f8-1635">Unterstützen der Konfiguration von Verbindungszeichenfolgen ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1635">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="4b7f8-1636">Unterstützen des Slottauschs mit Vorschau</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1636">support slot swap with preview</span></span>
* <span data-ttu-id="4b7f8-1637">Beheben von Fehlern in appservice-Befehlen ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1637">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="4b7f8-1638">Verwenden der Ressourcengruppe des App Service-Plans für Zertifizierungsvorgänge ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1638">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="4b7f8-1639">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1639">CosmosDB</span></span>

* <span data-ttu-id="4b7f8-1640">Umbenennen des documentdb-Moduls in cosmosdb</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1640">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="4b7f8-1641">Zusätzliche Unterstützung für documentdb-APIs auf Datenebene: Datenbank- und Sammlungsverwaltung</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1641">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="4b7f8-1642">Zusätzliche Unterstützung für das Aktivieren des automatischen Failovers für Datenbankkonten</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1642">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="4b7f8-1643">Zusätzliche Unterstützung für die neue ConsistentPrefix-Konsistenzrichtlinie</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1643">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="4b7f8-1644">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1644">Data Lake Analytics</span></span>

* <span data-ttu-id="4b7f8-1645">Beheben eines Fehlers, bei dem das Filtern von Auftragslisten nach Ergebnis und Status einen Fehler auslöst</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1645">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="4b7f8-1646">Hinzufügen von Unterstützung für den neuen Katalogelementtyp „Paket“</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1646">Add support for new catalog item type: package.</span></span> <span data-ttu-id="4b7f8-1647">Zugriff über: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1647">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="4b7f8-1648">Ermöglichen der Auflistung folgender Katalogelemente innerhalb einer Datenbank (keine Schemaspezifikation erforderlich):</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1648">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="4b7f8-1649">Table</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1649">Table</span></span>
  * <span data-ttu-id="4b7f8-1650">Tabellenwertfunktion</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1650">Table valued function</span></span>
  * <span data-ttu-id="4b7f8-1651">Sicht</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1651">View</span></span>
  * <span data-ttu-id="4b7f8-1652">Tabellenstatistiken.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1652">Table Statistics.</span></span> <span data-ttu-id="4b7f8-1653">Können auch mit einem Schema, jedoch ohne Angabe eines Tabellennamens aufgelistet werden.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1653">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="4b7f8-1654">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1654">Data Lake Store</span></span>

* <span data-ttu-id="4b7f8-1655">Aktualisieren der Version des zugrunde liegenden Dateisystem-SDK, wodurch eine bessere Unterstützung für die Verarbeitung von Drosselungsszenarien auf Serverseite gewährt wird</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1655">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="4b7f8-1656">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1656">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="4b7f8-1657">Fehlende Hilfe für Zugriffsanzeige</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1657">missed help for access show.</span></span> <span data-ttu-id="4b7f8-1658">hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1658">adding it.</span></span> <span data-ttu-id="4b7f8-1659">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1659">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="4b7f8-1660">Suchen</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1660">Find</span></span>

* <span data-ttu-id="4b7f8-1661">Verbessern von Suchergebnissen und Ermöglichen der Versionsverwaltung des Suchindex</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1661">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="4b7f8-1662">KeyVault</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1662">KeyVault</span></span>

* <span data-ttu-id="4b7f8-1663">BC:`az keyvault certificate download` Ändern von „-e“ von Zeichenfolge oder Binärdatentyp in PEM oder DER zur besseren Darstellung der Optionen</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1663">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="4b7f8-1664">BC: Entfernen von „--expires“ und „--not-before“ aus `keyvault certificate create`, da diese Parameter nicht vom Dienst unterstützt werden</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1664">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="4b7f8-1665">Hinzufügen des Parameters „--validity“ zu `keyvault certificate create`, um gezielt den Wert in „--policy“ zu überschreiben</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1665">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="4b7f8-1666">Beheben des Problems in `keyvault certificate get-default-policy`, bei dem „expires“ und „not_before“ verfügbar gemacht wurden, „validity_in_months“ hingegen nicht</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1666">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="4b7f8-1667">Keyvault-Korrektur für den Import von PEM und PFX ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1667">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="4b7f8-1668">Labor</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1668">Lab</span></span>

* <span data-ttu-id="4b7f8-1669">Hinzufügen der Befehle „create“, „show“, „delete“ und „list“ für die Laborumgebung</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1669">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="4b7f8-1670">Hinzufügen der Befehle „show“ und „list“ zur Anzeige von ARM-Vorlagen im Labor</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1670">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="4b7f8-1671">Hinzufügen des Kennzeichens „--environment“ in `az lab vm list`, um virtuelle Computer nach Umgebung im Labor zu filtern</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1671">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="4b7f8-1672">Hinzufügen des benutzerfreundlichen Befehls `az lab formula export-artifacts` zum Exportieren des Artefaktgerüsts innerhalb der Formel eines Labors</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1672">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="4b7f8-1673">Hinzufügen von Befehlen zum Verwalten von Geheimnissen in einem Labor</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1673">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="4b7f8-1674">Überwachen</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1674">Monitor</span></span>

* <span data-ttu-id="4b7f8-1675">Programmfehlerbehebung: Modellieren von `--actions` von `az alert-rules create` zum Verarbeiten von JSON-Zeichenfolgen ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1675">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="4b7f8-1676">Programmfehlerbehebung: Beim Erstellen von Diagnoseeinstellungen werden Protokolle/Metriken aus Anzeigebefehlen nicht akzeptiert ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1676">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="4b7f8-1677">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1677">Network</span></span>

* <span data-ttu-id="4b7f8-1678">Hinzufügen des `network watcher test-connectivity`-Befehls</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1678">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="4b7f8-1679">Hinzufügen von Unterstützung für den `--filters`-Parameter für `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1679">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="4b7f8-1680">Hinzufügen von Unterstützung für den Application Gateway-Verbindungsausgleich</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1680">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="4b7f8-1681">Hinzufügen von Unterstützung für die Konfiguration von Application Gateway-WAF-Regelsätzen</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1681">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="4b7f8-1682">Hinzufügen von Unterstützung für ExpressRoute-Routenfilter und -Regeln</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1682">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="4b7f8-1683">Hinzufügen von Unterstützung für geografisches TrafficManager-Routing</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1683">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="4b7f8-1684">Hinzufügen von Unterstützung für richtlinienbasierte Datenverkehrsselektoren für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1684">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="4b7f8-1685">Hinzufügen von Unterstützung für IPSec-Richtlinien für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1685">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="4b7f8-1686">Korrektur eines Fehlers bei `vpn-connection create` bei Verwendung der Parameter `--no-wait` oder `--validate`</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1686">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="4b7f8-1687">Hinzufügen von Unterstützung für Aktiv/Aktiv-VNET-Gateways</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1687">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="4b7f8-1688">Entfernen von NULL-Werten aus der Ausgabe von `network vpn-connection list/show`-Befehlen</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1688">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="4b7f8-1689">BC: Korrektur eines Fehlers in der Ausgabe von `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1689">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="4b7f8-1690">Korrektur eines Fehlers, bei dem das Argument „--key-length“ von „vpn-connection create“ nicht ordnungsgemäß analysiert wurde</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1690">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="4b7f8-1691">Korrektur eines Fehlers in `dns zone import`, bei dem Datensätze nicht ordnungsgemäß importiert wurden</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1691">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="4b7f8-1692">Korrektur eines Fehlers, bei dem `traffic-manager endpoint update` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1692">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="4b7f8-1693">Hinzufügen von Network Watcher-Vorschaubefehlen</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1693">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="4b7f8-1694">Profil</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1694">Profile</span></span>

* <span data-ttu-id="4b7f8-1695">Unterstützung der Anmeldung, wenn keine Abonnements gefunden werden ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1695">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="4b7f8-1696">Unterstützung für kurze Parameternamen in „az account set --subscription“ ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1696">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="4b7f8-1697">Redis</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1697">Redis</span></span>

* <span data-ttu-id="4b7f8-1698">Hinzufügen des Updatebefehls, durch den auch die Möglichkeit zum Skalieren für Redis Cache hinzugefügt wird</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1698">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="4b7f8-1699">Verwerfen des Befehls „update-settings“</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1699">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="4b7f8-1700">Ressource</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1700">Resource</span></span>

* <span data-ttu-id="4b7f8-1701">Hinzufügen der Befehle „managedapp“ und „managedapp definition“ ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1701">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="4b7f8-1702">Unterstützung für die „provider operation“-Befehle ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1702">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="4b7f8-1703">Unterstützung für die Erstellung generischer Ressourcen ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1703">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="4b7f8-1704">Korrigieren der Ressourcenanalyse und der API-Versionssuche</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1704">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="4b7f8-1705">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1705">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="4b7f8-1706">Hinzufügen von Dokumenten für „az lock update“</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1706">Add docs for az lock update.</span></span> <span data-ttu-id="4b7f8-1707">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1707">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="4b7f8-1708">Beenden mit Fehler bei dem Versuch, Ressourcen für eine nicht vorhandene Gruppe aufzulisten</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1708">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="4b7f8-1709">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1709">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="4b7f8-1710">[Compute] Beheben von Problemen mit dem Update von VMSS- und VM-Verfügbarkeitsgruppen</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1710">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="4b7f8-1711">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1711">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="4b7f8-1712">Korrigieren des Erstellungs- und Löschvorgangs für Sperren, wenn „parent-resource-path“ auf „None“ festgelegt ist ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1712">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="4b7f8-1713">Rolle</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1713">Role</span></span>

* <span data-ttu-id="4b7f8-1714">create-for-rbac: Sicherstellen, dass das SP-Enddatum nicht das Ablaufdatum des Zertifikats überschreitet ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1714">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="4b7f8-1715">RBAC: Hinzufügen vollständiger Unterstützung für „ad group“ ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1715">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="4b7f8-1716">Rolle: Beheben von Probleme beim Rollendefinitionsupdate ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1716">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="4b7f8-1717">create-for-rbac: Sicherstellen, dass das angegebene Benutzerkennwort übernommen wird</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1717">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="4b7f8-1718">SQL</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1718">SQL</span></span>

* <span data-ttu-id="4b7f8-1719">Hinzufügen der Befehle „az sql server list-usages“ und „az sql db list-usages“</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1719">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="4b7f8-1720">SQL: Möglichkeit zur direkten Verbindung mit Ressourcenanbieter ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1720">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="4b7f8-1721">Speicher</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1721">Storage</span></span>

* <span data-ttu-id="4b7f8-1722">Festlegen des Ressourcengruppenstandorts als Standardstandort für `storage account create`</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1722">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="4b7f8-1723">Hinzufügen von Unterstützung für das inkrementelle Kopieren von Blobs</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1723">Add support for incremental blob copy</span></span>
* <span data-ttu-id="4b7f8-1724">Hinzufügen von Unterstützung für den Upload umfangreicher Blockblobs</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1724">Add support for large block blob upload</span></span>
* <span data-ttu-id="4b7f8-1725">Ändern der Blockgröße auf 100 MB, wenn die hochzuladende Datei größer als 200 GB ist</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1725">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="4b7f8-1726">VM</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1726">VM</span></span>

* <span data-ttu-id="4b7f8-1727">avail-set: Festlegen der UD- und FD-Domänenanzahl als optional</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1727">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="4b7f8-1728">Hinweis zu VM-Befehlen in unabhängigen Clouds: Vermeiden Sie Features im Zusammenhang mit verwalteten Datenträgern, einschließlich der folgenden:</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1728">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="4b7f8-1729">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1729">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="4b7f8-1730">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1730">az vm/vmss disk</span></span>
  3. <span data-ttu-id="4b7f8-1731">Verwenden Sie in „az vm/vmss create“ den Befehl „—use-unmanaged-disk“, um verwaltete Datenträger zu vermeiden. Andere Befehle sollten funktionieren.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1731">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="4b7f8-1732">vm/vmss: Verbessern des Warnungstexts beim Generieren von SSH-Schlüsselpaaren</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1732">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="4b7f8-1733">vm/vmss: Unterstützen der Erstellung über ein Marketplace-Image, für das Planinformationen erforderlich sind ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1733">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="4b7f8-1734">3. April 2017</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1734">April 3, 2017</span></span>

<span data-ttu-id="4b7f8-1735">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1735">Version 2.0.2</span></span>

<span data-ttu-id="4b7f8-1736">In dieser Version wurden die Komponenten ACR, Batch, KeyVault und SQL eingeführt.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1736">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="4b7f8-1737">Core</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1737">Core</span></span>

* <span data-ttu-id="4b7f8-1738">Hinzufügen der Module „acr“, „lab“, „monitor“ und „find“ zur Standardliste</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1738">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="4b7f8-1739">Anmeldung: Überspringen des fehlerhaften Mandanten ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1739">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="4b7f8-1740">Anmeldung: Festlegen des Standardabonnements auf ein Abonnement mit dem Status „Enabled“ ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1740">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="4b7f8-1741">Hinzufügen von wait-Befehlen und Unterstützung von „--no-wait“ für mehr Befehle ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1741">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="4b7f8-1742">Core: Unterstützen der Anmeldung per Dienstprinzipal mit einem Zertifikat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1742">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="4b7f8-1743">Hinzufügen der Meldung zu fehlenden Vorlagenparametern</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1743">Add prompting for missing template parameters.</span></span> <span data-ttu-id="4b7f8-1744">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1744">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="4b7f8-1745">Unterstützen des Festlegens von Standardwerten für häufig verwendete Argumente, z.B. Standardressourcengruppe, Standardweb und Standard-VM</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1745">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="4b7f8-1746">Unterstützen der Anmeldung an einem bestimmten Mandanten</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1746">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="4b7f8-1747">ACS</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1747">ACS</span></span>

* <span data-ttu-id="4b7f8-1748">[ACS] Hinzufügen von Unterstützung für die Konfiguration eines ACS-Standardclusters ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1748">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="4b7f8-1749">Hinzufügen von Unterstützung der Aufforderung zur Kennworteingabe für SSH-Schlüssel</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1749">Add support for ssh key password prompting.</span></span> <span data-ttu-id="4b7f8-1750">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1750">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="4b7f8-1751">Hinzufügen von Unterstützung für Windows-Cluster</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1751">Add support for windows clusters.</span></span> <span data-ttu-id="4b7f8-1752">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1752">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="4b7f8-1753">Wechseln von der Rolle „Besitzer“ zur Rolle „Mitwirkender“</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1753">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="4b7f8-1754">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1754">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="4b7f8-1755">AppService</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1755">AppService</span></span>

* <span data-ttu-id="4b7f8-1756">appservice: Unterstützung für das Abrufen der externen IP-Adresse für DNS A-Einträge ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1756">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="4b7f8-1757">appservice: Unterstützung der Bindung von Platzhalterzertifikaten ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1757">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="4b7f8-1758">appservice: Unterstützung von Veröffentlichungsprofilen für Listen ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1758">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="4b7f8-1759">AppService: Auslösen der Synchronisierung der Quellcodeverwaltung nach der Konfiguration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1759">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="4b7f8-1760">DataLake</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1760">DataLake</span></span>

* <span data-ttu-id="4b7f8-1761">Erste Version des Data Lake Analytics-Moduls</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1761">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="4b7f8-1762">Erste Version des Data Lake Store-Moduls</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1762">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="4b7f8-1763">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1763">DocuemntDB</span></span>

* <span data-ttu-id="4b7f8-1764">DocumentDB: Hinzufügen von Unterstützung für das Auflisten von Verbindungszeichenfolgen ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1764">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="4b7f8-1765">VM</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1765">VM</span></span>

* <span data-ttu-id="4b7f8-1766">[Compute] Hinzufügen von AppGateway-Unterstützung für Erstellung von VM-Skalierungsgruppen ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1766">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="4b7f8-1767">[VM/VMSS] Verbesserte Unterstützung für die Datenträgerzwischenspeicherung ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1767">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="4b7f8-1768">VM/VMSS: Einbinden der vom Portal verwendeten Logik zur Überprüfung von Anmeldeinformationen ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1768">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="4b7f8-1769">Hinzufügen von wait-Befehlen und Unterstützung für „--no-wait“ ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1769">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="4b7f8-1770">VM-Skalierungsgruppe: Unterstützung von „\*“ zum Auflisten der übergreifenden Instanzansicht für VMs ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1770">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="4b7f8-1771">Hinzufügen – geheime Schlüssel für virtuellen Computer und VM-Skalierungsgruppe ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1771">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="4b7f8-1772">Zulassen der VM-Erstellung mit spezialisierter VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1772">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="4b7f8-1773">27. Februar 2017</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1773">February 27, 2017</span></span>

<span data-ttu-id="4b7f8-1774">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1774">Version 2.0.0</span></span>

<span data-ttu-id="4b7f8-1775">Diese Version der Azure CLI 2.0 ist die erste „allgemein verfügbare“ Version. Die allgemeine Verfügbarkeit gilt für die folgenden Befehlsmodule:</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1775">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="4b7f8-1776">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1776">Container Service (acs)</span></span>
- <span data-ttu-id="4b7f8-1777">Compute (einschließlich Resource Manager, VM, VM-Skalierungsgruppen, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1777">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="4b7f8-1778">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1778">Networking</span></span>
- <span data-ttu-id="4b7f8-1779">Speicher</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1779">Storage</span></span>

<span data-ttu-id="4b7f8-1780">Diese Befehlsmodule können in der Produktion verwendet werden und verfügen über Unterstützung durch eine Standard-SLA von Microsoft. Sie können Anfragen zu Problemen direkt beim Microsoft-Support oder in der [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/) öffnen. Sie haben die Möglichkeit, Fragen in [StackOverflow mit dem Tag „azure-cli“](http://stackoverflow.com/questions/tagged/azure-cli) zu stellen oder sich unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) an das Produktteam zu wenden. Außerdem können Sie über die Befehlszeile mit dem Befehl `az feedback` Feedback senden.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1780">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="4b7f8-1781">Die Befehle in diesen Modulen sind stabil, und es ist nicht zu erwarten, dass sich die Syntax in den anstehenden Veröffentlichungen dieser Version der Azure CLI ändern.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1781">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="4b7f8-1782">Verwenden Sie zum Überprüfen der Version der CLI den Befehl `az --version`. In der Ausgabe werden die Version der CLI selbst (für diese Veröffentlichung 2.0.0), die einzelnen Befehlsmodule und die von Ihnen genutzten Versionen von Python und GCC aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1782">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="4b7f8-1783">Einige Befehlsmodule verfügen über das Postfix „b*n*“ oder „rc*n*“. Diese Befehlsmodule befinden sich noch in der Vorschauphase und werden später die allgemeine Verfügbarkeit erlangen.</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1783">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="4b7f8-1784">Außerdem werden jeden Abend Vorschaubuilds der CLI bereitgestellt. Informationen hierzu finden Sie in der [Anleitung zum Abrufen der abendlichen Builds](https://github.com/Azure/azure-cli#nightly-builds) und im Abschnitt zum [Setup für Entwickler und Beitragen von Code](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1784">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="4b7f8-1785">Sie können für die abendlichen Vorschaubuilds wie folgt Probleme melden:</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1785">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="4b7f8-1786">Über die [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1786">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="4b7f8-1787">Per Kontaktaufnahme mit dem Produktteam unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1787">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="4b7f8-1788">Senden von Feedback über die Befehlszeile mit dem Befehl `az feedback`</span><span class="sxs-lookup"><span data-stu-id="4b7f8-1788">Provide feedback from the command line with the `az feedback` command</span></span>


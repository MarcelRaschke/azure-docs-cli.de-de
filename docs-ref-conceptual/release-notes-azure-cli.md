---
title: Versionshinweise für die Azure CLI
description: Enthält Informationen zu den aktuellen Updates der Azure CLI.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/21/2018
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: f0ee84c3f70cf168818de447289d6c7ab5a40c9e
ms.sourcegitcommit: c4462456dfb17993f098d47c37bc19f4d78b8179
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/25/2018
ms.locfileid: "47178081"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="4adad-103">Versionshinweise für die Azure CLI</span><span class="sxs-lookup"><span data-stu-id="4adad-103">Azure CLI release notes</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="4adad-104">21. September 2018</span><span class="sxs-lookup"><span data-stu-id="4adad-104">September 21, 2018</span></span>

<span data-ttu-id="4adad-105">Version 20.46</span><span class="sxs-lookup"><span data-stu-id="4adad-105">Version 20.46</span></span>

### <a name="acr"></a><span data-ttu-id="4adad-106">ACR</span><span class="sxs-lookup"><span data-stu-id="4adad-106">ACR</span></span>
* <span data-ttu-id="4adad-107">ACR-Aufgabenbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-107">Added ACR Task commands</span></span>
* <span data-ttu-id="4adad-108">Befehl für die Schnellausführung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-108">Added quick run command</span></span>
* <span data-ttu-id="4adad-109">`build-task`-Befehlsgruppe als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="4adad-109">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="4adad-110">`helm`-Befehlsgruppe hinzugefügt, um die Verwaltung von Helm-Diagrammen mit ACR zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="4adad-110">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="4adad-111">Unterstützung für idempotentes Erstellen für die verwaltete Registrierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-111">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="4adad-112">Formatfreies Flag für die Anzeige von Buildprotokollen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-112">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="4adad-113">ACS</span><span class="sxs-lookup"><span data-stu-id="4adad-113">ACS</span></span>
* <span data-ttu-id="4adad-114">Befehl `install-connector` zum Festlegen des AKS-Master-FQDN geändert</span><span class="sxs-lookup"><span data-stu-id="4adad-114">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="4adad-115">Erstellen der Rollenzuweisung für „vnet-subnet-id“ (wenn kein Dienstprinzipal angegeben wurde) und „skip-role-assignment“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="4adad-115">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="4adad-116">AppService</span><span class="sxs-lookup"><span data-stu-id="4adad-116">AppService</span></span>

* <span data-ttu-id="4adad-117">Unterstützung für WebJobs-Vorgangsverwaltung hinzugefügt (kontinuierlich/ausgelöst)</span><span class="sxs-lookup"><span data-stu-id="4adad-117">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="4adad-118">„az webapp config set“ unterstützt die Eigenschaft „--fts-state“; Unterstützung für „az functionapp config set/show“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-118">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="4adad-119">Unterstützung für Bring Your Own Storage für Web-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-119">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="4adad-120">Unterstützung für das Auflisten und Wiederherstellen gelöschter Web-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-120">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="4adad-121">Batch</span><span class="sxs-lookup"><span data-stu-id="4adad-121">Batch</span></span>
* <span data-ttu-id="4adad-122">Hinzufügen von Aufgaben über `--json-file` geändert, um die AddTaskCollectionParameter-Syntax zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="4adad-122">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="4adad-123">Dokumentation akzeptierter `--json-file`-Formate aktualisiert</span><span class="sxs-lookup"><span data-stu-id="4adad-123">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="4adad-124">`--max-tasks-per-node-option` zu `batch pool create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-124">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="4adad-125">Verhalten von `batch account` geändert, um das aktuell angemeldete Konto anzuzeigen, wenn keine Optionen angegeben wurden</span><span class="sxs-lookup"><span data-stu-id="4adad-125">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="4adad-126">Batch AI</span><span class="sxs-lookup"><span data-stu-id="4adad-126">Batch AI</span></span> 
* <span data-ttu-id="4adad-127">Fehler bei der automatischen Speicherkontoerstellung im Befehl `batchai cluster create` behoben</span><span class="sxs-lookup"><span data-stu-id="4adad-127">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="4adad-128">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="4adad-128">Cognitive Services</span></span>
* <span data-ttu-id="4adad-129">Vervollständigung für die Argumente `--sku`, `--kind` und `--location` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-129">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="4adad-130">Befehl `cognitiveservices account list-usage` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-130">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="4adad-131">Befehl `cognitiveservices account list-kinds` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-131">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="4adad-132">Befehl `cognitiveservices account list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-132">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="4adad-133">`cognitiveservices list` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="4adad-133">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="4adad-134">`--name` geändert (ist jetzt optional für `cognitiveservices account list-skus`)</span><span class="sxs-lookup"><span data-stu-id="4adad-134">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="4adad-135">Container</span><span class="sxs-lookup"><span data-stu-id="4adad-135">Container</span></span>
* <span data-ttu-id="4adad-136">Möglichkeit zum Neustarten und Beenden einer ausgeführten Containergruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-136">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="4adad-137">`--network-profile` zum Übergeben eines Netzwerkprofils hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-137">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="4adad-138">`--subnet` und `--vnet_name` hinzugefügt, um das Erstellen von Containergruppen in einem VNET zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="4adad-138">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="4adad-139">Tabellenausgabe geändert, sodass der Status der Containergruppe angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="4adad-139">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="4adad-140">Data Lake</span><span class="sxs-lookup"><span data-stu-id="4adad-140">Datalake</span></span>
* <span data-ttu-id="4adad-141">Befehle für VNET-Regeln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-141">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="4adad-142">Interaktive Shell</span><span class="sxs-lookup"><span data-stu-id="4adad-142">Interactive Shell</span></span>
* <span data-ttu-id="4adad-143">Fehler in Windows behoben, durch den Befehle nicht ordnungsgemäß ausgeführt wurden</span><span class="sxs-lookup"><span data-stu-id="4adad-143">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="4adad-144">Durch veraltete Objekte verursachtes Problem beim Laden von Befehlen im interaktiven Modus behoben</span><span class="sxs-lookup"><span data-stu-id="4adad-144">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="4adad-145">IoT</span><span class="sxs-lookup"><span data-stu-id="4adad-145">IoT</span></span>
* <span data-ttu-id="4adad-146">Routingunterstützung für IoT Hubs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-146">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="4adad-147">Key Vault</span><span class="sxs-lookup"><span data-stu-id="4adad-147">Key Vault</span></span>
* <span data-ttu-id="4adad-148">Key Vault-Schlüsselimport für RSA-Schlüssel korrigiert</span><span class="sxs-lookup"><span data-stu-id="4adad-148">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="4adad-149">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="4adad-149">Network</span></span>
* <span data-ttu-id="4adad-150">Befehle vom Typ `network public-ip prefix` hinzugefügt, um Präfixe von öffentlichen IP-Adressen zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="4adad-150">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="4adad-151">Befehle vom Typ `network service-endpoint` hinzugefügt, um Dienstendpunktrichtlinien-Features zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="4adad-151">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="4adad-152">Befehle vom Typ `network lb outbound-rule` hinzugefügt, um die Erstellung von Ausgangsregeln für Load Balancer Standard zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="4adad-152">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="4adad-153">`--public-ip-prefix` zu `network lb frontend-ip create/update` hinzugefügt, um Front-End-IP-Konfigurationen mit Präfixen von öffentlichen IP-Adressen zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="4adad-153">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="4adad-154">`--enable-tcp-reset` zu `network lb rule/inbound-nat-rule/inbound-nat-pool create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-154">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="4adad-155">`--disable-outbound-snat` zu `network lb rule create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-155">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="4adad-156">Verwendung von `network watcher flow-log show/configure` mit klassischen NSGs ermöglicht</span><span class="sxs-lookup"><span data-stu-id="4adad-156">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="4adad-157">Hinzufügen des `network watcher run-configuration-diagnostic`-Befehls</span><span class="sxs-lookup"><span data-stu-id="4adad-157">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="4adad-158">Befehl `network watcher test-connectivity` korrigiert und Eigenschaften `--method`, `--valid-status-codes` und `--headers` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-158">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="4adad-159">`network express-route create/update`: Flag `--allow-global-reach` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-159">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="4adad-160">`network vnet subnet create/update`: Unterstützung für `--delegation` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-160">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="4adad-161">Befehl `network vnet subnet list-available-delegations` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-161">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="4adad-162">`network traffic-manager profile create/update`: Unterstützung für `--interval`, `--timeout` und `--max-failures` für die Überwachungskonfiguration hinzugefügt; Optionen `--monitor-path`, `--monitor-port` und `--monitor-protocol` zugunsten von `--path`, `--port` und `--protocol` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="4adad-162">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="4adad-163">`network lb frontend-ip create/update`: Logik für das Festlegen der Zuweisungsmethode für private IP-Adressen korrigiert. Bei Angabe einer privaten IP-Adresse ist die Zuweisung statisch. Wird keine private IP-Adresse (oder eine leere Zeichenfolge für die private IP-Adresse) angegeben, erfolgt eine dynamische Zuweisung.</span><span class="sxs-lookup"><span data-stu-id="4adad-163">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="4adad-164">`dns record-set * create/update`: Unterstützung für `--target-resource` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-164">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="4adad-165">Befehle vom Typ `network interface-endpoint` hinzugefügt, um Schnittstellenendpunkt-Objekte abzufragen</span><span class="sxs-lookup"><span data-stu-id="4adad-165">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="4adad-166">`network profile show/list/delete` für die partielle Verwaltung von Netzwerkprofilen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-166">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="4adad-167">Befehle vom Typ `network express-route peering connection` für die Verwaltung von Peeringverbindungen zwischen ExpressRoute-Instanzen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-167">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="4adad-168">RDBMS</span><span class="sxs-lookup"><span data-stu-id="4adad-168">RDBMS</span></span>
* <span data-ttu-id="4adad-169">Unterstützung für den MariaDB-Dienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-169">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="4adad-170">Reservierung</span><span class="sxs-lookup"><span data-stu-id="4adad-170">Reservation</span></span>
* <span data-ttu-id="4adad-171">Cosmos DB im Enumerationstyp für reservierte Ressourcen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-171">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="4adad-172">Namenseigenschaft im Patchmodell hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-172">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="4adad-173">App-Verwaltung</span><span class="sxs-lookup"><span data-stu-id="4adad-173">Manage App</span></span>
* <span data-ttu-id="4adad-174">Fehler in `managedapp create --kind MarketPlace` korrigiert, der zum Absturz der Instanzerstellung einer verwalteten Marketplace-App führte</span><span class="sxs-lookup"><span data-stu-id="4adad-174">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="4adad-175">Befehle vom Typ `feature` geändert, um sie auf unterstützte Profile zu beschränken</span><span class="sxs-lookup"><span data-stu-id="4adad-175">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="4adad-176">Rolle</span><span class="sxs-lookup"><span data-stu-id="4adad-176">Role</span></span>
* <span data-ttu-id="4adad-177">Unterstützung für das Auflisten der Gruppenmitgliedschaften des Benutzers hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-177">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="4adad-178">SignalR</span><span class="sxs-lookup"><span data-stu-id="4adad-178">SignalR</span></span>
* <span data-ttu-id="4adad-179">Erste Version</span><span class="sxs-lookup"><span data-stu-id="4adad-179">First release</span></span>

### <a name="storage"></a><span data-ttu-id="4adad-180">Speicher</span><span class="sxs-lookup"><span data-stu-id="4adad-180">Storage</span></span>
* <span data-ttu-id="4adad-181">Parameter `--auth-mode login` für die Verwendung der Anmeldeinformationen des Benutzers für die Blob- und Warteschlangenautorisierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-181">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="4adad-182">`storage container immutability-policy/legal-hold` für die Verwaltung von unveränderlichem Speicher hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-182">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="4adad-183">VM</span><span class="sxs-lookup"><span data-stu-id="4adad-183">VM</span></span>
* <span data-ttu-id="4adad-184">Problem behoben, das dazu führte, dass die Datei mit dem privaten Schlüssel durch `vm create --generate-ssh-keys` überschrieben wird, wenn die Datei mit dem privaten Schlüssel fehlt (Nr. 4725, 6780)</span><span class="sxs-lookup"><span data-stu-id="4adad-184">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="4adad-185">Unterstützung für den gemeinsamen Image-Katalog über `az sig` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-185">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="4adad-186">28. August 2018</span><span class="sxs-lookup"><span data-stu-id="4adad-186">August 28, 2018</span></span>

<span data-ttu-id="4adad-187">Version 2.0.45</span><span class="sxs-lookup"><span data-stu-id="4adad-187">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="4adad-188">Core</span><span class="sxs-lookup"><span data-stu-id="4adad-188">Core</span></span>

* <span data-ttu-id="4adad-189">Das Problem, aufgrund dessen eine leere Konfigurationsdatei geladen wurde, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="4adad-189">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="4adad-190">Unterstützung für Profil `2018-03-01-hybrid` für Azure Stack hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-190">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="4adad-191">ACR</span><span class="sxs-lookup"><span data-stu-id="4adad-191">ACR</span></span>

* <span data-ttu-id="4adad-192">Problemumgehung für Laufzeitvorgänge ohne ARM-Anforderungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-192">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="4adad-193">Änderung vorgenommen, um im Befehl `build` Versionskontrolldateien (etwa „.git“ und „.gitignore“) standardmäßig aus der TAR-Datei auszuschließen</span><span class="sxs-lookup"><span data-stu-id="4adad-193">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="4adad-194">ACS</span><span class="sxs-lookup"><span data-stu-id="4adad-194">ACS</span></span>

* <span data-ttu-id="4adad-195">`aks create` geändert, dass standardmäßig virtuelle Computer vom Typ `Standard_DS2_v2` erstellt werden</span><span class="sxs-lookup"><span data-stu-id="4adad-195">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="4adad-196">`aks get-credentials` geändert, um nun neue APIs zum Abrufen der Clusteranmeldeinformationen aufzurufen</span><span class="sxs-lookup"><span data-stu-id="4adad-196">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="4adad-197">AppService</span><span class="sxs-lookup"><span data-stu-id="4adad-197">AppService</span></span>

* <span data-ttu-id="4adad-198">Unterstützung für CORS in „functionapp“ und „webapp“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-198">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="4adad-199">ARM-Tagunterstützung in Erstellungsbefehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-199">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="4adad-200">`[webapp|functionapp] identity show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="4adad-200">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="4adad-201">Backup</span><span class="sxs-lookup"><span data-stu-id="4adad-201">Backup</span></span>

* <span data-ttu-id="4adad-202">`backup vault backup-properties show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="4adad-202">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="4adad-203">Botdienst</span><span class="sxs-lookup"><span data-stu-id="4adad-203">Bot Service</span></span>

* <span data-ttu-id="4adad-204">Anfängliches Release der Botdienst-CLI</span><span class="sxs-lookup"><span data-stu-id="4adad-204">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="4adad-205">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="4adad-205">Cognitive Services</span></span>

* <span data-ttu-id="4adad-206">Neuer Parameter `--api-properties,` hinzugefügt, der zum Erstellen einiger Dienste erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="4adad-206">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="4adad-207">IoT</span><span class="sxs-lookup"><span data-stu-id="4adad-207">IoT</span></span>

* <span data-ttu-id="4adad-208">Problem mit dem Zuweisen verknüpfter Hubs behoben</span><span class="sxs-lookup"><span data-stu-id="4adad-208">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="4adad-209">Überwachen</span><span class="sxs-lookup"><span data-stu-id="4adad-209">Monitor</span></span>

* <span data-ttu-id="4adad-210">`monitor metrics alert`-Befehle für Metrikwarnungen nahezu in Echtzeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-210">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="4adad-211">`monitor alert`-Befehle als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="4adad-211">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="4adad-212">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="4adad-212">Network</span></span>

* <span data-ttu-id="4adad-213">`network application-gateway ssl-policy predefined show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="4adad-213">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="4adad-214">Ressource</span><span class="sxs-lookup"><span data-stu-id="4adad-214">Resource</span></span>

* <span data-ttu-id="4adad-215">`provider operation show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="4adad-215">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="4adad-216">Speicher</span><span class="sxs-lookup"><span data-stu-id="4adad-216">Storage</span></span>

* <span data-ttu-id="4adad-217">`storage share policy show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="4adad-217">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="4adad-218">VM</span><span class="sxs-lookup"><span data-stu-id="4adad-218">VM</span></span>

* <span data-ttu-id="4adad-219">`vm/vmss identity show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="4adad-219">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="4adad-220">`--storage-caching` für `vm create` eingestellt</span><span class="sxs-lookup"><span data-stu-id="4adad-220">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="4adad-221">14. August 2018</span><span class="sxs-lookup"><span data-stu-id="4adad-221">Auguest 14, 2018</span></span>

<span data-ttu-id="4adad-222">Version 2.0.44</span><span class="sxs-lookup"><span data-stu-id="4adad-222">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="4adad-223">Core</span><span class="sxs-lookup"><span data-stu-id="4adad-223">Core</span></span>

* <span data-ttu-id="4adad-224">Numerische Anzeige in `table`-Ausgabe korrigiert</span><span class="sxs-lookup"><span data-stu-id="4adad-224">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="4adad-225">YAML-Ausgabeformat hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-225">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="4adad-226">Telemetrie</span><span class="sxs-lookup"><span data-stu-id="4adad-226">Telemetry</span></span>

* <span data-ttu-id="4adad-227">Verbesserte Berichterstellung für Telemetriedaten</span><span class="sxs-lookup"><span data-stu-id="4adad-227">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="4adad-228">ACR</span><span class="sxs-lookup"><span data-stu-id="4adad-228">ACR</span></span>

* <span data-ttu-id="4adad-229">Befehle vom Typ `content-trust policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-229">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="4adad-230">Problem behoben, aufgrund dessen `.dockerignore` nicht richtig verarbeitet wurde</span><span class="sxs-lookup"><span data-stu-id="4adad-230">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="4adad-231">ACS</span><span class="sxs-lookup"><span data-stu-id="4adad-231">ACS</span></span>

* <span data-ttu-id="4adad-232">`az acs/aks install-cli` für die Installation in `%USERPROFILE%\.azure-kubectl` unter Windows geändert</span><span class="sxs-lookup"><span data-stu-id="4adad-232">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="4adad-233">`az aks install-connector` geändert, um zu ermitteln, ob der Cluster über RBAC verfügt, und um den ACI-Connector entsprechend zu konfigurieren</span><span class="sxs-lookup"><span data-stu-id="4adad-233">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="4adad-234">Geändert in Rollenzuweisung zum Subnetz bei entsprechender Angabe</span><span class="sxs-lookup"><span data-stu-id="4adad-234">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="4adad-235">Neue Option zum Überspringen der Rollenzuweisung für Subnetz hinzugefügt, wenn dieses angegeben ist</span><span class="sxs-lookup"><span data-stu-id="4adad-235">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="4adad-236">Geändert, um Rollenzuweisung zum Subnetz zu überspringen, wenn bereits eine Zuweisung vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="4adad-236">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="4adad-237">AppService</span><span class="sxs-lookup"><span data-stu-id="4adad-237">AppService</span></span>

* <span data-ttu-id="4adad-238">Fehler behoben, der das Erstellen einer Funktions-App mithilfe von Speicherkonten in externen Ressourcengruppen verhinderte</span><span class="sxs-lookup"><span data-stu-id="4adad-238">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="4adad-239">Absturz bei ZIP-Bereitstellung behoben</span><span class="sxs-lookup"><span data-stu-id="4adad-239">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="4adad-240">Batch AI</span><span class="sxs-lookup"><span data-stu-id="4adad-240">BatchAI</span></span>

* <span data-ttu-id="4adad-241">Protokollierungsausgabe für die automatische Speicherkontoerstellung geändert, sodass nun „Ressourcen*gruppe*“ angegeben wird</span><span class="sxs-lookup"><span data-stu-id="4adad-241">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="4adad-242">Container</span><span class="sxs-lookup"><span data-stu-id="4adad-242">Container</span></span>

* <span data-ttu-id="4adad-243">`--secure-environment-variables` zum Übergeben sicherer Umgebungsvariablen an einen Container hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-243">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="4adad-244">IoT</span><span class="sxs-lookup"><span data-stu-id="4adad-244">IoT</span></span>

* <span data-ttu-id="4adad-245">[WICHTIGE ÄNDERUNG] Veraltete Befehle entfernt, die in die IoT-Erweiterung verschoben wurden</span><span class="sxs-lookup"><span data-stu-id="4adad-245">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="4adad-246">Elemente aktualisiert, um nicht die Domäne `azure-devices.net` anzunehmen</span><span class="sxs-lookup"><span data-stu-id="4adad-246">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="4adad-247">Iot Central</span><span class="sxs-lookup"><span data-stu-id="4adad-247">Iot Central</span></span>

* <span data-ttu-id="4adad-248">Erstes Release des IoT Central-Moduls</span><span class="sxs-lookup"><span data-stu-id="4adad-248">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="4adad-249">KeyVault</span><span class="sxs-lookup"><span data-stu-id="4adad-249">KeyVault</span></span>


* <span data-ttu-id="4adad-250">Befehle zum Verwalten von Speicherkonten und SAS-Definitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-250">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="4adad-251">Befehle für Netzwerkregeln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-251">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="4adad-252">Parameter `--id` zu Geheimnis-, Schlüssel- und Zertifikatvorgängen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-252">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="4adad-253">Unterstützung für Version mit mehreren APIs zur Schlüsseltresorverwaltung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-253">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="4adad-254">Unterstützung für Version mit mehreren APIs zur Schlüsseltresordatenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-254">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="4adad-255">Relay</span><span class="sxs-lookup"><span data-stu-id="4adad-255">Relay</span></span>

* <span data-ttu-id="4adad-256">Erste Version</span><span class="sxs-lookup"><span data-stu-id="4adad-256">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="4adad-257">Sql</span><span class="sxs-lookup"><span data-stu-id="4adad-257">Sql</span></span>

* <span data-ttu-id="4adad-258">Befehle vom Typ `sql failover-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-258">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="4adad-259">Speicher</span><span class="sxs-lookup"><span data-stu-id="4adad-259">Storage</span></span>

* <span data-ttu-id="4adad-260">[WICHTIGE ÄNDERUNG] `storage account show-usage` geändert, um Parameter `--location` erforderlich zu machen. Auflistung nach Region</span><span class="sxs-lookup"><span data-stu-id="4adad-260">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="4adad-261">Parameter `--resource-group` geändert, sodass er für `storage account`-Befehle optional ist</span><span class="sxs-lookup"><span data-stu-id="4adad-261">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="4adad-262">Warnungen vom Typ „Fehler bei Vorbedingung“ für einzelne Fehler in Batch-Befehlen für eine aggregiert Nachricht entfernt</span><span class="sxs-lookup"><span data-stu-id="4adad-262">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="4adad-263">`[blob|file] delete-batch`-Befehle geändert, sodass kein Array mit Null-Werten mehr ausgegeben wird</span><span class="sxs-lookup"><span data-stu-id="4adad-263">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="4adad-264">`blob [download|upload|delete-batch]`-Befehle geändert, um SAS-Token aus Container-URL zu lesen</span><span class="sxs-lookup"><span data-stu-id="4adad-264">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="4adad-265">VM</span><span class="sxs-lookup"><span data-stu-id="4adad-265">VM</span></span>

* <span data-ttu-id="4adad-266">Allgemeine Filter zu `vm list-skus` für höhere Benutzerfreundlichkeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-266">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="4adad-267">31. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="4adad-267">July 31, 2018</span></span>

<span data-ttu-id="4adad-268">Version 2.0.43</span><span class="sxs-lookup"><span data-stu-id="4adad-268">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="4adad-269">ACR</span><span class="sxs-lookup"><span data-stu-id="4adad-269">ACR</span></span>

* <span data-ttu-id="4adad-270">Flag `--with-secure-properties` zum Befehl `acr build-task show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-270">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="4adad-271">Befehl `acr build-task update-build` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-271">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="4adad-272">ACS</span><span class="sxs-lookup"><span data-stu-id="4adad-272">ACS</span></span>

* <span data-ttu-id="4adad-273">Änderung, um 0 (Erfolg) zurückzugeben, wenn `az aks browse` durch Drücken von [STRG+C] beendet wird</span><span class="sxs-lookup"><span data-stu-id="4adad-273">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="4adad-274">Batch</span><span class="sxs-lookup"><span data-stu-id="4adad-274">Batch</span></span>

* <span data-ttu-id="4adad-275">Korrektur eines Fehlers bei der Anzeige des AAD-Tokens in Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="4adad-275">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="4adad-276">Container</span><span class="sxs-lookup"><span data-stu-id="4adad-276">Container</span></span>

* <span data-ttu-id="4adad-277">Voraussetzung von `--log-analytics-workspace-key` für Name oder ID im festgelegten Abonnement entfernt</span><span class="sxs-lookup"><span data-stu-id="4adad-277">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="4adad-278">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="4adad-278">Network</span></span>

* <span data-ttu-id="4adad-279">DNS-Unterstützung zu „2017-03-09-profile“ für Azure Stack hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-279">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="4adad-280">Ressource</span><span class="sxs-lookup"><span data-stu-id="4adad-280">Resource</span></span>

* <span data-ttu-id="4adad-281">`--rollback-on-error` zu `group deployment create` hinzugefügt, um bei einem Fehler eine als funktionierend bekannte Bereitstellung auszuführen</span><span class="sxs-lookup"><span data-stu-id="4adad-281">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="4adad-282">Problem behoben, aufgrund dessen `--parameters {}` mit `group deployment create` zu einem Fehler führte</span><span class="sxs-lookup"><span data-stu-id="4adad-282">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="4adad-283">Rolle</span><span class="sxs-lookup"><span data-stu-id="4adad-283">Role</span></span>

* <span data-ttu-id="4adad-284">Unterstützung für das Stack-Profil „2017-03-09-profile“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-284">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="4adad-285">Problem behoben, aufgrund dessen das generische Update von Parametern auf `app update` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="4adad-285">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="4adad-286">Suchen,</span><span class="sxs-lookup"><span data-stu-id="4adad-286">Search</span></span>

* <span data-ttu-id="4adad-287">Befehle für Azure Search-Dienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-287">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="4adad-288">Service Bus</span><span class="sxs-lookup"><span data-stu-id="4adad-288">Service Bus</span></span>

* <span data-ttu-id="4adad-289">Migrationsbefehlsgruppe hinzugefügt, um einen Namespace von Service Bus Standard zu Premium zu migrieren</span><span class="sxs-lookup"><span data-stu-id="4adad-289">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="4adad-290">Neue optionale Eigenschaften zu Service Bus-Warteschlange und -Abonnement hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-290">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="4adad-291">`--enable-batched-operations` und `--enable-dead-lettering-on-message-expiration` in `queue`</span><span class="sxs-lookup"><span data-stu-id="4adad-291">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="4adad-292">`--dead-letter-on-filter-exceptions` in `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="4adad-292">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="4adad-293">Speicher</span><span class="sxs-lookup"><span data-stu-id="4adad-293">Storage</span></span>

* <span data-ttu-id="4adad-294">Unterstützung für den Download großer Dateien über eine einzelne Verbindung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-294">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="4adad-295">`show`-Befehle konvertiert, bei denen im Falle einer fehlenden Ressource kein Fehler mit dem Exitcode 3 ausgelöst wurde</span><span class="sxs-lookup"><span data-stu-id="4adad-295">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="4adad-296">VM</span><span class="sxs-lookup"><span data-stu-id="4adad-296">VM</span></span>

* <span data-ttu-id="4adad-297">Unterstützung zum Auflisten von Verfügbarkeitsgruppen nach Abonnement hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-297">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="4adad-298">Unterstützung für `StandardSSD_LRS` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="4adad-298">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="4adad-299">Unterstützung für Anwendungssicherheitsgruppe beim Erstellen einer VM-Skalierungsgruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-299">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="4adad-300">[WICHTIGE ÄNDERUNG] `[vm|vmss] create`, `[vm|vmss] identity assign` und `[vm|vmss] identity remove` wurden geändert, um vom Benutzer zugewiesene Identitäten im Wörterbuchformat auszugeben.</span><span class="sxs-lookup"><span data-stu-id="4adad-300">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="4adad-301">18. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="4adad-301">July 18, 2018</span></span>

<span data-ttu-id="4adad-302">Version 2.0.42</span><span class="sxs-lookup"><span data-stu-id="4adad-302">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="4adad-303">Core</span><span class="sxs-lookup"><span data-stu-id="4adad-303">Core</span></span>

* <span data-ttu-id="4adad-304">Unterstützung für browserbasierte Anmeldung WSL-Bash-Fenster hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-304">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="4adad-305">`--force-string`-Flag für alle generischen Updatebefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-305">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="4adad-306">[WICHTIGE ÄNDERUNG] Befehle vom Typ „show“ so geändert, dass die Fehlermeldung protokolliert wird und der Vorgang bei einer fehlenden Ressource mit dem Exitcode 3 fehlschlägt</span><span class="sxs-lookup"><span data-stu-id="4adad-306">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="4adad-307">ACR</span><span class="sxs-lookup"><span data-stu-id="4adad-307">ACR</span></span>

* <span data-ttu-id="4adad-308">[WICHTIGE ÄNDERUNG] „--no-push“ in Befehl „acr build“ in reines Flag geändert</span><span class="sxs-lookup"><span data-stu-id="4adad-308">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="4adad-309">Befehle `show` und `update` unter Gruppe `acr repository` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-309">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="4adad-310">`--detail`-Flag für `show-manifests` und `show-tags` hinzugefügt, um ausführlichere Informationen anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="4adad-310">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="4adad-311">Parameter `--image` zur Unterstützung des Abrufs von Builddetails oder Protokollen anhand eines Images hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-311">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="4adad-312">ACS</span><span class="sxs-lookup"><span data-stu-id="4adad-312">ACS</span></span>

* <span data-ttu-id="4adad-313">`az aks create` so geändert, dass mit Fehler beendet wird, wenn `--max-pods` kleiner als 5 ist</span><span class="sxs-lookup"><span data-stu-id="4adad-313">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="4adad-314">AppService</span><span class="sxs-lookup"><span data-stu-id="4adad-314">AppService</span></span>

* <span data-ttu-id="4adad-315">Unterstützung für PremiumV2-SKUs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-315">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="4adad-316">Batch</span><span class="sxs-lookup"><span data-stu-id="4adad-316">Batch</span></span>

* <span data-ttu-id="4adad-317">Korrektur eines Fehlers bei der Verwendung von Anmeldeinformationen im Cloud Shell-Modus</span><span class="sxs-lookup"><span data-stu-id="4adad-317">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="4adad-318">JSON-Eingabe so geändert, dass Groß-/Kleinschreibung nicht beachtet wird</span><span class="sxs-lookup"><span data-stu-id="4adad-318">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="4adad-319">Batch AI</span><span class="sxs-lookup"><span data-stu-id="4adad-319">Batch AI</span></span>

* <span data-ttu-id="4adad-320">Befehl `az batchai job exec` korrigiert</span><span class="sxs-lookup"><span data-stu-id="4adad-320">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="4adad-321">Container</span><span class="sxs-lookup"><span data-stu-id="4adad-321">Container</span></span>

* <span data-ttu-id="4adad-322">Anforderung von Benutzername und Kennwort für Nicht-DockerHub-Registrierungen entfernt</span><span class="sxs-lookup"><span data-stu-id="4adad-322">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="4adad-323">Fehler beim Erstellen von Containergruppen aus YAML-Datei behoben</span><span class="sxs-lookup"><span data-stu-id="4adad-323">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="4adad-324">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="4adad-324">Network</span></span>

* <span data-ttu-id="4adad-325">Unterstützung für `--no-wait` zu `network nic [create|update|delete]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-325">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="4adad-326">`network nic wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-326">Added `network nic wait`</span></span>
* <span data-ttu-id="4adad-327">`--ids`-Argument für `network vnet [subnet|peering] list` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="4adad-327">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="4adad-328">`--include-default`-Flag hinzugefügt, um Standardsicherheitsregeln in die Ausgabe von `network nsg rule list` aufzunehmen</span><span class="sxs-lookup"><span data-stu-id="4adad-328">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="4adad-329">Ressource</span><span class="sxs-lookup"><span data-stu-id="4adad-329">Resource</span></span>

* <span data-ttu-id="4adad-330">Unterstützung für `--no-wait` zu `group deployment delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-330">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="4adad-331">Unterstützung für `--no-wait` zu `deployment delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-331">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="4adad-332">Befehl `deployment wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-332">Added `deployment wait` command</span></span>
* <span data-ttu-id="4adad-333">Problem behoben, aufgrund dessen die `az deployment`-Befehle auf Abonnementebene fälschlicherweise für Profil „2017-03-09-profile“ angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="4adad-333">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="4adad-334">SQL</span><span class="sxs-lookup"><span data-stu-id="4adad-334">SQL</span></span>

* <span data-ttu-id="4adad-335">Fehler „Der angegebene Ressourcengruppenname ... entsprach nicht dem Namen in der URL“ beim Angeben des Namens des Pools für elastische Datenbanken für `sql db copy`-und `sql db replica create`-Befehle behoben</span><span class="sxs-lookup"><span data-stu-id="4adad-335">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="4adad-336">Konfigurieren des Standard-SQL Servers durch Ausführen von `az configure --defaults sql-server=<name>` zulässig</span><span class="sxs-lookup"><span data-stu-id="4adad-336">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="4adad-337">Tabellenformatierer für Befehle `sql server`, `sql server firewall-rule`, `sql list-usages` und `sql show-usage` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-337">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="4adad-338">Speicher</span><span class="sxs-lookup"><span data-stu-id="4adad-338">Storage</span></span>

* <span data-ttu-id="4adad-339">`pageRanges`-Eigenschaft zu `storage blob show`-Ausgabe hinzugefügt, die für Seitenblobs ausgefüllt wird</span><span class="sxs-lookup"><span data-stu-id="4adad-339">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="4adad-340">VM</span><span class="sxs-lookup"><span data-stu-id="4adad-340">VM</span></span>

* <span data-ttu-id="4adad-341">[WICHTIGE ÄNDERUNG] `vmss create` so geändert, dass `Standard_DS1_v2` als standardmäßige Instanzgröße verwendet wird</span><span class="sxs-lookup"><span data-stu-id="4adad-341">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="4adad-342">Unterstützung für `--no-wait` zu `vm extension [set|delete]` und `vmss extension [set|delete]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-342">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="4adad-343">`vm extension wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-343">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="4adad-344">3. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="4adad-344">July 3, 2018</span></span>

<span data-ttu-id="4adad-345">Version 2.0.41</span><span class="sxs-lookup"><span data-stu-id="4adad-345">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="4adad-346">AKS</span><span class="sxs-lookup"><span data-stu-id="4adad-346">AKS</span></span>

* <span data-ttu-id="4adad-347">Überwachung geändert, sodass Abonnement-ID verwendet wird</span><span class="sxs-lookup"><span data-stu-id="4adad-347">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="4adad-348">3. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="4adad-348">July 3, 2018</span></span>

<span data-ttu-id="4adad-349">Version 2.0.40</span><span class="sxs-lookup"><span data-stu-id="4adad-349">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="4adad-350">Core</span><span class="sxs-lookup"><span data-stu-id="4adad-350">Core</span></span>

* <span data-ttu-id="4adad-351">Neuer Autorisierungscode-Flow für interaktive Anmeldung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-351">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="4adad-352">ACR</span><span class="sxs-lookup"><span data-stu-id="4adad-352">ACR</span></span>

* <span data-ttu-id="4adad-353">Abruf-Buildstatus hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-353">Added polling build status</span></span>
* <span data-ttu-id="4adad-354">Unterstützung für Enumerationswerte ohne Berücksichtigung von Groß-/Kleinschreibung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-354">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="4adad-355">Parameter `--top` und `--orderby` für `show-manifests` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-355">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="4adad-356">ACS</span><span class="sxs-lookup"><span data-stu-id="4adad-356">ACS</span></span>

* <span data-ttu-id="4adad-357">[WICHTIGE ÄNDERUNG] Standardmäßiges Aktivieren der rollenbasierten Zugriffssteuerung für Kubernetes</span><span class="sxs-lookup"><span data-stu-id="4adad-357">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="4adad-358">Argument `--disable-rbac` hinzugefügt und `--enable-rbac` als veraltet festgelegt, da es nun der Standard ist</span><span class="sxs-lookup"><span data-stu-id="4adad-358">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="4adad-359">Optionen für Befehl `aks browse` wurden aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="4adad-359">Updated options for `aks browse` command.</span></span> <span data-ttu-id="4adad-360">Unterstützung für `--listen-port` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-360">Added `--listen-port` support</span></span>
* <span data-ttu-id="4adad-361">Standardmäßiges Helm-Diagrammpaket für Befehl `aks install-connector` wurde aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="4adad-361">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="4adad-362">Verwenden von „virtual-kubelet-for-aks-latest.tgz“</span><span class="sxs-lookup"><span data-stu-id="4adad-362">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="4adad-363">Befehle `aks enable-addons` und `aks disable-addons` zum Aktualisieren eines vorhandenen Clusters hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-363">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="4adad-364">AppService</span><span class="sxs-lookup"><span data-stu-id="4adad-364">AppService</span></span>

* <span data-ttu-id="4adad-365">Unterstützung für das Deaktivieren der Identität über `webapp identity remove` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-365">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="4adad-366">`preview`-Tag für Identitätsfunktion entfernt</span><span class="sxs-lookup"><span data-stu-id="4adad-366">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="4adad-367">Backup</span><span class="sxs-lookup"><span data-stu-id="4adad-367">Backup</span></span>

* <span data-ttu-id="4adad-368">Moduldefinition aktualisiert</span><span class="sxs-lookup"><span data-stu-id="4adad-368">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="4adad-369">Batch AI</span><span class="sxs-lookup"><span data-stu-id="4adad-369">BatchAI</span></span>

* <span data-ttu-id="4adad-370">Tabellenausgabe für Befehle `batchai cluster node list` und `batchai job node list` korrigiert</span><span class="sxs-lookup"><span data-stu-id="4adad-370">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="4adad-371">Cloud</span><span class="sxs-lookup"><span data-stu-id="4adad-371">Cloud</span></span>

* <span data-ttu-id="4adad-372">Serversuffix `acr login` zu Cloudkonfiguration hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-372">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="4adad-373">Container</span><span class="sxs-lookup"><span data-stu-id="4adad-373">Container</span></span>

* <span data-ttu-id="4adad-374">`container create` zu Standard für Vorgang mit langer Ausführungsdauer geändert</span><span class="sxs-lookup"><span data-stu-id="4adad-374">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="4adad-375">Log Analytics-Parameter `--log-analytics-workspace` und `--log-analytics-workspace-key` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-375">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="4adad-376">Parameter `--protocol` zum Festlegen des zu verwendenden Netzwerkprotokolls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-376">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="4adad-377">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="4adad-377">Extension</span></span>

* <span data-ttu-id="4adad-378">`extension list-available` geändert, sodass nur mit der CLI-Version kompatible Erweiterungen angezeigt werden</span><span class="sxs-lookup"><span data-stu-id="4adad-378">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="4adad-379">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="4adad-379">Network</span></span>

* <span data-ttu-id="4adad-380">Problem behoben, aufgrund dessen bei Datensatztypen die Groß-/Kleinschreibung beachtet werden musste ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="4adad-380">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="4adad-381">Rdbms</span><span class="sxs-lookup"><span data-stu-id="4adad-381">Rdbms</span></span>

* <span data-ttu-id="4adad-382">Befehle vom Typ `[postgres|myql] server vnet-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-382">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="4adad-383">Ressource</span><span class="sxs-lookup"><span data-stu-id="4adad-383">Resource</span></span>

* <span data-ttu-id="4adad-384">Neue Vorgangsgruppe `deployment` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-384">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="4adad-385">VM</span><span class="sxs-lookup"><span data-stu-id="4adad-385">VM</span></span>

* <span data-ttu-id="4adad-386">Unterstützung für das Entfernen der vom System zugewiesenen Identität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-386">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="4adad-387">25. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="4adad-387">June 25, 2018</span></span>

<span data-ttu-id="4adad-388">Version 2.0.39</span><span class="sxs-lookup"><span data-stu-id="4adad-388">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="4adad-389">Befehlszeilenschnittstelle (CLI)</span><span class="sxs-lookup"><span data-stu-id="4adad-389">CLI</span></span>

* <span data-ttu-id="4adad-390">Dateieinschränkung in MSI-Installer aktualisiert, um Problem mit der Erweiterungsinstallation zu beheben</span><span class="sxs-lookup"><span data-stu-id="4adad-390">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="4adad-391">19. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="4adad-391">June 19, 2018</span></span>

<span data-ttu-id="4adad-392">Version 2.0.38</span><span class="sxs-lookup"><span data-stu-id="4adad-392">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="4adad-393">Core</span><span class="sxs-lookup"><span data-stu-id="4adad-393">Core</span></span>

* <span data-ttu-id="4adad-394">Globale Unterstützung für `--subscription` zu den meisten Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-394">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="4adad-395">ACR</span><span class="sxs-lookup"><span data-stu-id="4adad-395">ACR</span></span>

* <span data-ttu-id="4adad-396">`azure-storage-blob` als Abhängigkeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-396">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="4adad-397">CPU-Standardkonfiguration für `acr build-task create` geändert, sodass zwei Kerne verwendet werden</span><span class="sxs-lookup"><span data-stu-id="4adad-397">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="4adad-398">ACS</span><span class="sxs-lookup"><span data-stu-id="4adad-398">ACS</span></span>

* <span data-ttu-id="4adad-399">Optionen des Befehls `aks use-dev-spaces` wurden aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="4adad-399">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="4adad-400">Unterstützung für `--update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-400">Added `--update` support</span></span>
* <span data-ttu-id="4adad-401">`aks get-credentials --admin` geändert, sodass der Benutzerkontext in `$HOME/.kube/config` ersetzt wird</span><span class="sxs-lookup"><span data-stu-id="4adad-401">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="4adad-402">Schreibgeschützte `nodeResourceGroup`-Eigenschaft in verwalteten Clustern verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="4adad-402">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="4adad-403">Befehlsfehler `acs browse` korrigiert</span><span class="sxs-lookup"><span data-stu-id="4adad-403">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="4adad-404">`--connector-name` für `aks install-connector`, `aks upgrade-connector` und `aks remove-connector` als optional festgelegt</span><span class="sxs-lookup"><span data-stu-id="4adad-404">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="4adad-405">Neue Azure Container Instances-Regionen für `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-405">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="4adad-406">Normalisierter Speicherort im Helm-Versionsnamen und Knotenname zu `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-406">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="4adad-407">AppService</span><span class="sxs-lookup"><span data-stu-id="4adad-407">AppService</span></span>

* <span data-ttu-id="4adad-408">Unterstützung für neuere Versionen von „urllib“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-408">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="4adad-409">Unterstützung der Verwendung eines App Service-Plans aus externen Ressourcengruppen zu `functionapp create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-409">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="4adad-410">Batch</span><span class="sxs-lookup"><span data-stu-id="4adad-410">Batch</span></span>

* <span data-ttu-id="4adad-411">`azure-batch-extensions`-Abhängigkeit entfernt</span><span class="sxs-lookup"><span data-stu-id="4adad-411">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="4adad-412">Batch AI</span><span class="sxs-lookup"><span data-stu-id="4adad-412">Batch AI</span></span>

* <span data-ttu-id="4adad-413">Unterstützung für Arbeitsbereiche wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="4adad-413">Added support for workspaces.</span></span> <span data-ttu-id="4adad-414">Arbeitsbereiche ermöglichen das Zusammenfassen von Clustern, Dateiservern und Experimenten in Gruppen ohne Beschränkung der Anzahl von Ressourcen, die erstellt werden können.</span><span class="sxs-lookup"><span data-stu-id="4adad-414">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="4adad-415">Unterstützung für Experimente wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="4adad-415">Added support for experiments.</span></span> <span data-ttu-id="4adad-416">Experimente ermöglichen das Zusammenfassen von Aufträgen in Sammlungen ohne Beschränkung der Anzahl von erstellten Aufträgen.</span><span class="sxs-lookup"><span data-stu-id="4adad-416">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="4adad-417">Unterstützung für das Konfigurieren von `/dev/shm` für Aufträge hinzugefügt, die in einem Docker-Container ausgeführt werden</span><span class="sxs-lookup"><span data-stu-id="4adad-417">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="4adad-418">Die Befehle `batchai cluster node exec` und `batchai job node exec` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="4adad-418">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="4adad-419">Diese Befehle ermöglichen die Ausführung aller Befehle direkt auf Knoten und bieten Funktionen zur Portweiterleitung.</span><span class="sxs-lookup"><span data-stu-id="4adad-419">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="4adad-420">Unterstützung für `--ids` zu `batchai`-Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-420">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="4adad-421">[WICHTIGE ÄNDERUNG] Alle Cluster und Dateiserver müssen unter Arbeitsbereichen erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="4adad-421">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="4adad-422">[WICHTIGE ÄNDERUNG] Aufträge müssen unter Experimenten erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="4adad-422">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="4adad-423">[WICHTIGE ÄNDERUNG] `--nfs-resource-group` wurde aus den Befehlen `cluster create` und `job create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="4adad-423">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="4adad-424">Geben Sie zum Bereitstellen eines NFS, das einem anderen Arbeitsbereich/einer anderen Ressourcengruppe angehört, die ARM-ID des Dateiservers über die Option `--nfs` an.</span><span class="sxs-lookup"><span data-stu-id="4adad-424">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="4adad-425">[WICHTIGE ÄNDERUNG] `--cluster-resource-group` wurde aus dem Befehl `job create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="4adad-425">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="4adad-426">Geben Sie zum Übermitteln eines Auftrags, der einem anderen Arbeitsbereich/einer anderen Ressourcengruppe angehört, die ARM-ID des Clusters über die Option `--cluster` an.</span><span class="sxs-lookup"><span data-stu-id="4adad-426">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="4adad-427">[WICHTIGE ÄNDERUNG] Attribut `location` wurde aus Aufträgen, Clustern und Dateiservern entfernt.</span><span class="sxs-lookup"><span data-stu-id="4adad-427">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="4adad-428">„Location“ ist jetzt ein Attribut eines Arbeitsbereichs.</span><span class="sxs-lookup"><span data-stu-id="4adad-428">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="4adad-429">[WICHTIGE ÄNDERUNG] `--location` wurde aus den Befehlen `job create`, `cluster create` und `file-server create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="4adad-429">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="4adad-430">[WICHTIGE ÄNDERUNG] Namen von Kurzoptionen wurden geändert, um die Schnittstelle konsistenter zu machen:</span><span class="sxs-lookup"><span data-stu-id="4adad-430">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
 - <span data-ttu-id="4adad-431">[`--config`, `-c`] in [`--config-file`, `-f`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="4adad-431">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
 - <span data-ttu-id="4adad-432">[`--cluster`, `-r`] in [`--cluster`, `-c`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="4adad-432">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
 - <span data-ttu-id="4adad-433">[`--cluster`, `-n`] in [`--cluster`, `-c`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="4adad-433">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
 - <span data-ttu-id="4adad-434">[`--job`, `-n`] in [`--job`, `-j`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="4adad-434">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="4adad-435">Karten</span><span class="sxs-lookup"><span data-stu-id="4adad-435">Maps</span></span>

* <span data-ttu-id="4adad-436">[WICHTIGE ÄNDERUNG] `maps account create` wurde so geändert, dass Nutzungsbedingungen entweder durch interaktive Eingabeaufforderung oder `--accept-tos`-Flag akzeptiert werden müssen.</span><span class="sxs-lookup"><span data-stu-id="4adad-436">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="4adad-437">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="4adad-437">Network</span></span>

* <span data-ttu-id="4adad-438">Unterstützung für `https` zu `network lb probe create` hinzugefügt ([#6571](https://github.com/Azure/azure-cli/issues/6571))</span><span class="sxs-lookup"><span data-stu-id="4adad-438">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="4adad-439">Problem behoben, aufgrund dessen die Groß-/Kleinschreibung von `--endpoint-status` berücksichtigt wurde.</span><span class="sxs-lookup"><span data-stu-id="4adad-439">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="4adad-440">#6502</span><span class="sxs-lookup"><span data-stu-id="4adad-440">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="4adad-441">Reservations</span><span class="sxs-lookup"><span data-stu-id="4adad-441">Reservations</span></span>

* <span data-ttu-id="4adad-442">[WICHTIGE ÄNDERUNG] Erforderlicher Parameter `ReservedResourceType` zu `reservations catalog show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-442">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="4adad-443">Parameter `Location` zu `reservations catalog show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-443">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="4adad-444">[WICHTIGE ÄNDERUNG] `kind` aus `ReservationProperties` entfernt</span><span class="sxs-lookup"><span data-stu-id="4adad-444">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="4adad-445">[WICHTIGE ÄNDERUNG] `capabilities` wurde in `Catalog` in `sku_properties` umbenannt</span><span class="sxs-lookup"><span data-stu-id="4adad-445">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="4adad-446">[WICHTIGE ÄNDERUNG] Eigenschaften `size` und `tier` aus `Catalog` entfernt</span><span class="sxs-lookup"><span data-stu-id="4adad-446">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="4adad-447">Parameter `InstanceFlexibility` zu `reservations reservation update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-447">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="4adad-448">Rolle</span><span class="sxs-lookup"><span data-stu-id="4adad-448">Role</span></span>

* <span data-ttu-id="4adad-449">Fehlerbehandlung verbessert</span><span class="sxs-lookup"><span data-stu-id="4adad-449">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="4adad-450">SQL</span><span class="sxs-lookup"><span data-stu-id="4adad-450">SQL</span></span>

* <span data-ttu-id="4adad-451">Verwirrender Fehler behoben, der beim Ausführen von `az sql db list-editions` für einen Ort auftrat, der für Ihr Abonnement nicht verfügbar ist</span><span class="sxs-lookup"><span data-stu-id="4adad-451">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="4adad-452">Speicher</span><span class="sxs-lookup"><span data-stu-id="4adad-452">Storage</span></span>

* <span data-ttu-id="4adad-453">Lesbarkeit der Tabellenausgabe für `storage blob download` verbessert</span><span class="sxs-lookup"><span data-stu-id="4adad-453">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="4adad-454">VM</span><span class="sxs-lookup"><span data-stu-id="4adad-454">VM</span></span>

* <span data-ttu-id="4adad-455">Verbesserte Einschränkung der VM-Größenüberprüfung für Unterstützung von beschleunigten Netzwerken in `vm create`</span><span class="sxs-lookup"><span data-stu-id="4adad-455">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="4adad-456">Warnung für `vmss create` hinzugefügt, dass die VM-Standardgröße von `Standard_D1_v2` auf `Standard_DS1_v2` umgestellt wird</span><span class="sxs-lookup"><span data-stu-id="4adad-456">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="4adad-457">`--force-update` zu `[vm|vmss] extension set` hinzugefügt, um die Erweiterung auch dann zu aktualisieren, wenn die Konfiguration nicht geändert wurde</span><span class="sxs-lookup"><span data-stu-id="4adad-457">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="4adad-458">13. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="4adad-458">June 13, 2018</span></span>

<span data-ttu-id="4adad-459">Version 2.0.37</span><span class="sxs-lookup"><span data-stu-id="4adad-459">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="4adad-460">Core</span><span class="sxs-lookup"><span data-stu-id="4adad-460">Core</span></span>

* <span data-ttu-id="4adad-461">Verbesserte interaktive Telemetrie</span><span class="sxs-lookup"><span data-stu-id="4adad-461">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="4adad-462">13. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="4adad-462">June 13, 2018</span></span>

<span data-ttu-id="4adad-463">Version 2.0.36</span><span class="sxs-lookup"><span data-stu-id="4adad-463">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="4adad-464">AKS</span><span class="sxs-lookup"><span data-stu-id="4adad-464">AKS</span></span>

* <span data-ttu-id="4adad-465">Zusätzliche erweiterte Netzwerkoptionen zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-465">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="4adad-466">Argumente zu `aks create` zum Aktivieren der Überwachung und HTTP-Routing hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-466">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="4adad-467">Argument `--no-ssh-key` zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-467">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="4adad-468">Argument `--enable-rbac` zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-468">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="4adad-469">[VORSCHAUVERSION] Unterstützung für Azure Active Directory-Authentifizierung zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-469">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="4adad-470">AppService</span><span class="sxs-lookup"><span data-stu-id="4adad-470">AppService</span></span>

* <span data-ttu-id="4adad-471">Problem mit inkompatiblen urllib-Versionen behoben</span><span class="sxs-lookup"><span data-stu-id="4adad-471">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="4adad-472">5. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="4adad-472">June 5, 2018</span></span>

<span data-ttu-id="4adad-473">Version 2.0.35</span><span class="sxs-lookup"><span data-stu-id="4adad-473">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="4adad-474">Interactive</span><span class="sxs-lookup"><span data-stu-id="4adad-474">Interactive</span></span>

* <span data-ttu-id="4adad-475">Grenzwerte für die Abhängigkeiten des interaktiven Modus hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-475">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="4adad-476">5. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="4adad-476">June 5, 2018</span></span>

<span data-ttu-id="4adad-477">Version 2.0.34</span><span class="sxs-lookup"><span data-stu-id="4adad-477">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="4adad-478">Core</span><span class="sxs-lookup"><span data-stu-id="4adad-478">Core</span></span>

* <span data-ttu-id="4adad-479">Unterstützung für mandantenübergreifende Ressourcenverweise hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-479">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="4adad-480">Verbesserte Zuverlässigkeit bei Telemetrieuploads</span><span class="sxs-lookup"><span data-stu-id="4adad-480">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="4adad-481">ACR</span><span class="sxs-lookup"><span data-stu-id="4adad-481">ACR</span></span>

* <span data-ttu-id="4adad-482">Unterstützung für VSTS als Remotequellort hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-482">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="4adad-483">Befehl `acr import` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-483">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="4adad-484">AKS</span><span class="sxs-lookup"><span data-stu-id="4adad-484">AKS</span></span>

* <span data-ttu-id="4adad-485">`aks get-credentials` wurde geändert, um die Kube-Konfigurationsdatei mit sichereren Dateisystemberechtigungen zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="4adad-485">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="4adad-486">Batch</span><span class="sxs-lookup"><span data-stu-id="4adad-486">Batch</span></span>

* <span data-ttu-id="4adad-487">Fehler bei der Formatierung der Poollistentabelle behoben [[Problem 4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="4adad-487">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="4adad-488">IoT</span><span class="sxs-lookup"><span data-stu-id="4adad-488">IOT</span></span>

* <span data-ttu-id="4adad-489">Unterstützung für das Erstellen von IoT Hub-Instanzen im Tarif „Basic“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-489">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="4adad-490">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="4adad-490">Network</span></span>

* <span data-ttu-id="4adad-491">`network vnet peering` wurde verbessert.</span><span class="sxs-lookup"><span data-stu-id="4adad-491">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="4adad-492">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="4adad-492">Policy Insights</span></span>

* <span data-ttu-id="4adad-493">Erste Version</span><span class="sxs-lookup"><span data-stu-id="4adad-493">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="4adad-494">ARM</span><span class="sxs-lookup"><span data-stu-id="4adad-494">ARM</span></span>

* <span data-ttu-id="4adad-495">Befehle vom Typ `account management-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-495">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="4adad-496">SQL</span><span class="sxs-lookup"><span data-stu-id="4adad-496">SQL</span></span>

* <span data-ttu-id="4adad-497">Neue Befehle für verwaltete Instanzen hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="4adad-497">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="4adad-498">Neue Befehle für verwaltete Datenbanken hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="4adad-498">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="4adad-499">Speicher</span><span class="sxs-lookup"><span data-stu-id="4adad-499">Storage</span></span>

* <span data-ttu-id="4adad-500">Zusätzliche MimeTypes für JSON und JavaScript hinzugefügt (abzuleiten aus Dateierweiterungen)</span><span class="sxs-lookup"><span data-stu-id="4adad-500">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="4adad-501">VM</span><span class="sxs-lookup"><span data-stu-id="4adad-501">VM</span></span>

* <span data-ttu-id="4adad-502">`vm list-skus` wurde geändert, um feste Spalten zu verwenden und eine Warnung hinzuzufügen, dass `Tier` und `Size` entfernt werden.</span><span class="sxs-lookup"><span data-stu-id="4adad-502">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="4adad-503">Option `--accelerated-networking` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-503">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="4adad-504">`--tags` zu `identity create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-504">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="4adad-505">22. Mai 2018</span><span class="sxs-lookup"><span data-stu-id="4adad-505">May 22, 2018</span></span>

<span data-ttu-id="4adad-506">Version 2.0.33</span><span class="sxs-lookup"><span data-stu-id="4adad-506">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="4adad-507">Core</span><span class="sxs-lookup"><span data-stu-id="4adad-507">Core</span></span>

* <span data-ttu-id="4adad-508">Unterstützung für das Erweitern von `@` in Dateinamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-508">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="4adad-509">ACS</span><span class="sxs-lookup"><span data-stu-id="4adad-509">ACS</span></span>

* <span data-ttu-id="4adad-510">Neue Dev Spaces-Befehle `aks use-dev-spaces` und `aks remove-dev-spaces` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-510">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="4adad-511">Tippfehler in Hilfemeldung korrigiert</span><span class="sxs-lookup"><span data-stu-id="4adad-511">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="4adad-512">AppService</span><span class="sxs-lookup"><span data-stu-id="4adad-512">AppService</span></span>

* <span data-ttu-id="4adad-513">Verbesserte generische Aktualisierungsbefehle</span><span class="sxs-lookup"><span data-stu-id="4adad-513">Improved generic update commands</span></span>
* <span data-ttu-id="4adad-514">Asynchrone Unterstützung für `webapp deployment source config-zip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-514">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="4adad-515">Container</span><span class="sxs-lookup"><span data-stu-id="4adad-515">Container</span></span>

* <span data-ttu-id="4adad-516">Unterstützung für das Exportieren einer Containergruppe im YAML-Format hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-516">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="4adad-517">Unterstützung für die Verwendung einer YAML-Datei zum Erstellen/Aktualisieren einer Containergruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-517">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="4adad-518">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="4adad-518">Extension</span></span>

* <span data-ttu-id="4adad-519">Verbesserte Entfernung von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="4adad-519">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="4adad-520">Interactive</span><span class="sxs-lookup"><span data-stu-id="4adad-520">Interactive</span></span>

* <span data-ttu-id="4adad-521">Protokollierung geändert, um Parser für Abschlüsse zu deaktivieren</span><span class="sxs-lookup"><span data-stu-id="4adad-521">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="4adad-522">Verbesserte Verarbeitung beschädigter Hilfscaches</span><span class="sxs-lookup"><span data-stu-id="4adad-522">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="4adad-523">KeyVault</span><span class="sxs-lookup"><span data-stu-id="4adad-523">KeyVault</span></span>

* <span data-ttu-id="4adad-524">keyvault-Befehle wurden korrigiert, damit sie in Cloud Shell oder auf virtuellen Computern mit Identität verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="4adad-524">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="4adad-525">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="4adad-525">Network</span></span>

* <span data-ttu-id="4adad-526">Problem behoben, aufgrund dessen `network watcher show-topology` nicht mit einem VNET und/oder Subnetznamen verwendet werden konnte ([#6326](https://github.com/Azure/azure-cli/issues/6326))</span><span class="sxs-lookup"><span data-stu-id="4adad-526">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="4adad-527">Problem behoben, aufgrund dessen einige `network watcher`-Befehle fälschlicherweise angaben, dass Network Watcher nicht für bestimmte Regionen aktiviert ist ([#6264](https://github.com/Azure/azure-cli/issues/6264))</span><span class="sxs-lookup"><span data-stu-id="4adad-527">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="4adad-528">SQL</span><span class="sxs-lookup"><span data-stu-id="4adad-528">SQL</span></span>

* <span data-ttu-id="4adad-529">[WICHTIGE ÄNDERUNG] Von den Befehlen `db` und `dw` zurückgegebene Antwortobjekte geändert:</span><span class="sxs-lookup"><span data-stu-id="4adad-529">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="4adad-530">Eigenschaft `serviceLevelObjective` in `currentServiceObjectiveName` umbenannt</span><span class="sxs-lookup"><span data-stu-id="4adad-530">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="4adad-531">Eigenschaften `currentServiceObjectiveId` und `requestedServiceObjectiveId` entfernt</span><span class="sxs-lookup"><span data-stu-id="4adad-531">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="4adad-532">Eigenschaft `maxSizeBytes` geändert (ist nun keine Zeichenfolge mehr, sondern ein Ganzzahlwert)</span><span class="sxs-lookup"><span data-stu-id="4adad-532">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="4adad-533">[WICHTIGE ÄNDERUNG] Die folgenden `db`- und `dw`-Eigenschaften wurden geändert und sind jetzt schreibgeschützt:</span><span class="sxs-lookup"><span data-stu-id="4adad-533">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="4adad-534">`requestedServiceObjectiveName`(Fixierte Verbindung) festgelegt ist(Fixierte Verbindung) festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="4adad-534">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="4adad-535">Verwenden Sie zum Aktualisieren den Parameter `--service-objective`, oder legen Sie die Eigenschaft `sku.name` fest.</span><span class="sxs-lookup"><span data-stu-id="4adad-535">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="4adad-536">`edition`(Fixierte Verbindung) festgelegt ist(Fixierte Verbindung) festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="4adad-536">`edition`.</span></span> <span data-ttu-id="4adad-537">Verwenden Sie zum Aktualisieren den Parameter `--edition`, oder legen Sie die Eigenschaft `sku.tier` fest.</span><span class="sxs-lookup"><span data-stu-id="4adad-537">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="4adad-538">`elasticPoolName`(Fixierte Verbindung) festgelegt ist(Fixierte Verbindung) festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="4adad-538">`elasticPoolName`.</span></span> <span data-ttu-id="4adad-539">Verwenden Sie zum Aktualisieren den Parameter `--elastic-pool`, oder legen Sie die Eigenschaft `elasticPoolId` fest.</span><span class="sxs-lookup"><span data-stu-id="4adad-539">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="4adad-540">[WICHTIGE ÄNDERUNG] Die folgenden `elastic-pool`-Eigenschaften wurden geändert und sind jetzt schreibgeschützt:</span><span class="sxs-lookup"><span data-stu-id="4adad-540">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="4adad-541">`edition`(Fixierte Verbindung) festgelegt ist(Fixierte Verbindung) festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="4adad-541">`edition`.</span></span> <span data-ttu-id="4adad-542">Verwenden Sie zum Aktualisieren den Parameter `--edition`.</span><span class="sxs-lookup"><span data-stu-id="4adad-542">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="4adad-543">`dtu`(Fixierte Verbindung) festgelegt ist(Fixierte Verbindung) festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="4adad-543">`dtu`.</span></span> <span data-ttu-id="4adad-544">Verwenden Sie zum Aktualisieren den Parameter `--capacity`.</span><span class="sxs-lookup"><span data-stu-id="4adad-544">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="4adad-545">`databaseDtuMin`(Fixierte Verbindung) festgelegt ist(Fixierte Verbindung) festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="4adad-545">`databaseDtuMin`.</span></span> <span data-ttu-id="4adad-546">Verwenden Sie zum Aktualisieren den Parameter `--db-min-capacity`.</span><span class="sxs-lookup"><span data-stu-id="4adad-546">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="4adad-547">`databaseDtuMax`(Fixierte Verbindung) festgelegt ist(Fixierte Verbindung) festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="4adad-547">`databaseDtuMax`.</span></span> <span data-ttu-id="4adad-548">Verwenden Sie zum Aktualisieren den Parameter `--db-max-capacity`.</span><span class="sxs-lookup"><span data-stu-id="4adad-548">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="4adad-549">Die Parameter `--family` und `--capacity` wurden zu den `db`-, `dw`- und `elastic-pool`-Befehlen hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="4adad-549">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="4adad-550">Den `db`-, `dw`- und `elastic-pool`-Befehlen wurden Tabellenformatierer hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="4adad-550">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="4adad-551">Speicher</span><span class="sxs-lookup"><span data-stu-id="4adad-551">Storage</span></span>

* <span data-ttu-id="4adad-552">Vervollständigung für das Argument `--account-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-552">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="4adad-553">Problem mit `storage entity query` behoben</span><span class="sxs-lookup"><span data-stu-id="4adad-553">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="4adad-554">VM</span><span class="sxs-lookup"><span data-stu-id="4adad-554">VM</span></span>

* <span data-ttu-id="4adad-555">[WICHTIGE ÄNDERUNG] `--write-accelerator` aus `vm create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="4adad-555">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="4adad-556">Die gleiche Unterstützung kann über `vm update` oder `vm disk attach` erzielt werden.</span><span class="sxs-lookup"><span data-stu-id="4adad-556">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="4adad-557">Erweiterungsimageabgleich in `[vm|vmss] extension` korrigiert</span><span class="sxs-lookup"><span data-stu-id="4adad-557">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="4adad-558">`--boot-diagnostics-storage` zu `vm create` zur Erfassung des Startprotokolls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-558">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="4adad-559">`--license-type` zu `[vm|vmss] update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-559">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="4adad-560">7. Mai 2018</span><span class="sxs-lookup"><span data-stu-id="4adad-560">May 7, 2018</span></span>

<span data-ttu-id="4adad-561">Version 2.0.32</span><span class="sxs-lookup"><span data-stu-id="4adad-561">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="4adad-562">Core</span><span class="sxs-lookup"><span data-stu-id="4adad-562">Core</span></span>

* <span data-ttu-id="4adad-563">Ein Ausnahmefehler wurde behoben, der beim Abrufen von Geheimnissen aus einem Dienstprinzipalkonto mit Zertifikat auftrat.</span><span class="sxs-lookup"><span data-stu-id="4adad-563">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="4adad-564">Eingeschränkte Unterstützung für positionelle Argumente hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-564">Added limited support for positional arguments</span></span>
* <span data-ttu-id="4adad-565">Problem behoben, aufgrund dessen `--query` nicht mit `--ids` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="4adad-565">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="4adad-566">#5591</span><span class="sxs-lookup"><span data-stu-id="4adad-566">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="4adad-567">Pipingszenarien von Befehlen bei Verwendung von `--ids` verbessert</span><span class="sxs-lookup"><span data-stu-id="4adad-567">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="4adad-568">Unterstützt `-o tsv` mit angegebener Abfrage bzw. `-o json` ohne angegeben Abfrage</span><span class="sxs-lookup"><span data-stu-id="4adad-568">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="4adad-569">Befehlsvorschläge bei Fehler hinzugefügt, wenn Befehle Tippfehler enthielten</span><span class="sxs-lookup"><span data-stu-id="4adad-569">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="4adad-570">Fehler bei der Eingabe von `az ''` behandelt</span><span class="sxs-lookup"><span data-stu-id="4adad-570">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="4adad-571">Unterstützung für benutzerdefinierte Ressourcentypen für Befehlsmodule und -erweiterungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-571">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="4adad-572">ACR</span><span class="sxs-lookup"><span data-stu-id="4adad-572">ACR</span></span>

* <span data-ttu-id="4adad-573">ACR Build-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-573">Added ACR Build commands</span></span>
* <span data-ttu-id="4adad-574">Fehlermeldungen vom Typ „Ressource nicht gefunden.“ verbessert</span><span class="sxs-lookup"><span data-stu-id="4adad-574">Improved resource not found error messages</span></span>
* <span data-ttu-id="4adad-575">Höhere Leistung bei der Ressourcenerstellung und optimierte Fehlerbehandlung</span><span class="sxs-lookup"><span data-stu-id="4adad-575">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="4adad-576">ACR-Anmeldung bei nicht standardmäßigen Konsolen und WSL optimiert</span><span class="sxs-lookup"><span data-stu-id="4adad-576">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="4adad-577">Fehlermeldungen zu Repositorybefehlen optimiert</span><span class="sxs-lookup"><span data-stu-id="4adad-577">Improved repository commands error messages</span></span>
* <span data-ttu-id="4adad-578">Tabellenspalten und -reihenfolge aktualisiert</span><span class="sxs-lookup"><span data-stu-id="4adad-578">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="4adad-579">ACS</span><span class="sxs-lookup"><span data-stu-id="4adad-579">ACS</span></span>

* <span data-ttu-id="4adad-580">Warnung hinzugefügt, dass `az aks` eine Vorschauversion des Diensts ist</span><span class="sxs-lookup"><span data-stu-id="4adad-580">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="4adad-581">Berechtigungsproblem in `aks install-connector` behoben, wenn `--aci-resource-group` nicht angegeben wird</span><span class="sxs-lookup"><span data-stu-id="4adad-581">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="4adad-582">AMS</span><span class="sxs-lookup"><span data-stu-id="4adad-582">AMS</span></span>

* <span data-ttu-id="4adad-583">Erste Version: Verwalten von Azure Media Services-Ressourcen</span><span class="sxs-lookup"><span data-stu-id="4adad-583">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="4adad-584">AppService</span><span class="sxs-lookup"><span data-stu-id="4adad-584">Appservice</span></span>

* <span data-ttu-id="4adad-585">Ein Problem in `webapp delete` wurde behoben, das bei Angabe von `--slot` auftrat.</span><span class="sxs-lookup"><span data-stu-id="4adad-585">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="4adad-586">`--runtime-version` aus `webapp auth update` entfernt</span><span class="sxs-lookup"><span data-stu-id="4adad-586">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="4adad-587">Unterstützung für „min\_tls\_version“ und „https2.0“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-587">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="4adad-588">Unterstützung für mehrere Container hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-588">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="4adad-589">Batch AI</span><span class="sxs-lookup"><span data-stu-id="4adad-589">Batch AI</span></span>

* <span data-ttu-id="4adad-590">`batchai create cluster` wurde geändert, um die in der Konfigurationsdatei des Clusters konfigurierte VM-Priorität zu berücksichtigen.</span><span class="sxs-lookup"><span data-stu-id="4adad-590">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="4adad-591">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="4adad-591">Cognitive Services</span></span>

* <span data-ttu-id="4adad-592">Tippfehler im Beispiel für `cognitiveservices account create` korrigiert ([#5603](https://github.com/Azure/azure-cli/issues/5603))</span><span class="sxs-lookup"><span data-stu-id="4adad-592">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="4adad-593">Nutzung</span><span class="sxs-lookup"><span data-stu-id="4adad-593">Consumption</span></span>

* <span data-ttu-id="4adad-594">Neue Befehle für Budget-API hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-594">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="4adad-595">Container</span><span class="sxs-lookup"><span data-stu-id="4adad-595">Container</span></span>

* <span data-ttu-id="4adad-596">`--registry-server` muss nicht mehr für `container create` angegeben werden, wenn ein Registrierungsserver im Imagenamen enthalten ist.</span><span class="sxs-lookup"><span data-stu-id="4adad-596">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="4adad-597">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="4adad-597">Cosmos DB</span></span>

* <span data-ttu-id="4adad-598">VNET-Unterstützung für Azure CLI eingeführt: Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="4adad-598">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="4adad-599">DMS</span><span class="sxs-lookup"><span data-stu-id="4adad-599">DMS</span></span>

* <span data-ttu-id="4adad-600">Erste Version: Die Migration von SQL zu Azure SQL wird nun unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4adad-600">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="4adad-601">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="4adad-601">Extension</span></span>

* <span data-ttu-id="4adad-602">Fehler behoben, aufgrund dessen Erweiterungsmetadaten nicht mehr angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="4adad-602">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="4adad-603">Interactive</span><span class="sxs-lookup"><span data-stu-id="4adad-603">Interactive</span></span>

* <span data-ttu-id="4adad-604">Interaktive Vervollständigung funktioniert nun auch mit positionellen Argumenten.</span><span class="sxs-lookup"><span data-stu-id="4adad-604">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="4adad-605">Benutzerfreundlichere Ausgabe bei der Eingabe von '\'</span><span class="sxs-lookup"><span data-stu-id="4adad-605">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="4adad-606">Abschlüsse für Parameter ohne Hilfe korrigiert</span><span class="sxs-lookup"><span data-stu-id="4adad-606">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="4adad-607">Beschreibungen für Befehlsgruppen korrigiert</span><span class="sxs-lookup"><span data-stu-id="4adad-607">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="4adad-608">Labor</span><span class="sxs-lookup"><span data-stu-id="4adad-608">Lab</span></span>

* <span data-ttu-id="4adad-609">Regressionen aus Knack-Umwandlung korrigiert</span><span class="sxs-lookup"><span data-stu-id="4adad-609">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="4adad-610">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="4adad-610">Network</span></span>

* <span data-ttu-id="4adad-611">[WICHTIGE ÄNDERUNG] Parameter `--ids` entfernt für:</span><span class="sxs-lookup"><span data-stu-id="4adad-611">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="4adad-612">Profil</span><span class="sxs-lookup"><span data-stu-id="4adad-612">Profile</span></span>

* <span data-ttu-id="4adad-613">Quellerkennung für `disk create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="4adad-613">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="4adad-614">[WICHTIGE ÄNDERUNG] `--msi-port` und `--identity-port` entfernt, da sie nicht mehr verwendet werden</span><span class="sxs-lookup"><span data-stu-id="4adad-614">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="4adad-615">Tippfehler in kurzer Zusammenfassung für `account get-access-token` korrigiert</span><span class="sxs-lookup"><span data-stu-id="4adad-615">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="4adad-616">Redis</span><span class="sxs-lookup"><span data-stu-id="4adad-616">Redis</span></span>

* <span data-ttu-id="4adad-617">`redis patch-schedule patch-schedule show` wurde durch `redis patch-schedule show` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="4adad-617">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="4adad-618">`redis list-all` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="4adad-618">Deprecated `redis list-all`.</span></span> <span data-ttu-id="4adad-619">Diese Funktion wurde in `redis list` integriert.</span><span class="sxs-lookup"><span data-stu-id="4adad-619">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="4adad-620">`redis import-method` wurde durch `redis import` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="4adad-620">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="4adad-621">Unterstützung für `--ids` zu verschiedenen Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-621">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="4adad-622">Rolle</span><span class="sxs-lookup"><span data-stu-id="4adad-622">Role</span></span>

* <span data-ttu-id="4adad-623">[WICHTIGE ÄNDERUNG] Veralteter Befehl `ad sp reset-credentials` entfernt</span><span class="sxs-lookup"><span data-stu-id="4adad-623">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="4adad-624">Speicher</span><span class="sxs-lookup"><span data-stu-id="4adad-624">Storage</span></span>

* <span data-ttu-id="4adad-625">Zulassen, dass das Ziel-SAS-Token für die Blobkopie auf die Quelle angewendet wird, wenn Quell-SAS und Kontoschlüssel nicht angegeben werden</span><span class="sxs-lookup"><span data-stu-id="4adad-625">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="4adad-626">Verfügbar gemacht: Socket-Timeout für Blobuploads und -downloads</span><span class="sxs-lookup"><span data-stu-id="4adad-626">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="4adad-627">Blobnamen, die mit Pfadtrennzeichen beginnen, als relative Pfade behandeln</span><span class="sxs-lookup"><span data-stu-id="4adad-627">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="4adad-628">Zulassen, dass `storage blob copy --source-sas` mit dem Abfragezeichen „?“ beginnt</span><span class="sxs-lookup"><span data-stu-id="4adad-628">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="4adad-629">`storage entity query --marker` korrigiert, um Liste von Schlüsselwerten zu akzeptieren</span><span class="sxs-lookup"><span data-stu-id="4adad-629">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="4adad-630">VM</span><span class="sxs-lookup"><span data-stu-id="4adad-630">VM</span></span>

* <span data-ttu-id="4adad-631">Ungültige Erkennungslogik für nicht verwalteten Blob-URI korrigiert</span><span class="sxs-lookup"><span data-stu-id="4adad-631">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="4adad-632">Unterstützung für Datenträgerverschlüsselung ohne vom Benutzer bereitgestellte Dienstprinzipale hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-632">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="4adad-633">[WICHTIGE ÄNDERUNG] Verwenden Sie nicht „ManagedIdentityExtension“ des virtuellen Computers für MSI-Unterstützung.</span><span class="sxs-lookup"><span data-stu-id="4adad-633">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="4adad-634">Unterstützung für Entfernungsrichtlinie zu `vmss` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-634">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="4adad-635">[WICHTIGE ÄNDERUNG] `--ids` entfernt aus:</span><span class="sxs-lookup"><span data-stu-id="4adad-635">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="4adad-636">Unterstützung für Schreibbeschleunigung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-636">Added write accelerator support</span></span>
* <span data-ttu-id="4adad-637">`vmss perform-maintenance` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-637">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="4adad-638">`vm diagnostics set` korrigiert, um zuverlässig den Betriebssystemtyp des virtuellen Computers zu erkennen</span><span class="sxs-lookup"><span data-stu-id="4adad-638">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="4adad-639">`vm resize` geändert, um zu überprüfen, ob die angeforderte Größe von der derzeit festgelegten Größe abweicht, und nur bei einer Änderung eine Aktualisierung auszuführen</span><span class="sxs-lookup"><span data-stu-id="4adad-639">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="4adad-640">10. April 2018</span><span class="sxs-lookup"><span data-stu-id="4adad-640">April 10, 2018</span></span>

<span data-ttu-id="4adad-641">Version 2.0.31</span><span class="sxs-lookup"><span data-stu-id="4adad-641">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="4adad-642">ACR</span><span class="sxs-lookup"><span data-stu-id="4adad-642">ACR</span></span>

* <span data-ttu-id="4adad-643">Verbesserte Fehlerbehandlung für wincred-Fallback</span><span class="sxs-lookup"><span data-stu-id="4adad-643">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="4adad-644">ACS</span><span class="sxs-lookup"><span data-stu-id="4adad-644">ACS</span></span>

* <span data-ttu-id="4adad-645">Gültigkeit von per AKS erstellten SPNs in fünf Jahre geändert</span><span class="sxs-lookup"><span data-stu-id="4adad-645">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="4adad-646">AppService</span><span class="sxs-lookup"><span data-stu-id="4adad-646">Appservice</span></span>

* [WICHTIGE ÄNDERUNG]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="4adad-648">Nicht abgefangene Ausnahme für nicht vorhandene Web-App-Pläne behoben</span><span class="sxs-lookup"><span data-stu-id="4adad-648">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="4adad-649">Batch AI</span><span class="sxs-lookup"><span data-stu-id="4adad-649">BatchAI</span></span>

* <span data-ttu-id="4adad-650">Unterstützung für API 2018-03-01 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-650">Added support for 2018-03-01 API</span></span>

 - <span data-ttu-id="4adad-651">Bereitstellung auf Auftragsebene</span><span class="sxs-lookup"><span data-stu-id="4adad-651">Job level mounting</span></span>
 - <span data-ttu-id="4adad-652">Umgebungsvariablen mit Geheimniswerten</span><span class="sxs-lookup"><span data-stu-id="4adad-652">Environment variables with secret values</span></span>
 - <span data-ttu-id="4adad-653">Einstellungen von Leistungsindikatoren</span><span class="sxs-lookup"><span data-stu-id="4adad-653">Performance counters settings</span></span>
 - <span data-ttu-id="4adad-654">Berichtstellung für auftragsspezifisches Pfadsegment</span><span class="sxs-lookup"><span data-stu-id="4adad-654">Reporting of job specific path segment</span></span>
 - <span data-ttu-id="4adad-655">Unterstützung für Unterordner in Listendateien-API</span><span class="sxs-lookup"><span data-stu-id="4adad-655">Support for subfolders in list files api</span></span>
 - <span data-ttu-id="4adad-656">Berichterstellung zur Nutzung und zu Grenzwerten</span><span class="sxs-lookup"><span data-stu-id="4adad-656">Usage and limits reporting</span></span>
 - <span data-ttu-id="4adad-657">Zulassen der Angabe des Cachetyps für NFS-Server</span><span class="sxs-lookup"><span data-stu-id="4adad-657">Allow to specify caching type for NFS servers</span></span>
 - <span data-ttu-id="4adad-658">Unterstützung für benutzerdefinierte Images</span><span class="sxs-lookup"><span data-stu-id="4adad-658">Support for custom images</span></span>
 - <span data-ttu-id="4adad-659">Unterstützung für pyTorch-Toolkit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-659">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="4adad-660">Befehl `job wait` hinzugefügt, der das Warten auf die Auftragsfertigstellung ermöglicht und den Code für die Auftragsbeendigung meldet</span><span class="sxs-lookup"><span data-stu-id="4adad-660">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="4adad-661">Befehl `usage show` hinzugefügt, mit dem die aktuelle Nutzung von Batch AI-Ressourcen und die Grenzwerte für verschiedene Regionen aufgelistet werden</span><span class="sxs-lookup"><span data-stu-id="4adad-661">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="4adad-662">Nationale Clouds werden unterstützt</span><span class="sxs-lookup"><span data-stu-id="4adad-662">National clouds are supported</span></span>
* <span data-ttu-id="4adad-663">Befehlszeilenargumente für Aufträge hinzugefügt, um das Bereitstellen von Dateisystemen auf Auftragsebene zusätzlich zu Konfigurationsdateien zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="4adad-663">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="4adad-664">Weitere Optionen zum Anpassen von Clustern hinzugefügt – VM-Priorität, Subnetz, anfängliche Knotenanzahl für Cluster mit automatischer Skalierung, Angeben eines benutzerdefinierten Images</span><span class="sxs-lookup"><span data-stu-id="4adad-664">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="4adad-665">Befehlszeilenoption zum Angeben des Cachetyps für NFS mit Verwaltung per Batch AI hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-665">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="4adad-666">Angeben der Bereitstellung von Dateisystemen in Konfigurationsdateien vereinfacht.</span><span class="sxs-lookup"><span data-stu-id="4adad-666">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="4adad-667">Weglassen von Anmeldeinformationen für Azure-Dateifreigaben und Azure-Blobcontainer ist jetzt möglich. Die CLI füllt fehlende Anmeldeinformationen auf, indem der Speicherkontoschlüssel verwendet wird, der über Befehlszeilenparameter oder per Umgebungsvariable angegeben wird, oder der Schlüssel wird über Azure Storage abgefragt (sofern das Speicherkonto zum aktuellen Abonnement gehört).</span><span class="sxs-lookup"><span data-stu-id="4adad-667">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="4adad-668">Der Befehl zum Streamen von Auftragsdateien wird jetzt automatisch abgeschlossen, nachdem der Auftrag beendet ist (Erfolg, Fehler, Beendigung oder Löschung)</span><span class="sxs-lookup"><span data-stu-id="4adad-668">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="4adad-669">Verbesserte `table`-Ausgabe für `show`-Vorgänge</span><span class="sxs-lookup"><span data-stu-id="4adad-669">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="4adad-670">Option `--use-auto-storage` für die Clustererstellung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="4adad-670">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="4adad-671">Diese Option erleichtert die Verwaltung von Speicherkonten und die Bereitstellung von Azure-Dateifreigaben und Azure-Blobcontainern in Clustern.</span><span class="sxs-lookup"><span data-stu-id="4adad-671">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="4adad-672">`--generate-ssh-keys` für `cluster create` und `file-server create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-672">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="4adad-673">Möglichkeit zum Angeben der Knotensetupaufgabe über die Befehlszeile</span><span class="sxs-lookup"><span data-stu-id="4adad-673">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="4adad-674">[WICHTIGE ÄNDERUNG] Befehl `job stream-file` und `job list-files` in die Gruppe `job file` verschoben</span><span class="sxs-lookup"><span data-stu-id="4adad-674">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="4adad-675">[WICHTIGE ÄNDERUNG] `--admin-user-name` im Befehl `file-server create` in `--user-name` umbenannt, um Einheitlichkeit mit dem Befehl `cluster create` zu erzielen</span><span class="sxs-lookup"><span data-stu-id="4adad-675">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="4adad-676">Abrechnung</span><span class="sxs-lookup"><span data-stu-id="4adad-676">Billing</span></span>

* <span data-ttu-id="4adad-677">Registrierungskontobefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-677">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="4adad-678">Nutzung</span><span class="sxs-lookup"><span data-stu-id="4adad-678">Consumption</span></span>

* <span data-ttu-id="4adad-679">Befehle vom Typ `marketplace` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-679">Added `marketplace` commands</span></span>
* <span data-ttu-id="4adad-680">[WICHTIGE ÄNDERUNG] `reservations summaries` in `reservation summary` umbenannt</span><span class="sxs-lookup"><span data-stu-id="4adad-680">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="4adad-681">[WICHTIGE ÄNDERUNG] `reservations details` in `reservation detail` umbenannt</span><span class="sxs-lookup"><span data-stu-id="4adad-681">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="4adad-682">[WICHTIGE ÄNDERUNG] Kurzoptionen `--reservation-order-id` und `--reservation-id` für `reservation`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="4adad-682">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="4adad-683">[WICHTIGE ÄNDERUNG] `--grain`-Kurzoptionen für `reservation summary`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="4adad-683">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="4adad-684">[WICHTIGE ÄNDERUNG] `--include-meter-details`-Kurzoptionen für `pricesheet`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="4adad-684">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="4adad-685">Container</span><span class="sxs-lookup"><span data-stu-id="4adad-685">Container</span></span>

* <span data-ttu-id="4adad-686">Git-Repository-Parameter `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` und `--gitrepo-mount-path` für die Volumebereitstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-686">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="4adad-687">[#5926](https://github.com/Azure/azure-cli/issues/5926) behoben: Fehler bei `az container exec`, wenn „--container-name“ angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="4adad-687">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="4adad-688">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="4adad-688">Extension</span></span>

* <span data-ttu-id="4adad-689">Meldung für Distributionsüberprüfung in Debugebene geändert</span><span class="sxs-lookup"><span data-stu-id="4adad-689">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="4adad-690">Interactive</span><span class="sxs-lookup"><span data-stu-id="4adad-690">Interactive</span></span>

* <span data-ttu-id="4adad-691">Geändert: Verhinderung des Abschlusses bei nicht erkannten Befehlen</span><span class="sxs-lookup"><span data-stu-id="4adad-691">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="4adad-692">Ereignishooks vor und nach der Erstellung der Teilstruktur von Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-692">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="4adad-693">Abschluss für `--ids`-Parameter hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-693">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="4adad-694">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="4adad-694">Network</span></span>

* <span data-ttu-id="4adad-695">[#5936](https://github.com/Azure/azure-cli/issues/5936) behoben: `application-gateway create`-Tags konnten nicht festgelegt werden</span><span class="sxs-lookup"><span data-stu-id="4adad-695">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="4adad-696">Argument `--auth-certs` zum Anfügen von Authentifizierungszertifikaten für `application-gateway http-settings [create|update]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="4adad-696">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="4adad-697">#4910</span><span class="sxs-lookup"><span data-stu-id="4adad-697">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="4adad-698">`ddos-protection`-Befehle zum Erstellen von DDoS-Schutzplänen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-698">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="4adad-699">Unterstützung von `--ddos-protection-plan` für `vnet [create|update]` hinzugefügt, um das Zuordnen eines VNET zu einem DDoS-Schutzplan zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="4adad-699">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="4adad-700">Problem mit `--disable-bgp-route-propagation`-Flag in `network route-table [create|update]` behoben</span><span class="sxs-lookup"><span data-stu-id="4adad-700">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="4adad-701">Dummy-Argumente `--public-ip-address-type` und `--subnet-type` für `network lb [create|update]` entfernt</span><span class="sxs-lookup"><span data-stu-id="4adad-701">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="4adad-702">Unterstützung für TXT-Datensätze mit RFC 1035-Escapesequenzen für `network dns zone [import|export]` und `network dns record-set txt add-record` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-702">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="4adad-703">Profil</span><span class="sxs-lookup"><span data-stu-id="4adad-703">Profile</span></span>

* <span data-ttu-id="4adad-704">Unterstützung für klassische Azure-Konten in `account list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-704">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="4adad-705">[WICHTIGE ÄNDERUNG] `--msi` & `--msi-port`-Argumente entfernt</span><span class="sxs-lookup"><span data-stu-id="4adad-705">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="4adad-706">RDBMS</span><span class="sxs-lookup"><span data-stu-id="4adad-706">RDBMS</span></span>

* <span data-ttu-id="4adad-707">Befehl `georestore` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-707">Added `georestore` command</span></span>
* <span data-ttu-id="4adad-708">Speichergrößenbeschränkung aus Befehl `create` entfernt</span><span class="sxs-lookup"><span data-stu-id="4adad-708">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="4adad-709">Ressource</span><span class="sxs-lookup"><span data-stu-id="4adad-709">Resource</span></span>

* <span data-ttu-id="4adad-710">Unterstützung für `--metadata` zu `policy definition create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-710">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="4adad-711">Unterstützung von `--metadata`, `--set`, `--add`, `--remove` für `policy definition update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-711">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="4adad-712">SQL</span><span class="sxs-lookup"><span data-stu-id="4adad-712">SQL</span></span>

* <span data-ttu-id="4adad-713">`sql elastic-pool op list` und `sql elastic-pool op cancel` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-713">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="4adad-714">Speicher</span><span class="sxs-lookup"><span data-stu-id="4adad-714">Storage</span></span>

* <span data-ttu-id="4adad-715">Fehlermeldungen für falsch formatierte Verbindungszeichenfolgen verbessert</span><span class="sxs-lookup"><span data-stu-id="4adad-715">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="4adad-716">VM</span><span class="sxs-lookup"><span data-stu-id="4adad-716">VM</span></span>

* <span data-ttu-id="4adad-717">Unterstützung für die Konfiguration der Plattform-Fehlerdomänenanzahl für `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-717">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="4adad-718">`vmss create` geändert, damit standardmäßig „Standard LB“ für zonales, großes oder per einzelner Platzierungsgruppe deaktiviertes Scale Set festgelegt wird</span><span class="sxs-lookup"><span data-stu-id="4adad-718">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [WICHTIGE ÄNDERUNG]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="4adad-720">Unterstützung für SKU mit öffentlicher IP für `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-720">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="4adad-721">Argumente `--keyvault` und `--resource-group` für `vm secret format` hinzugefügt, um Szenarien zu unterstützen, bei denen der Befehl die Tresor-ID nicht auflösen kann.</span><span class="sxs-lookup"><span data-stu-id="4adad-721">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="4adad-722">#5718</span><span class="sxs-lookup"><span data-stu-id="4adad-722">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="4adad-723">Bessere Fehler für `[vm|vmss create]`, wenn der Standort einer Ressourcengruppe keine Zonenunterstützung aufweist</span><span class="sxs-lookup"><span data-stu-id="4adad-723">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="4adad-724">27. März 2018</span><span class="sxs-lookup"><span data-stu-id="4adad-724">March 27, 2018</span></span>

<span data-ttu-id="4adad-725">Version 2.0.30</span><span class="sxs-lookup"><span data-stu-id="4adad-725">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="4adad-726">Core</span><span class="sxs-lookup"><span data-stu-id="4adad-726">Core</span></span>

* <span data-ttu-id="4adad-727">Anzeigen einer Meldung für Erweiterungen, die in der Hilfe als Vorschauversion gekennzeichnet sind</span><span class="sxs-lookup"><span data-stu-id="4adad-727">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="4adad-728">ACS</span><span class="sxs-lookup"><span data-stu-id="4adad-728">ACS</span></span>

* <span data-ttu-id="4adad-729">Behebung eines Fehlers bei der SSL-Zertifikatprüfung für `aks install-cli` in Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="4adad-729">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="4adad-730">AppService</span><span class="sxs-lookup"><span data-stu-id="4adad-730">Appservice</span></span>

* <span data-ttu-id="4adad-731">Unterstützung nur von HTTPS zu `webapp update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-731">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="4adad-732">Unterstützung für Slots zu `az webapp identity [assign|show]` und `az functionapp identity [assign|show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-732">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="4adad-733">Backup</span><span class="sxs-lookup"><span data-stu-id="4adad-733">Backup</span></span>

* <span data-ttu-id="4adad-734">Neuer Befehl `az backup protection isenabled-for-vm` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="4adad-734">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="4adad-735">Mit diesem Befehl kann überprüft werden, ob ein virtueller Computer von einem beliebigen Tresor im Abonnement gesichert wird.</span><span class="sxs-lookup"><span data-stu-id="4adad-735">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="4adad-736">Azure-Objekt-IDs für Parameter `--resource-group` und `--vault-name` für die folgenden Befehle aktiviert:</span><span class="sxs-lookup"><span data-stu-id="4adad-736">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="4adad-737">`--name`-Parameter wurden geändert, um das Ausgabeformat von `backup ... show`-Befehlen zu akzeptieren.</span><span class="sxs-lookup"><span data-stu-id="4adad-737">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="4adad-738">Container</span><span class="sxs-lookup"><span data-stu-id="4adad-738">Container</span></span>

* <span data-ttu-id="4adad-739">Befehl `container exec` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="4adad-739">Added `container exec` command.</span></span> <span data-ttu-id="4adad-740">Ausführung von Befehlen in einem Container für eine ausgeführte Containergruppe</span><span class="sxs-lookup"><span data-stu-id="4adad-740">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="4adad-741">Zulassen der Tabellenausgabe zum Erstellen und Aktualisieren einer Containergruppe</span><span class="sxs-lookup"><span data-stu-id="4adad-741">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="4adad-742">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="4adad-742">Extension</span></span>

* <span data-ttu-id="4adad-743">Meldung für `extension add` hinzugefügt, wenn sich die Erweiterung in der Vorschauphase befindet</span><span class="sxs-lookup"><span data-stu-id="4adad-743">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="4adad-744">`extension list-available` geändert, um vollständige Erweiterungsdaten mit `--show-details` anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="4adad-744">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="4adad-745">[WICHTIGE ÄNDERUNG] `extension list-available` geändert, um standardmäßig vereinfachte Erweiterungsdaten anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="4adad-745">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="4adad-746">Interactive</span><span class="sxs-lookup"><span data-stu-id="4adad-746">Interactive</span></span>

* <span data-ttu-id="4adad-747">Vervollständigungen wurden geändert und werden jetzt aktiviert, sobald das Laden der Befehlstabelle abgeschlossen ist.</span><span class="sxs-lookup"><span data-stu-id="4adad-747">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="4adad-748">Fehler bei der Verwendung des Parameters `--style` behoben</span><span class="sxs-lookup"><span data-stu-id="4adad-748">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="4adad-749">Interaktiver Lexer nach Befehlstabellensicherung instanziiert (sofern nicht vorhanden)</span><span class="sxs-lookup"><span data-stu-id="4adad-749">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="4adad-750">Verbesserte Unterstützung der Vervollständigung</span><span class="sxs-lookup"><span data-stu-id="4adad-750">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="4adad-751">Labor</span><span class="sxs-lookup"><span data-stu-id="4adad-751">Lab</span></span>

* <span data-ttu-id="4adad-752">Probleme mit Befehl `create environment` behoben</span><span class="sxs-lookup"><span data-stu-id="4adad-752">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="4adad-753">Überwachen</span><span class="sxs-lookup"><span data-stu-id="4adad-753">Monitor</span></span>

* <span data-ttu-id="4adad-754">Unterstützung für `--top`, `--orderby` und `--namespace` zu `metrics list` hinzugefügt ([#5785](https://github.com/Azure/azure-cli/issues/5785))</span><span class="sxs-lookup"><span data-stu-id="4adad-754">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="4adad-755">[#4529](https://github.com/Azure/azure-cli/issues/5785) behoben: `metrics list` akzeptiert eine durch Leerzeichen getrennte Liste von abzurufenden Metriken.</span><span class="sxs-lookup"><span data-stu-id="4adad-755">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="4adad-756">Unterstützung für `--namespace` zu `metrics list-definitions` hinzugefügt ([#5785](https://github.com/Azure/azure-cli/issues/5785))</span><span class="sxs-lookup"><span data-stu-id="4adad-756">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="4adad-757">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="4adad-757">Network</span></span>

* <span data-ttu-id="4adad-758">Unterstützung für private DNS-Zonen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-758">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="4adad-759">Profil</span><span class="sxs-lookup"><span data-stu-id="4adad-759">Profile</span></span>

* <span data-ttu-id="4adad-760">Warnung für `--identity-port` und `--msi-port` zu `login` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-760">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="4adad-761">RDBMS</span><span class="sxs-lookup"><span data-stu-id="4adad-761">RDBMS</span></span>

* <span data-ttu-id="4adad-762">GA-API-Version 2017-12-01 (Geschäftsmodell) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-762">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="4adad-763">Ressource</span><span class="sxs-lookup"><span data-stu-id="4adad-763">Resource</span></span>

* [WICHTIGE ÄNDERUNG]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="4adad-765">Rolle</span><span class="sxs-lookup"><span data-stu-id="4adad-765">Role</span></span>

* <span data-ttu-id="4adad-766">Unterstützung für erforderliche Zugriffskonfigurationen und native Clients zu `az ad app create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-766">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="4adad-767">`rbac`-Befehle geändert, um maximal 1.000 IDs für Objektauflösung zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="4adad-767">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="4adad-768">Befehle zur Verwaltung von Anmeldeinformationen (`ad sp credential [reset|list|delete]`) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-768">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="4adad-769">[WICHTIGE ÄNDERUNG] „properties“ aus `az role assignment [list|show]`-Ausgabe entfernt</span><span class="sxs-lookup"><span data-stu-id="4adad-769">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="4adad-770">Unterstützung für `dataActions`- und `notDataActions`-Berechtigungen zu `role definition` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-770">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="4adad-771">Speicher</span><span class="sxs-lookup"><span data-stu-id="4adad-771">Storage</span></span>

* <span data-ttu-id="4adad-772">Problem beim Hochladen von Dateien mit einer Größe von 195 GB bis 200 GB behoben</span><span class="sxs-lookup"><span data-stu-id="4adad-772">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="4adad-773">[#4049](https://github.com/Azure/azure-cli/issues/4049) behoben: Probleme bei Uploads von Anfügeblobs behoben, die ein Ignorieren der Bedingungsparameter verursachten</span><span class="sxs-lookup"><span data-stu-id="4adad-773">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="4adad-774">VM</span><span class="sxs-lookup"><span data-stu-id="4adad-774">VM</span></span>

* <span data-ttu-id="4adad-775">Warnung für anstehende wichtige Änderungen für Sätze mit mehr als 100 Instanzen zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-775">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="4adad-776">Unterstützung der Zonenresilienz zu `vm [snapshot|image]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-776">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="4adad-777">Datenträgerinstanzansicht geändert, um besseren Verschlüsselungsstatus zu melden</span><span class="sxs-lookup"><span data-stu-id="4adad-777">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="4adad-778">[WICHTIGE ÄNDERUNG] `vm extension delete` geändert, um keine Ausgabe mehr zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="4adad-778">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="4adad-779">13. März 2018</span><span class="sxs-lookup"><span data-stu-id="4adad-779">March 13, 2018</span></span>

<span data-ttu-id="4adad-780">Version 2.0.29</span><span class="sxs-lookup"><span data-stu-id="4adad-780">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="4adad-781">ACR</span><span class="sxs-lookup"><span data-stu-id="4adad-781">ACR</span></span>

* <span data-ttu-id="4adad-782">Unterstützung für den Parameter `--image` zu `repository delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-782">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="4adad-783">Parameter `--manifest` und `--tag` des Befehls `repository delete` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="4adad-783">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="4adad-784">Befehl `repository untag` zum Entfernen eines Tags ohne das Löschen von Daten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-784">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="4adad-785">ACS</span><span class="sxs-lookup"><span data-stu-id="4adad-785">ACS</span></span>

* <span data-ttu-id="4adad-786">Befehl `aks upgrade-connector` zum Aktualisieren eines vorhandenen Connectors hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-786">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="4adad-787">`kubectl`-Konfigurationsdateien zur Verwendung von besser lesbarem YAML im Blockstil geändert</span><span class="sxs-lookup"><span data-stu-id="4adad-787">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="4adad-788">Advisor</span><span class="sxs-lookup"><span data-stu-id="4adad-788">Advisor</span></span>

* <span data-ttu-id="4adad-789">[WICHTIGE ÄNDERUNG] `advisor configuration get` in `advisor configuration list` umbenannt</span><span class="sxs-lookup"><span data-stu-id="4adad-789">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="4adad-790">[WICHTIGE ÄNDERUNG] `advisor configuration set` in `advisor configuration update` umbenannt</span><span class="sxs-lookup"><span data-stu-id="4adad-790">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="4adad-791">[WICHTIGE ÄNDERUNG] `advisor recommendation generate` entfernt</span><span class="sxs-lookup"><span data-stu-id="4adad-791">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="4adad-792">Parameter `--refresh` zu `advisor recommendation list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-792">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="4adad-793">Befehl `advisor recommendation show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-793">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="4adad-794">AppService</span><span class="sxs-lookup"><span data-stu-id="4adad-794">Appservice</span></span>

* <span data-ttu-id="4adad-795">`[webapp|functionapp] assign-identity` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="4adad-795">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="4adad-796">Befehle `webapp identity [assign|show]` und `functionapp identity [assign|show]` für verwaltete Identität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-796">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="4adad-797">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="4adad-797">Eventhubs</span></span>

* <span data-ttu-id="4adad-798">Erste Version</span><span class="sxs-lookup"><span data-stu-id="4adad-798">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="4adad-799">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="4adad-799">Extension</span></span>

* <span data-ttu-id="4adad-800">Überprüfung zum Warnen von Benutzern hinzugefügt, wenn sich die verwendete Distribution von der in der Paketquelldatei gespeicherten Distribution unterscheidet, da dies Fehlern führen kann</span><span class="sxs-lookup"><span data-stu-id="4adad-800">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="4adad-801">Interactive</span><span class="sxs-lookup"><span data-stu-id="4adad-801">Interactive</span></span>

* <span data-ttu-id="4adad-802">[#5625](https://github.com/Azure/azure-cli/issues/5625) behoben: Verlauf über verschiedene Sitzungen hinweg beibehalten</span><span class="sxs-lookup"><span data-stu-id="4adad-802">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="4adad-803">[#3016](https://github.com/Azure/azure-cli/issues/3016) behoben: Verlauf nicht aufgezeichnet, obwohl er innerhalb des Bereichs liegt</span><span class="sxs-lookup"><span data-stu-id="4adad-803">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="4adad-804">[#5688](https://github.com/Azure/azure-cli/issues/5688) behoben: Abschlüsse nicht angezeigt, wenn beim Laden der Befehlstabelle Ausnahme auftrat</span><span class="sxs-lookup"><span data-stu-id="4adad-804">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="4adad-805">Statusanzeige für lang ausgeführte Vorgänge korrigiert</span><span class="sxs-lookup"><span data-stu-id="4adad-805">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="4adad-806">Überwachen</span><span class="sxs-lookup"><span data-stu-id="4adad-806">Monitor</span></span>

* <span data-ttu-id="4adad-807">`monitor autoscale-settings`-Befehle als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="4adad-807">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="4adad-808">Befehle vom Typ `monitor autoscale` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-808">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="4adad-809">Befehle vom Typ `monitor autoscale profile` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-809">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="4adad-810">Befehle vom Typ `monitor autoscale rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-810">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="4adad-811">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="4adad-811">Network</span></span>

* <span data-ttu-id="4adad-812">[WICHTIGE ÄNDERUNG] Parameter `--tags` aus `route-filter rule create` entfernt</span><span class="sxs-lookup"><span data-stu-id="4adad-812">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="4adad-813">Einige fehlerhafte Standardwerte für die folgenden Befehle entfernt:</span><span class="sxs-lookup"><span data-stu-id="4adad-813">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="4adad-814">`network watcher connection-monitor`-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-814">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="4adad-815">Parameter `--vnet` und `--subnet` zu `network watcher show-topology` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-815">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="4adad-816">Profil</span><span class="sxs-lookup"><span data-stu-id="4adad-816">Profile</span></span>

* <span data-ttu-id="4adad-817">Parameter `--msi` für `az login` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="4adad-817">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="4adad-818">Parameter `--identity` für `az login` als Ersatz vor `--msi` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-818">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="4adad-819">RDBMS</span><span class="sxs-lookup"><span data-stu-id="4adad-819">RDBMS</span></span>

* <span data-ttu-id="4adad-820">[VORSCHAU] Geändert, sodass die API „2017-12-01-preview“ verwendet wird</span><span class="sxs-lookup"><span data-stu-id="4adad-820">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="4adad-821">Service Bus</span><span class="sxs-lookup"><span data-stu-id="4adad-821">Service Bus</span></span>

* <span data-ttu-id="4adad-822">Erste Version</span><span class="sxs-lookup"><span data-stu-id="4adad-822">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="4adad-823">Speicher</span><span class="sxs-lookup"><span data-stu-id="4adad-823">Storage</span></span>

* <span data-ttu-id="4adad-824">[#4971](https://github.com/Azure/azure-cli/issues/4971) behoben: `storage blob copy` unterstützt jetzt andere Azure-Clouds.</span><span class="sxs-lookup"><span data-stu-id="4adad-824">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="4adad-825">[#5286](https://github.com/Azure/azure-cli/issues/5286) behoben: `storage blob [delete-batch|download-batch|upload-batch]`-Batchbefehle lösen bei Vorbedingungsfehlern keinen Fehler mehr aus.</span><span class="sxs-lookup"><span data-stu-id="4adad-825">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="4adad-826">VM</span><span class="sxs-lookup"><span data-stu-id="4adad-826">VM</span></span>

* <span data-ttu-id="4adad-827">`[vm|vmss] create` unterstützt jetzt das Anfügen nicht verwalteter Datenträger und das Konfigurieren der Zwischenspeicherung.</span><span class="sxs-lookup"><span data-stu-id="4adad-827">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="4adad-828">`[vm|vmss] assign-identity` und `[vm|vmss] remove-identity` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="4adad-828">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="4adad-829">Befehle `vm identity [assign|remove|show]` und `vmss identity [assign|remove|show]` als Ersatz für veraltete Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-829">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="4adad-830">Standardpriorität in `vmss create` auf „Keine“ geändert</span><span class="sxs-lookup"><span data-stu-id="4adad-830">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="4adad-831">27. Februar 2018</span><span class="sxs-lookup"><span data-stu-id="4adad-831">February 27, 2018</span></span>

<span data-ttu-id="4adad-832">Version 2.0.28</span><span class="sxs-lookup"><span data-stu-id="4adad-832">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="4adad-833">Core</span><span class="sxs-lookup"><span data-stu-id="4adad-833">Core</span></span>

* <span data-ttu-id="4adad-834">[5184](https://github.com/Azure/azure-cli/issues/5184) (Problem beim Installieren von Homebrew) behoben</span><span class="sxs-lookup"><span data-stu-id="4adad-834">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="4adad-835">Unterstützung für Erweiterungstelemetrie mit benutzerdefinierten Schlüsseln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-835">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="4adad-836">HTTP-Protokollierung zu `--debug` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-836">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="4adad-837">ACS</span><span class="sxs-lookup"><span data-stu-id="4adad-837">ACS</span></span>

* <span data-ttu-id="4adad-838">Geändert, sodass für `aks install-connector` standardmäßig das Helm-Diagramm `virtual-kubelet-for-aks` verwendet wird</span><span class="sxs-lookup"><span data-stu-id="4adad-838">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="4adad-839">Problem behoben: Unzureichende Berechtigungen für Dienstprinzipale zum Erstellen einer ACI-Containergruppe</span><span class="sxs-lookup"><span data-stu-id="4adad-839">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="4adad-840">Parameter `--aci-container-group`, `--location` und `--image-tag` zu `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-840">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="4adad-841">Veraltungshinweis aus `aks get-versions` entfernt</span><span class="sxs-lookup"><span data-stu-id="4adad-841">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="4adad-842">AppService</span><span class="sxs-lookup"><span data-stu-id="4adad-842">Appservice</span></span>

* <span data-ttu-id="4adad-843">Updates für die neue SDK-Version (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="4adad-843">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="4adad-844">[5538](https://github.com/Azure/azure-cli/issues/5538) behoben: `Free` wurde als ungültige SKU gemeldet.</span><span class="sxs-lookup"><span data-stu-id="4adad-844">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="4adad-845">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="4adad-845">Cognitive Services</span></span>

* <span data-ttu-id="4adad-846">Hinweis beim Erstellen eines neuen Cognitive Services-Kontos aktualisiert</span><span class="sxs-lookup"><span data-stu-id="4adad-846">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="4adad-847">Nutzung</span><span class="sxs-lookup"><span data-stu-id="4adad-847">Consumption</span></span>

* <span data-ttu-id="4adad-848">Neue Befehle für PriceSheet-API hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-848">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="4adad-849">Vorhandene Formate für Nutzungsdetails und Reservierungsdetails aktualisiert</span><span class="sxs-lookup"><span data-stu-id="4adad-849">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="4adad-850">Container</span><span class="sxs-lookup"><span data-stu-id="4adad-850">Container</span></span>

* <span data-ttu-id="4adad-851">Argumente `--secrets` und `--secrets-mount-path` zu `container create` hinzugefügt, um Geheimnisse in ACI verwenden zu können</span><span class="sxs-lookup"><span data-stu-id="4adad-851">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="4adad-852">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="4adad-852">Network</span></span>

* <span data-ttu-id="4adad-853">[5559](https://github.com/Azure/azure-cli/issues/5559) behoben: Fehlender Client in `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="4adad-853">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="4adad-854">Ressource</span><span class="sxs-lookup"><span data-stu-id="4adad-854">Resource</span></span>

* <span data-ttu-id="4adad-855">`group deployment export` geändert, um eine partielle Vorlage und ggf. Fehler anzuzeigen, wenn der Vorgang nicht erfolgreich war</span><span class="sxs-lookup"><span data-stu-id="4adad-855">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="4adad-856">Rolle</span><span class="sxs-lookup"><span data-stu-id="4adad-856">Role</span></span>

* <span data-ttu-id="4adad-857">`role assignment list-changelogs` hinzugefügt, um die Überprüfung von Dienstprinzipalrollen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="4adad-857">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="4adad-858">SQL</span><span class="sxs-lookup"><span data-stu-id="4adad-858">SQL</span></span>

* <span data-ttu-id="4adad-859">Zonenredundanzunterstützung für Datenbanken und Pools für elastische Datenbanken hinzugefügt (bei Erstellung und Aktualisierung)</span><span class="sxs-lookup"><span data-stu-id="4adad-859">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="4adad-860">Speicher</span><span class="sxs-lookup"><span data-stu-id="4adad-860">Storage</span></span>

* <span data-ttu-id="4adad-861">Angabe von Zielpfad/Präfix für `storage blob [upload-batch|download-batch]` ermöglicht</span><span class="sxs-lookup"><span data-stu-id="4adad-861">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="4adad-862">VM</span><span class="sxs-lookup"><span data-stu-id="4adad-862">VM</span></span>

* <span data-ttu-id="4adad-863">Unterstützung für das Anfügen/Trennen von Datenträgern für eine einzelne VMSS-Instanz hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-863">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="4adad-864">13. Februar 2018</span><span class="sxs-lookup"><span data-stu-id="4adad-864">February 13, 2018</span></span>

<span data-ttu-id="4adad-865">Version 2.0.27</span><span class="sxs-lookup"><span data-stu-id="4adad-865">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="4adad-866">Core</span><span class="sxs-lookup"><span data-stu-id="4adad-866">Core</span></span>

* <span data-ttu-id="4adad-867">Authentifizierung für Abonnement-ID und Namen bei der MSI-Anmeldung in Authentifizierung mit Schlüssel geändert</span><span class="sxs-lookup"><span data-stu-id="4adad-867">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="4adad-868">ACS</span><span class="sxs-lookup"><span data-stu-id="4adad-868">ACS</span></span>

* <span data-ttu-id="4adad-869">[WICHTIGE ÄNDERUNG] `aks get-versions` aus Gründen der Genauigkeit in `aks get-upgrades` umbenannt</span><span class="sxs-lookup"><span data-stu-id="4adad-869">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="4adad-870">`aks get-versions` zur Anzeige der verfügbaren Kubernetes-Versionen für `aks create` geändert</span><span class="sxs-lookup"><span data-stu-id="4adad-870">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="4adad-871">Standardwerte von `aks create` in Auswahl der Kubernetes-Version durch den Server geändert</span><span class="sxs-lookup"><span data-stu-id="4adad-871">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="4adad-872">Hilfemeldungen zu dem von AKS generierten Dienstprinzipal aktualisiert</span><span class="sxs-lookup"><span data-stu-id="4adad-872">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="4adad-873">Standardknotengrößen für `aks create` von „Standard\_D1\_v2“ in „Standard\_DS1\_v2“ geändert</span><span class="sxs-lookup"><span data-stu-id="4adad-873">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="4adad-874">Zuverlässigkeit der Suche nach dem Dashboardpod für `az aks browse` verbessert</span><span class="sxs-lookup"><span data-stu-id="4adad-874">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="4adad-875">`aks get-credentials` korrigiert, um Unicode-Fehler beim Laden von Kubernetes-Konfigurationsdateien zu behandeln</span><span class="sxs-lookup"><span data-stu-id="4adad-875">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="4adad-876">Meldung zu `az aks install-cli` hinzugefügt, um das Abrufen von `kubectl` in `$PATH` zu erleichtern</span><span class="sxs-lookup"><span data-stu-id="4adad-876">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="4adad-877">AppService</span><span class="sxs-lookup"><span data-stu-id="4adad-877">Appservice</span></span>

* <span data-ttu-id="4adad-878">Problem behoben, das zu einem Fehler von `webapp [backup|restore]` aufgrund eines Nullverweises führte</span><span class="sxs-lookup"><span data-stu-id="4adad-878">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="4adad-879">Unterstützung für Standard-App Service-Pläne durch `az configure --defaults appserviceplan=my-asp` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-879">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="4adad-880">CDN</span><span class="sxs-lookup"><span data-stu-id="4adad-880">CDN</span></span>

* <span data-ttu-id="4adad-881">Befehle vom Typ `cdn custom-domain [enable-https|disable-https]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-881">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="4adad-882">Container</span><span class="sxs-lookup"><span data-stu-id="4adad-882">Container</span></span>

* <span data-ttu-id="4adad-883">Option `--follow` zu `az container logs` für Streamingprotokolle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-883">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="4adad-884">Befehl `container attach` hinzugefügt, der die lokale Standardausgabe und Fehlerdatenströme an einen Container in einer Containergruppe angefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-884">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="4adad-885">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="4adad-885">CosmosDB</span></span>

* <span data-ttu-id="4adad-886">Unterstützung für Einstellungsfunktionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-886">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="4adad-887">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="4adad-887">Extension</span></span>

* <span data-ttu-id="4adad-888">Unterstützung für den Parameter `--pip-proxy` zu Befehlen vom Typ `az extension [add|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-888">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="4adad-889">Unterstützung für das Argument `--pip-extra-index-urls` zu Befehlen vom Typ `az extension [add|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-889">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="4adad-890">Feedback</span><span class="sxs-lookup"><span data-stu-id="4adad-890">Feedback</span></span>

* <span data-ttu-id="4adad-891">Erweiterungsinformationen zu Telemetriedaten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-891">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="4adad-892">Interactive</span><span class="sxs-lookup"><span data-stu-id="4adad-892">Interactive</span></span>

* <span data-ttu-id="4adad-893">Problem behoben, aufgrund dessen der Benutzer bei Verwendung des interaktiven Modus in Cloud Shell zur Anmeldung aufgefordert wird</span><span class="sxs-lookup"><span data-stu-id="4adad-893">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="4adad-894">Regression mit fehlenden Parametervervollständigungen korrigiert</span><span class="sxs-lookup"><span data-stu-id="4adad-894">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="4adad-895">IoT</span><span class="sxs-lookup"><span data-stu-id="4adad-895">IoT</span></span>

* <span data-ttu-id="4adad-896">Problem behoben, aufgrund dessen `iot dps access policy [create|update]` bei erfolgreicher Ausführung einen Fehler „nicht gefunden“ zurückgibt</span><span class="sxs-lookup"><span data-stu-id="4adad-896">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="4adad-897">Problem behoben, aufgrund dessen `iot dps linked-hub [create|update]` bei erfolgreicher Ausführung einen Fehler „nicht gefunden“ zurückgibt</span><span class="sxs-lookup"><span data-stu-id="4adad-897">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="4adad-898">Unterstützung für `--no-wait` zu `iot dps access policy [create|update]` und `iot dps linked-hub [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-898">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="4adad-899">`iot hub create` geändert, um die Angabe der Anzahl von Partitionen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="4adad-899">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="4adad-900">Überwachen</span><span class="sxs-lookup"><span data-stu-id="4adad-900">Monitor</span></span>

* <span data-ttu-id="4adad-901">Befehl `az monitor log-profiles create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="4adad-901">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="4adad-902">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="4adad-902">Network</span></span>

* <span data-ttu-id="4adad-903">Option `--tags` für folgende Befehle korrigiert:</span><span class="sxs-lookup"><span data-stu-id="4adad-903">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="4adad-904">Profil</span><span class="sxs-lookup"><span data-stu-id="4adad-904">Profile</span></span>

* <span data-ttu-id="4adad-905">`az login` im interaktiven Modus aktiviert</span><span class="sxs-lookup"><span data-stu-id="4adad-905">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="4adad-906">Ressource</span><span class="sxs-lookup"><span data-stu-id="4adad-906">Resource</span></span>

* <span data-ttu-id="4adad-907">`feature show` wieder hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-907">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="4adad-908">Rolle</span><span class="sxs-lookup"><span data-stu-id="4adad-908">Role</span></span>

* <span data-ttu-id="4adad-909">Argument `--available-to-other-tenants` zu `ad app update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-909">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="4adad-910">SQL</span><span class="sxs-lookup"><span data-stu-id="4adad-910">SQL</span></span>

* <span data-ttu-id="4adad-911">Befehle vom Typ `sql server dns-alias` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-911">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="4adad-912">`sql db rename` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-912">Added `sql db rename`</span></span>
* <span data-ttu-id="4adad-913">Unterstützung für das Argument `--ids` für alle SQL-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-913">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="4adad-914">Speicher</span><span class="sxs-lookup"><span data-stu-id="4adad-914">Storage</span></span>

* <span data-ttu-id="4adad-915">Befehle `storage blob service-properties delete-policy` und `storage blob undelete` hinzugefügt, um vorläufiges Löschen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="4adad-915">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="4adad-916">VM</span><span class="sxs-lookup"><span data-stu-id="4adad-916">VM</span></span>

* <span data-ttu-id="4adad-917">Absturz bei unvollständiger Initialisierung der VM-Verschlüsselung behoben</span><span class="sxs-lookup"><span data-stu-id="4adad-917">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="4adad-918">Prinzipal-ID-Ausgabe beim Aktivieren von MSI hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-918">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="4adad-919">`vm boot-diagnostics get-boot-log` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="4adad-919">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="4adad-920">31. Januar 2018</span><span class="sxs-lookup"><span data-stu-id="4adad-920">January 31, 2018</span></span>

<span data-ttu-id="4adad-921">Version 2.0.26</span><span class="sxs-lookup"><span data-stu-id="4adad-921">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="4adad-922">Core</span><span class="sxs-lookup"><span data-stu-id="4adad-922">Core</span></span>

* <span data-ttu-id="4adad-923">Unterstützung für das Abrufen von unformatierten Token im MSI-Kontext hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-923">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="4adad-924">Abrufindikator-Zeichenfolge nach Fertigstellung von LRO für die Windows-Datei „cmd.exe“ entfernt</span><span class="sxs-lookup"><span data-stu-id="4adad-924">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="4adad-925">Warnung hinzugefügt, die angezeigt wird, wenn ein konfigurierter Standardwert in einen Eintrag auf INFO-Ebene geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="4adad-925">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="4adad-926">`--verbose` zum Anzeigen verwenden.</span><span class="sxs-lookup"><span data-stu-id="4adad-926">Use `--verbose` to see</span></span>
* <span data-ttu-id="4adad-927">Statusanzeige für Wait-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-927">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="4adad-928">ACS</span><span class="sxs-lookup"><span data-stu-id="4adad-928">ACS</span></span>

* <span data-ttu-id="4adad-929">Argument `--disable-browser` erläutert</span><span class="sxs-lookup"><span data-stu-id="4adad-929">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="4adad-930">Vervollständigung mit der TAB-TASTE für Argumente vom Typ `--vm-size` verbessert</span><span class="sxs-lookup"><span data-stu-id="4adad-930">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="4adad-931">AppService</span><span class="sxs-lookup"><span data-stu-id="4adad-931">Appservice</span></span>

* <span data-ttu-id="4adad-932">`webapp log [tail|download]` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="4adad-932">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="4adad-933">Überprüfung `kind` für Web-Apps und Funktionen entfernt</span><span class="sxs-lookup"><span data-stu-id="4adad-933">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="4adad-934">CDN</span><span class="sxs-lookup"><span data-stu-id="4adad-934">CDN</span></span>

* <span data-ttu-id="4adad-935">Problem mit fehlendem Client für `cdn custom-domain create` behoben</span><span class="sxs-lookup"><span data-stu-id="4adad-935">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="4adad-936">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="4adad-936">CosmosDB</span></span>

* <span data-ttu-id="4adad-937">Parameterbeschreibung für Failoverrichtlinien korrigiert</span><span class="sxs-lookup"><span data-stu-id="4adad-937">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="4adad-938">Interactive</span><span class="sxs-lookup"><span data-stu-id="4adad-938">Interactive</span></span>

* <span data-ttu-id="4adad-939">Problem behoben, aufgrund dessen Vervollständigungen von Befehlsoptionen nicht mehr angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="4adad-939">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="4adad-940">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="4adad-940">Network</span></span>

* <span data-ttu-id="4adad-941">Schutz für `--cert-password` zu `application-gateway create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-941">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="4adad-942">Problem mit `application-gateway update` behoben, aufgrund dessen `--sku` fälschlicherweise einen Standardwert anwendete</span><span class="sxs-lookup"><span data-stu-id="4adad-942">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="4adad-943">Schutz für `--shared-key` und `--authorization-key` zu `vpn-connection create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-943">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="4adad-944">Problem mit fehlendem Client für `asg create` behoben</span><span class="sxs-lookup"><span data-stu-id="4adad-944">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="4adad-945">Parameter `--file-name / -f` für exportierte Namen zu `dns zone export` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-945">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="4adad-946">Folgende Probleme mit `dns zone export` behoben:</span><span class="sxs-lookup"><span data-stu-id="4adad-946">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="4adad-947">Problem behoben, aufgrund dessen lange TXT-Einträge nicht korrekt exportiert wurden</span><span class="sxs-lookup"><span data-stu-id="4adad-947">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="4adad-948">Problem behoben, aufgrund dessen TXT-Einträge in Anführungszeichen fälschlich ohne Anführungszeichen in Escapezeichen exportiert wurden</span><span class="sxs-lookup"><span data-stu-id="4adad-948">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="4adad-949">Problem behoben, aufgrund dessen bestimmte Datensätze zweimal mit `dns zone import` importiert wurden</span><span class="sxs-lookup"><span data-stu-id="4adad-949">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="4adad-950">Befehle `vnet-gateway root-cert` und `vnet-gateway revoked-cert` wiederhergestellt</span><span class="sxs-lookup"><span data-stu-id="4adad-950">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="4adad-951">Profil</span><span class="sxs-lookup"><span data-stu-id="4adad-951">Profile</span></span>

* <span data-ttu-id="4adad-952">`get-access-token` zur Verwendung auf einer VM mit Identität korrigiert</span><span class="sxs-lookup"><span data-stu-id="4adad-952">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="4adad-953">Ressource</span><span class="sxs-lookup"><span data-stu-id="4adad-953">Resource</span></span>

* <span data-ttu-id="4adad-954">Fehler mit `deployment [create|validate]` korrigiert, aufgrund dessen fälschlich eine Warnung angezeigt wurde, wenn ein Vorlagenfeld „Typ“ Werte in Großbuchstaben enthielt</span><span class="sxs-lookup"><span data-stu-id="4adad-954">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="4adad-955">Speicher</span><span class="sxs-lookup"><span data-stu-id="4adad-955">Storage</span></span>

* <span data-ttu-id="4adad-956">Problem mit der Migration von Storage V1-Konten zu Storage V2 behoben</span><span class="sxs-lookup"><span data-stu-id="4adad-956">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="4adad-957">Statusberichterstellung für alle Upload-/Downloadbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-957">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="4adad-958">Fehler korrigiert, der die Verwendung der arg-Option „-n“ mit `storage account check-name` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="4adad-958">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="4adad-959">Spalte „Momentaufnahme“ zur Tabellenausgabe für `blob [list|show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-959">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="4adad-960">Fehler mit verschiedenen Parametern korrigiert, die als Int-Typen analysiert werden mussten</span><span class="sxs-lookup"><span data-stu-id="4adad-960">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="4adad-961">VM</span><span class="sxs-lookup"><span data-stu-id="4adad-961">VM</span></span>

* <span data-ttu-id="4adad-962">Befehl `vm image accept-terms` hinzugefügt, um die Erstellung von VMs aus Images mit zusätzlichen Gebühren zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="4adad-962">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="4adad-963">`[vm|vmss create]` korrigiert, um sicherzustellen, dass Befehle unter einem Proxy mit nicht signierten Zertifikaten ausgeführt werden können</span><span class="sxs-lookup"><span data-stu-id="4adad-963">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="4adad-964">[VORSCHAU] Unterstützung für „niedrige“ Priorität zu VMSS hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-964">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="4adad-965">Schutz für `--admin-password` zu `[vm|vmss] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-965">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="4adad-966">17. Januar 2018</span><span class="sxs-lookup"><span data-stu-id="4adad-966">January 17, 2018</span></span>

<span data-ttu-id="4adad-967">Version 2.0.25</span><span class="sxs-lookup"><span data-stu-id="4adad-967">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="4adad-968">ACR</span><span class="sxs-lookup"><span data-stu-id="4adad-968">ACR</span></span>

* <span data-ttu-id="4adad-969">Fallback auf ACR-Anmeldung bei Fehlern mit Windows-Anmeldeinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-969">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="4adad-970">Registrierungsprotokolle aktiviert</span><span class="sxs-lookup"><span data-stu-id="4adad-970">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="4adad-971">ACS</span><span class="sxs-lookup"><span data-stu-id="4adad-971">ACS</span></span>

* <span data-ttu-id="4adad-972">Befehl `get-credentials` korrigiert</span><span class="sxs-lookup"><span data-stu-id="4adad-972">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="4adad-973">SPN-Rollenanforderung entfernt</span><span class="sxs-lookup"><span data-stu-id="4adad-973">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="4adad-974">AppService</span><span class="sxs-lookup"><span data-stu-id="4adad-974">Appservice</span></span>

* <span data-ttu-id="4adad-975">Fehler mit `config ssl upload` behoben, bei dem `hosting_environment_profile` NULL war</span><span class="sxs-lookup"><span data-stu-id="4adad-975">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="4adad-976">Unterstützung benutzerdefinierter URLs zu `browse` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-976">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="4adad-977">Slotunterstützung für `log tail` korrigiert</span><span class="sxs-lookup"><span data-stu-id="4adad-977">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="4adad-978">Backup</span><span class="sxs-lookup"><span data-stu-id="4adad-978">Backup</span></span>

* <span data-ttu-id="4adad-979">Option `--container-name` von `backup item list` geändert (ist jetzt optional)</span><span class="sxs-lookup"><span data-stu-id="4adad-979">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="4adad-980">Speicherkontooptionen zu `backup restore restore-disks` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-980">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="4adad-981">Standortüberprüfung in `backup protection enable-for-vm` korrigiert (Groß-/Kleinschreibung wird jetzt nicht mehr beachtet)</span><span class="sxs-lookup"><span data-stu-id="4adad-981">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="4adad-982">Problem behoben, durch das bei Befehlen mit ungültigem Containernamen ein Fehler auftrat</span><span class="sxs-lookup"><span data-stu-id="4adad-982">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="4adad-983">`backup item list` geändert (Integritätsstatus jetzt standardmäßig enthalten)</span><span class="sxs-lookup"><span data-stu-id="4adad-983">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="4adad-984">Batch</span><span class="sxs-lookup"><span data-stu-id="4adad-984">Batch</span></span>

* <span data-ttu-id="4adad-985">`batch login` geändert, um Authentifizierungsdetails zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="4adad-985">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="4adad-986">Cloud</span><span class="sxs-lookup"><span data-stu-id="4adad-986">Cloud</span></span>

* <span data-ttu-id="4adad-987">Beim Festlegen von `--profile` für eine Cloud werden nun keine Endpunkte mehr benötigt.</span><span class="sxs-lookup"><span data-stu-id="4adad-987">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="4adad-988">Nutzung</span><span class="sxs-lookup"><span data-stu-id="4adad-988">Consumption</span></span>

* <span data-ttu-id="4adad-989">Neue Befehle für Reservierungen hinzugefügt: `consumption reservations summaries` und `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="4adad-989">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="4adad-990">Event Grid</span><span class="sxs-lookup"><span data-stu-id="4adad-990">Event Grid</span></span>

* <span data-ttu-id="4adad-991">[WICHTIGE ÄNDERUNG] Die Befehle vom Typ `az eventgrid topic event-subscription` wurden in `eventgrid event-subscription` verschoben.</span><span class="sxs-lookup"><span data-stu-id="4adad-991">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="4adad-992">[WICHTIGE ÄNDERUNG] Die Befehle vom Typ `az eventgrid resource event-subscription` wurden in `eventgrid event-subscription` verschoben.</span><span class="sxs-lookup"><span data-stu-id="4adad-992">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="4adad-993">[WICHTIGE ÄNDERUNG] Der Befehl `eventgrid event-subscription show-endpoint-url` wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="4adad-993">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="4adad-994">Verwenden Sie stattdessen `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="4adad-994">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="4adad-995">Befehl `eventgrid topic update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-995">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="4adad-996">Befehl `eventgrid event-subscription update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-996">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="4adad-997">Parameter `--ids` für Befehle vom Typ `eventgrid topic` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-997">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="4adad-998">Unterstützung der Vervollständigung mit der TAB-TASTE für Themennamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-998">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="4adad-999">Interactive</span><span class="sxs-lookup"><span data-stu-id="4adad-999">Interactive</span></span>

* <span data-ttu-id="4adad-1000">Problem behoben, das dazu führte, dass der interaktive Modus nicht mit Python 2.x verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="4adad-1000">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="4adad-1001">Fehler beim Start behoben</span><span class="sxs-lookup"><span data-stu-id="4adad-1001">Fixed errors on startup</span></span>
* <span data-ttu-id="4adad-1002">Problem behoben, das dazu führte, dass einige Befehle nicht im interaktiven Modus ausgeführt werden konnten</span><span class="sxs-lookup"><span data-stu-id="4adad-1002">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="4adad-1003">IoT</span><span class="sxs-lookup"><span data-stu-id="4adad-1003">IoT</span></span>

* <span data-ttu-id="4adad-1004">Unterstützung für Gerätebereitstellungsdienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1004">Added support for device provisioning service</span></span>
* <span data-ttu-id="4adad-1005">Benachrichtigungen zu veralteten Elementen in Befehlen und in der Befehlshilfe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1005">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="4adad-1006">IoT-Überprüfung hinzugefügt, um Benutzer über die IoT-Erweiterung zu informieren</span><span class="sxs-lookup"><span data-stu-id="4adad-1006">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="4adad-1007">Überwachen</span><span class="sxs-lookup"><span data-stu-id="4adad-1007">Monitor</span></span>

* <span data-ttu-id="4adad-1008">Unterstützung mehrerer Diagnoseeinstellung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="4adad-1008">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="4adad-1009">Der Parameter `--name` ist nun für `az monitor diagnostic-settings create` erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4adad-1009">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="4adad-1010">Befehl `monitor diagnostic-settings categories` zum Abrufen der Diagnoseeinstellungskategorie hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1010">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="4adad-1011">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="4adad-1011">Network</span></span>

* <span data-ttu-id="4adad-1012">Problem behoben, das beim Ändern des aktiven Standbymodus mit `vnet-gateway update` auftrat</span><span class="sxs-lookup"><span data-stu-id="4adad-1012">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="4adad-1013">Unterstützung für HTTP2 zu `application-gateway [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1013">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="4adad-1014">Profil</span><span class="sxs-lookup"><span data-stu-id="4adad-1014">Profile</span></span>

* <span data-ttu-id="4adad-1015">Unterstützung für die Anmeldung mit durch Benutzer zugewiesenen Identitäten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1015">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="4adad-1016">Rolle</span><span class="sxs-lookup"><span data-stu-id="4adad-1016">Role</span></span>

* <span data-ttu-id="4adad-1017">Argument `--assignee-object-id` zu `role assignment create` hinzugefügt, um Graph-Abfrage zu umgehen</span><span class="sxs-lookup"><span data-stu-id="4adad-1017">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="4adad-1018">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="4adad-1018">Service Fabric</span></span>

* <span data-ttu-id="4adad-1019">Ausführliche Fehler zur Überprüfungsantwort bei der Clustererstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1019">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="4adad-1020">Problem mit fehlendem Client für verschiedene Befehle behoben</span><span class="sxs-lookup"><span data-stu-id="4adad-1020">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="4adad-1021">VM</span><span class="sxs-lookup"><span data-stu-id="4adad-1021">VM</span></span>

* <span data-ttu-id="4adad-1022">[VORSCHAUVERSION] Zonenübergreifende Unterstützung für `vmss`</span><span class="sxs-lookup"><span data-stu-id="4adad-1022">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="4adad-1023">[WICHTIGE ÄNDERUNG] Standard für Einzelzone (`vmss`) in Standardlastenausgleich geändert</span><span class="sxs-lookup"><span data-stu-id="4adad-1023">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="4adad-1024">[WICHTIGE ÄNDERUNG] `externalIdentities` in `userAssignedIdentities` geändert für EMSI</span><span class="sxs-lookup"><span data-stu-id="4adad-1024">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="4adad-1025">[VORSCHAUVERSION] Unterstützung für Austausch des Betriebssystemdatenträgers hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1025">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="4adad-1026">Unterstützung der Verwendung von VM-Images aus anderen Abonnements hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1026">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="4adad-1027">Argumente `--plan-name`, `--plan-product`, `--plan-promotion-code` und `--plan-publisher` zu `[vm|vmss] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1027">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="4adad-1028">Fehlerbedingte Probleme mit `[vm|vmss] create` behoben</span><span class="sxs-lookup"><span data-stu-id="4adad-1028">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="4adad-1029">Übermäßige Ressourcenverwendung durch `vm image list --all` behoben</span><span class="sxs-lookup"><span data-stu-id="4adad-1029">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="4adad-1030">19. Dezember 2017</span><span class="sxs-lookup"><span data-stu-id="4adad-1030">December 19, 2017</span></span>

<span data-ttu-id="4adad-1031">Version 2.0.23</span><span class="sxs-lookup"><span data-stu-id="4adad-1031">Version 2.0.23</span></span>

* <span data-ttu-id="4adad-1032">Unterstützung für die Anmeldung mit durch Benutzer zugewiesenen Identitäten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1032">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="4adad-1033">Container</span><span class="sxs-lookup"><span data-stu-id="4adad-1033">Container</span></span>

* <span data-ttu-id="4adad-1034">Falsche Reihenfolge der Parameter für Containerprotokolle behoben</span><span class="sxs-lookup"><span data-stu-id="4adad-1034">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="4adad-1035">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="4adad-1035">Network</span></span>

* <span data-ttu-id="4adad-1036">Argument `--disable-bgp-route-propagation` zu `route-table [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1036">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="4adad-1037">Argument `--ip-tags` zu `public-ip [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1037">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="4adad-1038">Speicher</span><span class="sxs-lookup"><span data-stu-id="4adad-1038">Storage</span></span>

* <span data-ttu-id="4adad-1039">Unterstützung für Storage V2 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1039">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="4adad-1040">VM</span><span class="sxs-lookup"><span data-stu-id="4adad-1040">VM</span></span>

* <span data-ttu-id="4adad-1041">[VORSCHAUVERSION] Unterstützung für durch Benutzer zugewiesene Identitäten für virtuelle Computer und VMSSs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1041">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="4adad-1042">5. Dezember 2017</span><span class="sxs-lookup"><span data-stu-id="4adad-1042">December 5, 2017</span></span>

<span data-ttu-id="4adad-1043">Version 2.0.22</span><span class="sxs-lookup"><span data-stu-id="4adad-1043">Version 2.0.22</span></span>

* <span data-ttu-id="4adad-1044">`az component`-Befehle wurden entfernt.</span><span class="sxs-lookup"><span data-stu-id="4adad-1044">Removed `az component` commands.</span></span> <span data-ttu-id="4adad-1045">Verwenden Sie stattdessen `az extension`.</span><span class="sxs-lookup"><span data-stu-id="4adad-1045">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="4adad-1046">Core</span><span class="sxs-lookup"><span data-stu-id="4adad-1046">Core</span></span>
* <span data-ttu-id="4adad-1047">Der `AZURE_US_GOV_CLOUD`-Autoritätsendpunkt von AAD wurde von „login.microsoftonline.com“ in „login.microsoftonline.us“ geändert.</span><span class="sxs-lookup"><span data-stu-id="4adad-1047">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="4adad-1048">Problem behoben, aufgrund dessen Telemetriedaten fortlaufend neu gesendet wurden</span><span class="sxs-lookup"><span data-stu-id="4adad-1048">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="4adad-1049">ACS</span><span class="sxs-lookup"><span data-stu-id="4adad-1049">ACS</span></span>

* <span data-ttu-id="4adad-1050">Die Befehle `aks install-connector` und `aks remove-connector` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="4adad-1050">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="4adad-1051">Verbesserte Fehlerberichterstellung für `acs create`</span><span class="sxs-lookup"><span data-stu-id="4adad-1051">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="4adad-1052">Feste Verwendung von `aks get-credentials -f` ohne vollqualifizierten Pfad</span><span class="sxs-lookup"><span data-stu-id="4adad-1052">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="4adad-1053">Advisor</span><span class="sxs-lookup"><span data-stu-id="4adad-1053">Advisor</span></span>

* <span data-ttu-id="4adad-1054">Erste Version</span><span class="sxs-lookup"><span data-stu-id="4adad-1054">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="4adad-1055">AppService</span><span class="sxs-lookup"><span data-stu-id="4adad-1055">Appservice</span></span>

* <span data-ttu-id="4adad-1056">Erstellung feststehender Zertifikatnamen mit `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="4adad-1056">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="4adad-1057">`webapp [list|show]` und `functionapp [list|show]` wurden verbessert, um die richtigen Apps anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="4adad-1057">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="4adad-1058">Standardwert für `WEBSITE_NODE_DEFAULT_VERSION` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1058">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="4adad-1059">Nutzung</span><span class="sxs-lookup"><span data-stu-id="4adad-1059">Consumption</span></span>

* <span data-ttu-id="4adad-1060">Unterstützung für API-Version 2017-11-30 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1060">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="4adad-1061">Container</span><span class="sxs-lookup"><span data-stu-id="4adad-1061">Container</span></span>

* <span data-ttu-id="4adad-1062">Feste Regression für Standardports</span><span class="sxs-lookup"><span data-stu-id="4adad-1062">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="4adad-1063">Überwachen</span><span class="sxs-lookup"><span data-stu-id="4adad-1063">Monitor</span></span>

* <span data-ttu-id="4adad-1064">Unterstützung mehrerer Dimensionen zu Metrikbefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1064">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="4adad-1065">Ressource</span><span class="sxs-lookup"><span data-stu-id="4adad-1065">Resource</span></span>

* <span data-ttu-id="4adad-1066">Argument `--include-response-body` zu `resource show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1066">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="4adad-1067">Rolle</span><span class="sxs-lookup"><span data-stu-id="4adad-1067">Role</span></span>

* <span data-ttu-id="4adad-1068">Anzeige von Standardzuweisungen für „klassische“ Administratoren zu `role assignment list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1068">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="4adad-1069">Unterstützung für das Hinzufügen (anstelle der Überschreibung) von Anmeldeinformationen zu `ad sp reset-credentials` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1069">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="4adad-1070">Verbesserte Fehlerberichterstellung für `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="4adad-1070">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="4adad-1071">SQL</span><span class="sxs-lookup"><span data-stu-id="4adad-1071">SQL</span></span>

* <span data-ttu-id="4adad-1072">Die Befehle `sql db list-usages` und `sql db show-usage` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="4adad-1072">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="4adad-1073">Die Befehle `sql server conn-policy show` und `sql server conn-policy update` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="4adad-1073">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="4adad-1074">VM</span><span class="sxs-lookup"><span data-stu-id="4adad-1074">VM</span></span>

* <span data-ttu-id="4adad-1075">Zoneninformationen zu `az vm list-skus` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1075">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="4adad-1076">14. November 2017</span><span class="sxs-lookup"><span data-stu-id="4adad-1076">November 14, 2017</span></span>

<span data-ttu-id="4adad-1077">Version 2.0.21</span><span class="sxs-lookup"><span data-stu-id="4adad-1077">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="4adad-1078">ACR</span><span class="sxs-lookup"><span data-stu-id="4adad-1078">ACR</span></span>

* <span data-ttu-id="4adad-1079">Unterstützung für das Erstellen von Webhooks in Replikationsregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1079">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="4adad-1080">ACS</span><span class="sxs-lookup"><span data-stu-id="4adad-1080">ACS</span></span>

* <span data-ttu-id="4adad-1081">Formulierung in AKS von „Agent“ in „Knoten“ geändert</span><span class="sxs-lookup"><span data-stu-id="4adad-1081">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="4adad-1082">Option `--orchestrator-release` für `acs create` als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="4adad-1082">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="4adad-1083">VM-Standardgröße für AKS in `Standard_D1_v2` geändert</span><span class="sxs-lookup"><span data-stu-id="4adad-1083">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="4adad-1084">`az aks browse` für Windows korrigiert</span><span class="sxs-lookup"><span data-stu-id="4adad-1084">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="4adad-1085">`az aks get-credentials` für Windows korrigiert</span><span class="sxs-lookup"><span data-stu-id="4adad-1085">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="4adad-1086">AppService</span><span class="sxs-lookup"><span data-stu-id="4adad-1086">Appservice</span></span>

* <span data-ttu-id="4adad-1087">Bereitstellungsquelle `config-zip` für Web-Apps und Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1087">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="4adad-1088">Option `--docker-container-logging` zu `az webapp log config` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1088">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="4adad-1089">Option `storage` aus dem Parameter `--web-server-logging` von `az webapp log config` entfernt</span><span class="sxs-lookup"><span data-stu-id="4adad-1089">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="4adad-1090">Fehlermeldungen für `deployment user set` verbessert</span><span class="sxs-lookup"><span data-stu-id="4adad-1090">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="4adad-1091">Unterstützung für das Erstellen von Linux-Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1091">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="4adad-1092">`list-locations` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="4adad-1092">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="4adad-1093">Batch</span><span class="sxs-lookup"><span data-stu-id="4adad-1093">Batch</span></span>

* <span data-ttu-id="4adad-1094">Fehler im Poolerstellungsbefehl korrigiert, der bei Verwendung einer Ressourcen-ID mit dem Flag `--image` aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="4adad-1094">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="4adad-1095">BatchAI</span><span class="sxs-lookup"><span data-stu-id="4adad-1095">Batchai</span></span>

* <span data-ttu-id="4adad-1096">Kurzoption (`-s`) für `--vm-size` zur Angabe der VM-Größe im Befehl `file-server create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1096">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="4adad-1097">Argumente für Speicherkontoname und -schlüssel zum Parameter `cluster create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1097">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="4adad-1098">Dokumentation für `job list-files` und `job stream-file` korrigiert</span><span class="sxs-lookup"><span data-stu-id="4adad-1098">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="4adad-1099">Kurzoption (`-r`) für `--cluster-name` zur Angabe des Clusternamens im Befehl `job create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1099">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="4adad-1100">Cloud</span><span class="sxs-lookup"><span data-stu-id="4adad-1100">Cloud</span></span>

* <span data-ttu-id="4adad-1101">`cloud [register|update]` geändert, um die Registrierung von Clouds ohne erforderliche Endpunkte zu verhindern</span><span class="sxs-lookup"><span data-stu-id="4adad-1101">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="4adad-1102">Container</span><span class="sxs-lookup"><span data-stu-id="4adad-1102">Container</span></span>

* <span data-ttu-id="4adad-1103">Unterstützung für das Öffnen mehrerer Ports hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1103">Added support to open multiple ports</span></span>
* <span data-ttu-id="4adad-1104">Neustartrichtlinie für Containergruppen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1104">Added container group restart policy</span></span>
* <span data-ttu-id="4adad-1105">Unterstützung zum Einbinden einer Azure-Dateifreigabe als Volume hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1105">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="4adad-1106">Hilfedokumente aktualisiert</span><span class="sxs-lookup"><span data-stu-id="4adad-1106">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="4adad-1107">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="4adad-1107">Data Lake Analytics</span></span>

* <span data-ttu-id="4adad-1108">`[job|account] list` geändert, um präzisere Informationen zu erhalten</span><span class="sxs-lookup"><span data-stu-id="4adad-1108">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="4adad-1109">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="4adad-1109">Data Lake Store</span></span>

* <span data-ttu-id="4adad-1110">`account list` geändert, um präzisere Informationen zu erhalten</span><span class="sxs-lookup"><span data-stu-id="4adad-1110">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="4adad-1111">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="4adad-1111">Extension</span></span>

* <span data-ttu-id="4adad-1112">`extension list-available` hinzugefügt, um das Auflisten offizieller Microsoft-Erweiterungen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="4adad-1112">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="4adad-1113">`--name` zu `extension [add|update]` hinzugefügt, um das Installieren von Erweiterungen nach Name zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="4adad-1113">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="4adad-1114">IoT</span><span class="sxs-lookup"><span data-stu-id="4adad-1114">IoT</span></span>

* <span data-ttu-id="4adad-1115">Unterstützung für Zertifizierungsstellen (CAs) und Zertifikatketten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1115">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="4adad-1116">Überwachen</span><span class="sxs-lookup"><span data-stu-id="4adad-1116">Monitor</span></span>

* <span data-ttu-id="4adad-1117">Befehle vom Typ `activity-log alert` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1117">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="4adad-1118">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="4adad-1118">Network</span></span>

* <span data-ttu-id="4adad-1119">Unterstützung für CAA-DNS-Einträge hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1119">Added support for CAA DNS records</span></span>
* <span data-ttu-id="4adad-1120">Problem behoben, durch das Endpunkte nicht mit `traffic-manager profile update` aktualisiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="4adad-1120">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="4adad-1121">Problem behoben, durch das `vnet update --dns-servers` je nach VNet-Erstellungsmethode nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="4adad-1121">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="4adad-1122">Problem behoben, durch das relative DNS-Namen durch `dns zone import` nicht korrekt importiert wurden</span><span class="sxs-lookup"><span data-stu-id="4adad-1122">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="4adad-1123">Reservations</span><span class="sxs-lookup"><span data-stu-id="4adad-1123">Reservations</span></span>

* <span data-ttu-id="4adad-1124">Erste Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="4adad-1124">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="4adad-1125">Ressource</span><span class="sxs-lookup"><span data-stu-id="4adad-1125">Resource</span></span>

* <span data-ttu-id="4adad-1126">Unterstützung für Ressourcen-IDs zum Parameter `--resource` und Sperren auf Ressourcenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1126">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="4adad-1127">SQL</span><span class="sxs-lookup"><span data-stu-id="4adad-1127">SQL</span></span>

* <span data-ttu-id="4adad-1128">Parameter `--ignore-missing-vnet-service-endpoint` zu `sql server vnet-rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1128">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="4adad-1129">Speicher</span><span class="sxs-lookup"><span data-stu-id="4adad-1129">Storage</span></span>

* <span data-ttu-id="4adad-1130">`storage account create` geändert, sodass die SKU `Standard_RAGRS` als Standard verwendet wird</span><span class="sxs-lookup"><span data-stu-id="4adad-1130">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="4adad-1131">Fehler im Zusammenhang mit Datei-/Blobnamen korrigiert, die ASCII-fremde Zeichen enthalten</span><span class="sxs-lookup"><span data-stu-id="4adad-1131">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="4adad-1132">Fehler korrigiert, der die Verwendung von `--source-uri` mit `storage [blob|file] copy start-batch` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="4adad-1132">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="4adad-1133">Befehle zum Globalisieren und Löschen mehrerer Objekte mit `storage [blob|file] delete-batch` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1133">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="4adad-1134">Problem beim Aktivieren von Metriken mit `storage metrics update` behoben</span><span class="sxs-lookup"><span data-stu-id="4adad-1134">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="4adad-1135">Problem mit Dateien über 200 GB bei Verwendung von `storage blob upload-batch` behoben</span><span class="sxs-lookup"><span data-stu-id="4adad-1135">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="4adad-1136">Problem behoben, durch das `--bypass` und `--default-action` von `storage account [create|update]` ignoriert wurden</span><span class="sxs-lookup"><span data-stu-id="4adad-1136">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="4adad-1137">VM</span><span class="sxs-lookup"><span data-stu-id="4adad-1137">VM</span></span>

* <span data-ttu-id="4adad-1138">Fehler mit `vmss create` korrigiert, der die Verwendung der Größenebene `Basic` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="4adad-1138">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="4adad-1139">`--plan`-Argumente zu `[vm|vmss] create` für benutzerdefinierte Images mit Abrechnungsinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1139">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="4adad-1140">Befehle hinzugefügt: `vm secret `[add|remove|list]</span><span class="sxs-lookup"><span data-stu-id="4adad-1140">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="4adad-1141">`vm format-secret` in `vm secret format` umbenannt</span><span class="sxs-lookup"><span data-stu-id="4adad-1141">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="4adad-1142">Argument `--encrypt format` zu `vm encryption enable` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1142">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="4adad-1143">24. Oktober 2017</span><span class="sxs-lookup"><span data-stu-id="4adad-1143">October 24, 2017</span></span>

<span data-ttu-id="4adad-1144">Version 2.0.20</span><span class="sxs-lookup"><span data-stu-id="4adad-1144">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="4adad-1145">Core</span><span class="sxs-lookup"><span data-stu-id="4adad-1145">Core</span></span>

* <span data-ttu-id="4adad-1146">Aktualisierung von `2017-03-09-profile` zur Verwendung von Version `2016-01-01` der `MGMT_STORAGE`-API</span><span class="sxs-lookup"><span data-stu-id="4adad-1146">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="4adad-1147">ACR</span><span class="sxs-lookup"><span data-stu-id="4adad-1147">ACR</span></span>

* <span data-ttu-id="4adad-1148">Die Ressourcenverwaltung wurde aktualisiert und verweist nun auf die API-Version `2017-10-01`.</span><span class="sxs-lookup"><span data-stu-id="4adad-1148">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="4adad-1149">SKU „Bring Your Own Storage“ wurde in „Klassisch“ geändert.</span><span class="sxs-lookup"><span data-stu-id="4adad-1149">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="4adad-1150">Die Registrierungs-SKUs wurden in „Basic“, „Standard“ und „Premium“ umbenannt.</span><span class="sxs-lookup"><span data-stu-id="4adad-1150">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="4adad-1151">ACS</span><span class="sxs-lookup"><span data-stu-id="4adad-1151">ACS</span></span>

* <span data-ttu-id="4adad-1152">[VORSCHAUVERSION] Befehle vom Typ `az aks` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1152">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="4adad-1153">Problem mit `get-credentials` in Kubernetes behoben</span><span class="sxs-lookup"><span data-stu-id="4adad-1153">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="4adad-1154">AppService</span><span class="sxs-lookup"><span data-stu-id="4adad-1154">Appservice</span></span>

* <span data-ttu-id="4adad-1155">Problem behoben, aufgrund dessen heruntergeladene `webapp`-Protokolle unter Umständen ungültig waren</span><span class="sxs-lookup"><span data-stu-id="4adad-1155">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="4adad-1156">Komponente</span><span class="sxs-lookup"><span data-stu-id="4adad-1156">Component</span></span>

* <span data-ttu-id="4adad-1157">Deutlichere Meldung zur Einstellung für alle Installer und für Bestätigungsaufforderung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1157">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="4adad-1158">Überwachen</span><span class="sxs-lookup"><span data-stu-id="4adad-1158">Monitor</span></span>

* <span data-ttu-id="4adad-1159">Befehle vom Typ `action-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1159">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="4adad-1160">Ressource</span><span class="sxs-lookup"><span data-stu-id="4adad-1160">Resource</span></span>

* <span data-ttu-id="4adad-1161">Inkompatibilität mit der aktuellen Version der msrest-Abhängigkeit in `group export` behoben</span><span class="sxs-lookup"><span data-stu-id="4adad-1161">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="4adad-1162">Problem mit `policy assignment create` behoben, sodass der Befehl mit integrierten Richtliniendefinitionen und Richtliniensatzdefinitionen verwendet werden kann</span><span class="sxs-lookup"><span data-stu-id="4adad-1162">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="4adad-1163">VM</span><span class="sxs-lookup"><span data-stu-id="4adad-1163">VM</span></span>

* <span data-ttu-id="4adad-1164">Argument `--accelerated-networking` zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1164">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="4adad-1165">9. Oktober 2017</span><span class="sxs-lookup"><span data-stu-id="4adad-1165">October 9, 2017</span></span>

<span data-ttu-id="4adad-1166">Version 2.0.19</span><span class="sxs-lookup"><span data-stu-id="4adad-1166">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="4adad-1167">Core</span><span class="sxs-lookup"><span data-stu-id="4adad-1167">Core</span></span>

* <span data-ttu-id="4adad-1168">Verarbeitung von ADFS-Autoritäts-URLs wurde mit einem nachgestellten Schrägstrich zu Azure Stack hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="4adad-1168">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="4adad-1169">AppService</span><span class="sxs-lookup"><span data-stu-id="4adad-1169">Appservice</span></span>

* <span data-ttu-id="4adad-1170">Mit dem neuen Befehl `webapp update` wurde ein allgemeines Update hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="4adad-1170">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="4adad-1171">Batch</span><span class="sxs-lookup"><span data-stu-id="4adad-1171">Batch</span></span>

* <span data-ttu-id="4adad-1172">Aktualisierung auf Batch SDK 4.0.0</span><span class="sxs-lookup"><span data-stu-id="4adad-1172">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="4adad-1173">Die Option `--image` von „VirtualMachineConfiguration“ wurde aktualisiert, um zusätzlich zu „publish:offer:sku:version“ ARM-Imageverweise zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="4adad-1173">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="4adad-1174">Unterstützung für das neue CLI-Erweiterungsmodell für Batch-Erweiterungsbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1174">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="4adad-1175">Batch-Unterstützung aus dem Komponentenmodell entfernt</span><span class="sxs-lookup"><span data-stu-id="4adad-1175">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="4adad-1176">BatchAI</span><span class="sxs-lookup"><span data-stu-id="4adad-1176">Batchai</span></span>

* <span data-ttu-id="4adad-1177">Erste Version des Batch AI-Moduls</span><span class="sxs-lookup"><span data-stu-id="4adad-1177">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="4adad-1178">KeyVault</span><span class="sxs-lookup"><span data-stu-id="4adad-1178">Keyvault</span></span>

* <span data-ttu-id="4adad-1179">Key Vault-Authentifizierungsproblem behoben, das bei Verwendung von ADFS in Azure Stack auftrat.</span><span class="sxs-lookup"><span data-stu-id="4adad-1179">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="4adad-1180">(#4448)</span><span class="sxs-lookup"><span data-stu-id="4adad-1180">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="4adad-1181">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="4adad-1181">Network</span></span>

* <span data-ttu-id="4adad-1182">Das Argument `--server` von `application-gateway address-pool create` ist nun optional, sodass leere Adresspools zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="4adad-1182">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="4adad-1183">`traffic-manager` wurde aktualisiert, um aktuelle Features zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="4adad-1183">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="4adad-1184">Ressource</span><span class="sxs-lookup"><span data-stu-id="4adad-1184">Resource</span></span>

* <span data-ttu-id="4adad-1185">Zusätzliche Unterstützung für `--resource-group/-g`-Optionen für Ressourcengruppennamen zu `group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1185">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="4adad-1186">Befehle für `account lock` hinzugefügt, um die Verwendung mit Sperren auf Abonnementebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="4adad-1186">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="4adad-1187">Befehle für `group lock` hinzugefügt, um die Verwendung mit Sperren auf Gruppenebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="4adad-1187">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="4adad-1188">Befehle für `resource lock` hinzugefügt, um die Verwendung mit Sperren auf Ressourcenebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="4adad-1188">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="4adad-1189">Sql</span><span class="sxs-lookup"><span data-stu-id="4adad-1189">Sql</span></span>

* <span data-ttu-id="4adad-1190">Unterstützung für SQL Transparent Data Encryption (TDE) und TDE für Bring Your Own Key-Szenarien hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1190">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="4adad-1191">Der Befehl `db list-deleted` und der Parameter `db restore --deleted-time` wurden hinzugefügt, um die Ermittlung und Wiederherstellung gelöschter Datenbanken zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="4adad-1191">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="4adad-1192">`db op list` und `db op cancel` wurden hinzugefügt, um das Auflisten und Abbrechen ausgeführter Vorgänge für eine Datenbank zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="4adad-1192">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="4adad-1193">Speicher</span><span class="sxs-lookup"><span data-stu-id="4adad-1193">Storage</span></span>

* <span data-ttu-id="4adad-1194">Unterstützung für Momentaufnahme von Dateifreigaben hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1194">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="4adad-1195">VM</span><span class="sxs-lookup"><span data-stu-id="4adad-1195">Vm</span></span>

* <span data-ttu-id="4adad-1196">Korrektur eines Fehlers in `vm show`, bei dem die Verwendung von `-d` in Verbindung mit fehlenden privaten IP-Adressen einen Absturz verursachte</span><span class="sxs-lookup"><span data-stu-id="4adad-1196">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="4adad-1197">[VORSCHAUVERSION] Unterstützung für paralleles Upgrade zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1197">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="4adad-1198">Unterstützung für das Aktualisieren der Verschlüsselungseinstellungen mit `vm encryption enable` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1198">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="4adad-1199">Parameter `--os-disk-size-gb` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1199">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="4adad-1200">Parameter `--license-type` für Windows zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1200">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="4adad-1201">22. September 2017</span><span class="sxs-lookup"><span data-stu-id="4adad-1201">September 22, 2017</span></span>

<span data-ttu-id="4adad-1202">Version 2.0.18</span><span class="sxs-lookup"><span data-stu-id="4adad-1202">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="4adad-1203">Ressource</span><span class="sxs-lookup"><span data-stu-id="4adad-1203">Resource</span></span>

* <span data-ttu-id="4adad-1204">Unterstützung für das Anzeigen integrierter Richtliniendefinitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1204">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="4adad-1205">Unterstützungsmodusparameter zum Erstellen von Richtliniendefinitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1205">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="4adad-1206">Unterstützung für UI-Definitionen und -Vorlagen zu `managedapp definition create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1206">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="4adad-1207">[WICHTIGE ÄNDERUNG] Der Ressourcentyp `managedapp` wurde von `appliances` in `applications` und von `applianceDefinitions` in `applicationDefinitions` geändert.</span><span class="sxs-lookup"><span data-stu-id="4adad-1207">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="4adad-1208">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="4adad-1208">Network</span></span>

* <span data-ttu-id="4adad-1209">Unterstützung für Verfügbarkeitszone zu Unterbefehlen `network lb` und `network public-ip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1209">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="4adad-1210">Unterstützung für IPv6-Microsoft-Peering zu `express-route` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1210">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="4adad-1211">Befehle für Anwendungssicherheitsgruppe `asg` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1211">Added `asg` application security group commands</span></span>
* <span data-ttu-id="4adad-1212">Argument `--application-security-groups` zu `nic [create|ip-config create|ip-config update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1212">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="4adad-1213">Argumente `--source-asgs` und `--destination-asgs` zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1213">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="4adad-1214">Argumente `--ddos-protection` und `--vm-protection` zu `vnet [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1214">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="4adad-1215">Befehle vom Typ `network [vnet-gateway|vpn-client|show-url]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1215">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="4adad-1216">Speicher</span><span class="sxs-lookup"><span data-stu-id="4adad-1216">Storage</span></span>

* <span data-ttu-id="4adad-1217">Problem behoben, das nach der Aktualisierung des SDK unter Umständen einen Fehler der `storage account network-rule`-Befehle zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="4adad-1217">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="4adad-1218">Eventgrid</span><span class="sxs-lookup"><span data-stu-id="4adad-1218">Eventgrid</span></span>

* <span data-ttu-id="4adad-1219">Azure Event Grid Python SDK für die Verwendung der neueren API-Version „2017-09-15-preview“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="4adad-1219">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="4adad-1220">SQL</span><span class="sxs-lookup"><span data-stu-id="4adad-1220">SQL</span></span>

* <span data-ttu-id="4adad-1221">`sql server list`-Argument `--resource-group` geändert, sodass es nun optional ist.</span><span class="sxs-lookup"><span data-stu-id="4adad-1221">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="4adad-1222">Wird es nicht angegeben, werden alle SQL Server-Instanzen im Abonnement zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4adad-1222">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="4adad-1223">Parameter `--no-wait` zu `db [create|copy|restore|update|replica create|create|update]` und `dw [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1223">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="4adad-1224">KeyVault</span><span class="sxs-lookup"><span data-stu-id="4adad-1224">Keyvault</span></span>

* <span data-ttu-id="4adad-1225">Unterstützung für die Keyvault-Befehlsausführung hinter einem Proxy hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1225">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="4adad-1226">VM</span><span class="sxs-lookup"><span data-stu-id="4adad-1226">VM</span></span>

* <span data-ttu-id="4adad-1227">Unterstützung für Verfügbarkeitszone zu `[vm|vmss|disk] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1227">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="4adad-1228">Problem behoben, das bei Verwendung von `--app-gateway ID` mit `vmss create` einen Fehler zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="4adad-1228">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="4adad-1229">Argument `--asgs` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1229">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="4adad-1230">Unterstützung für die Ausführung von Befehlen auf virtuellen Computern mit `vm run-command` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1230">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="4adad-1231">[VORSCHAU] Unterstützung für VMSS-Datenträgerverschlüsselung mit `vmss encryption` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1231">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="4adad-1232">Unterstützung für die Durchführung der Wartung auf virtuellen Computern mit `vm perform-maintenance` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1232">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="4adad-1233">ACS</span><span class="sxs-lookup"><span data-stu-id="4adad-1233">ACS</span></span>

* <span data-ttu-id="4adad-1234">[VORSCHAU] Argument `--orchestrator-release` zu `acs create` für ACS-Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1234">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="4adad-1235">AppService</span><span class="sxs-lookup"><span data-stu-id="4adad-1235">Appservice</span></span>

* <span data-ttu-id="4adad-1236">Neue Möglichkeit zum Aktualisieren und Anzeigen der Authentifizierungseinstellungen mit `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="4adad-1236">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="4adad-1237">Backup</span><span class="sxs-lookup"><span data-stu-id="4adad-1237">Backup</span></span>

* <span data-ttu-id="4adad-1238">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="4adad-1238">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="4adad-1239">11. September 2017</span><span class="sxs-lookup"><span data-stu-id="4adad-1239">September 11, 2017</span></span>

<span data-ttu-id="4adad-1240">Version 2.0.17</span><span class="sxs-lookup"><span data-stu-id="4adad-1240">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="4adad-1241">Core</span><span class="sxs-lookup"><span data-stu-id="4adad-1241">Core</span></span>

* <span data-ttu-id="4adad-1242">Festlegung einer eigenen Korrelations-ID in Telemetrie durch das Befehlsmodul aktiviert</span><span class="sxs-lookup"><span data-stu-id="4adad-1242">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="4adad-1243">Ein Problem mit der JSON-Sicherungsdatei wurde behoben, das beim Festlegen des Diagnosemodus für Telemetrie auftrat</span><span class="sxs-lookup"><span data-stu-id="4adad-1243">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="4adad-1244">ACS</span><span class="sxs-lookup"><span data-stu-id="4adad-1244">Acs</span></span>

* <span data-ttu-id="4adad-1245">Befehl `acs list-locations` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1245">Added `acs list-locations` command</span></span>
* <span data-ttu-id="4adad-1246">`ssh-key-file` wird mit dem erwarteten Standardwert versehen.</span><span class="sxs-lookup"><span data-stu-id="4adad-1246">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="4adad-1247">AppService</span><span class="sxs-lookup"><span data-stu-id="4adad-1247">Appservice</span></span>

* <span data-ttu-id="4adad-1248">Neue Möglichkeit zum Erstellen einer Web-App in einer anderen Ressourcengruppe als der des aktiven Diensttarifs</span><span class="sxs-lookup"><span data-stu-id="4adad-1248">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="4adad-1249">CDN</span><span class="sxs-lookup"><span data-stu-id="4adad-1249">CDN</span></span>

* <span data-ttu-id="4adad-1250">Der Fehler bei `cdn custom-domain create`, dass „CustomDomain“ nicht wiederholbar ist, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="4adad-1250">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="4adad-1251">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="4adad-1251">Extension</span></span>

* <span data-ttu-id="4adad-1252">Erste Version</span><span class="sxs-lookup"><span data-stu-id="4adad-1252">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="4adad-1253">KeyVault</span><span class="sxs-lookup"><span data-stu-id="4adad-1253">Keyvault</span></span>

* <span data-ttu-id="4adad-1254">Problem behoben, aufgrund dessen bei den Berechtigungen für `keyvault set-policy` die Groß-/Kleinschreibung beachtet werden musste</span><span class="sxs-lookup"><span data-stu-id="4adad-1254">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="4adad-1255">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="4adad-1255">Network</span></span>

* <span data-ttu-id="4adad-1256">`vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="4adad-1256">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="4adad-1257">Das Argument `--private-access-services` wurde für `vnet subnet create/update` in `--service-endpoints` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="4adad-1257">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="4adad-1258">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1258">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="4adad-1259">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1259">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="4adad-1260">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1260">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="4adad-1261">Ressource</span><span class="sxs-lookup"><span data-stu-id="4adad-1261">Resource</span></span>

* <span data-ttu-id="4adad-1262">Übergabe von Parameterdefinitionen für Ressourcenrichtlinien in `policy definition create` und `policy definition update` zulassen</span><span class="sxs-lookup"><span data-stu-id="4adad-1262">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="4adad-1263">Übergabe von Parameterwerten für `policy assignment create` zulassen</span><span class="sxs-lookup"><span data-stu-id="4adad-1263">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="4adad-1264">Übergabe von JSON-Code oder einer Datei für alle Parameter zulassen</span><span class="sxs-lookup"><span data-stu-id="4adad-1264">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="4adad-1265">Inkrementierte API-Version</span><span class="sxs-lookup"><span data-stu-id="4adad-1265">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="4adad-1266">SQL</span><span class="sxs-lookup"><span data-stu-id="4adad-1266">SQL</span></span>

* <span data-ttu-id="4adad-1267">Befehle vom Typ `sql server vnet-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1267">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="4adad-1268">VM</span><span class="sxs-lookup"><span data-stu-id="4adad-1268">VM</span></span>

* <span data-ttu-id="4adad-1269">Behoben: Zugriff nur zuweisen, wenn `--scope` angegeben wird</span><span class="sxs-lookup"><span data-stu-id="4adad-1269">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="4adad-1270">Behoben: Gleiche Erweiterungsbenennung wie Portal verwenden</span><span class="sxs-lookup"><span data-stu-id="4adad-1270">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="4adad-1271">`subscription` aus der Ausgabe von `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="4adad-1271">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="4adad-1272">Behoben: Speicher-SKU vom Typ `[vm|vmss] create` wird nicht auf Datenträger mit einem Image angewendet.</span><span class="sxs-lookup"><span data-stu-id="4adad-1272">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="4adad-1273">Behoben: `vm format-secret --secrets` akzeptierte keine durch neue Zeilen getrennte IDs.</span><span class="sxs-lookup"><span data-stu-id="4adad-1273">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="4adad-1274">31. August 2017</span><span class="sxs-lookup"><span data-stu-id="4adad-1274">August 31, 2017</span></span>

<span data-ttu-id="4adad-1275">Version 2.0.16</span><span class="sxs-lookup"><span data-stu-id="4adad-1275">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="4adad-1276">KeyVault</span><span class="sxs-lookup"><span data-stu-id="4adad-1276">Keyvault</span></span>

* <span data-ttu-id="4adad-1277">Fehler behoben, der beim Versuch auftrat, die Geheimniscodierung mit `secret download` automatisch aufzulösen</span><span class="sxs-lookup"><span data-stu-id="4adad-1277">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="4adad-1278">Sf</span><span class="sxs-lookup"><span data-stu-id="4adad-1278">Sf</span></span>

* <span data-ttu-id="4adad-1279">Alle Befehle wurden durch die Service Fabric-Befehlszeilenschnittstelle (sfctl) ersetzt.</span><span class="sxs-lookup"><span data-stu-id="4adad-1279">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="4adad-1280">Speicher</span><span class="sxs-lookup"><span data-stu-id="4adad-1280">Storage</span></span>

* <span data-ttu-id="4adad-1281">Problem behoben, aufgrund dessen Speicherkonten nicht in Regionen erstellt werden konnten, die die NetworkACLs-Funktion nicht unterstützen</span><span class="sxs-lookup"><span data-stu-id="4adad-1281">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="4adad-1282">Festlegen des Inhaltstyps und der Inhaltscodierung während Blob- und Dateiuploads, wenn weder Inhaltstyp noch Inhaltscodierung angegeben sind</span><span class="sxs-lookup"><span data-stu-id="4adad-1282">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="4adad-1283">28. August 2017</span><span class="sxs-lookup"><span data-stu-id="4adad-1283">August 28, 2017</span></span>

<span data-ttu-id="4adad-1284">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="4adad-1284">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="4adad-1285">Befehlszeilenschnittstelle (CLI)</span><span class="sxs-lookup"><span data-stu-id="4adad-1285">CLI</span></span>

* <span data-ttu-id="4adad-1286">Rechtlichen Hinweis zu `--version` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1286">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="4adad-1287">ACS</span><span class="sxs-lookup"><span data-stu-id="4adad-1287">ACS</span></span>

* <span data-ttu-id="4adad-1288">Vorschauregionen korrigiert</span><span class="sxs-lookup"><span data-stu-id="4adad-1288">Corrected preview regions</span></span>
* <span data-ttu-id="4adad-1289">Standardmäßiges DNS-Namenspräfix (`dns_name_prefix`) ordnungsgemäß formatiert</span><span class="sxs-lookup"><span data-stu-id="4adad-1289">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="4adad-1290">ACS-Befehlsausgabe optimiert</span><span class="sxs-lookup"><span data-stu-id="4adad-1290">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="4adad-1291">AppService</span><span class="sxs-lookup"><span data-stu-id="4adad-1291">Appservice</span></span>

* <span data-ttu-id="4adad-1292">[WICHTIGE ÄNDERUNG] Inkonsistenzen in der Ausgabe von `az webapp config appsettings [delete|set]` behoben</span><span class="sxs-lookup"><span data-stu-id="4adad-1292">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="4adad-1293">Neuen Alias (`-i`) für `az webapp config container set --docker-custom-image-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1293">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="4adad-1294">`az webapp log show` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="4adad-1294">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="4adad-1295">Neue Argumente aus `az webapp delete` verfügbar gemacht, um App Service-Plan, Metriken oder DNS-Registrierung beizubehalten</span><span class="sxs-lookup"><span data-stu-id="4adad-1295">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="4adad-1296">Behoben: Korrekte Erkennung der Sloteinstellungen</span><span class="sxs-lookup"><span data-stu-id="4adad-1296">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="4adad-1297">IoT</span><span class="sxs-lookup"><span data-stu-id="4adad-1297">IoT</span></span>

* <span data-ttu-id="4adad-1298">Behoben (3934): Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="4adad-1298">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="4adad-1299">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="4adad-1299">Network</span></span>

* <span data-ttu-id="4adad-1300">[WICHTIGE ÄNDERUNG] `vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="4adad-1300">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="4adad-1301">[WICHTIGE ÄNDERUNG] Option `--private-access-services` für `--service-endpoints` in `vnet subnet [create|update]` umbenannt</span><span class="sxs-lookup"><span data-stu-id="4adad-1301">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="4adad-1302">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1302">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="4adad-1303">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1303">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="4adad-1304">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1304">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="4adad-1305">Profil</span><span class="sxs-lookup"><span data-stu-id="4adad-1305">Profile</span></span>

* <span data-ttu-id="4adad-1306">`--msi` und `--msi-port` für die Anmeldung mit der Identität eines virtuellen Computers verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="4adad-1306">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="4adad-1307">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="4adad-1307">Service Fabric</span></span>

* <span data-ttu-id="4adad-1308">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="4adad-1308">Preview release</span></span>
* <span data-ttu-id="4adad-1309">Registrierungsbenutzer-/-kennwortregeln für Befehl vereinfacht</span><span class="sxs-lookup"><span data-stu-id="4adad-1309">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="4adad-1310">Kennwortanforderung für Benutzer trotz Parameterübergabe behoben</span><span class="sxs-lookup"><span data-stu-id="4adad-1310">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="4adad-1311">Unterstützung für leere Registrierungsanmeldeinformationen (`registry_cred`) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1311">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="4adad-1312">Speicher</span><span class="sxs-lookup"><span data-stu-id="4adad-1312">Storage</span></span>

* <span data-ttu-id="4adad-1313">Festlegen des Blobtarifs ermöglicht</span><span class="sxs-lookup"><span data-stu-id="4adad-1313">Enabled setting blob tier</span></span>
* <span data-ttu-id="4adad-1314">Argumente `--bypass` und `--default-action` zur Unterstützung von Diensttunneling zu `storage account [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1314">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="4adad-1315">Befehle zum Hinzufügen von VNet-Regeln und IP-basierten Regeln zu `storage account network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1315">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="4adad-1316">Dienstverschlüsselung durch vom Kunden verwalteten Schlüssel ermöglicht</span><span class="sxs-lookup"><span data-stu-id="4adad-1316">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="4adad-1317">[WICHTIGE ÄNDERUNG] Option `--encryption` für Befehl `az storage account create and az storage account update` in `--encryption-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="4adad-1317">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="4adad-1318">Behoben (4220): `az storage account update encryption` – Syntaxkonflikt</span><span class="sxs-lookup"><span data-stu-id="4adad-1318">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="4adad-1319">VM</span><span class="sxs-lookup"><span data-stu-id="4adad-1319">VM</span></span>

* <span data-ttu-id="4adad-1320">Problem behoben, aufgrund dessen bei Verwendung von `--instance-id *` zusätzliche, fehlerhafte Informationen für `vmss get-instance-view` angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="4adad-1320">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="4adad-1321">Unterstützung für `--lb-sku` zu `vmss create` hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="4adad-1321">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="4adad-1322">Menschliche Namen aus der Administratornamen-Blacklist für `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="4adad-1322">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="4adad-1323">Problem behoben, aufgrund dessen `[vm|vmss] create` einen Fehler ausgelöst hat, wenn aus einem Image keine Tarifinformationen extrahiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="4adad-1323">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="4adad-1324">Absturzproblem beim Erstellen einer VMMS-Skalierungsgruppe mit einem internen Lastenausgleich behoben</span><span class="sxs-lookup"><span data-stu-id="4adad-1324">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="4adad-1325">Problem behoben, aufgrund dessen das Argument `--no-wait` nicht mit `vm availability-set create` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="4adad-1325">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="4adad-1326">15. August 2017</span><span class="sxs-lookup"><span data-stu-id="4adad-1326">August 15, 2017</span></span>

<span data-ttu-id="4adad-1327">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="4adad-1327">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="4adad-1328">ACS</span><span class="sxs-lookup"><span data-stu-id="4adad-1328">ACS</span></span>

* <span data-ttu-id="4adad-1329">sshMaster0-Portnummer für Kubernetes korrigiert</span><span class="sxs-lookup"><span data-stu-id="4adad-1329">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="4adad-1330">AppService</span><span class="sxs-lookup"><span data-stu-id="4adad-1330">Appservice</span></span>

* <span data-ttu-id="4adad-1331">Ausnahme beim Erstellen einer neuen Git-basierten Linux-Web-App behoben</span><span class="sxs-lookup"><span data-stu-id="4adad-1331">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="4adad-1332">Event Grid</span><span class="sxs-lookup"><span data-stu-id="4adad-1332">Event Grid</span></span>

* <span data-ttu-id="4adad-1333">SDK-Abhängigkeiten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1333">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="4adad-1334">11. August 2017</span><span class="sxs-lookup"><span data-stu-id="4adad-1334">August 11, 2017</span></span>

<span data-ttu-id="4adad-1335">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="4adad-1335">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="4adad-1336">ACS</span><span class="sxs-lookup"><span data-stu-id="4adad-1336">ACS</span></span>

* <span data-ttu-id="4adad-1337">Weitere Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1337">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="4adad-1338">Batch</span><span class="sxs-lookup"><span data-stu-id="4adad-1338">Batch</span></span>

* <span data-ttu-id="4adad-1339">Auf Batch SDK 3.1.0 und Batch Management SDK 4.1.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="4adad-1339">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="4adad-1340">Neuen Befehl zum Anzeigen der Aufgabenanzahl eines Auftrags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1340">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="4adad-1341">Fehler in der SAS-URL-Verarbeitung der Ressourcendatei behoben</span><span class="sxs-lookup"><span data-stu-id="4adad-1341">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="4adad-1342">Batch-Kontoendpunkt unterstützt nun optionales Präfix „https://“</span><span class="sxs-lookup"><span data-stu-id="4adad-1342">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="4adad-1343">Unterstützung für das Hinzufügen von Listen mit mehr als 100 Aufgaben zu einem Auftrag</span><span class="sxs-lookup"><span data-stu-id="4adad-1343">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="4adad-1344">Debugprotokollierung für das Laden des Erweiterungsbefehlsmoduls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1344">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="4adad-1345">Komponente</span><span class="sxs-lookup"><span data-stu-id="4adad-1345">Component</span></span>

* <span data-ttu-id="4adad-1346">Warnung für veraltete Befehle vom Typ „az component“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1346">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="4adad-1347">Container</span><span class="sxs-lookup"><span data-stu-id="4adad-1347">Container</span></span>

* <span data-ttu-id="4adad-1348">`create`: Problem behoben, aufgrund dessen das Gleichheitszeichen innerhalb einer Umgebungsvariablen nicht zulässig war</span><span class="sxs-lookup"><span data-stu-id="4adad-1348">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="4adad-1349">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="4adad-1349">Data Lake Store</span></span>

* <span data-ttu-id="4adad-1350">Fortschrittsüberwachung ermöglicht</span><span class="sxs-lookup"><span data-stu-id="4adad-1350">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="4adad-1351">Event Grid</span><span class="sxs-lookup"><span data-stu-id="4adad-1351">Event Grid</span></span>

* <span data-ttu-id="4adad-1352">Erste Version</span><span class="sxs-lookup"><span data-stu-id="4adad-1352">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="4adad-1353">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="4adad-1353">Network</span></span>

* <span data-ttu-id="4adad-1354">`lb`: Problem behoben, aufgrund dessen bestimmte Namen untergeordneter Ressourcen bei Auslassung nicht ordnungsgemäß aufgelöst wurden</span><span class="sxs-lookup"><span data-stu-id="4adad-1354">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="4adad-1355">`application-gateway {subresource} delete`: Problem behoben, aufgrund dessen `--no-wait` nicht berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="4adad-1355">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="4adad-1356">`application-gateway http-settings update`: Problem behoben, aufgrund dessen `--connection-draining-timeout` nicht deaktiviert werden konnte</span><span class="sxs-lookup"><span data-stu-id="4adad-1356">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="4adad-1357">Fehler behoben: Unerwartetes Schlüsselwortargument `sa_data_size_kilobyes` bei `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="4adad-1357">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="4adad-1358">Profil</span><span class="sxs-lookup"><span data-stu-id="4adad-1358">Profile</span></span>

* <span data-ttu-id="4adad-1359">`account list`: `--refresh` hinzugefügt, um die neuesten Abonnements vom Server zu synchronisieren</span><span class="sxs-lookup"><span data-stu-id="4adad-1359">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="4adad-1360">Speicher</span><span class="sxs-lookup"><span data-stu-id="4adad-1360">Storage</span></span>

* <span data-ttu-id="4adad-1361">Aktualisieren des Speicherkontos mit vom System zugewiesener Identität ermöglicht</span><span class="sxs-lookup"><span data-stu-id="4adad-1361">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="4adad-1362">VM</span><span class="sxs-lookup"><span data-stu-id="4adad-1362">VM</span></span>

* <span data-ttu-id="4adad-1363">`availability-set`: Fehlerdomänenanzahl bei Konvertierung verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="4adad-1363">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="4adad-1364">Befehl `list-skus` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="4adad-1364">Exposed `list-skus` command</span></span>
* <span data-ttu-id="4adad-1365">Unterstützung der Identitätszuweisung ohne Erstellung von Rollenzuweisungen</span><span class="sxs-lookup"><span data-stu-id="4adad-1365">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="4adad-1366">Anwenden von Speicher-SKU beim Anfügen von Datenträgern</span><span class="sxs-lookup"><span data-stu-id="4adad-1366">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="4adad-1367">Standardmäßiger Betriebssystemdatenträger-Name und Speicher-SKU bei Verwendung verwalteter Datenträger entfernt</span><span class="sxs-lookup"><span data-stu-id="4adad-1367">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="4adad-1368">28. Juli 2017</span><span class="sxs-lookup"><span data-stu-id="4adad-1368">July 28, 2017</span></span>

<span data-ttu-id="4adad-1369">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="4adad-1369">Version 2.0.12</span></span>

* <span data-ttu-id="4adad-1370">Containerbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1370">Added container commands</span></span>
* <span data-ttu-id="4adad-1371">Abrechnungs- und Nutzungsmodule hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1371">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="4adad-1372">Core</span><span class="sxs-lookup"><span data-stu-id="4adad-1372">Core</span></span>

* <span data-ttu-id="4adad-1373">Ausgabe von SDK-Authentifizierungsinformationen für Dienstprinzipale mit Zertifikaten</span><span class="sxs-lookup"><span data-stu-id="4adad-1373">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="4adad-1374">Ausnahmen beim Bereitstellungsfortschritt behoben</span><span class="sxs-lookup"><span data-stu-id="4adad-1374">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="4adad-1375">Verwendung des ARM-Endpunkts aus der aktuellen Cloud für die Erstellung des Abonnementclients</span><span class="sxs-lookup"><span data-stu-id="4adad-1375">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="4adad-1376">Gleichzeitige Verarbeitung der Datei „clouds.config“ verbessert (3636)</span><span class="sxs-lookup"><span data-stu-id="4adad-1376">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="4adad-1377">Aktualisierung der Clientanforderungs-ID für jede Befehlsausführung</span><span class="sxs-lookup"><span data-stu-id="4adad-1377">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="4adad-1378">Erstellung von Abonnementclients mit richtigem SDK-Profil (3635)</span><span class="sxs-lookup"><span data-stu-id="4adad-1378">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="4adad-1379">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="4adad-1379">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="4adad-1380">Unterstützung für Auswahl von Tabellenausgabefeldern über jmespath Abfrage hinzugefügt (3581)</span><span class="sxs-lookup"><span data-stu-id="4adad-1380">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="4adad-1381">Stummschaltung von Analyseargumenten und Anfügeverlauf mit Gesten verbessert (3434)</span><span class="sxs-lookup"><span data-stu-id="4adad-1381">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="4adad-1382">Erstellung von Abonnementclients mit richtigem SDK-Profil</span><span class="sxs-lookup"><span data-stu-id="4adad-1382">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="4adad-1383">Verschiebung aller vorhandenen Erfassungsdateien in den neuesten Ordner</span><span class="sxs-lookup"><span data-stu-id="4adad-1383">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="4adad-1384">Idempotenz für VM-/VMSS-Erstellung behoben (3586)</span><span class="sxs-lookup"><span data-stu-id="4adad-1384">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="4adad-1385">Bei Befehlspfaden wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="4adad-1385">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="4adad-1386">Bei bestimmten booleschen Parametern wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="4adad-1386">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="4adad-1387">Unterstützung der Anmeldung bei lokalem AD FS-Server wie Azure Stack</span><span class="sxs-lookup"><span data-stu-id="4adad-1387">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="4adad-1388">Gleichzeitige Schreibvorgänge in „clouds.config“ behoben (3255)</span><span class="sxs-lookup"><span data-stu-id="4adad-1388">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="4adad-1389">ACR</span><span class="sxs-lookup"><span data-stu-id="4adad-1389">ACR</span></span>

* <span data-ttu-id="4adad-1390">Befehl `show-usage` für verwaltete Registrierungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1390">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="4adad-1391">Unterstützung der SKU-Aktualisierung für verwaltete Registrierungen</span><span class="sxs-lookup"><span data-stu-id="4adad-1391">Support SKU update for managed registries</span></span>
* <span data-ttu-id="4adad-1392">Verwaltete Registrierungen mit verwalteter SKU hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1392">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="4adad-1393">Webhooks für verwaltete Registrierungen mit ACR-Webhook-Befehlsmodul hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1393">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="4adad-1394">AAD-Authentifizierung mit ACR-Anmeldebefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1394">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="4adad-1395">Löschbefehl für Docker-Repositorys, Manifeste und Tags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1395">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="4adad-1396">ACS</span><span class="sxs-lookup"><span data-stu-id="4adad-1396">ACS</span></span>

* <span data-ttu-id="4adad-1397">Unterstützung der API-Version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="4adad-1397">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="4adad-1398">AppService</span><span class="sxs-lookup"><span data-stu-id="4adad-1398">Appservice</span></span>

* <span data-ttu-id="4adad-1399">Fehler behoben, aufgrund dessen die Auflistung der Linux-Web-App keine Werte zurückgegeben hat</span><span class="sxs-lookup"><span data-stu-id="4adad-1399">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="4adad-1400">Unterstützung für das Abrufen von Anmeldeinformationen aus dem ACR</span><span class="sxs-lookup"><span data-stu-id="4adad-1400">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="4adad-1401">Entfernung aller Befehle unter `appservice web`</span><span class="sxs-lookup"><span data-stu-id="4adad-1401">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="4adad-1402">Maskierung von Docker-Registrierungskennwörtern aus der Befehlsausgabe (3656)</span><span class="sxs-lookup"><span data-stu-id="4adad-1402">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="4adad-1403">Gewährleistung der fehlerfreien Verwendung des Standardbrowsers unter macOS (3623)</span><span class="sxs-lookup"><span data-stu-id="4adad-1403">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="4adad-1404">Verbesserung des Nutzens von `webapp log tail` und `webapp log download` (3624)</span><span class="sxs-lookup"><span data-stu-id="4adad-1404">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="4adad-1405">Befehl `traffic-routing` zum Konfigurieren des statischen Routings verfügbar gemacht (3566)</span><span class="sxs-lookup"><span data-stu-id="4adad-1405">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="4adad-1406">Zuverlässigkeit beim Konfigurieren der Quellcodeverwaltung verbessert (3245)</span><span class="sxs-lookup"><span data-stu-id="4adad-1406">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="4adad-1407">Nicht unterstütztes Argument `--node-version` aus `webapp config update` für Windows-Web-Apps entfernt.</span><span class="sxs-lookup"><span data-stu-id="4adad-1407">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="4adad-1408">Verwenden Sie stattdessen `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="4adad-1408">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="4adad-1409">Batch</span><span class="sxs-lookup"><span data-stu-id="4adad-1409">Batch</span></span>

* <span data-ttu-id="4adad-1410">Auf Batch SDK 3.0.0 mit Unterstützung virtueller Computer mit niedriger Priorität in Pools aktualisiert</span><span class="sxs-lookup"><span data-stu-id="4adad-1410">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="4adad-1411">`pool create`-Option `--target-dedicated` in `--target-dedicated-nodes` umbenannt</span><span class="sxs-lookup"><span data-stu-id="4adad-1411">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="4adad-1412">`pool create`-Optionen `--target-low-priority-nodes` und `--application-licenses` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1412">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="4adad-1413">CDN</span><span class="sxs-lookup"><span data-stu-id="4adad-1413">CDN</span></span>

* <span data-ttu-id="4adad-1414">Besser verständliche Fehlermeldung für `cdn endpoint list`, wenn das von `--profile-name` angegebene Profil nicht vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="4adad-1414">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="4adad-1415">Cloud</span><span class="sxs-lookup"><span data-stu-id="4adad-1415">Cloud</span></span>

* <span data-ttu-id="4adad-1416">API-Version des Cloudmetadaten-Endpunkts in das Format JJJJ-MM-TT umgewandelt</span><span class="sxs-lookup"><span data-stu-id="4adad-1416">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="4adad-1417">Katalogendpunkt nicht erforderlich</span><span class="sxs-lookup"><span data-stu-id="4adad-1417">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="4adad-1418">Unterstützung für die Cloudregistrierung nur mit ARM-Endpunkt</span><span class="sxs-lookup"><span data-stu-id="4adad-1418">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="4adad-1419">Option für `cloud set` bereitgestellt, um beim Auswählen der aktuellen Cloud das Profil auswählen zu können</span><span class="sxs-lookup"><span data-stu-id="4adad-1419">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="4adad-1420">`endpoint_vm_image_alias_doc` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="4adad-1420">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="4adad-1421">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="4adad-1421">CosmosDB</span></span>

* <span data-ttu-id="4adad-1422">Möglichkeit zum Erstellen einer Auflistung mit benutzerdefiniertem Partitionsschlüssel behoben</span><span class="sxs-lookup"><span data-stu-id="4adad-1422">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="4adad-1423">Unterstützung für Auflistungs-Standardgültigkeitsdauer hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1423">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="4adad-1424">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="4adad-1424">Data Lake Analytics</span></span>

* <span data-ttu-id="4adad-1425">Zusätzliche Befehle für Compute-Richtlinienverwaltung unter der Überschrift `dla account compute-policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1425">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="4adad-1426">`dla job pipeline show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1426">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="4adad-1427">`dla job recurrence list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1427">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="4adad-1428">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="4adad-1428">Data Lake Store</span></span>

* <span data-ttu-id="4adad-1429">Unterstützung für vom Benutzer verwaltete Schlüsseltresor-Schlüsselrotation in `dls account update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1429">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="4adad-1430">Zugrunde liegende SDK-Version des Data Lake Store-Dateisystems aktualisiert, um ein Leistungsproblem zu behandeln</span><span class="sxs-lookup"><span data-stu-id="4adad-1430">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="4adad-1431">Befehl `dls enable-key-vault` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="4adad-1431">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="4adad-1432">Dieser Befehl versucht, eine vom Benutzer angegebene Key Vault-Instanz zur Verschlüsselung der Daten in einem Data Lake Store-Konto zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="4adad-1432">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="4adad-1433">Interaktiv</span><span class="sxs-lookup"><span data-stu-id="4adad-1433">Interactive</span></span>

* <span data-ttu-id="4adad-1434">Startzeit durch Verwendung zwischengespeicherter Befehle verbessert</span><span class="sxs-lookup"><span data-stu-id="4adad-1434">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="4adad-1435">Testabdeckung verbessert</span><span class="sxs-lookup"><span data-stu-id="4adad-1435">Increased test coverage</span></span>
* <span data-ttu-id="4adad-1436">?-Geste erweitert, sodass sie auch in den nächsten Befehl eingefügt wird</span><span class="sxs-lookup"><span data-stu-id="4adad-1436">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="4adad-1437">Interaktive Fehler mit dem Profil „2017-03-09-profile-preview“ behoben (3587)</span><span class="sxs-lookup"><span data-stu-id="4adad-1437">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="4adad-1438">`--version` als Parameter für den interaktiven Modus zugelassen (3645)</span><span class="sxs-lookup"><span data-stu-id="4adad-1438">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="4adad-1439">Beseitigung von Fehlern im interaktiven Modus beim Abschluss von Überprüfungen (3570)</span><span class="sxs-lookup"><span data-stu-id="4adad-1439">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="4adad-1440">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="4adad-1440">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="4adad-1441">Flag `--progress` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1441">Added `--progress` flag</span></span>
* <span data-ttu-id="4adad-1442">`--debug` und `--verbose` aus Abschlüssen entfernt</span><span class="sxs-lookup"><span data-stu-id="4adad-1442">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="4adad-1443">`interactive` aus Abschlüssen entfernt (3324)</span><span class="sxs-lookup"><span data-stu-id="4adad-1443">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="4adad-1444">IoT</span><span class="sxs-lookup"><span data-stu-id="4adad-1444">IoT</span></span>

* <span data-ttu-id="4adad-1445">Behoben: Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="4adad-1445">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="4adad-1446">(3934)</span><span class="sxs-lookup"><span data-stu-id="4adad-1446">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="4adad-1447">Schlüsseltresor</span><span class="sxs-lookup"><span data-stu-id="4adad-1447">Key vault</span></span>

* <span data-ttu-id="4adad-1448">Befehle für Schlüsseltresor-Wiederherstellungsfeatures hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="4adad-1448">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="4adad-1449">`keyvault`-Unterbefehle: `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="4adad-1449">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="4adad-1450">`keyvault secret`-Unterbefehle: `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="4adad-1450">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="4adad-1451">`keyvault certificate`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="4adad-1451">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="4adad-1452">`keyvault key`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="4adad-1452">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="4adad-1453">Dienstprinzipal-Schlüsseltresorintegration hinzugefügt (3133)</span><span class="sxs-lookup"><span data-stu-id="4adad-1453">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="4adad-1454">Schlüsseltresor-Datenebene auf 0.3.2. aktualisiert</span><span class="sxs-lookup"><span data-stu-id="4adad-1454">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="4adad-1455">(3307)</span><span class="sxs-lookup"><span data-stu-id="4adad-1455">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="4adad-1456">Labor</span><span class="sxs-lookup"><span data-stu-id="4adad-1456">Lab</span></span>

* <span data-ttu-id="4adad-1457">Unterstützung für Übernahme eines beliebigen virtuellen Computers im Labor über `az lab vm claim` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1457">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="4adad-1458">Tabellenausgabeformatierer für `az lab vm list` und `az lab vm show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1458">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="4adad-1459">Überwachen</span><span class="sxs-lookup"><span data-stu-id="4adad-1459">Monitor</span></span>

* <span data-ttu-id="4adad-1460">Korrektur für Vorlagendatei mit Befehl `monitor autoscale-settings get-parameters-template` (3349)</span><span class="sxs-lookup"><span data-stu-id="4adad-1460">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="4adad-1461">`monitor alert-rule-incidents list` in `monitor alert list-incidents` umbenannt</span><span class="sxs-lookup"><span data-stu-id="4adad-1461">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="4adad-1462">`monitor alert-rule-incidents show` in `monitor alert show-incident` umbenannt</span><span class="sxs-lookup"><span data-stu-id="4adad-1462">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="4adad-1463">`monitor metric-defintions list` in `monitor metrics list-definitions` umbenannt</span><span class="sxs-lookup"><span data-stu-id="4adad-1463">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="4adad-1464">`monitor alert-rules` in `monitor alert` umbenannt</span><span class="sxs-lookup"><span data-stu-id="4adad-1464">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="4adad-1465">`monitor alert create` geändert:</span><span class="sxs-lookup"><span data-stu-id="4adad-1465">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="4adad-1466">Unterbefehle vom Typ `condition` und `action` akzeptieren keinen JSON-Code mehr.</span><span class="sxs-lookup"><span data-stu-id="4adad-1466">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="4adad-1467">Hinzufügung zahlreicher Parameter zur Vereinfachung der Regelerstellung</span><span class="sxs-lookup"><span data-stu-id="4adad-1467">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="4adad-1468">`location` nicht mehr erforderlich</span><span class="sxs-lookup"><span data-stu-id="4adad-1468">`location` no longer required</span></span>
  * <span data-ttu-id="4adad-1469">Hinzufügung von Namen- und ID-Unterstützung für Ziel</span><span class="sxs-lookup"><span data-stu-id="4adad-1469">Add name and ID support for target</span></span>
  * <span data-ttu-id="4adad-1470">Entfernung von `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="4adad-1470">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="4adad-1471">Umbenennung von `is-enabled` in `enabled` (nicht mehr erforderlich)</span><span class="sxs-lookup"><span data-stu-id="4adad-1471">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="4adad-1472">`description` wird nun abhängig von der angegebenen Bedingung auf einen Standardwert festgelegt.</span><span class="sxs-lookup"><span data-stu-id="4adad-1472">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="4adad-1473">Hinzufügung von Beispielen zur Verdeutlichung des neuen Formats</span><span class="sxs-lookup"><span data-stu-id="4adad-1473">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="4adad-1474">Unterstützung von Namen oder IDs für Befehle vom Typ `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="4adad-1474">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="4adad-1475">Komfortargumente und Beispiele zu `monitor alert rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1475">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="4adad-1476">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="4adad-1476">Network</span></span>

* <span data-ttu-id="4adad-1477">Befehl `list-private-access-services` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1477">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="4adad-1478">Argument `--private-access-services` zu `vnet subnet create` und `vnet subnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1478">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="4adad-1479">Problem behoben, das einen Fehler für `application-gateway redirect-config create` zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="4adad-1479">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="4adad-1480">Problem behoben, aufgrund dessen `application-gateway redirect-config update` nicht mit `--no-wait` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="4adad-1480">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="4adad-1481">Fehler behoben, der bei der Verwendung des Arguments `--servers` mit `application-gateway address-pool create` und `application-gateway address-pool update` aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="4adad-1481">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="4adad-1482">Befehle vom Typ `application-gateway redirect-config` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1482">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="4adad-1483">Befehle zu `application-gateway ssl-policy` hinzugefügt: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="4adad-1483">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="4adad-1484">Argumente zu `application-gateway ssl-policy set` hinzugefügt: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="4adad-1484">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="4adad-1485">Argumente zu `application-gateway http-settings create` und `application-gateway http-settings update` hinzugefügt: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="4adad-1485">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="4adad-1486">Argumente zu `application-gateway url-path-map create` und `application-gateway url-path-map update` hinzugefügt: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="4adad-1486">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="4adad-1487">Argument `--redirect-config` zu `application-gateway url-path-map rule create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1487">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="4adad-1488">Unterstützung für `--no-wait` zu `application-gateway url-path-map rule delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1488">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="4adad-1489">Argumente zu `application-gateway probe create` und `application-gateway probe update` hinzugefügt: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="4adad-1489">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="4adad-1490">Argument `--redirect-config` zu `application-gateway rule create` und `application-gateway rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1490">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="4adad-1491">Unterstützung für `--accelerated-networking` zu `nic create` und `nic update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1491">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="4adad-1492">Argument `--internal-dns-name-suffix` von `nic create` entfernt</span><span class="sxs-lookup"><span data-stu-id="4adad-1492">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="4adad-1493">Unterstützung für `--dns-servers` zu `nic update` und `nic create` hinzugefügt: Unterstützung für „--dns-servers“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1493">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="4adad-1494">Fehler korrigiert, aufgrund dessen `--local-address-prefixes` von `local-gateway create` ignoriert wurde</span><span class="sxs-lookup"><span data-stu-id="4adad-1494">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="4adad-1495">Unterstützung für `--dns-servers` zu `vnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1495">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="4adad-1496">Fehler beim Erstellen eines Peerings ohne Routenfilterung mit `express-route peering create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="4adad-1496">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="4adad-1497">Fehler korrigiert, aufgrund dessen die Argumente `--provider` und `--bandwidth` nicht mit `express-route update` verwendet werden konnten</span><span class="sxs-lookup"><span data-stu-id="4adad-1497">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="4adad-1498">Fehler mit Standardlogik von `network watcher show-topology` korrigiert</span><span class="sxs-lookup"><span data-stu-id="4adad-1498">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="4adad-1499">Ausgabeformatierung für `network list-usages` verbessert</span><span class="sxs-lookup"><span data-stu-id="4adad-1499">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="4adad-1500">Verwendung der standardmäßigen Front-End-IP-Adresse für `application-gateway http-listener create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="4adad-1500">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="4adad-1501">Verwendung des Standardadresspools, der HTTP-Standardeinstellungen und des HTTP-Standardlisteners für `application-gateway rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="4adad-1501">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="4adad-1502">Verwendung der standardmäßigen Front-End-IP-Adresse und des standardmäßigen Back-End-Pools für `lb rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="4adad-1502">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="4adad-1503">Verwendung der standardmäßigen Front-End-IP-Adresse für `lb inbound-nat-rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="4adad-1503">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="4adad-1504">Profil</span><span class="sxs-lookup"><span data-stu-id="4adad-1504">Profile</span></span>

* <span data-ttu-id="4adad-1505">Unterstützung der Anmeldung innerhalb eines virtuellen Computers mit einer verwalteten Identität</span><span class="sxs-lookup"><span data-stu-id="4adad-1505">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="4adad-1506">Unterstützung der Ausgabe für `account show` im SDK-Authentifizierungsdateiformat</span><span class="sxs-lookup"><span data-stu-id="4adad-1506">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="4adad-1507">Anzeige von Warnungen für veraltete Befehle bei Verwendung von „--expanded-view“</span><span class="sxs-lookup"><span data-stu-id="4adad-1507">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="4adad-1508">Befehl `get-access-token` für die Bereitstellung eines unformatierten AAD-Tokens hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1508">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="4adad-1509">Unterstützung der Anmeldung mit einem Benutzerkonto ohne zugeordnete Abonnements</span><span class="sxs-lookup"><span data-stu-id="4adad-1509">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="4adad-1510">RDBMS</span><span class="sxs-lookup"><span data-stu-id="4adad-1510">RDBMS</span></span>

* <span data-ttu-id="4adad-1511">Unterstützung der abonnementübergreifenden Auflistung von Servern (3417)</span><span class="sxs-lookup"><span data-stu-id="4adad-1511">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="4adad-1512">Behoben: `%s` wird aufgrund von fehlendem `% server_type` nicht verarbeitet (3393)</span><span class="sxs-lookup"><span data-stu-id="4adad-1512">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="4adad-1513">Dokumentquellenzuordnung behoben und CI-Aufgabe zur Überprüfung hinzugefügt (3361)</span><span class="sxs-lookup"><span data-stu-id="4adad-1513">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="4adad-1514">MySQL- und PostgreSQL-Hilfe korrigiert (3369)</span><span class="sxs-lookup"><span data-stu-id="4adad-1514">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="4adad-1515">Ressource</span><span class="sxs-lookup"><span data-stu-id="4adad-1515">Resource</span></span>

* <span data-ttu-id="4adad-1516">Eingabeaufforderungen bei fehlenden Parametern für `group deployment create` verbessert</span><span class="sxs-lookup"><span data-stu-id="4adad-1516">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="4adad-1517">Analyse der Syntax `--parameters KEY=VALUE` verbessert</span><span class="sxs-lookup"><span data-stu-id="4adad-1517">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="4adad-1518">Probleme behoben, durch die Parameterdateien von `group deployment create` bei Verwendung der Syntax `@<file>` nicht mehr erkannt wurden</span><span class="sxs-lookup"><span data-stu-id="4adad-1518">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="4adad-1519">Unterstützung des Arguments `--ids` für Befehle vom Typ `resource` und `managedapp`</span><span class="sxs-lookup"><span data-stu-id="4adad-1519">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="4adad-1520">Einige Analyse- und Fehlermeldungen korrigiert (3584)</span><span class="sxs-lookup"><span data-stu-id="4adad-1520">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="4adad-1521">Analyse vom Typ `--resource-type` für den Befehl `lock` korrigiert, sodass `<resource-namespace>` und `<resource-type>` akzeptiert werden</span><span class="sxs-lookup"><span data-stu-id="4adad-1521">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="4adad-1522">Parameterüberprüfung für Vorlagenlinkvorlagen hinzugefügt (3629)</span><span class="sxs-lookup"><span data-stu-id="4adad-1522">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="4adad-1523">Unterstützung für die Angabe von Bereitstellungsparametern mit der Syntax `KEY=VALUE` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1523">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="4adad-1524">Rolle</span><span class="sxs-lookup"><span data-stu-id="4adad-1524">Role</span></span>

* <span data-ttu-id="4adad-1525">Unterstützung der Ausgabe im SDK-Authentifizierungsdateiformat für `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="4adad-1525">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="4adad-1526">Rollenzuweisungen und dazugehörige AAD-Anwendung beim Löschen eines Dienstprinzipals bereinigt (3610)</span><span class="sxs-lookup"><span data-stu-id="4adad-1526">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="4adad-1527">Einbeziehung des Zeitformats in Beschreibungen vom Typ `--start-date` und `--end-date` für `app create`-Argumente</span><span class="sxs-lookup"><span data-stu-id="4adad-1527">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="4adad-1528">Anzeige von Warnungen für veraltete Befehle bei Verwendung von `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="4adad-1528">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="4adad-1529">Schlüsseltresorintegration zu den Befehlen `create-for-rbac` und `reset-credentials` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1529">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="4adad-1530">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="4adad-1530">Service Fabric</span></span>
* <span data-ttu-id="4adad-1531">Problem behoben, aufgrund dessen große Dateien in Anwendungen beim Hochladen gekürzt wurden (3666)</span><span class="sxs-lookup"><span data-stu-id="4adad-1531">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="4adad-1532">Tests für Service Fabric-Befehle hinzugefügt (3424)</span><span class="sxs-lookup"><span data-stu-id="4adad-1532">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="4adad-1533">Zahlreiche Service Fabric-Befehle korrigiert (3234)</span><span class="sxs-lookup"><span data-stu-id="4adad-1533">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="4adad-1534">SQL</span><span class="sxs-lookup"><span data-stu-id="4adad-1534">SQL</span></span>

* <span data-ttu-id="4adad-1535">Fehlerhaften Parameter `--identity` für `sql server create` entfernt</span><span class="sxs-lookup"><span data-stu-id="4adad-1535">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="4adad-1536">Kennwortwerte aus der Befehlsausgabe von `sql server create` und `sql server update` entfernt</span><span class="sxs-lookup"><span data-stu-id="4adad-1536">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="4adad-1537">Befehle `sql db list-editions` und `sql elastic-pool list-editions` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1537">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="4adad-1538">Speicher</span><span class="sxs-lookup"><span data-stu-id="4adad-1538">Storage</span></span>

* <span data-ttu-id="4adad-1539">Option `--marker` für die Befehle `storage blob list`, `storage container list` und `storage share list` entfernt (3745)</span><span class="sxs-lookup"><span data-stu-id="4adad-1539">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="4adad-1540">Erstellung eines reinen HTTPS-Speicherkontos ermöglicht</span><span class="sxs-lookup"><span data-stu-id="4adad-1540">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="4adad-1541">Speichermetriken, Protokollierung und CORS-Befehle aktualisiert (3495)</span><span class="sxs-lookup"><span data-stu-id="4adad-1541">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="4adad-1542">Ausnahmemeldung von „cors add“ umformuliert (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="4adad-1542">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="4adad-1543">Generator im Probelaufmodus des Downloadbatchbefehls in eine Liste konvertiert (3592)</span><span class="sxs-lookup"><span data-stu-id="4adad-1543">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="4adad-1544">Problem bei Probelauf des Blobdownloadbatchs behoben (3640) (3592)</span><span class="sxs-lookup"><span data-stu-id="4adad-1544">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="4adad-1545">VM</span><span class="sxs-lookup"><span data-stu-id="4adad-1545">VM</span></span>

* <span data-ttu-id="4adad-1546">Unterstützung der NSG-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="4adad-1546">Support configuring nsg</span></span>
* <span data-ttu-id="4adad-1547">Fehler behoben, aufgrund dessen der DNS-Server nicht ordnungsgemäß konfiguriert wurde</span><span class="sxs-lookup"><span data-stu-id="4adad-1547">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="4adad-1548">Unterstützung verwalteter Dienstidentitäten</span><span class="sxs-lookup"><span data-stu-id="4adad-1548">Support managed service identities</span></span>
* <span data-ttu-id="4adad-1549">Problem behoben, aufgrund dessen `cmss create` mit einem vorhandenen Lastenausgleich `--backend-pool-name` benötigte</span><span class="sxs-lookup"><span data-stu-id="4adad-1549">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="4adad-1550">Festlegung, dass die LUN von mit `vm image create` erstellten Datenträgern mit 0 beginnt</span><span class="sxs-lookup"><span data-stu-id="4adad-1550">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="4adad-1551">10. Mai 2017</span><span class="sxs-lookup"><span data-stu-id="4adad-1551">May 10, 2017</span></span>

<span data-ttu-id="4adad-1552">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="4adad-1552">Version 2.0.6</span></span>

* <span data-ttu-id="4adad-1553">Umbenennen von „documentdb“ in „cosmosdb“</span><span class="sxs-lookup"><span data-stu-id="4adad-1553">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="4adad-1554">Hinzufügen von rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="4adad-1554">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="4adad-1555">Einbeziehen der Data Lake Analytics- und Data Lake Store-Module</span><span class="sxs-lookup"><span data-stu-id="4adad-1555">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="4adad-1556">Einbeziehen des Cognitive Services-Moduls</span><span class="sxs-lookup"><span data-stu-id="4adad-1556">Include Cognitive Services module</span></span>
* <span data-ttu-id="4adad-1557">Einbeziehen des Service Fabric-Moduls</span><span class="sxs-lookup"><span data-stu-id="4adad-1557">Include Service Fabric module</span></span>
* <span data-ttu-id="4adad-1558">Einbeziehen des interaktiven Moduls (Umbenennen von „az-shell“)</span><span class="sxs-lookup"><span data-stu-id="4adad-1558">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="4adad-1559">Hinzufügen von Unterstützung für CDN-Befehle</span><span class="sxs-lookup"><span data-stu-id="4adad-1559">Add support for CDN commands</span></span>
* <span data-ttu-id="4adad-1560">Entfernen des Containermoduls</span><span class="sxs-lookup"><span data-stu-id="4adad-1560">Remove Container module</span></span>
* <span data-ttu-id="4adad-1561">Hinzufügen von „az -v“ als Verknüpfung für „az --version“ ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="4adad-1561">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="4adad-1562">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="4adad-1562">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="4adad-1563">Core</span><span class="sxs-lookup"><span data-stu-id="4adad-1563">Core</span></span>

* <span data-ttu-id="4adad-1564">Core: Erfassen von Ausnahmen, die durch einen nicht registrierten Anbieter verursacht werden, und automatische Registrierung</span><span class="sxs-lookup"><span data-stu-id="4adad-1564">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="4adad-1565">Leistung: Dauerhaftes Speichern des ADAL-Tokencaches im Arbeitsspeicher bis zum Prozessende ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="4adad-1565">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="4adad-1566">Korrigieren der vom hexadezimalen Fingerabdruck -o tsv zurückgegebenen Bytes ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="4adad-1566">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="4adad-1567">Verbessern des Downloads des Schlüsseltresorzertifikats und der AAD-SP-Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="4adad-1567">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="4adad-1568">Hinzufügen des Python-Speicherorts zu „az –version“ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="4adad-1568">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="4adad-1569">Anmeldung: Unterstützung der Anmeldung, wenn keine Abonnements vorhanden sind ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="4adad-1569">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="4adad-1570">Core: Beheben eines Fehlers bei zweimaliger Verwendung eines Dienstprinzipals bei der Anmeldung ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="4adad-1570">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="4adad-1571">Core: Ermöglichen der Konfiguration des Dateipfads von „accessTokens.json“ über eine Umgebungsvariable ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="4adad-1571">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="4adad-1572">Core: Zulassen der Anwendung konfigurierter Standardwerte auf optionale Argumente ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="4adad-1572">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="4adad-1573">Core: Verbesserte Leistung</span><span class="sxs-lookup"><span data-stu-id="4adad-1573">core: Improved performance</span></span>
* <span data-ttu-id="4adad-1574">Core: Zertifikate von benutzerdefinierter Zertifizierungsstelle – Unterstützung für das Festlegen der REQUESTS_CA_BUNDLE-Umgebungsvariablen</span><span class="sxs-lookup"><span data-stu-id="4adad-1574">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="4adad-1575">Core: Cloudkonfiguration – Verwenden des Endpunkts „resource manager“, wenn Endpunkt „management“ nicht festgelegt ist</span><span class="sxs-lookup"><span data-stu-id="4adad-1575">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="4adad-1576">ACS</span><span class="sxs-lookup"><span data-stu-id="4adad-1576">ACS</span></span>

* <span data-ttu-id="4adad-1577">Korrigieren der Master- und Agentanzahl als ganze Zahl statt Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4adad-1577">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="4adad-1578">Verfügbarmachen von „az acs create --no-wait“ und „az acs wait“ für die asynchrone Erstellung</span><span class="sxs-lookup"><span data-stu-id="4adad-1578">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="4adad-1579">Verfügbarmachen von „az acs create --validate“ für Probelaufüberprüfungen</span><span class="sxs-lookup"><span data-stu-id="4adad-1579">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="4adad-1580">Entfernen von Windows-Profil vor PUT-Aufruf für Skalierungsbefehl ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="4adad-1580">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="4adad-1581">AppService</span><span class="sxs-lookup"><span data-stu-id="4adad-1581">AppService</span></span>

* <span data-ttu-id="4adad-1582">functionapp: Hinzufügen der vollständigen functionapp-Unterstützung, einschließlich Erstellen, Anzeigen, Auflisten, Löschen, Hostname, SSL usw.</span><span class="sxs-lookup"><span data-stu-id="4adad-1582">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="4adad-1583">Hinzufügen von Team Services (vsts) als Continuous Delivery-Option zu „appservice web source-control config“</span><span class="sxs-lookup"><span data-stu-id="4adad-1583">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="4adad-1584">Erstellen von „az webapp“ als Ersatz für „az appservice web“ (für Abwärtskompatibilität bleibt „az appservice web“ für 2 weitere Releases erhalten)</span><span class="sxs-lookup"><span data-stu-id="4adad-1584">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="4adad-1585">Verfügbarmachen von Argumenten zum Konfigurieren von Bereitstellung und Laufzeitstapeln beim Erstellen von Web-Apps</span><span class="sxs-lookup"><span data-stu-id="4adad-1585">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="4adad-1586">Verfügbarmachen von „webapp list-runtimes“</span><span class="sxs-lookup"><span data-stu-id="4adad-1586">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="4adad-1587">Unterstützen der Konfiguration von Verbindungszeichenfolgen ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="4adad-1587">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="4adad-1588">Unterstützen des Slottauschs mit Vorschau</span><span class="sxs-lookup"><span data-stu-id="4adad-1588">support slot swap with preview</span></span>
* <span data-ttu-id="4adad-1589">Beheben von Fehlern in appservice-Befehlen ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="4adad-1589">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="4adad-1590">Verwenden der Ressourcengruppe des App Service-Plans für Zertifizierungsvorgänge ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="4adad-1590">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="4adad-1591">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="4adad-1591">CosmosDB</span></span>

* <span data-ttu-id="4adad-1592">Umbenennen des documentdb-Moduls in cosmosdb</span><span class="sxs-lookup"><span data-stu-id="4adad-1592">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="4adad-1593">Zusätzliche Unterstützung für documentdb-APIs auf Datenebene: Datenbank- und Sammlungsverwaltung</span><span class="sxs-lookup"><span data-stu-id="4adad-1593">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="4adad-1594">Zusätzliche Unterstützung für das Aktivieren des automatischen Failovers für Datenbankkonten</span><span class="sxs-lookup"><span data-stu-id="4adad-1594">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="4adad-1595">Zusätzliche Unterstützung für die neue ConsistentPrefix-Konsistenzrichtlinie</span><span class="sxs-lookup"><span data-stu-id="4adad-1595">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="4adad-1596">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="4adad-1596">Data Lake Analytics</span></span>

* <span data-ttu-id="4adad-1597">Beheben eines Fehlers, bei dem das Filtern von Auftragslisten nach Ergebnis und Status einen Fehler auslöst</span><span class="sxs-lookup"><span data-stu-id="4adad-1597">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="4adad-1598">Hinzufügen von Unterstützung für den neuen Katalogelementtyp „Paket“</span><span class="sxs-lookup"><span data-stu-id="4adad-1598">Add support for new catalog item type: package.</span></span> <span data-ttu-id="4adad-1599">Zugriff über: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="4adad-1599">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="4adad-1600">Ermöglichen der Auflistung folgender Katalogelemente innerhalb einer Datenbank (keine Schemaspezifikation erforderlich):</span><span class="sxs-lookup"><span data-stu-id="4adad-1600">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="4adad-1601">Table</span><span class="sxs-lookup"><span data-stu-id="4adad-1601">Table</span></span>
  * <span data-ttu-id="4adad-1602">Tabellenwertfunktion</span><span class="sxs-lookup"><span data-stu-id="4adad-1602">Table valued function</span></span>
  * <span data-ttu-id="4adad-1603">Sicht</span><span class="sxs-lookup"><span data-stu-id="4adad-1603">View</span></span>
  * <span data-ttu-id="4adad-1604">Tabellenstatistiken.</span><span class="sxs-lookup"><span data-stu-id="4adad-1604">Table Statistics.</span></span> <span data-ttu-id="4adad-1605">Können auch mit einem Schema, jedoch ohne Angabe eines Tabellennamens aufgelistet werden.</span><span class="sxs-lookup"><span data-stu-id="4adad-1605">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="4adad-1606">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="4adad-1606">Data Lake Store</span></span>

* <span data-ttu-id="4adad-1607">Aktualisieren der Version des zugrunde liegenden Dateisystem-SDK, wodurch eine bessere Unterstützung für die Verarbeitung von Drosselungsszenarien auf Serverseite gewährt wird</span><span class="sxs-lookup"><span data-stu-id="4adad-1607">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="4adad-1608">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="4adad-1608">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="4adad-1609">Fehlende Hilfe für Zugriffsanzeige</span><span class="sxs-lookup"><span data-stu-id="4adad-1609">missed help for access show.</span></span> <span data-ttu-id="4adad-1610">hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="4adad-1610">adding it.</span></span> <span data-ttu-id="4adad-1611">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="4adad-1611">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="4adad-1612">Suchen</span><span class="sxs-lookup"><span data-stu-id="4adad-1612">Find</span></span>

* <span data-ttu-id="4adad-1613">Verbessern von Suchergebnissen und Ermöglichen der Versionsverwaltung des Suchindex</span><span class="sxs-lookup"><span data-stu-id="4adad-1613">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="4adad-1614">KeyVault</span><span class="sxs-lookup"><span data-stu-id="4adad-1614">KeyVault</span></span>

* <span data-ttu-id="4adad-1615">BC:`az keyvault certificate download` Ändern von „-e“ von Zeichenfolge oder Binärdatentyp in PEM oder DER zur besseren Darstellung der Optionen</span><span class="sxs-lookup"><span data-stu-id="4adad-1615">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="4adad-1616">BC: Entfernen von „--expires“ und „--not-before“ aus `keyvault certificate create`, da diese Parameter nicht vom Dienst unterstützt werden</span><span class="sxs-lookup"><span data-stu-id="4adad-1616">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="4adad-1617">Hinzufügen des Parameters „--validity“ zu `keyvault certificate create`, um gezielt den Wert in „--policy“ zu überschreiben</span><span class="sxs-lookup"><span data-stu-id="4adad-1617">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="4adad-1618">Beheben des Problems in `keyvault certificate get-default-policy`, bei dem „expires“ und „not_before“ verfügbar gemacht wurden, „validity_in_months“ hingegen nicht</span><span class="sxs-lookup"><span data-stu-id="4adad-1618">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="4adad-1619">Keyvault-Korrektur für den Import von PEM und PFX ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="4adad-1619">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="4adad-1620">Labor</span><span class="sxs-lookup"><span data-stu-id="4adad-1620">Lab</span></span>

* <span data-ttu-id="4adad-1621">Hinzufügen der Befehle „create“, „show“, „delete“ und „list“ für die Laborumgebung</span><span class="sxs-lookup"><span data-stu-id="4adad-1621">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="4adad-1622">Hinzufügen der Befehle „show“ und „list“ zur Anzeige von ARM-Vorlagen im Labor</span><span class="sxs-lookup"><span data-stu-id="4adad-1622">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="4adad-1623">Hinzufügen des Kennzeichens „--environment“ in `az lab vm list`, um virtuelle Computer nach Umgebung im Labor zu filtern</span><span class="sxs-lookup"><span data-stu-id="4adad-1623">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="4adad-1624">Hinzufügen des benutzerfreundlichen Befehls `az lab formula export-artifacts` zum Exportieren des Artefaktgerüsts innerhalb der Formel eines Labors</span><span class="sxs-lookup"><span data-stu-id="4adad-1624">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="4adad-1625">Hinzufügen von Befehlen zum Verwalten von Geheimnissen in einem Labor</span><span class="sxs-lookup"><span data-stu-id="4adad-1625">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="4adad-1626">Überwachen</span><span class="sxs-lookup"><span data-stu-id="4adad-1626">Monitor</span></span>

* <span data-ttu-id="4adad-1627">Programmfehlerbehebung: Modellieren von `--actions` von `az alert-rules create` zum Verarbeiten von JSON-Zeichenfolgen ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="4adad-1627">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="4adad-1628">Programmfehlerbehebung: Beim Erstellen von Diagnoseeinstellungen werden Protokolle/Metriken aus Anzeigebefehlen nicht akzeptiert ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="4adad-1628">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="4adad-1629">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="4adad-1629">Network</span></span>

* <span data-ttu-id="4adad-1630">Hinzufügen des `network watcher test-connectivity`-Befehls</span><span class="sxs-lookup"><span data-stu-id="4adad-1630">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="4adad-1631">Hinzufügen von Unterstützung für den `--filters`-Parameter für `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="4adad-1631">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="4adad-1632">Hinzufügen von Unterstützung für den Application Gateway-Verbindungsausgleich</span><span class="sxs-lookup"><span data-stu-id="4adad-1632">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="4adad-1633">Hinzufügen von Unterstützung für die Konfiguration von Application Gateway-WAF-Regelsätzen</span><span class="sxs-lookup"><span data-stu-id="4adad-1633">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="4adad-1634">Hinzufügen von Unterstützung für ExpressRoute-Routenfilter und -Regeln</span><span class="sxs-lookup"><span data-stu-id="4adad-1634">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="4adad-1635">Hinzufügen von Unterstützung für geografisches TrafficManager-Routing</span><span class="sxs-lookup"><span data-stu-id="4adad-1635">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="4adad-1636">Hinzufügen von Unterstützung für richtlinienbasierte Datenverkehrsselektoren für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="4adad-1636">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="4adad-1637">Hinzufügen von Unterstützung für IPSec-Richtlinien für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="4adad-1637">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="4adad-1638">Korrektur eines Fehlers bei `vpn-connection create` bei Verwendung der Parameter `--no-wait` oder `--validate`</span><span class="sxs-lookup"><span data-stu-id="4adad-1638">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="4adad-1639">Hinzufügen von Unterstützung für Aktiv/Aktiv-VNET-Gateways</span><span class="sxs-lookup"><span data-stu-id="4adad-1639">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="4adad-1640">Entfernen von NULL-Werten aus der Ausgabe von `network vpn-connection list/show`-Befehlen</span><span class="sxs-lookup"><span data-stu-id="4adad-1640">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="4adad-1641">BC: Korrektur eines Fehlers in der Ausgabe von `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="4adad-1641">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="4adad-1642">Korrektur eines Fehlers, bei dem das Argument „--key-length“ von „vpn-connection create“ nicht ordnungsgemäß analysiert wurde</span><span class="sxs-lookup"><span data-stu-id="4adad-1642">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="4adad-1643">Korrektur eines Fehlers in `dns zone import`, bei dem Datensätze nicht ordnungsgemäß importiert wurden</span><span class="sxs-lookup"><span data-stu-id="4adad-1643">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="4adad-1644">Korrektur eines Fehlers, bei dem `traffic-manager endpoint update` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="4adad-1644">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="4adad-1645">Hinzufügen von Network Watcher-Vorschaubefehlen</span><span class="sxs-lookup"><span data-stu-id="4adad-1645">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="4adad-1646">Profil</span><span class="sxs-lookup"><span data-stu-id="4adad-1646">Profile</span></span>

* <span data-ttu-id="4adad-1647">Unterstützung der Anmeldung, wenn keine Abonnements gefunden werden ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="4adad-1647">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="4adad-1648">Unterstützung für kurze Parameternamen in „az account set --subscription“ ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="4adad-1648">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="4adad-1649">Redis</span><span class="sxs-lookup"><span data-stu-id="4adad-1649">Redis</span></span>

* <span data-ttu-id="4adad-1650">Hinzufügen des Updatebefehls, durch den auch die Möglichkeit zum Skalieren für Redis Cache hinzugefügt wird</span><span class="sxs-lookup"><span data-stu-id="4adad-1650">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="4adad-1651">Verwerfen des Befehls „update-settings“</span><span class="sxs-lookup"><span data-stu-id="4adad-1651">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="4adad-1652">Ressource</span><span class="sxs-lookup"><span data-stu-id="4adad-1652">Resource</span></span>

* <span data-ttu-id="4adad-1653">Hinzufügen der Befehle „managedapp“ und „managedapp definition“ ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="4adad-1653">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="4adad-1654">Unterstützung für die „provider operation“-Befehle ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="4adad-1654">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="4adad-1655">Unterstützung für die Erstellung generischer Ressourcen ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="4adad-1655">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="4adad-1656">Korrigieren der Ressourcenanalyse und der API-Versionssuche</span><span class="sxs-lookup"><span data-stu-id="4adad-1656">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="4adad-1657">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="4adad-1657">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="4adad-1658">Hinzufügen von Dokumenten für „az lock update“</span><span class="sxs-lookup"><span data-stu-id="4adad-1658">Add docs for az lock update.</span></span> <span data-ttu-id="4adad-1659">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="4adad-1659">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="4adad-1660">Beenden mit Fehler bei dem Versuch, Ressourcen für eine nicht vorhandene Gruppe aufzulisten</span><span class="sxs-lookup"><span data-stu-id="4adad-1660">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="4adad-1661">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="4adad-1661">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="4adad-1662">[Compute] Beheben von Problemen mit dem Update von VMSS- und VM-Verfügbarkeitsgruppen</span><span class="sxs-lookup"><span data-stu-id="4adad-1662">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="4adad-1663">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="4adad-1663">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="4adad-1664">Korrigieren des Erstellungs- und Löschvorgangs für Sperren, wenn „parent-resource-path“ auf „None“ festgelegt ist ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="4adad-1664">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="4adad-1665">Rolle</span><span class="sxs-lookup"><span data-stu-id="4adad-1665">Role</span></span>

* <span data-ttu-id="4adad-1666">create-for-rbac: Sicherstellen, dass das SP-Enddatum nicht das Ablaufdatum des Zertifikats überschreitet ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="4adad-1666">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="4adad-1667">RBAC: Hinzufügen vollständiger Unterstützung für „ad group“ ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="4adad-1667">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="4adad-1668">Rolle: Beheben von Probleme beim Rollendefinitionsupdate ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="4adad-1668">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="4adad-1669">create-for-rbac: Sicherstellen, dass das angegebene Benutzerkennwort übernommen wird</span><span class="sxs-lookup"><span data-stu-id="4adad-1669">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="4adad-1670">SQL</span><span class="sxs-lookup"><span data-stu-id="4adad-1670">SQL</span></span>

* <span data-ttu-id="4adad-1671">Hinzufügen der Befehle „az sql server list-usages“ und „az sql db list-usages“</span><span class="sxs-lookup"><span data-stu-id="4adad-1671">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="4adad-1672">SQL: Möglichkeit zur direkten Verbindung mit Ressourcenanbieter ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="4adad-1672">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="4adad-1673">Speicher</span><span class="sxs-lookup"><span data-stu-id="4adad-1673">Storage</span></span>

* <span data-ttu-id="4adad-1674">Festlegen des Ressourcengruppenstandorts als Standardstandort für `storage account create`</span><span class="sxs-lookup"><span data-stu-id="4adad-1674">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="4adad-1675">Hinzufügen von Unterstützung für das inkrementelle Kopieren von Blobs</span><span class="sxs-lookup"><span data-stu-id="4adad-1675">Add support for incremental blob copy</span></span>
* <span data-ttu-id="4adad-1676">Hinzufügen von Unterstützung für den Upload umfangreicher Blockblobs</span><span class="sxs-lookup"><span data-stu-id="4adad-1676">Add support for large block blob upload</span></span>
* <span data-ttu-id="4adad-1677">Ändern der Blockgröße auf 100 MB, wenn die hochzuladende Datei größer als 200 GB ist</span><span class="sxs-lookup"><span data-stu-id="4adad-1677">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="4adad-1678">VM</span><span class="sxs-lookup"><span data-stu-id="4adad-1678">VM</span></span>

* <span data-ttu-id="4adad-1679">avail-set: Festlegen der UD- und FD-Domänenanzahl als optional</span><span class="sxs-lookup"><span data-stu-id="4adad-1679">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="4adad-1680">Hinweis zu VM-Befehlen in unabhängigen Clouds: Vermeiden Sie Features im Zusammenhang mit verwalteten Datenträgern, einschließlich der folgenden:</span><span class="sxs-lookup"><span data-stu-id="4adad-1680">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="4adad-1681">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="4adad-1681">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="4adad-1682">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="4adad-1682">az vm/vmss disk</span></span>
  3. <span data-ttu-id="4adad-1683">Verwenden Sie in „az vm/vmss create“ den Befehl „—use-unmanaged-disk“, um verwaltete Datenträger zu vermeiden. Andere Befehle sollten funktionieren.</span><span class="sxs-lookup"><span data-stu-id="4adad-1683">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="4adad-1684">vm/vmss: Verbessern des Warnungstexts beim Generieren von SSH-Schlüsselpaaren</span><span class="sxs-lookup"><span data-stu-id="4adad-1684">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="4adad-1685">vm/vmss: Unterstützen der Erstellung über ein Marketplace-Image, für das Planinformationen erforderlich sind ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="4adad-1685">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="4adad-1686">3. April 2017</span><span class="sxs-lookup"><span data-stu-id="4adad-1686">April 3, 2017</span></span>

<span data-ttu-id="4adad-1687">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="4adad-1687">Version 2.0.2</span></span>

<span data-ttu-id="4adad-1688">In dieser Version wurden die Komponenten ACR, Batch, KeyVault und SQL eingeführt.</span><span class="sxs-lookup"><span data-stu-id="4adad-1688">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="4adad-1689">Core</span><span class="sxs-lookup"><span data-stu-id="4adad-1689">Core</span></span>

* <span data-ttu-id="4adad-1690">Hinzufügen der Module „acr“, „lab“, „monitor“ und „find“ zur Standardliste</span><span class="sxs-lookup"><span data-stu-id="4adad-1690">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="4adad-1691">Anmeldung: Überspringen des fehlerhaften Mandanten ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="4adad-1691">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="4adad-1692">Anmeldung: Festlegen des Standardabonnements auf ein Abonnement mit dem Status „Enabled“ ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="4adad-1692">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="4adad-1693">Hinzufügen von wait-Befehlen und Unterstützung von „--no-wait“ für mehr Befehle ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="4adad-1693">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="4adad-1694">Core: Unterstützen der Anmeldung per Dienstprinzipal mit einem Zertifikat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="4adad-1694">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="4adad-1695">Hinzufügen der Meldung zu fehlenden Vorlagenparametern</span><span class="sxs-lookup"><span data-stu-id="4adad-1695">Add prompting for missing template parameters.</span></span> <span data-ttu-id="4adad-1696">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="4adad-1696">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="4adad-1697">Unterstützen des Festlegens von Standardwerten für häufig verwendete Argumente, z.B. Standardressourcengruppe, Standardweb und Standard-VM</span><span class="sxs-lookup"><span data-stu-id="4adad-1697">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="4adad-1698">Unterstützen der Anmeldung an einem bestimmten Mandanten</span><span class="sxs-lookup"><span data-stu-id="4adad-1698">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="4adad-1699">ACS</span><span class="sxs-lookup"><span data-stu-id="4adad-1699">ACS</span></span>

* <span data-ttu-id="4adad-1700">[ACS] Hinzufügen von Unterstützung für die Konfiguration eines ACS-Standardclusters ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="4adad-1700">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="4adad-1701">Hinzufügen von Unterstützung der Aufforderung zur Kennworteingabe für SSH-Schlüssel</span><span class="sxs-lookup"><span data-stu-id="4adad-1701">Add support for ssh key password prompting.</span></span> <span data-ttu-id="4adad-1702">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="4adad-1702">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="4adad-1703">Hinzufügen von Unterstützung für Windows-Cluster</span><span class="sxs-lookup"><span data-stu-id="4adad-1703">Add support for windows clusters.</span></span> <span data-ttu-id="4adad-1704">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="4adad-1704">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="4adad-1705">Wechseln von der Rolle „Besitzer“ zur Rolle „Mitwirkender“</span><span class="sxs-lookup"><span data-stu-id="4adad-1705">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="4adad-1706">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="4adad-1706">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="4adad-1707">AppService</span><span class="sxs-lookup"><span data-stu-id="4adad-1707">AppService</span></span>

* <span data-ttu-id="4adad-1708">appservice: Unterstützung für das Abrufen der externen IP-Adresse für DNS A-Einträge ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="4adad-1708">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="4adad-1709">appservice: Unterstützung der Bindung von Platzhalterzertifikaten ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="4adad-1709">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="4adad-1710">appservice: Unterstützung von Veröffentlichungsprofilen für Listen ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="4adad-1710">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="4adad-1711">AppService: Auslösen der Synchronisierung der Quellcodeverwaltung nach der Konfiguration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="4adad-1711">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="4adad-1712">DataLake</span><span class="sxs-lookup"><span data-stu-id="4adad-1712">DataLake</span></span>

* <span data-ttu-id="4adad-1713">Erste Version des Data Lake Analytics-Moduls</span><span class="sxs-lookup"><span data-stu-id="4adad-1713">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="4adad-1714">Erste Version des Data Lake Store-Moduls</span><span class="sxs-lookup"><span data-stu-id="4adad-1714">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="4adad-1715">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="4adad-1715">DocuemntDB</span></span>

* <span data-ttu-id="4adad-1716">DocumentDB: Hinzufügen von Unterstützung für das Auflisten von Verbindungszeichenfolgen ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="4adad-1716">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="4adad-1717">VM</span><span class="sxs-lookup"><span data-stu-id="4adad-1717">VM</span></span>

* <span data-ttu-id="4adad-1718">[Compute] Hinzufügen von AppGateway-Unterstützung für Erstellung von VM-Skalierungsgruppen ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="4adad-1718">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="4adad-1719">[VM/VMSS] Verbesserte Unterstützung für die Datenträgerzwischenspeicherung ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="4adad-1719">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="4adad-1720">VM/VMSS: Einbinden der vom Portal verwendeten Logik zur Überprüfung von Anmeldeinformationen ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="4adad-1720">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="4adad-1721">Hinzufügen von wait-Befehlen und Unterstützung für „--no-wait“ ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="4adad-1721">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="4adad-1722">VM-Skalierungsgruppe: Unterstützung von „\*“ zum Auflisten der übergreifenden Instanzansicht für VMs ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="4adad-1722">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="4adad-1723">Hinzufügen – geheime Schlüssel für virtuellen Computer und VM-Skalierungsgruppe ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="4adad-1723">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="4adad-1724">Zulassen der VM-Erstellung mit spezialisierter VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="4adad-1724">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="4adad-1725">27. Februar 2017</span><span class="sxs-lookup"><span data-stu-id="4adad-1725">February 27, 2017</span></span>

<span data-ttu-id="4adad-1726">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="4adad-1726">Version 2.0.0</span></span>

<span data-ttu-id="4adad-1727">Diese Version der Azure CLI 2.0 ist die erste „allgemein verfügbare“ Version. Die allgemeine Verfügbarkeit gilt für die folgenden Befehlsmodule:</span><span class="sxs-lookup"><span data-stu-id="4adad-1727">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="4adad-1728">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="4adad-1728">Container Service (acs)</span></span>
- <span data-ttu-id="4adad-1729">Compute (einschließlich Resource Manager, VM, VM-Skalierungsgruppen, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="4adad-1729">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="4adad-1730">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="4adad-1730">Networking</span></span>
- <span data-ttu-id="4adad-1731">Speicher</span><span class="sxs-lookup"><span data-stu-id="4adad-1731">Storage</span></span>

<span data-ttu-id="4adad-1732">Diese Befehlsmodule können in der Produktion verwendet werden und verfügen über Unterstützung durch eine Standard-SLA von Microsoft. Sie können Anfragen zu Problemen direkt beim Microsoft-Support oder in der [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/) öffnen. Sie haben die Möglichkeit, Fragen in [StackOverflow mit dem Tag „azure-cli“](http://stackoverflow.com/questions/tagged/azure-cli) zu stellen oder sich unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) an das Produktteam zu wenden. Außerdem können Sie über die Befehlszeile mit dem Befehl `az feedback` Feedback senden.</span><span class="sxs-lookup"><span data-stu-id="4adad-1732">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="4adad-1733">Die Befehle in diesen Modulen sind stabil, und es ist nicht zu erwarten, dass sich die Syntax in den anstehenden Veröffentlichungen dieser Version der Azure CLI ändern.</span><span class="sxs-lookup"><span data-stu-id="4adad-1733">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="4adad-1734">Verwenden Sie zum Überprüfen der Version der CLI den Befehl `az --version`. In der Ausgabe werden die Version der CLI selbst (für diese Veröffentlichung 2.0.0), die einzelnen Befehlsmodule und die von Ihnen genutzten Versionen von Python und GCC aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="4adad-1734">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="4adad-1735">Einige Befehlsmodule verfügen über das Postfix „b*n*“ oder „rc*n*“. Diese Befehlsmodule befinden sich noch in der Vorschauphase und werden später die allgemeine Verfügbarkeit erlangen.</span><span class="sxs-lookup"><span data-stu-id="4adad-1735">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="4adad-1736">Außerdem werden jeden Abend Vorschaubuilds der CLI bereitgestellt. Informationen hierzu finden Sie in der [Anleitung zum Abrufen der abendlichen Builds](https://github.com/Azure/azure-cli#nightly-builds) und im Abschnitt zum [Setup für Entwickler und Beitragen von Code](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="4adad-1736">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="4adad-1737">Sie können für die abendlichen Vorschaubuilds wie folgt Probleme melden:</span><span class="sxs-lookup"><span data-stu-id="4adad-1737">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="4adad-1738">Über die [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="4adad-1738">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="4adad-1739">Per Kontaktaufnahme mit dem Produktteam unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="4adad-1739">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="4adad-1740">Senden von Feedback über die Befehlszeile mit dem Befehl `az feedback`</span><span class="sxs-lookup"><span data-stu-id="4adad-1740">Provide feedback from the command line with the `az feedback` command</span></span>


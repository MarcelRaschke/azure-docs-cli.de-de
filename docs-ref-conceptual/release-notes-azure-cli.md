---
title: Versionshinweise für die Azure CLI
description: Enthält Informationen zu den aktuellen Updates der Azure CLI.
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 08/04/2020
ms.topic: article
ms.service: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 68cd2632e33dcd4e35f818d2a330f009fcbfbdbc
ms.sourcegitcommit: bf84dfb62e910ea246586481863bb43d09d07795
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/04/2020
ms.locfileid: "87551556"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="15ad5-103">Versionshinweise für die Azure CLI</span><span class="sxs-lookup"><span data-stu-id="15ad5-103">Azure CLI release notes</span></span>

# <a name="current-release-notes"></a>[<span data-ttu-id="15ad5-104">Aktuelle Versionshinweise</span><span class="sxs-lookup"><span data-stu-id="15ad5-104">Current release notes</span></span>](#tab/azure-cli)

## <a name="august-04-2020"></a><span data-ttu-id="15ad5-105">04. August 2020</span><span class="sxs-lookup"><span data-stu-id="15ad5-105">August 04, 2020</span></span>

<span data-ttu-id="15ad5-106">Version 2.10.0</span><span class="sxs-lookup"><span data-stu-id="15ad5-106">Version 2.10.0</span></span>

### <a name="aks"></a><span data-ttu-id="15ad5-107">AKS</span><span class="sxs-lookup"><span data-stu-id="15ad5-107">AKS</span></span>

* <span data-ttu-id="15ad5-108">`az aks update`: Argument „--enable-aad“ geändert, um einen RBAC-fähigen AAD-fremden Cluster zu einem von AKS-verwalteten AAD-Cluster zu migrieren</span><span class="sxs-lookup"><span data-stu-id="15ad5-108">`az aks update`: Change --enable-aad argument to migrate a RBAC-enabled non-AAD cluster to a AKS-managed AAD cluster</span></span>
* <span data-ttu-id="15ad5-109">`az aks install-cli`: Argumente „--kubelogin-version“ und „--kubelogin-install-location“ zum Installieren von kubelogin hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-109">`az aks install-cli`: Add --kubelogin-version and --kubelogin-install-location arguments to install kubelogin</span></span>
* <span data-ttu-id="15ad5-110">Befehl „az aks nodepool get-upgrades“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-110">Add az aks nodepool get-upgrades command</span></span>

### <a name="ams"></a><span data-ttu-id="15ad5-111">AMS</span><span class="sxs-lookup"><span data-stu-id="15ad5-111">AMS</span></span>

* <span data-ttu-id="15ad5-112">Korrektur 14021: „az ams account sp“ ist nicht idempotent.</span><span class="sxs-lookup"><span data-stu-id="15ad5-112">Fix #14021: az ams account sp is not idempotent</span></span>

### <a name="apim"></a><span data-ttu-id="15ad5-113">APIM</span><span class="sxs-lookup"><span data-stu-id="15ad5-113">APIM</span></span>

* <span data-ttu-id="15ad5-114">APIM-API-Import: API-Importunterstützung und Erweiterung anderer CLI-Befehle auf der API-Ebene</span><span class="sxs-lookup"><span data-stu-id="15ad5-114">apim api import: support API import and enchance other api level cli commands</span></span>

### <a name="app-service"></a><span data-ttu-id="15ad5-115">App Service</span><span class="sxs-lookup"><span data-stu-id="15ad5-115">App Service</span></span>

* <span data-ttu-id="15ad5-116">Korrektur 13035: Zugriffsbeschränkungsüberprüfung für „az webapp config“ hinzugefügt, um Duplikate zu vermeiden</span><span class="sxs-lookup"><span data-stu-id="15ad5-116">Fix #13035: Add validation for az webapp config access-restriction to avoid adding duplicates</span></span>

### <a name="appconfig"></a><span data-ttu-id="15ad5-117">AppConfig</span><span class="sxs-lookup"><span data-stu-id="15ad5-117">AppConfig</span></span>

* <span data-ttu-id="15ad5-118">Bei fehlender Angabe wird die Standard-SKU verwendet.</span><span class="sxs-lookup"><span data-stu-id="15ad5-118">Default to standard sku if not specified</span></span>
* <span data-ttu-id="15ad5-119">[BREAKING CHANGE] Einstellungen mit JSON-Inhaltstyp werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-119">[BREAKING CHANGE] Support settings with JSON content type</span></span>

### <a name="arm"></a><span data-ttu-id="15ad5-120">ARM</span><span class="sxs-lookup"><span data-stu-id="15ad5-120">ARM</span></span>

* <span data-ttu-id="15ad5-121">`az resource tag`: Fehler im Zusammenhang mit managedApp-Kennzeichnung sowie einige damit zusammenhängende Testprobleme behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-121">`az resource tag`: Fix the bug of managedApp tagging and some related test issues</span></span>
* <span data-ttu-id="15ad5-122">`az deployment mg/tenant what-if`: Unterstützung für die Bereitstellung auf Verwaltungsgruppen- und Mandantenebene hinzugefügt (Was-wäre-wenn)</span><span class="sxs-lookup"><span data-stu-id="15ad5-122">`az deployment mg/tenant what-if`: Add support to management group and tenant level deployment What-If</span></span>
* <span data-ttu-id="15ad5-123">`az deployment mg/tenant create`: Parameter „--confirm-with-what-if/-c“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-123">`az deployment mg/tenant create`: Add --confirm-with-what-if/-c parameter.</span></span>
* <span data-ttu-id="15ad5-124">`az deployment mg/tenant create`: Parameter „--what-if-result-format/-r“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-124">`az deployment mg/tenant create`: Add --what-if-result-format/-r parameter.</span></span>
* <span data-ttu-id="15ad5-125">`az deployment mg/tenant create`: Parameter „--what-if-exclude-change-types/-x“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-125">`az deployment mg/tenant create`: Add --what-if-exclude-change-types/-x parameter.</span></span>
* <span data-ttu-id="15ad5-126">`az tag`: Unterstützung von „az tag“ für Ressourcen-ID-Parameter</span><span class="sxs-lookup"><span data-stu-id="15ad5-126">`az tag`: az tag support for resource id parameter</span></span>

### <a name="backup"></a><span data-ttu-id="15ad5-127">Backup</span><span class="sxs-lookup"><span data-stu-id="15ad5-127">Backup</span></span>

* <span data-ttu-id="15ad5-128">Auslösung von AFS-Container-/Elementerkennung nur bei Bedarf</span><span class="sxs-lookup"><span data-stu-id="15ad5-128">Trigger AFS container/item discovery only when needed</span></span>

### <a name="cdn"></a><span data-ttu-id="15ad5-129">CDN</span><span class="sxs-lookup"><span data-stu-id="15ad5-129">CDN</span></span>

* <span data-ttu-id="15ad5-130">Private Link-Felder zu Ursprung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-130">Add private link fields to origin</span></span>

### <a name="compute"></a><span data-ttu-id="15ad5-131">Compute</span><span class="sxs-lookup"><span data-stu-id="15ad5-131">Compute</span></span>

* <span data-ttu-id="15ad5-132">`az vm/vmss create`: Wahl eines gültigen Benutzernamens für den Benutzer bei ungültigem Standardbenutzernamen</span><span class="sxs-lookup"><span data-stu-id="15ad5-132">`az vm/vmss create`: Select a valid username for user if the default username is invalid</span></span>
* <span data-ttu-id="15ad5-133">`az vm update`: Unterstützung mandantenübergreifender Images</span><span class="sxs-lookup"><span data-stu-id="15ad5-133">`az vm update`: support cross tenant image</span></span>
* <span data-ttu-id="15ad5-134">`az disk-access`: Neue Befehlsgruppe für die Verwendung der Datenträgerzugriffsressource hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-134">`az disk-access`: Add new command group to operate disk access resource</span></span>
* <span data-ttu-id="15ad5-135">Unterstützung der automatischen Platzierung dedizierter Hostgruppen</span><span class="sxs-lookup"><span data-stu-id="15ad5-135">Support dedicated host group automatic placement</span></span>
* <span data-ttu-id="15ad5-136">Unterstützung von PPG und SPG im VMSS-Orchestrierungsmodus</span><span class="sxs-lookup"><span data-stu-id="15ad5-136">Support ppg and spg in VMSS orchestration mode</span></span>

### <a name="config"></a><span data-ttu-id="15ad5-137">Config</span><span class="sxs-lookup"><span data-stu-id="15ad5-137">Config</span></span>

* <span data-ttu-id="15ad5-138">`az config`: Neuer Befehl (`config`) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-138">`az config`: Add new `config` command module</span></span>

### <a name="extension"></a><span data-ttu-id="15ad5-139">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="15ad5-139">Extension</span></span>

* <span data-ttu-id="15ad5-140">Unterstützung der automatischen Installation einer Erweiterung, wenn die Erweiterung eines Befehls nicht installiert ist</span><span class="sxs-lookup"><span data-stu-id="15ad5-140">Support automatically installing an extension if the extension of a command is not installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="15ad5-141">HDInsight</span><span class="sxs-lookup"><span data-stu-id="15ad5-141">HDInsight</span></span>

* <span data-ttu-id="15ad5-142">Drei Parameter zum Befehl `az hdinsight create` hinzugefügt, um Private Link und Verschlüsselung während der Übertragung zu unterstützen:</span><span class="sxs-lookup"><span data-stu-id="15ad5-142">Add 3 parameters to the command `az hdinsight create` to support private link and encryption in transit feature:</span></span>

### <a name="iot-hub"></a><span data-ttu-id="15ad5-143">IoT Hub</span><span class="sxs-lookup"><span data-stu-id="15ad5-143">Iot Hub</span></span>

* <span data-ttu-id="15ad5-144">Korrektur 7792: „iot hub create“ ist nicht idempotent.</span><span class="sxs-lookup"><span data-stu-id="15ad5-144">Fix #7792: IoT Hub Create is not idempotent</span></span>

### <a name="iot-central"></a><span data-ttu-id="15ad5-145">IoT Central</span><span class="sxs-lookup"><span data-stu-id="15ad5-145">IoT Central</span></span>

* <span data-ttu-id="15ad5-146">Parameteroptionenliste für IoT Central hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-146">Add paramater option list for iot central</span></span>

### <a name="keyvault"></a><span data-ttu-id="15ad5-147">KeyVault</span><span class="sxs-lookup"><span data-stu-id="15ad5-147">KeyVault</span></span>

* <span data-ttu-id="15ad5-148">`az keyvault key encrypt/decrypt`: Parameter `--data-type` zum expliziten Angeben der Art von Originaldaten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-148">`az keyvault key encrypt/decrypt`: add parameter `--data-type` for explicitly specifing the type of original data</span></span>

### <a name="monitor"></a><span data-ttu-id="15ad5-149">Überwachen</span><span class="sxs-lookup"><span data-stu-id="15ad5-149">Monitor</span></span>

* <span data-ttu-id="15ad5-150">`az monitor log-analytics workspace data-export`: Unterstützung des Event Hub-Namespace als Ziel</span><span class="sxs-lookup"><span data-stu-id="15ad5-150">`az monitor log-analytics workspace data-export`: support event hub namespace as the destination.</span></span>
* <span data-ttu-id="15ad5-151">`az monitor autoscale`: Unterstützung von Namespace und Dimensionen für „--condition“</span><span class="sxs-lookup"><span data-stu-id="15ad5-151">`az monitor autoscale`: support namespace and dimensions for --condition</span></span>

### <a name="netappfiles"></a><span data-ttu-id="15ad5-152">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="15ad5-152">NetAppFiles</span></span>

* <span data-ttu-id="15ad5-153">`az volume revert`:  Volumewiederherstellung hinzugefügt, um ein Volume auf eine der zugehörigen Momentaufnahmen zurückzusetzen</span><span class="sxs-lookup"><span data-stu-id="15ad5-153">`az volume revert`:  Add Volume Revert to revert a volume to one of its snapshots.</span></span>
* <span data-ttu-id="15ad5-154">[BREAKING CHANGE] `az netappfiles mount-target` entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-154">[BREAKING CHANGE] Remove `az netappfiles mount-target`.</span></span>
* <span data-ttu-id="15ad5-155">`az volume show`: Standort zu Active Directory-Eigenschaften hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-155">`az volume show`: Add site to Active Directory Properties</span></span>

### <a name="network"></a><span data-ttu-id="15ad5-156">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="15ad5-156">Network</span></span>

* <span data-ttu-id="15ad5-157">`az application-gateway private-link add`: Unterstützung der Angabe eines vorhandenen Subnetzes nach ID</span><span class="sxs-lookup"><span data-stu-id="15ad5-157">`az application-gateway private-link add`: support to specify an existing subnet by ID</span></span>
* <span data-ttu-id="15ad5-158">`az network application-gateway waf-policy create`: Unterstützung von Version und Typ</span><span class="sxs-lookup"><span data-stu-id="15ad5-158">`az network application-gateway waf-policy create`: support version and type</span></span>

### <a name="storage"></a><span data-ttu-id="15ad5-159">Storage</span><span class="sxs-lookup"><span data-stu-id="15ad5-159">Storage</span></span>

* <span data-ttu-id="15ad5-160">Korrektur 10302: Unterstützung der Ermittlung des wahrscheinlichen Inhaltstyps beim Synchronisieren von Dateien</span><span class="sxs-lookup"><span data-stu-id="15ad5-160">Fix #10302: Support guess content-type when synchronizing files</span></span>
* <span data-ttu-id="15ad5-161">`az storage blob lease`: Neue API-Version für Blobleasevorgänge angewendet</span><span class="sxs-lookup"><span data-stu-id="15ad5-161">`az storage blob lease`: Apply new api version for blob lease operations</span></span>
* <span data-ttu-id="15ad5-162">`az storage fs access`: Unterstützung von AAD-Anmeldeinformationen bei der Verwaltung der Zugriffssteuerung für das ADLS Gen2-Konto</span><span class="sxs-lookup"><span data-stu-id="15ad5-162">`az storage fs access`: Support AAD credential in managing access control for ADLS Gen2 account</span></span>
* <span data-ttu-id="15ad5-163">`az storage share-rm create/update`: „--access-tier“ hinzugefügt, um die Zugriffsebene zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="15ad5-163">`az storage share-rm create/update`: add --access-tier to support access tier</span></span>

## <a name="july-16-2020"></a><span data-ttu-id="15ad5-164">16. Juli 2020</span><span class="sxs-lookup"><span data-stu-id="15ad5-164">July 16, 2020</span></span>

<span data-ttu-id="15ad5-165">Version 2.9.1</span><span class="sxs-lookup"><span data-stu-id="15ad5-165">Version 2.9.1</span></span>

### <a name="aks"></a><span data-ttu-id="15ad5-166">AKS</span><span class="sxs-lookup"><span data-stu-id="15ad5-166">AKS</span></span>

* <span data-ttu-id="15ad5-167">Explizite Einstellung von VMSS im Windows-Beispielbefehl entfernt, da dies jetzt die Standardeinstellung ist</span><span class="sxs-lookup"><span data-stu-id="15ad5-167">Remove explicit setting of VMSS in Windows example command since it is now default</span></span>

### <a name="iot"></a><span data-ttu-id="15ad5-168">IoT</span><span class="sxs-lookup"><span data-stu-id="15ad5-168">IoT</span></span>

* <span data-ttu-id="15ad5-169">[BREAKING CHANGE] `az iot pnp`: IoT-PNP-Vorschaubefehle aus Core-CLI entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-169">[BREAKING CHANGE] `az iot pnp`: Remove IoT PNP preview commands from core CLI</span></span>

### <a name="rest"></a><span data-ttu-id="15ad5-170">REST</span><span class="sxs-lookup"><span data-stu-id="15ad5-170">REST</span></span>

* <span data-ttu-id="15ad5-171">Behebung Nr. 14152: `az rest`: ARM-URLs ohne Abonnement-ID werden nun akzeptiert.</span><span class="sxs-lookup"><span data-stu-id="15ad5-171">Fix #14152: `az rest`: Accept ARM URLs without subscription ID</span></span>

### <a name="storage"></a><span data-ttu-id="15ad5-172">Storage</span><span class="sxs-lookup"><span data-stu-id="15ad5-172">Storage</span></span>

* <span data-ttu-id="15ad5-173">Behebung Nr. 14138: Einige Berechtigungen sind nun optional.</span><span class="sxs-lookup"><span data-stu-id="15ad5-173">Fix #14138: Make some permissions optional</span></span>

## <a name="july-14-2020"></a><span data-ttu-id="15ad5-174">14. Juli 2020</span><span class="sxs-lookup"><span data-stu-id="15ad5-174">July 14, 2020</span></span>

<span data-ttu-id="15ad5-175">Version 2.9.0</span><span class="sxs-lookup"><span data-stu-id="15ad5-175">Version 2.9.0</span></span>

### <a name="acr"></a><span data-ttu-id="15ad5-176">ACR</span><span class="sxs-lookup"><span data-stu-id="15ad5-176">ACR</span></span>

* <span data-ttu-id="15ad5-177">Verarbeiten des Protokollartefaktlinks aus der Registrierung zum Streamen von Protokollen</span><span class="sxs-lookup"><span data-stu-id="15ad5-177">Handle log artifact link from Registry to stream logs</span></span>
* <span data-ttu-id="15ad5-178">Helm2-Befehle als veraltet kennzeichnen</span><span class="sxs-lookup"><span data-stu-id="15ad5-178">Deprecate helm2 commands</span></span>

### <a name="aks"></a><span data-ttu-id="15ad5-179">AKS</span><span class="sxs-lookup"><span data-stu-id="15ad5-179">AKS</span></span>

* <span data-ttu-id="15ad5-180">`az aks create`: Argument „--enable-aad“ hinzufügen</span><span class="sxs-lookup"><span data-stu-id="15ad5-180">`az aks create`: add --enable-aad argument</span></span>
* <span data-ttu-id="15ad5-181">`az aks update`: Argument „--enable-aad“ hinzufügen</span><span class="sxs-lookup"><span data-stu-id="15ad5-181">`az aks update`: add --enable-aad argument</span></span>

### <a name="apim"></a><span data-ttu-id="15ad5-182">APIM</span><span class="sxs-lookup"><span data-stu-id="15ad5-182">APIM</span></span>

* <span data-ttu-id="15ad5-183">Allgemeine Befehle vom Typ „az apim api“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-183">Added general az apim api commands</span></span>

### <a name="appconfig"></a><span data-ttu-id="15ad5-184">AppConfig</span><span class="sxs-lookup"><span data-stu-id="15ad5-184">AppConfig</span></span>

* <span data-ttu-id="15ad5-185">Beispiel für die Verwendung von „--fields“ in AppConfig-Revision hinzufügen</span><span class="sxs-lookup"><span data-stu-id="15ad5-185">Add example for using --fields in appconfig revision</span></span>

### <a name="appservice"></a><span data-ttu-id="15ad5-186">AppService</span><span class="sxs-lookup"><span data-stu-id="15ad5-186">AppService</span></span>

* <span data-ttu-id="15ad5-187">`az functionapp create`: Unterstützung für Java 11 und PowerShell 7 hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-187">`az functionapp create`: Added support for Java 11 and Powershell 7.</span></span> <span data-ttu-id="15ad5-188">Unterstützung für Stapel-API hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-188">Added Stacks API Support.</span></span>
* <span data-ttu-id="15ad5-189">Behebung von Nr. 14208: Erstellen einer App mit mehreren Containern erzeugt einen Fehler</span><span class="sxs-lookup"><span data-stu-id="15ad5-189">Fix #14208 multi-container app creation fails</span></span>
* <span data-ttu-id="15ad5-190">Korrektur von „az webapp create“ – hartcodierte Laufzeitstapel verwenden</span><span class="sxs-lookup"><span data-stu-id="15ad5-190">Fix az webapp create - use hardcoded runtime stacks</span></span>

### <a name="arm"></a><span data-ttu-id="15ad5-191">ARM</span><span class="sxs-lookup"><span data-stu-id="15ad5-191">ARM</span></span>

* <span data-ttu-id="15ad5-192">`az resource tag`: Behebung des Problems beim Taggen von Ressourcen mit dem Ressourcentyp `Microsoft.ContainerInstance/containerGroups`</span><span class="sxs-lookup"><span data-stu-id="15ad5-192">`az resource tag`: Fix the problem of tagging resources with resource type `Microsoft.ContainerInstance/containerGroups`</span></span>

### <a name="compute"></a><span data-ttu-id="15ad5-193">Compute</span><span class="sxs-lookup"><span data-stu-id="15ad5-193">Compute</span></span>

* <span data-ttu-id="15ad5-194">Datenträgerversion aktualisieren 2020-05-01, Compute 2020-06-01</span><span class="sxs-lookup"><span data-stu-id="15ad5-194">Bump version disks 2020-05-01, compute 2020-06-01</span></span>
* <span data-ttu-id="15ad5-195">Doppelte Verschlüsselung des Datenträgerverschlüsselungssatzes</span><span class="sxs-lookup"><span data-stu-id="15ad5-195">Double encryption of disk encryption set</span></span>
* <span data-ttu-id="15ad5-196">`az vmss update`: Unterstützung für das Angeben eines mandantenübergreifendes Image.</span><span class="sxs-lookup"><span data-stu-id="15ad5-196">`az vmss update`: support specify cross tenant image.</span></span>
* <span data-ttu-id="15ad5-197">`az sig image-version create`: Unterstützung für das Angeben eines mandantenübergreifendes Image.</span><span class="sxs-lookup"><span data-stu-id="15ad5-197">`az sig image-version create`: support specify cross tenant image.</span></span>
* <span data-ttu-id="15ad5-198">vm/vmss create: Verschlüsselung von Cache und Daten während der Übertragung für (Betriebssystem-)Datenträger und temporäre Datenträger für VM und VMSS</span><span class="sxs-lookup"><span data-stu-id="15ad5-198">vm/vmss create: Encryption of cache & data-in-transit for OS/Data disks and temp disks for VM & VMSS</span></span>
* <span data-ttu-id="15ad5-199">Vorgang „simulate-eviction“ für VM und VMSS hinzufügen</span><span class="sxs-lookup"><span data-stu-id="15ad5-199">Add simulate-eviction operation for VM and VMSS</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="15ad5-200">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="15ad5-200">CosmosDB</span></span>

* <span data-ttu-id="15ad5-201">Aktuelle Features: Autoscale, IpRules, EnableFreeTier und EnableAnalyticalStorage</span><span class="sxs-lookup"><span data-stu-id="15ad5-201">Recent features: Autoscale, IpRules, EnableFreeTier and EnableAnalyticalStorage</span></span>

### <a name="eventgrid"></a><span data-ttu-id="15ad5-202">EventGrid</span><span class="sxs-lookup"><span data-stu-id="15ad5-202">EventGrid</span></span>

* <span data-ttu-id="15ad5-203">CLI-Unterstützung für 2020-04-01-preview hinzufügen und Previewfunktionen mit „is_Preview=True“ kennzeichnen</span><span class="sxs-lookup"><span data-stu-id="15ad5-203">Add CLI support for 2020-04-01-preview and mark preview features with is_Preview=True</span></span>

### <a name="find"></a><span data-ttu-id="15ad5-204">Suchen</span><span class="sxs-lookup"><span data-stu-id="15ad5-204">Find</span></span>

* <span data-ttu-id="15ad5-205">Behebung von Nr. 14094 „az find“: Abfragen schlagen fehl, wenn nicht angemeldet und Telemetrie deaktiviert</span><span class="sxs-lookup"><span data-stu-id="15ad5-205">Fix #14094 az find Fix Queries failing when not logged in and when telemetry is disabled</span></span>

### <a name="hdinsight"></a><span data-ttu-id="15ad5-206">HDInsight</span><span class="sxs-lookup"><span data-stu-id="15ad5-206">HDInsight</span></span>

* <span data-ttu-id="15ad5-207">Zwei Befehle zur Unterstützung der Neustartfunktion für HDInsight-Knoten hinzufügen</span><span class="sxs-lookup"><span data-stu-id="15ad5-207">Add two commands to support hdinsight node reboot feature</span></span>

### <a name="monitor"></a><span data-ttu-id="15ad5-208">Überwachen</span><span class="sxs-lookup"><span data-stu-id="15ad5-208">Monitor</span></span>

* <span data-ttu-id="15ad5-209">Vorschaukennzeichnung für Befehle unter Log Analytics-Arbeitsbereich entfernen</span><span class="sxs-lookup"><span data-stu-id="15ad5-209">Remove preview flag for commands under Log Analytics workspace</span></span>
* <span data-ttu-id="15ad5-210">`az monitor diagnostic-settings subscription`: Diagnoseeinstellungen für Abonnement unterstützen</span><span class="sxs-lookup"><span data-stu-id="15ad5-210">`az monitor diagnostic-settings subscription`: Support diagnositc settings for subscription</span></span>
* <span data-ttu-id="15ad5-211">`az monitor metrics`: „,“ und „|“ in Metrikname unterstützen</span><span class="sxs-lookup"><span data-stu-id="15ad5-211">`az monitor metrics`: support ',' and '|' in metric name</span></span>
* <span data-ttu-id="15ad5-212">`az monitor log-analytics workspace data-export`: Log Analytics-Datenexport unterstützen</span><span class="sxs-lookup"><span data-stu-id="15ad5-212">`az monitor log-analytics workspace data-export`: support log analytics data export</span></span>

### <a name="network"></a><span data-ttu-id="15ad5-213">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="15ad5-213">Network</span></span>

* <span data-ttu-id="15ad5-214">`az network application-gateway frontend-ip update`: Parameter „--public-ip-address“ als veraltet markieren</span><span class="sxs-lookup"><span data-stu-id="15ad5-214">`az network application-gateway frontend-ip update`: Deprecating the --public-ip-address parameter</span></span>
* <span data-ttu-id="15ad5-215">„azure-mgmt-network“ auf 11.0.0 aktualisieren</span><span class="sxs-lookup"><span data-stu-id="15ad5-215">Bump azure-mgmt-network to 11.0.0</span></span>
* <span data-ttu-id="15ad5-216">`az network express-route gateway connection`: Routingkonfiguration unterstützen</span><span class="sxs-lookup"><span data-stu-id="15ad5-216">`az network express-route gateway connection`: support routing configuration</span></span>
* <span data-ttu-id="15ad5-217">`az network virtual-appliance`: Virtuelle Azure-Netzwerkgerät unterstützen.</span><span class="sxs-lookup"><span data-stu-id="15ad5-217">`az network virtual-appliance`: Support Azure network virtual appliance.</span></span>
* <span data-ttu-id="15ad5-218">Application Gateway-Unterstützung der Funktion für private Links</span><span class="sxs-lookup"><span data-stu-id="15ad5-218">Application Gateway support private link feature</span></span>

### <a name="policyinsights"></a><span data-ttu-id="15ad5-219">PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="15ad5-219">PolicyInsights</span></span>

* <span data-ttu-id="15ad5-220">`az policy state`: Befehl „trigger-scan“ zu Auswertungen der Compliance von Auslöserrichtinien hinzufügen</span><span class="sxs-lookup"><span data-stu-id="15ad5-220">`az policy state`: add trigger-scan command to trigger policy compliance evaluations</span></span>
* <span data-ttu-id="15ad5-221">`az policy state list`: Versionen von Richtlinienentitäten in jedem Compliancedatensatz verfügbar machen</span><span class="sxs-lookup"><span data-stu-id="15ad5-221">`az policy state list`: expose versions of policy entities in each compliance record</span></span>

### <a name="profile"></a><span data-ttu-id="15ad5-222">Profil</span><span class="sxs-lookup"><span data-stu-id="15ad5-222">Profile</span></span>

* <span data-ttu-id="15ad5-223">`az account get-access-token`: „expiresOn“ für verwaltete Identität anzeigen</span><span class="sxs-lookup"><span data-stu-id="15ad5-223">`az account get-access-token`: Show expiresOn for Managed Identity</span></span>

### <a name="rdbms"></a><span data-ttu-id="15ad5-224">RDBMS</span><span class="sxs-lookup"><span data-stu-id="15ad5-224">RDBMS</span></span>

* <span data-ttu-id="15ad5-225">TLS-Mindestversion unterstützen</span><span class="sxs-lookup"><span data-stu-id="15ad5-225">Support Minimum TLS version</span></span>
* <span data-ttu-id="15ad5-226">Infrastrukturverschlüsselung für Azure Postgres und MySQL hinzufügen</span><span class="sxs-lookup"><span data-stu-id="15ad5-226">Add Infrastructure Encryption for Azure Postgres and MySQL</span></span>

### <a name="security"></a><span data-ttu-id="15ad5-227">Sicherheit</span><span class="sxs-lookup"><span data-stu-id="15ad5-227">Security</span></span>

* <span data-ttu-id="15ad5-228">Befehl „allowed_connections“ hinzufügen</span><span class="sxs-lookup"><span data-stu-id="15ad5-228">Add allowed_connections commands</span></span>
* <span data-ttu-id="15ad5-229">Befehle für adaptive Netzwerkhärtung hinzufügen</span><span class="sxs-lookup"><span data-stu-id="15ad5-229">Add Adaptive network hardeningss commands</span></span>
* <span data-ttu-id="15ad5-230">Befehle vom Typ „adaptive_application_controls“ hinzufügen</span><span class="sxs-lookup"><span data-stu-id="15ad5-230">Add adaptive_application_controls commands</span></span>
* <span data-ttu-id="15ad5-231">Hinzufügen von „az security iot-solution“/„iot-alerts“/„iot-recommendations“/„iot-analytics“ REST zu Azure CLI</span><span class="sxs-lookup"><span data-stu-id="15ad5-231">Addition of az security iot-solution/ iot-alerts/iot-recommendations/iot-analytics REST to Azure CLI</span></span>
* <span data-ttu-id="15ad5-232">CLI für Einhaltung gesetzlicher Bestimmungen hinzufügen</span><span class="sxs-lookup"><span data-stu-id="15ad5-232">Add regulatory compliance CLI</span></span>

### <a name="signalr"></a><span data-ttu-id="15ad5-233">SignalR</span><span class="sxs-lookup"><span data-stu-id="15ad5-233">SignalR</span></span>

* <span data-ttu-id="15ad5-234">Features einschließlich der Verwaltung privater Endpunktverbindungen, Netzwerkregeln und Upstream hinzufügen</span><span class="sxs-lookup"><span data-stu-id="15ad5-234">Add features including managing private endpoint connections, network rules and upstream</span></span>

### <a name="sql"></a><span data-ttu-id="15ad5-235">SQL</span><span class="sxs-lookup"><span data-stu-id="15ad5-235">SQL</span></span>

* <span data-ttu-id="15ad5-236">`az sql mi create`, `az sql mi update`: Parameter `--tags` zur Unterstützung von Ressourcenkennzeichnung hinzufügen</span><span class="sxs-lookup"><span data-stu-id="15ad5-236">`az sql mi create`, `az sql mi update`: Add `--tags` parameter to support resource tagging</span></span>
* <span data-ttu-id="15ad5-237">`az sql mi failover`: Failover vom primären oder sekundären Punkt unterstützen</span><span class="sxs-lookup"><span data-stu-id="15ad5-237">`az sql mi failover`: Support failover from primary or secondary point</span></span>

### <a name="storage"></a><span data-ttu-id="15ad5-238">Storage</span><span class="sxs-lookup"><span data-stu-id="15ad5-238">Storage</span></span>

* <span data-ttu-id="15ad5-239">`az storage account create/update`: „--allow-blob-public-access“ hinzufügen, um den öffentlichen Zugriff für Blob und Container zuzulassen oder zu unterbinden</span><span class="sxs-lookup"><span data-stu-id="15ad5-239">`az storage account create/update`: Add --allow-blob-public-access to allow or disallow public access for blob and containers</span></span>
* <span data-ttu-id="15ad5-240">`az storage account create/update`: `--min-tls-version` hinzufügen, um das Festlegen der TLS-Mindestversion für Anforderungen an den Speicher zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="15ad5-240">`az storage account create/update`: Add `--min-tls-version` to support setting the minimum TLS version to be permitted on requests to storage.</span></span>
* <span data-ttu-id="15ad5-241">Token-Anmeldeinformationen zum Einchecken entfernen</span><span class="sxs-lookup"><span data-stu-id="15ad5-241">Remove check in token credential</span></span>
* <span data-ttu-id="15ad5-242">Namen des Speicherkontos in Beispielen korrigieren</span><span class="sxs-lookup"><span data-stu-id="15ad5-242">Fix the storage account name in examples</span></span>

### <a name="webapp"></a><span data-ttu-id="15ad5-243">Webapp</span><span class="sxs-lookup"><span data-stu-id="15ad5-243">Webapp</span></span>

* <span data-ttu-id="15ad5-244">Fehlerbehebung: „az webapp log deployment show -“ gibt Bereitstellungsprotokolle anstatt von Protokollmetadaten zurück</span><span class="sxs-lookup"><span data-stu-id="15ad5-244">Bugfix: az webapp log deployment show - return deployment logs instead of log metadata</span></span>
* <span data-ttu-id="15ad5-245">Fehlerbehebung: „az webapp vnet-integration“ hinzufügen – Fehlerbehandlung korrigieren bei ungültigem VNET-Namen, VNET-Ressourcen-ID unterstützen</span><span class="sxs-lookup"><span data-stu-id="15ad5-245">Bugfix: az webapp vnet-integration add - fix error handling if bad vnet name, support vnet resource ID</span></span>

## <a name="june-23-2020"></a><span data-ttu-id="15ad5-246">23. Juni 2020</span><span class="sxs-lookup"><span data-stu-id="15ad5-246">June 23, 2020</span></span>

<span data-ttu-id="15ad5-247">Version 2.8.0</span><span class="sxs-lookup"><span data-stu-id="15ad5-247">Version 2.8.0</span></span>

### <a name="acr"></a><span data-ttu-id="15ad5-248">ACR</span><span class="sxs-lookup"><span data-stu-id="15ad5-248">ACR</span></span>

* <span data-ttu-id="15ad5-249">Unterstützung für Deaktivierung des Regionsendpunkts/Routings hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-249">Add support for region endpoint disable / routing disable</span></span>
* <span data-ttu-id="15ad5-250">[BREAKING CHANGE] `az acr login --expose-token` akzeptiert Benutzername und Kennwort nicht.</span><span class="sxs-lookup"><span data-stu-id="15ad5-250">[BREAKING CHANGE] `az acr login --expose-token` does not accept username and password</span></span>

### <a name="acs"></a><span data-ttu-id="15ad5-251">ACS</span><span class="sxs-lookup"><span data-stu-id="15ad5-251">ACS</span></span>

* <span data-ttu-id="15ad5-252">Privater Cluster und API „2019-10-27-preview“ entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-252">Remove private cluster and 2019-10-27-preview API</span></span>

### <a name="aks"></a><span data-ttu-id="15ad5-253">AKS</span><span class="sxs-lookup"><span data-stu-id="15ad5-253">AKS</span></span>

* <span data-ttu-id="15ad5-254">Unterstützung: Ja, für „az aks upgrade“</span><span class="sxs-lookup"><span data-stu-id="15ad5-254">Support --yes for az aks upgrade</span></span>
* <span data-ttu-id="15ad5-255">„Änderung der Standard-VM-SKU in Standard_D2s_v3 (Nr. 13541)“ wiederhergestellt</span><span class="sxs-lookup"><span data-stu-id="15ad5-255">Revert "change default vm sku to Standard_D2s_v3 (#13541)"</span></span>
* <span data-ttu-id="15ad5-256">„az aks update --uptime-sla“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-256">Add "az aks update --uptime-sla"</span></span>
* <span data-ttu-id="15ad5-257">Tippfehler im Befehl „az aks update“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-257">Fix typo in az aks update command</span></span>
* <span data-ttu-id="15ad5-258">Änderung, um einen Agentpool mit 0 Knoten zu unterstützen und die manuelle Skalierung für einen Pool mit CAS-Aktivierung zu blockieren</span><span class="sxs-lookup"><span data-stu-id="15ad5-258">Change to support 0 node agent pool and block manual scale for CAS enabled pool</span></span>
* <span data-ttu-id="15ad5-259">Tippfehler in VirtualMachineScaleSets korrigiert und Verweise auf Kubernetes-Versionen aktualisiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-259">Fix typo on VirtualMachineScaleSets and update references to Kubernetes versions</span></span>

### <a name="ams"></a><span data-ttu-id="15ad5-260">AMS</span><span class="sxs-lookup"><span data-stu-id="15ad5-260">AMS</span></span>

* <span data-ttu-id="15ad5-261">ÄNDERUNG: Hilfetext für Parameter „--expiry“</span><span class="sxs-lookup"><span data-stu-id="15ad5-261">CHANGE help text for "--expiry" parameter.</span></span>

### <a name="appservice"></a><span data-ttu-id="15ad5-262">AppService</span><span class="sxs-lookup"><span data-stu-id="15ad5-262">AppService</span></span>

* <span data-ttu-id="15ad5-263">`az webapp log deployment show`: Anzeigen des aktuellen Bereitstellungsprotokolls oder der Bereitstellungsprotokolle einer bestimmten Bereitstellung, wenn die Bereitstellungs-ID angegeben ist</span><span class="sxs-lookup"><span data-stu-id="15ad5-263">`az webapp log deployment show`: Show the latest deployment log, or the deployment logs of a specific deployment if deployment-id is specified</span></span>
* <span data-ttu-id="15ad5-264">`az webapp log deployment list`: Liste der verfügbaren Bereitstellungsprotokolle</span><span class="sxs-lookup"><span data-stu-id="15ad5-264">`az webapp log deployment list`: List of deployment logs available</span></span>
* <span data-ttu-id="15ad5-265">Behebung: Oberflächenfehler bei Angabe eines ungültigen Web-App-Namens</span><span class="sxs-lookup"><span data-stu-id="15ad5-265">Fix: Surface error when invalid webapp name provided</span></span>
* <span data-ttu-id="15ad5-266">Nr. 13261 korrigiert: „az webapp list-runtimes“ nutzt eine statische Liste, bis die neue API für verfügbare Stapel zur Verfügung steht</span><span class="sxs-lookup"><span data-stu-id="15ad5-266">Fix #13261 az webapp list-runtimes use static list until new Available Stacks API is available</span></span>
* <span data-ttu-id="15ad5-267">`az appservice ase create`: Erstellungsproblem behoben (Nr. 13361)</span><span class="sxs-lookup"><span data-stu-id="15ad5-267">`az appservice ase create`: Fix create issue #13361</span></span>
* <span data-ttu-id="15ad5-268">`az appservice ase list-addresses`: SDK-Änderung korrigiert (Nr. 13140)</span><span class="sxs-lookup"><span data-stu-id="15ad5-268">`az appservice ase list-addresses`: Fix change of SDK #13140.</span></span>
* <span data-ttu-id="15ad5-269">Web-App-/Sloterstellung für Windows-Container korrigiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-269">Fix webapp/slot creation for Windows Containers</span></span>
* <span data-ttu-id="15ad5-270">`az webapp auth update`: Optionaler Parameter zum Aktualisieren der Laufzeitversion hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-270">`az webapp auth update`: Add optional parameter to update runtime-version</span></span>
* <span data-ttu-id="15ad5-271">Unterstützung für das Auflisten, Löschen, Genehmigen und Ablehnen der Verbindung mit privatem Endpunkt für eine Web-App in der CLI</span><span class="sxs-lookup"><span data-stu-id="15ad5-271">Support list, delete, approve and reject private endpoint connection for webapp in CLI</span></span>
* <span data-ttu-id="15ad5-272">Behebung Nr. 13888: Unterstützung für Static Web Apps hinzugefügt: Befehle zum Abrufen, Auflisten und Erstellen</span><span class="sxs-lookup"><span data-stu-id="15ad5-272">Fix #13888 : Add support for Static WebApps: get, list, create commands</span></span>
* <span data-ttu-id="15ad5-273">Fehlermeldungen für die SSH-Tunnelverbindung verbessert</span><span class="sxs-lookup"><span data-stu-id="15ad5-273">Improved error messages for SSH Tunnel Connection</span></span>

### <a name="arm"></a><span data-ttu-id="15ad5-274">ARM</span><span class="sxs-lookup"><span data-stu-id="15ad5-274">ARM</span></span>

* <span data-ttu-id="15ad5-275">`az tag`: Beispiele für „-h“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-275">`az tag`: Add examples for -h</span></span>
* <span data-ttu-id="15ad5-276">`az deployment group/sub what-if`: Parameter „--exclude-change-types/-x“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-276">`az deployment group/sub what-if`: Add --exclude-change-types/-x parameter.</span></span>
* <span data-ttu-id="15ad5-277">`az deployment group/sub/mg/tenant create`: Parameter „--what-if-exclude-change-types/-x“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-277">`az deployment group/sub/mg/tenant create`: Add --what-if-exclude-change-types/-x parameter.</span></span>
* <span data-ttu-id="15ad5-278">`az deployment group/sub/mg/tenant validate`: Anzeigen von Fehlermeldungen in einem besseren Format</span><span class="sxs-lookup"><span data-stu-id="15ad5-278">`az deployment group/sub/mg/tenant validate`: Show error messages in a better format.</span></span>
* <span data-ttu-id="15ad5-279">`az group export`: Neue Parameter `--skip-resource-name-params` und `--skip-all-params` hinzugefügt, um das Überspringen der Parametrisierung zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="15ad5-279">`az group export`: Add new parameters `--skip-resource-name-params` and `--skip-all-params` to support skip parameterization</span></span>
* <span data-ttu-id="15ad5-280">API „az feature unregister“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-280">Add az feature unregister api</span></span>

### <a name="aro"></a><span data-ttu-id="15ad5-281">ARO</span><span class="sxs-lookup"><span data-stu-id="15ad5-281">ARO</span></span>

* <span data-ttu-id="15ad5-282">„Public“/„Private“ zu Parametern zur Unterstützung bei Eingangs-/APIServer-Sichtbarkeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-282">Add Public, Private to params for help with ingress/apiserver visibility</span></span>

### <a name="batch"></a><span data-ttu-id="15ad5-283">Batch</span><span class="sxs-lookup"><span data-stu-id="15ad5-283">Batch</span></span>

* <span data-ttu-id="15ad5-284">`az batch account create`: Neuer Parameter `--public-network-access` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-284">`az batch account create`: Add new parameter `--public-network-access`</span></span>
* <span data-ttu-id="15ad5-285">`az batch account create`: Neuer Parameter `--identity-type` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-285">`az batch account create`: Add new parameter `--identity-type`</span></span>
* <span data-ttu-id="15ad5-286">`az batch account set`: Neuer Parameter `--identity-type` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-286">`az batch account set`: Add new parameter `--identity-type`</span></span>
* <span data-ttu-id="15ad5-287">[BREAKING CHANGE] az batch pool create: Bei der Erstellung eines Pools mithilfe eines benutzerdefinierten Images kann die Eigenschaft „--image“ nun ausschließlich auf ein Shared Image Gallery-Image verweisen.</span><span class="sxs-lookup"><span data-stu-id="15ad5-287">[BREAKING CHANGE] az batch pool create: When creating a pool using a custom image, the --image property of can now only refer to a Shared Image Gallery image.</span></span>
* <span data-ttu-id="15ad5-288">[BREAKING CHANGE] az batch pool create: Bei der Erstellung eines Pools mit der Option „--json-file“ und Angabe einer Netzwerkkonfiguration (networkConfiguration) wurde die Eigenschaft „publicIPs“ in die neue Eigenschaft „publicIPAddressConfiguration“ verschoben.</span><span class="sxs-lookup"><span data-stu-id="15ad5-288">[BREAKING CHANGE] az batch pool create: When creating a pool with --json-file option and specifying a networkConfiguration, the publicIPs property has moved in to a new property publicIPAddressConfiguration.</span></span> <span data-ttu-id="15ad5-289">Diese neue Eigenschaft unterstützt außerdem die neue Eigenschaft „ipAddressProvisioningType“. Diese gibt an, wie der Pool IP-Adressen und die Eigenschaft „publicIPs“ zuordnen muss, um die Konfiguration einer Liste mit PublicIP-Ressourcen zu ermöglichen, die bei der Festlegung von „ipAddressProvisioningType“ auf „UserManaged“ verwendet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="15ad5-289">This new property also supports a new ipAddressProvisioningType property which specifies how the pool should allocate IP's and a publicIPs property which allows for configuration of a list of PublicIP resources to use in the case ipAddressProvisioningType is set to UserManaged</span></span>
* <span data-ttu-id="15ad5-290">`az network private-link-resource`: Unterstützung für die Microsoft.Batch-Ressource „batchAccount“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-290">`az network private-link-resource`: Add support for the Microsoft.Batch batchAccount resource</span></span>
* <span data-ttu-id="15ad5-291">`az network private-endpoint-connection`: Unterstützung für die Microsoft.Batch-Ressource „batchAccount“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-291">`az network private-endpoint-connection`: Add support for the Microsoft.Batch batchAccount resource</span></span>

### <a name="cdn"></a><span data-ttu-id="15ad5-292">CDN</span><span class="sxs-lookup"><span data-stu-id="15ad5-292">CDN</span></span>

* <span data-ttu-id="15ad5-293">`az cdn custom-domain enable-https`: Unterstützung für BYOC hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-293">`az cdn custom-domain enable-https`: Add BYOC support.</span></span>
* <span data-ttu-id="15ad5-294">`az cdn custom-domain enable-https`: Aktivierung von benutzerdefiniertem HTTPS mit CDN-verwalteten Zertifikaten für die SKUs Standard_Verizon und Standard_Microsoft korrigiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-294">`az cdn custom-domain enable-https`: Fix enabling custom HTTPS with CDN managed certificates for Standard_Verizon and Standard_Microsoft SKUs.</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="15ad5-295">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="15ad5-295">Cognitive Services</span></span>

* <span data-ttu-id="15ad5-296">[BREAKING CHANGE] `az cognitiveservices account` besitzt nun eine einheitliche Struktur für alle Befehle.</span><span class="sxs-lookup"><span data-stu-id="15ad5-296">[BREAKING CHANGE] `az cognitiveservices account` now have a unified structure for all commands.</span></span>
* <span data-ttu-id="15ad5-297">`az cognitiveservices account identity`: Identitätsverwaltung für Cognitive Services hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-297">`az cognitiveservices account identity`: Add identity management for Cognitive Services.</span></span>

### <a name="compute"></a><span data-ttu-id="15ad5-298">Compute</span><span class="sxs-lookup"><span data-stu-id="15ad5-298">Compute</span></span>

* <span data-ttu-id="15ad5-299">`az image builder`: API-Version auf 2020-02-14 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-299">`az image builder`: Upgrade API version to 2020-02-14</span></span>
* <span data-ttu-id="15ad5-300">`az image builder create`: `--identity` zur Unterstützung der Identitätskonfiguration hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-300">`az image builder create`: Add `--identity` to support identity configuration</span></span>
* <span data-ttu-id="15ad5-301">`az image builder customizer add`: Unterstützung für Windows Update-Anpassung</span><span class="sxs-lookup"><span data-stu-id="15ad5-301">`az image builder customizer add`: Support Windows update customizer</span></span>
* <span data-ttu-id="15ad5-302">Neuer Befehl `az image builder cancel`</span><span class="sxs-lookup"><span data-stu-id="15ad5-302">New command `az image builder cancel`</span></span>
* <span data-ttu-id="15ad5-303">Anzeigen einer Warnung, wenn ein Benutzer eine VMSS bereitstellt, die an eine bestimmte (und nicht an die neueste) Imageversion angeheftet ist</span><span class="sxs-lookup"><span data-stu-id="15ad5-303">Show a warning when a user deploys a VMSS pinned to a specific image version rather than latest</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="15ad5-304">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="15ad5-304">Cosmos DB</span></span>

* <span data-ttu-id="15ad5-305">`az cosmosdb`: Befehl „exists“ zu Datenbank- und Containergruppen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-305">`az cosmosdb`: Add exists command to database and container groups</span></span>
* <span data-ttu-id="15ad5-306">Zulassen der Erstellung fester Sammlungen</span><span class="sxs-lookup"><span data-stu-id="15ad5-306">Allow creating fixed collections</span></span>

### <a name="eventhub"></a><span data-ttu-id="15ad5-307">EventHub</span><span class="sxs-lookup"><span data-stu-id="15ad5-307">EventHub</span></span>

* <span data-ttu-id="15ad5-308">`az eventhubs namespace create` : Parameter für verwaltete Identität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-308">`az eventhubs namespace create` : Add managed identity parameters</span></span>

### <a name="extension"></a><span data-ttu-id="15ad5-309">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="15ad5-309">Extension</span></span>

* <span data-ttu-id="15ad5-310">„--version“ hinzugefügt, um die Installation über eine bestimmte Version zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="15ad5-310">Add --version to support to install from a specific version</span></span>
* <span data-ttu-id="15ad5-311">CLI-Erweiterungen dürfen nun Pakete im Namespace „azure“ enthalten.</span><span class="sxs-lookup"><span data-stu-id="15ad5-311">Enable CLI extensions to include packages in the 'azure' namespace</span></span>

### <a name="iot-hub"></a><span data-ttu-id="15ad5-312">IoT Hub</span><span class="sxs-lookup"><span data-stu-id="15ad5-312">Iot Hub</span></span>

* <span data-ttu-id="15ad5-313">[BREAKING CHANGE] az iot hub job: Veraltete job-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-313">[BREAKING CHANGE] az iot hub job: Remove deprecated job commands</span></span>

### <a name="keyvault"></a><span data-ttu-id="15ad5-314">KeyVault</span><span class="sxs-lookup"><span data-stu-id="15ad5-314">KeyVault</span></span>

* <span data-ttu-id="15ad5-315">`az keyvault key import`: Unterstützt das Importieren aus Zeichenfolgen über zwei neue Parameter.</span><span class="sxs-lookup"><span data-stu-id="15ad5-315">`az keyvault key import`: Supports importing from strings via two new parameters.</span></span>
* <span data-ttu-id="15ad5-316">Unterstützung der Ver- und Entschlüsselung von Zeichenfolgen/Bytes mit gespeicherten Schlüsseln</span><span class="sxs-lookup"><span data-stu-id="15ad5-316">Support string/bytes encryption and decryption with stored keys</span></span>

### <a name="monitor"></a><span data-ttu-id="15ad5-317">Überwachen</span><span class="sxs-lookup"><span data-stu-id="15ad5-317">Monitor</span></span>

* <span data-ttu-id="15ad5-318">Unterstützung für „no wait“ bei der Clustererstellung</span><span class="sxs-lookup"><span data-stu-id="15ad5-318">Support no wait for cluster creation</span></span>
* <span data-ttu-id="15ad5-319">`az monitor log-analytics workspace saved-search`: Unterstützung neuer Befehle für gespeicherte Suche</span><span class="sxs-lookup"><span data-stu-id="15ad5-319">`az monitor log-analytics workspace saved-search`: Support new commands for saved search</span></span>

### <a name="network"></a><span data-ttu-id="15ad5-320">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="15ad5-320">Network</span></span>

* <span data-ttu-id="15ad5-321">`az network application-gateway address-pool update`: Hilfenachricht optimiert und Beispiele hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-321">`az network application-gateway address-pool update`: Refine help message and add examples.</span></span>
* <span data-ttu-id="15ad5-322">`az network vnet create`: Unterstützung für das Argument „--nsg“</span><span class="sxs-lookup"><span data-stu-id="15ad5-322">`az network vnet create`: Support --nsg argument</span></span>
* <span data-ttu-id="15ad5-323">`az network lb address-pool`: Unterstützung für das Erstellen eines Back-End-Pools des Lastenausgleichs mit Back-End-Adresse</span><span class="sxs-lookup"><span data-stu-id="15ad5-323">`az network lb address-pool`: Support create lb backend pool with backend address.</span></span>
* <span data-ttu-id="15ad5-324">`az network application-gateway address-pool`: Korrektur für das Argument „--add“</span><span class="sxs-lookup"><span data-stu-id="15ad5-324">`az network application-gateway address-pool`: Fix for --add argument</span></span>

### <a name="rbac"></a><span data-ttu-id="15ad5-325">RBAC</span><span class="sxs-lookup"><span data-stu-id="15ad5-325">RBAC</span></span>

* <span data-ttu-id="15ad5-326">`az ad sp create-for-rabc`: Unterstützung von Namen mit Leerzeichen, Schrägstrich und umgekehrtem Schrägstrich</span><span class="sxs-lookup"><span data-stu-id="15ad5-326">`az ad sp create-for-rabc`: Support name with space, slash and back slash</span></span>
* <span data-ttu-id="15ad5-327">`az ad sp create-for-rbac`: Fehlermeldung optimiert, die angezeigt wird, wenn Benutzer einen ungültigen Bereich angeben</span><span class="sxs-lookup"><span data-stu-id="15ad5-327">`az ad sp create-for-rbac`: Refine error message when user specify an invalid scope</span></span>

### <a name="security"></a><span data-ttu-id="15ad5-328">Sicherheit</span><span class="sxs-lookup"><span data-stu-id="15ad5-328">Security</span></span>

* <span data-ttu-id="15ad5-329">Befehle für Sicherheitsbewertungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-329">Add security assessment commands</span></span>

### <a name="sql"></a><span data-ttu-id="15ad5-330">SQL</span><span class="sxs-lookup"><span data-stu-id="15ad5-330">SQL</span></span>

* <span data-ttu-id="15ad5-331">`az sql db ltr-policy/ltr-backup`: Aktualisieren/Anzeigen der Richtlinie zur langfristigen Aufbewahrung, Anzeigen/Löschen von Sicherungen zur langfristigen Aufbewahrung, Wiederherstellen von Sicherungen zur langfristigen Aufbewahrung</span><span class="sxs-lookup"><span data-stu-id="15ad5-331">`az sql db ltr-policy/ltr-backup`: update/show long term retention policy, show/delete long term retention backups, restore long term retention backup</span></span>

### <a name="storage"></a><span data-ttu-id="15ad5-332">Storage</span><span class="sxs-lookup"><span data-stu-id="15ad5-332">Storage</span></span>

* <span data-ttu-id="15ad5-333">Authentifizierungsproblem behoben, um das Abrufen eines Tokens für „--subscription“ zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="15ad5-333">Fix authentication issue to support get token for --subscription</span></span>
* <span data-ttu-id="15ad5-334">`az storage remove`: Problem Nr. 13459 behoben, um eine Ausnahme bei einem Vorgangsfehler auszulösen</span><span class="sxs-lookup"><span data-stu-id="15ad5-334">`az storage remove`: Fix issue #13459 to raise exception for operation failure</span></span>
* <span data-ttu-id="15ad5-335">Probleme Nr. 13012, 13632 und 13657 behoben, um nicht verwendete Argumente für Befehle im Zusammenhang mit „generate-sas“ zu entfernen</span><span class="sxs-lookup"><span data-stu-id="15ad5-335">Fix issues #13012, #13632 and #13657 to remove unused arguments for generate-sas related commands</span></span>
* <span data-ttu-id="15ad5-336">`az storage logging update`: Überprüfung für Protokollierungsversion hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-336">`az storage logging update`: Add check for logging version</span></span>
* <span data-ttu-id="15ad5-337">`az storage blob show`: Weitere Eigenschaften für Blob mit Track 2 SDK hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-337">`az storage blob show`: Add more properties for blob with track 2 SDK</span></span>
* <span data-ttu-id="15ad5-338">Behebung Nr. 13708: Warnmeldung für Anmeldeinformationen optimiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-338">Fix #13708: Refine warning message for credential</span></span>
* <span data-ttu-id="15ad5-339">`az storage share-rm create/update`: Unterstützung für NFS-Protokoll und Root-Squash hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-339">`az storage share-rm create/update`: Add NFS protocol and root squash support</span></span>
* <span data-ttu-id="15ad5-340">`az storage account create`: Unterstützung für doppelte Verschlüsselung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-340">`az storage account create`: Add support for double encryption</span></span>
* <span data-ttu-id="15ad5-341">[BREAKING CHANGE] `az storage blob/container/file/share/table/queue generate-sas`: „--expiry“ und „--permissions“ als erforderlich festgelegt</span><span class="sxs-lookup"><span data-stu-id="15ad5-341">[BREAKING CHANGE] `az storage blob/container/file/share/table/queue generate-sas`: make --expiry and --permissions required</span></span>
* <span data-ttu-id="15ad5-342">`az storage blob set-tier`: Migration zu Track 2, um das Festlegen der Aktivierungspriorität zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="15ad5-342">`az storage blob set-tier`: Migrate to Track 2 to support setting rehydrate priority</span></span>

## <a name="june-02-2020"></a><span data-ttu-id="15ad5-343">2\. Juni 2020</span><span class="sxs-lookup"><span data-stu-id="15ad5-343">June 02, 2020</span></span>

<span data-ttu-id="15ad5-344">Version 2.7.0</span><span class="sxs-lookup"><span data-stu-id="15ad5-344">Version 2.7.0</span></span>

### <a name="acr"></a><span data-ttu-id="15ad5-345">ACR</span><span class="sxs-lookup"><span data-stu-id="15ad5-345">ACR</span></span>

* <span data-ttu-id="15ad5-346">Tippfehler in einer Fehlermeldung der Tokenerstellung korrigiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-346">Fix a typo in an error message of token creation</span></span>

### <a name="aks"></a><span data-ttu-id="15ad5-347">AKS</span><span class="sxs-lookup"><span data-stu-id="15ad5-347">AKS</span></span>

* <span data-ttu-id="15ad5-348">Standard-VM-SKU in „Standard_D2s_v3“ geändert</span><span class="sxs-lookup"><span data-stu-id="15ad5-348">Change default vm sku to Standard_D2s_v3</span></span>
* <span data-ttu-id="15ad5-349">Erstellung der Rollenzuweisung für MSI-Cluster plus benutzerdefiniertes Subnetz korrigiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-349">Fix creating role assignment for MSI clsuter plus custom subnet</span></span>

### <a name="appservice"></a><span data-ttu-id="15ad5-350">AppService</span><span class="sxs-lookup"><span data-stu-id="15ad5-350">AppService</span></span>

* <span data-ttu-id="15ad5-351">Fehlerbehebung Nr. 12739: Von „az appservice list-locations“ werden einige ungültige Standorte zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="15ad5-351">Fix #12739 az appservice list-locations returns some invalid locations</span></span>

### <a name="arm"></a><span data-ttu-id="15ad5-352">ARM</span><span class="sxs-lookup"><span data-stu-id="15ad5-352">ARM</span></span>

* <span data-ttu-id="15ad5-353">`az deployment`: Fehlerbehebung Nr. 13159 der fehlerhaften JSON-Meldung nach dem Entfernen von Kommentaren und nach dem Komprimieren</span><span class="sxs-lookup"><span data-stu-id="15ad5-353">`az deployment`: Fix issue #13159 of incorrect message of JSON after removing comments and compressing</span></span>
* <span data-ttu-id="15ad5-354">`az resource tag`: Fehlerbehebung Nr. 13255 für das Markieren von Ressourcen mit dem Ressourcentyp `Microsoft.ContainerRegistry/registries/webhooks`</span><span class="sxs-lookup"><span data-stu-id="15ad5-354">`az resource tag`: Fix issue #13255 of tagging resources with resource type `Microsoft.ContainerRegistry/registries/webhooks`</span></span>
* <span data-ttu-id="15ad5-355">Beispiele für das Ressourcenmodul verbessert</span><span class="sxs-lookup"><span data-stu-id="15ad5-355">Improve the examples for the resource module</span></span>

### <a name="aro"></a><span data-ttu-id="15ad5-356">ARO</span><span class="sxs-lookup"><span data-stu-id="15ad5-356">ARO</span></span>

* <span data-ttu-id="15ad5-357">CLIError in das richtige Flag für „--worker-vm-disk-size-gb“ geändert</span><span class="sxs-lookup"><span data-stu-id="15ad5-357">Change CLIError to correct flag for --worker-vm-disk-size-gb</span></span>

### <a name="eventhub"></a><span data-ttu-id="15ad5-358">EventHub</span><span class="sxs-lookup"><span data-stu-id="15ad5-358">EventHub</span></span>

* <span data-ttu-id="15ad5-359">Fehlerbehebung Nr. 12406: „intervalInSeconds“ wird von Argument „--capture-interval“ nicht aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="15ad5-359">Fix for issue #12406 Argument --capture-interval does not update the "intervalInSeconds"</span></span>

### <a name="hdinsight"></a><span data-ttu-id="15ad5-360">HDInsight</span><span class="sxs-lookup"><span data-stu-id="15ad5-360">HDInsight</span></span>

* <span data-ttu-id="15ad5-361">„get_json_object“ in „shell_safe_json_parse“ geändert</span><span class="sxs-lookup"><span data-stu-id="15ad5-361">Change get_json_object to shell_safe_json_parse</span></span>

### <a name="monitor"></a><span data-ttu-id="15ad5-362">Überwachen</span><span class="sxs-lookup"><span data-stu-id="15ad5-362">Monitor</span></span>

* <span data-ttu-id="15ad5-363">`az monitor metrics alert`: Verschiedene Hilfemeldungen optimiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-363">`az monitor metrics alert`: refine several help messages</span></span>
* <span data-ttu-id="15ad5-364">`az monitor diagnostic-settings create`: Unterstützung für das Argument „--export-to-resource-specific“</span><span class="sxs-lookup"><span data-stu-id="15ad5-364">`az monitor diagnostic-settings create`: support --export-to-resource-specific argument</span></span>
* <span data-ttu-id="15ad5-365">Unterstützung für die Wiederherstellung von LA-Arbeitsbereichen</span><span class="sxs-lookup"><span data-stu-id="15ad5-365">Support LA workspace recover</span></span>

### <a name="network"></a><span data-ttu-id="15ad5-366">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="15ad5-366">Network</span></span>

* <span data-ttu-id="15ad5-367">`az network dns zone`: Unterstützung des Bindestrichs (-)</span><span class="sxs-lookup"><span data-stu-id="15ad5-367">`az network dns zone`: support - character</span></span>
* <span data-ttu-id="15ad5-368">`az network vpn-connection ipsec-policy`: „--sa-lifetime“ und „--sa-max-size“ im Beispiel in höhere Werte geändert</span><span class="sxs-lookup"><span data-stu-id="15ad5-368">`az network vpn-connection ipsec-policy`: change the --sa-lifetime and --sa-max-size to larger values in example</span></span>
* <span data-ttu-id="15ad5-369">Netzwerk auf 2020-04-01 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-369">Bump network to 2020-04-01</span></span>
* <span data-ttu-id="15ad5-370">`az network private-endpoint-connection`: Unterstützung von Event Grid</span><span class="sxs-lookup"><span data-stu-id="15ad5-370">`az network private-endpoint-connection`: support event grid</span></span>
* <span data-ttu-id="15ad5-371">`az network express-route list-route-tables`: Fehler behoben, der dazu führte, dass Routen nicht als Tabelle aufgeführt werden konnten</span><span class="sxs-lookup"><span data-stu-id="15ad5-371">`az network express-route list-route-tables`: fix bug that cannot list routes as table</span></span>

### <a name="packaging"></a><span data-ttu-id="15ad5-372">Verpackung</span><span class="sxs-lookup"><span data-stu-id="15ad5-372">Packaging</span></span>

* <span data-ttu-id="15ad5-373">Ubuntu-Paket (Focal) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-373">Add Ubuntu Focal Package</span></span>

### <a name="rbac"></a><span data-ttu-id="15ad5-374">RBAC</span><span class="sxs-lookup"><span data-stu-id="15ad5-374">RBAC</span></span>

* <span data-ttu-id="15ad5-375">`az ad sp credential reset`: Erstellung von Anmeldeinformationen geändert, um problematische Sonderzeichen zu vermeiden</span><span class="sxs-lookup"><span data-stu-id="15ad5-375">`az ad sp credential reset`: modify credential generation to avoid troublesome special characters</span></span>

### <a name="redis"></a><span data-ttu-id="15ad5-376">Redis</span><span class="sxs-lookup"><span data-stu-id="15ad5-376">Redis</span></span>

* <span data-ttu-id="15ad5-377">Fehlerbehebung Nr. 13529: Dokumentation des Parameters „enable_non_ssl_port“ geändert</span><span class="sxs-lookup"><span data-stu-id="15ad5-377">Fix #13529: Change documentation of parameter enable_non_ssl_port</span></span>

### <a name="storage"></a><span data-ttu-id="15ad5-378">Storage</span><span class="sxs-lookup"><span data-stu-id="15ad5-378">Storage</span></span>

* <span data-ttu-id="15ad5-379">`az storage copy`: Parameter `--follow-symlinks` zur Unterstützung von symbolischen Verknüpfungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-379">`az storage copy`: Add parameter `--follow-symlinks` to support symlinks</span></span>
* <span data-ttu-id="15ad5-380">Lokaler Kontext für Speicherkonto aktiviert</span><span class="sxs-lookup"><span data-stu-id="15ad5-380">Enable local context for storage account</span></span>
* <span data-ttu-id="15ad5-381">`az storage logging`: Fehlerbehebung Nr. 11969: Fehlermeldung optimiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-381">`az storage logging`: Fix issue #11969 to refine error message</span></span>

## <a name="may-19-2020"></a><span data-ttu-id="15ad5-382">19. Mai 2020</span><span class="sxs-lookup"><span data-stu-id="15ad5-382">May 19, 2020</span></span>

<span data-ttu-id="15ad5-383">Version 2.6.0</span><span class="sxs-lookup"><span data-stu-id="15ad5-383">Version 2.6.0</span></span>

### <a name="acr"></a><span data-ttu-id="15ad5-384">ACR</span><span class="sxs-lookup"><span data-stu-id="15ad5-384">ACR</span></span>

* <span data-ttu-id="15ad5-385">Standardtimeout von fünf Minuten für jede an ACR gesendete Anforderung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-385">Add default timeout of 5 minutes for any requests to ACR</span></span>
* <span data-ttu-id="15ad5-386">Unterstützung für das Deaktivieren des Zugriffs auf das öffentliche Netzwerk</span><span class="sxs-lookup"><span data-stu-id="15ad5-386">Support disable public network access</span></span>
* <span data-ttu-id="15ad5-387">`az acr token create`: Argument „--days“ verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="15ad5-387">`az acr token create`: expose --days argument</span></span>
* <span data-ttu-id="15ad5-388">`az acr import`: Akzeptiert Werte für das Argument „--source“, bei denen der Servername einen Anmeldenamen enthält (mittels clientseitiger Korrektur)</span><span class="sxs-lookup"><span data-stu-id="15ad5-388">`az acr import`: accept --source argument values which contain login in server name through client end correction</span></span>

### <a name="acs"></a><span data-ttu-id="15ad5-389">ACS</span><span class="sxs-lookup"><span data-stu-id="15ad5-389">ACS</span></span>

* <span data-ttu-id="15ad5-390">Fehlerbehebung: Felderbereinigung für Felder entfernt, die nicht mehr vorhanden sind</span><span class="sxs-lookup"><span data-stu-id="15ad5-390">Bug fix: remove fields cleanup for fields that no longer exist</span></span>

### <a name="aks"></a><span data-ttu-id="15ad5-391">AKS</span><span class="sxs-lookup"><span data-stu-id="15ad5-391">AKS</span></span>

* <span data-ttu-id="15ad5-392">Hilfekontext des Befehls „uptime-sla“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-392">Update uptime-sla command help context</span></span>
* <span data-ttu-id="15ad5-393">Bereichsüberprüfung für die Aktualisierung der Mindestanzahl für die Autoskalierung entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-393">Remove range check for updating min count for autoscaler</span></span>
* <span data-ttu-id="15ad5-394">Hotfix, der bewirkt, dass bei der CLI kein Fehler auftritt, wenn der Benutzer nur das Windows-Kennwort angibt</span><span class="sxs-lookup"><span data-stu-id="15ad5-394">Fix that cli doe not fail when user only specifies Windows password</span></span>

### <a name="ams"></a><span data-ttu-id="15ad5-395">AMS</span><span class="sxs-lookup"><span data-stu-id="15ad5-395">AMS</span></span>

* <span data-ttu-id="15ad5-396">`az ams transform create`: Funktion zum Erstellen einer Transformation mit einer FaceDetector-Voreinstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-396">`az ams transform create`: Add ability to create a transform with a FaceDetector preset</span></span>
* <span data-ttu-id="15ad5-397">`az ams content-key-policy create` : Funktion zum Erstellen einer FairPlay-Inhaltsschlüsselrichtlinie mit einer Konfiguration für die Offlinemiete hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-397">`az ams content-key-policy create` : Add ability to create a FairPlay content key policy with an offline rental configuration</span></span>

### <a name="appconfig"></a><span data-ttu-id="15ad5-398">AppConfig</span><span class="sxs-lookup"><span data-stu-id="15ad5-398">AppConfig</span></span>

* <span data-ttu-id="15ad5-399">Fehlerbehebung für die Schlüsselauflistungswerte mit Feldern</span><span class="sxs-lookup"><span data-stu-id="15ad5-399">Bug fix for list key values with fields</span></span>

### <a name="appservice"></a><span data-ttu-id="15ad5-400">AppService</span><span class="sxs-lookup"><span data-stu-id="15ad5-400">AppService</span></span>

* <span data-ttu-id="15ad5-401">`az functionapp create`: AzureWebJobsDashboard wird nur festgelegt, wenn AppInsights deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="15ad5-401">`az functionapp create`: AzureWebJobsDashboard will only be set if AppInsights is disabled</span></span>
* <span data-ttu-id="15ad5-402">Fehlerbehebung Nr. 10664: VNET-Integration – Standortüberprüfungsfehler und Fehlerbehebung Nr. 13257: Fehler bei „az webapp up“, wenn eine Ressourcengruppe erstellt werden muss</span><span class="sxs-lookup"><span data-stu-id="15ad5-402">Fix #10664- VNet Integration - Location Check Issue & fix #13257- az webapp up failing when RG needs to be created</span></span>
* <span data-ttu-id="15ad5-403">`az webapp|functionapp config ssl import`: Ressourcengruppenübergreifende Suche des Schlüsseltresors im Abonnement und verbesserte Hilfe und Beispiele</span><span class="sxs-lookup"><span data-stu-id="15ad5-403">`az webapp|functionapp config ssl import`: Lookup key vault across resources groups in subscription and improve help and examples.</span></span>
* <span data-ttu-id="15ad5-404">Lokaler Kontext für App Service integriert</span><span class="sxs-lookup"><span data-stu-id="15ad5-404">Onboard local context for app service</span></span>

### <a name="arm"></a><span data-ttu-id="15ad5-405">ARM</span><span class="sxs-lookup"><span data-stu-id="15ad5-405">ARM</span></span>

* <span data-ttu-id="15ad5-406">`az deployment`: Problem behoben, das dazu führte, dass templateLink beim Bereitstellen oder Überprüfen von „template-uri“ nicht zurückgegeben wurde</span><span class="sxs-lookup"><span data-stu-id="15ad5-406">`az deployment`: Fix the problem that the templateLink will not be returned when deploying or validating template-uri</span></span>
* <span data-ttu-id="15ad5-407">`az deployment`: Problem behoben, das dazu führte, dass speziell codierte Zeichen von der Bereitstellung/Überprüfung nicht unterstützt wurden</span><span class="sxs-lookup"><span data-stu-id="15ad5-407">`az deployment`: Fix the problem that deployment/validate does not support specially encoded character</span></span>
* <span data-ttu-id="15ad5-408">`az deployment sub/group what-if`: Arrayausrichtung und Fehlerbehandlung korrigiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-408">`az deployment sub/group what-if`: Fix array alignment and error handling</span></span>
* <span data-ttu-id="15ad5-409">`az deployment operation`: Veraltete Informationen angepasst</span><span class="sxs-lookup"><span data-stu-id="15ad5-409">`az deployment operation`: Modify the deprecate information</span></span>

### <a name="aro"></a><span data-ttu-id="15ad5-410">ARO</span><span class="sxs-lookup"><span data-stu-id="15ad5-410">ARO</span></span>

* <span data-ttu-id="15ad5-411">Beispiele zu folgenden Befehlen hinzugefügt: az aro create, list, list-credentials, show, delete</span><span class="sxs-lookup"><span data-stu-id="15ad5-411">Add examples to az aro create, list, list-credentials, show, delete</span></span>
* <span data-ttu-id="15ad5-412">Funktion „generate_random_id“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-412">Add generate_random_id function</span></span>

### <a name="backup"></a><span data-ttu-id="15ad5-413">Backup</span><span class="sxs-lookup"><span data-stu-id="15ad5-413">Backup</span></span>

* <span data-ttu-id="15ad5-414">FriendlyName im Befehl zum Aktivieren des Schutzes für AzureFileShare zulässig</span><span class="sxs-lookup"><span data-stu-id="15ad5-414">Allow FriendlyName in enable protection for AzureFileShare command</span></span>
* <span data-ttu-id="15ad5-415">Korrektur im IaasVM-Befehl „restore-disks“</span><span class="sxs-lookup"><span data-stu-id="15ad5-415">Fix in IaasVM restore-disks Command</span></span>
* <span data-ttu-id="15ad5-416">BackupManagementType „MAB“ zum Befehl zum Auflisten der Elemente hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-416">Add "MAB" BackupManagementType to item list command</span></span>
* <span data-ttu-id="15ad5-417">Unterstützung für die Wiederholung des Richtlinienupdates für fehlerhafte Elemente hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-417">Add support for retrying policy update for failed items.</span></span>
* <span data-ttu-id="15ad5-418">Funktion zum Fortsetzen des Schutzes für virtuelle Azure-Computer hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-418">Add Resume Protection functionality for Azure Virtual Machine</span></span>
* <span data-ttu-id="15ad5-419">Unterstützung zum Angeben der Ressourcengruppe zum Speichern von instantRP beim Erstellen oder Ändern der Richtlinie hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-419">Add support to specify ResourceGroup for storing instantRP during Create or Modify Policy</span></span>

### <a name="ci"></a><span data-ttu-id="15ad5-420">CI</span><span class="sxs-lookup"><span data-stu-id="15ad5-420">CI</span></span>

* <span data-ttu-id="15ad5-421">Unterstützung für flake8 3.8.0</span><span class="sxs-lookup"><span data-stu-id="15ad5-421">Support flake8 3.8.0</span></span>

### <a name="compute"></a><span data-ttu-id="15ad5-422">Compute</span><span class="sxs-lookup"><span data-stu-id="15ad5-422">Compute</span></span>

* <span data-ttu-id="15ad5-423">Neuer Befehl: az vm auto-shutdown</span><span class="sxs-lookup"><span data-stu-id="15ad5-423">New command az vm auto-shutdown</span></span>
* <span data-ttu-id="15ad5-424">`az vm list-skus`: Verhalten von „--zone“aktualisiert. Jetzt werden alle SKU-Typen zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="15ad5-424">`az vm list-skus`: Update --zone behavior, return all type skus now</span></span>

### <a name="core"></a><span data-ttu-id="15ad5-425">Core</span><span class="sxs-lookup"><span data-stu-id="15ad5-425">Core</span></span>

* <span data-ttu-id="15ad5-426">Aktivierungsstatus aus dem lokalen Kontext für globale Benutzerebene aktualisiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-426">Update local context on/off status to global user level</span></span>

### <a name="extension"></a><span data-ttu-id="15ad5-427">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="15ad5-427">Extension</span></span>

* <span data-ttu-id="15ad5-428">`az extension add`: „--system“ hinzugefügt, um die Installation von Erweiterungen in einem Systempfad zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="15ad5-428">`az extension add`: Add --system to enable installing extensions in a system path</span></span>
* <span data-ttu-id="15ad5-429">Unterstützung für „.egg-info“ zum Speichern der Metadaten für die Radtyperweiterung</span><span class="sxs-lookup"><span data-stu-id="15ad5-429">Support .egg-info to store wheel type extension metadata</span></span>

### <a name="iot"></a><span data-ttu-id="15ad5-430">IoT</span><span class="sxs-lookup"><span data-stu-id="15ad5-430">IoT</span></span>

* <span data-ttu-id="15ad5-431">`az iot`: Nachricht des IoT-Befehlsmoduls mit dem Hinweis auf die Erweiterung für die erste Ausführung aktualisiert, sodass sie anstelle der veralteten ID die korrekte moderne ID (`azure-iot`) enthält</span><span class="sxs-lookup"><span data-stu-id="15ad5-431">`az iot`: Update the IoT command module first run extension awareness message to the accurate, non-deprecated modern Id `azure-iot`.</span></span>

### <a name="iot-hub"></a><span data-ttu-id="15ad5-432">IoT Hub</span><span class="sxs-lookup"><span data-stu-id="15ad5-432">IoT Hub</span></span>

* <span data-ttu-id="15ad5-433">Unterstützung für API- und Netzwerkisolationsbefehle für 2020-03-01</span><span class="sxs-lookup"><span data-stu-id="15ad5-433">Support for 2020-03-01 API and Network Isolation commands</span></span>

### <a name="netappfiles"></a><span data-ttu-id="15ad5-434">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="15ad5-434">NetAppFiles</span></span>

* <span data-ttu-id="15ad5-435">`az volume create`: „snapshot-id“ als Parameter zum Erstellen eines Volumes hinzugefügt. Ermöglicht Benutzern das Erstellen eines Volumes auf der Grundlage einer vorhandenen Momentaufnahme.</span><span class="sxs-lookup"><span data-stu-id="15ad5-435">`az volume create`: Adds snapshot-id as a parameter to create volume this will allow users to create a volume from existing snapshot.</span></span>

### <a name="network"></a><span data-ttu-id="15ad5-436">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="15ad5-436">Network</span></span>

* <span data-ttu-id="15ad5-437">TTL-Wert korrigiert, der für „dns add-record“ unbeabsichtigt geändert wurde</span><span class="sxs-lookup"><span data-stu-id="15ad5-437">Fix ttl value changed unintended for dns add-record</span></span>
* <span data-ttu-id="15ad5-438">`az network public-ip create`: Kunden über einen bevorstehenden Breaking Change informiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-438">`az network public-ip create`: Inform customers of a coming breaking change</span></span>
* <span data-ttu-id="15ad5-439">Unterstützung von generischen Befehlen für Private Link-Szenario</span><span class="sxs-lookup"><span data-stu-id="15ad5-439">Support generic commands for private link scenario</span></span>
* <span data-ttu-id="15ad5-440">`az network private-endpoint-connection`: Unterstützung für MySQL-, Postgre- und MariaDB-Typen</span><span class="sxs-lookup"><span data-stu-id="15ad5-440">`az network private-endpoint-connection`: Support mysql, postgre and mariadb types</span></span>
* <span data-ttu-id="15ad5-441">`az network private-endpoint-connection`: Unterstützung von CosmosDB-Typen</span><span class="sxs-lookup"><span data-stu-id="15ad5-441">`az network private-endpoint-connection`: Support cosmosdb types</span></span>
* <span data-ttu-id="15ad5-442">`az network private-endpoint`: „--group-ids“ und Umleitung an „--group-id“ als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="15ad5-442">`az network private-endpoint`: deprecate --group-ids and redirect to --group-id</span></span>

### <a name="output"></a><span data-ttu-id="15ad5-443">Output</span><span class="sxs-lookup"><span data-stu-id="15ad5-443">Output</span></span>

* <span data-ttu-id="15ad5-444">Anzeigen der Updateanweisung bei der Suche, beim Feedback und in „--help“</span><span class="sxs-lookup"><span data-stu-id="15ad5-444">Show update instruction in find, feedback and --help</span></span>

### <a name="packaging"></a><span data-ttu-id="15ad5-445">Verpackung</span><span class="sxs-lookup"><span data-stu-id="15ad5-445">Packaging</span></span>

* <span data-ttu-id="15ad5-446">Erstellen von MSI-/Homebrew-Paketen mit Abhängigkeiten, die aus „requirements.txt“ aufgelöst werden</span><span class="sxs-lookup"><span data-stu-id="15ad5-446">Build MSI/Homebrew packages with dependecies resolved from requirements.txt</span></span>

### <a name="rbac"></a><span data-ttu-id="15ad5-447">RBAC</span><span class="sxs-lookup"><span data-stu-id="15ad5-447">RBAC</span></span>

* <span data-ttu-id="15ad5-448">`az ad sp credential reset`: Erstellung unsicherer Anmeldeinformationen korrigiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-448">`az ad sp credential reset`: fix weak credential generation</span></span>

### <a name="storage"></a><span data-ttu-id="15ad5-449">Storage</span><span class="sxs-lookup"><span data-stu-id="15ad5-449">Storage</span></span>

* <span data-ttu-id="15ad5-450">`az storage account file-service-properties update/show`: Unterstützung für Dateieigenschaften für Speicherkonto hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-450">`az storage account file-service-properties update/show`: Add File Properties Support for Storage Account</span></span>
* <span data-ttu-id="15ad5-451">`az storage container create`: Fehlerbehebung Nr. 13373 durch Hinzufügen eines Validierungssteuerelements für öffentlichen Zugriff</span><span class="sxs-lookup"><span data-stu-id="15ad5-451">`az storage container create`: Fix #13373 by adding validator for public access</span></span>
* <span data-ttu-id="15ad5-452">Unterstützung für ADLS Gen2 (track2) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-452">Add ADLS Gen2 track2 support</span></span>
* <span data-ttu-id="15ad5-453">`az storage blob sync`: Unterstützung für `--connection-string`</span><span class="sxs-lookup"><span data-stu-id="15ad5-453">`az storage blob sync`: Support `--connection-string`</span></span>
* <span data-ttu-id="15ad5-454">`az storage blob sync`: Falsche Fehlermeldung korrigiert, die angezeigt wird, wenn der Installationsspeicherort von „azcopy“ nicht gefunden wird</span><span class="sxs-lookup"><span data-stu-id="15ad5-454">`az storage blob sync`: Fix the incorrect error message when azcopy cannot find the installation location</span></span>

## <a name="april-30-2020"></a><span data-ttu-id="15ad5-455">30. April 2020</span><span class="sxs-lookup"><span data-stu-id="15ad5-455">April 30, 2020</span></span>

<span data-ttu-id="15ad5-456">Version 2.5.1</span><span class="sxs-lookup"><span data-stu-id="15ad5-456">Version 2.5.1</span></span>

### <a name="acr"></a><span data-ttu-id="15ad5-457">ACR</span><span class="sxs-lookup"><span data-stu-id="15ad5-457">ACR</span></span>

* <span data-ttu-id="15ad5-458">`az acr check-health`: „DOCKER_PULL_ERROR“ unter Windows behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-458">`az acr check-health`: Fix "DOCKER_PULL_ERROR" on Windows</span></span>

### <a name="compute"></a><span data-ttu-id="15ad5-459">Compute</span><span class="sxs-lookup"><span data-stu-id="15ad5-459">Compute</span></span>

* <span data-ttu-id="15ad5-460">`az vm list-ip-addresses`: Fehlerbehandlung</span><span class="sxs-lookup"><span data-stu-id="15ad5-460">`az vm list-ip-addresses`: Error handling</span></span>
* <span data-ttu-id="15ad5-461">Fehler behoben, der bei der VM-Erstellung auftrat, wenn „endpoint_vm_image_alias_doc“ im Cloudprofil nicht festgelegt war</span><span class="sxs-lookup"><span data-stu-id="15ad5-461">Fix a bug of vm create if endpoint_vm_image_alias_doc is not set in cloud profile</span></span>
* <span data-ttu-id="15ad5-462">`az vmss create`: „--os-disk-size-gb“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-462">`az vmss create`: Add --os-disk-size-gb</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="15ad5-463">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="15ad5-463">Cosmos DB</span></span>

* <span data-ttu-id="15ad5-464">`az cosmosdb create/update`: Unterstützung für „--enable-public-network“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-464">`az cosmosdb create/update`: add --enable-public-network support</span></span>

### <a name="extension"></a><span data-ttu-id="15ad5-465">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="15ad5-465">Extension</span></span>

* <span data-ttu-id="15ad5-466">Laden der falschen Metadaten für die Radtyperweiterung korrigiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-466">Fix loading wrong metadata for wheel type extension</span></span>

### <a name="packaging"></a><span data-ttu-id="15ad5-467">Verpackung</span><span class="sxs-lookup"><span data-stu-id="15ad5-467">Packaging</span></span>

* <span data-ttu-id="15ad5-468">Az-Skript für Git Bash/Cygwin unter Windows hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-468">Add az script for Git Bash/Cygwin on Windows</span></span>

### <a name="sql"></a><span data-ttu-id="15ad5-469">SQL</span><span class="sxs-lookup"><span data-stu-id="15ad5-469">SQL</span></span>

* <span data-ttu-id="15ad5-470">`az sql instance-pool`: Befehlsgruppe für Instanzpools hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-470">`az sql instance-pool`: Add instance pools command group</span></span>

### <a name="storage"></a><span data-ttu-id="15ad5-471">Storage</span><span class="sxs-lookup"><span data-stu-id="15ad5-471">Storage</span></span>

* <span data-ttu-id="15ad5-472">Paket „azure-multiapi-storage“ auf 0.3.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-472">Upgrade package azure-multiapi-storage to 0.3.0</span></span>
* <span data-ttu-id="15ad5-473">Unterstützung von GZRS für Speicherkontoerstellung und -aktualisierung</span><span class="sxs-lookup"><span data-stu-id="15ad5-473">Support GZRS for storage account creation and update</span></span>
* <span data-ttu-id="15ad5-474">`az storage account failover`: Unterstützung für das Failover von GRS/GZRS-Speicherkonten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-474">`az storage account failover`: Add support for grs/gzrs storage account failover</span></span>
* <span data-ttu-id="15ad5-475">`az storage blob upload`: Parameter „--encryption-scope“ hinzugefügt, um die Angabe von Informationen zum Verschlüsselungsbereich zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="15ad5-475">`az storage blob upload`: Add --encryption-scope parameter to support specifying encryption scope information</span></span>

## <a name="april-28-2020"></a><span data-ttu-id="15ad5-476">28. April 2020</span><span class="sxs-lookup"><span data-stu-id="15ad5-476">April 28, 2020</span></span>

<span data-ttu-id="15ad5-477">Version 2.5.0</span><span class="sxs-lookup"><span data-stu-id="15ad5-477">Version 2.5.0</span></span>

### <a name="acs"></a><span data-ttu-id="15ad5-478">ACS</span><span class="sxs-lookup"><span data-stu-id="15ad5-478">ACS</span></span>

* <span data-ttu-id="15ad5-479">[BREAKING CHANGE] az openshift create: Parameter „--vnet-peer“ entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-479">[BREAKING CHANGE] az openshift create: remove --vnet-peer parameter.</span></span>
* <span data-ttu-id="15ad5-480">`az openshift create`: Flags zur Unterstützung des privaten Clusters hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-480">`az openshift create`: add flags to support private cluster.</span></span>
* <span data-ttu-id="15ad5-481">`az openshift`: Upgrade auf API-Version `2019-10-27-preview`</span><span class="sxs-lookup"><span data-stu-id="15ad5-481">`az openshift`: upgrade to `2019-10-27-preview` API version.</span></span>
* <span data-ttu-id="15ad5-482">`az openshift`: Befehl `update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-482">`az openshift`: add `update` command.</span></span>

### <a name="aks"></a><span data-ttu-id="15ad5-483">AKS</span><span class="sxs-lookup"><span data-stu-id="15ad5-483">AKS</span></span>

* <span data-ttu-id="15ad5-484">`az aks create`: Unterstützung für Windows hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-484">`az aks create`: Add support for Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="15ad5-485">AppService</span><span class="sxs-lookup"><span data-stu-id="15ad5-485">AppService</span></span>

* <span data-ttu-id="15ad5-486">`az webapp deployment source config-zip`: Energiesparmodus nach „request.get()“ entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-486">`az webapp deployment source config-zip`: remove sleep after request.get()</span></span>

### <a name="arm"></a><span data-ttu-id="15ad5-487">ARM</span><span class="sxs-lookup"><span data-stu-id="15ad5-487">ARM</span></span>

* <span data-ttu-id="15ad5-488">Was-wäre-wenn-Befehle für Vorlagenbereitstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-488">Add template deployment What-If commands</span></span>

### <a name="aro"></a><span data-ttu-id="15ad5-489">ARO</span><span class="sxs-lookup"><span data-stu-id="15ad5-489">ARO</span></span>

* <span data-ttu-id="15ad5-490">`az aro`: Tabellenausgabe korrigiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-490">`az aro`: Fix table output</span></span>

### <a name="ci"></a><span data-ttu-id="15ad5-491">CI</span><span class="sxs-lookup"><span data-stu-id="15ad5-491">CI</span></span>

* <span data-ttu-id="15ad5-492">pytest integriert und nose für Automatisierungstest als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="15ad5-492">Onboard pytest and deprecate nose for Automation Test</span></span>

### <a name="compute"></a><span data-ttu-id="15ad5-493">Compute</span><span class="sxs-lookup"><span data-stu-id="15ad5-493">Compute</span></span>

* <span data-ttu-id="15ad5-494">`az vmss disk detach`: Datenträgerfehler „NoneType“ behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-494">`az vmss disk detach`: fix data disk NoneType issue</span></span>
* <span data-ttu-id="15ad5-495">`az vm availability-set list`: Unterstützung zum Anzeigen der VM-Liste</span><span class="sxs-lookup"><span data-stu-id="15ad5-495">`az vm availability-set list`: Support showing VM list</span></span>
* <span data-ttu-id="15ad5-496">`az vm list-skus`: Anzeigeproblem des Tabellenformats behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-496">`az vm list-skus`: Fix display problem of table format</span></span>

### <a name="keyvault"></a><span data-ttu-id="15ad5-497">KeyVault</span><span class="sxs-lookup"><span data-stu-id="15ad5-497">KeyVault</span></span>

* <span data-ttu-id="15ad5-498">Neuer Parameter `--enable-rbac-authorization` bei Erstellung oder Aktualisierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-498">Add new parameter `--enable-rbac-authorization` during creating or updating</span></span>

### <a name="monitor"></a><span data-ttu-id="15ad5-499">Überwachen</span><span class="sxs-lookup"><span data-stu-id="15ad5-499">Monitor</span></span>

* <span data-ttu-id="15ad5-500">Unterstützung der CMK-Features für LA-Cluster</span><span class="sxs-lookup"><span data-stu-id="15ad5-500">Support LA cluster CMK features</span></span>
* <span data-ttu-id="15ad5-501">`az monitor log-analytics workspace linked-storage`: Unterstützung für BYOS-Features</span><span class="sxs-lookup"><span data-stu-id="15ad5-501">`az monitor log-analytics workspace linked-storage`: supports BYOS features</span></span>

### <a name="network"></a><span data-ttu-id="15ad5-502">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="15ad5-502">Network</span></span>

* <span data-ttu-id="15ad5-503">`az network security-partner`: Unterstützung des Sicherheitspartneranbieters</span><span class="sxs-lookup"><span data-stu-id="15ad5-503">`az network security-partner`: support security partner provider</span></span>

### <a name="privatedns"></a><span data-ttu-id="15ad5-504">PrivateDNS</span><span class="sxs-lookup"><span data-stu-id="15ad5-504">Privatedns</span></span>

* <span data-ttu-id="15ad5-505">Funktion in privater DNS-Zone zum Importieren der Exportzonendatei hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-505">Add feature in private DNS zone to import export zone file</span></span>

## <a name="april-21-2020"></a><span data-ttu-id="15ad5-506">21. April 2020</span><span class="sxs-lookup"><span data-stu-id="15ad5-506">April 21, 2020</span></span>

<span data-ttu-id="15ad5-507">Version 2.4.0</span><span class="sxs-lookup"><span data-stu-id="15ad5-507">Version 2.4.0</span></span>

### <a name="acr"></a><span data-ttu-id="15ad5-508">ACR</span><span class="sxs-lookup"><span data-stu-id="15ad5-508">ACR</span></span>

* <span data-ttu-id="15ad5-509">`az acr run --cmd`: Deaktivieren der Arbeitsverzeichnisaußerkraftsetzung</span><span class="sxs-lookup"><span data-stu-id="15ad5-509">`az acr run --cmd`: disable working directory override</span></span>
* <span data-ttu-id="15ad5-510">Unterstützung dedizierter Datenendpunkte</span><span class="sxs-lookup"><span data-stu-id="15ad5-510">Support dedicated data endpoint</span></span>

### <a name="aks"></a><span data-ttu-id="15ad5-511">AKS</span><span class="sxs-lookup"><span data-stu-id="15ad5-511">AKS</span></span>

* <span data-ttu-id="15ad5-512">`az aks list -o table` sollte „privateFqdn“ als FQDN für private Cluster anzeigen</span><span class="sxs-lookup"><span data-stu-id="15ad5-512">`az aks list -o table` should show privateFqdn as fqdn for private clusters</span></span>
* <span data-ttu-id="15ad5-513">„--uptime-sla“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-513">Add --uptime-sla</span></span>
* <span data-ttu-id="15ad5-514">containerservice-Paket aktualisiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-514">Update containerservice package</span></span>
* <span data-ttu-id="15ad5-515">Unterstützung für öffentliche IP-Adressen für Knoten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-515">Add node public IP support</span></span>
* <span data-ttu-id="15ad5-516">Tippfehler im help-Befehl korrigiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-516">Fix typo in the help command</span></span>

### <a name="appconfig"></a><span data-ttu-id="15ad5-517">AppConfig</span><span class="sxs-lookup"><span data-stu-id="15ad5-517">AppConfig</span></span>

* <span data-ttu-id="15ad5-518">Schlüsseltresorverweis für die Befehle „kv list“ und „kv export“ aufgelöst</span><span class="sxs-lookup"><span data-stu-id="15ad5-518">Resolve key vault reference for kv list and export commands</span></span>
* <span data-ttu-id="15ad5-519">Fehlerbehebung für die Werte für das Auflisten von Schlüsseln</span><span class="sxs-lookup"><span data-stu-id="15ad5-519">Bug fix for list key values</span></span>

### <a name="appservice"></a><span data-ttu-id="15ad5-520">AppService</span><span class="sxs-lookup"><span data-stu-id="15ad5-520">AppService</span></span>

* <span data-ttu-id="15ad5-521">`az functionapp create`: Vorgehensweise zum Festlegen von „linuxFxVersion“ für Linux-Funktions-Apps (.NET) geändert.</span><span class="sxs-lookup"><span data-stu-id="15ad5-521">`az functionapp create`: Changed the way linuxFxVersion was being set for dotnet linux function apps.</span></span> <span data-ttu-id="15ad5-522">Dadurch sollte der Fehler behoben sein, der die Erstellung von Linux-Verbrauchs-Apps (.NET) verhindert hat.</span><span class="sxs-lookup"><span data-stu-id="15ad5-522">This should fix a bug that was preventing dotnet linux consumption apps from being created</span></span>
* <span data-ttu-id="15ad5-523">[BREAKING CHANGE] `az webapp create`: Korrektur vorgenommen, um vorhandene App-Einstellungen (AppSettings) für „az webapp create“ beizubehalten</span><span class="sxs-lookup"><span data-stu-id="15ad5-523">[BREAKING CHANGE] `az webapp create`: fix to keep existing AppSettings with az webapp create</span></span>
* <span data-ttu-id="15ad5-524">[BREAKING CHANGE] `az webapp up`: Korrektur vorgenommen, um bei Verwendung des Flags „-g“ eine RG für den Befehl „az webapp up“ zu erstellen</span><span class="sxs-lookup"><span data-stu-id="15ad5-524">[BREAKING CHANGE] `az webapp up`: fix to create RG for az webapp up command when using -g flag</span></span>
* <span data-ttu-id="15ad5-525">[BREAKING CHANGE] `az webapp config`: Korrektur vorgenommen, um Werte für Nicht-JSON-Ausgaben mit „az webapp config connection-string list“ anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="15ad5-525">[BREAKING CHANGE] `az webapp config`: fix to show values for non-JSON output with az webapp config connection-string list</span></span>

### <a name="arm"></a><span data-ttu-id="15ad5-526">ARM</span><span class="sxs-lookup"><span data-stu-id="15ad5-526">ARM</span></span>

* <span data-ttu-id="15ad5-527">`az deployment create/validate`: Parameter `--no-prompt` hinzugefügt, um das Überspringen der Eingabeaufforderung für fehlende Parameter für die ARM-Vorlage zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="15ad5-527">`az deployment create/validate`: Add parameter `--no-prompt` to support skipping the prompt of missing parameters for ARM template</span></span>
* <span data-ttu-id="15ad5-528">`az deployment group/mg/sub/tenant validate`: Unterstützung von Kommentaren in der Bereitstellungsparameterdatei</span><span class="sxs-lookup"><span data-stu-id="15ad5-528">`az deployment group/mg/sub/tenant validate`: Support comments in deployment parameter file</span></span>
* <span data-ttu-id="15ad5-529">`az deployment`: `is_preview` für Parameter `--handle-extended-json-format` entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-529">`az deployment`: Remove `is_preview` for parameter `--handle-extended-json-format`</span></span>
* <span data-ttu-id="15ad5-530">`az deployment group/mg/sub/tenant cancel`: Unterstützung für den Abbruch der Bereitstellung für ARM-Vorlagen</span><span class="sxs-lookup"><span data-stu-id="15ad5-530">`az deployment group/mg/sub/tenant cancel`: Support cancel deployment for ARM template</span></span>
* <span data-ttu-id="15ad5-531">`az deployment group/mg/sub/tenant validate`: Fehlermeldung bei einem Fehler der Bereitstellungsüberprüfung verbessert</span><span class="sxs-lookup"><span data-stu-id="15ad5-531">`az deployment group/mg/sub/tenant validate`: Improve the error message when deployment verification fails</span></span>
* <span data-ttu-id="15ad5-532">`az deployment-scripts`: Neue Befehle für DeploymentScripts hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-532">`az deployment-scripts`: Add new commands for DeploymentScripts</span></span>
* <span data-ttu-id="15ad5-533">`az resource tag`: Parameter `--is-incremental` hinzugefügt, um das inkrementelle Hinzufügen von Tags zur Ressource zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="15ad5-533">`az resource tag`: Add parameter `--is-incremental` to support adding tags to resource incrementally</span></span>

### <a name="aro"></a><span data-ttu-id="15ad5-534">ARO</span><span class="sxs-lookup"><span data-stu-id="15ad5-534">ARO</span></span>

* <span data-ttu-id="15ad5-535">`az aro`:  ARO-Befehlsmodul von Azure RedHat OpenShift V4 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-535">`az aro`:  Add Azure RedHat OpenShift V4 aro command module</span></span>

### <a name="batch"></a><span data-ttu-id="15ad5-536">Batch</span><span class="sxs-lookup"><span data-stu-id="15ad5-536">Batch</span></span>

* <span data-ttu-id="15ad5-537">Batch-API aktualisiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-537">Update Batch API</span></span>

### <a name="compute"></a><span data-ttu-id="15ad5-538">Compute</span><span class="sxs-lookup"><span data-stu-id="15ad5-538">Compute</span></span>

* <span data-ttu-id="15ad5-539">`az sig image-version create`: Speicherkontotyp „Premium_LRS“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-539">`az sig image-version create`: Add storage account type Premium_LRS</span></span>
* <span data-ttu-id="15ad5-540">`az vmss update`: Problem behoben, das beim Aktualisieren der Beendigungsbenachrichtigung auftrat</span><span class="sxs-lookup"><span data-stu-id="15ad5-540">`az vmss update`: Fix terminate notification update issue</span></span>
* <span data-ttu-id="15ad5-541">`az vm/vmss create`: Unterstützung für spezialisierte Imageversion hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-541">`az vm/vmss create`: Add support for specialized image version</span></span>
* <span data-ttu-id="15ad5-542">SIG-API-Version 2019-12-01</span><span class="sxs-lookup"><span data-stu-id="15ad5-542">SIG API Version 2019-12-01</span></span>
* <span data-ttu-id="15ad5-543">`az sig image-version create`: „--target-region-encryption“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-543">`az sig image-version create`: Add --target-region-encryption</span></span>
* <span data-ttu-id="15ad5-544">Fehler bei Serientestausführung behoben, der auf die Duplizierung des Schlüsseltresornamens im globalen In-Memory-Cache zurückzuführen war.</span><span class="sxs-lookup"><span data-stu-id="15ad5-544">Fix tests fail when running in serial due to keyvault name is duplicated in global in-momery cache</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="15ad5-545">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="15ad5-545">CosmosDB</span></span>

* <span data-ttu-id="15ad5-546">Unterstützung für `az cosmosdb private-link-resource/private-endpoint-connection`</span><span class="sxs-lookup"><span data-stu-id="15ad5-546">Support `az cosmosdb private-link-resource/private-endpoint-connection`</span></span>

### <a name="iot-central"></a><span data-ttu-id="15ad5-547">IoT Central</span><span class="sxs-lookup"><span data-stu-id="15ad5-547">IoT Central</span></span>

* <span data-ttu-id="15ad5-548">`az iotcentral` als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="15ad5-548">Deprecate `az iotcentral`</span></span>
* <span data-ttu-id="15ad5-549">Befehlsmodul `az iot central` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-549">Add `az iot central` command module</span></span>

### <a name="monitor"></a><span data-ttu-id="15ad5-550">Überwachen</span><span class="sxs-lookup"><span data-stu-id="15ad5-550">Monitor</span></span>

* <span data-ttu-id="15ad5-551">Unterstützung eines Private Link-Szenarios für die Überwachung</span><span class="sxs-lookup"><span data-stu-id="15ad5-551">Support private link scenario for monitor</span></span>
* <span data-ttu-id="15ad5-552">Falsche Simulationsmethode in „test_monitor_general_operations.py“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-552">Fix wrong mocking way in test_monitor_general_operations.py</span></span>

### <a name="network"></a><span data-ttu-id="15ad5-553">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="15ad5-553">Network</span></span>

* <span data-ttu-id="15ad5-554">SKU für den Befehl zur Aktualisierung der öffentlichen IP-Adresse als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="15ad5-554">Deprecate sku for public ip update command</span></span>
* <span data-ttu-id="15ad5-555">`az network private-endpoint`: Unterstützung für private DNS-Zonengruppe</span><span class="sxs-lookup"><span data-stu-id="15ad5-555">`az network private-endpoint`: Support private dns zone group</span></span>
* <span data-ttu-id="15ad5-556">Feature für lokalen Kontext für VNET-/Subnetzparameter aktiviert</span><span class="sxs-lookup"><span data-stu-id="15ad5-556">Enable local context feature for vnet/subnet parameter</span></span>
* <span data-ttu-id="15ad5-557">Falsches Verwendungsbeispiel in „test_nw_flow_log_delete“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-557">Fix wrong usage example in test_nw_flow_log_delete</span></span>

### <a name="packaging"></a><span data-ttu-id="15ad5-558">Verpackung</span><span class="sxs-lookup"><span data-stu-id="15ad5-558">Packaging</span></span>

* <span data-ttu-id="15ad5-559">Unterstützung für Ubuntu-/Disco-Paket eingestellt</span><span class="sxs-lookup"><span data-stu-id="15ad5-559">Drop support for Ubuntu/Disco package</span></span>

### <a name="rbac"></a><span data-ttu-id="15ad5-560">RBAC</span><span class="sxs-lookup"><span data-stu-id="15ad5-560">RBAC</span></span>

* <span data-ttu-id="15ad5-561">`az ad app create/update`: Unterstützung von „--optional-claims“ als Parameter</span><span class="sxs-lookup"><span data-stu-id="15ad5-561">`az ad app create/update`: support --optional-claims as a parameter</span></span>

### <a name="rdbms"></a><span data-ttu-id="15ad5-562">RDBMS</span><span class="sxs-lookup"><span data-stu-id="15ad5-562">RDBMS</span></span>

* <span data-ttu-id="15ad5-563">Azure Active Directory-Administratorbefehle für PostgreSQL und MySQL hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-563">Add Azure active directory administrator commands for PostgreSQL and MySQL</span></span>

### <a name="service-fabric"></a><span data-ttu-id="15ad5-564">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="15ad5-564">Service Fabric</span></span>

* <span data-ttu-id="15ad5-565">Fehlerbehebung Nr. 12891: `az sf application update --application-parameters` entfernt alte Parameter, die nicht in der Anforderung enthalten sind.</span><span class="sxs-lookup"><span data-stu-id="15ad5-565">Fix #12891: `az sf application update --application-parameters` removes old parameters that are not in the request</span></span>
* <span data-ttu-id="15ad5-566">Fehlerbehebung Nr. 12470: az sf create cluster: Fehler im Zusammenhang mit der Dauerhaftigkeit und Zuverlässigkeit von Updates sowie im Zusammenhang mit der codebasierten Suche der VMSS unter Angabe eines bestimmten Knotentypnamens behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-566">Fix #12470 az sf create cluster, fix bugs in update durability and reliability and find vmss correctly through the code given a node type name</span></span>

### <a name="sql"></a><span data-ttu-id="15ad5-567">SQL</span><span class="sxs-lookup"><span data-stu-id="15ad5-567">SQL</span></span>

* <span data-ttu-id="15ad5-568">`az sql mi op list`, `az sql mi op get`, `az sql mi op cancel` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-568">Add `az sql mi op list`, `az sql mi op get`, `az sql mi op cancel`</span></span>
* <span data-ttu-id="15ad5-569">`az sql midb`: Aktualisieren/Anzeigen der Richtlinie zur langfristigen Aufbewahrung, Anzeigen/Löschen von Sicherungen zur langfristigen Aufbewahrung, Wiederherstellen von Sicherungen zur langfristigen Aufbewahrung</span><span class="sxs-lookup"><span data-stu-id="15ad5-569">`az sql midb`: update/show long term retention policy,  show/delete long term retention backups, restore long term retention backup</span></span>

### <a name="storage"></a><span data-ttu-id="15ad5-570">Storage</span><span class="sxs-lookup"><span data-stu-id="15ad5-570">Storage</span></span>

* <span data-ttu-id="15ad5-571">„azure-mgmt-storage“ auf 9.0.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-571">Upgrade azure-mgmt-storage to 9.0.0</span></span>
* <span data-ttu-id="15ad5-572">`az storage logging off`: Unterstützung für das Ausschalten der Protokollierung für ein Speicherkonto</span><span class="sxs-lookup"><span data-stu-id="15ad5-572">`az storage logging off`: Support turning off logging for a storage account</span></span>
* <span data-ttu-id="15ad5-573">`az storage account update`: Automatische Rotation von Schlüsseln für CMK aktiviert</span><span class="sxs-lookup"><span data-stu-id="15ad5-573">`az storage account update`: Enable key auto-rotated for CMK</span></span>
* <span data-ttu-id="15ad5-574">`az storage account encryption-scope create/update/list/show`: Unterstützung zum Anpassen des Verschlüsselungsbereichs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-574">`az storage account encryption-scope create/update/list/show`: Add support to customize encryption scope</span></span>
* <span data-ttu-id="15ad5-575">`az storage container create`: „--default-encryption-scope“ und „--deny-encryption-scope-override“ hinzugefügt, um den Verschlüsselungsbereich für die Containerebene festzulegen</span><span class="sxs-lookup"><span data-stu-id="15ad5-575">`az storage container create`: Add --default-encryption-scope and --deny-encryption-scope-override to set encryption scope for container level</span></span>

### <a name="survey"></a><span data-ttu-id="15ad5-576">Umfrage</span><span class="sxs-lookup"><span data-stu-id="15ad5-576">Survey</span></span>

* <span data-ttu-id="15ad5-577">Switch zum Deaktivieren des Umfragelinks hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-577">Add switch to turn off survey link</span></span>

## <a name="april-01-2020"></a><span data-ttu-id="15ad5-578">01. April 2020</span><span class="sxs-lookup"><span data-stu-id="15ad5-578">April 01, 2020</span></span>

<span data-ttu-id="15ad5-579">Version 2.3.1</span><span class="sxs-lookup"><span data-stu-id="15ad5-579">Version 2.3.1</span></span>

### <a name="acr"></a><span data-ttu-id="15ad5-580">ACR</span><span class="sxs-lookup"><span data-stu-id="15ad5-580">ACR</span></span>

* <span data-ttu-id="15ad5-581">Falsche Version von „azure-mgmt-containerregistry“ für Linux korrigiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-581">Fix wrong version of azure-mgmt-containerregistry for Linux</span></span>

### <a name="profile"></a><span data-ttu-id="15ad5-582">Profil</span><span class="sxs-lookup"><span data-stu-id="15ad5-582">Profile</span></span>

* <span data-ttu-id="15ad5-583">az login: Anmeldefehler behoben, der auftrat, wenn nicht das Cloudprofil `latest` verwendet wurde</span><span class="sxs-lookup"><span data-stu-id="15ad5-583">az login: Fix login failure with cloud profiles other than `latest`</span></span>

## <a name="march-31-2020"></a><span data-ttu-id="15ad5-584">31. März 2020</span><span class="sxs-lookup"><span data-stu-id="15ad5-584">March 31, 2020</span></span>

<span data-ttu-id="15ad5-585">Version 2.3.0</span><span class="sxs-lookup"><span data-stu-id="15ad5-585">Version 2.3.0</span></span>

### <a name="acr"></a><span data-ttu-id="15ad5-586">ACR</span><span class="sxs-lookup"><span data-stu-id="15ad5-586">ACR</span></span>

* <span data-ttu-id="15ad5-587">„az acr task update“: NULL-Zeiger-Ausnahme</span><span class="sxs-lookup"><span data-stu-id="15ad5-587">'az acr task update': null pointer exception</span></span>
* <span data-ttu-id="15ad5-588">`az acr import`: Hilfe und Fehlermeldung geändert, um die Verwendung von „--source“ und „--registry“ zu verdeutlichen</span><span class="sxs-lookup"><span data-stu-id="15ad5-588">`az acr import`: Modify help and error message to clarify the usage of --source and --registry</span></span>
* <span data-ttu-id="15ad5-589">Überprüfung für das Argument „registry_name“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-589">Add a validator for argument 'registry_name'</span></span>
* <span data-ttu-id="15ad5-590">`az acr login`: Vorschauflag für „--expose-token“ entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-590">`az acr login`:Remove the preview flag on '--expose-token'</span></span>
* <span data-ttu-id="15ad5-591">[BREAKING CHANGE] Branch-Parameter „az acr task create/update“ entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-591">[BREAKING CHANGE] 'az acr task create/update' Branch parameter is removed</span></span>
* <span data-ttu-id="15ad5-592">„az acr task update“: Kunde kann nun Kontext, Git-Token und/oder Trigger einzeln aktualisieren</span><span class="sxs-lookup"><span data-stu-id="15ad5-592">'az acr task update' Customer now can update context, git-token, and or triggers individually</span></span>
* <span data-ttu-id="15ad5-593">„az acr agentpool“: Neues Feature</span><span class="sxs-lookup"><span data-stu-id="15ad5-593">'az acr agentpool': new feature</span></span>

### <a name="aks"></a><span data-ttu-id="15ad5-594">AKS</span><span class="sxs-lookup"><span data-stu-id="15ad5-594">AKS</span></span>

* <span data-ttu-id="15ad5-595">„apiServerAccessProfile“ bei der Aktualisierung von „--api-server-authorized-ip-ranges“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-595">Fix apiServerAccessProfile when updating --api-server-authorized-ip-ranges</span></span>
* <span data-ttu-id="15ad5-596">aks update: Überschreibung ausgehender IP-Adressen mit Eingabewerten bei der Aktualisierung</span><span class="sxs-lookup"><span data-stu-id="15ad5-596">aks update: Override outbound IPs with input values when update</span></span>
* <span data-ttu-id="15ad5-597">Keine SPN-Erstellung für MSI-Cluster sowie Unterstützung der Anfügung von ACR an MSI-Cluster</span><span class="sxs-lookup"><span data-stu-id="15ad5-597">Do not create SPN for MSI clusters and support attach acr to MSI clusters</span></span>

### <a name="ams"></a><span data-ttu-id="15ad5-598">AMS</span><span class="sxs-lookup"><span data-stu-id="15ad5-598">AMS</span></span>

* <span data-ttu-id="15ad5-599">Fix 12469: Hinzufügen von „content-key-policy“ für Fairplay aufgrund von Problemen mit dem Parameter „ask“ nicht erfolgreich</span><span class="sxs-lookup"><span data-stu-id="15ad5-599">Fix #12469: adding Fairplay content-key-policy fails due to problems with 'ask' parameter</span></span>

### <a name="appconfig"></a><span data-ttu-id="15ad5-600">AppConfig</span><span class="sxs-lookup"><span data-stu-id="15ad5-600">AppConfig</span></span>

* <span data-ttu-id="15ad5-601">„--skip-keyvault“ für „kv export“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-601">Add --skip-keyvault for kv export</span></span>

### <a name="appservice"></a><span data-ttu-id="15ad5-602">AppService</span><span class="sxs-lookup"><span data-stu-id="15ad5-602">AppService</span></span>

* <span data-ttu-id="15ad5-603">Fix 12509: Tag für „az webapp up“ standardmäßig entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-603">Fix #12509: Remove the tag to az webapp up by default</span></span>
* <span data-ttu-id="15ad5-604">az functionapp create: Hilfemenü für „--runtime-version“ aktualisiert und Warnung hinzugefügt, wenn der Benutzer „--runtime-version“ für .NET angibt</span><span class="sxs-lookup"><span data-stu-id="15ad5-604">az functionapp create: Updated --runtime-version help menu and added warning when user specifies --runtime-version for dotnet</span></span>
* <span data-ttu-id="15ad5-605">az functionapp create: Methode zum Festlegen von „javaVersion“ für Windows-Funktions-Apps aktualisiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-605">az functionapp create: Updated the way javaVersion was being set for Windows function apps</span></span>

### <a name="arm"></a><span data-ttu-id="15ad5-606">ARM</span><span class="sxs-lookup"><span data-stu-id="15ad5-606">ARM</span></span>

* <span data-ttu-id="15ad5-607">az deployment create/validate: Standardmäßige Verwendung von „--handle-extended-json-format“</span><span class="sxs-lookup"><span data-stu-id="15ad5-607">az deployment create/validate: Use --handle-extended-json-format by default</span></span>
* <span data-ttu-id="15ad5-608">az lock create: Beispiele für die Erstellung einer Unterressource in der Hilfedokumentation hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-608">az lock create: Add examples of creating subresource in the help documentation</span></span>
* <span data-ttu-id="15ad5-609">az deployment {group/mg/sub/tenant} list: Unterstützung der provisioningState-Filterung</span><span class="sxs-lookup"><span data-stu-id="15ad5-609">az deployment {group/mg/sub/tenant} list: Support provisioningState filtering</span></span>
* <span data-ttu-id="15ad5-610">az deployment: Analysefehler für Kommentar unter letztem Argument behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-610">az deployment: Fix the parse bug for comment under the last argument</span></span>

### <a name="backup"></a><span data-ttu-id="15ad5-611">Backup</span><span class="sxs-lookup"><span data-stu-id="15ad5-611">Backup</span></span>

* <span data-ttu-id="15ad5-612">Mehrere Dateiwiederherstellungsfunktionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-612">Added multiple files restore capabilities</span></span>
* <span data-ttu-id="15ad5-613">Unterstützung der ausschließlichen Sicherung von Betriebssystemdatenträgern hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-613">Added support for Backing up OS Disks only</span></span>
* <span data-ttu-id="15ad5-614">Parameter „restore-as-unmanaged-disk“ für die Angabe einer nicht verwalteten Wiederherstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-614">Added restore-as-unmanaged-disk parameter to specify unmanaged restore</span></span>

### <a name="compute"></a><span data-ttu-id="15ad5-615">Compute</span><span class="sxs-lookup"><span data-stu-id="15ad5-615">Compute</span></span>

* <span data-ttu-id="15ad5-616">az vm create: Option „NONE“ von „--nsg-rule“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-616">az vm create: Add NONE option of --nsg-rule</span></span>
* <span data-ttu-id="15ad5-617">az vmss create/update: Vorschautag für automatische VMSS-Reparaturen entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-617">az vmss create/update: remove vmss automatic repairs preview tag</span></span>
* <span data-ttu-id="15ad5-618">az vm update: Unterstützung von „--workspace“</span><span class="sxs-lookup"><span data-stu-id="15ad5-618">az vm update: Support --workspace</span></span>
* <span data-ttu-id="15ad5-619">Fehler im VirtualMachineScaleSetExtension-Initialisierungscode behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-619">Fix a bug in VirtualMachineScaleSetExtension initialization code</span></span>
* <span data-ttu-id="15ad5-620">Upgrade der VMAccessAgent-Version auf 2.4 durchgeführt</span><span class="sxs-lookup"><span data-stu-id="15ad5-620">Upgrade VMAccessAgent version to 2.4</span></span>
* <span data-ttu-id="15ad5-621">az vmss set-orchestration-service-state: Unterstützung zum Festlegen des Orchestrierungdienstzustands für VMSS</span><span class="sxs-lookup"><span data-stu-id="15ad5-621">az vmss set-orchestration-service-state: support vmss set orchestration service state</span></span>
* <span data-ttu-id="15ad5-622">Upgrade der Datenträger-API-Version auf 2019-11-01 durchgeführt</span><span class="sxs-lookup"><span data-stu-id="15ad5-622">Upgrade disk API version to 2019-11-01</span></span>
* <span data-ttu-id="15ad5-623">az disk create: add --disk-iops-read-only, --disk-mbps-read-only, --max-shares, --image-reference, --image-reference-lun, --gallery-image-reference, --gallery-image-reference-lun</span><span class="sxs-lookup"><span data-stu-id="15ad5-623">az disk create: add --disk-iops-read-only, --disk-mbps-read-only, --max-shares, --image-reference, --image-reference-lun, --gallery-image-reference, --gallery-image-reference-lun</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="15ad5-624">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="15ad5-624">Cosmos DB</span></span>

* <span data-ttu-id="15ad5-625">Fehlende Option „--type“ für Veraltungsumleitungen korrigiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-625">Fix missing --type option for deprecation redirections</span></span>

### <a name="docker"></a><span data-ttu-id="15ad5-626">Docker</span><span class="sxs-lookup"><span data-stu-id="15ad5-626">Docker</span></span>

* <span data-ttu-id="15ad5-627">Update auf Alpine 3.11 und Python 3.6.10 durchgeführt</span><span class="sxs-lookup"><span data-stu-id="15ad5-627">Update to Alpine 3.11 and Python 3.6.10</span></span>

### <a name="extension"></a><span data-ttu-id="15ad5-628">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="15ad5-628">Extension</span></span>

* <span data-ttu-id="15ad5-629">Laden von Erweiterungen im Systempfad mittels Paketen ermöglicht</span><span class="sxs-lookup"><span data-stu-id="15ad5-629">Allow to load extensions in the system path via packages</span></span>

### <a name="hdinsight"></a><span data-ttu-id="15ad5-630">HDInsight</span><span class="sxs-lookup"><span data-stu-id="15ad5-630">HDInsight</span></span>

* <span data-ttu-id="15ad5-631">(az hdinsight create:) Unterstützung der Angabe der unterstützten TLS-Mindestversion durch Kunden unter Verwendung des Parameters `--minimal-tls-version`.</span><span class="sxs-lookup"><span data-stu-id="15ad5-631">(az hdinsight create:) Support customers specify minimal supported tls version by using parameter `--minimal-tls-version`.</span></span> <span data-ttu-id="15ad5-632">Zulässiger Wert: 1.0,1.1,1.2</span><span class="sxs-lookup"><span data-stu-id="15ad5-632">The allowed value is 1.0,1.1,1.2</span></span>

### <a name="iot"></a><span data-ttu-id="15ad5-633">IoT</span><span class="sxs-lookup"><span data-stu-id="15ad5-633">IoT</span></span>

* <span data-ttu-id="15ad5-634">Codebesitzer hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-634">Add codeowner</span></span>
* <span data-ttu-id="15ad5-635">az iot hub create: Standard-SKU von F1 in S1 geändert</span><span class="sxs-lookup"><span data-stu-id="15ad5-635">az iot hub create : Change default sku to S1 from F1</span></span>
* <span data-ttu-id="15ad5-636">iot hub: Unterstützung von „IotHub“ im Profil „2019-03-01-hybrid“</span><span class="sxs-lookup"><span data-stu-id="15ad5-636">iot hub: Support IotHub in the profile of 2019-03-01-hybrid</span></span>

### <a name="iotcentral"></a><span data-ttu-id="15ad5-637">IoTCentral</span><span class="sxs-lookup"><span data-stu-id="15ad5-637">IoTCentral</span></span>

* <span data-ttu-id="15ad5-638">Fehlerdetails sowie Standardanwendungsvorlage und Aufforderungsmeldung aktualisiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-638">Update error details, update default application template and prompt message</span></span>

### <a name="keyvault"></a><span data-ttu-id="15ad5-639">KeyVault</span><span class="sxs-lookup"><span data-stu-id="15ad5-639">KeyVault</span></span>

* <span data-ttu-id="15ad5-640">Unterstützung von Zertifikatsicherung/-wiederherstellung</span><span class="sxs-lookup"><span data-stu-id="15ad5-640">Support certificate backup/restore</span></span>
* <span data-ttu-id="15ad5-641">keyvault create/update: Unterstützung von „--retention-days“</span><span class="sxs-lookup"><span data-stu-id="15ad5-641">keyvault create/update: Support --retention-days</span></span>
* <span data-ttu-id="15ad5-642">Keine Anzeige von verwalteten Schlüsseln/Geheimnissen bei der Auflistung mehr</span><span class="sxs-lookup"><span data-stu-id="15ad5-642">No longer display managed keys/secrets while listing</span></span>
* <span data-ttu-id="15ad5-643">az keyvault create: Unterstützung von `--network-acls`, `--network-acls-ips` und `--network-acls-vnets` zur Angabe von Netzwerkregeln bei der Tresorerstellung</span><span class="sxs-lookup"><span data-stu-id="15ad5-643">az keyvault create: support `--network-acls`, `--network-acls-ips` and `--network-acls-vnets` for specifying network rules while creating vault</span></span>

### <a name="lock"></a><span data-ttu-id="15ad5-644">Sperre</span><span class="sxs-lookup"><span data-stu-id="15ad5-644">Lock</span></span>

* <span data-ttu-id="15ad5-645">Fehlerbehebung für „az lock delete“: „az lock delete“ funktioniert für „Microsoft.DocumentDB“ nicht.</span><span class="sxs-lookup"><span data-stu-id="15ad5-645">az lock delete fix bug: az lock delete does not work on Microsoft.DocumentDB</span></span>

### <a name="monitor"></a><span data-ttu-id="15ad5-646">Überwachen</span><span class="sxs-lookup"><span data-stu-id="15ad5-646">Monitor</span></span>

* <span data-ttu-id="15ad5-647">az monitor clone: Unterstützung des Klonens von Metrikregeln zwischen Ressourcen</span><span class="sxs-lookup"><span data-stu-id="15ad5-647">az monitor clone: support clone metric rules from one resource to another</span></span>
* <span data-ttu-id="15ad5-648">Fix IcM179210086: Erstellung einer benutzerdefinierten Metrikwarnung für die Application Insights-Metrik nicht möglich</span><span class="sxs-lookup"><span data-stu-id="15ad5-648">Fix IcM179210086: unable to create custom metric alert for their Application Insights metric</span></span>

### <a name="netappfiles"></a><span data-ttu-id="15ad5-649">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="15ad5-649">NetAppFiles</span></span>

* <span data-ttu-id="15ad5-650">az volume create: Datenschutzvolumes zum Hinzufügen von Replikationsvorgängen zugelassen: Genehmigen, Aussetzen, Fortsetzen, Status, Entfernen</span><span class="sxs-lookup"><span data-stu-id="15ad5-650">az volume create: Allow data protection volumes adding replication operations: approve, suspend, resume, status, remove</span></span>

### <a name="network"></a><span data-ttu-id="15ad5-651">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="15ad5-651">Network</span></span>

* <span data-ttu-id="15ad5-652">az network application-gateway waf-policy managed-rule rule-set add: Unterstützung von „ Microsoft_BotManagerRuleSet“</span><span class="sxs-lookup"><span data-stu-id="15ad5-652">az network application-gateway waf-policy managed-rule rule-set add: support Microsoft_BotManagerRuleSet</span></span>
* <span data-ttu-id="15ad5-653">network watcher flow-log show: Falsche Veraltungsinformationen behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-653">network watcher flow-log show: fix wrong deprecating info</span></span>
* <span data-ttu-id="15ad5-654">Unterstützung von Hostnamen im Application Gateway-Listener</span><span class="sxs-lookup"><span data-stu-id="15ad5-654">support host names in application gateway listener</span></span>
* <span data-ttu-id="15ad5-655">az network nat gateway: Unterstützung der Erstellung einer leeren Ressource ohne öffentliche IP-Adresse oder Präfix für öffentliche IP-Adressen</span><span class="sxs-lookup"><span data-stu-id="15ad5-655">az network nat gateway: support create empty resource without public ip or public ip prefix</span></span>
* <span data-ttu-id="15ad5-656">Unterstützung der VPN-Gateway-Generierung</span><span class="sxs-lookup"><span data-stu-id="15ad5-656">Support vpn gateway generation</span></span>
* <span data-ttu-id="15ad5-657">Unterstützung von `--if-none-match` in `az network dns record-set {} add-record`</span><span class="sxs-lookup"><span data-stu-id="15ad5-657">Support `--if-none-match` in `az network dns record-set {} add-record`</span></span>

### <a name="packaging"></a><span data-ttu-id="15ad5-658">Verpackung</span><span class="sxs-lookup"><span data-stu-id="15ad5-658">Packaging</span></span>

* <span data-ttu-id="15ad5-659">Unterstützung von Python 3.5 eingestellt</span><span class="sxs-lookup"><span data-stu-id="15ad5-659">Drop support for python 3.5</span></span>

### <a name="profile"></a><span data-ttu-id="15ad5-660">Profil</span><span class="sxs-lookup"><span data-stu-id="15ad5-660">Profile</span></span>

* <span data-ttu-id="15ad5-661">az login: Warnung für MFA-Fehler</span><span class="sxs-lookup"><span data-stu-id="15ad5-661">az login: Show warning for MFA error</span></span>

### <a name="rdbms"></a><span data-ttu-id="15ad5-662">RDBMS</span><span class="sxs-lookup"><span data-stu-id="15ad5-662">RDBMS</span></span>

* <span data-ttu-id="15ad5-663">Befehle zur Verwaltung von Verschlüsselungsschlüsseln für Serverdaten für PostgreSQL und MySQL hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-663">Add server data encryption key management commands for PostgreSQL and MySQL</span></span>

## <a name="march-10-2020"></a><span data-ttu-id="15ad5-664">10. März 2020</span><span class="sxs-lookup"><span data-stu-id="15ad5-664">March 10, 2020</span></span>

<span data-ttu-id="15ad5-665">Version 2.2.0</span><span class="sxs-lookup"><span data-stu-id="15ad5-665">Version 2.2.0</span></span>

### <a name="acr"></a><span data-ttu-id="15ad5-666">ACR</span><span class="sxs-lookup"><span data-stu-id="15ad5-666">ACR</span></span>

* <span data-ttu-id="15ad5-667">Fix: `az acr login` löst fälschlicherweise Fehler aus</span><span class="sxs-lookup"><span data-stu-id="15ad5-667">Fix: `az acr login` wrongly raise error</span></span>
* <span data-ttu-id="15ad5-668">Neuer Befehl `az acr helm install-cli` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-668">Add new command `az acr helm install-cli`</span></span>
* <span data-ttu-id="15ad5-669">Privater Link und CMK-Unterstützung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-669">Add private link and CMK support</span></span>
* <span data-ttu-id="15ad5-670">Befehl „private-link-resource list“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-670">add 'private-link-resource list' command</span></span>

### <a name="aks"></a><span data-ttu-id="15ad5-671">AKS</span><span class="sxs-lookup"><span data-stu-id="15ad5-671">AKS</span></span>

* <span data-ttu-id="15ad5-672">Durchsuchen von AKS in Cloud-Shell korrigiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-672">fix the aks browse in cloud shell</span></span>
* <span data-ttu-id="15ad5-673">az aks: NoneType-Fehler beim Überwachen von „addon“ und „agentpool“ behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-673">az aks: Fix monitoring addon and agentpool NoneType errors</span></span>
* <span data-ttu-id="15ad5-674">„--nodepool-tags“ zum Knotenpool beim Erstellen von Azure-Kubernetes-Clustern hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-674">Add --nodepool-tags to node pool when creating azure kubernetes cluster</span></span>
* <span data-ttu-id="15ad5-675">„--tags“ beim Hinzufügen oder Aktualisieren eines Knotenpool in einem Cluster hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-675">Add --tags when adding or updating a nodepool to cluster</span></span>
* <span data-ttu-id="15ad5-676">aks create: `--enable-private-cluster` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-676">aks create: add `--enable-private-cluster`</span></span>
* <span data-ttu-id="15ad5-677">„--nodepool-labels“ beim Erstellen von Azure-Kubernetes-Clustern hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-677">add --nodepool-labels when creating azure kubernetes cluster</span></span>
* <span data-ttu-id="15ad5-678">„--labels“ beim Hinzufügen eines neuen Knotenpools zu einem Azure-Kubernetes-Cluster hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-678">add --labels when adding a new nodepool to azure kubernetes cluster</span></span>
* <span data-ttu-id="15ad5-679">Fehlender Schrägstrich (/) in der Dashboard-URL hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-679">add missing / in the dashboard url</span></span>
* <span data-ttu-id="15ad5-680">Unterstützung der Erstellung von AKS-Clustern, sodass verwaltete Identitäten möglich sind</span><span class="sxs-lookup"><span data-stu-id="15ad5-680">Support create aks clusters enabling managed identity</span></span>
* <span data-ttu-id="15ad5-681">az aks: Überprüfen, ob das Netzwerk-Plug-In entweder „azure“ oder „kubenet“ ist</span><span class="sxs-lookup"><span data-stu-id="15ad5-681">az aks: Validate network plugin to be either "azure" or "kubenet"</span></span>
* <span data-ttu-id="15ad5-682">az aks: Unterstützung für AAD-Sitzungsschlüssel hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-682">az aks: Add aad session key support</span></span>
* <span data-ttu-id="15ad5-683">[BREAKING CHANGE] az aks: Unterstützung von MSI-Änderungen für GF und BF für omsagent (Containerüberwachung)(#1)</span><span class="sxs-lookup"><span data-stu-id="15ad5-683">[BREAKING CHANGE] az aks: support msi changes for GF and BF for omsagent (Container monitoring)(#1)</span></span>
* <span data-ttu-id="15ad5-684">az aks use-dev-spaces: Endpunkt-Typoption zum Befehl „use-dev-spaces“, hinzugefügt, um den auf einem Azure Dev Spaces-Controller erstellten Endpunkt anzupassen</span><span class="sxs-lookup"><span data-stu-id="15ad5-684">az aks use-dev-spaces: Adding endpoint type option to the use-dev-spaces command to customize the endpoint created on an Azure Dev Spaces controller</span></span>

### <a name="appconfig"></a><span data-ttu-id="15ad5-685">AppConfig</span><span class="sxs-lookup"><span data-stu-id="15ad5-685">AppConfig</span></span>

* <span data-ttu-id="15ad5-686">Verwendung von „kv set“ entsperrt, um Schlüsseltresorverweis und -funktion hinzuzufügen …</span><span class="sxs-lookup"><span data-stu-id="15ad5-686">Unblock using "kv set" to add keyvault reference and feature …</span></span>

### <a name="appservice"></a><span data-ttu-id="15ad5-687">AppService</span><span class="sxs-lookup"><span data-stu-id="15ad5-687">AppService</span></span>

* <span data-ttu-id="15ad5-688">az webapp create : Beheben eines Problems beim Ausführen des Befehls mit „--runtime“</span><span class="sxs-lookup"><span data-stu-id="15ad5-688">az webapp create : Fix issue when running the command with --runtime</span></span>
* <span data-ttu-id="15ad5-689">az functionapp deployment source config-zip: Fehlermeldung hinzugefügt, wenn der Ressourcengruppen- oder Funktionsname ungültig oder nicht vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="15ad5-689">az functionapp deployment source config-zip: Add an error message if resource group or function name are invalid/don't exist</span></span>
* <span data-ttu-id="15ad5-690">functionapp create: Warnmeldung korrigiert, die derzeit mit `functionapp create` angezeigt wird und ein `--functions_version`-Flag angibt, aber irrtümlich ein `_` anstelle eines `-` im Flagnamen verwendet</span><span class="sxs-lookup"><span data-stu-id="15ad5-690">functionapp create: Fix the warning message that appears with `functionapp create` today which cites a `--functions_version` flag but erroneously uses a `_` instead of a `-` in the flag name</span></span>
* <span data-ttu-id="15ad5-691">az functionapp create: Es wurde aktualisiert, wie linuxFxVersion und der Containerimagename für Linux-Funktions-Apps festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="15ad5-691">az functionapp create: Updated the way linuxFxVersion and container image name were being set for linux function apps</span></span>
* <span data-ttu-id="15ad5-692">az functionapp deployment source config-zip: Problems behoben, das durch die Racebedingung für die Änderung von App-Einstellungen während der ZIP-Bereitstellung verursacht wird und während der Bereitstellung 5xx-Fehler ausgibt</span><span class="sxs-lookup"><span data-stu-id="15ad5-692">az functionapp deployment source config-zip: Fix an issue caused by app settings change racing condition during zip deploy, giving 5xx errors during deployment</span></span>
* <span data-ttu-id="15ad5-693">Fix #5720946: „az webapp backup“ legt Namen nicht fest</span><span class="sxs-lookup"><span data-stu-id="15ad5-693">Fix #5720946: az webapp backup fails to set name</span></span>

### <a name="arm"></a><span data-ttu-id="15ad5-694">ARM</span><span class="sxs-lookup"><span data-stu-id="15ad5-694">ARM</span></span>

* <span data-ttu-id="15ad5-695">az resource: Beispiele für das Ressourcenmodul verbessert</span><span class="sxs-lookup"><span data-stu-id="15ad5-695">az resource: Improve the examples of the resource module</span></span>
* <span data-ttu-id="15ad5-696">az policy assignment list: Unterstützung für das Auflisten von Richtlinienzuweisungen im Verwaltungsgruppenbereich</span><span class="sxs-lookup"><span data-stu-id="15ad5-696">az policy assignment list: Support listing policy assignments at Management Group scope</span></span>
* <span data-ttu-id="15ad5-697">`az deployment group` und `az deployment operation group` für Vorlagenbereitstellung in Ressourcengruppen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-697">Add `az deployment group` and `az deployment operation group` for template deployment at resource groups.</span></span> <span data-ttu-id="15ad5-698">Dies ist ein Duplikat von `az group deployment` und `az group deployment operation`.</span><span class="sxs-lookup"><span data-stu-id="15ad5-698">This is a duplicate of `az group deployment` and `az group deployment operation`</span></span>
* <span data-ttu-id="15ad5-699">`az deployment sub` und `az deployment operation sub` für Vorlagenbereitstellung im Abonnementbereich hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-699">Add `az deployment sub` and `az deployment operation sub` for template deployment at subscription scope.</span></span> <span data-ttu-id="15ad5-700">Dies ist ein Duplikat von `az deployment` und `az deployment operation`.</span><span class="sxs-lookup"><span data-stu-id="15ad5-700">This is a duplicate of `az deployment` and `az deployment operation`</span></span>
* <span data-ttu-id="15ad5-701">`az deployment mg` und `az deployment operation mg` für Vorlagenbereitstellung in Verwaltungsgruppen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-701">Add `az deployment mg` and `az deployment operation mg` for template deployment at management groups</span></span>
* <span data-ttu-id="15ad5-702">`az deployment tenant` und `az deployment operation tenant` für Vorlagenbereitstellung im Mandantenbereich hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-702">Add `az deployment tenant` and `az deployment operation tenant` for template deployment at tenant scope</span></span>
* <span data-ttu-id="15ad5-703">az policy assignment create: Beschreibung zu Parameter `--location` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-703">az policy assignment create: Add a description to the `--location` parameter</span></span>
* <span data-ttu-id="15ad5-704">az group deployment create: Parameter `--aux-tenants` zur mandantenübergreifenden Unterstützung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-704">az group deployment create: Add parameter `--aux-tenants` to support cross tenants</span></span>

### <a name="cdn"></a><span data-ttu-id="15ad5-705">CDN</span><span class="sxs-lookup"><span data-stu-id="15ad5-705">CDN</span></span>

* <span data-ttu-id="15ad5-706">CDN-WAF-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-706">Add CDN WAF commands</span></span>

### <a name="compute"></a><span data-ttu-id="15ad5-707">Compute</span><span class="sxs-lookup"><span data-stu-id="15ad5-707">Compute</span></span>

* <span data-ttu-id="15ad5-708">az sig image-version: „--data-snapshot-luns“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-708">az sig image-version: add --data-snapshot-luns</span></span>
* <span data-ttu-id="15ad5-709">az ppg show: „--colocation-status“ hinzugefügt, um das Abrufen des Zusammenstellungsstatus aller Ressourcen in der Näherungsplatzierungsgruppe zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="15ad5-709">az ppg show: add --colocation-status to enable fetching the colocation status of all the resources in the proximity placement group</span></span>
* <span data-ttu-id="15ad5-710">az vmss create/update: Unterstützung automatischer Reparaturen</span><span class="sxs-lookup"><span data-stu-id="15ad5-710">az vmss create/update: support automatic repairs</span></span>
* <span data-ttu-id="15ad5-711">[BREAKING CHANGE] az image template: „template“ in „builder“ umbenannt</span><span class="sxs-lookup"><span data-stu-id="15ad5-711">[BREAKING CHANGE] az image template: rename template to builder</span></span>
* <span data-ttu-id="15ad5-712">az image builder create: „--image-template“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-712">az image builder create: add --image-template</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="15ad5-713">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="15ad5-713">Cosmos DB</span></span>

* <span data-ttu-id="15ad5-714">Gespeicherte Prozedur „Add Sql“, udf- und trigger-Cmdlets hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-714">Add Sql stored procedure, udf and trigger cmdlets</span></span>
* <span data-ttu-id="15ad5-715">az cosmosdb create: „--key-uri“ hinzugefügt, um das Hinzufügen von Schlüsseltresor-Verschlüsselungsinformationen zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="15ad5-715">az cosmosdb create: add --key-uri to support adding key vault encryption information</span></span>

### <a name="keyvault"></a><span data-ttu-id="15ad5-716">KeyVault</span><span class="sxs-lookup"><span data-stu-id="15ad5-716">KeyVault</span></span>

* <span data-ttu-id="15ad5-717">keyvault create: „soft-delete“ standardmäßig aktiviert</span><span class="sxs-lookup"><span data-stu-id="15ad5-717">keyvault create: enable soft-delete by default</span></span>

### <a name="monitor"></a><span data-ttu-id="15ad5-718">Überwachen</span><span class="sxs-lookup"><span data-stu-id="15ad5-718">Monitor</span></span>

* <span data-ttu-id="15ad5-719">az monitor metrics alert create: Unterstützung von `~` in `--condition`</span><span class="sxs-lookup"><span data-stu-id="15ad5-719">az monitor metrics alert create: support `~` in `--condition`</span></span>

### <a name="network"></a><span data-ttu-id="15ad5-720">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="15ad5-720">Network</span></span>

* <span data-ttu-id="15ad5-721">az network application-gateway rewrite-rule create: Unterstützung der URL-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="15ad5-721">az network application-gateway rewrite-rule create: support url configuration</span></span>
* <span data-ttu-id="15ad5-722">az network dns zone import: Bei „--zone-name“ wird die Groß-/Kleinschreibung künftig nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="15ad5-722">az network dns zone import: --zone-name will be case insensitive in the future</span></span>
* <span data-ttu-id="15ad5-723">az network private-endpoint/private-link-service: Vorschaubezeichnung entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-723">az network private-endpoint/private-link-service: remove preview label</span></span>
* <span data-ttu-id="15ad5-724">az network bastion: Unterstützung von „bastion“</span><span class="sxs-lookup"><span data-stu-id="15ad5-724">az network bastion: support bastion</span></span>
* <span data-ttu-id="15ad5-725">az network vnet list-available-ips: Unterstützung für das Auflisten verfügbarer IPs in einem VNET</span><span class="sxs-lookup"><span data-stu-id="15ad5-725">az network vnet list-available-ips: support list available ips in a vnet</span></span>
* <span data-ttu-id="15ad5-726">az network watcher flow-log create/list/delete/update: neue Befehle hinzugefügt, um Watcher-Datenflussprotokolle zu verwalten und „--location“ zur expliziten Identifizierung von Watcher verfügbar zu machen</span><span class="sxs-lookup"><span data-stu-id="15ad5-726">az network watcher flow-log create/list/delete/update: add new commands to manage watcher flow log and exposing --location to identify watcher explicitly</span></span>
* <span data-ttu-id="15ad5-727">az network watcher flow-log configure: veraltet</span><span class="sxs-lookup"><span data-stu-id="15ad5-727">az network watcher flow-log configure: deprecated</span></span>
* <span data-ttu-id="15ad5-728">az network watcher flow-log show: Unterstützung von „--location“ und „--name“, um ein ARM-formatiertes Ergebnis zu erhalten; alte formatierte Ausgabe als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-728">az network watcher flow-log show: support --location and --name to get ARM-formatted result, deprecated old formatted output</span></span>

### <a name="policy"></a><span data-ttu-id="15ad5-729">Richtlinie</span><span class="sxs-lookup"><span data-stu-id="15ad5-729">Policy</span></span>

* <span data-ttu-id="15ad5-730">az policy assignment create: Fehler behoben, dass automatisch generierter Name der Richtlinienzuweisung den Grenzwert überschreitet</span><span class="sxs-lookup"><span data-stu-id="15ad5-730">az policy assignment create: Fix the bug that automatically generated name of policy assignment exceeds the limit</span></span>

### <a name="rbac"></a><span data-ttu-id="15ad5-731">RBAC</span><span class="sxs-lookup"><span data-stu-id="15ad5-731">RBAC</span></span>

* <span data-ttu-id="15ad5-732">az ad group show: Problem behoben, dass „--group“-Wert als regulärer Ausdruck behandelt wurde</span><span class="sxs-lookup"><span data-stu-id="15ad5-732">az ad group show: fix --group value treated as regex problem</span></span>

### <a name="rdbms"></a><span data-ttu-id="15ad5-733">RDBMS</span><span class="sxs-lookup"><span data-stu-id="15ad5-733">RDBMS</span></span>

* <span data-ttu-id="15ad5-734">SDK-Version von „azure-mgmt-rdbms“ auf 2.0.0 festgelegt</span><span class="sxs-lookup"><span data-stu-id="15ad5-734">Bump the azure-mgmt-rdbms SDK version to 2.0.0</span></span>
* <span data-ttu-id="15ad5-735">az postgres private-endpoint-connection: Verwalten von Verbindungen mit privatem Postgres-Endpunkt</span><span class="sxs-lookup"><span data-stu-id="15ad5-735">az postgres private-endpoint-connection: manage postgres private endpoint connections</span></span>
* <span data-ttu-id="15ad5-736">az postgres private-link-resource: Verwalten von privaten Postgres-Linkressourcen</span><span class="sxs-lookup"><span data-stu-id="15ad5-736">az postgres private-link-resource: manage postgres private link resources</span></span>
* <span data-ttu-id="15ad5-737">az mysql private-endpoint-connection: Verwalten von Verbindungen mit privatem MySQL-Endpunkt</span><span class="sxs-lookup"><span data-stu-id="15ad5-737">az mysql private-endpoint-connection: manage mysql private endpoint connections</span></span>
* <span data-ttu-id="15ad5-738">az mysql private-link-resource: Verwalten von privaten MySQL-Linkressourcen</span><span class="sxs-lookup"><span data-stu-id="15ad5-738">az mysql private-link-resource: manage mysql private link resources</span></span>
* <span data-ttu-id="15ad5-739">az mariadb private-endpoint-connection: Verwalten von Verbindungen mit privatem MariaDB-Endpunkt</span><span class="sxs-lookup"><span data-stu-id="15ad5-739">az mariadb private-endpoint-connection: manage mariadb private endpoint connections</span></span>
* <span data-ttu-id="15ad5-740">az mariadb private-link-resource: Verwalten von privaten MariaDB-Linkressourcen</span><span class="sxs-lookup"><span data-stu-id="15ad5-740">az mariadb private-link-resource: manage mariadb private link resources</span></span>
* <span data-ttu-id="15ad5-741">Aktualisieren von Tests von privaten RDBMS-Endpunkten</span><span class="sxs-lookup"><span data-stu-id="15ad5-741">Updating RDBMS Private Endpoint Tests</span></span>

### <a name="sql"></a><span data-ttu-id="15ad5-742">SQL</span><span class="sxs-lookup"><span data-stu-id="15ad5-742">SQL</span></span>

* <span data-ttu-id="15ad5-743">Sql midb: list-deleted, show-deleted, update-retention, show-retention hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-743">Sql midb Add: list-deleted, show-deleted, update-retention, show-retention</span></span>
* <span data-ttu-id="15ad5-744">(sql server create:) Optionales Flag „Enable“/„Disable“ für public-network-access zu „sql server create“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-744">(sql server create:) Add optional public-network-access 'Enable'/'Disable' flag to sql server create</span></span>
* <span data-ttu-id="15ad5-745">(sql server update): kundenorientierte Änderung vorgenommen</span><span class="sxs-lookup"><span data-stu-id="15ad5-745">(sql server update:) make some customer-facing change</span></span>
* <span data-ttu-id="15ad5-746">Eigenschaft „minimal_tls_version“ für MI und SQL-Datenbank hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-746">Add minimal_tls_version property for MI and SQL DB</span></span>

### <a name="storage"></a><span data-ttu-id="15ad5-747">Storage</span><span class="sxs-lookup"><span data-stu-id="15ad5-747">Storage</span></span>

* <span data-ttu-id="15ad5-748">az storage blob delete-batch: Flag `--dryrun` mit Fehlverhalten</span><span class="sxs-lookup"><span data-stu-id="15ad5-748">az storage blob delete-batch: Misbehaving `--dryrun` flag</span></span>
* <span data-ttu-id="15ad5-749">az storage account network-rule hinzugefügt (Fehlerbehebung): Hinzufügen von Vorgängen muss idempotent sein</span><span class="sxs-lookup"><span data-stu-id="15ad5-749">az storage account network-rule add (bug fix): add operation should be idempotent</span></span>
* <span data-ttu-id="15ad5-750">az storage account create/update: Unterstützung für Routingpräferenz hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-750">az storage account create/update: Add Routing Preference support</span></span>
* <span data-ttu-id="15ad5-751">„azure-mgmt-storage“ auf Version 8.0.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-751">Upgrade azure-mgmt-storage version to 8.0.0</span></span>
* <span data-ttu-id="15ad5-752">az storage container immutability create: Parameter „--allow-protected-append-write“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-752">az storage container immutability create: add --allow-protected-append-write parameter</span></span>
* <span data-ttu-id="15ad5-753">az storage account private-link-resource list: Unterstützung zum Auflisten privater Linkressourcen für Speicherkonto hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-753">az storage account private-link-resource list: Add support to list private link resources for storage account</span></span>
* <span data-ttu-id="15ad5-754">az storage account private-endpoint-connection approve/reject/show/delete: Unterstützung der Verwaltung von Verbindungen mit privaten Endpunkten</span><span class="sxs-lookup"><span data-stu-id="15ad5-754">az storage account private-endpoint-connection approve/reject/show/delete: Support to manage private endpoint connections</span></span>
* <span data-ttu-id="15ad5-755">az storage account blob-service-properties update: „--enable-restore-policy“ und „--restore-days“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-755">az storage account blob-service-properties update: add --enable-restore-policy and --restore-days</span></span>
* <span data-ttu-id="15ad5-756">az storage blob restore: Unterstützung für die Wiederherstellung von Blobbereichen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-756">az storage blob restore: Add support to restore blob ranges</span></span>

## <a name="february-18-2020"></a><span data-ttu-id="15ad5-757">18. Februar 2020</span><span class="sxs-lookup"><span data-stu-id="15ad5-757">February 18, 2020</span></span>

<span data-ttu-id="15ad5-758">Version 2.1.0</span><span class="sxs-lookup"><span data-stu-id="15ad5-758">Version 2.1.0</span></span>

### <a name="acr"></a><span data-ttu-id="15ad5-759">ACR</span><span class="sxs-lookup"><span data-stu-id="15ad5-759">ACR</span></span>

* <span data-ttu-id="15ad5-760">Neues Argument `--expose-token` für `az acr login` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-760">Add a new argument `--expose-token` for `az acr login`</span></span>
* <span data-ttu-id="15ad5-761">Falsche Ausgabe für `az acr task identity show -n Name -r Registry -o table` korrigiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-761">Fix the incorrect output of `az acr task identity show -n Name -r Registry -o table`</span></span>
* <span data-ttu-id="15ad5-762">az acr login: Auslösen von „CLIError“, wenn vom Docker-Befehl Fehler zurückgegeben werden</span><span class="sxs-lookup"><span data-stu-id="15ad5-762">az acr login: Throw a CLIError if there are errors returned by docker command</span></span>

### <a name="acs"></a><span data-ttu-id="15ad5-763">ACS</span><span class="sxs-lookup"><span data-stu-id="15ad5-763">ACS</span></span>

* <span data-ttu-id="15ad5-764">aks create/update: Validierung für `--vnet-subnet-id` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-764">aks create/update: add `--vnet-subnet-id` validation</span></span>

### <a name="aladdin"></a><span data-ttu-id="15ad5-765">Aladdin</span><span class="sxs-lookup"><span data-stu-id="15ad5-765">Aladdin</span></span>

* <span data-ttu-id="15ad5-766">Analysieren der generierten Beispiele in „_help.py“ der Befehle</span><span class="sxs-lookup"><span data-stu-id="15ad5-766">Parse generated examples into commands' _help.py</span></span>

### <a name="ams"></a><span data-ttu-id="15ad5-767">AMS</span><span class="sxs-lookup"><span data-stu-id="15ad5-767">AMS</span></span>

* <span data-ttu-id="15ad5-768">az ams ist jetzt allgemein verfügbar.</span><span class="sxs-lookup"><span data-stu-id="15ad5-768">az ams is GA now</span></span>

### <a name="appconfig"></a><span data-ttu-id="15ad5-769">AppConfig</span><span class="sxs-lookup"><span data-stu-id="15ad5-769">AppConfig</span></span>

* <span data-ttu-id="15ad5-770">Hilfenachricht überarbeitet, um nicht unterstützte Schlüssel-/Bezeichnungsfilter auszuschließen</span><span class="sxs-lookup"><span data-stu-id="15ad5-770">Revise help message to exclude unsupported key/label filter</span></span>
* <span data-ttu-id="15ad5-771">Vorschautag für die meisten Befehle entfernt (mit Ausnahme der Flags für verwaltete Identitäten und Features)</span><span class="sxs-lookup"><span data-stu-id="15ad5-771">Remove preview tag for most commands excluding managed identity and feature flags</span></span>
* <span data-ttu-id="15ad5-772">Kundenseitig verwalteter Schlüssel beim Aktualisieren der Speicher hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-772">Add customer managed key when updating stores</span></span>

### <a name="appservice"></a><span data-ttu-id="15ad5-773">AppService</span><span class="sxs-lookup"><span data-stu-id="15ad5-773">AppService</span></span>

* <span data-ttu-id="15ad5-774">az webapp list-runtimes: Fehler bei „list-runtimes“ behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-774">az webapp list-runtimes: Fix the bug for list-runtimes</span></span>
* <span data-ttu-id="15ad5-775">„az webapp|functionapp config ssl create“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-775">Add az webapp|functionapp config ssl create</span></span>
* <span data-ttu-id="15ad5-776">Unterstützung für v3-Funktions-Apps und Node 12</span><span class="sxs-lookup"><span data-stu-id="15ad5-776">Add support for v3 function apps and node 12</span></span>

### <a name="arm"></a><span data-ttu-id="15ad5-777">ARM</span><span class="sxs-lookup"><span data-stu-id="15ad5-777">ARM</span></span>

* <span data-ttu-id="15ad5-778">az policy assignment create: Fehlermeldung korrigiert, die angezeigt wird, wenn der Parameter `--policy` ungültig ist</span><span class="sxs-lookup"><span data-stu-id="15ad5-778">az policy assignment create: Fix the error message when the `--policy` parameter is invalid</span></span>
* <span data-ttu-id="15ad5-779">az group deployment create: Fehler „stat: path too long for Windows" korrigiert, der angezeigt wird, wenn eine zu große Datei vom Typ „parameters.json“ verwendet wird</span><span class="sxs-lookup"><span data-stu-id="15ad5-779">az group deployment create: Fix "stat: path too long for Windows" error when using large parameters.json file</span></span>

### <a name="backup"></a><span data-ttu-id="15ad5-780">Backup</span><span class="sxs-lookup"><span data-stu-id="15ad5-780">Backup</span></span>

* <span data-ttu-id="15ad5-781">Korrektur des Wiederherstellungsflows auf Elementebene am ursprünglichen Speicherort</span><span class="sxs-lookup"><span data-stu-id="15ad5-781">Fix for item level recovery flow in OLR</span></span>
* <span data-ttu-id="15ad5-782">Unterstützung von „Als Dateien wiederherstellen“ für SQL- und SAP-Datenbanken hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-782">Add restore as files support for SQL and SAP Databases</span></span>

### <a name="compute"></a><span data-ttu-id="15ad5-783">Compute</span><span class="sxs-lookup"><span data-stu-id="15ad5-783">Compute</span></span>

* <span data-ttu-id="15ad5-784">vm/vmss/availability-set update: „--ppg“ hinzugefügt, um die Aktualisierung von „ProximityPlacementGroup“ zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="15ad5-784">vm/vmss/availability-set update: add --ppg to allowing updating ProximityPlacementGroup</span></span>
* <span data-ttu-id="15ad5-785">vmss create: „--data-disk-iops“ und „--data-disk-mbps“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-785">vmss create: add --data-disk-iops and --data-disk-mbps</span></span>
* <span data-ttu-id="15ad5-786">az vm host: Vorschautag für `vm host` und `vm host group` entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-786">az vm host: remove preview tag for `vm host` and `vm host group`</span></span>
* <span data-ttu-id="15ad5-787">[BREAKING CHANGE] Behebung Nr. 10728: `az vm create`: Automatisches Erstellen des Subnetzes, wenn das VNET angegeben wird und das Subnetz nicht vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="15ad5-787">[BREAKING CHANGE] Fix #10728: `az vm create`: create subnet automatically if vnet is specified and subnet not exists</span></span>
* <span data-ttu-id="15ad5-788">Erhöhen der Stabilität von „vm image list“</span><span class="sxs-lookup"><span data-stu-id="15ad5-788">Increase robustness of vm image list</span></span>

### <a name="eventhub"></a><span data-ttu-id="15ad5-789">Eventhub</span><span class="sxs-lookup"><span data-stu-id="15ad5-789">Eventhub</span></span>

* <span data-ttu-id="15ad5-790">Azure Stack-Unterstützung für Profil „2019-03-01-hybrid“</span><span class="sxs-lookup"><span data-stu-id="15ad5-790">Azure Stack support for 2019-03-01-hybrid profile</span></span>

### <a name="keyvault"></a><span data-ttu-id="15ad5-791">KeyVault</span><span class="sxs-lookup"><span data-stu-id="15ad5-791">KeyVault</span></span>

* <span data-ttu-id="15ad5-792">az keyvault key create: neuer Wert `import` für Parameter `--ops` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-792">az keyvault key create: add a new value `import` for parameter `--ops`</span></span>
* <span data-ttu-id="15ad5-793">az keyvault key list-versions: Unterstützung des Parameters `--id` für die Angabe von Schlüsseln</span><span class="sxs-lookup"><span data-stu-id="15ad5-793">az keyvault key list-versions: support parameter `--id` for specifying keys</span></span>
* <span data-ttu-id="15ad5-794">Unterstützung für Verbindungen mit privaten Endpunkten</span><span class="sxs-lookup"><span data-stu-id="15ad5-794">Support private endpoint connections</span></span>

### <a name="network"></a><span data-ttu-id="15ad5-795">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="15ad5-795">Network</span></span>

* <span data-ttu-id="15ad5-796">Geändert in „azure-mgmt-network 9.0.0“</span><span class="sxs-lookup"><span data-stu-id="15ad5-796">Bump to azure-mgmt-network 9.0.0</span></span>
* <span data-ttu-id="15ad5-797">az network private-link-service update/create: Unterstützung von „--enable-proxy-protocol“</span><span class="sxs-lookup"><span data-stu-id="15ad5-797">az network private-link-service update/create: support --enable-proxy-protocol</span></span>
* <span data-ttu-id="15ad5-798">Feature für Version 2 von Verbindungsmonitor hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-798">Add connection Monitor V2 feature</span></span>

### <a name="packaging"></a><span data-ttu-id="15ad5-799">Verpackung</span><span class="sxs-lookup"><span data-stu-id="15ad5-799">Packaging</span></span>

* <span data-ttu-id="15ad5-800">[BREAKING CHANGE] Unterstützung für Python 2.7 eingestellt</span><span class="sxs-lookup"><span data-stu-id="15ad5-800">[BREAKING CHANGE] Drop support for Python 2.7</span></span>

### <a name="profile"></a><span data-ttu-id="15ad5-801">Profil</span><span class="sxs-lookup"><span data-stu-id="15ad5-801">Profile</span></span>

* <span data-ttu-id="15ad5-802">Vorschau: Neue Attribute `homeTenantId` und `managedByTenants` zu Abonnementkonten hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-802">Preview: Add new attributes `homeTenantId` and `managedByTenants` to subscription accounts.</span></span> <span data-ttu-id="15ad5-803">Führen Sie `az login` erneut aus, damit die Änderungen wirksam werden.</span><span class="sxs-lookup"><span data-stu-id="15ad5-803">Please re-run `az login` for the changes to take effect</span></span>
* <span data-ttu-id="15ad5-804">az login: Eine Warnung wird angezeigt, wenn ein Abonnement von mehren Mandanten aufgeführt wird und der erste als Standard festgelegt wird.</span><span class="sxs-lookup"><span data-stu-id="15ad5-804">az login: Show a warning when a subscription is listed from more than one tenants and default to the first one.</span></span> <span data-ttu-id="15ad5-805">Fügen Sie `--tenant` in `az login` ein, um beim Zugreifen auf dieses Abonnement einen bestimmten Mandanten auszuwählen.</span><span class="sxs-lookup"><span data-stu-id="15ad5-805">To select a specific tenant when accessing this subscription, please include `--tenant` in `az login`</span></span>

### <a name="role"></a><span data-ttu-id="15ad5-806">Role</span><span class="sxs-lookup"><span data-stu-id="15ad5-806">Role</span></span>

* <span data-ttu-id="15ad5-807">az role assignment create: Problem behoben, das beim Zuweisen einer Rolle zu einem Dienstprinzipal nach Anzeigename einen Fehler vom Typ „HTTP 400“ verursachte</span><span class="sxs-lookup"><span data-stu-id="15ad5-807">az role assignment create: Fix the error that assigning a role to a service principal by display name yields a HTTP 400</span></span>

### <a name="sql"></a><span data-ttu-id="15ad5-808">SQL</span><span class="sxs-lookup"><span data-stu-id="15ad5-808">SQL</span></span>

* <span data-ttu-id="15ad5-809">Cmdlet `az sql mi update` der verwalteten SQL-Instanz mit zwei neuen Parametern aktualisiert: tier und family</span><span class="sxs-lookup"><span data-stu-id="15ad5-809">Update SQL Managed Instance cmdlet `az sql mi update` with two new parameters: tier and family</span></span>

### <a name="storage"></a><span data-ttu-id="15ad5-810">Storage</span><span class="sxs-lookup"><span data-stu-id="15ad5-810">Storage</span></span>

* <span data-ttu-id="15ad5-811">[BREAKING CHANGE] `az storage account create`: Art des Standardspeicherkontos in StorageV2 geändert</span><span class="sxs-lookup"><span data-stu-id="15ad5-811">[BREAKING CHANGE] `az storage account create`: Change default storage account kind to StorageV2</span></span>

## <a name="february-04-2020"></a><span data-ttu-id="15ad5-812">04. Februar 2020</span><span class="sxs-lookup"><span data-stu-id="15ad5-812">February 04, 2020</span></span>

<span data-ttu-id="15ad5-813">Version 2.0.81</span><span class="sxs-lookup"><span data-stu-id="15ad5-813">Version 2.0.81</span></span>

### <a name="acs"></a><span data-ttu-id="15ad5-814">ACS</span><span class="sxs-lookup"><span data-stu-id="15ad5-814">ACS</span></span>

* <span data-ttu-id="15ad5-815">Unterstützung für das Festlegen zugeordneter Ausgangsports und Leerlauftimeouts für Load Balancer Standard hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-815">Add support to set outbound allocated ports and idle timeouts on standard load balancer</span></span>
* <span data-ttu-id="15ad5-816">Aktualisierung auf API-Version 2019-11-01</span><span class="sxs-lookup"><span data-stu-id="15ad5-816">Update to API Version 2019-11-01</span></span>

### <a name="acr"></a><span data-ttu-id="15ad5-817">ACR</span><span class="sxs-lookup"><span data-stu-id="15ad5-817">ACR</span></span>

* <span data-ttu-id="15ad5-818">[BREAKING CHANGE] `az acr delete` löst eine Eingabeaufforderung aus.</span><span class="sxs-lookup"><span data-stu-id="15ad5-818">[BREAKING CHANGE] `az acr delete` will prompt</span></span>
* <span data-ttu-id="15ad5-819">[BREAKING CHANGE] „az acr task delete“ löst eine Eingabeaufforderung aus.</span><span class="sxs-lookup"><span data-stu-id="15ad5-819">[BREAKING CHANGE] 'az acr task delete' will prompt</span></span>
* <span data-ttu-id="15ad5-820">Neue Befehlsgruppe „az acr taskrun show/list/delete“ für die Aufgabenausführungsverwaltung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-820">Add a new command group 'az acr taskrun show/list/delete' for taskrun management</span></span>

### <a name="aks"></a><span data-ttu-id="15ad5-821">AKS</span><span class="sxs-lookup"><span data-stu-id="15ad5-821">AKS</span></span>

* <span data-ttu-id="15ad5-822">Jeder Cluster erhält einen separaten Dienstprinzipal zur Verbesserung der Isolation.</span><span class="sxs-lookup"><span data-stu-id="15ad5-822">Each cluster gets a separate service principal to improve isolation</span></span>

### <a name="appconfig"></a><span data-ttu-id="15ad5-823">AppConfig</span><span class="sxs-lookup"><span data-stu-id="15ad5-823">AppConfig</span></span>

* <span data-ttu-id="15ad5-824">Unterstützung für den Import/Export von KeyVault-Verweisen in/aus AppService</span><span class="sxs-lookup"><span data-stu-id="15ad5-824">Support import/export of keyvault references from/to appservice</span></span>
* <span data-ttu-id="15ad5-825">Unterstützung für den Import/Export aller Bezeichnungen in appconfig und aus appconfig</span><span class="sxs-lookup"><span data-stu-id="15ad5-825">Support import/export of all labels from appconfig to appconfig</span></span>
* <span data-ttu-id="15ad5-826">Überprüfen der Schlüssel- und Featurenamen vor dem Festlegen und Importieren</span><span class="sxs-lookup"><span data-stu-id="15ad5-826">Validate key and feature names before setting and importing</span></span>
* <span data-ttu-id="15ad5-827">Verfügbarmachen der SKU-Änderung für den Konfigurationsspeicher</span><span class="sxs-lookup"><span data-stu-id="15ad5-827">Expose sku modification for configuration store.</span></span>
* <span data-ttu-id="15ad5-828">Befehlsgruppe für die verwaltete Identität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-828">Add command group for managed identity.</span></span>

### <a name="appservice"></a><span data-ttu-id="15ad5-829">AppService</span><span class="sxs-lookup"><span data-stu-id="15ad5-829">AppService</span></span>

* <span data-ttu-id="15ad5-830">Azure Stack: Oberflächenbefehle im Profil „2019-03-01-hybrid“</span><span class="sxs-lookup"><span data-stu-id="15ad5-830">Azure Stack: surface commands under the profile of 2019-03-01-hybrid</span></span>
* <span data-ttu-id="15ad5-831">functionapp: Funktion zum Erstellen von Java-Funktions-Apps in Linux hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-831">functionapp: Add ability to create Java function apps in Linux</span></span>

### <a name="arm"></a><span data-ttu-id="15ad5-832">ARM</span><span class="sxs-lookup"><span data-stu-id="15ad5-832">ARM</span></span>

* <span data-ttu-id="15ad5-833">Behebung von Problem Nr. 10246: `az resource tag` stürzt ab, wenn der übergebene Parameter `--ids` der Ressourcengruppen-ID entspricht.</span><span class="sxs-lookup"><span data-stu-id="15ad5-833">Fix issue #10246: `az resource tag` crashes when the parameter `--ids` passed in is resource group ID</span></span>
* <span data-ttu-id="15ad5-834">Behebung von Problem Nr. 11658: Der Befehl `az group export` unterstützt die Parameter `--query` und `--output` nicht.</span><span class="sxs-lookup"><span data-stu-id="15ad5-834">Fix issue #11658: `az group export` command does not support `--query` and `--output` parameters</span></span>
* <span data-ttu-id="15ad5-835">Behebung von Problem Nr. 10279: Der Exitcode von `az group deployment validate` ist 0, wenn bei der Überprüfung ein Fehler auftritt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-835">Fix issue #10279: The exit code of `az group deployment validate` is 0 when the verification fails</span></span>
* <span data-ttu-id="15ad5-836">Behebung von Problem Nr. 9916: Fehlermeldung des Konflikts zwischen Tag und anderen Filterbedingungen für Befehl `az resource list` verbessert</span><span class="sxs-lookup"><span data-stu-id="15ad5-836">Fix issue #9916: Improve the error message of the conflict between tag and other filter conditions for `az resource list` command</span></span>
* <span data-ttu-id="15ad5-837">Neuer Parameter `--managed-by` hinzugefügt, um das Hinzufügen der Informationen vom Typ „managedBy“ für Befehl `az group create` zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="15ad5-837">Add new parameter `--managed-by` to support adding managedBy information for command `az group create`</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="15ad5-838">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="15ad5-838">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="15ad5-839">Untergruppe `monitor` hinzugefügt, um Log Analytics-Überwachung im Azure Red Hat OpenShift-Cluster zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="15ad5-839">Add `monitor` subgroup to manage Log Analytics monitoring in Azure Red Hat OpensShift cluster</span></span>

### <a name="botservice"></a><span data-ttu-id="15ad5-840">BotService</span><span class="sxs-lookup"><span data-stu-id="15ad5-840">BotService</span></span>

* <span data-ttu-id="15ad5-841">Behebung von Problem Nr. 11697: `az bot create` ist nicht idempotent.</span><span class="sxs-lookup"><span data-stu-id="15ad5-841">Fix issue #11697: `az bot create` is not idempotent</span></span>
* <span data-ttu-id="15ad5-842">Tests zur Namenskorrektur geändert, sodass sie nur im Livemodus ausgeführt werden</span><span class="sxs-lookup"><span data-stu-id="15ad5-842">Change name-correcting tests to run in Live-mode only</span></span>

### <a name="cdn"></a><span data-ttu-id="15ad5-843">CDN</span><span class="sxs-lookup"><span data-stu-id="15ad5-843">CDN</span></span>

* <span data-ttu-id="15ad5-844">Unterstützung für das rulesEngine-Feature hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-844">Add support for rulesEngine feature</span></span>
* <span data-ttu-id="15ad5-845">Neue Befehlsgruppe „cdn endpoint rule“ zum Verwalten von Regeln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-845">Add new commands group 'cdn endpoint rule' to manage rules</span></span>
* <span data-ttu-id="15ad5-846">azure-mgmt-cdn-Version auf 4.0.0 aktualisiert, um API-Version 2019-04-15 zu verwenden</span><span class="sxs-lookup"><span data-stu-id="15ad5-846">Update azure-mgmt-cdn version to 4.0.0 to use api version 2019-04-15</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="15ad5-847">Bereitstellungs-Manager</span><span class="sxs-lookup"><span data-stu-id="15ad5-847">Deployment Manager</span></span>

* <span data-ttu-id="15ad5-848">Auflistungsvorgang für alle Ressourcen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-848">Add list operation for all resources.</span></span>
* <span data-ttu-id="15ad5-849">Schrittressource für neuen Schritttyp optimiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-849">Enhance step resource for new step type.</span></span>
* <span data-ttu-id="15ad5-850">Paket „azure-mgmt-deploymentmanager“ zur Verwendung von Version 0.2.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-850">Update azure-mgmt-deploymentmanager package to use version 0.2.0.</span></span>

### <a name="iot"></a><span data-ttu-id="15ad5-851">IoT</span><span class="sxs-lookup"><span data-stu-id="15ad5-851">IoT</span></span>

* <span data-ttu-id="15ad5-852">Befehle vom Typ „IoT hub Job“ als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="15ad5-852">Deprecate 'IoT hub Job' commands.</span></span>

### <a name="iot-central"></a><span data-ttu-id="15ad5-853">IoT Central</span><span class="sxs-lookup"><span data-stu-id="15ad5-853">IoT Central</span></span>

* <span data-ttu-id="15ad5-854">Unterstützung der App-Erstellung/-Aktualisierung mit neuem SKU-Namen ST0, ST1, ST2</span><span class="sxs-lookup"><span data-stu-id="15ad5-854">Support app creation/update with the new sku name ST0, ST1, ST2.</span></span>

### <a name="key-vault"></a><span data-ttu-id="15ad5-855">Key Vault</span><span class="sxs-lookup"><span data-stu-id="15ad5-855">Key Vault</span></span>

* <span data-ttu-id="15ad5-856">Neuer Befehl `az keyvault key download` zum Herunterladen von Schlüsseln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-856">Add a new command `az keyvault key download` for downloading keys.</span></span>

### <a name="misc"></a><span data-ttu-id="15ad5-857">Sonstiges</span><span class="sxs-lookup"><span data-stu-id="15ad5-857">Misc</span></span>

* <span data-ttu-id="15ad5-858">Behebung Nr. 6371: Unterstützung für die Vervollständigung von Dateinamen und Umgebungsvariablen in Bash</span><span class="sxs-lookup"><span data-stu-id="15ad5-858">Fix #6371: Support filename and environment variable completion in Bash</span></span>

### <a name="network"></a><span data-ttu-id="15ad5-859">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="15ad5-859">Network</span></span>

* <span data-ttu-id="15ad5-860">Behebung Nr. 2092: az network dns record-set add/remove: Warnung hinzugefügt, wenn Datensatzgruppe nicht gefunden wurde.</span><span class="sxs-lookup"><span data-stu-id="15ad5-860">Fix #2092: az network dns record-set add/remove: add warning when record-set is not found.</span></span> <span data-ttu-id="15ad5-861">In Zukunft wird ein zusätzliches Argument unterstützt, um diese automatische Erstellung zu bestätigen.</span><span class="sxs-lookup"><span data-stu-id="15ad5-861">In the future, an extra argument will be supported to confirm this auto creation.</span></span>

### <a name="policy"></a><span data-ttu-id="15ad5-862">Richtlinie</span><span class="sxs-lookup"><span data-stu-id="15ad5-862">Policy</span></span>

* <span data-ttu-id="15ad5-863">Neuer Befehl `az policy metadata` hinzugefügt, um umfangreiche Richtlinienmetadatenressourcen abzurufen</span><span class="sxs-lookup"><span data-stu-id="15ad5-863">Add new command `az policy metadata` to retrieve rich policy metadata resources</span></span>
* <span data-ttu-id="15ad5-864">`az policy remediation create`: Geben Sie mit dem Parameter `--resource-discovery-mode` an, ob die Konformität vor der Wartung neu bewertet werden soll.</span><span class="sxs-lookup"><span data-stu-id="15ad5-864">`az policy remediation create`: Specify whether compliance should be re-evaluated prior to remediation with the `--resource-discovery-mode` parameter</span></span>

### <a name="profile"></a><span data-ttu-id="15ad5-865">Profil</span><span class="sxs-lookup"><span data-stu-id="15ad5-865">Profile</span></span>

* <span data-ttu-id="15ad5-866">`az account get-access-token`: Parameter `--tenant` hinzugefügt, um das Token für den Mandanten direkt abzurufen. Es muss kein Abonnement angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="15ad5-866">`az account get-access-token`: Add `--tenant` parameter to acquire token for the tenant directly, needless to specify a subscription</span></span>

### <a name="rbac"></a><span data-ttu-id="15ad5-867">RBAC</span><span class="sxs-lookup"><span data-stu-id="15ad5-867">RBAC</span></span>

* <span data-ttu-id="15ad5-868">[BREAKING CHANGE] Behebung Nr. 11883: `az role assignment create`: Bei leerem Bereich wird ein Fehler ausgegeben.</span><span class="sxs-lookup"><span data-stu-id="15ad5-868">[BREAKING CHANGE] Fix #11883: `az role assignment create`: empty scope will prompt error</span></span>

### <a name="security"></a><span data-ttu-id="15ad5-869">Sicherheit</span><span class="sxs-lookup"><span data-stu-id="15ad5-869">Security</span></span>

* <span data-ttu-id="15ad5-870">Neue Befehle `az atp show` und `az atp update` hinzugefügt, um erweiterte Einstellungen für den Bedrohungsschutz für Speicherkonten anzuzeigen und zu verwalten</span><span class="sxs-lookup"><span data-stu-id="15ad5-870">Add new commands `az atp show` and `az atp update` to view and manage advanced threat protection settings for storage accounts.</span></span>

### <a name="sql"></a><span data-ttu-id="15ad5-871">SQL</span><span class="sxs-lookup"><span data-stu-id="15ad5-871">SQL</span></span>

* <span data-ttu-id="15ad5-872">`sql dw create`: Parameter `--zone-redundant` und `--read-replica-count` als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="15ad5-872">`sql dw create`: deprecate `--zone-redundant` and `--read-replica-count` parameters.</span></span> <span data-ttu-id="15ad5-873">Diese Parameter gelten nicht für Datawarehouse.</span><span class="sxs-lookup"><span data-stu-id="15ad5-873">These parameters do not apply to DataWarehouse.</span></span>
* <span data-ttu-id="15ad5-874">[BREAKING CHANGE] `az sql db create`: „WideWorldImportersStd“ und „WideWorldImportersFull“ als dokumentierte zulässige Werte für „az sql db create --sample-name“ entfernt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-874">[BREAKING CHANGE] `az sql db create`: Remove "WideWorldImportersStd" and "WideWorldImportersFull" as documented allowed values for "az sql db create --sample-name".</span></span> <span data-ttu-id="15ad5-875">Diese Beispieldatenbanken führen immer zu einem Fehler bei der Erstellung.</span><span class="sxs-lookup"><span data-stu-id="15ad5-875">These sample databases would always cause creation to fail.</span></span>
* <span data-ttu-id="15ad5-876">Neue Befehle `sql db classification show/list/update/delete` und `sql db classification recommendation list/enable/disable` zur Verwaltung von Vertraulichkeitsklassifizierungen für SQL-Datenbanken hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-876">Add New commands `sql db classification show/list/update/delete` and `sql db classification recommendation list/enable/disable` to manage sensitivity classifications for SQL databases.</span></span>
* <span data-ttu-id="15ad5-877">`az sql db audit-policy`: Behebung für leere Überwachungsaktionen und -gruppen</span><span class="sxs-lookup"><span data-stu-id="15ad5-877">`az sql db audit-policy`: Fix for empty audit actions and groups</span></span>

### <a name="storage"></a><span data-ttu-id="15ad5-878">Storage</span><span class="sxs-lookup"><span data-stu-id="15ad5-878">Storage</span></span>

* <span data-ttu-id="15ad5-879">Neue Befehlsgruppe `az storage share-rm` hinzugefügt, um den Ressourcenanbieter „Microsoft.Storage“ für Verwaltungsvorgänge der Azure-Dateifreigabe zu verwenden</span><span class="sxs-lookup"><span data-stu-id="15ad5-879">Add a new command group `az storage share-rm` to use the Microsoft.Storage resource provider for Azure file share management operations.</span></span>
* <span data-ttu-id="15ad5-880">Behebung für Problem Nr. 11415: Berechtigungsfehler für `az storage blob update`</span><span class="sxs-lookup"><span data-stu-id="15ad5-880">Fix issue #11415: permission error for `az storage blob update`</span></span>
* <span data-ttu-id="15ad5-881">Integration von Azcopy 10.3.3 und Unterstützung von Win32</span><span class="sxs-lookup"><span data-stu-id="15ad5-881">Integrate Azcopy 10.3.3 and support Win32.</span></span>
* <span data-ttu-id="15ad5-882">`az storage copy`: Parameter `--include-path`, `--include-pattern`, `--exclude-path` und`--exclude-pattern` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-882">`az storage copy`: Add `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="15ad5-883">`az storage remove`: Parameter `--inlcude` und `--exclude` in Parameter `--include-path`, `--include-pattern`, `--exclude-path` und`--exclude-pattern` geändert</span><span class="sxs-lookup"><span data-stu-id="15ad5-883">`az storage remove`: Change `--inlcude` and `--exclude` parameters to `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="15ad5-884">`az storage sync`: Parameter `--include-pattern`, `--exclude-path` und`--exclude-pattern` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-884">`az storage sync`: Add `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>

### <a name="servicefabric"></a><span data-ttu-id="15ad5-885">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="15ad5-885">ServiceFabric</span></span>

* <span data-ttu-id="15ad5-886">Neue Befehle zum Verwalten von Anwendung und Diensten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-886">Add new commands to manage appliaction and services.</span></span>

## <a name="january-13-2020"></a><span data-ttu-id="15ad5-887">13. Januar 2020</span><span class="sxs-lookup"><span data-stu-id="15ad5-887">January 13, 2020</span></span>

<span data-ttu-id="15ad5-888">Version 2.0.80</span><span class="sxs-lookup"><span data-stu-id="15ad5-888">Version 2.0.80</span></span>

### <a name="compute"></a><span data-ttu-id="15ad5-889">Compute</span><span class="sxs-lookup"><span data-stu-id="15ad5-889">Compute</span></span>

* <span data-ttu-id="15ad5-890">Datenträgeraktualisierung: „--disk-encryption-set“ und „--encryption-type“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-890">disk update: Add --disk-encryption-set and --encryption-type</span></span>
* <span data-ttu-id="15ad5-891">Momentaufnahmeerstellung/-aktualisierung: „--disk-encryption-set“ und „--encryption-type“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-891">snapshot create/update: Add --disk-encryption-set and --encryption-type</span></span>

### <a name="storage"></a><span data-ttu-id="15ad5-892">Storage</span><span class="sxs-lookup"><span data-stu-id="15ad5-892">Storage</span></span>

* <span data-ttu-id="15ad5-893">„azure-mgmt-storage“ auf Version 7.1.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-893">Upgrade azure-mgmt-storage version to 7.1.0</span></span>
* <span data-ttu-id="15ad5-894">`az storage account create`: `--encryption-key-type-for-table` und `--encryption-key-type-for-queue` zur Unterstützung des Tabellen- und Warteschlangenverschlüsselungsdiensts hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-894">`az storage account create`: Add `--encryption-key-type-for-table` and `--encryption-key-type-for-queue` to support Table and Queue Encryption Service</span></span>

## <a name="january-07-2020"></a><span data-ttu-id="15ad5-895">7\. Januar 2020</span><span class="sxs-lookup"><span data-stu-id="15ad5-895">January 07, 2020</span></span>

<span data-ttu-id="15ad5-896">Version 2.0.79</span><span class="sxs-lookup"><span data-stu-id="15ad5-896">Version 2.0.79</span></span>

### <a name="acr"></a><span data-ttu-id="15ad5-897">ACR</span><span class="sxs-lookup"><span data-stu-id="15ad5-897">ACR</span></span>

* <span data-ttu-id="15ad5-898">[BREAKING CHANGE] Parameter „--os“ für „acr build“, „acr task create/update“, „acr run“ und „acr pack“ wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-898">[BREAKING CHANGE] Remove '--os' parameter for 'acr build', 'acr task create/update', 'acr run', and 'acr pack'.</span></span> <span data-ttu-id="15ad5-899">Verwenden Sie stattdessen „--platform“.</span><span class="sxs-lookup"><span data-stu-id="15ad5-899">Use '--platform' instead.</span></span>

### <a name="appconfig"></a><span data-ttu-id="15ad5-900">AppConfig</span><span class="sxs-lookup"><span data-stu-id="15ad5-900">AppConfig</span></span>

* <span data-ttu-id="15ad5-901">Unterstützung für das Importieren/Exportieren von Featureflags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-901">Add support for importing/exporting feature flags</span></span>
* <span data-ttu-id="15ad5-902">Neuer Befehl „az appconfig kv set-keyvault“ für das Erstellen einer KeyVault-Referenz hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-902">Add new command 'az appconfig kv set-keyvault' for creating keyvault reference</span></span>
* <span data-ttu-id="15ad5-903">Unterstützung verschiedener Benennungskonventionen beim Exportieren von Featureflags in eine Datei</span><span class="sxs-lookup"><span data-stu-id="15ad5-903">Support various naming conventions when exporting feature flags to file</span></span>

### <a name="appservice"></a><span data-ttu-id="15ad5-904">AppService</span><span class="sxs-lookup"><span data-stu-id="15ad5-904">AppService</span></span>

* <span data-ttu-id="15ad5-905">Behebung von Problem Nr. 7154: Aktualisierung der Dokumentation für Befehl „<>“, sodass Backticks anstelle von einfachen Anführungszeichen verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="15ad5-905">Fix issue #7154: Updating documentation for command <> to use back ticks instead of single quotes</span></span>
* <span data-ttu-id="15ad5-906">Behebung von Problem Nr. 11287: „webapp up“: Für die mit „up“ erstellte App muss standardmäßig SSL aktiviert sein.</span><span class="sxs-lookup"><span data-stu-id="15ad5-906">Fix issue #11287: webapp up: By default make the app created using up 'should be 'SSL enabled'</span></span>
* <span data-ttu-id="15ad5-907">Behebung von Problem Nr. 11592: Flag „az webapp up“ für statische HTML-Websites hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-907">Fix issue #11592: Add az webapp up flag for html static sites</span></span>

### <a name="arm"></a><span data-ttu-id="15ad5-908">ARM</span><span class="sxs-lookup"><span data-stu-id="15ad5-908">ARM</span></span>

* <span data-ttu-id="15ad5-909">Behebung `az resource tag`: Recovery Services-Tresor-Tags können nicht aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="15ad5-909">Fix `az resource tag`: Recovery Services Vault tags cannot be updated</span></span>

### <a name="backup"></a><span data-ttu-id="15ad5-910">Backup</span><span class="sxs-lookup"><span data-stu-id="15ad5-910">Backup</span></span>

* <span data-ttu-id="15ad5-911">Neuer Befehl „backup protection undelete“ hinzugefügt, um die Funktion zum vorläufigen Löschen für IaasVM-Workloads zu aktivieren</span><span class="sxs-lookup"><span data-stu-id="15ad5-911">Added new command 'backup protection undelete' to enable soft-delete feature for IaasVM workload</span></span>
* <span data-ttu-id="15ad5-912">Neuer Parameter „--soft-delete-feature-state“ hinzugefügt, um den Befehl „backup-properties“ festzulegen</span><span class="sxs-lookup"><span data-stu-id="15ad5-912">Added new parameter '--soft-delete-feature-state' to set backup-properties command</span></span>
* <span data-ttu-id="15ad5-913">Unterstützung für den Ausschluss von Datenträgern für IaasVM-Workload hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-913">Added disk exclusion support for IaasVM workload</span></span>

### <a name="compute"></a><span data-ttu-id="15ad5-914">Compute</span><span class="sxs-lookup"><span data-stu-id="15ad5-914">Compute</span></span>

* <span data-ttu-id="15ad5-915">Fehler `vm create` in Azure Stack-Profil behoben.</span><span class="sxs-lookup"><span data-stu-id="15ad5-915">Fix `vm create` failure in Azure Stack profile.</span></span>
* <span data-ttu-id="15ad5-916">vm monitor metrics tail/list-definitions: Unterstützung einer Abfragemetrik und von Listendefinitionen für eine VM.</span><span class="sxs-lookup"><span data-stu-id="15ad5-916">vm monitor metrics tail/list-definitions: support query metric and list definitions for a vm.</span></span>
* <span data-ttu-id="15ad5-917">Neue Aktion des Befehls zum erneuten Anwenden für „az vm“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-917">Add new reapply command action for az vm</span></span>

### <a name="hdinsight"></a><span data-ttu-id="15ad5-918">HDInsight</span><span class="sxs-lookup"><span data-stu-id="15ad5-918">HDInsight</span></span>

* <span data-ttu-id="15ad5-919">Unterstützung für das Erstellen eines Kafka-Clusters mit Kafka-REST-Proxy</span><span class="sxs-lookup"><span data-stu-id="15ad5-919">Support for creating a Kafka cluster with Kafka Rest Proxy</span></span>
* <span data-ttu-id="15ad5-920">„azure-mgmt-hdinsight“ auf 1.3.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-920">Upgrade azure-mgmt-hdinsight to 1.3.0</span></span>

### <a name="misc"></a><span data-ttu-id="15ad5-921">Verschiedenes:</span><span class="sxs-lookup"><span data-stu-id="15ad5-921">Misc.</span></span>

* <span data-ttu-id="15ad5-922">Vorschaubefehl `az version show` hinzugefügt, um die Versionen der Azure CLI-Module und Erweiterungen standardmäßig im JSON-Format oder im mit „--output“ konfigurierten Format anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="15ad5-922">Add preview command `az version show` to show the versions of Azure CLI modules and extensions in JSON format by default or format configured by --output</span></span>

### <a name="event-hubs"></a><span data-ttu-id="15ad5-923">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="15ad5-923">Event Hubs</span></span>

* <span data-ttu-id="15ad5-924">[BREAKING CHANGE] Statusoption „ReceiveDisabled“ aus „az eventhubs eventhub update“ und „az eventhubs eventhub create“ entfernt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-924">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az eventhubs eventhub update' and 'az eventhubs eventhub create'.</span></span> <span data-ttu-id="15ad5-925">Diese Option ist für Event Hub-Entitäten nicht gültig.</span><span class="sxs-lookup"><span data-stu-id="15ad5-925">This option is not valid for Event Hub entities.</span></span>

### <a name="service-bus"></a><span data-ttu-id="15ad5-926">Service Bus</span><span class="sxs-lookup"><span data-stu-id="15ad5-926">Service Bus</span></span>

* <span data-ttu-id="15ad5-927">[BREAKING CHANGE] Statusoption „ReceiveDisabled“ aus Befehlen „az servicebus topic create“, „az servicebus topic update“, „az servicebus queue create“ und „az servicebus queue update“ entfernt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-927">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az servicebus topic create', 'az servicebus topic update', 'az servicebus queue create', and 'az servicebus queue update'.</span></span> <span data-ttu-id="15ad5-928">Diese Option ist für Service Bus-Themen und -Warteschlangen nicht gültig.</span><span class="sxs-lookup"><span data-stu-id="15ad5-928">This option is not valid for Service Bus topics and queues.</span></span>

### <a name="rbac"></a><span data-ttu-id="15ad5-929">RBAC</span><span class="sxs-lookup"><span data-stu-id="15ad5-929">RBAC</span></span>

* <span data-ttu-id="15ad5-930">Behebung Nr. 11712: `az ad app/sp show` gibt nicht den Exitcode 3 zurück, wenn die Anwendung oder der Dienstprinzipal nicht vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="15ad5-930">Fix #11712: `az ad app/sp show` does not return exit code 3 when the application or service principal does not exist</span></span>

### <a name="storage"></a><span data-ttu-id="15ad5-931">Storage</span><span class="sxs-lookup"><span data-stu-id="15ad5-931">Storage</span></span>

* <span data-ttu-id="15ad5-932">`az storage account create`: Vorschaukennzeichnung für Parameter „--enable-hierarchical-namespace“ entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-932">`az storage account create`: Remove preview flag for --enable-hierarchical-namespace parameter</span></span>
* <span data-ttu-id="15ad5-933">azure-mgmt-storage-Version auf 7.0.0 aktualisiert, um API-Version 2019-06-01 zu verwenden</span><span class="sxs-lookup"><span data-stu-id="15ad5-933">Update azure-mgmt-storage version to 7.0.0 to use api version 2019-06-01</span></span>
* <span data-ttu-id="15ad5-934">Neue Parameter `--enable-delete-retention` und `--delete-retention-days` hinzugefügt, um die Verwaltung der Aufbewahrungsrichtlinie für Löschen für „blob-service-properties“ von Speicherkonten zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="15ad5-934">Add new parameters `--enable-delete-retention` and `--delete-retention-days` to support managing delete retention policy for storage account blob-service-properties.</span></span>

## <a name="december-17-2019"></a><span data-ttu-id="15ad5-935">17. Dezember 2019</span><span class="sxs-lookup"><span data-stu-id="15ad5-935">December 17, 2019</span></span>

<span data-ttu-id="15ad5-936">2.0.78</span><span class="sxs-lookup"><span data-stu-id="15ad5-936">2.0.78</span></span>

### <a name="acr"></a><span data-ttu-id="15ad5-937">ACR</span><span class="sxs-lookup"><span data-stu-id="15ad5-937">ACR</span></span>

* <span data-ttu-id="15ad5-938">Unterstützung für lokalen Kontext in „acr task run“</span><span class="sxs-lookup"><span data-stu-id="15ad5-938">Added support Local context in acr task run</span></span>

### <a name="acs"></a><span data-ttu-id="15ad5-939">ACS</span><span class="sxs-lookup"><span data-stu-id="15ad5-939">ACS</span></span>

* <span data-ttu-id="15ad5-940">[BREAKING CHANGE] az openshift create: `--workspace-resource-id` in `--workspace-id` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-940">[BREAKING CHANGE]az openshift create: rename `--workspace-resource-id` to `--workspace-id`.</span></span>

### <a name="ams"></a><span data-ttu-id="15ad5-941">AMS</span><span class="sxs-lookup"><span data-stu-id="15ad5-941">AMS</span></span>

* <span data-ttu-id="15ad5-942">Befehle zum Anzeigen aktualisiert, sodass 3 zurückgegeben wird, wenn die Ressource nicht gefunden wurde</span><span class="sxs-lookup"><span data-stu-id="15ad5-942">Updated show commands to return 3 when resource not found</span></span>

### <a name="appconfig"></a><span data-ttu-id="15ad5-943">AppConfig</span><span class="sxs-lookup"><span data-stu-id="15ad5-943">AppConfig</span></span>

* <span data-ttu-id="15ad5-944">Fehler beim Anhängen der API-Version an die Anforderungs-URL korrigiert.</span><span class="sxs-lookup"><span data-stu-id="15ad5-944">Fixed bug when appending api-version to request url.</span></span> <span data-ttu-id="15ad5-945">Die vorhandene Lösung funktioniert nicht mit Paginierung.</span><span class="sxs-lookup"><span data-stu-id="15ad5-945">The existing solution doesn't work with pagination.</span></span>
* <span data-ttu-id="15ad5-946">Unterstützung für die Anzeige von weiteren Sprachen neben Englisch hinzugefügt, da der Back-End-Dienst Unicode für die Globalisierung unterstützt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-946">Added support for showing languages besides English as our backend service support unicode for globalization.</span></span>

### <a name="appservice"></a><span data-ttu-id="15ad5-947">AppService</span><span class="sxs-lookup"><span data-stu-id="15ad5-947">AppService</span></span>

* <span data-ttu-id="15ad5-948">Problem Nr. 11217 behoben: Web-App: „az webapp config ssl upload“ muss Slot-Parameter unterstützen.</span><span class="sxs-lookup"><span data-stu-id="15ad5-948">Fixed issue #11217: webapp: az webapp config ssl upload should support slot parameter</span></span>
* <span data-ttu-id="15ad5-949">Problem Nr. 10965 behoben: Error: Der Name darf nicht leer sein.</span><span class="sxs-lookup"><span data-stu-id="15ad5-949">Fixed issue #10965: Error: Name cannot be empty.</span></span> <span data-ttu-id="15ad5-950">Entfernen anhand von „ip_address“ und „subnet“ zulassen</span><span class="sxs-lookup"><span data-stu-id="15ad5-950">Allow remove by ip_address and subnet</span></span>
* <span data-ttu-id="15ad5-951">Unterstützung des Imports von Zertifikaten aus Key Vault hinzugefügt `az webapp config ssl import`</span><span class="sxs-lookup"><span data-stu-id="15ad5-951">Added support for importing certificates from Key Vault `az webapp config ssl import`</span></span>

### <a name="arm"></a><span data-ttu-id="15ad5-952">ARM</span><span class="sxs-lookup"><span data-stu-id="15ad5-952">ARM</span></span>

* <span data-ttu-id="15ad5-953">Paket „azure-mgmt-resource“ auf die Verwendung von 6.0.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-953">Updated azure-mgmt-resource package to use 6.0.0</span></span>
* <span data-ttu-id="15ad5-954">Mandantenübergreifende Unterstützung für Befehl `az group deployment create` durch Hinzufügen des neuen Parameters `--aux-subs`</span><span class="sxs-lookup"><span data-stu-id="15ad5-954">Cross Tenant Support for `az group deployment create` command by adding new parameter `--aux-subs`</span></span>
* <span data-ttu-id="15ad5-955">Neuer Parameter `--metadata` hinzugefügt, um das Hinzufügen von Metadateninformationen für Richtliniensatzdefinitionen zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="15ad5-955">Added new parameter `--metadata` to support adding metadata information for policy set definitions.</span></span>

### <a name="backup"></a><span data-ttu-id="15ad5-956">Backup</span><span class="sxs-lookup"><span data-stu-id="15ad5-956">Backup</span></span>

* <span data-ttu-id="15ad5-957">Unterstützung der Sicherung für SQL- und SAP Hana-Workloads hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-957">Added Backup support for SQL and SAP Hana workload.</span></span>

### <a name="botservice"></a><span data-ttu-id="15ad5-958">BotService</span><span class="sxs-lookup"><span data-stu-id="15ad5-958">BotService</span></span>

* <span data-ttu-id="15ad5-959">[Breaking Change] Flag „--version“ aus Vorschaubefehl „az bot create“ entfernt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-959">[Breaking change] Remove '--version' flag from preview command 'az bot create'.</span></span> <span data-ttu-id="15ad5-960">Nur v4-SDK-Bots werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-960">Only v4 SDK bots are supported.</span></span>
* <span data-ttu-id="15ad5-961">Überprüfung der Namensverfügbarkeit für „az bot create“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-961">Added name availability check for 'az bot create'.</span></span>
* <span data-ttu-id="15ad5-962">Unterstützung für das Aktualisieren der Symbol-URL für einen Bot über „az bot update“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-962">Added support for updating the icon URL for a bot via 'az bot update'.</span></span>
* <span data-ttu-id="15ad5-963">Unterstützung für das Aktualisieren eines Direct Line-Kanals über „az bot directline update“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-963">Added support for updating a Direct Line channel via 'az bot directline update'.</span></span>
* <span data-ttu-id="15ad5-964">Unterstützung für Flag „--enable-enhanced-auth“ zu „az bot directline create“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-964">Added '--enable-enhanced-auth' flag support to 'az bot directline create'.</span></span>
* <span data-ttu-id="15ad5-965">Die folgenden Befehlsgruppen sind allgemein verfügbar und befinden sich nicht in der Vorschau: „az bot authsetting“.</span><span class="sxs-lookup"><span data-stu-id="15ad5-965">The following command groups are GA and not in preview: 'az bot authsetting'.</span></span>
* <span data-ttu-id="15ad5-966">Die folgenden Befehle in „az bot“ sind allgemein verfügbar und befinden sich nicht in der Vorschau: „create“, „prepare-deploy“, „show“, „delete“, „update“.</span><span class="sxs-lookup"><span data-stu-id="15ad5-966">The following commands in 'az bot' are GA and not in preview: 'create', 'prepare-deploy', 'show', 'delete', 'update'.</span></span>
* <span data-ttu-id="15ad5-967">„az bot prepare-deploy“ korrigiert, indem der Wert voon „--proj-file-path“ in Kleinschreibung geändert wurde (z. B. „Test.csproj“ in „test.csproj“).</span><span class="sxs-lookup"><span data-stu-id="15ad5-967">Fixed 'az bot prepare-deploy' changing '--proj-file-path' value to lower case (e.g. "Test.csproj" to "test.csproj").</span></span>

### <a name="compute"></a><span data-ttu-id="15ad5-968">Compute</span><span class="sxs-lookup"><span data-stu-id="15ad5-968">Compute</span></span>

* <span data-ttu-id="15ad5-969">vmss create/update: „--scale-in-policy“ hinzugefügt, womit entschieden wird, welche virtuellen Computer beim horizontalen Herunterskalieren einer VM-Skalierungsgruppe zum Entfernen ausgewählt werden.</span><span class="sxs-lookup"><span data-stu-id="15ad5-969">vmss create/update: Added --scale-in-policy, which decides which virtual machines are chosen for removal when a VMSS is scaled-in.</span></span>
* <span data-ttu-id="15ad5-970">vm/vmss update: „--priority“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-970">vm/vmss update: Added --priority.</span></span>
* <span data-ttu-id="15ad5-971">vm/vmss update: „--max-price“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-971">vm/vmss update: Added --max-price.</span></span>
* <span data-ttu-id="15ad5-972">Befehlsgruppe „disk-encryption-set“ hinzugefügt (create, show, update, delete, list).</span><span class="sxs-lookup"><span data-stu-id="15ad5-972">Added disk-encryption-set command group (create, show, update, delete, list).</span></span>
* <span data-ttu-id="15ad5-973">disk create: „--encryption-type“ und „--disk-encryption-set“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-973">disk create: Added --encryption-type and --disk-encryption-set.</span></span>
* <span data-ttu-id="15ad5-974">vm/vmss create: „--os-disk-encryption-set“ und „--data-disk-encryption-sets“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-974">vm/vmss create: Added --os-disk-encryption-set and --data-disk-encryption-sets.</span></span>

### <a name="core"></a><span data-ttu-id="15ad5-975">Core</span><span class="sxs-lookup"><span data-stu-id="15ad5-975">Core</span></span>

* <span data-ttu-id="15ad5-976">Unterstützung für Python 3.4 entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-976">Removed support for Python 3.4</span></span>
* <span data-ttu-id="15ad5-977">Plug-In für HaTS-Umfrage in mehreren Befehlen</span><span class="sxs-lookup"><span data-stu-id="15ad5-977">Plug in HaTS survey in multiple commands</span></span>

### <a name="dls"></a><span data-ttu-id="15ad5-978">DLS</span><span class="sxs-lookup"><span data-stu-id="15ad5-978">DLS</span></span>

* <span data-ttu-id="15ad5-979">ADLS-SDK-Version aktualisiert (0.0.48).</span><span class="sxs-lookup"><span data-stu-id="15ad5-979">Updated ADLS sdk version (0.0.48).</span></span>

### <a name="install"></a><span data-ttu-id="15ad5-980">Installieren</span><span class="sxs-lookup"><span data-stu-id="15ad5-980">Install</span></span>

* <span data-ttu-id="15ad5-981">Installationsskript unterstützt Python 3.8</span><span class="sxs-lookup"><span data-stu-id="15ad5-981">Install script support python 3.8</span></span>

### <a name="iot"></a><span data-ttu-id="15ad5-982">IoT</span><span class="sxs-lookup"><span data-stu-id="15ad5-982">IOT</span></span>

* <span data-ttu-id="15ad5-983">[BREAKING CHANGE] Parameter „--failover-region“ aus „manual-failover“ entfernt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-983">[BREAKING CHANGE] Removed --failover-region parameter from manual-failover.</span></span> <span data-ttu-id="15ad5-984">Das Failover erfolgt jetzt in eine zugewiesene, geografisch gekoppelte sekundäre Region.</span><span class="sxs-lookup"><span data-stu-id="15ad5-984">Now it will failover to assigned geo-paired secondary region.</span></span>

### <a name="key-vault"></a><span data-ttu-id="15ad5-985">Key Vault</span><span class="sxs-lookup"><span data-stu-id="15ad5-985">Key Vault</span></span>

* <span data-ttu-id="15ad5-986">Nr. 8095 behoben: `az keyvault storage remove`: Hilfemeldung verbessert</span><span class="sxs-lookup"><span data-stu-id="15ad5-986">Fixed #8095: `az keyvault storage remove`: improve the help message</span></span>
* <span data-ttu-id="15ad5-987">Nr. 8921 behoben: `az keyvault key/secret/certificate list/list-deleted/list-versions`: Validierungsfehler in Parameter `--maxresults` behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-987">Fixed #8921: `az keyvault key/secret/certificate list/list-deleted/list-versions`: fix the validation bug on parameter `--maxresults`</span></span>
* <span data-ttu-id="15ad5-988">Nr. 10512 behoben: `az keyvault set-policy`: Fehlermeldung verbessert, wenn weder `--object-id`, `--spn` noch `--upn` angegeben ist</span><span class="sxs-lookup"><span data-stu-id="15ad5-988">Fixed #10512: `az keyvault set-policy`: improve the error message when none of `--object-id`, `--spn` or `--upn` is specified</span></span>
* <span data-ttu-id="15ad5-989">Nr. 10846 behoben: `az keyvault secret show-deleted`: Wenn `--id` angegeben ist, ist `--name/-n` nicht erforderlich.</span><span class="sxs-lookup"><span data-stu-id="15ad5-989">Fixed #10846: `az keyvault secret show-deleted`: when `--id` is specified, `--name/-n` is not required</span></span>
* <span data-ttu-id="15ad5-990">Nr. 11084 behoben: `az keyvault secret download`: Hilfemeldung von Parameter `--encoding` verbessert</span><span class="sxs-lookup"><span data-stu-id="15ad5-990">Fixed #11084: `az keyvault secret download`: improve the help message of parameter `--encoding`</span></span>

### <a name="network"></a><span data-ttu-id="15ad5-991">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="15ad5-991">Network</span></span>

* <span data-ttu-id="15ad5-992">az network application-gateway probe: Unterstützung für Option „--port“ hinzugefügt, um einen Port zum Prüfen von Back-End-Servern beim Erstellen und Aktualisieren anzugeben</span><span class="sxs-lookup"><span data-stu-id="15ad5-992">az network application-gateway probe: Added support --port option to specify a port for probing backend servers when create and update</span></span>
* <span data-ttu-id="15ad5-993">az network application-gateway url-path-map create/update: Fehlerbehebung für `--waf-policy`</span><span class="sxs-lookup"><span data-stu-id="15ad5-993">az network application-gateway url-path-map create/update: bug fix for `--waf-policy`</span></span>
* <span data-ttu-id="15ad5-994">az network application-gateway: Unterstützung für `--rewrite-rule-set` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-994">az network application-gateway: Added support `--rewrite-rule-set`</span></span>
* <span data-ttu-id="15ad5-995">az network list-service-aliases: Unterstützung für Listendienstaliase hinzugefügt, die für Dienstendpunktrichtlinien verwendet werden können</span><span class="sxs-lookup"><span data-stu-id="15ad5-995">az network list-service-aliases: Added support list service aliases which can be used for Service Endpoint Policies</span></span>
* <span data-ttu-id="15ad5-996">az network dns zone import: Unterstützung für „.@“ in Datensatzname hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-996">az network dns zone import: Added support .@ in record name</span></span>

### <a name="packaging"></a><span data-ttu-id="15ad5-997">Verpackung</span><span class="sxs-lookup"><span data-stu-id="15ad5-997">Packaging</span></span>

* <span data-ttu-id="15ad5-998">Back-Edge-Builds für PIP-Installation hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-998">Added back edge builds for pip install</span></span>
* <span data-ttu-id="15ad5-999">Ubuntu-Eoan-Paket hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-999">Added Ubuntu eoan package</span></span>

### <a name="policy"></a><span data-ttu-id="15ad5-1000">Richtlinie</span><span class="sxs-lookup"><span data-stu-id="15ad5-1000">Policy</span></span>

* <span data-ttu-id="15ad5-1001">Unterstützung für Version 2019-09-01 der Richtlinien-API hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1001">Added support for Policy API version 2019-09-01.</span></span>
* <span data-ttu-id="15ad5-1002">az policy set-definition: Unterstützung der Gruppierung innerhalb von Richtliniensatzdefinitionen mit `--definition-groups`-Parameter hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1002">az policy set-definition: Added support grouping within policy set definitions with `--definition-groups` parameter</span></span>

### <a name="redis"></a><span data-ttu-id="15ad5-1003">Redis</span><span class="sxs-lookup"><span data-stu-id="15ad5-1003">Redis</span></span>

* <span data-ttu-id="15ad5-1004">Vorschauparameter `--replicas-per-master` zu Befehl `az redis create`hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1004">Added preview param `--replicas-per-master` to `az redis create` command</span></span>
* <span data-ttu-id="15ad5-1005">„azure-mgmt-redis“ von 6.0.0 auf 7.0.0rc1 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-1005">Updated azure-mgmt-redis from 6.0.0 to 7.0.0rc1</span></span>

### <a name="servicefabric"></a><span data-ttu-id="15ad5-1006">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="15ad5-1006">ServiceFabric</span></span>

* <span data-ttu-id="15ad5-1007">Hinzufügen von Logik in Knotentyp korrigiert, einschließlich Nr. 10963: Beim Hinzufügen eines neuen Knotentyps mit Dauerhaftigkeitsstufe „Gold“ wird immer ein CLI-Fehler ausgegeben.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1007">Fixed in node-type add logic including #10963: Adding new node type with durability level Gold will always throw CLI error</span></span>
* <span data-ttu-id="15ad5-1008">ServiceFabricNodeVmExt-Version in Erstellungsvorlage auf 1.1 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-1008">Updated ServiceFabricNodeVmExt version to 1.1 in creation template</span></span>

### <a name="sql"></a><span data-ttu-id="15ad5-1009">SQL</span><span class="sxs-lookup"><span data-stu-id="15ad5-1009">SQL</span></span>

* <span data-ttu-id="15ad5-1010">Parameter „--read-scale“ und „--read-replicas“ zu Befehlen „sql db create“ und „sql db update“ hinzugefügt, um Leseskalierungsverwaltung zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1010">Added "--read-scale" and "--read-replicas" parameters to sql db create and update commands, to support read scale management.</span></span>

### <a name="storage"></a><span data-ttu-id="15ad5-1011">Storage</span><span class="sxs-lookup"><span data-stu-id="15ad5-1011">Storage</span></span>

* <span data-ttu-id="15ad5-1012">Allgemein verfügbares Release – Eigenschaft „Large File Shares“ für Befehle „storage account create“ und „storage account update“</span><span class="sxs-lookup"><span data-stu-id="15ad5-1012">GA Release Large File Shares property for storage account create and update command</span></span>
* <span data-ttu-id="15ad5-1013">Allgemein verfügbares Release – Unterstützung von SAS-Token für die Benutzerdelegierung</span><span class="sxs-lookup"><span data-stu-id="15ad5-1013">GA Release User Delegation SAS token Support</span></span>
* <span data-ttu-id="15ad5-1014">Neue Befehle `az storage account blob-service-properties show` und `az storage account blob-service-properties update --enable-change-feed` hinzugefügt, um Blob-Diensteigenschaften für das Speicherkonto zu verwalten.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1014">Added new commands `az storage account blob-service-properties show` and `az storage account blob-service-properties update --enable-change-feed` to manage blob service properties for storage account.</span></span>
* <span data-ttu-id="15ad5-1015">[BEVORSTEHENDER BREAKING CHANGE] `az storage copy`: Das Zeichen `*` wird nicht mehr als Platzhalter in der URL, es werden jedoch die neuen Parameter „--include-pattern“ und „--exclude-pattern“ mit Unterstützung des Platzhalters `*` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1015">[COMING BREAKING CHANGE] `az storage copy`: `*` character is no longer supported as a wildcard in URL, but new parameters --include-pattern and --exclude-pattern will be added with `*` wildcard support.</span></span>
* <span data-ttu-id="15ad5-1016">Problem Nr. 11043 behoben: Unterstützung für das Entfernen des gesamten Containers/der gesamten Freigabe in `az storage remove` Befehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1016">Fixed issue #11043: Added support to remove whole container/share in `az storage remove` command</span></span>

## <a name="november-26-2019"></a><span data-ttu-id="15ad5-1017">26. November 2019</span><span class="sxs-lookup"><span data-stu-id="15ad5-1017">November 26, 2019</span></span>

<span data-ttu-id="15ad5-1018">Version 2.0.77</span><span class="sxs-lookup"><span data-stu-id="15ad5-1018">Version 2.0.77</span></span>

### <a name="acr"></a><span data-ttu-id="15ad5-1019">ACR</span><span class="sxs-lookup"><span data-stu-id="15ad5-1019">ACR</span></span>

* <span data-ttu-id="15ad5-1020">Parameter `--branch` in „acr task create/update“ als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-1020">Deprecated parameter `--branch` from acr task create/update</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="15ad5-1021">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="15ad5-1021">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="15ad5-1022">`--workspace-resource-id`-Flag hinzugefügt, um die Erstellung eines Azure Red Hat OpenShift-Clusters mit Überwachung zuzulassen</span><span class="sxs-lookup"><span data-stu-id="15ad5-1022">Added `--workspace-resource-id` flag to allow creation of Azure Red Hat Openshift cluster with monitoring</span></span>
* <span data-ttu-id="15ad5-1023">`monitor_profile`-Flag hinzugefügt, um einen Azure Red Hat OpenShift-Clusters mit Überwachung zu erstellen</span><span class="sxs-lookup"><span data-stu-id="15ad5-1023">Added `monitor_profile` to create Azure Red Hat OpenShift cluster with monitoring</span></span>

### <a name="aks"></a><span data-ttu-id="15ad5-1024">AKS</span><span class="sxs-lookup"><span data-stu-id="15ad5-1024">AKS</span></span>

* <span data-ttu-id="15ad5-1025">Unterstützung des Rotationsvorgangs für Clusterzertifikate mithilfe von für Cluster Zertifikat Rotation mit „az aks rotate-certs“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1025">Added support cluster certificate rotation operation using "az aks rotate-certs".</span></span>

### <a name="appconfig"></a><span data-ttu-id="15ad5-1026">AppConfig</span><span class="sxs-lookup"><span data-stu-id="15ad5-1026">AppConfig</span></span>

* <span data-ttu-id="15ad5-1027">Unterstützung für die Verwendung von „:“ für `as az appconfig kv import`-Trennzeichen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1027">Added support for using ":" for `as az appconfig kv import` separator</span></span>
* <span data-ttu-id="15ad5-1028">Problem beim Auflisten von Schlüsselwerten mit mehreren Bezeichnungen, einschließlich NULL-Bezeichnung, behoben.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1028">Fixed issue for listing key values with multiple labels including null label.</span></span> 
* <span data-ttu-id="15ad5-1029">Verwaltungsebenen-SDK, „azure-mgmt-appconfiguration“, auf Version 0.3.0 aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1029">Updated management plane sdk, azure-mgmt-appconfiguration, to version 0.3.0.</span></span> 

### <a name="appservice"></a><span data-ttu-id="15ad5-1030">AppService</span><span class="sxs-lookup"><span data-stu-id="15ad5-1030">AppService</span></span>

* <span data-ttu-id="15ad5-1031">Problem Nr. 11100 behoben AttributeError für „az webapp up“ beim Erstellen eines Dienstplans</span><span class="sxs-lookup"><span data-stu-id="15ad5-1031">Fixed issue #11100: AttributeError for az webapp up when create service plan</span></span>
* <span data-ttu-id="15ad5-1032">az webapp up: Erzwingen der Erstellung oder Bereitstellung auf einer Website für unterstützte Sprachen, es werden keine Standardeinstellungen verwendet.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1032">az webapp up: Forcing the creation or deployment to a site for supported languages, no defaults used.</span></span>
* <span data-ttu-id="15ad5-1033">Unterstützung für App Service-Umgebung hinzugefügt: az appservice ase show | list | list-addresses | list-plans | create | update | delete</span><span class="sxs-lookup"><span data-stu-id="15ad5-1033">Added support for App Service Environment: az appservice ase show | list | list-addresses | list-plans | create | update | delete</span></span>

### <a name="backup"></a><span data-ttu-id="15ad5-1034">Backup</span><span class="sxs-lookup"><span data-stu-id="15ad5-1034">Backup</span></span>

* <span data-ttu-id="15ad5-1035">Problem in Az-Sicherungsrichtlinie „list-associated-items“ behoben.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1035">Fixed issue in az backup policy list-associated-items.</span></span> <span data-ttu-id="15ad5-1036">Optionaler Parameter „BackupManagementType“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1036">Added optional BackupManagementType parameter.</span></span>

### <a name="compute"></a><span data-ttu-id="15ad5-1037">Compute</span><span class="sxs-lookup"><span data-stu-id="15ad5-1037">Compute</span></span>

* <span data-ttu-id="15ad5-1038">API-Version von Compute, Datenträger, Momentaufnahmen auf 2019-07-01 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-1038">Upgraded API version of compute, disks, snapshots to 2019-07-01</span></span>
* <span data-ttu-id="15ad5-1039">vmss create: Verbesserung für – Orchestrierungsmodus</span><span class="sxs-lookup"><span data-stu-id="15ad5-1039">vmss create: Improvement for --orchestration-mode</span></span>
* <span data-ttu-id="15ad5-1040">sig image-definition create: „--os-state“ hinzugefügt, um die Angabe zu ermöglichen, ob die unter diesem Image erstellten virtuellen Computer „generalisiert“ oder „spezialisiert“ sind</span><span class="sxs-lookup"><span data-stu-id="15ad5-1040">sig image-definition create: Added --os-state to allow specifying whether the virtual machines created under this image are 'Generalized' or 'Specialized'</span></span>
* <span data-ttu-id="15ad5-1041">sig image-definition create: „--hyper-v-generation“ hinzugefügt, um die Angabe der Hypervisorgeneration zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="15ad5-1041">sig image-definition create: Added --hyper-v-generation to allow specifying the hypervisor generation</span></span>
* <span data-ttu-id="15ad5-1042">sig image-version create: Unterstützung für „--os-snapshot“ und „--data-snapshots“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1042">sig image-version create: Added support --os-snapshot and --data-snapshots</span></span>
* <span data-ttu-id="15ad5-1043">image create: „--data-disk-caching“ hinzugefügt, um die Angabe der Zwischenspeicherungseinstellung von Datenträger zu ermöflichen</span><span class="sxs-lookup"><span data-stu-id="15ad5-1043">image create: Added --data-disk-caching to allow specifying caching setting of data disks</span></span>
* <span data-ttu-id="15ad5-1044">Upgrade des Python-Compute-SDK auf 10.0.0</span><span class="sxs-lookup"><span data-stu-id="15ad5-1044">Upgraded Python Compute SDK to 10.0.0</span></span>
* <span data-ttu-id="15ad5-1045">vm/vmss create: „Spot“ zu Aufzählungseigenschaft „Priority“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1045">vm/vmss create: Added 'Spot' to 'Priority' enum property</span></span>
* <span data-ttu-id="15ad5-1046">[Breaking Change] Parameter „--max-billing“ für sowohl VM als auch VMSS in „--max-price“ umbenannt, um die Konsistenz mit Swagger- und PowerShell-Cmdlets sicherzustellen</span><span class="sxs-lookup"><span data-stu-id="15ad5-1046">[Breaking change] Renamed '--max-billing' parameter to '--max-price', for both VM and VMSS, to be consistent with Swagger and Powershell cmdlets</span></span>
* <span data-ttu-id="15ad5-1047">vm monitor log show: Unterstützung für das Abfragen von Protokollen über verknüpften Protokollanalyse-Arbeitsbereich hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1047">vm monitor log show: Added support for querying log over linked log analytics workspace.</span></span>

### <a name="iot"></a><span data-ttu-id="15ad5-1048">IoT</span><span class="sxs-lookup"><span data-stu-id="15ad5-1048">IOT</span></span>

* <span data-ttu-id="15ad5-1049">Behebung Nr. 2531: Argumente für Benutzerfreundlichkeit für Hub-Update hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1049">Fix #2531: Added convenience arguments for hub update.</span></span>
* <span data-ttu-id="15ad5-1050">Behebung Nr. 8323: Fehlende Parameter zum Erstellen eines benutzerdefinierten Speicherendpunkts hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1050">Fix #8323: Added missing parameters to create storage custom endpoint.</span></span>
* <span data-ttu-id="15ad5-1051">Regressionsfehler behoben: Die Änderungen wurden rückgängig gemacht, sodass der standardmäßige Speicherendpunkt überschrieben wurde.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1051">Fix regression bug: Reverted the changes which overrides the default storage endpoint.</span></span>

### <a name="key-vault"></a><span data-ttu-id="15ad5-1052">Key Vault</span><span class="sxs-lookup"><span data-stu-id="15ad5-1052">Key Vault</span></span>

* <span data-ttu-id="15ad5-1053">Nr. 11121 behoben: Bei der Verwendung von `az keyvault certificate list` erfordert die Übergabe von `--include-pending` jetzt nicht mehr den Wert `true` oder `false`.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1053">Fixed #11121: When using `az keyvault certificate list`, passing `--include-pending` now doesn't require a value of `true` or `false`</span></span>

### <a name="netappfiles"></a><span data-ttu-id="15ad5-1054">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="15ad5-1054">NetAppFiles</span></span>

* <span data-ttu-id="15ad5-1055">Upgrade von „azure-mgmt-netapp“ auf Version 0.7.0, die einige zusätzliche Volumeeigenschaften enthält, die bevorstehenden Replikationsvorgängen zugeordnet sind</span><span class="sxs-lookup"><span data-stu-id="15ad5-1055">Upgraded azure-mgmt-netapp to 0.7.0 which includes some additional volume properties associated with upcoming replication operations</span></span>

### <a name="network"></a><span data-ttu-id="15ad5-1056">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="15ad5-1056">Network</span></span>

* <span data-ttu-id="15ad5-1057">application-gateway waf-config: veraltet</span><span class="sxs-lookup"><span data-stu-id="15ad5-1057">application-gateway waf-config: deprecated</span></span>
* <span data-ttu-id="15ad5-1058">application-gateway waf-policy: Untergruppe „managed-rules“ zur Verwaltung von verwalteten Regelsätzen und Ausschlussregeln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1058">application-gateway waf-policy: Added subgroup managed-rules to manage managed rule sets and exclusion rules</span></span>
* <span data-ttu-id="15ad5-1059">application-gateway waf-policy: Untergruppe „policy-setting“ zur Verwaltung der globalen Konfiguration von „waf-policy“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1059">application-gateway waf-policy: Added subgroup policy-setting to manage global configuration of a waf-policy</span></span>
* <span data-ttu-id="15ad5-1060">[BREAKING CHANGE] application-gateway waf-policy: Untergruppenregel in „custom-rule“ umbenannt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1060">[BREAKING CHANGE] application-gateway waf-policy: Renamed subgroup rule to custom-rule</span></span>
* <span data-ttu-id="15ad5-1061">application-gateway http-listener: „--firewall-policy“ beim Erstellen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1061">application-gateway http-listener: Added --firewall-policy when create</span></span>
* <span data-ttu-id="15ad5-1062">application-gateway url-path-map rule: „--firewall-policy“ beim Erstellen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1062">application-gateway url-path-map rule: Added --firewall-policy when create</span></span>

### <a name="packaging"></a><span data-ttu-id="15ad5-1063">Verpackung</span><span class="sxs-lookup"><span data-stu-id="15ad5-1063">Packaging</span></span>

* <span data-ttu-id="15ad5-1064">Az-Wrapper in Python neu geschrieben</span><span class="sxs-lookup"><span data-stu-id="15ad5-1064">Rewrote the az wrapper in Python</span></span>
* <span data-ttu-id="15ad5-1065">Unterstützung für Python 3.8 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1065">Added support for Python 3.8</span></span>
* <span data-ttu-id="15ad5-1066">Für RPM-Paket in Python 3 geändert</span><span class="sxs-lookup"><span data-stu-id="15ad5-1066">Changed to Python 3 for RPM package</span></span>

### <a name="profile"></a><span data-ttu-id="15ad5-1067">Profil</span><span class="sxs-lookup"><span data-stu-id="15ad5-1067">Profile</span></span>

* <span data-ttu-id="15ad5-1068">Fehler beim Ausführen von `az login -u {} -p {}` mit Microsoft-Konto entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1068">Polished error when running `az login -u {} -p {}` with Microsoft account</span></span>
* <span data-ttu-id="15ad5-1069">`SSLError` beim Ausführen von `az login` hinter einem Proxy mit einem selbstsignierten Stammzertifikat entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1069">Polished `SSLError` when running `az login` behind a proxy with self-signed root certificate</span></span>
* <span data-ttu-id="15ad5-1070">Nr. 10578 behoben: `az login` hängt, wenn mehrere Instanzen gleichzeitig unter Windows oder WSL gestartet werden.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1070">Fixed #10578: `az login` hangs when more than one instances are launched at the same time on Windows or WSL</span></span>
* <span data-ttu-id="15ad5-1071">Nr. 11059 behoben: `az login --allow-no-subscriptions` schlägt fehl, wenn Abonnements im Mandanten vorhanden sind.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1071">Fixed #11059: `az login --allow-no-subscriptions` fails if there are subscriptions in the tenant</span></span>
* <span data-ttu-id="15ad5-1072">Nr. 11238 behoben: Nach dem Umbenennen eines Abonnements führt die Anmeldung mit MSI dazu, dass das gleiche Abonnement zweimal angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1072">Fixed #11238: After renaming a subscription, logging in with MSI will result in the same subscription appearing twice</span></span>

### <a name="rbac"></a><span data-ttu-id="15ad5-1073">RBAC</span><span class="sxs-lookup"><span data-stu-id="15ad5-1073">RBAC</span></span>

* <span data-ttu-id="15ad5-1074">Nr. 10996 behoben: Fehler für `--force-change-password-next-login` in `az ad user update` entfernt, wenn `--password` nicht angegeben ist</span><span class="sxs-lookup"><span data-stu-id="15ad5-1074">Fixed #10996: Polish error for `--force-change-password-next-login` in `az ad user update` when `--password` is not specified</span></span>

### <a name="redis"></a><span data-ttu-id="15ad5-1075">Redis</span><span class="sxs-lookup"><span data-stu-id="15ad5-1075">Redis</span></span>

* <span data-ttu-id="15ad5-1076">Nr. 2902 behoben: Festlegen von Speicherkonfigurationen beim Aktualisieren des Basic-SKU-Cache vermeiden</span><span class="sxs-lookup"><span data-stu-id="15ad5-1076">Fixed #2902: Avoid setting memory configs while updating Basic SKU cache</span></span>

### <a name="reservations"></a><span data-ttu-id="15ad5-1077">Reservations</span><span class="sxs-lookup"><span data-stu-id="15ad5-1077">Reservations</span></span>

* <span data-ttu-id="15ad5-1078">SDK-Version auf 0.6.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-1078">Upgraded SDK Version to 0.6.0</span></span>
* <span data-ttu-id="15ad5-1079">Abrechnungsplandetails nach dem Aufrufen von „Get-Gatalogs“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1079">Added billingplan details info after calling Get-Gatalogs</span></span>
* <span data-ttu-id="15ad5-1080">Neuer Befehl `az reservations reservation-order calculate` zum Berechnen des Preises für eine Reservierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1080">Added new command `az reservations reservation-order calculate` to calculate the price for a reservation</span></span>
* <span data-ttu-id="15ad5-1081">Neuer Befehl `az reservations reservation-order purchase` zum Erwerb einer neuen Reservierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1081">Added new command `az reservations reservation-order purchase` to purchase a new reservation</span></span>

### <a name="rest"></a><span data-ttu-id="15ad5-1082">REST</span><span class="sxs-lookup"><span data-stu-id="15ad5-1082">Rest</span></span>
* <span data-ttu-id="15ad5-1083">`az rest` in allgemeine Verfügbarkeit geändert</span><span class="sxs-lookup"><span data-stu-id="15ad5-1083">Changed `az rest` to GA</span></span>

### <a name="sql"></a><span data-ttu-id="15ad5-1084">SQL</span><span class="sxs-lookup"><span data-stu-id="15ad5-1084">SQL</span></span>

* <span data-ttu-id="15ad5-1085">„azure-mgmt-sql“ auf Version 0.15.0 aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1085">Updated azure-mgmt-sql to version 0.15.0.</span></span>

### <a name="storage"></a><span data-ttu-id="15ad5-1086">Storage</span><span class="sxs-lookup"><span data-stu-id="15ad5-1086">Storage</span></span>

* <span data-ttu-id="15ad5-1087">storage account create: „--enable-hierarchical-namespace“ hinzugefügt, um Dateisystemsemantik in Blobdienst zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1087">storage account create: Added --enable-hierarchical-namespace to support filesystem semantics in blob service.</span></span>
* <span data-ttu-id="15ad5-1088">Ausnahme ohne Zusammenhang aus Fehlermeldung entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1088">Removed unrelated exception from error message</span></span>
* <span data-ttu-id="15ad5-1089">Probleme mit falscher Fehlermeldung „Sie verfügen nicht über die erforderlichen Berechtigungen zum Ausführen dieses Vorgangs“ behoben.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1089">Fixed issues with incorrect error message "You do not have the required permissions needed to perform this operation."</span></span> <span data-ttu-id="15ad5-1090">bei Blockierung durch Netzwerkregeln oder bei „AuthenticationFailed“.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1090">when blocked by network rules or AuthenticationFailed.</span></span>

## <a name="november-4-2019"></a><span data-ttu-id="15ad5-1091">4\. November 2019</span><span class="sxs-lookup"><span data-stu-id="15ad5-1091">November 4, 2019</span></span>

<span data-ttu-id="15ad5-1092">Version 2.0.76</span><span class="sxs-lookup"><span data-stu-id="15ad5-1092">Version 2.0.76</span></span>

### <a name="acr"></a><span data-ttu-id="15ad5-1093">ACR</span><span class="sxs-lookup"><span data-stu-id="15ad5-1093">ACR</span></span>

* <span data-ttu-id="15ad5-1094">Vorschauparameter `--pack-image-tag` wurde dem Befehl `az acr pack build` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1094">Added a preview parameter `--pack-image-tag` to command `az acr pack build`.</span></span>
* <span data-ttu-id="15ad5-1095">Unterstützung der Aktivierung der Überwachung beim Erstellen einer Registrierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1095">Added support for enabling auditing on creating a registry</span></span>
* <span data-ttu-id="15ad5-1096">Unterstützung von RBAC mit Repositoryumfang hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1096">Added support for Repository-scoped RBAC</span></span>

### <a name="aks"></a><span data-ttu-id="15ad5-1097">AKS</span><span class="sxs-lookup"><span data-stu-id="15ad5-1097">AKS</span></span>

* <span data-ttu-id="15ad5-1098">`--enable-cluster-autoscaler`, `--min-count` und `--max-count` wurden dem Befehl `az aks create` hinzugefügt, sodass die automatische Clusterskalierung für den Knotenpool aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1098">Added `--enable-cluster-autoscaler`, `--min-count` and `--max-count` to the `az aks create` command, which enables cluster autoscaler for the node pool.</span></span>
* <span data-ttu-id="15ad5-1099">Die obigen Flags sowie `--update-cluster-autoscaler` und `--disable-cluster-autoscaler` wurden dem Befehl `az aks update` hinzugefügt, sodass Updates der automatischen Clusterskalierung zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1099">Added the above flags as well as `--update-cluster-autoscaler` and `--disable-cluster-autoscaler` to the `az aks update` command, allowing updates to cluster autoscaler.</span></span>

### <a name="appconfig"></a><span data-ttu-id="15ad5-1100">AppConfig</span><span class="sxs-lookup"><span data-stu-id="15ad5-1100">AppConfig</span></span>

* <span data-ttu-id="15ad5-1101">Befehlsgruppe der AppConfig-Funktion zum Verwalten von in einer App Configuration-Instanz gespeicherten Featureflags wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1101">Added appconfig feature command group to manage feature flags stored in an App Configuration.</span></span>
* <span data-ttu-id="15ad5-1102">Geringfügiger Programmfehler für Befehl „appconfig kv export to file“ wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1102">Fixed minor bug for appconfig kv export to file command.</span></span> <span data-ttu-id="15ad5-1103">Das Lesen der Zieldateiinhalte wird während des Exports angehalten.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1103">Stop reading dest file contents during export.</span></span>

### <a name="appservice"></a><span data-ttu-id="15ad5-1104">AppService</span><span class="sxs-lookup"><span data-stu-id="15ad5-1104">AppService</span></span>

* <span data-ttu-id="15ad5-1105">`az appservice plan create`: Unterstützung für das Festlegen von „persitescalung“ beim Erstellen eines App-Serviceplans wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1105">`az appservice plan create`: Added support to set 'persitescaling' on appservice plan create.</span></span>
* <span data-ttu-id="15ad5-1106">Ein Problem wurde behoben, aufgrund dessen der Vorgang „webapp config ssl bind“ vorhandene Tags aus der Ressource entfernt hat.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1106">Fixed an issue where webapp config ssl bind operation was removing existing tags from the resource</span></span>
* <span data-ttu-id="15ad5-1107">Flag `--build-remote` wurde für `az functionapp deployment source config-zip` hinzugefügt, um die Remotebuildaktion während der Funktions-App-Bereitstellung zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1107">Added `--build-remote` flag for `az functionapp deployment source config-zip` to support remote build action during function app deployment.</span></span>
* <span data-ttu-id="15ad5-1108">Die Standardknotenversion in Funktions-Apps wurde für Windows in ~ 10 geändert.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1108">Changed default node version on function apps to ~10 for Windows</span></span>
* <span data-ttu-id="15ad5-1109">`--runtime-version`-Eigenschaft zu `az functionapp create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1109">Added `--runtime-version` property to `az functionapp create`</span></span>

### <a name="arm"></a><span data-ttu-id="15ad5-1110">ARM</span><span class="sxs-lookup"><span data-stu-id="15ad5-1110">ARM</span></span>

* <span data-ttu-id="15ad5-1111">`az deployment/group deployment validate`: Parameter `--handle-extended-json-format` wurde hinzugefügt, um bei der Bereitstellung mehrere Zeilen und Kommentare in der JSON-Vorlage zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1111">`az deployment/group deployment validate`: Added `--handle-extended-json-format` parameter to support multiline and comments in json template when deployment.</span></span>
* <span data-ttu-id="15ad5-1112">„azure-mgmt-resource“ auf „2019-07-01“ festgelegt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1112">Bumped azure-mgmt-resource to 2019-07-01</span></span>

### <a name="backup"></a><span data-ttu-id="15ad5-1113">Backup</span><span class="sxs-lookup"><span data-stu-id="15ad5-1113">Backup</span></span>

* <span data-ttu-id="15ad5-1114">Unterstützung für AzureFiles-Sicherung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1114">Added AzureFiles backup support</span></span>

### <a name="compute"></a><span data-ttu-id="15ad5-1115">Compute</span><span class="sxs-lookup"><span data-stu-id="15ad5-1115">Compute</span></span>

* <span data-ttu-id="15ad5-1116">`az vm create`: Beim gleichzeitigen Festlegen von beschleunigtem Netzwerkbetrieb und einer vorhandenen NIC wurde eine Warnung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1116">`az vm create`: Added warning when specifying accelerated networking and an existing NIC together.</span></span>
* <span data-ttu-id="15ad5-1117">`az vm create`: `--vmss` hinzugefügt, um eine vorhandene VM-Skalierungsgruppe anzugeben, welcher der virtuelle Computer zugewiesen werden soll.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1117">`az vm create`: Added `--vmss` to specify an existing virtual machine scale set that the virtual machine should be assigned to.</span></span>
* <span data-ttu-id="15ad5-1118">`az vm/vmss create`: Eine lokale Kopie der Imagealiasdatei wurde hinzugefügt, sodass in einer eingeschränkten Netzwerkumgebung darauf zugegriffen werden kann.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1118">`az vm/vmss create`: Added a local copy of image alias file so that it can be accessed in a restricted network environment.</span></span>
* <span data-ttu-id="15ad5-1119">`az vmss create`: `--orchestration-mode` hinzugefügt, um anzugeben, wie virtuelle Computer von der Skalierungsgruppe verwaltet werden.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1119">`az vmss create`: Added `--orchestration-mode` to specify how virtual machines are managed by the scale set.</span></span>
* <span data-ttu-id="15ad5-1120">`az vm/vmss update`: `--ultra-ssd-enabled` hinzugefügt, um das Aktualisieren der SSD-Einstellung zuzulassen.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1120">`az vm/vmss update`: Added `--ultra-ssd-enabled` to allow updating ultra SSD setting.</span></span>
* <span data-ttu-id="15ad5-1121">[BREAKING CHANGE] `az vm extension set`: Ein Fehler wurde behoben, aufgrund dessen Benutzer mit `--ids` keine Erweiterung auf einem virtuellen Computer festlegen konnten.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1121">[BREAKING CHANGE] `az vm extension set`: Fixed bug where users could not set an extension on a VM with `--ids`.</span></span>
* <span data-ttu-id="15ad5-1122">Neue Befehle wurden zu `az vm image terms accept/cancel/show` hinzugefügt , um Azure Marketplace-Imagebedingungen zu verwalten.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1122">Added new commands `az vm image terms accept/cancel/show` to manage Azure Marketplace image terms.</span></span>
* <span data-ttu-id="15ad5-1123">VMAccessForLinux auf Version 1.5 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-1123">Updated VMAccessForLinux to version 1.5</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="15ad5-1124">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="15ad5-1124">CosmosDB</span></span>

* <span data-ttu-id="15ad5-1125">[BREAKING CHANGE] `az sql container create`: `--partition-key-path` in erforderlichen Parameter geändert</span><span class="sxs-lookup"><span data-stu-id="15ad5-1125">[BREAKING CHANGE] `az sql container create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="15ad5-1126">[BREAKING CHANGE] `az gremlin graph create`: `--partition-key-path` in erforderlichen Parameter geändert</span><span class="sxs-lookup"><span data-stu-id="15ad5-1126">[BREAKING CHANGE] `az gremlin graph create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="15ad5-1127">`az sql container create`: `--unique-key-policy` und `--conflict-resolution-policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1127">`az sql container create`: Added `--unique-key-policy` and `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="15ad5-1128">`az sql container create/update`: Aktualisierung des `--idx`-Standardschemas</span><span class="sxs-lookup"><span data-stu-id="15ad5-1128">`az sql container create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="15ad5-1129">`gremlin graph create`: `--conflict-resolution-policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1129">`gremlin graph create`: Added `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="15ad5-1130">`gremlin graph create/update`: Aktualisierung des `--idx`-Standardschemas</span><span class="sxs-lookup"><span data-stu-id="15ad5-1130">`gremlin graph create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="15ad5-1131">Tippfehler in Hilfemeldung korrigiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-1131">Fixed typo in help message</span></span>
* <span data-ttu-id="15ad5-1132">Datenbank: Informationen zur eingestellten Unterstützung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1132">database: Added deprecation information</span></span>
* <span data-ttu-id="15ad5-1133">Auflistung: Informationen zur eingestellten Unterstützung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1133">collection: Added deprecation information</span></span>

### <a name="iot"></a><span data-ttu-id="15ad5-1134">IoT</span><span class="sxs-lookup"><span data-stu-id="15ad5-1134">IoT</span></span>

* <span data-ttu-id="15ad5-1135">Neuer Routingquelltyp hinzugefügt: DigitalTwinChangeEvents</span><span class="sxs-lookup"><span data-stu-id="15ad5-1135">Added new routing source type: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="15ad5-1136">Fehlende Features in `az iot hub create` behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-1136">Fixed missing features in `az iot hub create`</span></span>

### <a name="key-vault"></a><span data-ttu-id="15ad5-1137">Key Vault</span><span class="sxs-lookup"><span data-stu-id="15ad5-1137">Key Vault</span></span>

* <span data-ttu-id="15ad5-1138">Ein unerwarteter Fehler wurde behoben, bei dem keine Zertifikatdatei vorhanden war.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1138">Fixed an unexpected error when certificate file does not exist</span></span>
* <span data-ttu-id="15ad5-1139">Funktionsunfähigkeit von `az keyvault recover/purge` behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-1139">Fixed `az keyvault recover/purge` not working</span></span>

### <a name="netappfiles"></a><span data-ttu-id="15ad5-1140">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="15ad5-1140">NetAppFiles</span></span>

* <span data-ttu-id="15ad5-1141">„azure-mgmt-netapp“ wurde auf 0.6.0 aktualisiert, um API-Version 2019-07-01 zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1141">Upgraded azure-mgmt-netapp to 0.6.0 to use API version 2019-07-01.</span></span> <span data-ttu-id="15ad5-1142">Diese neue API-Version umfasst:</span><span class="sxs-lookup"><span data-stu-id="15ad5-1142">This new API version includes:</span></span>

    - <span data-ttu-id="15ad5-1143">Volumeerstellung `--protocol-types` akzeptiert jetzt „NFSv4.1“ anstelle von „NFSv4“.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1143">Volume creation `--protocol-types` accepts now "NFSv4.1" not "NFSv4"</span></span>
    - <span data-ttu-id="15ad5-1144">Die Richtlinie der Volumeexportrichtlinie heißt jetzt „nfsv41“ anstelle von „nfsv4“.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1144">Volume export policy property now named 'nfsv41' not 'nfsv4'</span></span>
    - <span data-ttu-id="15ad5-1145">Volume `--creation-token` wurde in `--file-path` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1145">Volume `--creation-token` renamed to `--file-path`</span></span>
    - <span data-ttu-id="15ad5-1146">Das Erstellungsdatum einer Momentaufnahme heißt jetzt einfach „erstellt“.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1146">Snapshot creation date now named just 'created'</span></span>

### <a name="network"></a><span data-ttu-id="15ad5-1147">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="15ad5-1147">Network</span></span>

* <span data-ttu-id="15ad5-1148">`az network private-dns link vnet create/update`: Unterstützung für mandantenübergreifende Verknüpfung virtueller Netzwerke.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1148">`az network private-dns link vnet create/update`: Support cross-tenant virtual network linking.</span></span>
* <span data-ttu-id="15ad5-1149">[BREAKING CHANGE] `az network vnet subnet list`: `--resource-group` und `--vnet-name` wurden geändert und sind jetzt erforderlich.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1149">[BREAKING CHANGE] `az network vnet subnet list`: Changed `--resource-group` and `--vnet-name` to be required now.</span></span>
* <span data-ttu-id="15ad5-1150">`az network public-ip prefix create`: Unterstützung der Angabe der IP-Adressversion (IPv4, IPv6) bei der Erstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1150">`az network public-ip prefix create`: Added support to specify IP address version (IPv4, IPv6) when creation</span></span>
* <span data-ttu-id="15ad5-1151">„azure-mgmt-network“ auf 7.0.0 und „api-version“ auf 2019-09-01 festgelegt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1151">Bumped azure-mgmt-network to 7.0.0 and api-version to 2019-09-01</span></span>
* <span data-ttu-id="15ad5-1152">`az network vrouter`: Unterstützung für neuen virtuellen Dienstrouter und virtuelles Routerpeering hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1152">`az network vrouter`: Added support for new service virtual router and virtual router peering</span></span>
* <span data-ttu-id="15ad5-1153">`az network express-route gateway connection`: Unterstützung für `--internet-security` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1153">`az network express-route gateway connection`: Added support for `--internet-security`</span></span>

### <a name="profile"></a><span data-ttu-id="15ad5-1154">Profil</span><span class="sxs-lookup"><span data-stu-id="15ad5-1154">Profile</span></span>

* <span data-ttu-id="15ad5-1155">Funktionsunfähigkeit von `az account get-access-token --resource-type ms-graph` behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-1155">Fixed `az account get-access-token --resource-type ms-graph` not working</span></span>
* <span data-ttu-id="15ad5-1156">Warnung aus `az login` entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1156">Removed warning from `az login`</span></span>

### <a name="rbac"></a><span data-ttu-id="15ad5-1157">RBAC</span><span class="sxs-lookup"><span data-stu-id="15ad5-1157">RBAC</span></span>

* <span data-ttu-id="15ad5-1158">Funktionsunfähigkeit von `az ad app update --id {} --display-name {}` behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-1158">Fixed `az ad app update --id {} --display-name {}` doesn't work</span></span>

### <a name="servicefabric"></a><span data-ttu-id="15ad5-1159">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="15ad5-1159">ServiceFabric</span></span>

* <span data-ttu-id="15ad5-1160">`az sf cluster create`: Ein Problem wurde behoben, indem die Compute-VMSS von „template.json“ für Service Fabric unter Linux und Windows von Standarddatenträgern auf verwaltete Datenträger umgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1160">`az sf cluster create`: Fixed an issue by modifying service fabric linux and windows template.json compute vmss from standard to managed disks</span></span>

### <a name="sql"></a><span data-ttu-id="15ad5-1161">SQL</span><span class="sxs-lookup"><span data-stu-id="15ad5-1161">SQL</span></span>

* <span data-ttu-id="15ad5-1162">Die Parameter `--compute-model`, `--auto-pause-delay` und `--min-capacity` wurden hinzugefügt, um CRUD-Vorgänge für das neue SQL-Datenbank-Angebot zu unterstützen: Serverloses Computemodell.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1162">Added `--compute-model`, `--auto-pause-delay`, and `--min-capacity` parameters to support CRUD operations for new SQL Database offering: Serverless compute model.</span></span>

### <a name="storage"></a><span data-ttu-id="15ad5-1163">Storage</span><span class="sxs-lookup"><span data-stu-id="15ad5-1163">Storage</span></span>

* <span data-ttu-id="15ad5-1164">`az storage account create/update`: Parameter „--enable-files-adds“ und Azure Active Directory-Eigenschaftenargumentgruppe hinzugefügt, um Active Directory Domain-Dienstauthentifizierung für Azure Files zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1164">`az storage account create/update`: Added --enable-files-adds parameter and Azure Active Directory Properties Argument group to support Azure Files Active Directory Domain Service Authentication</span></span>
* <span data-ttu-id="15ad5-1165">`az storage account keys list/renew` wurde erweitert, um die Auflistung oder erneute Generierung von Kerberos-Schlüsseln des Speicherkontos zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1165">Expanded `az storage account keys list/renew` to support listing or regenerating Kerberos keys of storage account.</span></span>

## <a name="october-15-2019"></a><span data-ttu-id="15ad5-1166">15. Oktober 2019</span><span class="sxs-lookup"><span data-stu-id="15ad5-1166">October 15, 2019</span></span>

<span data-ttu-id="15ad5-1167">Version 2.0.75</span><span class="sxs-lookup"><span data-stu-id="15ad5-1167">Version 2.0.75</span></span>

### <a name="aks"></a><span data-ttu-id="15ad5-1168">AKS</span><span class="sxs-lookup"><span data-stu-id="15ad5-1168">AKS</span></span>

* <span data-ttu-id="15ad5-1169">Standardwert `--load-balancer-sku` in `standard` geändert, sofern von der Kubernetes-Version unterstützt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1169">Changed `--load-balancer-sku` default value to `standard` if supported by the kubernetes version</span></span>
* <span data-ttu-id="15ad5-1170">Standardwert `--vm-set-type` in `virtualmachinescalesets` geändert, sofern von der Kubernetes-Version unterstützt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1170">Changed `--vm-set-type` default value to `virtualmachinescalesets` if supported by the kubernetes version</span></span>

### <a name="ams"></a><span data-ttu-id="15ad5-1171">AMS</span><span class="sxs-lookup"><span data-stu-id="15ad5-1171">AMS</span></span>

* <span data-ttu-id="15ad5-1172">[BREAKING CHANGE] Name von `job start` in `job create` geändert</span><span class="sxs-lookup"><span data-stu-id="15ad5-1172">[BREAKING CHANGE] Changed the name of `job start` to `job create`</span></span>
* <span data-ttu-id="15ad5-1173">[BREAKING CHANGE] Parameter `--ask` von `content-key-policy create` geändert, sodass eine hexadezimale Zeichenfolge mit 32 Zeichen anstelle von UTF8 verwendet wird</span><span class="sxs-lookup"><span data-stu-id="15ad5-1173">[BREAKING CHANGE] Changed the `--ask` parameter of `content-key-policy create` to use a 32-character hex string instead of UTF8</span></span>

### <a name="appservice"></a><span data-ttu-id="15ad5-1174">AppService</span><span class="sxs-lookup"><span data-stu-id="15ad5-1174">AppService</span></span>

* <span data-ttu-id="15ad5-1175">Befehle vom Typ `webapp config access-restriction show|set|add|remove` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1175">Added commands `webapp config access-restriction show|set|add|remove`</span></span>
* <span data-ttu-id="15ad5-1176">Bessere Fehlerbehandlung zu `webapp up` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1176">Added better error handling to `webapp up`</span></span>
* <span data-ttu-id="15ad5-1177">Unterstützung für SKU `Isolated` zu `appservice plan update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1177">Added support for `Isolated` SKU to `appservice plan update`</span></span>

### <a name="arm"></a><span data-ttu-id="15ad5-1178">ARM</span><span class="sxs-lookup"><span data-stu-id="15ad5-1178">ARM</span></span>

* <span data-ttu-id="15ad5-1179">Parameter `--handle-extended-json-format` zu `deployment create` hinzugefügt, um mehrere Zeilen und Kommentare in der JSON-Vorlage zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="15ad5-1179">Added `--handle-extended-json-format` parameter `deployment create` to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="15ad5-1180">Compute</span><span class="sxs-lookup"><span data-stu-id="15ad5-1180">Compute</span></span>

* <span data-ttu-id="15ad5-1181">Parameter `--enable-agent` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1181">Added `--enable-agent` parameter to `vm create`</span></span>
* <span data-ttu-id="15ad5-1182">`vm create` geändert, um bei der Verwendung von Zonen die SKU „Standard“ für die öffentliche IP-Adresse zu verwenden</span><span class="sxs-lookup"><span data-stu-id="15ad5-1182">Changed `vm create` to use standard public IP SKU automatically when using zones</span></span>
* <span data-ttu-id="15ad5-1183">`vm create` geändert, um automatisch einen gültigen Computernamen für eine VM zu erstellen, falls keiner angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="15ad5-1183">Changed `vm create` to automatically create a valid computer name for a VM if none is provided</span></span>
* <span data-ttu-id="15ad5-1184">Parameter `--computer-name-prefix` zu `vmss create` hinzugefügt, um das benutzerdefinierte Computernamenspräfix virtueller Computer in VMSS zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="15ad5-1184">Added `--computer-name-prefix` parameter to `vmss create` to support custom computer name prefix of virtual machines in the VMSS</span></span>
* <span data-ttu-id="15ad5-1185">Parameter `--workspace` zu `vm create` hinzugefügt, um automatisch einen Log Analytics-Arbeitsbereich zu aktivieren</span><span class="sxs-lookup"><span data-stu-id="15ad5-1185">Add `--workspace` parameter to `vm create` to enable log analytics workspace automatically</span></span>
* <span data-ttu-id="15ad5-1186">API-Version für Kataloge auf 2019-07-01 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-1186">Updated galleries API version to 2019-07-01</span></span>

### <a name="core"></a><span data-ttu-id="15ad5-1187">Core</span><span class="sxs-lookup"><span data-stu-id="15ad5-1187">Core</span></span>

* <span data-ttu-id="15ad5-1188">Syntaxprüfung für Parameter `--set` im generischen Updatebefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1188">Added syntax check for `--set` parameter in generic update command</span></span>

### <a name="iot"></a><span data-ttu-id="15ad5-1189">IoT</span><span class="sxs-lookup"><span data-stu-id="15ad5-1189">IoT</span></span>

* <span data-ttu-id="15ad5-1190">Problem behoben, bei dem für `iot hub show` der Fehler „Ressource nicht gefunden.“ zurückgegeben wurde</span><span class="sxs-lookup"><span data-stu-id="15ad5-1190">Fixed an issue where `iot hub show` would incorrectly error with "resource not found"</span></span>

### <a name="monitor"></a><span data-ttu-id="15ad5-1191">Überwachen</span><span class="sxs-lookup"><span data-stu-id="15ad5-1191">Monitor</span></span>

* <span data-ttu-id="15ad5-1192">Unterstützung für CRUD zu `monitor log-analytics workspace` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1192">Added support for CRUD to `monitor log-analytics workspace`</span></span>

### <a name="network"></a><span data-ttu-id="15ad5-1193">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="15ad5-1193">Network</span></span>

* <span data-ttu-id="15ad5-1194">Unterstützung für mandantenübergreifende virtuelle Verbindung zu `network private-dns link vnet [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1194">Added support for cross-tenant virtual linking to `network private-dns link vnet [create|update]`</span></span>
* <span data-ttu-id="15ad5-1195">[BREAKING CHANGE]`network vnet subnet list` geändert, um Parameter `--resource-group` und `--vnet-name` vorauszusetzen</span><span class="sxs-lookup"><span data-stu-id="15ad5-1195">[BREAKING CHANGE] Changed `network vnet subnet list` to require `--resource-group` and `--vnet-name` parameters</span></span>

### <a name="sql"></a><span data-ttu-id="15ad5-1196">SQL</span><span class="sxs-lookup"><span data-stu-id="15ad5-1196">SQL</span></span>

* <span data-ttu-id="15ad5-1197">Befehle zu `sql mi ad-admin` hinzugefügt, die das Festlegen eines AAD-Administrators für verwaltete Instanzen unterstützen</span><span class="sxs-lookup"><span data-stu-id="15ad5-1197">Added commands to `sql mi ad-admin` that support setting an AAD administrator on managed instances</span></span>

### <a name="storage"></a><span data-ttu-id="15ad5-1198">Storage</span><span class="sxs-lookup"><span data-stu-id="15ad5-1198">Storage</span></span>

* <span data-ttu-id="15ad5-1199">Parameter `--preserve-s2s-access-tier` zu `storage copy` hinzugefügt, um die Zugriffsebene beim Kopieren von Dienst zu Dienst beizubehalten</span><span class="sxs-lookup"><span data-stu-id="15ad5-1199">Added `--preserve-s2s-access-tier` parameter `storage copy` to preserve access tier during service to service copy</span></span>
* <span data-ttu-id="15ad5-1200">Parameter `--enable-large-file-share` zu `storage account [create|update]` hinzugefügt, um große Dateifreigaben für ein Speicherkonto zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="15ad5-1200">Added `--enable-large-file-share` parameter to `storage account [create|update]` to support large file shares for storage account</span></span>

## <a name="september-24-2019"></a><span data-ttu-id="15ad5-1201">24. September 2019</span><span class="sxs-lookup"><span data-stu-id="15ad5-1201">September 24, 2019</span></span>

<span data-ttu-id="15ad5-1202">Version 2.0.74</span><span class="sxs-lookup"><span data-stu-id="15ad5-1202">Version 2.0.74</span></span>

### <a name="acr"></a><span data-ttu-id="15ad5-1203">ACR</span><span class="sxs-lookup"><span data-stu-id="15ad5-1203">ACR</span></span>

* <span data-ttu-id="15ad5-1204">Erforderlicher Parameter `--type` zu `acr config retention update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1204">Added a required `--type` parameter to `acr config retention update`</span></span>
* <span data-ttu-id="15ad5-1205">[BREAKING CHANGE] Umbenannter Parameter `--name -n` in `--registry -r ` für Befehlsgruppe `acr config` geändert</span><span class="sxs-lookup"><span data-stu-id="15ad5-1205">[BREAKING CHANGE] Renamed parameter `--name -n` changed to `--registry -r ` for `acr config` command group</span></span>

### <a name="aks"></a><span data-ttu-id="15ad5-1206">AKS</span><span class="sxs-lookup"><span data-stu-id="15ad5-1206">AKS</span></span>

* <span data-ttu-id="15ad5-1207">Parameter `--load-balancer-sku` zum Befehl `aks create` hinzugefügt, um die Erstellung von AKS-Clustern mit SLB zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="15ad5-1207">Added `--load-balancer-sku` parameter to `aks create` command, which allows for creating AKS cluster with SLB</span></span>
* <span data-ttu-id="15ad5-1208">Parameter `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` und `--load-balancer-outbound-ip-prefixes` zu den Befehlen `aks [create|update]` hinzugefügt,um die Aktualisierung des Lastenausgleichsprofils eines AKS-Clusters mit SLB zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="15ad5-1208">Added `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` and `--load-balancer-outbound-ip-prefixes` parameters to `aks [create|update]` commands, which allow for updating load balancer profile of an AKS cluster with SLB</span></span>
* <span data-ttu-id="15ad5-1209">Parameter `--vm-set-type` zum Befehl `aks create` hinzugefügt, um die Angabe von VM-Typen eines AKS-Clusters (vmas oder vmss) zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="15ad5-1209">Added `--vm-set-type` parameter to `aks create` command, which allows to specify vm types of an AKS Cluster (vmas or vmss)</span></span>

### <a name="arm"></a><span data-ttu-id="15ad5-1210">ARM</span><span class="sxs-lookup"><span data-stu-id="15ad5-1210">ARM</span></span>

* <span data-ttu-id="15ad5-1211">Parameter `--handle-extended-json-format` zum Befehl `group deployment create` hinzugefügt, um mehrere Zeilen und Kommentare in der JSON-Vorlage zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="15ad5-1211">Added `--handle-extended-json-format` parameter to `group deployment create` command to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="15ad5-1212">Compute</span><span class="sxs-lookup"><span data-stu-id="15ad5-1212">Compute</span></span>

* <span data-ttu-id="15ad5-1213">Parameter `--terminate-notification-time` zu den Befehlen `vmss [create|update]` hinzugefügt, um die Konfigurierbarkeit der Beendigung geplanter Ereignisse zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="15ad5-1213">Added `--terminate-notification-time` parameter to `vmss [create|update]` commands to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="15ad5-1214">Parameter `--enable-terminate-notification` zu den Befehlen `vmss update` hinzugefügt, um die Konfigurierbarkeit der Beendigung geplanter Ereignisse zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="15ad5-1214">Added `--enable-terminate-notification` parameter to `vmss update` command to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="15ad5-1215">Parameter `--priority,` `--eviction-policy,` `--max-billing` zu `[vm|vmss] create`-Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1215">Added `--priority,` `--eviction-policy,` `--max-billing` parameters to `[vm|vmss] create` commands</span></span>
* <span data-ttu-id="15ad5-1216">`disk create` geändert, um die Angabe der genauen Größe des Datenträgeruploads zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="15ad5-1216">Changed `disk create` to allow specifying the exact size of the disk upload</span></span>
* <span data-ttu-id="15ad5-1217">Unterstützung für inkrementelle Momentaufnahmen für verwaltete Datenträger zu `snapshot create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1217">Added support for incremental snapshots for managed disks to `snapshot create`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="15ad5-1218">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="15ad5-1218">Cosmos DB</span></span>

* <span data-ttu-id="15ad5-1219">Parameter `--type <key-type>` zum Befehl `cosmosdb keys list` hinzugefügt, um Schlüssel, schreibgeschützte Schlüssel oder Verbindungszeichenfolgen anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="15ad5-1219">Added `--type <key-type>` parameter to `cosmosdb keys list` command to show key, read only keys or connection strings</span></span>
* <span data-ttu-id="15ad5-1220">Befehl `cosmosdb keys regenerate` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1220">Added `cosmosdb keys regenerate` command</span></span>
* <span data-ttu-id="15ad5-1221">[VERALTET] Befehle `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` und `cosmosdb list-read-only-keys` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-1221">[DEPRECATED] Deprecated `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` and `cosmosdb list-read-only-keys` commands</span></span>

### <a name="eventgrid"></a><span data-ttu-id="15ad5-1222">EventGrid</span><span class="sxs-lookup"><span data-stu-id="15ad5-1222">EventGrid</span></span>

* <span data-ttu-id="15ad5-1223">Endpunkthilfetext korrigiert, um auf den richtigen Parameter zu verweisen</span><span class="sxs-lookup"><span data-stu-id="15ad5-1223">Fixed the endpoint help text to refer to the right parameter</span></span>

### <a name="key-vault"></a><span data-ttu-id="15ad5-1224">Key Vault</span><span class="sxs-lookup"><span data-stu-id="15ad5-1224">Key Vault</span></span>

* <span data-ttu-id="15ad5-1225">Problem behoben, aufgrund dessen die Anmeldung mit einem Mandanten (`login -t`) unter Umständen zu einem Fehler von `keyvault create` führte</span><span class="sxs-lookup"><span data-stu-id="15ad5-1225">Fixed issue where logging in with a tenant (`login -t`) could cause `keyvault create` to fail</span></span>

### <a name="monitor"></a><span data-ttu-id="15ad5-1226">Überwachen</span><span class="sxs-lookup"><span data-stu-id="15ad5-1226">Monitor</span></span>

* <span data-ttu-id="15ad5-1227">Problem behoben, aufgrund dessen das Zeichen `:` in `--condition` für `monitor metrics alert create` nicht zulässig war</span><span class="sxs-lookup"><span data-stu-id="15ad5-1227">Fixed issue where `:` character was not allowed in `--condition` argument to `monitor metrics alert create`</span></span>

### <a name="policy"></a><span data-ttu-id="15ad5-1228">Richtlinie</span><span class="sxs-lookup"><span data-stu-id="15ad5-1228">Policy</span></span>

* <span data-ttu-id="15ad5-1229">Unterstützung für Policy-API-Version 2019-06-01 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1229">Added support for Policy API version 2019-06-01</span></span>
* <span data-ttu-id="15ad5-1230">Parameter `--enforcement-mode` zum Befehl `policy assignment create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1230">Added `--enforcement-mode` parameter to `policy assignment create` command</span></span>

### <a name="storage"></a><span data-ttu-id="15ad5-1231">Storage</span><span class="sxs-lookup"><span data-stu-id="15ad5-1231">Storage</span></span>

* <span data-ttu-id="15ad5-1232">Parameter `--blob-type` zum Befehl `az storage copy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1232">Added `--blob-type` parameter to `az storage copy` command</span></span>

## <a name="september-10-2019"></a><span data-ttu-id="15ad5-1233">10. September 2019</span><span class="sxs-lookup"><span data-stu-id="15ad5-1233">September 10, 2019</span></span>

### <a name="acr"></a><span data-ttu-id="15ad5-1234">ACR</span><span class="sxs-lookup"><span data-stu-id="15ad5-1234">ACR</span></span>

* <span data-ttu-id="15ad5-1235">Befehlsgruppe `acr config retention` zum Konfigurieren der Aufbewahrungsrichtlinie hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1235">Added command group `acr config retention` to configure retention policy</span></span>

### <a name="aks"></a><span data-ttu-id="15ad5-1236">AKS</span><span class="sxs-lookup"><span data-stu-id="15ad5-1236">AKS</span></span>

* <span data-ttu-id="15ad5-1237">Unterstützung für die ACR-Integration mit den folgenden Befehlen hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="15ad5-1237">Added support for ACR integration with the following commands:</span></span>
  * <span data-ttu-id="15ad5-1238">Parameter `--attach-acr` zu `aks [create|update]` hinzugefügt, um einen ACR an einen AKS-Cluster anzufügen</span><span class="sxs-lookup"><span data-stu-id="15ad5-1238">Added `--attach-acr` parameter to `aks [create|update]` to attach an ACR to an AKS cluster</span></span>
  * <span data-ttu-id="15ad5-1239">Parameter `--detach-acr` zu `aks update` hinzugefügt, um den ACR von einem AKS-Cluster zu trennen</span><span class="sxs-lookup"><span data-stu-id="15ad5-1239">Added `--detach-acr` parameter to `aks update` to detach the ACR from an AKS cluster</span></span>

### <a name="arm"></a><span data-ttu-id="15ad5-1240">ARM</span><span class="sxs-lookup"><span data-stu-id="15ad5-1240">ARM</span></span>

* <span data-ttu-id="15ad5-1241">Zur Verwendung der API-Version 2019-05-10 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-1241">Updated to use API version 2019-05-10</span></span>

### <a name="batch"></a><span data-ttu-id="15ad5-1242">Batch</span><span class="sxs-lookup"><span data-stu-id="15ad5-1242">Batch</span></span>

* <span data-ttu-id="15ad5-1243">Neue JSON-Konfigurationseinstellungen für `batch pool create` zu `--json-file` hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="15ad5-1243">Added new JSON configuration settings to `--json-file` for `batch pool create`:</span></span>
  * <span data-ttu-id="15ad5-1244">`MountConfigurations` für Dateisystemeinbindungen hinzugefügt (Details siehe https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body )</span><span class="sxs-lookup"><span data-stu-id="15ad5-1244">Added `MountConfigurations` for file system mounts (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
  * <span data-ttu-id="15ad5-1245">Optionale Eigenschaft `publicIPs` in `NetworkConfiguration` für öffentliche IP-Adressen für Pools hinzugefügt (Details siehe https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body )</span><span class="sxs-lookup"><span data-stu-id="15ad5-1245">Added optional property `publicIPs` on `NetworkConfiguration` for public IPs on pools (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
* <span data-ttu-id="15ad5-1246">Unterstützung für Kataloge mit freigegebenen Images zu `--image` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1246">Added support for shared image galleries to `--image`</span></span>
* <span data-ttu-id="15ad5-1247">[BREAKING CHANGE] Standardwert von `--start-task-wait-for-success` für `batch pool create` in `true` geändert</span><span class="sxs-lookup"><span data-stu-id="15ad5-1247">[BREAKING CHANGE] Changed default value of `--start-task-wait-for-success` on `batch pool create` to be `true`</span></span>
* <span data-ttu-id="15ad5-1248">[BREAKING CHANGE] Standardwert von `Scope` für `AutoUserSpecification` geändert, damit immer „Pool“ verwendet wird (vormals `Task` für Windows-Knoten bzw. `Pool` für Linux-Knoten)</span><span class="sxs-lookup"><span data-stu-id="15ad5-1248">[BREAKING CHANGE] Changed default value for `Scope` on `AutoUserSpecification` to always be Pool (was `Task` on Windows nodes, `Pool` on Linux nodes)</span></span>
  * <span data-ttu-id="15ad5-1249">Dieses Argument kann nur über eine JSON-Konfiguration mit `--json-file` festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1249">This argument can only be set from a JSON configuration with `--json-file`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="15ad5-1250">HDInsight</span><span class="sxs-lookup"><span data-stu-id="15ad5-1250">HDInsight</span></span>

* <span data-ttu-id="15ad5-1251">Allgemein verfügbares Release</span><span class="sxs-lookup"><span data-stu-id="15ad5-1251">GA release</span></span>
* <span data-ttu-id="15ad5-1252">[BREAKING CHANGE] Parameter `--workernode-count/-c` von `az hdinsight resize` in erforderlich geändert</span><span class="sxs-lookup"><span data-stu-id="15ad5-1252">[BREAKING CHANGE] Changed parameter `--workernode-count/-c` of `az hdinsight resize` to be required.</span></span>

### <a name="key-vault"></a><span data-ttu-id="15ad5-1253">Key Vault</span><span class="sxs-lookup"><span data-stu-id="15ad5-1253">Key Vault</span></span>

* <span data-ttu-id="15ad5-1254">Problem behoben, aufgrund dessen Subnetze nicht aus Netzwerkregeln gelöscht werden konnten</span><span class="sxs-lookup"><span data-stu-id="15ad5-1254">Fixed issue where subnets couldn't be deleted from network rules</span></span>
* <span data-ttu-id="15ad5-1255">Problem behoben, aufgrund dessen doppelte Subnetze und IP-Adressen zu Netzwerkregeln hinzugefügt werden konnten</span><span class="sxs-lookup"><span data-stu-id="15ad5-1255">Fixed issue where duplicated subnets and IP addresses could be added to network rules</span></span>

### <a name="network"></a><span data-ttu-id="15ad5-1256">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="15ad5-1256">Network</span></span>

* <span data-ttu-id="15ad5-1257">Parameter `--interval` zu `network watcher flow-log` hinzugefügt, um den Wert für das Intervall der Datenverkehrsanalyse festzulegen</span><span class="sxs-lookup"><span data-stu-id="15ad5-1257">Added `--interval` parameter to `network watcher flow-log` to set traffic analysis interval value</span></span>
* <span data-ttu-id="15ad5-1258">`network application-gateway identity` zum Verwalten der Gatewayidentität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1258">Added `network application-gateway identity` to manage gateway identity</span></span>
* <span data-ttu-id="15ad5-1259">Unterstützung zum Festlegen der Key Vault-ID zu `network application-gateway ssl-cert` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1259">Added support for setting Key Vault ID to `network application-gateway ssl-cert`</span></span>
* <span data-ttu-id="15ad5-1260">`network express-route peering peer-connection [show|list]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1260">Added `network express-route peering peer-connection [show|list]`</span></span>

### <a name="policy"></a><span data-ttu-id="15ad5-1261">Richtlinie</span><span class="sxs-lookup"><span data-stu-id="15ad5-1261">Policy</span></span>

* <span data-ttu-id="15ad5-1262">Zur Verwendung der API-Version 2019-01-01 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-1262">Updated to use API version 2019-01-01</span></span>

## <a name="august-27-2019"></a><span data-ttu-id="15ad5-1263">27. August 2019</span><span class="sxs-lookup"><span data-stu-id="15ad5-1263">August 27, 2019</span></span>

<span data-ttu-id="15ad5-1264">Version 2.0.72</span><span class="sxs-lookup"><span data-stu-id="15ad5-1264">Version 2.0.72</span></span>

### <a name="acr"></a><span data-ttu-id="15ad5-1265">ACR</span><span class="sxs-lookup"><span data-stu-id="15ad5-1265">ACR</span></span>

* <span data-ttu-id="15ad5-1266">[BREAKING CHANGE] Unterstützung für SKU `classic` entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1266">[BREAKING CHANGE] Removed support for the `classic` SKU</span></span>

### <a name="api-management"></a><span data-ttu-id="15ad5-1267">API Management</span><span class="sxs-lookup"><span data-stu-id="15ad5-1267">API Management</span></span>

* <span data-ttu-id="15ad5-1268">[VORSCHAU] Befehlsgruppe `apim` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1268">[PREVIEW] Added `apim` command group</span></span>

### <a name="appservice"></a><span data-ttu-id="15ad5-1269">AppService</span><span class="sxs-lookup"><span data-stu-id="15ad5-1269">AppService</span></span>

* <span data-ttu-id="15ad5-1270">Problem mit dem Befehl `webapp webjob continuous start` bei Angabe eines Slots behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-1270">Fixed issue with `webapp webjob continuous start` command when specifying a slot</span></span>
* <span data-ttu-id="15ad5-1271">`webapp up` geändert, um den Ordner `env` zu erkennen und aus der für die Bereitstellung verwendeten Datei zu entfernen</span><span class="sxs-lookup"><span data-stu-id="15ad5-1271">Changed `webapp up` to detect `env` folder and remove it from the file used for deployment</span></span>

### <a name="keyvault"></a><span data-ttu-id="15ad5-1272">KeyVault</span><span class="sxs-lookup"><span data-stu-id="15ad5-1272">Keyvault</span></span>

* <span data-ttu-id="15ad5-1273">Fehler in `keyvault secret set` behoben, aufgrund dessen das Argument `--expires` ignoriert wurde</span><span class="sxs-lookup"><span data-stu-id="15ad5-1273">Fixed a bug in `keyvault secret set` that igored the `--expires` argument</span></span>

### <a name="network"></a><span data-ttu-id="15ad5-1274">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="15ad5-1274">Network</span></span>

* <span data-ttu-id="15ad5-1275">Unterstützung für IPv6-Adressen zu Argumenten vom Typ `--private-ip-address-version` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1275">Added support for IPv6 addresses to `--private-ip-address-version` arguments</span></span>
* <span data-ttu-id="15ad5-1276">Neue Befehle vom Typ `network private-endpoint [create|update|list-types]` für die Verwaltung privater Endpunkte hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1276">Added new commands `network private-endpoint [create|update|list-types]` for private endpoint management</span></span>
* <span data-ttu-id="15ad5-1277">Befehlsgruppe `network private-link-service` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1277">Added command group `network private-link-service`</span></span>
* <span data-ttu-id="15ad5-1278">Argumente `--private-endpoint-network-policies` und `--private-link-service-network-policies` zu `network vnet subnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1278">Added `--private-endpoint-network-policies` and `--private-link-service-network-policies` arguments to `network vnet subnet update`</span></span>

### <a name="rbac"></a><span data-ttu-id="15ad5-1279">RBAC</span><span class="sxs-lookup"><span data-stu-id="15ad5-1279">RBAC</span></span>

* <span data-ttu-id="15ad5-1280">Problem mit `ad app update --homepage` behoben, aufgrund dessen die Startseite nicht aktualisiert wurde</span><span class="sxs-lookup"><span data-stu-id="15ad5-1280">Fixed issue with `ad app update --homepage` where homepage would not be updated</span></span>

### <a name="servicefabric"></a><span data-ttu-id="15ad5-1281">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="15ad5-1281">ServiceFabric</span></span>

* <span data-ttu-id="15ad5-1282">Unterstützung für Key Vault-Namen mit Groß- und Kleinschreibung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1282">Added support for mixed-case Key Vault names</span></span>
* <span data-ttu-id="15ad5-1283">Problem bei der Verwendung von Zertifikaten in Key Vault behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-1283">Fixed issue when using certificates in Key Vault</span></span>
* <span data-ttu-id="15ad5-1284">Problem bei der Verwendung von PFX-Zertifikatdateien behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-1284">Fixed issue with using PFX certificate files</span></span>
* <span data-ttu-id="15ad5-1285">Problem mit `sf cluster certificate add` behoben, wenn keine Key Vault-Ressourcengruppe angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="15ad5-1285">Fixed issue with `sf cluster certificate add` when Key Vault resource group wasn't specified</span></span>
* <span data-ttu-id="15ad5-1286">Problem behoben, aufgrund dessen `sf cluster set` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="15ad5-1286">Fixed issue with `sf cluster set` not working</span></span>

### <a name="signalr"></a><span data-ttu-id="15ad5-1287">SignalR</span><span class="sxs-lookup"><span data-stu-id="15ad5-1287">SignalR</span></span>

* <span data-ttu-id="15ad5-1288">Neue Befehle hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="15ad5-1288">Added new commands:</span></span>
  * <span data-ttu-id="15ad5-1289">`signalr cors`: Verwalten von CORS für SignalR</span><span class="sxs-lookup"><span data-stu-id="15ad5-1289">`signalr cors`: Manage SignalR CORS</span></span>
  * <span data-ttu-id="15ad5-1290">`signalr restart`: Starten eines SignalR-Diensts</span><span class="sxs-lookup"><span data-stu-id="15ad5-1290">`signalr restart`: Restart a SignalR service</span></span>
  * <span data-ttu-id="15ad5-1291">`signalr update`: Aktualisieren eines SignalR-Diensts</span><span class="sxs-lookup"><span data-stu-id="15ad5-1291">`signalr update`: Update a SignalR service</span></span>
* <span data-ttu-id="15ad5-1292">Argument `--service-mode` zu `signalr create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1292">Added `--service-mode` argument to `signalr create`</span></span>

### <a name="storage"></a><span data-ttu-id="15ad5-1293">Storage</span><span class="sxs-lookup"><span data-stu-id="15ad5-1293">Storage</span></span>

* <span data-ttu-id="15ad5-1294">Befehl `storage account revoke-delegation-keys` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1294">Added `storage account revoke-delegation-keys` command</span></span>

## <a name="august-13-2019"></a><span data-ttu-id="15ad5-1295">13. August 2019</span><span class="sxs-lookup"><span data-stu-id="15ad5-1295">August 13, 2019</span></span>

<span data-ttu-id="15ad5-1296">Version 2.0.71</span><span class="sxs-lookup"><span data-stu-id="15ad5-1296">Version 2.0.71</span></span>

### <a name="appservice"></a><span data-ttu-id="15ad5-1297">AppService</span><span class="sxs-lookup"><span data-stu-id="15ad5-1297">AppService</span></span>

* <span data-ttu-id="15ad5-1298">Problem behoben, aufgrund dessen bei Befehlen vom Typ `webapp webjob continuous` für Slots Fehler auftraten</span><span class="sxs-lookup"><span data-stu-id="15ad5-1298">Fixed issue where `webapp webjob continuous` commands were failing for slots</span></span>

### <a name="botservice"></a><span data-ttu-id="15ad5-1299">BotService</span><span class="sxs-lookup"><span data-stu-id="15ad5-1299">BotService</span></span>

* <span data-ttu-id="15ad5-1300">[BREAKING CHANGE] Unterstützung für die Erstellung von Bots der Version 3 entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1300">[BREAKING CHANGE] Removed support for creating v3 SDK bots</span></span>

### <a name="cognitiveservices"></a><span data-ttu-id="15ad5-1301">CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="15ad5-1301">CognitiveServices</span></span>

* <span data-ttu-id="15ad5-1302">Befehle vom Typ `cognitiveservices account network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1302">Added `cognitiveservices account network-rule` commands</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="15ad5-1303">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="15ad5-1303">Cosmos DB</span></span>

* <span data-ttu-id="15ad5-1304">Beim Aktualisieren mehrerer Schreibstandorte wurde eine Warnung entfernt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1304">Removed warning when updating multiple write locations</span></span>
* <span data-ttu-id="15ad5-1305">CRUD-Befehle für CosmosDB SQL-, MongoDB-, Cassandra-, Gremlin- und Tabellenressourcen sowie den Ressourcendurchsatz hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1305">Added CRUD commands for CosmosDB SQL, MongoDB, Cassandra, Gremlin and Table resources and resource's throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="15ad5-1306">HDInsight</span><span class="sxs-lookup"><span data-stu-id="15ad5-1306">HDInsight</span></span>

<span data-ttu-id="15ad5-1307">Dieses Release enthält zahlreiche wichtige Änderungen.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1307">This release contains a large number of breaking changes.</span></span>

* <span data-ttu-id="15ad5-1308">[BREAKING CHANGE] Parameter für `hdinsight create` umbenannt:</span><span class="sxs-lookup"><span data-stu-id="15ad5-1308">[BREAKING CHANGE] Renamed parameters for `hdinsight create`:</span></span>
  * <span data-ttu-id="15ad5-1309">`--storage-default-container` in `--storage-container` umbenannt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1309">Renamed `--storage-default-container` to `--storage-container`</span></span>
  * <span data-ttu-id="15ad5-1310">`--storage-default-filesystem` in `--storage-filesystem` umbenannt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1310">Renamed `--storage-default-filesystem` to `--storage-filesystem`</span></span>
* <span data-ttu-id="15ad5-1311">[BREAKING CHANGE] Das Argument `--name` von `application create` wurde so geändert, dass es den Anwendungsnamen anstelle des Clusternamens darstellt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1311">[BREAKING CHANGE] Changed the `--name` argument of `application create` to represent the application name instead of the cluster name</span></span>
* <span data-ttu-id="15ad5-1312">Argument `--cluster-name` zu `application create` hinzugefügt, um die alte Funktion `--name` zu ersetzen</span><span class="sxs-lookup"><span data-stu-id="15ad5-1312">Added `--cluster-name` argument to `application create` to replace old `--name` functionality</span></span>
* <span data-ttu-id="15ad5-1313">[BREAKING CHANGE] Parameter für `application create` umbenannt:</span><span class="sxs-lookup"><span data-stu-id="15ad5-1313">[BREAKING CHANGE] Renamed parameters for `application create`:</span></span>
  * <span data-ttu-id="15ad5-1314">`--application-type` in `--type` umbenannt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1314">Renamed `--application-type` to `--type`</span></span>
  * <span data-ttu-id="15ad5-1315">`--marketplace-identifier` in `--marketplace-id` umbenannt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1315">Renamed `--marketplace-identifier` to `--marketplace-id`</span></span>
  * <span data-ttu-id="15ad5-1316">`--https-endpoint-access-mode` in `--access-mode` umbenannt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1316">Renamed `--https-endpoint-access-mode` to `--access-mode`</span></span>
  * <span data-ttu-id="15ad5-1317">`--https-endpoint-destination-port` in `--destination-port` umbenannt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1317">Renamed  `--https-endpoint-destination-port` to `--destination-port`</span></span>
* <span data-ttu-id="15ad5-1318">[BREAKING CHANGE] Parameter für `application create` entfernt:</span><span class="sxs-lookup"><span data-stu-id="15ad5-1318">[BREAKING CHANGE] Removed parameters for `application create`:</span></span>
  * `--https-endpoint-location`
  * `--https-endpoint-public-port`
  * `--ssh-endpoint-destination-port`
  * `--ssh-endpoint-location`
  * `--ssh-endpoint-public-port`
* <span data-ttu-id="15ad5-1319">[WICHTIGE ÄNDERUNG] `--target-instance-count` für `hdinsight resize` in `--workernode-count` umbenannt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1319">[BREAKING CHNAGE] Renamed `--target-instance-count` to `--workernode-count` for `hdinsight resize`</span></span>
* <span data-ttu-id="15ad5-1320">[BREAKING CHANGE] Alle Befehle in der Gruppe `hdinsight script-action` wurden so geändert, dass sie den Parameter `--name` als Namen der Skriptaktion verwenden.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1320">[BREAKING CHANGE] Changed all commands in the `hdinsight script-action` group to use the `--name` parameter as the name of the script action.</span></span>
* <span data-ttu-id="15ad5-1321">Argument `--cluster-name` zu allen Befehlen vom Typ `hdinsight script-action` hinzugefügt, um die alte Funktion `--name` zu ersetzen</span><span class="sxs-lookup"><span data-stu-id="15ad5-1321">Added `--cluster-name` argument to all `hdinsight script-action` commands to replace old `--name` functionality</span></span>
* <span data-ttu-id="15ad5-1322">[BREAKING CHANGE]`--script-execution-id` für alle Befehle vom Typ `hdinsight script-action` in `--execution-id` umbenannt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1322">[BREAKING CHANGE] Renamed `--script-execution-id` to `--execution-id` for all `hdinsight script-action` commands</span></span>
* <span data-ttu-id="15ad5-1323">[BREAKING CHANGE]`hdinsight script-action show` in `hdinsight script-action show-execution-details` umbenannt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1323">[BREAKING CHANGE] Renamed `hdinsight script-action show` to `hdinsight script-action show-execution-details`</span></span>
* <span data-ttu-id="15ad5-1324">[WICHTIGE ÄNDERUNG] Parameter in `hdinsight script-action execute --roles` geändert, sodass sie durch Leerzeichen anstelle von Kommas getrennt sind</span><span class="sxs-lookup"><span data-stu-id="15ad5-1324">[BREAKING CHNAGE] Changed parameters to `hdinsight script-action execute --roles` to be space-separated instead of comma-separated</span></span>
* <span data-ttu-id="15ad5-1325">[BREAKING CHANGE] Parameter `--persisted` für `hdinsight script-action list` entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1325">[BREAKING CHANGE] Removed the `--persisted` parameter of `hdinsight script-action list`</span></span>
* <span data-ttu-id="15ad5-1326">Der Parameter `hdinsight create --cluster-configurations` wurde so geändert, dass er einen Pfad zu einer lokalen JSON-Datei oder JSON-Zeichenfolge akzeptiert.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1326">Changed the `hdinsight create --cluster-configurations` parameter to accept a path to a local JSON file or a JSON string</span></span>
* <span data-ttu-id="15ad5-1327">Befehl `hdinsight script-action list-execution-history` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1327">Added command `hdinsight script-action list-execution-history`</span></span>
* <span data-ttu-id="15ad5-1328">`hdinsight monitor enable --workspace` geändert, um die ID oder den Namen eines Log Analytics-Arbeitsbereichs zu akzeptieren</span><span class="sxs-lookup"><span data-stu-id="15ad5-1328">Changed `hdinsight monitor enable --workspace` to accept a Log Analytics workspace ID or workspace name</span></span>
* <span data-ttu-id="15ad5-1329">Argument `hdinsight monitor enable --primary-key` hinzugefügt. Dieses Argument wird benötigt, wenn eine Arbeitsbereichs-ID als Parameter angegeben wird.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1329">Added the `hdinsight monitor enable --primary-key` argument, which is needed if a workspace ID is provided as the parameter</span></span>
* <span data-ttu-id="15ad5-1330">Weitere Beispiele und aktualisierte Beschreibungen für Hilfemeldungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1330">Added more examples and updated descriptions for help messages</span></span>

### <a name="interactive"></a><span data-ttu-id="15ad5-1331">Interactive</span><span class="sxs-lookup"><span data-stu-id="15ad5-1331">Interactive</span></span>

* <span data-ttu-id="15ad5-1332">Ladefehler behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-1332">Fixed a loading error</span></span>

### <a name="kubernetes"></a><span data-ttu-id="15ad5-1333">Kubernetes</span><span class="sxs-lookup"><span data-stu-id="15ad5-1333">Kubernetes</span></span>

* <span data-ttu-id="15ad5-1334">Änderung, um `https` zu verwenden, wenn der Dashboardcontainerport `https` verwendet</span><span class="sxs-lookup"><span data-stu-id="15ad5-1334">Changed to use `https` if dashboard container port is using `https`</span></span>

### <a name="network"></a><span data-ttu-id="15ad5-1335">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="15ad5-1335">Network</span></span>

* <span data-ttu-id="15ad5-1336">Argument `--yes` hinzugefügt zu `network dns record-set cname delete`</span><span class="sxs-lookup"><span data-stu-id="15ad5-1336">Added `--yes` argument `network dns record-set cname delete`</span></span>

### <a name="profile"></a><span data-ttu-id="15ad5-1337">Profil</span><span class="sxs-lookup"><span data-stu-id="15ad5-1337">Profile</span></span>

* <span data-ttu-id="15ad5-1338">Argument `--resource-type` zu `account get-access-token` zum Abrufen von Ressourcenzugriffstoken hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1338">Added `--resource-type` argument to `account get-access-token` to get resource access tokens</span></span>

### <a name="servicefabric"></a><span data-ttu-id="15ad5-1339">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="15ad5-1339">ServiceFabric</span></span>

* <span data-ttu-id="15ad5-1340">Alle unterstützten Betriebssystemversionen für „sf cluster create“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1340">Added all supported os version for sf cluster create</span></span>
* <span data-ttu-id="15ad5-1341">Fehler beim Überprüfen des primären Zertifikats behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-1341">Fixed primary certificate validation bug</span></span>

### <a name="storage"></a><span data-ttu-id="15ad5-1342">Storage</span><span class="sxs-lookup"><span data-stu-id="15ad5-1342">Storage</span></span>

* <span data-ttu-id="15ad5-1343">Befehl `storage copy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1343">Added command `storage copy`</span></span>

## <a name="july-30-2019"></a><span data-ttu-id="15ad5-1344">30. Juli 2019</span><span class="sxs-lookup"><span data-stu-id="15ad5-1344">July 30, 2019</span></span>

<span data-ttu-id="15ad5-1345">Version 2.0.70</span><span class="sxs-lookup"><span data-stu-id="15ad5-1345">Version 2.0.70</span></span>

### <a name="acr"></a><span data-ttu-id="15ad5-1346">ACR</span><span class="sxs-lookup"><span data-stu-id="15ad5-1346">ACR</span></span>

* <span data-ttu-id="15ad5-1347">Problem #9952 behoben (Regression im Befehl `acr pack build`)</span><span class="sxs-lookup"><span data-stu-id="15ad5-1347">Fixed issue #9952 (a regression in the `acr pack build` command)</span></span>
* <span data-ttu-id="15ad5-1348">Standardname des Generatorimages in `acr pack build` entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1348">Removed the default builder image name in `acr pack build`</span></span>

### <a name="appservice"></a><span data-ttu-id="15ad5-1349">AppService</span><span class="sxs-lookup"><span data-stu-id="15ad5-1349">Appservice</span></span>

* <span data-ttu-id="15ad5-1350">`webapp config ssl` geändert, um eine Meldung anzuzeigen, wenn eine Ressource nicht gefunden wurde</span><span class="sxs-lookup"><span data-stu-id="15ad5-1350">Changed `webapp config ssl` to show a message if a resource is not found</span></span>
* <span data-ttu-id="15ad5-1351">Problem behoben, aufgrund dessen `functionapp create` den Speicherkontotypen `Standard_RAGRS` nicht akzeptiert hat</span><span class="sxs-lookup"><span data-stu-id="15ad5-1351">Fixed issue where `functionapp create` does not accept `Standard_RAGRS` storage account type</span></span>
* <span data-ttu-id="15ad5-1352">Problem behoben, aufgrund dessen für `webapp up` ein Fehler auftrat, wenn für die Ausführung ältere Python-Versionen verwendet wurden</span><span class="sxs-lookup"><span data-stu-id="15ad5-1352">Fixed an issue where `webapp up` would fail if run using older versions of python</span></span>

### <a name="network"></a><span data-ttu-id="15ad5-1353">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="15ad5-1353">Network</span></span>

* <span data-ttu-id="15ad5-1354">Ungültiger Parameter `--ids` aus `network nic ip-config add` entfernt (Fehlerbehebungen #9861)</span><span class="sxs-lookup"><span data-stu-id="15ad5-1354">Removed invalid parameter `--ids` from `network nic ip-config add` (fixes #9861)</span></span>
* <span data-ttu-id="15ad5-1355">Fehlerbehebungen #9604.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1355">Fixes #9604.</span></span> <span data-ttu-id="15ad5-1356">Parameter `--root-certs` zu `network application-gateway http-settings [create|update]` hinzugefügt, um vom Benutzer zugewiesene vertrauenswürdige Stammzertifikate zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1356">Added `--root-certs` parameter to `network application-gateway http-settings [create|update]` to support user associate trusted root certificates.</span></span>
* <span data-ttu-id="15ad5-1357">Argument `--subscription` für `network dns record-set ns create` korrigiert (#9965)</span><span class="sxs-lookup"><span data-stu-id="15ad5-1357">Fixed arguent `--subscription` for `network dns record-set ns create` (#9965)</span></span>

### <a name="rbac"></a><span data-ttu-id="15ad5-1358">RBAC</span><span class="sxs-lookup"><span data-stu-id="15ad5-1358">RBAC</span></span>

* <span data-ttu-id="15ad5-1359">Befehl `user update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1359">Added `user update` command</span></span>
* <span data-ttu-id="15ad5-1360">[VERALTET]`--upn-or-object-id` in benutzerbezogenen Befehlen als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-1360">[DEPRECATED] Deprecated `--upn-or-object-id` from user-related commands</span></span>
    * <span data-ttu-id="15ad5-1361">Verwenden Sie das Ersatzargument `--id`.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1361">Use replacement argument `--id`</span></span>
* <span data-ttu-id="15ad5-1362">Argument `--id` zu benutzerbezogenen Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1362">Added `--id` argument to user-related commands</span></span>

### <a name="sql"></a><span data-ttu-id="15ad5-1363">SQL</span><span class="sxs-lookup"><span data-stu-id="15ad5-1363">SQL</span></span>

* <span data-ttu-id="15ad5-1364">Verwaltungsbefehle für Schlüssel verwalteter Instanzen und TDE-Schutzvorrichtung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1364">Added management commands for managed instance keys and TDE protector</span></span>

### <a name="storage"></a><span data-ttu-id="15ad5-1365">Storage</span><span class="sxs-lookup"><span data-stu-id="15ad5-1365">Storage</span></span>

* <span data-ttu-id="15ad5-1366">Befehl `storage remove` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1366">Added `storage remove` command</span></span>
* <span data-ttu-id="15ad5-1367">Problem mit `storage blob update` behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-1367">Fixed an issue with `storage blob update`</span></span>

### <a name="vm"></a><span data-ttu-id="15ad5-1368">VM</span><span class="sxs-lookup"><span data-stu-id="15ad5-1368">VM</span></span>

* <span data-ttu-id="15ad5-1369">`list-skus` wurde geändert, um eine neuere API-Version für die Ausgabe von Zonendetails zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1369">Changed `list-skus` to use newer api-version to output zone details</span></span>
* <span data-ttu-id="15ad5-1370">Standardwert `--single-placement-group` für `vmss create` in `false` geändert</span><span class="sxs-lookup"><span data-stu-id="15ad5-1370">Changed default of `--single-placement-group` to `false` for `vmss create`</span></span>
* <span data-ttu-id="15ad5-1371">Möglichkeit zum Auswählen von ZRS-Speicher-SKUs für `[snapshot|disk] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1371">Added ability to select ZRS storage SKUs for `[snapshot|disk] create`</span></span>
* <span data-ttu-id="15ad5-1372">Neue Befehlsgruppe `vm host` zur Unterstützung dedizierter Hosts hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1372">Added new command group `vm host` to support dedicated hosts</span></span>
* <span data-ttu-id="15ad5-1373">Parameter `--host` und `--host-group` für `vm create` hinzugefügt, um den dedizierten VM-Host festzulegen</span><span class="sxs-lookup"><span data-stu-id="15ad5-1373">Added parameters `--host` and `--host-group` on `vm create` to set VM dedicated host</span></span>

## <a name="july-16-2019"></a><span data-ttu-id="15ad5-1374">16. Juli 2019</span><span class="sxs-lookup"><span data-stu-id="15ad5-1374">July 16, 2019</span></span>

<span data-ttu-id="15ad5-1375">Version 2.0.69</span><span class="sxs-lookup"><span data-stu-id="15ad5-1375">Version 2.0.69</span></span>

### <a name="appservice"></a><span data-ttu-id="15ad5-1376">AppService</span><span class="sxs-lookup"><span data-stu-id="15ad5-1376">Appservice</span></span>

* <span data-ttu-id="15ad5-1377">`webapp identity`-Befehle geändert, um eine korrekte Fehlermeldung zurückzugeben, wenn „ResourceGroupName“ oder der App-Name ungültig sind</span><span class="sxs-lookup"><span data-stu-id="15ad5-1377">Changed `webapp identity` commands to return a proper error message if ResourceGroupName or App name are invalid</span></span>
* <span data-ttu-id="15ad5-1378">`webapp list` korrigiert, sodass der korrekte Wert für „numberOfSites“ zurückgegeben wird, wenn „ResourceGroup“ nicht angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="15ad5-1378">Fixed `webapp list` to return the correct value for numberOfSites if no ResourceGroup was provided</span></span>
* <span data-ttu-id="15ad5-1379">Nebeneffekte von `appservice plan create` und `webapp create` behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-1379">Fixed side-effects of `appservice plan create` and `webapp create`</span></span>

### <a name="core"></a><span data-ttu-id="15ad5-1380">Core</span><span class="sxs-lookup"><span data-stu-id="15ad5-1380">Core</span></span>

* <span data-ttu-id="15ad5-1381">Problem behoben, aufgrund dessen `--subscription` angezeigt wurde, obwohl nicht anwendbar</span><span class="sxs-lookup"><span data-stu-id="15ad5-1381">Fixed issue where `--subscription` would appear despite being not applicable</span></span>

### <a name="batch"></a><span data-ttu-id="15ad5-1382">Batch</span><span class="sxs-lookup"><span data-stu-id="15ad5-1382">Batch</span></span>

* <span data-ttu-id="15ad5-1383">[BREAKING CHANGE]`batch pool node-agent-skus list` durch `batch pool supported-images list` ersetzt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1383">[BREAKING CHANGE] Replaced `batch pool node-agent-skus list` with `batch pool supported-images list`</span></span>
* <span data-ttu-id="15ad5-1384">Unterstützung für Sicherheitsregeln hinzugefügt, die den Netzwerkzugriff auf einen Pool basierend auf dem Quellport des Datenverkehrs blockieren, wenn die Option `--json-file` von `batch pool create network` verwendet wird</span><span class="sxs-lookup"><span data-stu-id="15ad5-1384">Added support for security rules blocking network access to a pool based on the source port of the traffic when using the `--json-file` option of `batch pool create network`</span></span>
* <span data-ttu-id="15ad5-1385">Unterstützung für die Ausführung der Aufgabe im Arbeitsverzeichnis des Containers oder der Batch-Aufgabe hinzugefügt, wenn die Option `--json-file` von `batch task create` verwendet wird</span><span class="sxs-lookup"><span data-stu-id="15ad5-1385">Added support for executing the task in the container working directory or in the Batch task working directory when using the `--json-file` option of `batch task create`</span></span>
* <span data-ttu-id="15ad5-1386">Fehler in Option `--application-package-references` von `batch pool create` behoben, aufgrund dessen nur Standardeinstellungen möglich waren</span><span class="sxs-lookup"><span data-stu-id="15ad5-1386">Fixed error in `--application-package-references` option of `batch pool create` where it would only work with defaults</span></span>

### <a name="eventhubs"></a><span data-ttu-id="15ad5-1387">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="15ad5-1387">Eventhubs</span></span>

* <span data-ttu-id="15ad5-1388">Validierung für Parameter `--rights` von `authorizationrule`-Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1388">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="rdbms"></a><span data-ttu-id="15ad5-1389">RDBMS</span><span class="sxs-lookup"><span data-stu-id="15ad5-1389">RDBMS</span></span>

* <span data-ttu-id="15ad5-1390">Optionaler Parameter zum Angeben der Replikat-SKU für den Befehl zum Erstellen von Replikaten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1390">Added optional parameter to specify replica SKU for create replica command</span></span>
* <span data-ttu-id="15ad5-1391">Problem mit CI-Testfehler bei der Erstellung von MySQL-Replikaten behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-1391">Fixed the issue with CI test failure with creating MySQL replica</span></span>

### <a name="relay"></a><span data-ttu-id="15ad5-1392">Relay</span><span class="sxs-lookup"><span data-stu-id="15ad5-1392">Relay</span></span>

* <span data-ttu-id="15ad5-1393">Problem mit Hybridverbindung behoben, wenn die Client-Autorisierung deaktiviert ist [#8775](https://github.com/azure/azure-cli/issues/8775)</span><span class="sxs-lookup"><span data-stu-id="15ad5-1393">Fixed issue with hybrid connection when client authroization disabled [#8775](https://github.com/azure/azure-cli/issues/8775)</span></span>
* <span data-ttu-id="15ad5-1394">Parameter `--requires-transport-security` zu `relay wcfrelay create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1394">Added parameter `--requires-transport-security` to `relay wcfrelay create`</span></span>

### <a name="servicebus"></a><span data-ttu-id="15ad5-1395">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="15ad5-1395">Servicebus</span></span>

* <span data-ttu-id="15ad5-1396">Validierung für Parameter `--rights` von `authorizationrule`-Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1396">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="storage"></a><span data-ttu-id="15ad5-1397">Storage</span><span class="sxs-lookup"><span data-stu-id="15ad5-1397">Storage</span></span>

* <span data-ttu-id="15ad5-1398">AADDS für Files für Speicherkontoaktualisierung aktiviert</span><span class="sxs-lookup"><span data-stu-id="15ad5-1398">Enable Files AADDS for storage account update</span></span>
* <span data-ttu-id="15ad5-1399">Problem `storage blob service-properties update --set` behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-1399">Fixed issue `storage blob service-properties update --set`</span></span>

## <a name="july-2-2019"></a><span data-ttu-id="15ad5-1400">2\. Juli 2019</span><span class="sxs-lookup"><span data-stu-id="15ad5-1400">July 2, 2019</span></span>

<span data-ttu-id="15ad5-1401">Version 2.0.68</span><span class="sxs-lookup"><span data-stu-id="15ad5-1401">Version 2.0.68</span></span>

### <a name="core"></a><span data-ttu-id="15ad5-1402">Core</span><span class="sxs-lookup"><span data-stu-id="15ad5-1402">Core</span></span>

* <span data-ttu-id="15ad5-1403">Befehlsmodule sind jetzt in einer einzelnen verteilbaren Python-Komponente zusammengefasst.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1403">Command modules are now consolidated into a single Python distributable.</span></span> <span data-ttu-id="15ad5-1404">Die direkte Verwendung zahlreicher Pakete vom Typ `azure-cli-` in PyPI ist daher veraltet.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1404">This deprecates direct use of many `azure-cli-` packages on PyPI.</span></span>
  <span data-ttu-id="15ad5-1405">Dadurch sollte sich die Installationsgröße reduzieren. Darüber hinaus sollte es nur Benutzer betreffen, die eine direkte Installation über `pip` ausgeführt haben.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1405">This should reduce install size and only affect users who have directly installed via `pip`.</span></span>

### <a name="acr"></a><span data-ttu-id="15ad5-1406">ACR</span><span class="sxs-lookup"><span data-stu-id="15ad5-1406">ACR</span></span>

* <span data-ttu-id="15ad5-1407">Unterstützung für Trigger mit Timer zu Aufgabe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1407">Added support for Timer Triggers to Task</span></span>

### <a name="appservice"></a><span data-ttu-id="15ad5-1408">AppService</span><span class="sxs-lookup"><span data-stu-id="15ad5-1408">Appservice</span></span>

* <span data-ttu-id="15ad5-1409">`functionapp create` wurde so geändert, das Application Insights standardmäßig aktiviert wird.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1409">Changed `functionapp create` to enable application insights by default</span></span>
* <span data-ttu-id="15ad5-1410">[BREAKING CHANGE] Veralteter Befehl `functionapp devops-build` entfernt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1410">[BREAKING CHANGE] Removed deprecated `functionapp devops-build` command.</span></span>
  *  <span data-ttu-id="15ad5-1411">Verwenden Sie stattdessen den neuen Befehl `az functionapp devops-pipeline`.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1411">Use the new command `az functionapp devops-pipeline` instead</span></span>
* <span data-ttu-id="15ad5-1412">Unterstützung des Funktions-App-Plans für Linux-Verbrauch zu `functionapp deployment config-zip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1412">Added Linux Consumption function app plan support to `functionapp deployment config-zip`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="15ad5-1413">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="15ad5-1413">Cosmos DB</span></span>

* <span data-ttu-id="15ad5-1414">Unterstützung für das Deaktivieren von TTL hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1414">Added support for disabling TTL</span></span>

### <a name="dls"></a><span data-ttu-id="15ad5-1415">DLS</span><span class="sxs-lookup"><span data-stu-id="15ad5-1415">DLS</span></span>

* <span data-ttu-id="15ad5-1416">Aktualisierte ADLS-Version (0.0.45)</span><span class="sxs-lookup"><span data-stu-id="15ad5-1416">Updated ADLS version (0.0.45)</span></span>

### <a name="feedback"></a><span data-ttu-id="15ad5-1417">Feedback</span><span class="sxs-lookup"><span data-stu-id="15ad5-1417">Feedback</span></span>

* <span data-ttu-id="15ad5-1418">Wird ein fehlgeschlagener Erweiterungsbefehl gemeldet, versucht `az feedback` nun, über den Index die Projekt-/Repository-URL der Erweiterung im Browser zu öffnen.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1418">When reporting a failed extension command, `az feedback` now attempts to open the browser to the project/repo url of the extension from the index</span></span>

### <a name="hdinsight"></a><span data-ttu-id="15ad5-1419">HDInsight</span><span class="sxs-lookup"><span data-stu-id="15ad5-1419">HDInsight</span></span>

* <span data-ttu-id="15ad5-1420">[BREAKING CHANGE] Der Befehlsgruppenname `oms` wurde in `monitor` geändert.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1420">[BREAKING CHANGE] Changed `oms` command group name to `monitor`</span></span>
* <span data-ttu-id="15ad5-1421">[BREAKING CHANGE]`--http-password/-p` als erforderlicher Parameter festgelegt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1421">[BREAKING CHANGE] Made `--http-password/-p` a required parameter</span></span> 
* <span data-ttu-id="15ad5-1422">Vervollständigungen für `--cluster-admin-account` und `cluster-users-group-dns` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1422">Added completers for `--cluster-admin-account` and `cluster-users-group-dns` parameters completer</span></span> 
* <span data-ttu-id="15ad5-1423">Parameter `cluster-users-group-dns` so geändert, dass er erforderlich ist, wenn `—esp` vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="15ad5-1423">Changed `cluster-users-group-dns` parameter to be required when `—esp` is present</span></span>
* <span data-ttu-id="15ad5-1424">Timeout für alle vorhandenen automatischen Argumentvervollständigungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1424">Added a timeout for all existing argument auto-completers</span></span>
* <span data-ttu-id="15ad5-1425">Timeout für das Transformieren des Ressourcennamens in eine Ressourcen-ID hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1425">Added a timeout for transforming resource name to resource id</span></span>
* <span data-ttu-id="15ad5-1426">Die automatischen Vervollständigungen wurden so geändert, dass Ressourcen aus einer beliebigen Ressourcengruppe ausgewählt werden.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1426">Changed Auto-completers to select resources from any resource group.</span></span> <span data-ttu-id="15ad5-1427">Dabei kann es sich um eine andere Ressourcengruppe als die mit `-g` angegebene Gruppe handeln.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1427">It can be a different resource group than the one specified with `-g`</span></span>
* <span data-ttu-id="15ad5-1428">Unterstützung für die Parameter `--sub-domain-suffix` und `--disable_gateway_auth` im Befehl `hdinsight application create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1428">Added support for `--sub-domain-suffix` and `--disable_gateway_auth` parameters in the `hdinsight application create` command</span></span>

### <a name="managed-services"></a><span data-ttu-id="15ad5-1429">Verwaltete Dienste</span><span class="sxs-lookup"><span data-stu-id="15ad5-1429">Managed Services</span></span>

* <span data-ttu-id="15ad5-1430">Befehlsmodul für verwaltete Dienste als Vorschau eingeführt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1430">Introducing managed service command module in preview</span></span>

### <a name="profile"></a><span data-ttu-id="15ad5-1431">Profil</span><span class="sxs-lookup"><span data-stu-id="15ad5-1431">Profile</span></span>
* <span data-ttu-id="15ad5-1432">Argument `--subscription` für Abmeldebefehl unterdrückt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1432">Suppress `--subscription` argument for logout command</span></span>

### <a name="rbac"></a><span data-ttu-id="15ad5-1433">RBAC</span><span class="sxs-lookup"><span data-stu-id="15ad5-1433">RBAC</span></span>

* <span data-ttu-id="15ad5-1434">[BREAKING CHANGE] Argument `--password` für `create-for-rbac` entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1434">[BREAKING CHANGE] Removed `--password` argument for `create-for-rbac`</span></span>
* <span data-ttu-id="15ad5-1435">Parameter `--assignee-principal-type` zum Befehl `create` hinzugefügt, um zeitweilige Fehler zu vermeiden, die durch die Replikationswartezeit des AAD-Graph-Servers verursacht werden</span><span class="sxs-lookup"><span data-stu-id="15ad5-1435">Added `--assignee-principal-type` parameter to `create` command to avoid intermittent failures caused by AAD graph server replication latency</span></span>
* <span data-ttu-id="15ad5-1436">Absturz in `ad signed-in-user` beim Auflisten von in Besitz befindlichen Objekten behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-1436">Fixed a crash in `ad signed-in-user` when listing owned objects</span></span>
* <span data-ttu-id="15ad5-1437">Problem behoben, aufgrund dessen `ad sp` nicht die richtige Anwendung über einen Dienstprinzipal fand</span><span class="sxs-lookup"><span data-stu-id="15ad5-1437">Fixed issue where `ad sp` would not find the right application from a service principal</span></span>

### <a name="rdbms"></a><span data-ttu-id="15ad5-1438">RDBMS</span><span class="sxs-lookup"><span data-stu-id="15ad5-1438">RDBMS</span></span>

* <span data-ttu-id="15ad5-1439">Unterstützung für die Replikation für MariaDB hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1439">Added support for replication for MariaDB</span></span>

### <a name="sql"></a><span data-ttu-id="15ad5-1440">SQL</span><span class="sxs-lookup"><span data-stu-id="15ad5-1440">SQL</span></span>

* <span data-ttu-id="15ad5-1441">Zulässige Werte für `sql db create --sample-name` dokumentiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-1441">Documented allowed values for `sql db create --sample-name`</span></span>

### <a name="storage"></a><span data-ttu-id="15ad5-1442">Storage</span><span class="sxs-lookup"><span data-stu-id="15ad5-1442">Storage</span></span>

* <span data-ttu-id="15ad5-1443">Unterstützung von SAS-Token für die Benutzerdelegierung mit `--as-user` zu `storage blob generate-sas` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1443">Added user delegation SAS token support with `--as-user` to `storage blob generate-sas`</span></span> 
* <span data-ttu-id="15ad5-1444">Unterstützung von SAS-Token für die Benutzerdelegierung mit `--as-user` zu `storage container generate-sas` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1444">Added user delegation SAS token support with `--as-user` to `storage container generate-sas`</span></span> 

### <a name="vm"></a><span data-ttu-id="15ad5-1445">VM</span><span class="sxs-lookup"><span data-stu-id="15ad5-1445">VM</span></span>

* <span data-ttu-id="15ad5-1446">Fehler behoben, aufgrund dessen `vmss create` bei der Ausführung mit `--no-wait` eine Fehlermeldung zurückgab</span><span class="sxs-lookup"><span data-stu-id="15ad5-1446">Fixed bug where `vmss create` returns an error message when run with `--no-wait`</span></span>
* <span data-ttu-id="15ad5-1447">Die clientseitige Validierung für `vmss create --single-placement-group` wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1447">Removed client-side validation for `vmss create --single-placement-group`.</span></span> <span data-ttu-id="15ad5-1448">Es tritt kein Fehler auf, wenn `--single-placement-group` auf `true` und für `--instance-count` ein größerer Wert als 100 festgelegt wird oder wenn Verfügbarkeitszonen angegeben werden. Diese Validierung wird jedoch dem Computedienst überlassen.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1448">Does not fail if `--single-placement-group` is set to `true` and`--instance-count` is greater than 100 or availability zones are specified, but leaves this validation to the compute service</span></span>
* <span data-ttu-id="15ad5-1449">Problem behoben, aufgrund dessen bei der Verwendung von `--latest` für `[vm|vmss] extension image list` ein Fehler auftrat</span><span class="sxs-lookup"><span data-stu-id="15ad5-1449">Fixed bug where `[vm|vmss] extension image list` fails when used with `--latest`</span></span>


## <a name="june-18-2019"></a><span data-ttu-id="15ad5-1450">18. Juni 2019</span><span class="sxs-lookup"><span data-stu-id="15ad5-1450">June 18, 2019</span></span>

<span data-ttu-id="15ad5-1451">Version 2.0.67</span><span class="sxs-lookup"><span data-stu-id="15ad5-1451">Version 2.0.67</span></span>

### <a name="core"></a><span data-ttu-id="15ad5-1452">Core</span><span class="sxs-lookup"><span data-stu-id="15ad5-1452">Core</span></span>

<span data-ttu-id="15ad5-1453">In diesem Release wird das neue [Preview]-Tag eingeführt, um Kunden gegenüber deutlich zu machen, dass sich eine Befehlsgruppe, ein Befehl oder ein Argument in der Vorschauphase befindet.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1453">This release introduces a new [Preview] tag to more clearly communicate to customers when a command group, command or argument is in preview status.</span></span> <span data-ttu-id="15ad5-1454">Diese Information war zuvor im Hilfetext oder implizit durch die Versionsnummer des Befehlsmoduls angegeben.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1454">This was previously called out in help text or communicated implicitly by the command module version number.</span></span>
<span data-ttu-id="15ad5-1455">Die Befehlszeilenschnittstelle wird künftig Versionsnummern für einzelne Pakete entfernen.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1455">The CLI will be removing version numbers for individual packages in the future.</span></span> <span data-ttu-id="15ad5-1456">Wenn sich ein Befehl in der Vorschauphase befindet, gilt dies auch für alle seine Argumente.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1456">If a command is in preview, all of its arguments are as well.</span></span> <span data-ttu-id="15ad5-1457">Wenn eine Befehlsgruppe als Vorschau gekennzeichnet ist, befinden sich auch alle Befehle und Argumente in der Vorschauphase.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1457">If a command group is labeled as being in preview, then all commands and arguments are considered to be in preview as well.</span></span>

<span data-ttu-id="15ad5-1458">Infolge dieser Änderung befinden sich in diesem Release verschiedene Befehlsgruppen anscheinend „plötzlich“ in der Vorschauphase.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1458">As a result of this change, several command groups may seem to "suddenly" appear to be in a preview status with this release.</span></span> <span data-ttu-id="15ad5-1459">Tatsächlich ist es jedoch so, dass sich die meisten Pakete in der Vorschauphase befanden, in diesem Release jedoch als allgemein verfügbar gelten.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1459">What actually happened is that most packages were in a preview status, but are being deemed GA with this release</span></span>

### <a name="acr"></a><span data-ttu-id="15ad5-1460">ACR</span><span class="sxs-lookup"><span data-stu-id="15ad5-1460">ACR</span></span>
* <span data-ttu-id="15ad5-1461">Befehl „acr check-health“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1461">Added 'acr check-health' command</span></span>
* <span data-ttu-id="15ad5-1462">Verbesserte Fehlerbehandlung für AAD-Token und für das Abrufen externer Befehle</span><span class="sxs-lookup"><span data-stu-id="15ad5-1462">Improved error handling for AAD tokens and for retrieving external commands</span></span>

### <a name="acs"></a><span data-ttu-id="15ad5-1463">ACS</span><span class="sxs-lookup"><span data-stu-id="15ad5-1463">ACS</span></span>
* <span data-ttu-id="15ad5-1464">Veraltete ACS-Befehle werden jetzt in der Hilfeansicht ausgeblendet.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1464">Deprecated ACS commands are now hidden from help view</span></span>

### <a name="ams"></a><span data-ttu-id="15ad5-1465">AMS</span><span class="sxs-lookup"><span data-stu-id="15ad5-1465">AMS</span></span>
* <span data-ttu-id="15ad5-1466">[BREAKING CHANGE] Änderung, damit ISO 8601-Zeitzeichenfolgen für „archive-window-length“ und „key-frame-interval-duration“ zurückgegeben werden</span><span class="sxs-lookup"><span data-stu-id="15ad5-1466">[BREAKING CHANGE] Changed to return ISO 8601 time strings for archive-window-length and key-frame-interval-duration</span></span>

### <a name="appservice"></a><span data-ttu-id="15ad5-1467">AppService</span><span class="sxs-lookup"><span data-stu-id="15ad5-1467">AppService</span></span>
* <span data-ttu-id="15ad5-1468">Standortbasiertes Routing für `webapp deleted list` und `webapp deleted restore` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1468">Added location based routing for `webapp deleted list` and `webapp deleted restore`</span></span>
* <span data-ttu-id="15ad5-1469">Problem behoben, aufgrund dessen in Azure Cloud Shell nicht auf die von einer Web-App protokollierte Ziel-URL („Sie können die App starten unter...“) geklickt werden konnte</span><span class="sxs-lookup"><span data-stu-id="15ad5-1469">Fixed issue where webapp up logged target URL ("You can launch the app at...") was not clickable in Azure Cloud Shell</span></span>
* <span data-ttu-id="15ad5-1470">Problem behoben, aufgrund dessen beim Erstellen von Apps bei einigen SKUs ein AlwaysOn-Fehler auftrat</span><span class="sxs-lookup"><span data-stu-id="15ad5-1470">Fixed an issue where creating apps with the some SKUs was failing with an AlwaysOn error</span></span>
* <span data-ttu-id="15ad5-1471">Vorabüberprüfung zu `[appservice|webapp] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1471">Added pre-validation to `[appservice|webapp] create`</span></span>
* <span data-ttu-id="15ad5-1472">`[webapp|functionapp] traffic-routing` korrigiert, damit der richtige actionHostName-Wert verwendet wird</span><span class="sxs-lookup"><span data-stu-id="15ad5-1472">Fixed `[webapp|functionapp] traffic-routing` to use the correct actionHostName</span></span>
* <span data-ttu-id="15ad5-1473">Slotunterstützung zu `functionapp`-Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1473">Added slot support to `functionapp` commands</span></span>

### <a name="batch"></a><span data-ttu-id="15ad5-1474">Batch</span><span class="sxs-lookup"><span data-stu-id="15ad5-1474">Batch</span></span>
* <span data-ttu-id="15ad5-1475">AAD-Authentifizierungsregression korrigiert, die von übermäßiger Berichterstellung für Authentifizierung mit gemeinsam verwendetem Schlüssel verursacht wurde</span><span class="sxs-lookup"><span data-stu-id="15ad5-1475">Fixed AAD auth regression caused by over-aggressive error reporting for Shared Key Auth</span></span>

### <a name="batchai"></a><span data-ttu-id="15ad5-1476">Batch AI</span><span class="sxs-lookup"><span data-stu-id="15ad5-1476">BatchAI</span></span>
* <span data-ttu-id="15ad5-1477">BatchAI-Befehle sind jetzt veraltet und ausgeblendet.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1477">BatchAI commands are now deprecated and hidden</span></span>

### <a name="botservice"></a><span data-ttu-id="15ad5-1478">BotService</span><span class="sxs-lookup"><span data-stu-id="15ad5-1478">BotService</span></span>
* <span data-ttu-id="15ad5-1479">Für Befehle, die Version 3 des SDK unterstützen, wurden die Warnmeldungen „Support eingestellt“/„Wartungsmodus“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1479">Added "discontinued support"/"maintenance mode" warning messages for commands that support the v3 SDK</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="15ad5-1480">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="15ad5-1480">CosmosDB</span></span>
* <span data-ttu-id="15ad5-1481">[VERALTET] Der Befehl `cosmosdb list-keys` wurde als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1481">[DEPRECATED] Deprecated the `cosmosdb list-keys` command</span></span>
* <span data-ttu-id="15ad5-1482">Befehl `cosmosdb keys list` hinzugefügt, er ersetzt `cosmosdb list-keys`.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1482">Added the `cosmosdb keys list` command - replaces `cosmosdb list-keys`</span></span>
* <span data-ttu-id="15ad5-1483">`cosmsodb create/update`: Neues Format für „--location“ hinzugefügt, um das Festlegen der Eigenschaft „isZoneRedundant“ zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="15ad5-1483">`cosmsodb create/update`: Added new format for --location to allow setting "isZoneRedundant" property.</span></span> <span data-ttu-id="15ad5-1484">Das alte Format wurde als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1484">Deprecated old format</span></span>

### <a name="eventgrid"></a><span data-ttu-id="15ad5-1485">EventGrid</span><span class="sxs-lookup"><span data-stu-id="15ad5-1485">EventGrid</span></span>
* <span data-ttu-id="15ad5-1486">`eventgrid domain`-Befehle für CRUD-Vorgänge für Domänen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1486">Added `eventgrid domain` commands for domain CRUD operations</span></span>
* <span data-ttu-id="15ad5-1487">`eventgrid domain topic`-Befehle für CRUD-Vorgänge für Domänenthemen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1487">Added `eventgrid domain topic` commands for domain topics CRUD operations</span></span>
* <span data-ttu-id="15ad5-1488">Argument `--odata-query` zu `eventgrid [topic|event-subscription] list` zum Filtern der Ergebnisse mithilfe von OData-Syntax hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1488">Added `--odata-query` argument to `eventgrid [topic|event-subscription] list` for filtering results using OData syntax</span></span>
* <span data-ttu-id="15ad5-1489">`event-subscription create/update`: „servicebusqueue“ als neue Werte für den Parameter `--endpoint-type` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1489">`event-subscription create/update`: Added servicebusqueue as new values for the `--endpoint-type` parameter</span></span>
* <span data-ttu-id="15ad5-1490">[BREAKING CHANGE] Unterstützung für `--included-event-types All` mit `eventgrid event-subscription [create|update]` entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1490">[BREAKING CHANGE] Removed support for `--included-event-types All` with `eventgrid event-subscription [create|update]`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="15ad5-1491">HDInsight</span><span class="sxs-lookup"><span data-stu-id="15ad5-1491">HDInsight</span></span>
* <span data-ttu-id="15ad5-1492">Unterstützung für den Parameter `--ssh-public-key` im Befehl vom Typ `hdinsight create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1492">Added support for `--ssh-public-key` parameter in `hdinsight create` command</span></span>

### <a name="iot"></a><span data-ttu-id="15ad5-1493">IoT</span><span class="sxs-lookup"><span data-stu-id="15ad5-1493">IoT</span></span>
* <span data-ttu-id="15ad5-1494">Unterstützung für das erneute Generieren von Autorisierungsrichtlinienschlüsseln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1494">Added support to regenerate authorization policy keys</span></span>
* <span data-ttu-id="15ad5-1495">SDK und Unterstützung für den Bereitstellungsdienst des DigitalTwin-Repositorys hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1495">Added SDK and support for DigitalTwin Repository Provisioning Service</span></span>

### <a name="network"></a><span data-ttu-id="15ad5-1496">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="15ad5-1496">Network</span></span>
* <span data-ttu-id="15ad5-1497">Zonenunterstützung für NAT Gateway hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1497">Added Zone support for Nat Gateway</span></span>
* <span data-ttu-id="15ad5-1498">Befehl `network list-service-tags` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1498">Added command `network list-service-tags`</span></span>
* <span data-ttu-id="15ad5-1499">Problem mit `dns zone import` behoben, aufgrund dessen Benutzer keine A-Platzhaltereinträge importieren konnten</span><span class="sxs-lookup"><span data-stu-id="15ad5-1499">Fixed issue with `dns zone import` where users could not import wildcard A records</span></span>
* <span data-ttu-id="15ad5-1500">Problem mit `watcher flow-log configure` behoben, aufgrund dessen die Flowprotokollierung in bestimmten Regionen nicht aktiviert werden konnte</span><span class="sxs-lookup"><span data-stu-id="15ad5-1500">Fixed issue with `watcher flow-log configure` where flow logging could not be enabled in certain regions</span></span>

### <a name="resource"></a><span data-ttu-id="15ad5-1501">Resource</span><span class="sxs-lookup"><span data-stu-id="15ad5-1501">Resource</span></span>
* <span data-ttu-id="15ad5-1502">Befehl `az rest` zum Ausführen von REST-Aufrufen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1502">Added `az rest` command for making REST calls</span></span>
* <span data-ttu-id="15ad5-1503">Fehler behoben, der bei Verwendung von `policy assignment list` mit `--scope` auf Ressourcengruppen- oder Abonnementebene auftrat</span><span class="sxs-lookup"><span data-stu-id="15ad5-1503">Fixed error when using `policy assignment list` with a resource group or subscription level `--scope`</span></span>

### <a name="servicebus"></a><span data-ttu-id="15ad5-1504">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="15ad5-1504">ServiceBus</span></span>
* <span data-ttu-id="15ad5-1505">Problem mit `servicebus topic create --max-size` behoben [Nr. 9319](https://github.com/azure/azure-cli/issues/9319)</span><span class="sxs-lookup"><span data-stu-id="15ad5-1505">Fixed issue with `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span></span>

### <a name="sql"></a><span data-ttu-id="15ad5-1506">SQL</span><span class="sxs-lookup"><span data-stu-id="15ad5-1506">SQL</span></span>
* <span data-ttu-id="15ad5-1507">`--location` wurde geändert und ist nun für `sql [server|mi] create` optional. Ohne Angabe wird der Ressourcengruppenstandort verwendet.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1507">Changed `--location` to be optional for `sql [server|mi] create` - uses resource group location if not specified</span></span>
* <span data-ttu-id="15ad5-1508">Der Fehler, dass das Objekt „NoneType“ nicht wiederholbar ist, wurde für `sql db list-editions --available` behoben.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1508">Fixed "'NoneType' object is not iterable" error for `sql db list-editions --available`</span></span>

### <a name="sqlvm"></a><span data-ttu-id="15ad5-1509">SQLVm</span><span class="sxs-lookup"><span data-stu-id="15ad5-1509">SQLVm</span></span>
* <span data-ttu-id="15ad5-1510">[WICHTIGE ÄNDERUNG] `sql vm create` wurde geändert und erfordert nun den Parameter `--license-type`.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1510">[BREAKING CHNAGE] Changed `sql vm create` to require `--license-type` parameter</span></span>
* <span data-ttu-id="15ad5-1511">Änderung, um beim Erstellen oder Aktualisieren einer SQL-VM das Festlegen der SQL-Image-SKU zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="15ad5-1511">Changed to allow setting SQL image SKU when creating or updating a sql vm</span></span>

### <a name="storage"></a><span data-ttu-id="15ad5-1512">Storage</span><span class="sxs-lookup"><span data-stu-id="15ad5-1512">Storage</span></span>
* <span data-ttu-id="15ad5-1513">Problem mit fehlendem Kontoschlüssel für `storage container generate-sas` behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-1513">Fixed issue with missing account key for `storage container generate-sas`</span></span>
* <span data-ttu-id="15ad5-1514">Problem mit `storage blob sync` unter Linux behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-1514">Fixed issue with `storage blob sync` on Linux</span></span>

### <a name="vm"></a><span data-ttu-id="15ad5-1515">VM</span><span class="sxs-lookup"><span data-stu-id="15ad5-1515">VM</span></span>
* <span data-ttu-id="15ad5-1516">[VORSCHAU] Befehle vom Typ `vm image template` zum Erstellen von VM-Images hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1516">[PREVIEW] Added `vm image template` commands to build VM images</span></span>

## <a name="june-4-2019"></a><span data-ttu-id="15ad5-1517">4\. Juni 2019</span><span class="sxs-lookup"><span data-stu-id="15ad5-1517">June 4, 2019</span></span>

<span data-ttu-id="15ad5-1518">Version 2.0.66</span><span class="sxs-lookup"><span data-stu-id="15ad5-1518">Version 2.0.66</span></span>

### <a name="core"></a><span data-ttu-id="15ad5-1519">Core</span><span class="sxs-lookup"><span data-stu-id="15ad5-1519">Core</span></span>
* <span data-ttu-id="15ad5-1520">Fehler behoben, aufgrund dessen bei Befehlen ein Fehler auftrat, wenn `--output yaml` mit `--query` verwendet wurde</span><span class="sxs-lookup"><span data-stu-id="15ad5-1520">Fixed bug where commands fail if `--output yaml` is used with `--query`</span></span>

### <a name="acr"></a><span data-ttu-id="15ad5-1521">ACR</span><span class="sxs-lookup"><span data-stu-id="15ad5-1521">ACR</span></span>
* <span data-ttu-id="15ad5-1522">Befehlsgruppe „acr pack“ zum Erstellen von Aufgaben zur Schnellerstellung mit Buildpacks hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1522">Added 'acr pack' command group for creating quick build Tasks using Buildpacks.</span></span>

### <a name="acs"></a><span data-ttu-id="15ad5-1523">ACS</span><span class="sxs-lookup"><span data-stu-id="15ad5-1523">ACS</span></span>
* <span data-ttu-id="15ad5-1524">Zulassen der Aktivierung/Deaktivierung des AKS-Add-Ons für das Kube-Dashboard</span><span class="sxs-lookup"><span data-stu-id="15ad5-1524">Allow enabling/disabling AKS kube-dashboard addon</span></span>
* <span data-ttu-id="15ad5-1525">Ausgeben einer benutzerfreundlichen Nachricht, wenn das Abonnement nicht in der Whitelist zur Verwendung von Azure Red Hat OpenShift enthalten ist</span><span class="sxs-lookup"><span data-stu-id="15ad5-1525">Print a friendly message when the subscription is not whitelisted to use Azure Red Hat OpenShift</span></span>

### <a name="batch"></a><span data-ttu-id="15ad5-1526">Batch</span><span class="sxs-lookup"><span data-stu-id="15ad5-1526">Batch</span></span>
* <span data-ttu-id="15ad5-1527">Bessere Fehlerbehandlung, wenn der Benutzer nicht bei einem Konto angemeldet ist \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span><span class="sxs-lookup"><span data-stu-id="15ad5-1527">Improved error handling when not logged in to an account \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span></span>

### <a name="iot"></a><span data-ttu-id="15ad5-1528">IoT</span><span class="sxs-lookup"><span data-stu-id="15ad5-1528">IoT</span></span>
* <span data-ttu-id="15ad5-1529">Unterstützung für manuelles Failover hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1529">Added support for manual failover</span></span>

### <a name="network"></a><span data-ttu-id="15ad5-1530">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="15ad5-1530">Network</span></span>
* <span data-ttu-id="15ad5-1531">Befehle vom Typ `network application-gateway waf-policy` hinzugefügt, um benutzerdefinierte WAF-Regeln zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="15ad5-1531">Added `network application-gateway waf-policy` commands to support custom WAF rules.</span></span>
* <span data-ttu-id="15ad5-1532">Argumente `--waf-policy` und `--max-capacity` zu `network application-gateway [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1532">Added `--waf-policy` and `--max-capacity` arguments to `network application-gateway [create|update]`</span></span> 

### <a name="resource"></a><span data-ttu-id="15ad5-1533">Resource</span><span class="sxs-lookup"><span data-stu-id="15ad5-1533">Resource</span></span>
* <span data-ttu-id="15ad5-1534">Verbesserte Fehlermeldungen aus `deployment create`, wenn TTY nicht verfügbar ist</span><span class="sxs-lookup"><span data-stu-id="15ad5-1534">Improved error message from `deployment create` when there is no TTY available</span></span>

### <a name="role"></a><span data-ttu-id="15ad5-1535">Role</span><span class="sxs-lookup"><span data-stu-id="15ad5-1535">Role</span></span>
* <span data-ttu-id="15ad5-1536">Hilfetext aktualisiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-1536">Updated help text.</span></span>

### <a name="compute"></a><span data-ttu-id="15ad5-1537">Compute</span><span class="sxs-lookup"><span data-stu-id="15ad5-1537">Compute</span></span>
* <span data-ttu-id="15ad5-1538">Unterstützung zu `vm create` für virtuelle Computer aus einem verwalteten Image mit Datenträger-LUNs hinzugefügt, die nicht bei 0 beginnen oder die Nummern überspringen</span><span class="sxs-lookup"><span data-stu-id="15ad5-1538">Added support to `vm create` for VMs from a managed image with data-disk luns that do not start from 0 or that skip numbers</span></span>

## <a name="may-21-2019"></a><span data-ttu-id="15ad5-1539">21. Mai 2019</span><span class="sxs-lookup"><span data-stu-id="15ad5-1539">May 21, 2019</span></span>

<span data-ttu-id="15ad5-1540">Version 2.0.65</span><span class="sxs-lookup"><span data-stu-id="15ad5-1540">Version 2.0.65</span></span>

### <a name="core"></a><span data-ttu-id="15ad5-1541">Core</span><span class="sxs-lookup"><span data-stu-id="15ad5-1541">Core</span></span>
* <span data-ttu-id="15ad5-1542">Besseres Feedback für Authentifizierungsfehler hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1542">Added better feedback for authentication errors</span></span>
* <span data-ttu-id="15ad5-1543">Problem behoben, aufgrund dessen die CLI Erweiterungen lädt, die nicht mit der Core-Version kompatibel waren</span><span class="sxs-lookup"><span data-stu-id="15ad5-1543">Fixed issue where the CLI would load extensions that were not compatible with its core version</span></span>
* <span data-ttu-id="15ad5-1544">Problem beim Starten behoben, wenn `clouds.config` beschädigt ist</span><span class="sxs-lookup"><span data-stu-id="15ad5-1544">Fixed issue with launching when `clouds.config` is corrupted</span></span>

### <a name="acr"></a><span data-ttu-id="15ad5-1545">ACR</span><span class="sxs-lookup"><span data-stu-id="15ad5-1545">ACR</span></span>
* <span data-ttu-id="15ad5-1546">Unterstützung für verwaltete Identitäten zu Aufgaben hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1546">Added support for Managed Identities to Tasks</span></span>

### <a name="acs"></a><span data-ttu-id="15ad5-1547">ACS</span><span class="sxs-lookup"><span data-stu-id="15ad5-1547">ACS</span></span>
* <span data-ttu-id="15ad5-1548">`openshift create`-Befehl bei der Verwendung mit dem AAD-Kundenclient korrigiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-1548">Fixed `openshift create` command when used with customer AAD client</span></span>

### <a name="appservice"></a><span data-ttu-id="15ad5-1549">AppService</span><span class="sxs-lookup"><span data-stu-id="15ad5-1549">AppService</span></span>
* <span data-ttu-id="15ad5-1550">[VERALTET] Befehl `functionapp devops-build` als veraltet gekennzeichnet – wird in der nächsten Version entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1550">[DEPRECATED] Deprecated `functionapp devops-build` command - will be removed in next release</span></span>
* <span data-ttu-id="15ad5-1551">`functionapp devops-pipeline` geändert, um das Buildprotokoll von Azure DevOps im ausführlichen Modus abzurufen</span><span class="sxs-lookup"><span data-stu-id="15ad5-1551">Changed `functionapp devops-pipeline` to fetch build log from Azure DevOps in verbose mode</span></span>
* <span data-ttu-id="15ad5-1552">[BREAKING CHANGE] Flag `--use_local_settings` aus dem Befehl `functionapp devops-pipeline` entfernt – kein Vorgang wurde ausgeführt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1552">[BREAKING CHANGE] Removed `--use_local_settings` flag from `functionapp devops-pipeline` command - was a no-op</span></span>
* <span data-ttu-id="15ad5-1553">`webapp up` geändert, sodass die JSON-Ausgabe zurückgegeben wird, wenn `--logs` nicht verwendet wird</span><span class="sxs-lookup"><span data-stu-id="15ad5-1553">Changed `webapp up` to return JSON output if `--logs` is not used</span></span>
* <span data-ttu-id="15ad5-1554">Unterstützung hinzugefügt zum Schreiben von Standardressourcen in die lokale Konfiguration für `webapp up`</span><span class="sxs-lookup"><span data-stu-id="15ad5-1554">Added support for writing default resources to local config for `webapp up`</span></span>
* <span data-ttu-id="15ad5-1555">Unterstützung zu `webapp up` hinzugefügt für die erneute Bereitstellung einer App ohne Verwendung des `--location`-Arguments</span><span class="sxs-lookup"><span data-stu-id="15ad5-1555">Added support to `webapp up` for redeploying an app without using the `--location` argument</span></span>
* <span data-ttu-id="15ad5-1556">Problem behoben, bei dem für die ASP-Erstellung der Linux-SKU „Free“ der SKU-Wert „Free“ nicht funktioniert hat</span><span class="sxs-lookup"><span data-stu-id="15ad5-1556">Fixed an issue where for Linux Free SKU ASP creation use Free as SKU value was not working</span></span>

### <a name="botservice"></a><span data-ttu-id="15ad5-1557">BotService</span><span class="sxs-lookup"><span data-stu-id="15ad5-1557">BotService</span></span>
* <span data-ttu-id="15ad5-1558">Geändert, sodass Groß-/Kleinschreibung für `--lang`-Parameter für Befehle zulässig ist</span><span class="sxs-lookup"><span data-stu-id="15ad5-1558">Changed to allow all casing for `--lang` parameters for commands</span></span>
* <span data-ttu-id="15ad5-1559">Beschreibung für das Befehlsmodul aktualisiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-1559">Updated description for command module</span></span>

### <a name="consumption"></a><span data-ttu-id="15ad5-1560">Nutzung</span><span class="sxs-lookup"><span data-stu-id="15ad5-1560">Consumption</span></span>
* <span data-ttu-id="15ad5-1561">Fehlende erforderliche Parameter bei der Ausführung von `consumption usage list --billing-period-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1561">Added missing required parameter when running `consumption usage list --billing-period-name`</span></span>

### <a name="iot"></a><span data-ttu-id="15ad5-1562">IoT</span><span class="sxs-lookup"><span data-stu-id="15ad5-1562">IoT</span></span>
* <span data-ttu-id="15ad5-1563">Unterstützung für das Auflisten aller Schlüssel hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1563">Added support to list all keys</span></span>

### <a name="network"></a><span data-ttu-id="15ad5-1564">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="15ad5-1564">Network</span></span>
* [BREAKING CHANGE]: Removed `network interface-endpoints` command group - use `network private-endpoints` 
* <span data-ttu-id="15ad5-1566">`--nat-gateway`-Argument zu `network vnet subnet [create|update]` für das Anfügen an ein NAT-Gateway hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1566">Added `--nat-gateway` argument to `network vnet subnet [create|update]` for attaching to a NAT gateway</span></span>
* <span data-ttu-id="15ad5-1567">Problem mit `dns zone import` behoben, aufgrund dessen Eintragsnamen keinem Datensatztyp entsprochen haben</span><span class="sxs-lookup"><span data-stu-id="15ad5-1567">Fixed issue with `dns zone import` where record names could not match a record type</span></span>

### <a name="rdbms"></a><span data-ttu-id="15ad5-1568">RDBMS</span><span class="sxs-lookup"><span data-stu-id="15ad5-1568">RDBMS</span></span>
* <span data-ttu-id="15ad5-1569">Postgres- und MySLQ-Unterstützung für die Georeplikation hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1569">Added postgres and mysql support for geo replication</span></span>

### <a name="rbac"></a><span data-ttu-id="15ad5-1570">RBAC</span><span class="sxs-lookup"><span data-stu-id="15ad5-1570">RBAC</span></span>
* <span data-ttu-id="15ad5-1571">Unterstützung für den Verwaltungsgruppenumfang zu `role assignment` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1571">Added support for management group scope to `role assignment`</span></span>

### <a name="storage"></a><span data-ttu-id="15ad5-1572">Storage</span><span class="sxs-lookup"><span data-stu-id="15ad5-1572">Storage</span></span>
* <span data-ttu-id="15ad5-1573">`storage blob sync`: Synchronisierungsbefehl für Speicherblob hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1573">`storage blob sync`: add sync command for storage blob</span></span>

### <a name="compute"></a><span data-ttu-id="15ad5-1574">Compute</span><span class="sxs-lookup"><span data-stu-id="15ad5-1574">Compute</span></span>
* <span data-ttu-id="15ad5-1575">`--computer-name` zu `vm create` zum Festlegen des Computernamens eines virtuellen Computers hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1575">Added `--computer-name` to `vm create` for setting a VM's computer name</span></span>
* <span data-ttu-id="15ad5-1576">`--ssh-key-value` umbenannt in `--ssh-key-values` für `[vm|vmss] create`: Jetzt können mehrere öffentliche SSH-Schlüsselwerte oder -pfade akzeptiert werden.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1576">Renamed `--ssh-key-value` renamed to `--ssh-key-values` for `[vm|vmss] create` - can now accept multiple ssh public key values or paths</span></span>
  * <span data-ttu-id="15ad5-1577">__Hinweis__: Dies ist **kein** Breaking Change: `--ssh-key-value` wird korrekt analysiert, da nur eine Übereinstimmung mit `--ssh-key-values` besteht.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1577">__Note__: This is **not** a breaking change - `--ssh-key-value` will be parsed correctly as it matches only `--ssh-key-values`</span></span>
* <span data-ttu-id="15ad5-1578">`--type`-Argument von `ppg create` in optionales Argument geändert</span><span class="sxs-lookup"><span data-stu-id="15ad5-1578">Changed the `--type` argument of `ppg create` to be optional</span></span>

## <a name="may-6-2019"></a><span data-ttu-id="15ad5-1579">6\. Mai 2019</span><span class="sxs-lookup"><span data-stu-id="15ad5-1579">May 6, 2019</span></span>

<span data-ttu-id="15ad5-1580">Version 2.0.64</span><span class="sxs-lookup"><span data-stu-id="15ad5-1580">Version 2.0.64</span></span>

### <a name="acs"></a><span data-ttu-id="15ad5-1581">ACS</span><span class="sxs-lookup"><span data-stu-id="15ad5-1581">ACS</span></span>
* <span data-ttu-id="15ad5-1582">[BREAKING CHANGE] Flag `--fqdn` aus den `openshift`-Befehlen entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1582">[BREAKING CHANGE] Removed `--fqdn` flag on `openshift` commands</span></span>
* <span data-ttu-id="15ad5-1583">Geändert, sodass die allgemein verfügbare Azure Red Hat Openshift-API-Version verwendet wird</span><span class="sxs-lookup"><span data-stu-id="15ad5-1583">Changed to use Azure Red Hat Openshift GA API Version</span></span>
* <span data-ttu-id="15ad5-1584">Flag `customer-admin-group-id` wurde zu `openshift create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1584">Added `customer-admin-group-id` flag to `openshift create`</span></span>
* <span data-ttu-id="15ad5-1585">[ALLGEMEIN VERFÜGBAR] `(PREVIEW)` aus der `aks create`-Option `--network-policy` entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1585">[GA] Removed `(PREVIEW)` from `aks create` option `--network-policy`</span></span>

### <a name="appservice"></a><span data-ttu-id="15ad5-1586">AppService</span><span class="sxs-lookup"><span data-stu-id="15ad5-1586">Appservice</span></span>
* <span data-ttu-id="15ad5-1587">[VERALTET] Befehl `functionapp devops-build` als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="15ad5-1587">[DEPRECATED] Deprecated `functionapp devops-build` command</span></span>
  * <span data-ttu-id="15ad5-1588">Umbenannt in `functionapp devops-pipeline`</span><span class="sxs-lookup"><span data-stu-id="15ad5-1588">Renamed to `functionapp devops-pipeline`</span></span>
* <span data-ttu-id="15ad5-1589">Fehler beim Abrufen des richtigen Benutzernamens für Cloud Shell behoben, der einen Fehler von `webapp up` verursachte</span><span class="sxs-lookup"><span data-stu-id="15ad5-1589">Fixed getting the correct username for cloudshell which was causing `webapp up` to fail</span></span>
* <span data-ttu-id="15ad5-1590">Dokumentation von `appservice plan --sku` mit den unterstützten App Service-Plänen aktualisiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-1590">Updated `appservice plan --sku` documentation updated to reflect the supported appserviceplans</span></span>
* <span data-ttu-id="15ad5-1591">Optionale Argumente für Ressourcengruppe und Plan zu `webapp up` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1591">Added optional arguments for resource group and plan to `webapp up`</span></span>
* <span data-ttu-id="15ad5-1592">Unterstützung zur Berücksichtigung der Umgebungsvariablen `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` zu `webapp ssh` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1592">Added support to `webapp ssh` to respect `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>
* <span data-ttu-id="15ad5-1593">Unterstützung für `appserviceplan create` für die kostenlose Linux-SKU hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1593">Added `appserviceplan create` support for Linux Free SKU</span></span>
* <span data-ttu-id="15ad5-1594">`webapp up` geändert, um nach dem Festlegen der App-Einstellung `SCM_DO_BUILD_DURING_DEPLOYMENT=true` zum Verarbeiten des Kudu-Kaltstarts für 30 Sekunden in den Energiesparmodus zu wechseln</span><span class="sxs-lookup"><span data-stu-id="15ad5-1594">Changed `webapp up` to have a 30s sleep after setting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` appsetting to handle kudu cold start</span></span>
* <span data-ttu-id="15ad5-1595">Unterstützung für die `powershell`-Runtime zu `functionapp create` unter Windows hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1595">Added support for `powershell` runtime to `functionapp create` on Windows</span></span>
* <span data-ttu-id="15ad5-1596">Befehl `create-remote-connection` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1596">Added `create-remote-connection` command</span></span>

### <a name="batch"></a><span data-ttu-id="15ad5-1597">Batch</span><span class="sxs-lookup"><span data-stu-id="15ad5-1597">Batch</span></span>
* <span data-ttu-id="15ad5-1598">Fehler im Validierungssteuerelement für `--application-package-references`-Optionen korrigiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-1598">Fixed bug in validator for `--application-package-references` options</span></span>

### <a name="botservice"></a><span data-ttu-id="15ad5-1599">Botservice</span><span class="sxs-lookup"><span data-stu-id="15ad5-1599">Botservice</span></span>
* <span data-ttu-id="15ad5-1600">[BREAKING CHANGE]`bot create -v v4 -k webapp` geändert, sodass standardmäßig eine leerer Web-App-Bot erstellt wird (d. h. kein Bot wird in App Service bereitgestellt)</span><span class="sxs-lookup"><span data-stu-id="15ad5-1600">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to create an empty Web App Bot by default (i.e. no bot is deployed to the App Service)</span></span>
* <span data-ttu-id="15ad5-1601">`--echo`-Flag zu `bot create` hinzugefügt, sodass das alte Verhalten mit `-v v4` verwendet wird</span><span class="sxs-lookup"><span data-stu-id="15ad5-1601">Added `--echo` flag to `bot create` to use the old behavior with `-v v4`</span></span>
* <span data-ttu-id="15ad5-1602">[BREAKING CHANGE] Standardwert von `--version` in `v4` geändert</span><span class="sxs-lookup"><span data-stu-id="15ad5-1602">[BREAKING CHANGE] Changed the default value of  `--version` to `v4`</span></span>
  * <span data-ttu-id="15ad5-1603">__HINWEIS:__ `bot prepare-publish` verwendet weiterhin den alten Standard.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1603">__NOTE:__ `bot prepare-publish` still uses the its old default</span></span>
* <span data-ttu-id="15ad5-1604">[BREAKING CHANGE]`--lang` geändert, sodass der Standard nicht mehr `Csharp` ist.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1604">[BREAKING CHANGE] Changed `--lang` to no longer default to `Csharp`.</span></span> <span data-ttu-id="15ad5-1605">Wenn der Befehl `--lang` erfordert und dies nicht angegeben ist, wird der Befehl nun mit Fehler beendet.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1605">If the command requires `--lang` and it is not provided, the command will now error out</span></span>
* <span data-ttu-id="15ad5-1606">[BREAKING CHANGE]`--appid`- und `--password`-Argumente für `bot create` in erforderlich geändert, sie können jetzt über `ad app create` erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1606">[BREAKING CHANGE] Changed the `--appid` and `--password` args for `bot create` to be required and can now be created via `ad app create`</span></span>
* <span data-ttu-id="15ad5-1607">`--appid`- und `--password`-Validierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1607">Added `--appid` and `--password` validation</span></span>
* <span data-ttu-id="15ad5-1608">[BREAKING CHANGE]`bot create -v v4` geändert, sodass kein Speicherkonto bzw. keine Application Insights-Instanz erstellt oder verwendet wird</span><span class="sxs-lookup"><span data-stu-id="15ad5-1608">[BREAKING CHANGE] Changed `bot create -v v4` to not create or use a Storage Account or Application Insights</span></span>
* <span data-ttu-id="15ad5-1609">[BREAKING CHANGE]`bot create -v v3` geändert, sodass eine Region erforderlich ist, in der Application Insights verfügbar ist</span><span class="sxs-lookup"><span data-stu-id="15ad5-1609">[BREAKING CHANGE] Changed `bot create -v v3` to require a region where Application Insights is available</span></span>
* <span data-ttu-id="15ad5-1610">[BREAKING CHANGE]`bot update` geändert, sodass es sich jetzt nur auf spezifische Eigenschaften eines Bots auswirkt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1610">[BREAKING CHANGE] Changed `bot update` to now affect only specific properties of a bot</span></span>
* <span data-ttu-id="15ad5-1611">[BREAKING CHANGE]`--lang`-Flags geändert, sodass `Javascript` anstelle von `Node` akzeptiert wird</span><span class="sxs-lookup"><span data-stu-id="15ad5-1611">[BREAKING CHANGE] Changed `--lang` flags to accept `Javascript` instead of `Node`</span></span>
* <span data-ttu-id="15ad5-1612">[BREAKING CHANGE]`Node` als zulässiger `--lang`-Wert entfernt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1612">[BREAKING CHANGE] Removed `Node` as an allowed `--lang` value</span></span>
* <span data-ttu-id="15ad5-1613">[BREAKING CHANGE]`bot create -v v4 -k webapp` geändert, sodass `SCM_DO_BUILD_DURING_DEPLOYMENT` nicht mehr auf TRUE festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1613">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to no longer set `SCM_DO_BUILD_DURING_DEPLOYMENT` to true.</span></span> <span data-ttu-id="15ad5-1614">Alle Bereitstellungen über Kudu fungieren ihrem Standardverhalten entsprechend.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1614">All deployments through Kudu will act according to their default behavior</span></span>
* <span data-ttu-id="15ad5-1615">`bot download` für Bots ohne `.bot`-Dateien geändert, sodass die sprachspezifische Konfigurationsdatei mit Werten aus den Anwendungseinstellungen für den Bot erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1615">Changed `bot download` for bots without `.bot` files to create the language-specific configuration file with values from the Application Settings for the bot</span></span>
* <span data-ttu-id="15ad5-1616">Unterstützung für `Typescript` zu `bot prepare-deploy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1616">Added `Typescript` support to `bot prepare-deploy`</span></span>
* <span data-ttu-id="15ad5-1617">Warnmeldung zu `bot prepare-deploy` für `Javascript`- und `Typescript`-Bots hinzugefügt, wenn `package.json` in `--code-dir` nicht enthalten ist</span><span class="sxs-lookup"><span data-stu-id="15ad5-1617">Added warning message to `bot prepare-deploy` for `Javascript` and `Typescript` bots for when `--code-dir` does not contain `package.json`</span></span>
* <span data-ttu-id="15ad5-1618">`bot prepare-deploy` geändert, sodass bei Erfolg `true` zurückgegeben wird</span><span class="sxs-lookup"><span data-stu-id="15ad5-1618">Changed `bot prepare-deploy` to return `true` if successful</span></span>
* <span data-ttu-id="15ad5-1619">Ausführliche Protokollierung zu `bot prepare-deploy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1619">Added verbose logging to `bot prepare-deploy`</span></span>
* <span data-ttu-id="15ad5-1620">Mehr verfügbare Application Insights-Regionen zu `az bot create -v v3` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1620">Added more available Application Insights regions to `az bot create -v v3`</span></span>

### <a name="configure"></a><span data-ttu-id="15ad5-1621">Konfigurieren</span><span class="sxs-lookup"><span data-stu-id="15ad5-1621">Configure</span></span>
* <span data-ttu-id="15ad5-1622">Unterstützung für die ordnerbasierte Argument-Standardwertkonfigurationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1622">Added support for folder based argument default value configurations</span></span>

### <a name="eventhubs"></a><span data-ttu-id="15ad5-1623">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="15ad5-1623">Eventhubs</span></span>
* <span data-ttu-id="15ad5-1624">Befehle vom Typ `namespace network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1624">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="15ad5-1625">`--default-action`-Argument für Netzwerkregeln zu `namespace [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1625">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="15ad5-1626">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="15ad5-1626">Network</span></span>
* <span data-ttu-id="15ad5-1627">[BREAKING CHANGE]`--cache`-Argument mit `--defer` für `vnet [create|update]` ersetzt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1627">[BREAKING CHANGE] Replaced `--cache` arugment with `--defer` for `vnet [create|update]`</span></span> 

### <a name="policy-insights"></a><span data-ttu-id="15ad5-1628">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="15ad5-1628">Policy Insights</span></span>
* <span data-ttu-id="15ad5-1629">Unterstützung für `--expand PolicyEvaluationDetails` hinzugefügt, sodass Richtlinienauswertungsdetails von der Ressource abgefragt werden</span><span class="sxs-lookup"><span data-stu-id="15ad5-1629">Added support for `--expand PolicyEvaluationDetails` to query policy evaluation details on the resource</span></span>

### <a name="role"></a><span data-ttu-id="15ad5-1630">Role</span><span class="sxs-lookup"><span data-stu-id="15ad5-1630">Role</span></span>
* <span data-ttu-id="15ad5-1631">[VERALTET]: Ausblenden des „--password"-Arguments von `create-for-rbac` geändert; Unterstützung wird im Mai 2019 entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1631">[DEPRECATED] Changed `create-for-rbac` hide '--password' argument - support will be removed in May 2019</span></span>

### <a name="service-bus"></a><span data-ttu-id="15ad5-1632">Service Bus</span><span class="sxs-lookup"><span data-stu-id="15ad5-1632">Service Bus</span></span>
* <span data-ttu-id="15ad5-1633">Befehle vom Typ `namespace network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1633">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="15ad5-1634">`--default-action`-Argument für Netzwerkregeln zu `namespace [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1634">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>
* <span data-ttu-id="15ad5-1635">`topic [create|update]` korrigiert, sodass `--max-size`-Unterstützung für 10-, 20-, 40- und 80-GB-Werte mit Premium-SKU zulässig ist</span><span class="sxs-lookup"><span data-stu-id="15ad5-1635">Fixed `topic [create|update]` to allow `--max-size` support for 10, 20, 40 and 80GB values with premium SKU</span></span>

### <a name="sql"></a><span data-ttu-id="15ad5-1636">SQL</span><span class="sxs-lookup"><span data-stu-id="15ad5-1636">SQL</span></span>
* <span data-ttu-id="15ad5-1637">Befehle vom Typ `sql virtual-cluster [list|show|delete]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1637">Added `sql virtual-cluster [list|show|delete]` commands</span></span>

### <a name="vm"></a><span data-ttu-id="15ad5-1638">VM</span><span class="sxs-lookup"><span data-stu-id="15ad5-1638">VM</span></span>
* <span data-ttu-id="15ad5-1639">`--protect-from-scale-in` und `--protect-from-scale-set-actions` zu `vmss update` hinzugefügt, sodass Aktualisierungen der Schutzrichtlinie von VMSS-VM-Instanzen aktiviert sind</span><span class="sxs-lookup"><span data-stu-id="15ad5-1639">Added `--protect-from-scale-in` and `--protect-from-scale-set-actions` to `vmss update` to enable updates to the protection policy of VMSS VM instances</span></span>
* <span data-ttu-id="15ad5-1640">`--instance-id` zu `vmss update` hinzugefügt, sodass allgemeine Aktualisierungen von VMSS-VM-Instanzen aktiviert sind</span><span class="sxs-lookup"><span data-stu-id="15ad5-1640">Added `--instance-id` to `vmss update` to enable generic update of VMSS VM instances</span></span>
* <span data-ttu-id="15ad5-1641">`--instance-id` zu `vmss wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1641">Added `--instance-id` to `vmss wait`</span></span>
* <span data-ttu-id="15ad5-1642">Neue `ppg`-Befehlsgruppe für die Verwaltung von Näherungsplatzierungsgruppen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1642">Added new `ppg` command group for managing Proximity Placement Groups</span></span>
* <span data-ttu-id="15ad5-1643">`--ppg` zu `[vm|vmss] create` und `vm availability-set create` für die Verwaltung von PPGs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1643">Added `--ppg` to `[vm|vmss] create` and `vm availability-set create` for managing PPGs</span></span>
* <span data-ttu-id="15ad5-1644">Parameter `--hyper-v-generation` zu `image create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1644">Added `--hyper-v-generation` parameter to `image create`</span></span>

## <a name="april-23-2019"></a><span data-ttu-id="15ad5-1645">23. April 2019</span><span class="sxs-lookup"><span data-stu-id="15ad5-1645">April 23, 2019</span></span>

<span data-ttu-id="15ad5-1646">Version 2.0.63</span><span class="sxs-lookup"><span data-stu-id="15ad5-1646">Version 2.0.63</span></span>

### <a name="acs"></a><span data-ttu-id="15ad5-1647">ACS</span><span class="sxs-lookup"><span data-stu-id="15ad5-1647">ACS</span></span>
* <span data-ttu-id="15ad5-1648">`aks get-credentials` zur Anzeige einer Eingabeaufforderung zum Überschreiben doppelter Werte geändert</span><span class="sxs-lookup"><span data-stu-id="15ad5-1648">Changed `aks get-credentials` to prompt to overwrite duplicated values</span></span>
* <span data-ttu-id="15ad5-1649">`(PREVIEW)` aus Dev Spaces-Befehlen „aks use-dev-spaces“ und „aks remove-dev-spaces“ entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1649">Removed `(PREVIEW)` from Dev Spaces commands "aks use-dev-spaces" and "aks remove-dev-spaces"</span></span>

### <a name="ams"></a><span data-ttu-id="15ad5-1650">AMS</span><span class="sxs-lookup"><span data-stu-id="15ad5-1650">AMS</span></span>
* <span data-ttu-id="15ad5-1651">Fehler bei der Objekt- und Kontofilteraktualisierung behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-1651">Fixed bug with asset and account filters update</span></span>

### <a name="appservice"></a><span data-ttu-id="15ad5-1652">AppService</span><span class="sxs-lookup"><span data-stu-id="15ad5-1652">AppService</span></span>
* <span data-ttu-id="15ad5-1653">Unterstützung für die App Service-Umgebung (App Service Environment, ASE) und Zeitlimit zu `webapp ssh` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1653">Added support for ASE and timeout to `webapp ssh`</span></span>
* <span data-ttu-id="15ad5-1654">Unterstützung für die Einrichtung von CI/CD für eine Azure DevOps-Pipeline aus einem GitHub-Repository zu Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1654">Added support for establishing CI CD to an Azure DevOps pipeline from a Github repository to Function apps</span></span>
* <span data-ttu-id="15ad5-1655">`--github-pat`-Argument zu `functionapp devops-build create` hinzugefügt, um persönliche GitHub-Zugriffstoken zu akzeptieren</span><span class="sxs-lookup"><span data-stu-id="15ad5-1655">Added `--github-pat` argument to `functionapp devops-build create` to accept Github personal access token</span></span>
* <span data-ttu-id="15ad5-1656">`--github-repository`-Argument zu `functionapp devops-build create` hinzugefügt, um das GitHub-Repository mit dem Quellcode einer Funktions-App zu akzeptieren</span><span class="sxs-lookup"><span data-stu-id="15ad5-1656">Added `--github-repository` argument to `functionapp devops-build create` to accept Github repository that contains a functionapp source code</span></span>
* <span data-ttu-id="15ad5-1657">Problem behoben, aufgrund dessen bei `az webapp up --logs` ein Fehler auftrat und die .NET Core-Standardversion auf 2.1 aktualisiert wurde</span><span class="sxs-lookup"><span data-stu-id="15ad5-1657">Fixed issue where `az webapp up --logs` was failing with a error and updating default .NETCORE version to 2.1</span></span>
* <span data-ttu-id="15ad5-1658">Unnötige Funktions-App-Einstellungen beim Erstellen einer Funktions-App mit Verbrauchsplan entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1658">Removed unnecessary functionapp settings when creating a function app with consumption plan</span></span>
* <span data-ttu-id="15ad5-1659">`webapp up` geändert, sodass die ASP-Standardzeichenfolge jetzt eine Zahl am Ende anfügt, um einen neuen ASP basierend auf SKU-Optionen zu erstellen</span><span class="sxs-lookup"><span data-stu-id="15ad5-1659">Changed `webapp up` so the default asp string now appends number at the end to create a new ASP based on SKU options</span></span>
* <span data-ttu-id="15ad5-1660">`-b` als Option für `webapp up` hinzugefügt, um die App im Browser zu starten</span><span class="sxs-lookup"><span data-stu-id="15ad5-1660">Added `-b` as an option to `webapp up` to launch the app in the browser</span></span>
* <span data-ttu-id="15ad5-1661">`webapp deployment source config zip` geändert, um die `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`-Umgebungsvariable zu behandeln</span><span class="sxs-lookup"><span data-stu-id="15ad5-1661">Changed `webapp deployment source config zip` to handle `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="15ad5-1662">Bereitstellungs-Manager</span><span class="sxs-lookup"><span data-stu-id="15ad5-1662">Deployment Manager</span></span>
* <span data-ttu-id="15ad5-1663">[VORSCHAUVERSIPN] Erstellen und Verwalten von Artefakten, die Rollouts unterstützen</span><span class="sxs-lookup"><span data-stu-id="15ad5-1663">[PREVIEW] Create and manage artifacts that support rollouts</span></span>

### <a name="lab"></a><span data-ttu-id="15ad5-1664">Labor</span><span class="sxs-lookup"><span data-stu-id="15ad5-1664">Lab</span></span>
* <span data-ttu-id="15ad5-1665">Fehler behoben, der zu einer vorzeitigen Beendigung führen würde</span><span class="sxs-lookup"><span data-stu-id="15ad5-1665">Fixed bug which would cause an early exit</span></span>

### <a name="network"></a><span data-ttu-id="15ad5-1666">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="15ad5-1666">Network</span></span>
* <span data-ttu-id="15ad5-1667">Automatische Delegierung des Namenservers im übergeordneten Element während der Erstellung der untergeordneten Zone zu `dns zone create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1667">Added auto name server delegation to `dns zone create` in parent during child zone creation</span></span>

### <a name="resource"></a><span data-ttu-id="15ad5-1668">Resource</span><span class="sxs-lookup"><span data-stu-id="15ad5-1668">Resource</span></span>
* <span data-ttu-id="15ad5-1669">[VERALTET]: Argumente `--link-id`, `--target-id` und `--filter-string` von `resource link` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-1669">[DEPRECATED] Deprecated `--link-id`, `--target-id` and `--filter-string` arguments of `resource link`</span></span>
  * <span data-ttu-id="15ad5-1670">Verwenden Sie stattdessen die Argumente `--link`, `--target` und `--filter`.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1670">Use the arguments `--link`, `--target`, and `--filter` instead</span></span>
* <span data-ttu-id="15ad5-1671">Problem behoben, aufgrund dessen `resource link [create|update]`-Befehle nicht verwendet werden konnten</span><span class="sxs-lookup"><span data-stu-id="15ad5-1671">Fixed issue where `resource link [create|update]` commands would not work</span></span>
* <span data-ttu-id="15ad5-1672">Problem behoben, aufgrund dessen das Löschen anhand einer Ressourcen-ID bei einem Fehler zu einem Absturz führen konnte</span><span class="sxs-lookup"><span data-stu-id="15ad5-1672">Fixed an issue where deleting using a resource ID could crash on error</span></span>

### <a name="sql"></a><span data-ttu-id="15ad5-1673">SQL</span><span class="sxs-lookup"><span data-stu-id="15ad5-1673">SQL</span></span>
* <span data-ttu-id="15ad5-1674">Unterstützung für benutzerdefinierte Zeitzonen auf verwalteten Instanzen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1674">Added support for custom time zone on managed instances</span></span>
* <span data-ttu-id="15ad5-1675">Geändert, um die Verwendung des Namens eines Pools für elastische Datenbanken mit `sql db update` zuzulassen</span><span class="sxs-lookup"><span data-stu-id="15ad5-1675">Changed to allow elastic pool name to be used with `sql db update`</span></span>
* <span data-ttu-id="15ad5-1676">Unterstützung für `--no-wait` zu `sql server [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1676">Added `--no-wait` support to `sql server [create|update]`</span></span>
* <span data-ttu-id="15ad5-1677">Befehl `sql server wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1677">Added command `sql server wait`</span></span>

### <a name="storage"></a><span data-ttu-id="15ad5-1678">Storage</span><span class="sxs-lookup"><span data-stu-id="15ad5-1678">Storage</span></span>
* <span data-ttu-id="15ad5-1679">Problem mit doppelt codierten SAS-Token in `storage blob generate-sas` behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-1679">Fixed issue with double-encoded SAS tokens in `storage blob generate-sas`</span></span>

### <a name="vm"></a><span data-ttu-id="15ad5-1680">VM</span><span class="sxs-lookup"><span data-stu-id="15ad5-1680">VM</span></span>
* <span data-ttu-id="15ad5-1681">`--skip-shutdown`-Flag zum Ausschalten von VMs ohne Herunterfahren zu `vm|vmss stop` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1681">Added `--skip-shutdown` flag to `vm|vmss stop` to power-off VMs without shutdown</span></span>
* <span data-ttu-id="15ad5-1682">`--storage-account-type`-Argument zum Festlegen des Kontotyps des Veröffentlichungsprofils zu `sig image-version create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1682">Added `--storage-account-type` argument to `sig image-version create` to set the publishing profile's account type</span></span>
* <span data-ttu-id="15ad5-1683">`--target-regions`-Argument zu `sig image-version create` hinzugefügt, um das Festlegen von regionsspezifischen Speicherkontotypen zuzulassen</span><span class="sxs-lookup"><span data-stu-id="15ad5-1683">Added `--target-regions` argument to `sig image-version create` to allow setting region-specific storage account types</span></span>

## <a name="april-9-2019"></a><span data-ttu-id="15ad5-1684">9\. April 2019</span><span class="sxs-lookup"><span data-stu-id="15ad5-1684">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="15ad5-1685">Core</span><span class="sxs-lookup"><span data-stu-id="15ad5-1685">Core</span></span>
* <span data-ttu-id="15ad5-1686">Problem behoben, aufgrund dessen einige Erweiterungen mit der Version `Unknown` angezeigt wurden und nicht aktualisiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="15ad5-1686">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="15ad5-1687">ACR</span><span class="sxs-lookup"><span data-stu-id="15ad5-1687">ACR</span></span>
* <span data-ttu-id="15ad5-1688">Unterstützung für die kontextlose Ausführung eines Images hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1688">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="15ad5-1689">AMS</span><span class="sxs-lookup"><span data-stu-id="15ad5-1689">AMS</span></span>
* [VERALTET]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
[DEPRECATED]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [BREAKING CHANGE]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="15ad5-1692">Unterstützung für neue Verschlüsselungsparameter in `ams streaming-policy create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1692">Added new encryption parameters support in `ams streaming-policy create`</span></span>
* <span data-ttu-id="15ad5-1693">Neuer Parameter `--filters` zu `ams streaming-locator create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1693">Added new paramter `--filters` to `ams streaming-locator create`</span></span>

### <a name="appservice"></a><span data-ttu-id="15ad5-1694">AppService</span><span class="sxs-lookup"><span data-stu-id="15ad5-1694">AppService</span></span>
* <span data-ttu-id="15ad5-1695">Unterstützung für `--logs` zu `webapp up` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1695">Added `--logs` support to `webapp up`</span></span>
* <span data-ttu-id="15ad5-1696">Probleme bei der Generierung von `azure-pipelines.yml` beim Befehl `functionapp devops-build create` behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-1696">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="15ad5-1697">Fehlerbehandlung und Indikatoren für `unctionapp devops-build create` verbessert</span><span class="sxs-lookup"><span data-stu-id="15ad5-1697">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="15ad5-1698">[BREAKING CHANGE] Flag `--local-git` für den Befehl `devops-build` entfernt; lokale Git-Erkennung und -Verarbeitung sind zum Erstellen von Azure DevOps-Pipelines obligatorisch</span><span class="sxs-lookup"><span data-stu-id="15ad5-1698">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="15ad5-1699">Unterstützung für das Erstellen von Linux-Functions-Plänen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1699">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="15ad5-1700">Möglichkeit zum Wechseln eines Plans unter einer Funktions-App mit `functionapp update --plan` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1700">Added ability to switch a plan underneath a function app using `functionapp update --plan`</span></span>
* <span data-ttu-id="15ad5-1701">Unterstützung für Einstellungen zum Aufskalieren für den Azure Functions-Premium-Plan hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1701">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="15ad5-1702">CDN</span><span class="sxs-lookup"><span data-stu-id="15ad5-1702">CDN</span></span>
* <span data-ttu-id="15ad5-1703">Unterstützung hinzugefügt für `Microsoft_Standard` und `Standard_ChinaCdn`</span><span class="sxs-lookup"><span data-stu-id="15ad5-1703">Added support for `Microsoft_Standard` and `Standard_ChinaCdn`</span></span>

### <a name="feedback"></a><span data-ttu-id="15ad5-1704">Feedback</span><span class="sxs-lookup"><span data-stu-id="15ad5-1704">Feedback</span></span>
* <span data-ttu-id="15ad5-1705">`feedback` zur Anzeige von Metadaten zu den zuletzt ausgeführten Befehlen geändert</span><span class="sxs-lookup"><span data-stu-id="15ad5-1705">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="15ad5-1706">`feedback` geändert, um den Benutzer zur Unterstützung beim Issueerstellungsprozess aufzufordern (durch Öffnen eines Browsers und Verwenden einer Issuevorlage)</span><span class="sxs-lookup"><span data-stu-id="15ad5-1706">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="15ad5-1707">`feedback` geändert, um den Issuetext bei der Ausführung mit „--verbose“ auszugeben</span><span class="sxs-lookup"><span data-stu-id="15ad5-1707">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="15ad5-1708">Überwachen</span><span class="sxs-lookup"><span data-stu-id="15ad5-1708">Monitor</span></span>
* <span data-ttu-id="15ad5-1709">Problem behoben, aufgrund dessen „Count“ kein zulässiger Wert für `metrics alert [create|update]` war</span><span class="sxs-lookup"><span data-stu-id="15ad5-1709">Fixed issue where "count" was not a permitted value with `metrics alert [create|update]`</span></span> 

### <a name="network"></a><span data-ttu-id="15ad5-1710">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="15ad5-1710">Network</span></span>
* <span data-ttu-id="15ad5-1711">Problem behoben, aufgrund dessen das Tabellenformat mit `vnet-gateway list-bgp-peer-status` nicht angezeigt wurde</span><span class="sxs-lookup"><span data-stu-id="15ad5-1711">Fixed table format not displaying with `vnet-gateway list-bgp-peer-status`</span></span>
* <span data-ttu-id="15ad5-1712">Befehle `list-request-headers` und `list-response-headers` zu `application-gateway rewrite-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1712">Added `list-request-headers` and `list-response-headers` commands to `application-gateway rewrite-rule`</span></span>
* <span data-ttu-id="15ad5-1713">Befehl `list-server-variables` zu `application-gateway rewrite-rule condition` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1713">Added `list-server-variables` command to `application-gateway rewrite-rule condition`</span></span>
* <span data-ttu-id="15ad5-1714">Problem behoben, aufgrund dessen durch das Aktualisieren des Linkstatus für einen ExpressRoute-Port eine Ausnahme vom Typ „unbekanntes Attribut“ ausgelöst wurde: `express-route port update`</span><span class="sxs-lookup"><span data-stu-id="15ad5-1714">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception `express-route port update`</span></span>

### <a name="privatedns"></a><span data-ttu-id="15ad5-1715">PrivateDNS</span><span class="sxs-lookup"><span data-stu-id="15ad5-1715">PrivateDNS</span></span>
* <span data-ttu-id="15ad5-1716">`network private-dns` für private DNS-Zonen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1716">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="15ad5-1717">Resource</span><span class="sxs-lookup"><span data-stu-id="15ad5-1717">Resource</span></span>
* <span data-ttu-id="15ad5-1718">Problem mit `deployment create` und `group deployment create` behoben, aufgrund dessen eine Parameterdatei mit leerem Parametersatz nicht verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="15ad5-1718">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="15ad5-1719">Role</span><span class="sxs-lookup"><span data-stu-id="15ad5-1719">Role</span></span>
* <span data-ttu-id="15ad5-1720">`create-for-rbac` korrigiert, um `--years` korrekt zu verarbeiten</span><span class="sxs-lookup"><span data-stu-id="15ad5-1720">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="15ad5-1721">[BREAKING CHANGE]`role assignment delete` geändert, um eine Eingabeaufforderung anzuzeigen, wenn alle Zuweisungen im Abonnement ohne Bedingungen gelöscht werden</span><span class="sxs-lookup"><span data-stu-id="15ad5-1721">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="15ad5-1722">SQL</span><span class="sxs-lookup"><span data-stu-id="15ad5-1722">SQL</span></span>
* <span data-ttu-id="15ad5-1723">`sql mi [create|update]` mit den Eigenschaften „proxyOverride“ und „publicDataEndpointEnabled“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-1723">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="15ad5-1724">Storage</span><span class="sxs-lookup"><span data-stu-id="15ad5-1724">Storage</span></span>
* <span data-ttu-id="15ad5-1725">[BREAKING CHANGE] Ergebnis von `storage blob delete` entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1725">[BREAKING CHANGE] Removed result of `storage blob delete`</span></span>
* <span data-ttu-id="15ad5-1726">`--full-uri` zu `storage blob generate-sas` hinzugefügt, um den vollständigen URI für das Blob mit SAS zu erstellen</span><span class="sxs-lookup"><span data-stu-id="15ad5-1726">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="15ad5-1727">`--file-snapshot` zu `storage file copy start` hinzugefügt, um die Datei aus der Momentaufnahme zu kopieren</span><span class="sxs-lookup"><span data-stu-id="15ad5-1727">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="15ad5-1728">`storage blob copy cancel` geändert, um anstelle der Ausnahme für „NoPendingCopyOperation“ nur den Fehler anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="15ad5-1728">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="15ad5-1729">26. März 2019</span><span class="sxs-lookup"><span data-stu-id="15ad5-1729">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="15ad5-1730">Core</span><span class="sxs-lookup"><span data-stu-id="15ad5-1730">Core</span></span>
* <span data-ttu-id="15ad5-1731">Probleme mit der Inkompatibilität der Entwicklungserweiterung behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-1731">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="15ad5-1732">Die Fehlerbehandlung verweist Kunden jetzt auf die Problemseite.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1732">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="15ad5-1733">Cloud</span><span class="sxs-lookup"><span data-stu-id="15ad5-1733">Cloud</span></span>
* <span data-ttu-id="15ad5-1734">Fehler „Abonnement nicht gefunden“ in `cloud set` behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-1734">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="15ad5-1735">ACR</span><span class="sxs-lookup"><span data-stu-id="15ad5-1735">ACR</span></span>
* <span data-ttu-id="15ad5-1736">Redundante Quellen im Imageimport korrigiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-1736">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="15ad5-1737">`--auth-mode` wurde den Befehlen `acr build`, `acr run`, `acr task create` und `acr task update` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1737">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="15ad5-1738">Befehlsgruppe „acr task credential“ zum Verwalten von Anmeldeinformationen für eine Aufgabe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1738">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="15ad5-1739">„--no-wait“ zum Befehl `acr build` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1739">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="15ad5-1740">AppService</span><span class="sxs-lookup"><span data-stu-id="15ad5-1740">AppService</span></span>
* <span data-ttu-id="15ad5-1741">Problem behoben, das dazu führte, dass die Ausführung aus einem leeren Verzeichnis oder ein Szenario mit unbekannten Code von `webapp up` nicht korrekt behandelt wurde</span><span class="sxs-lookup"><span data-stu-id="15ad5-1741">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="15ad5-1742">Problem behoben, aufgrund dessen Slots für `[webapp|functionapp] config ssl bind` nicht verwendet werden konnten</span><span class="sxs-lookup"><span data-stu-id="15ad5-1742">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="15ad5-1743">Bot Service</span><span class="sxs-lookup"><span data-stu-id="15ad5-1743">BOT Service</span></span>
* <span data-ttu-id="15ad5-1744">`bot prepare-deploy` hinzugefügt, um die Bereitstellung von Bots über `webapp` vorzubereiten</span><span class="sxs-lookup"><span data-stu-id="15ad5-1744">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="15ad5-1745">`bot create --kind registration` geändert, um das Kennwort anzuzeigen, falls kein Kennwort angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="15ad5-1745">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="15ad5-1746">[BREAKING CHANGE]`--endpoint` wurde in `bot create --kind registration` geändert, sodass nun standardmäßig eine leere Zeichenfolge verwendet wird, anstatt eine Angabe zu erfordern.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1746">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="15ad5-1747">`SCM_DO_BUILD_DURING_DEPLOYMENT` zu den Anwendungseinstellungen der ARM-Vorlage für Web-App-Bot (v4) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1747">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="15ad5-1748">CDN</span><span class="sxs-lookup"><span data-stu-id="15ad5-1748">CDN</span></span>
* <span data-ttu-id="15ad5-1749">Unterstützung für `--no-wait` zu `cdn endpoint [create|update|start|stop|delete|load|purge]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1749">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* <span data-ttu-id="15ad5-1750">[BREAKING CHANGE] Das standardmäßige Zwischenspeicherverhalten für Abfragezeichenfolgen von `cdn endpoint create` wurde geändert.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1750">[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour.</span></span> <span data-ttu-id="15ad5-1751">Es wird nicht mehr standardmäßig „IgnoreQueryString“ festgelegt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1751">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="15ad5-1752">Er wird jetzt vom Dienst festgelegt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1752">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="15ad5-1753">Cosmosdb</span><span class="sxs-lookup"><span data-stu-id="15ad5-1753">Cosmosdb</span></span>
* <span data-ttu-id="15ad5-1754">Unterstützung für `--enable-multiple-write-locations` bei Kontoaktualisierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1754">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="15ad5-1755">Untergruppe `network-rule` mit Befehlen `add`, `remove` und `list` zum Verwalten von VNET-Regeln eines Cosmos DB-Kontos hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1755">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="15ad5-1756">Interactive</span><span class="sxs-lookup"><span data-stu-id="15ad5-1756">Interactive</span></span>
* <span data-ttu-id="15ad5-1757">Inkompatibilität mit der über azdev installierten interaktiven Erweiterung korrigiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-1757">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="15ad5-1758">Überwachen</span><span class="sxs-lookup"><span data-stu-id="15ad5-1758">Monitor</span></span>
* <span data-ttu-id="15ad5-1759">Geändert, sodass der Dimensionswert `*` für `monitor metrics alert [create|update]` zulässig ist</span><span class="sxs-lookup"><span data-stu-id="15ad5-1759">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="15ad5-1760">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="15ad5-1760">Network</span></span>
* <span data-ttu-id="15ad5-1761">Befehlsgruppe `rewrite-rule` zu `application-gateway` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1761">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="15ad5-1762">Profil</span><span class="sxs-lookup"><span data-stu-id="15ad5-1762">Profile</span></span>
* <span data-ttu-id="15ad5-1763">Kontounterstützung auf Mandantenebene für verwaltete Dienstidentität zu `login` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1763">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="15ad5-1764">Postgres</span><span class="sxs-lookup"><span data-stu-id="15ad5-1764">Postgres</span></span> 
* <span data-ttu-id="15ad5-1765">postgresql-Befehle vom Typ `replica` und Befehl `restart server` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1765">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="15ad5-1766">Änderungen vorgenommen, um den Standardspeicherort aus der Ressourcengruppe abzurufen, wenn er für die Erstellung von Servern nicht angegeben wurde, und um eine Überprüfung für die Aufbewahrungstage hinzuzufügen</span><span class="sxs-lookup"><span data-stu-id="15ad5-1766">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="15ad5-1767">Resource</span><span class="sxs-lookup"><span data-stu-id="15ad5-1767">Resource</span></span>
* <span data-ttu-id="15ad5-1768">Verbesserte Tabellenausgabe für `deployment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="15ad5-1768">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="15ad5-1769">Problem mit `deployment [create|validate]` behoben, aufgrund dessen der Typ „secureObject“ nicht erkannt wurde</span><span class="sxs-lookup"><span data-stu-id="15ad5-1769">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="15ad5-1770">Graph</span><span class="sxs-lookup"><span data-stu-id="15ad5-1770">Graph</span></span>
* <span data-ttu-id="15ad5-1771">Unterstützung für `--end-date` zu `ad [app|sp] credential reset` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1771">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="15ad5-1772">Unterstützung für das Hinzufügen von Berechtigungen mit `ad app permission add` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1772">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="15ad5-1773">Fehler mit `ad app permission list` behoben, wenn keine Berechtigungen vorlagen</span><span class="sxs-lookup"><span data-stu-id="15ad5-1773">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="15ad5-1774">Änderung an `ad sp delete` vorgenommen, um das Entfernen einer Rollenzuweisung zu überspringen, wenn das aktuelle Konto kein Abonnement enthält</span><span class="sxs-lookup"><span data-stu-id="15ad5-1774">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="15ad5-1775">`ad app create` geändert, sodass ohne Angabe für `--identifier-uris` standardmäßig eine leere Liste verwendet wird</span><span class="sxs-lookup"><span data-stu-id="15ad5-1775">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="15ad5-1776">storage</span><span class="sxs-lookup"><span data-stu-id="15ad5-1776">storage</span></span>
* <span data-ttu-id="15ad5-1777">`--snapshot` zu `storage file download-batch` für den Download von einer Freigabemomentaufnahme hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1777">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="15ad5-1778">Statusanzeige für `storage blob [download-batch|upload-batch]` geändert, damit sie weniger ausführlich dargestellt wird und das aktuelle Blob angibt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1778">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="15ad5-1779">Problem mit `storage account update` behoben, das beim Aktualisieren von Verschlüsselungsparametern auftrat</span><span class="sxs-lookup"><span data-stu-id="15ad5-1779">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="15ad5-1780">Problem behoben, bei dem für `storage blob show` ein Fehler auftrat, wenn oauth (`--auth-mode=login`) verwendet wurde</span><span class="sxs-lookup"><span data-stu-id="15ad5-1780">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="15ad5-1781">VM</span><span class="sxs-lookup"><span data-stu-id="15ad5-1781">VM</span></span>
* <span data-ttu-id="15ad5-1782">Befehl `image update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1782">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="15ad5-1783">12. März 2019</span><span class="sxs-lookup"><span data-stu-id="15ad5-1783">March 12, 2019</span></span>

<span data-ttu-id="15ad5-1784">Version 2.0.60</span><span class="sxs-lookup"><span data-stu-id="15ad5-1784">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="15ad5-1785">Core</span><span class="sxs-lookup"><span data-stu-id="15ad5-1785">Core</span></span>

* <span data-ttu-id="15ad5-1786">Falsche Fehlermeldung in `cloud set` zu nicht gefundenem Abonnement korrigiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-1786">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="15ad5-1787">ACR</span><span class="sxs-lookup"><span data-stu-id="15ad5-1787">ACR</span></span>

* <span data-ttu-id="15ad5-1788">Redundante Quellen im Imageimport korrigiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-1788">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="15ad5-1789">ACS</span><span class="sxs-lookup"><span data-stu-id="15ad5-1789">ACS</span></span>

* <span data-ttu-id="15ad5-1790">Änderung vorgenommen, um den Parameter `--listen-address` für `aks browse` zu ignorieren, wenn er nicht von kubectl unterstützt wird</span><span class="sxs-lookup"><span data-stu-id="15ad5-1790">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="15ad5-1791">AppService</span><span class="sxs-lookup"><span data-stu-id="15ad5-1791">AppService</span></span>

* <span data-ttu-id="15ad5-1792">`[webapp|functionapp] deployment list-publishing-credentials` hinzugefügt, um die Kudu-Veröffentlichungs-URL und die entsprechenden Anmeldeinformationen abzurufen</span><span class="sxs-lookup"><span data-stu-id="15ad5-1792">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="15ad5-1793">Fehlerhafte Ausgabeanweisung für `webapp auth update` entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1793">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="15ad5-1794">`functionapp` korrigiert, um das korrekte Image für die Runtime in App Service-Plänen unter Linux festzulegen</span><span class="sxs-lookup"><span data-stu-id="15ad5-1794">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="15ad5-1795">Vorschau-Tag für `webapp up` entfernt und Verbesserungen am Befehl implementiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-1795">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="15ad5-1796">Botservice</span><span class="sxs-lookup"><span data-stu-id="15ad5-1796">Botservice</span></span>

* <span data-ttu-id="15ad5-1797">`SCM_DO_BUILD_DURING_DEPLOYMENT` zu den Anwendungseinstellungen der ARM-Vorlage für Web-App-Bot (v4) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1797">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="15ad5-1798">`Microsoft-BotFramework-AppId` und `Microsoft-BotFramework-AppPassword` zu den Anwendungseinstellungen der ARM-Vorlage für Web-App-Bot (v4) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1798">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="15ad5-1799">Einfache Anführungszeichen aus der Befehlsausgabe von `bot publish` am Ende von `bot create` entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1799">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="15ad5-1800">`bot publish` wurde geändert und ist jetzt asynchron.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1800">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="15ad5-1801">Container</span><span class="sxs-lookup"><span data-stu-id="15ad5-1801">Container</span></span>

* <span data-ttu-id="15ad5-1802">Argument `--no-wait` zu `container [start|restart]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1802">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="15ad5-1803">EventHub</span><span class="sxs-lookup"><span data-stu-id="15ad5-1803">EventHub</span></span>

* <span data-ttu-id="15ad5-1804">Flag `--skip-empty-archives` zu `eventhub create|update` hinzugefügt, um leere Archive in der Aufzeichnung zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="15ad5-1804">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="15ad5-1805">Suchen</span><span class="sxs-lookup"><span data-stu-id="15ad5-1805">Find</span></span>

* <span data-ttu-id="15ad5-1806">Umfangreiches Funktionsupdate</span><span class="sxs-lookup"><span data-stu-id="15ad5-1806">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="15ad5-1807">HDInsight</span><span class="sxs-lookup"><span data-stu-id="15ad5-1807">HDInsight</span></span>

* <span data-ttu-id="15ad5-1808">Parameter `--storage-account-managed-identity` zu `hdinsight create` hinzugefügt, um MSI in ADLS Gen2 zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="15ad5-1808">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="15ad5-1809">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="15ad5-1809">Network</span></span>

* <span data-ttu-id="15ad5-1810">Problem mit `vpn-connection update` behoben, aufgrund dessen die Aktualisierung einer VPN-Verbindung zwischen Gateways in verschiedenen Abonnements fehlschlug</span><span class="sxs-lookup"><span data-stu-id="15ad5-1810">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="15ad5-1811">Rdbms</span><span class="sxs-lookup"><span data-stu-id="15ad5-1811">Rdbms</span></span>

* <span data-ttu-id="15ad5-1812">Kleinere Korrekturen, um den Standardspeicherort aus der Ressourcengruppe abzurufen, wenn er für die Erstellung von Servern nicht angegeben wurde, und um eine Überprüfung für die Aufbewahrungstage hinzuzufügen</span><span class="sxs-lookup"><span data-stu-id="15ad5-1812">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="15ad5-1813">Role</span><span class="sxs-lookup"><span data-stu-id="15ad5-1813">Role</span></span>

* <span data-ttu-id="15ad5-1814">`role definition update` wurde korrigiert und nutzt nun die ID, um die Definition korrekt aufzulösen.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1814">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="15ad5-1815">`ad app credential reset` geändert, um die Annahme zu entfernen, dass der Dienstprinzipal der App stets vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="15ad5-1815">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="15ad5-1816">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="15ad5-1816">Service Fabric</span></span>

* <span data-ttu-id="15ad5-1817">Das Problem, dass `sf cluster list` nicht wiederholbar war, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1817">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="15ad5-1818">26. Februar 2019</span><span class="sxs-lookup"><span data-stu-id="15ad5-1818">February 26, 2019</span></span>

<span data-ttu-id="15ad5-1819">Version 2.0.59</span><span class="sxs-lookup"><span data-stu-id="15ad5-1819">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="15ad5-1820">Core</span><span class="sxs-lookup"><span data-stu-id="15ad5-1820">Core</span></span>

* <span data-ttu-id="15ad5-1821">Problem behoben, aufgrund dessen die Verwendung von `--subscription NAME` in einigen Instanzen eine Ausnahme ausgelöst hat</span><span class="sxs-lookup"><span data-stu-id="15ad5-1821">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="15ad5-1822">ACR</span><span class="sxs-lookup"><span data-stu-id="15ad5-1822">ACR</span></span>

* <span data-ttu-id="15ad5-1823">Parameter `--target` für die Befehle `acr build`, `acr task create` und `acr task update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1823">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="15ad5-1824">Verbesserte Fehlerbehandlung für Runtimebefehle, wenn keine Anmeldung bei Azure besteht</span><span class="sxs-lookup"><span data-stu-id="15ad5-1824">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="15ad5-1825">ACS</span><span class="sxs-lookup"><span data-stu-id="15ad5-1825">ACS</span></span>

* <span data-ttu-id="15ad5-1826">Option `--listen-address` zu `aks port-forward` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1826">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="15ad5-1827">AppService</span><span class="sxs-lookup"><span data-stu-id="15ad5-1827">AppService</span></span>

* <span data-ttu-id="15ad5-1828">Befehl `functionapp devops-build` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1828">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="15ad5-1829">Batch</span><span class="sxs-lookup"><span data-stu-id="15ad5-1829">Batch</span></span>
* <span data-ttu-id="15ad5-1830">[BREAKING CHANGE] Befehl `batch pool upgrade os` entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1830">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="15ad5-1831">[BREAKING CHANGE]`Pacakges`-Eigenschaft aus `Application`-Antworten entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1831">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="15ad5-1832">Befehl `batch application package list` zum Auflisten von Paketen einer Anwendung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1832">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="15ad5-1833">[BREAKING CHANGE]`--application-id` in allen `batch application`-Befehlen in `--application-name` geändert</span><span class="sxs-lookup"><span data-stu-id="15ad5-1833">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="15ad5-1834">Argument `--json-file` für Befehle zum Anfordern der unformatierten API-Antwort hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1834">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="15ad5-1835">Validierung aktualisiert, sodass das `https://`-Element automatisch in alle Endpunkte aufgenommen wird, wenn es fehlt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1835">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="15ad5-1836">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="15ad5-1836">CosmosDB</span></span>

* <span data-ttu-id="15ad5-1837">Untergruppe `network-rule` mit Befehlen `add`, `remove` und `list` zum Verwalten von VNET-Regeln eines Cosmos DB-Kontos hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1837">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="15ad5-1838">Kusto</span><span class="sxs-lookup"><span data-stu-id="15ad5-1838">Kusto</span></span>

* <span data-ttu-id="15ad5-1839">[BREAKING CHANGE] Typen `hot_cache_period` und `soft_delete_period` für Datenbank in Format der Zeitspanne nach ISO8601 geändert</span><span class="sxs-lookup"><span data-stu-id="15ad5-1839">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="15ad5-1840">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="15ad5-1840">Network</span></span>

* <span data-ttu-id="15ad5-1841">Argument `--express-route-gateway-bypass` zu `vpn-connection [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1841">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="15ad5-1842">Befehlsgruppen aus `express-route`-Erweiterungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1842">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="15ad5-1843">Befehlsgruppen `express-route gateway` und `express-route port` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1843">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="15ad5-1844">Argument `--legacy-mode` zu `express-route peering [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1844">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="15ad5-1845">Argumente `--allow-classic-operations` und `--express-route-port` zu `express-route [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1845">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="15ad5-1846">Argument `--gateway-default-site` zu `vnet-gateway [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1846">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="15ad5-1847">Befehle vom Typ `ipsec-policy` zu `vnet-gateway` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1847">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="15ad5-1848">Resource</span><span class="sxs-lookup"><span data-stu-id="15ad5-1848">Resource</span></span>

* <span data-ttu-id="15ad5-1849">Problem mit `deployment create` behoben, aufgrund dessen beim Feld „Typ“ die Groß-/Kleinschreibung beachtet wurde</span><span class="sxs-lookup"><span data-stu-id="15ad5-1849">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="15ad5-1850">Unterstützung für URI-basierte Parameterdatei zu `policy assignment create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1850">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="15ad5-1851">Unterstützung für URI-basierte Parameter und Definitionen zu `policy set-definition update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1851">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="15ad5-1852">Verarbeitung von Parametern und Regeln für `policy definition update` korrigiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-1852">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="15ad5-1853">Problem mit `resource show/update/delete/tag/invoke-action` behoben, aufgrund dessen bei abonnementübergreifenden IDs die Abonnement-ID nicht ordnungsgemäß berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="15ad5-1853">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="15ad5-1854">Role</span><span class="sxs-lookup"><span data-stu-id="15ad5-1854">Role</span></span>

* <span data-ttu-id="15ad5-1855">Unterstützung für App-Rollen zu `ad app [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1855">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="15ad5-1856">VM</span><span class="sxs-lookup"><span data-stu-id="15ad5-1856">VM</span></span>

* <span data-ttu-id="15ad5-1857">Problem mit `vm create where ` behoben, aufgrund dessen der beschleunigte Netzwerkbetrieb für Ubuntu 18.0 nicht standardmäßig aktiviert war</span><span class="sxs-lookup"><span data-stu-id="15ad5-1857">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="15ad5-1858">12. Februar 2019</span><span class="sxs-lookup"><span data-stu-id="15ad5-1858">February 12, 2019</span></span>

<span data-ttu-id="15ad5-1859">Version 2.0.58</span><span class="sxs-lookup"><span data-stu-id="15ad5-1859">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="15ad5-1860">Core</span><span class="sxs-lookup"><span data-stu-id="15ad5-1860">Core</span></span>

* <span data-ttu-id="15ad5-1861">`az --version` zeigt jetzt eine Benachrichtigung an, wenn Sie Pakete haben, für die ein Update verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1861">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="15ad5-1862">Die Regression, dass `--ids` nicht mehr mit JSON-Ausgaben verwendet werden konnte, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1862">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="15ad5-1863">ACR</span><span class="sxs-lookup"><span data-stu-id="15ad5-1863">ACR</span></span>
* <span data-ttu-id="15ad5-1864">[BREAKING CHANGE] Die Befehlsgruppe `acr build-task` wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1864">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="15ad5-1865">[BREAKING CHANGE] Die Optionen `--tag` und `--manifest` wurden aus `acr repository delete` entfernt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1865">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="15ad5-1866">ACS</span><span class="sxs-lookup"><span data-stu-id="15ad5-1866">ACS</span></span>
* <span data-ttu-id="15ad5-1867">Unterstützung für Namen ohne Berücksichtigung von Groß-/Kleinschreibung wurde zu `aks [enable-addons|disable-addons]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1867">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="15ad5-1868">Unterstützung für Azure Active Directory-Aktualisierungsvorgang mithilfe von `aks update-credentials --reset-aad` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1868">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="15ad5-1869">Die Information, dass `--output` für `aks get-credentials` ignoriert wird, wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1869">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="15ad5-1870">AMS</span><span class="sxs-lookup"><span data-stu-id="15ad5-1870">AMS</span></span>
* <span data-ttu-id="15ad5-1871">Befehle vom Typ `ams streaming-endpoint [start | stop | create | update] wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1871">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="15ad5-1872">Befehle vom Typ `ams live-event [create | start | stop | reset] wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1872">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="15ad5-1873">AppService</span><span class="sxs-lookup"><span data-stu-id="15ad5-1873">Appservice</span></span>
* <span data-ttu-id="15ad5-1874">Die Möglichkeit zum Erstellen und Konfigurieren von Funktionen mithilfe von ACR-Containern wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1874">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="15ad5-1875">Unterstützung für das Aktualisieren von Web-App-Konfigurationen über JSON wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1875">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="15ad5-1876">Die Hilfe für `appservice-plan-update` wurde verbessert.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1876">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="15ad5-1877">Unterstützung für App-Erkenntnisse beim Erstellen von Funktions-Apps wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1877">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="15ad5-1878">Probleme mit der Web-App SSH wurden behoben.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1878">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="15ad5-1879">Botservice</span><span class="sxs-lookup"><span data-stu-id="15ad5-1879">Botservice</span></span>
* <span data-ttu-id="15ad5-1880">Die Benutzeroberfläche für `bot publish` wurde verbessert.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1880">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="15ad5-1881">Eine Warnung für Zeitlimit bei der Ausführung von `npm install` während `az bot publish` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1881">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="15ad5-1882">Ungültiges char-Element wurde `.` aus `--name` in `az bot create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1882">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="15ad5-1883">Eine Änderung wurde vorgenommen, um die zufällige Zuordnung von Ressourcennamen beim Erstellen von Azure Storage-Instanzen, App Service-Plänen, Funktions-/Web-Apps und Application Insights-Instanzen zu verhindern.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1883">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="15ad5-1884">[VERALTET] Argument `--proj-name` zugunsten von `--proj-file-path` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-1884">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="15ad5-1885">`az bot publish` wurde geändert, um abgerufene IIS-Bereitstellungsdateien vom Typ „Node.js“ zu entfernen, wenn sie nicht bereits vorhanden waren.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1885">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="15ad5-1886">Das `--keep-node-modules` Argument wurde zu `az bot publish` hinzugefügt, damit der Ordner `node_modules` in App Service nicht gelöscht wird.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1886">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="15ad5-1887">Das Schlüssel-Wert-Paar `"publishCommand"` wurde der Ausgabe von `az bot create` beim Erstellen einer Funktions-App oder eines Web-App-Bots hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1887">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="15ad5-1888">Der Wert von `"publishCommand"` ist ein `az bot publish`-Befehl, der bereits die erforderlichen Parameter zum Veröffentlichen des neu erstellten Bots enthält.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1888">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="15ad5-1889">`"WEBSITE_NODE_DEFAULT_VERSION"` in der ARM-Vorlage wurde so aktualisiert, dass v4-SDK-Bots 10.14.1 anstelle von 8.9.4 verwenden.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1889">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="15ad5-1890">Key Vault</span><span class="sxs-lookup"><span data-stu-id="15ad5-1890">Key Vault</span></span>
* <span data-ttu-id="15ad5-1891">Ein Problem mit `keyvault secret backup` wurde behoben, aufgrund dessen einige Benutzer bei Verwendung von `--id` einen `unexpected_keyword`-Fehler erhielten.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1891">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="15ad5-1892">Überwachen</span><span class="sxs-lookup"><span data-stu-id="15ad5-1892">Monitor</span></span>
* <span data-ttu-id="15ad5-1893">`monitor metrics alert [create|update]` wurde so geändert, dass der Dimensionswert `*` zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1893">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="15ad5-1894">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="15ad5-1894">Network</span></span>
* <span data-ttu-id="15ad5-1895">`dns zone export` wurde geändert, um sicherzustellen, dass es sich bei exportierten CNAMEs um FQDNs handelt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1895">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="15ad5-1896">Parameter `--gateway-name` wurde zu `nic ip-config address-pool [add|remove]` hinzugefügt, um Back-End-Adresspools von Anwendungsgateways zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1896">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="15ad5-1897">Argumente `--traffic-analytics` und `--workspace` wurden zu `network watcher flow-log configure` hinzugefügt, um Datenverkehrsanalysen über einen Log Analytics-Arbeitsbereich zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1897">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="15ad5-1898">`--idle-timeout` und `--floating-ip` wurden zu `lb inbound-nat-pool [create|update]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1898">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="15ad5-1899">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="15ad5-1899">Policy Insights</span></span>
* <span data-ttu-id="15ad5-1900">`policy remediation`-Befehle wurden hinzugefügt, um Korrekturfunktionen der Ressourcenrichtlinie zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1900">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="15ad5-1901">RDBMS</span><span class="sxs-lookup"><span data-stu-id="15ad5-1901">RDBMS</span></span>
* <span data-ttu-id="15ad5-1902">Hilfemeldung und Befehlsparameter wurden verbessert.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1902">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="15ad5-1903">Redis</span><span class="sxs-lookup"><span data-stu-id="15ad5-1903">Redis</span></span>
* <span data-ttu-id="15ad5-1904">Befehle zum Verwalten von „firewall-rules“ (erstellen, aktualisieren, löschen, anzeigen, auflisten) wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1904">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="15ad5-1905">Befehle zum Verwalten von „server-link“ (erstellen, aktualisieren, löschen, anzeigen, auflisten) wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1905">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="15ad5-1906">Befehle zum Verwalten von „patch-schedule“ (erstellen, aktualisieren, löschen, anzeigen, auflisten) wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1906">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="15ad5-1907">Unterstützung für Verfügbarkeitszonen und TLS-Mindestversion wurden zu „redis create“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1907">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="15ad5-1908">[BREAKING CHANGE] Befehle `redis update-settings` und `redis list-all` wurden entfernt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1908">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="15ad5-1909">[BREAKING CHANGE] Parameter für `redis create`: „Mandanteneinstellungen“ werden im Format „Schlüssel[=Wert] nicht akzeptiert.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1909">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="15ad5-1910">[VERALTET] Warnmeldung zur Markierung des Befehls `redis import-method` als veraltet hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1910">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="15ad5-1911">Role</span><span class="sxs-lookup"><span data-stu-id="15ad5-1911">Role</span></span>
* <span data-ttu-id="15ad5-1912">[BREAKING CHANGE] Befehl `az identity` wurde aus den `vm`-Befehlen hierher verschoben.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1912">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="15ad5-1913">SQL-VM</span><span class="sxs-lookup"><span data-stu-id="15ad5-1913">SQL VM</span></span>
* <span data-ttu-id="15ad5-1914">[VERALTET] Argument `--boostrap-acc-pwd` aufgrund eines Tippfehlers als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-1914">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="15ad5-1915">VM</span><span class="sxs-lookup"><span data-stu-id="15ad5-1915">VM</span></span>
* <span data-ttu-id="15ad5-1916">`vm list-skus` wurde so geändert, dass `--all` anstelle von `--all true` verwendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1916">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="15ad5-1917">`vmss run-command [invoke | list | show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1917">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="15ad5-1918">Ein Fehler wurde behoben, aufgrund dessen bei der Ausführung von `vmss encryption enable` bisher ein Fehler auftrat.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1918">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="15ad5-1919">[BREAKING CHANGE] Die Befehle vom Typ `az identity` wurden zu `role`-Befehlen verschoben.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1919">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="15ad5-1920">31. Januar 2019</span><span class="sxs-lookup"><span data-stu-id="15ad5-1920">January 31, 2019</span></span>

<span data-ttu-id="15ad5-1921">Version 2.0.57</span><span class="sxs-lookup"><span data-stu-id="15ad5-1921">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="15ad5-1922">Core</span><span class="sxs-lookup"><span data-stu-id="15ad5-1922">Core</span></span>

* <span data-ttu-id="15ad5-1923">Hotfix für [Problem 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="15ad5-1923">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="15ad5-1924">28. Januar 2019</span><span class="sxs-lookup"><span data-stu-id="15ad5-1924">January 28, 2019</span></span>

<span data-ttu-id="15ad5-1925">Version 2.0.56</span><span class="sxs-lookup"><span data-stu-id="15ad5-1925">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="15ad5-1926">ACR</span><span class="sxs-lookup"><span data-stu-id="15ad5-1926">ACR</span></span>
* <span data-ttu-id="15ad5-1927">Unterstützung für VNet/IP-Regeln wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1927">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="15ad5-1928">ACS</span><span class="sxs-lookup"><span data-stu-id="15ad5-1928">ACS</span></span>
* <span data-ttu-id="15ad5-1929">Virtuelle Knoten (Vorschau) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1929">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="15ad5-1930">Verwaltete OpenShift-Befehle wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1930">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="15ad5-1931">Unterstützung für den Dienstprinzipal-Updatevorgang mit `aks update-credentials -reset-service-principal` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1931">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="15ad5-1932">AMS</span><span class="sxs-lookup"><span data-stu-id="15ad5-1932">AMS</span></span>
* <span data-ttu-id="15ad5-1933">[BREAKING CHANGE]`ams asset get-streaming-locators` in `ams asset list-streaming-locators` umbenannt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1933">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="15ad5-1934">[BREAKING CHANGE]`ams streaming-locator get-content-keys` in `ams streaming-locator list-content-keys` umbenannt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1934">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="15ad5-1935">AppService</span><span class="sxs-lookup"><span data-stu-id="15ad5-1935">Appservice</span></span>
* <span data-ttu-id="15ad5-1936">Unterstützung für App-Erkenntnisse in `functionapp create` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1936">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="15ad5-1937">Unterstützung für die Erstellung von App Service-Plänen (einschließlich Elastic Premium) wurde zu Funktions-Apps hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1937">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="15ad5-1938">Probleme bei einer App-Einstellung mit Elastic Premium-Plänen wurden behoben.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1938">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="15ad5-1939">Container</span><span class="sxs-lookup"><span data-stu-id="15ad5-1939">Container</span></span>
* <span data-ttu-id="15ad5-1940">Befehl `container start` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1940">Added `container start` command</span></span>
* <span data-ttu-id="15ad5-1941">Eine Änderung wurde vorgenommen, um bei der Containererstellung die Verwendung von Dezimalwerten für die CPU zuzulassen.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1941">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="15ad5-1942">EventGrid</span><span class="sxs-lookup"><span data-stu-id="15ad5-1942">EventGrid</span></span>
* <span data-ttu-id="15ad5-1943">Parameter `--deadletter-endpoint` zu `event-subscription [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1943">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="15ad5-1944">„storagequeue“ und „hybridconnection“ wurden als neue Werte für „event-subscription [create|update] --endpoint-type“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1944">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="15ad5-1945">Parameter `--max-delivery-attempts` und `--event-ttl` wurden zu `event-subscription create` hinzugefügt, um die Wiederholungsrichtlinie für Ereignisse anzugeben.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1945">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="15ad5-1946">Eine Warnmeldung wurde zu `event-subscription [create|update]` hinzugefügt, wenn Webhook als Ziel für ein Ereignisabonnement verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1946">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="15ad5-1947">Parameter „source-resource-id“ wurde für alle Befehle im Zusammenhang mit Ereignisabonnements hinzugefügt, und alle anderen Parameter im Zusammenhang mit Quellressourcen wurden als veraltet markiert.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1947">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="15ad5-1948">HDInsight</span><span class="sxs-lookup"><span data-stu-id="15ad5-1948">HDInsight</span></span>
* <span data-ttu-id="15ad5-1949">[BREAKING CHANGE] Die Parameter `--virtual-network` und `--subnet-name` wurden aus `hdinsight [application] create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1949">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="15ad5-1950">[BREAKING CHANGE]`hdinsight create --storage-account` wurde so geändert, dass der Name oder die ID eines Speicherkontos anstellen von Blobendpunkten akzeptiert wird.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1950">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="15ad5-1951">Parameter `--vnet-name` und `--subnet-name` zu `hdinsight create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1951">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="15ad5-1952">Unterstützung für das Enterprise-Sicherheitspaket und Datenträgerverschlüsselung wurde zu `hdinsight create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1952">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="15ad5-1953">Befehl `hdinsight rotate-disk-encryption-key` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1953">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="15ad5-1954">Befehl `hdinsight update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1954">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="15ad5-1955">IoT</span><span class="sxs-lookup"><span data-stu-id="15ad5-1955">IoT</span></span>
* <span data-ttu-id="15ad5-1956">Codierungsformat wurde zu Befehl „routing-endpoint“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1956">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="15ad5-1957">Kusto</span><span class="sxs-lookup"><span data-stu-id="15ad5-1957">Kusto</span></span>
* <span data-ttu-id="15ad5-1958">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="15ad5-1958">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="15ad5-1959">Überwachen</span><span class="sxs-lookup"><span data-stu-id="15ad5-1959">Monitor</span></span>
* <span data-ttu-id="15ad5-1960">ID-Vergleich wurde so geändert, dass Groß-/Kleinschreibung nicht mehr beachtet wird.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1960">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="15ad5-1961">Profil</span><span class="sxs-lookup"><span data-stu-id="15ad5-1961">Profile</span></span>
* <span data-ttu-id="15ad5-1962">Konto auf Mandantenebene für verwaltete Dienstidentität für `login` wird aktiviert.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1962">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="15ad5-1963">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="15ad5-1963">Network</span></span>
* <span data-ttu-id="15ad5-1964">Ein Problem mit `express-route update` wurde behoben, aufgrund dessen das Argument `--bandwidth` ignoriert wurde.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1964">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="15ad5-1965">Ein Problem mit `ddos-protection update` wurde behoben, aufgrund dessen das festgelegte Verständnis zu einer Stapelüberwachung führte.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1965">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="15ad5-1966">Resource</span><span class="sxs-lookup"><span data-stu-id="15ad5-1966">Resource</span></span>
* <span data-ttu-id="15ad5-1967">Unterstützung für die URI-Parameterdatei wurde zu `group deployment create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1967">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="15ad5-1968">Unterstützung für verwaltete Identitäten wurde zu `policy assignment [create|list|show]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1968">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="15ad5-1969">Virtueller SQL-Computer</span><span class="sxs-lookup"><span data-stu-id="15ad5-1969">SQL Virtual Machine</span></span>
* <span data-ttu-id="15ad5-1970">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="15ad5-1970">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="15ad5-1971">Storage</span><span class="sxs-lookup"><span data-stu-id="15ad5-1971">Storage</span></span>
* <span data-ttu-id="15ad5-1972">Eine Lösung wurde so geändert, dass nur Eigenschaften aktualisiert werden, die im selben Objekt geändert werden.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1972">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="15ad5-1973">Nr. 8021 wurde korrigiert, Binärdaten werden bei der Rückgabe in Base64 codiert.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1973">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="15ad5-1974">VM</span><span class="sxs-lookup"><span data-stu-id="15ad5-1974">VM</span></span>
* <span data-ttu-id="15ad5-1975">`vm encryption enable` wurde geändert, um den Schlüsseltresor für die Datenträgerverschlüsselung zu überprüfen und sicherzustellen, dass der Schlüsseltresor für die Schlüsselverschlüsselung vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1975">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="15ad5-1976">Flag `--force` wurde zu `vm encryption enable` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1976">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="15ad5-1977">15. Januar 2019</span><span class="sxs-lookup"><span data-stu-id="15ad5-1977">January 15, 2019</span></span>

<span data-ttu-id="15ad5-1978">Version 2.0.55</span><span class="sxs-lookup"><span data-stu-id="15ad5-1978">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="15ad5-1979">ACR</span><span class="sxs-lookup"><span data-stu-id="15ad5-1979">ACR</span></span>
* <span data-ttu-id="15ad5-1980">Wurde geändert, um den Push eines nicht vorhandenen Helm-Diagramms zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1980">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="15ad5-1981">Wurde geändert, um Laufzeitvorgänge ohne ARM-Anforderungen zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1981">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="15ad5-1982">[VERALTET] Parameter `--resource-group` in folgenden Befehlen als veraltet markiert:</span><span class="sxs-lookup"><span data-stu-id="15ad5-1982">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="15ad5-1983">ACS</span><span class="sxs-lookup"><span data-stu-id="15ad5-1983">ACS</span></span>
* <span data-ttu-id="15ad5-1984">Unterstützung für neue ACI-Regionen wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1984">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="15ad5-1985">AppService</span><span class="sxs-lookup"><span data-stu-id="15ad5-1985">Appservice</span></span>
* <span data-ttu-id="15ad5-1986">Ein Problem beim Hochladen von Zertifikaten für in einer ASE gehostete Apps wurde behoben, aufgrund dessen die AS-RG und die App-RG nicht übereinstimmten.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1986">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="15ad5-1987">`webapp up` wurde geändert, sodass SKU P1V1 als Standard für Linux verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1987">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="15ad5-1988">`[webapp|functionapp] deployment source config-zip` wurde korrigiert, sodass beim Fehlschlagen einer Bereitstellung die richtige Fehlermeldung angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1988">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="15ad5-1989">Befehl `webapp ssh` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-1989">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="15ad5-1990">Botservice</span><span class="sxs-lookup"><span data-stu-id="15ad5-1990">Botservice</span></span>
* <span data-ttu-id="15ad5-1991">Aktualisierungen des Bereitstellungsstatus wurden zu `bot create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1991">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="15ad5-1992">Konfigurieren</span><span class="sxs-lookup"><span data-stu-id="15ad5-1992">Configure</span></span>
* <span data-ttu-id="15ad5-1993">`none` wurde als konfigurierbares Ausgabeformat hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1993">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="15ad5-1994">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="15ad5-1994">CosmosDB</span></span>
* <span data-ttu-id="15ad5-1995">Unterstützung für das Erstellen einer Datenbank mit gemeinsam genutztem Durchsatz wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1995">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="15ad5-1996">HDInsight</span><span class="sxs-lookup"><span data-stu-id="15ad5-1996">HDInsight</span></span>
* <span data-ttu-id="15ad5-1997">Befehle zum Verwalten von Anwendungen wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1997">Added commands for managing applications</span></span>
* <span data-ttu-id="15ad5-1998">Befehle zum Verwalten von Skriptaktionen wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1998">Added commands for managing script actions</span></span>
* <span data-ttu-id="15ad5-1999">Befehle zum Verwalten von der Operations Management Suite (OMS) wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-1999">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="15ad5-2000">Unterstützung zum Auflisten der regionalen Nutzung wurde zu `hdinsight list-usage` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2000">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="15ad5-2001">[BREAKING CHANGE] Standardclustertyp wurde aus `hdinsight create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2001">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="15ad5-2002">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="15ad5-2002">Network</span></span>
* <span data-ttu-id="15ad5-2003">Argumente `--custom-headers` und `--status-code-ranges` zu `traffic-manager profile [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2003">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="15ad5-2004">Neue Routingtypen wurden hinzugefügt: Subnetz und MultiValue</span><span class="sxs-lookup"><span data-stu-id="15ad5-2004">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="15ad5-2005">Argumente `--custom-headers` und `--subnets` zu `traffic-manager endpoint [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2005">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="15ad5-2006">Eine Problem wurde behoben, aufgrund dessen die Angabe von `--vnets ""` für `ddos-protection update` einen Fehler verursacht hat.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2006">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="15ad5-2007">Role</span><span class="sxs-lookup"><span data-stu-id="15ad5-2007">Role</span></span>
* <span data-ttu-id="15ad5-2008">[VERALTET] Argument `--password` als veraltet markiert für `create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2008">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="15ad5-2009">Verwenden Sie stattdessen sichere, von der CLI generierte Kennwörter.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2009">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="15ad5-2010">Sicherheit</span><span class="sxs-lookup"><span data-stu-id="15ad5-2010">Security</span></span>
* <span data-ttu-id="15ad5-2011">Erstrelease</span><span class="sxs-lookup"><span data-stu-id="15ad5-2011">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="15ad5-2012">Storage</span><span class="sxs-lookup"><span data-stu-id="15ad5-2012">Storage</span></span>
* <span data-ttu-id="15ad5-2013">[BREAKING CHANGE] Die Standardanzahl von Ergebnissen wurde für `storage [blob|file|container|share] list` in 5.000 geändert.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2013">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="15ad5-2014">Verwenden Sie `--num-results *` für das ursprüngliche Verhalten, alle Ergebnisse zurückzugeben.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2014">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="15ad5-2015">Parameter `--marker` zu `storage [blob|file|container|share] list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2015">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="15ad5-2016">Ein Protokollmarker für die nächste Seite wurde zur STDERR für `storage [blob|file|container|share] list` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2016">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="15ad5-2017">Der Befehl `storage blob service-properties update` mit Unterstützung für statische Websites wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2017">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="15ad5-2018">VM</span><span class="sxs-lookup"><span data-stu-id="15ad5-2018">VM</span></span>
* <span data-ttu-id="15ad5-2019">`vm [disk|unmanaged-disk]` und `vmss disk` wurden geändert, sodass sie konsistentere Parameter enthalten.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2019">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="15ad5-2020">Unterstützung für mandantenübergreifende Imageverweise wurden zu `[vm|vmss] create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2020">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="15ad5-2021">Fehler bei Standardkonfiguration in `vm diagnostics get-default-config --windows-os` wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2021">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="15ad5-2022">Argument `--provision-after-extensions` wurde zu `vmss extension set` hinzugefügt, um zu definieren, welche Erweiterungen vor dem Festlegen der Erweiterung bereitgestellt werden müssen.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2022">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="15ad5-2023">Argument `--replica-count` wurde zu `sig image-version update` hinzugefügt, um die Standardanzahl für die Replikation festzulegen.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2023">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="15ad5-2024">Fehler bei `image create --source` wurde behoben, aufgrund dessen, der Quellbetriebssystem-Datenträger für einen virtuellen Computer mit dem gleichen Namen gehalten wurde, selbst wenn die vollständige Ressourcen-ID angegeben war.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2024">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="15ad5-2025">20. Dezember 2018</span><span class="sxs-lookup"><span data-stu-id="15ad5-2025">December 20, 2018</span></span>

<span data-ttu-id="15ad5-2026">Version 2.0.54</span><span class="sxs-lookup"><span data-stu-id="15ad5-2026">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="15ad5-2027">AppService</span><span class="sxs-lookup"><span data-stu-id="15ad5-2027">Appservice</span></span>
* <span data-ttu-id="15ad5-2028">Problem behoben, bei dem `webapp up` nicht erneut bereitgestellt werden konnte</span><span class="sxs-lookup"><span data-stu-id="15ad5-2028">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="15ad5-2029">Unterstützung für das Auflisten und Wiederherstellen von Web-App-Momentaufnahmen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2029">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="15ad5-2030">Unterstützung für das Flag `--runtime` zu Windows-Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2030">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="15ad5-2031">IoTCentral</span><span class="sxs-lookup"><span data-stu-id="15ad5-2031">IoTCentral</span></span>
* <span data-ttu-id="15ad5-2032">Fehler bei API-Aufruf für update-Befehl behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-2032">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="15ad5-2033">Role</span><span class="sxs-lookup"><span data-stu-id="15ad5-2033">Role</span></span>
* <span data-ttu-id="15ad5-2034">[BREAKING CHANGE]`ad [app|sp] list` geändert, damit standardmäßig nur die ersten 100 Objekte aufgelistet werden</span><span class="sxs-lookup"><span data-stu-id="15ad5-2034">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="15ad5-2035">SQL</span><span class="sxs-lookup"><span data-stu-id="15ad5-2035">SQL</span></span>
* <span data-ttu-id="15ad5-2036">Unterstützung für die benutzerdefinierte Sortierung auf verwalteten Instanzen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2036">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="15ad5-2037">VM</span><span class="sxs-lookup"><span data-stu-id="15ad5-2037">VM</span></span>
* <span data-ttu-id="15ad5-2038">Parameter `---os-type` zu `disk create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2038">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="15ad5-2039">18. Dezember 2018</span><span class="sxs-lookup"><span data-stu-id="15ad5-2039">December 18, 2018</span></span>

<span data-ttu-id="15ad5-2040">Version 2.0.53</span><span class="sxs-lookup"><span data-stu-id="15ad5-2040">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="15ad5-2041">ACR</span><span class="sxs-lookup"><span data-stu-id="15ad5-2041">ACR</span></span>
* <span data-ttu-id="15ad5-2042">Unterstützung für Imageimport aus externen Containerregistrierungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2042">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="15ad5-2043">Tabellenlayout für Aufgabenliste komprimiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-2043">Condensed the table layout for task list</span></span>
* <span data-ttu-id="15ad5-2044">Unterstützung für Azure DevOps-URLs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2044">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="15ad5-2045">ACS</span><span class="sxs-lookup"><span data-stu-id="15ad5-2045">ACS</span></span>
* <span data-ttu-id="15ad5-2046">Virtuelle Knoten (Vorschau) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2046">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="15ad5-2047">„(PREVIEW)“ aus AAD-Argumenten für `aks create` entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2047">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="15ad5-2048">[VERALTET]`az acs`-Befehle als veraltet markiert.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2048">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="15ad5-2049">ACS wird am 31. Januar 2020 eingestellt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2049">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="15ad5-2050">Unterstützung für Netzwerkrichtlinie bei der Erstellung neuer AKS-Cluster hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2050">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="15ad5-2051">Anforderung des Arguments `--nodepool-name` bei nur einem Knotenpool für `aks scale` entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2051">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="15ad5-2052">AppService</span><span class="sxs-lookup"><span data-stu-id="15ad5-2052">Appservice</span></span>
* <span data-ttu-id="15ad5-2053">Problem behoben, bei dem für `webapp config container` der Parameter `--slot` nicht berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="15ad5-2053">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="15ad5-2054">Botservice</span><span class="sxs-lookup"><span data-stu-id="15ad5-2054">Botservice</span></span>
* <span data-ttu-id="15ad5-2055">Unterstützung für Analyse von `.bot`-Dateien beim Aufrufen von `bot show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2055">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="15ad5-2056">Fehler bei der AppInsights-Bereitstellung behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-2056">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="15ad5-2057">Leerzeichenfehler bei Dateipfaden behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-2057">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="15ad5-2058">Kudu-Netzwerkaufrufe reduziert</span><span class="sxs-lookup"><span data-stu-id="15ad5-2058">Reduced Kudu network calls</span></span>
* <span data-ttu-id="15ad5-2059">Allgemeine Verbesserungen bei Befehlen der Benutzeroberfläche durchgeführt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2059">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="15ad5-2060">Nutzung</span><span class="sxs-lookup"><span data-stu-id="15ad5-2060">Consumption</span></span>
* <span data-ttu-id="15ad5-2061">Fehler für Budget-API zum Anzeigen von Benachrichtigungen behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-2061">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="15ad5-2062">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="15ad5-2062">CosmosDB</span></span>
* <span data-ttu-id="15ad5-2063">Unterstützung für die Aktualisierung des Kontos von „Singlemaster“ auf „Multimaster“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2063">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="15ad5-2064">Karten</span><span class="sxs-lookup"><span data-stu-id="15ad5-2064">Maps</span></span>
* <span data-ttu-id="15ad5-2065">Unterstützung für SKU „S1“ für `maps account [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2065">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="15ad5-2066">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="15ad5-2066">Network</span></span>
* <span data-ttu-id="15ad5-2067">Unterstützung für `--format` und `--log-version` für `watcher flow-log configure` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2067">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="15ad5-2068">Problem mit `dns zone update` behoben, bei dem die Verwendung von "" zum Löschen von Auflösungs- und Registrierungs-VNETs nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="15ad5-2068">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="15ad5-2069">Resource</span><span class="sxs-lookup"><span data-stu-id="15ad5-2069">Resource</span></span>
* <span data-ttu-id="15ad5-2070">Verarbeitung des Bereichsparameters für Verwaltungsgruppen in `policy assignment [create|list|delete|show|update]` behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-2070">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="15ad5-2071">Neuen Befehl `resource wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2071">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="15ad5-2072">Storage</span><span class="sxs-lookup"><span data-stu-id="15ad5-2072">Storage</span></span>
*  <span data-ttu-id="15ad5-2073">Möglichkeit zum Aktualisieren der Protokollschemaversion für Speicherdienste in `storage logging update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2073">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="15ad5-2074">VM</span><span class="sxs-lookup"><span data-stu-id="15ad5-2074">VM</span></span>
* <span data-ttu-id="15ad5-2075">Absturz in `vm identity remove` behoben, der aufgetreten ist, wenn der angegebenen VM keine verwalteten Dienstidentitäten zugewiesen waren</span><span class="sxs-lookup"><span data-stu-id="15ad5-2075">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="15ad5-2076">4\. Dezember 2018</span><span class="sxs-lookup"><span data-stu-id="15ad5-2076">December 4, 2018</span></span>

<span data-ttu-id="15ad5-2077">Version 2.0.52</span><span class="sxs-lookup"><span data-stu-id="15ad5-2077">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="15ad5-2078">Core</span><span class="sxs-lookup"><span data-stu-id="15ad5-2078">Core</span></span>
* <span data-ttu-id="15ad5-2079">Unterstützung für mandantenübergreifende Ressourcenbereitstellung für mehrinstanzenfähigen Dienstprinzipal hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2079">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="15ad5-2080">Behebung eines Fehlers, aufgrund dessen IDs, die von einem Befehl mit Ausgabe im TSV-Format weitergeleitet wurden, nicht ordnungsgemäß analysiert wurden</span><span class="sxs-lookup"><span data-stu-id="15ad5-2080">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="15ad5-2081">AppService</span><span class="sxs-lookup"><span data-stu-id="15ad5-2081">Appservice</span></span>
* <span data-ttu-id="15ad5-2082">[VORSCHAU] Befehl `webapp up` hinzugefügt, der Benutzer beim Erstellen und Bereitstellen von Inhalten in Apps unterstützt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2082">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="15ad5-2083">Behebung eines Fehlers in einer containerbasierten Windows-App, der aufgrund einer Back-End-Änderung auftrat</span><span class="sxs-lookup"><span data-stu-id="15ad5-2083">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="15ad5-2084">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="15ad5-2084">Network</span></span>
* <span data-ttu-id="15ad5-2085">Argument `--exclusion` zu `application-gateway waf-config set` hinzugefügt, um WAF-Ausschlüsse zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="15ad5-2085">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="15ad5-2086">Role</span><span class="sxs-lookup"><span data-stu-id="15ad5-2086">Role</span></span>
* <span data-ttu-id="15ad5-2087">Unterstützung für benutzerdefinierte Bezeichner für Kennwortanmeldeinformation hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2087">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="15ad5-2088">VM</span><span class="sxs-lookup"><span data-stu-id="15ad5-2088">VM</span></span>
* <span data-ttu-id="15ad5-2089">[VERALTET] Parameter `vm extension [show|wait] --expand` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-2089">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="15ad5-2090">Parameter `--force` zu `vm restart` hinzugefügt, um nicht reagierende virtuelle Computer erneut bereitzustellen</span><span class="sxs-lookup"><span data-stu-id="15ad5-2090">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="15ad5-2091">`[vm|vmss] create --authentication-type` geändert, um „all“ zu akzeptieren und einen virtuellen Computer mit Kennwort- und SSH-Authentifizierung zu erstellen</span><span class="sxs-lookup"><span data-stu-id="15ad5-2091">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="15ad5-2092">Parameter `image create --os-disk-caching` hinzugefügt, um die Zwischenspeicherung von Betriebssystemdatenträgern für ein Image festzulegen</span><span class="sxs-lookup"><span data-stu-id="15ad5-2092">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="15ad5-2093">20. November 2018</span><span class="sxs-lookup"><span data-stu-id="15ad5-2093">November 20, 2018</span></span>

<span data-ttu-id="15ad5-2094">Version 2.0.51</span><span class="sxs-lookup"><span data-stu-id="15ad5-2094">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="15ad5-2095">Core</span><span class="sxs-lookup"><span data-stu-id="15ad5-2095">Core</span></span>
* <span data-ttu-id="15ad5-2096">MSI-Anmeldung geändert, sodass der Abonnementname nicht in der Identität wiederverwendet wird</span><span class="sxs-lookup"><span data-stu-id="15ad5-2096">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="15ad5-2097">ACR</span><span class="sxs-lookup"><span data-stu-id="15ad5-2097">ACR</span></span>
* <span data-ttu-id="15ad5-2098">Kontexttoken zum Aufgabenschritt hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2098">Added context token to task step</span></span>
* <span data-ttu-id="15ad5-2099">Unterstützung für das Festlegen von Geheimnissen in „acr run“ zum Spiegeln der ACR-Aufgabe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2099">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="15ad5-2100">Unterstützung für `--top` und `--orderby` für die Befehle `show-tags` und `show-manifests` verbessert</span><span class="sxs-lookup"><span data-stu-id="15ad5-2100">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="15ad5-2101">AppService</span><span class="sxs-lookup"><span data-stu-id="15ad5-2101">Appservice</span></span>
* <span data-ttu-id="15ad5-2102">Standardtimeout der ZIP-Bereitstellung für das Abrufen des Status auf fünf Minuten erhöht und Timeout-Eigenschaft zum Anpassen dieses Werts hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2102">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="15ad5-2103">Aktualisierung der standardmäßigen `node_version`.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2103">Updated the default `node_version`.</span></span> <span data-ttu-id="15ad5-2104">Während eines Austauschvorgangs mit zwei Phasen werden bei der Austauschaktion zum Zurücksetzen des Slots alle App-Einstellungen und Verbindungszeichenfolgen beibehalten.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2104">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="15ad5-2105">Clientseitige SKU-Überprüfung für die Erstellung eines Linux-App Service-Plans entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2105">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="15ad5-2106">Behebung eines Fehlers beim Abrufen des ZipDeploy-Status</span><span class="sxs-lookup"><span data-stu-id="15ad5-2106">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="15ad5-2107">IotCentral</span><span class="sxs-lookup"><span data-stu-id="15ad5-2107">IotCentral</span></span>
* <span data-ttu-id="15ad5-2108">Verfügbarkeitsprüfung für Unterdomänen beim Erstellen einer IoT Central-Anwendung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2108">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="15ad5-2109">KeyVault</span><span class="sxs-lookup"><span data-stu-id="15ad5-2109">KeyVault</span></span>
* <span data-ttu-id="15ad5-2110">Behebung eines Fehlers, aufgrund dessen Fehler mitunter ignoriert wurden</span><span class="sxs-lookup"><span data-stu-id="15ad5-2110">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="15ad5-2111">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="15ad5-2111">Network</span></span>
* <span data-ttu-id="15ad5-2112">`root-cert`-Unterbefehle zum Behandeln von vertrauenswürdigen Stammzertifikaten zu `application-gateway` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2112">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="15ad5-2113">Optionen `--min-capacity` und `--custom-error-pages` zu `application-gateway [create|update]` hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="15ad5-2113">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="15ad5-2114">`--zones` zur Unterstützung von Verfügbarkeitszonen zu `application-gateway create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2114">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="15ad5-2115">Argumente `--file-upload-limit`, `--max-request-body-size` und `--request-body-check` zu `application-gateway waf-config set` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2115">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="15ad5-2116">Rdbms</span><span class="sxs-lookup"><span data-stu-id="15ad5-2116">Rdbms</span></span>
* <span data-ttu-id="15ad5-2117">MariaDB-VNET-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2117">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="15ad5-2118">RBAC</span><span class="sxs-lookup"><span data-stu-id="15ad5-2118">Rbac</span></span>
* <span data-ttu-id="15ad5-2119">Problem beim Aktualisieren unveränderlicher Anmeldeinformationen in `ad app update` behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-2119">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="15ad5-2120">Ausgabewarnungen zur Ankündigung bevorstehender Breaking Changes für `ad [app|sp] list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2120">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="15ad5-2121">Storage</span><span class="sxs-lookup"><span data-stu-id="15ad5-2121">Storage</span></span>
* <span data-ttu-id="15ad5-2122">Behandlung von Ausnahmefällen für Speicherkopierbefehle verbessert</span><span class="sxs-lookup"><span data-stu-id="15ad5-2122">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="15ad5-2123">Problem behoben, aufgrund dessen `storage blob copy start-batch` bei identischen Ziel- und Quellkonten keine Anmeldeinformationen verwendete</span><span class="sxs-lookup"><span data-stu-id="15ad5-2123">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="15ad5-2124">Fehler bei `storage [blob|file] url` behoben, aufgrund dessen `sas_token` nicht in die URL eingebunden wurde</span><span class="sxs-lookup"><span data-stu-id="15ad5-2124">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="15ad5-2125">Breaking Change-Warnung zu `[blob|container] list` hinzugefügt: In Kürze werden standardmäßig nur die ersten 5.000 Ergebnisse ausgegeben.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2125">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="15ad5-2126">VM</span><span class="sxs-lookup"><span data-stu-id="15ad5-2126">VM</span></span>
* <span data-ttu-id="15ad5-2127">Unterstützung für die separate Angabe einer Speicherkonto-SKU für verwaltete Betriebssystemdatenträger und Datenträger zu `[vm|vmss] create --storage-sku` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2127">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="15ad5-2128">Parameter für den Versionsnamen von `sig image-version` in `--image-version -e` geändert</span><span class="sxs-lookup"><span data-stu-id="15ad5-2128">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="15ad5-2129">`sig image-version`-Argument `--image-version-name` als veraltet markiert und durch `--image-version` ersetzt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2129">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="15ad5-2130">Unterstützung für die Verwendung des lokalen Betriebssystemdatenträgers für `[vm|vmss] create --ephemeral-os-disk` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2130">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="15ad5-2131">Unterstützung für `--no-wait` zu `snapshot create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2131">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="15ad5-2132">Befehl `snapshot wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2132">Added `snapshot wait` command</span></span>
* <span data-ttu-id="15ad5-2133">Unterstützung für die Verwendung von Instanznamen mit `[vm|vmss] extension set --extension-instance-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2133">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="15ad5-2134">6\. November 2018</span><span class="sxs-lookup"><span data-stu-id="15ad5-2134">November 6, 2018</span></span>

<span data-ttu-id="15ad5-2135">Version 2.0.50</span><span class="sxs-lookup"><span data-stu-id="15ad5-2135">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="15ad5-2136">Core</span><span class="sxs-lookup"><span data-stu-id="15ad5-2136">Core</span></span>
* <span data-ttu-id="15ad5-2137">Unterstützung für die Dienstprinzipalauthentifizierung (SN und Aussteller) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2137">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="15ad5-2138">ACR</span><span class="sxs-lookup"><span data-stu-id="15ad5-2138">ACR</span></span>
* <span data-ttu-id="15ad5-2139">Unterstützung für Commit- und Pull Request-Git-Ereignisse für Aufgabenquellentrigger hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2139">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="15ad5-2140">Auf Verwendung des Standard-Dockerfiles umgestellt, falls im Erstellungsbefehl kein Dockerfile angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="15ad5-2140">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="15ad5-2141">ACS</span><span class="sxs-lookup"><span data-stu-id="15ad5-2141">ACS</span></span>
* <span data-ttu-id="15ad5-2142">[BREAKING CHANGE]`enable_cloud_console_aks_browse` entfernt, um standardmäßig „az aks browse“ zu aktivieren</span><span class="sxs-lookup"><span data-stu-id="15ad5-2142">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="15ad5-2143">Advisor</span><span class="sxs-lookup"><span data-stu-id="15ad5-2143">Advisor</span></span>
* <span data-ttu-id="15ad5-2144">Allgemein verfügbares Release</span><span class="sxs-lookup"><span data-stu-id="15ad5-2144">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="15ad5-2145">AMS</span><span class="sxs-lookup"><span data-stu-id="15ad5-2145">AMS</span></span>
* <span data-ttu-id="15ad5-2146">Neue Befehlsgruppen hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="15ad5-2146">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="15ad5-2147">Neue Befehle hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="15ad5-2147">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="15ad5-2148">Unterstützung von Verschlüsselungsparametern für `ams streaming-policy create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2148">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="15ad5-2149">Für `ams transform output remove` kann jetzt der zu entfernende Ausgabeindex angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2149">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="15ad5-2150">Argumente `--correlation-data` und `--label` zur Befehlsgruppe `ams job` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2150">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="15ad5-2151">Argumente `--storage-account` und `--container` zur Befehlsgruppe `ams asset` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2151">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="15ad5-2152">Standardwerte für Ablaufzeit (aktueller Zeitpunkt + 23 Std.) und Berechtigungen (Lesen) im Befehl `ams asset get-sas-url` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2152">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="15ad5-2153">[BREAKING CHANGE] Befehl `ams streaming locator` durch `ams streaming-locator` ersetzt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2153">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="15ad5-2154">[BREAKING CHANGE] Argument `--content-keys` von `ams streaming locator` aktualisiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-2154">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="15ad5-2155">[BREAKING CHANGE]`--content-policy-name` im Befehl `ams streaming locator` in `--content-key-policy-name` umbenannt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2155">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="15ad5-2156">[BREAKING CHANGE] Befehl `ams streaming policy` durch `ams streaming-policy` ersetzt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2156">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="15ad5-2157">[BREAKING CHANGE] Das Argument `--preset-names` wurde in der Befehlsgruppe `--preset` durch `ams transform` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2157">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="15ad5-2158">Ab sofort kann nur noch eine einzelne Ausgabe/Voreinstellung festgelegt werden. (Wenn Sie weitere hinzufügen möchten, müssen Sie `ams transform output add` ausführen.)</span><span class="sxs-lookup"><span data-stu-id="15ad5-2158">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="15ad5-2159">Darüber hinaus können Sie eine benutzerdefinierte Voreinstellung für den Standard-Encoder (StandardEncoderPreset) festlegen, indem Sie den Pfad an Ihr benutzerdefiniertes JSON-Objekt übergeben.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2159">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="15ad5-2160">[BREAKING CHANGE]`--output-asset-names ` wurde im Befehl `ams job start` in `--output-assets` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2160">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="15ad5-2161">Ab sofort wird eine durch Leerzeichen getrennte Ressourcenliste im Format „assetName=Bezeichnung“ akzeptiert.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2161">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="15ad5-2162">Ressourcen ohne Bezeichnung können wie folgt gesendet werden: „assetName=“.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2162">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="15ad5-2163">AppService</span><span class="sxs-lookup"><span data-stu-id="15ad5-2163">AppService</span></span>
* <span data-ttu-id="15ad5-2164">Fehler in `az webapp config backup update` behoben, der dazu führte, dass kein Sicherungszeitplan festgelegt werden konnte, wenn noch keiner festgelegt war</span><span class="sxs-lookup"><span data-stu-id="15ad5-2164">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="15ad5-2165">Konfigurieren</span><span class="sxs-lookup"><span data-stu-id="15ad5-2165">Configure</span></span>
* <span data-ttu-id="15ad5-2166">YAML zu Ausgabeformatoptionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2166">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="15ad5-2167">Container</span><span class="sxs-lookup"><span data-stu-id="15ad5-2167">Container</span></span>
* <span data-ttu-id="15ad5-2168">Auf Anzeige der Identität umgestellt, wenn eine Containergruppe nach YAML exportiert wird</span><span class="sxs-lookup"><span data-stu-id="15ad5-2168">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="15ad5-2169">EventHub</span><span class="sxs-lookup"><span data-stu-id="15ad5-2169">EventHub</span></span>
* <span data-ttu-id="15ad5-2170">Flag `--enable-kafka` hinzugefügt, um Kafka in `eventhub namespace [create|update]` zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="15ad5-2170">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="15ad5-2171">Interactive</span><span class="sxs-lookup"><span data-stu-id="15ad5-2171">Interactive</span></span>
* <span data-ttu-id="15ad5-2172">Interactive installiert nun die Erweiterung `interactive`, um schnellere Updates und schnelleren Support zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="15ad5-2172">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="15ad5-2173">Überwachen</span><span class="sxs-lookup"><span data-stu-id="15ad5-2173">Monitor</span></span>
* <span data-ttu-id="15ad5-2174">Unterstützung für Metriknamen mit Schrägstrichen und Punkten zu `--condition` in `monitor metrics alert [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2174">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="15ad5-2175">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="15ad5-2175">Network</span></span>
* <span data-ttu-id="15ad5-2176">Befehlsnamen vom Typ `network interface-endpoint` zugunsten von `network private-endpoint` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-2176">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="15ad5-2177">Problem behoben, das dazu führte, dass das Argument `--peer-circuit` in `express-route peering connection create` keine ID akzeptiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-2177">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="15ad5-2178">Problem behoben, das dazu führte, dass `--ip-tags` mit `public-ip create` nicht ordnungsgemäß funktioniert</span><span class="sxs-lookup"><span data-stu-id="15ad5-2178">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="15ad5-2179">Profil</span><span class="sxs-lookup"><span data-stu-id="15ad5-2179">Profile</span></span>
* <span data-ttu-id="15ad5-2180">`--use-cert-sn-issuer` zu `az login` hinzugefügt, um Dienstprinzipalanmeldungen mit automatischem Zertifikatrollover zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="15ad5-2180">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="15ad5-2181">RDBMS</span><span class="sxs-lookup"><span data-stu-id="15ad5-2181">RDBMS</span></span>
* <span data-ttu-id="15ad5-2182">MySQL-Replikatbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2182">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="15ad5-2183">Resource</span><span class="sxs-lookup"><span data-stu-id="15ad5-2183">Resource</span></span>
* <span data-ttu-id="15ad5-2184">Unterstützung für Verwaltungsgruppen und Abonnements zu Befehlen vom Typ `policy definition|set-definition` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2184">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="15ad5-2185">Role</span><span class="sxs-lookup"><span data-stu-id="15ad5-2185">Role</span></span>
* <span data-ttu-id="15ad5-2186">Unterstützung für die API-Berechtigungsverwaltung, den angemeldeten Benutzer und die Verwaltung von Anwendungskennwörtern und Zertifikatanmeldeinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2186">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="15ad5-2187">`ad sp create-for-rbac` geändert, um „displayName“ und Dienstprinzipalname besser unterscheiden zu können</span><span class="sxs-lookup"><span data-stu-id="15ad5-2187">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="15ad5-2188">Unterstützung der Gewährung von Berechtigungen für AAD-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2188">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="15ad5-2189">Storage</span><span class="sxs-lookup"><span data-stu-id="15ad5-2189">Storage</span></span>
* <span data-ttu-id="15ad5-2190">Möglichkeit hinzugefügt, allein mit SAS und Endpunkten (ohne Kontoname oder Schlüssel) eine Verbindung mit Speicherdiensten herzustellen, wie unter `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>` beschrieben</span><span class="sxs-lookup"><span data-stu-id="15ad5-2190">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="15ad5-2191">VM</span><span class="sxs-lookup"><span data-stu-id="15ad5-2191">VM</span></span>
* <span data-ttu-id="15ad5-2192">Argument `storage-sku` zu `image create` hinzugefügt, um das Festlegen des standardmäßigen Speicherkontotyps für das Image zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="15ad5-2192">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="15ad5-2193">Fehler für `vm resize` behoben, durch den die Option `--no-wait` einen Absturz des Befehls verursachte</span><span class="sxs-lookup"><span data-stu-id="15ad5-2193">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="15ad5-2194">Tabellenausgabeformat für `vm encryption show` geändert, um den Status anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="15ad5-2194">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="15ad5-2195">`vm secret format` geändert, um JSON/JSONC-Ausgabe erforderlich zu machen.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2195">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="15ad5-2196">Der Benutzer wird gewarnt, und es wird standardmäßig die JSON-Ausgabe verwendet, wenn ein unzulässiges Ausgabeformat ausgewählt wird.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2196">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="15ad5-2197">Argumentüberprüfung für `vm create --image` verbessert</span><span class="sxs-lookup"><span data-stu-id="15ad5-2197">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="15ad5-2198">23. Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="15ad5-2198">October 23, 2018</span></span>

<span data-ttu-id="15ad5-2199">Version 2.0.49</span><span class="sxs-lookup"><span data-stu-id="15ad5-2199">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="15ad5-2200">Core</span><span class="sxs-lookup"><span data-stu-id="15ad5-2200">Core</span></span>
* <span data-ttu-id="15ad5-2201">Problem mit `--ids` behoben, aufgrund dessen `--subscription` Vorrang vor dem Abonnement in `--ids` hatte</span><span class="sxs-lookup"><span data-stu-id="15ad5-2201">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="15ad5-2202">Ausdrückliche Warnungen hinzugefügt, wenn Parameter durch die Verwendung von `--ids` ignoriert würden</span><span class="sxs-lookup"><span data-stu-id="15ad5-2202">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="15ad5-2203">ACR</span><span class="sxs-lookup"><span data-stu-id="15ad5-2203">ACR</span></span>
* <span data-ttu-id="15ad5-2204">Problem mit der ACR Build-Codierung in Python2 behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-2204">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="15ad5-2205">CDN</span><span class="sxs-lookup"><span data-stu-id="15ad5-2205">CDN</span></span>
* <span data-ttu-id="15ad5-2206">[BREAKING CHANGE] Standardverhalten beim Zwischenspeichern der Abfragezeichenfolge von `cdn endpoint create` so geändert, dass der Standardwert nicht mehr „IgnoreQueryString“ ist.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2206">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="15ad5-2207">Er wird jetzt vom Dienst festgelegt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2207">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="15ad5-2208">Container</span><span class="sxs-lookup"><span data-stu-id="15ad5-2208">Container</span></span>
* <span data-ttu-id="15ad5-2209">`Private` als gültiger Typ für die Übergabe an „--ip-address“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2209">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="15ad5-2210">Geändert, sodass nur eine Subnetz-ID für das Einrichten eines virtuellen Netzwerks für die Containergruppe zulässig ist</span><span class="sxs-lookup"><span data-stu-id="15ad5-2210">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="15ad5-2211">Geändert, sodass das Verwenden eines VNET-Namens oder einer Ressourcen-ID zulässig ist, um die Verwendung von VNETs aus verschiedenen Ressourcengruppen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="15ad5-2211">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="15ad5-2212">`--assign-identity` hinzugefügt, um einer Containergruppe eine MSI-Identität hinzuzufügen</span><span class="sxs-lookup"><span data-stu-id="15ad5-2212">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="15ad5-2213">`--scope` hinzugefügt, um eine Rollenzuweisung für die vom System zugewiesene MSI-Identität zu erstellen</span><span class="sxs-lookup"><span data-stu-id="15ad5-2213">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="15ad5-2214">Warnung hinzugefügt, wenn eine Containergruppe mit einem Image ohne Prozess mit langer Ausführungszeit erstellt wird</span><span class="sxs-lookup"><span data-stu-id="15ad5-2214">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="15ad5-2215">Probleme mit der Tabellenausgabe für Befehle `list` und `show` behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-2215">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="15ad5-2216">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="15ad5-2216">CosmosDB</span></span>
* <span data-ttu-id="15ad5-2217">Unterstützung für `--enable-multiple-write-locations` zu `cosmosdb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2217">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="15ad5-2218">Interactive</span><span class="sxs-lookup"><span data-stu-id="15ad5-2218">Interactive</span></span>
* <span data-ttu-id="15ad5-2219">Geändert, um sicherzustellen, dass der Parameter für globales Abonnement in Parametern angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="15ad5-2219">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="15ad5-2220">IoT Central</span><span class="sxs-lookup"><span data-stu-id="15ad5-2220">IoT Central</span></span>
* <span data-ttu-id="15ad5-2221">Optionen für Vorlagen und Anzeigenamen für die Erstellung von IoT Central-Anwendungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2221">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="15ad5-2222">[BREAKING CHANGE] Unterstützung für F1-SKU entfernt; stattdessen ist die S1-SKU zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2222">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="15ad5-2223">Überwachen</span><span class="sxs-lookup"><span data-stu-id="15ad5-2223">Monitor</span></span>
* <span data-ttu-id="15ad5-2224">Änderungen an `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="15ad5-2224">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="15ad5-2225">Unterstützung für das Auflisten aller Ereignisse auf Abonnementebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2225">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="15ad5-2226">`--offset`-Parameter für das einfachere Erstellen von Zeitabfragen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2226">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="15ad5-2227">Validierung für `--start-time` und `--end-time` verbessert, um die Verwendung von mehr ISO8601-Formate und benutzerfreundlicheren datetime-Formaten zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="15ad5-2227">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="15ad5-2228">`--namespace` als Alias für veraltete Option `--resource-provider` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2228">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="15ad5-2229">`--filters` als veraltet markiert, da vom Dienst ausschließlich Werte mit stark typisierten Optionen unterstützt werden</span><span class="sxs-lookup"><span data-stu-id="15ad5-2229">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="15ad5-2230">Änderungen an `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="15ad5-2230">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="15ad5-2231">`--offset`-Parameter für das einfachere Erstellen von Zeitabfragen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2231">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="15ad5-2232">Validierung für `--start-time` und `--end-time` verbessert, um die Verwendung von mehr ISO8601-Formate und benutzerfreundlicheren datetime-Formaten zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="15ad5-2232">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="15ad5-2233">Validierung für `--event-hub`- und `--event-hub-rule`-Argumente an `monitor diagnostic-settings create` verbessert</span><span class="sxs-lookup"><span data-stu-id="15ad5-2233">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="15ad5-2234">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="15ad5-2234">Network</span></span>
* <span data-ttu-id="15ad5-2235">`--app-gateway-address-pools`- und `--gateway-name`-Argumente zu `nic create` hinzugefügt, um das Hinzufügen von Back-End-Adresspools für Anwendungsgateways zu einer NIC zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="15ad5-2235">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="15ad5-2236">`--app-gateway-address-pools`- und `--gateway-name`-Argumente zu `nic ip-config create/update` hinzugefügt, um das Hinzufügen von Back-End-Adresspools für Anwendungsgateways zu einer NIC zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="15ad5-2236">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="15ad5-2237">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="15ad5-2237">ServiceBus</span></span>
* <span data-ttu-id="15ad5-2238">Schreibgeschütztes `migration_state`-Element zu „MigrationConfigProperties“ hinzugefügt, um den aktuellen Status der Migration von Service Bus Standard- zu Premium-Namespace anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="15ad5-2238">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="15ad5-2239">SQL</span><span class="sxs-lookup"><span data-stu-id="15ad5-2239">SQL</span></span>
* <span data-ttu-id="15ad5-2240">`sql failover-group create` und `sql failover-group update` korrigiert, damit die Verwendung einer Richtlinie für manuelles Failover möglich ist</span><span class="sxs-lookup"><span data-stu-id="15ad5-2240">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="15ad5-2241">Storage</span><span class="sxs-lookup"><span data-stu-id="15ad5-2241">Storage</span></span>
* <span data-ttu-id="15ad5-2242">Formatierung der `az storage cors list`-Ausgabe korrigiert, sodass alle Elemente den richtigen Dienstschlüssel anzeigen</span><span class="sxs-lookup"><span data-stu-id="15ad5-2242">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="15ad5-2243">`--bypass-immutability-policy`-Parameter für das Löschen von durch Unveränderlichkeitsrichtlinien blockierten Containern hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2243">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="15ad5-2244">VM</span><span class="sxs-lookup"><span data-stu-id="15ad5-2244">VM</span></span>
* <span data-ttu-id="15ad5-2245">Datenträger-Zwischenspeicherungsmodus `None` für Lv/Lv2-Computerserine in `[vm|vmss] create` erzwungen</span><span class="sxs-lookup"><span data-stu-id="15ad5-2245">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="15ad5-2246">Liste der unterstützten Größen für unterstützenden Netzwerkbeschleuniger für `vm create` aktualisiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-2246">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="15ad5-2247">Stark typisierte Argumente für UltraSSD-IOPS und MBit/s-Konfigurationen für `disk create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2247">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="15ad5-2248">16. Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="15ad5-2248">October 16, 2018</span></span>

<span data-ttu-id="15ad5-2249">Version 2.0.48</span><span class="sxs-lookup"><span data-stu-id="15ad5-2249">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="15ad5-2250">VM</span><span class="sxs-lookup"><span data-stu-id="15ad5-2250">VM</span></span>
* <span data-ttu-id="15ad5-2251">SDK-Problem behoben, das ein Fehlschlagen der Homebrew-Installation verursacht hat</span><span class="sxs-lookup"><span data-stu-id="15ad5-2251">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="15ad5-2252">9\. Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="15ad5-2252">October 9, 2018</span></span>

<span data-ttu-id="15ad5-2253">Version 2.0.47</span><span class="sxs-lookup"><span data-stu-id="15ad5-2253">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="15ad5-2254">Core</span><span class="sxs-lookup"><span data-stu-id="15ad5-2254">Core</span></span>
* <span data-ttu-id="15ad5-2255">Verbesserte Fehlerbehandlung für Fehler vom Typ „Ungültige Anforderung“</span><span class="sxs-lookup"><span data-stu-id="15ad5-2255">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="15ad5-2256">ACR</span><span class="sxs-lookup"><span data-stu-id="15ad5-2256">ACR</span></span>
* <span data-ttu-id="15ad5-2257">Unterstützung für ähnliches Tabellenformat wie Helm-Client hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2257">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="15ad5-2258">ACS</span><span class="sxs-lookup"><span data-stu-id="15ad5-2258">ACS</span></span>
* <span data-ttu-id="15ad5-2259">`aks [create|scale] --nodepool-name` zum Konfigurieren des Knotenpoolnamens hinzugefügt, auf 12 Zeichen gekürzt, Standard: nodepool1</span><span class="sxs-lookup"><span data-stu-id="15ad5-2259">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="15ad5-2260">Korrektur, bei der auf „scp“ zurückgegriffen wird, wenn Parimiko nicht funktioniert</span><span class="sxs-lookup"><span data-stu-id="15ad5-2260">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="15ad5-2261">`aks create` geändert, sodass `--aad-tenant-id` nicht mehr erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="15ad5-2261">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="15ad5-2262">Verbesserte Zusammenführung von Kubernetes-Anmeldeinformationen, wenn doppelte Einträge vorhanden sind</span><span class="sxs-lookup"><span data-stu-id="15ad5-2262">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="15ad5-2263">Container</span><span class="sxs-lookup"><span data-stu-id="15ad5-2263">Container</span></span>
* <span data-ttu-id="15ad5-2264">`functionapp create` geändert, sodass das Erstellen eines Linux-Nutzungsplans mit einer bestimmten Runtime unterstützt wird</span><span class="sxs-lookup"><span data-stu-id="15ad5-2264">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="15ad5-2265">[VORSCHAUVERSION] Unterstützung für das Hosten von Web-Apps in Windows-Containern hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2265">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="15ad5-2266">Event Hub</span><span class="sxs-lookup"><span data-stu-id="15ad5-2266">Event Hub</span></span>
* <span data-ttu-id="15ad5-2267">Befehl `eventhub update` korrigiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-2267">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="15ad5-2268">[BREAKING CHANGE]`list`-Befehle geändert, sodass Fehler von Typ „NotFound(404)“ für Ressourcen mit der typische Vorgehensweise behandelt werden, anstatt eine leere Liste anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="15ad5-2268">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="15ad5-2269">Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="15ad5-2269">Extensions</span></span>
* <span data-ttu-id="15ad5-2270">Problem beim Hinzufügen einer Erweiterung behoben, die bereits installiert ist</span><span class="sxs-lookup"><span data-stu-id="15ad5-2270">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="15ad5-2271">HDInsight</span><span class="sxs-lookup"><span data-stu-id="15ad5-2271">HDInsight</span></span>
* <span data-ttu-id="15ad5-2272">Erste Veröffentlichung</span><span class="sxs-lookup"><span data-stu-id="15ad5-2272">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="15ad5-2273">IoT</span><span class="sxs-lookup"><span data-stu-id="15ad5-2273">IoT</span></span>
* <span data-ttu-id="15ad5-2274">Befehl zur Erweiterungsinstallation zu Banner bei der ersten Ausführung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2274">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="15ad5-2275">KeyVault</span><span class="sxs-lookup"><span data-stu-id="15ad5-2275">KeyVault</span></span>
* <span data-ttu-id="15ad5-2276">Geändert, sodass Key Vault-Speicherbefehle auf das aktuelle API-Profil beschränkt sind</span><span class="sxs-lookup"><span data-stu-id="15ad5-2276">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="15ad5-2277">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="15ad5-2277">Network</span></span>
* <span data-ttu-id="15ad5-2278">`network dns zone create` korrigiert: Befehl ist auch erfolgreich, wenn der Benutzer einen Standardspeicherort konfiguriert hat.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2278">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="15ad5-2279">Siehe Nr. 6052</span><span class="sxs-lookup"><span data-stu-id="15ad5-2279">See #6052</span></span>
* <span data-ttu-id="15ad5-2280">`--remote-vnet-id` für `network vnet peering create` eingestellt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2280">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="15ad5-2281">`--remote-vnet` zum `network vnet peering create`-Element hinzugefügt, das einen Namen oder eine ID akzeptiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-2281">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="15ad5-2282">Unterstützung für mehrere Subnetzpräfixe zu `network vnet create` in `--subnet-prefixes` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2282">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="15ad5-2283">Unterstützung für mehrere Subnetzpräfixe zu `network vnet subnet [create|update]` in `--address-prefixes` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2283">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="15ad5-2284">Problem mit `network application-gateway create` behoben, das die Erstellung von Gateways mit der SKU `WAF_v2` oder `Standard_v2` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="15ad5-2284">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="15ad5-2285">`--service-endpoint-policy`-Argument für Benutzerfreundlichkeit zu `network vnet subnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2285">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="15ad5-2286">Role</span><span class="sxs-lookup"><span data-stu-id="15ad5-2286">Role</span></span>
* <span data-ttu-id="15ad5-2287">Unterstützung für das Auflisten von Azure AD-App-Besitzern in `ad app owner` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2287">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="15ad5-2288">Unterstützung für das Auflisten von Azure AD-Dienstprinzipalbesitzern in `ad sp owner` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2288">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="15ad5-2289">Geändert, um sicherzustellen, dass die Erstellungs- und Aktualisierungsbefehle für die Rollendefinition Konfigurationen mit mehreren Berechtigungen akzeptieren</span><span class="sxs-lookup"><span data-stu-id="15ad5-2289">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="15ad5-2290">`ad sp create-for-rbac` geändert, um sicherzustellen, dass der Homepage-URI immer „https“ ist</span><span class="sxs-lookup"><span data-stu-id="15ad5-2290">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="15ad5-2291">Service Bus</span><span class="sxs-lookup"><span data-stu-id="15ad5-2291">Service Bus</span></span>
* <span data-ttu-id="15ad5-2292">[BREAKING CHANGE]`list`-Befehle geändert, sodass Fehler von Typ „NotFound(404)“ für Ressourcen mit der typische Vorgehensweise behandelt werden, anstatt eine leere Liste anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="15ad5-2292">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="15ad5-2293">VM</span><span class="sxs-lookup"><span data-stu-id="15ad5-2293">VM</span></span>
* <span data-ttu-id="15ad5-2294">Leeres `accessSas`-Feld in `disk grant-access` korrigiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-2294">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="15ad5-2295">`vmss create` geändert, sodass ein ausreichend großer Front-End-Portbereich zur Verarbeitung von Überbereitstellung reserviert ist</span><span class="sxs-lookup"><span data-stu-id="15ad5-2295">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="15ad5-2296">Aktualisierungsbefehle für `sig` korrigiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-2296">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="15ad5-2297">`--no-wait`-Unterstützung für die Verwaltung von Imageversionen in `sig` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2297">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="15ad5-2298">`vm list-ip-addresses` geändert, sodass die Verfügbarkeitszone von öffentlichen IP-Adressen angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="15ad5-2298">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="15ad5-2299">`[vm|vmss] disk attach` geändert, sodass die Standard-LUN eines Datenträgers standardmäßig auf die erste verfügbare Stelle festgelegt wird</span><span class="sxs-lookup"><span data-stu-id="15ad5-2299">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="15ad5-2300">21. September 2018</span><span class="sxs-lookup"><span data-stu-id="15ad5-2300">September 21, 2018</span></span>

<span data-ttu-id="15ad5-2301">Version 2.0.46</span><span class="sxs-lookup"><span data-stu-id="15ad5-2301">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="15ad5-2302">ACR</span><span class="sxs-lookup"><span data-stu-id="15ad5-2302">ACR</span></span>
* <span data-ttu-id="15ad5-2303">ACR-Aufgabenbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2303">Added ACR Task commands</span></span>
* <span data-ttu-id="15ad5-2304">Befehl für die Schnellausführung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2304">Added quick run command</span></span>
* <span data-ttu-id="15ad5-2305">`build-task`-Befehlsgruppe als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-2305">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="15ad5-2306">`helm`-Befehlsgruppe hinzugefügt, um die Verwaltung von Helm-Diagrammen mit ACR zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="15ad5-2306">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="15ad5-2307">Unterstützung für idempotentes Erstellen für die verwaltete Registrierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2307">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="15ad5-2308">Formatfreies Flag für die Anzeige von Buildprotokollen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2308">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="15ad5-2309">ACS</span><span class="sxs-lookup"><span data-stu-id="15ad5-2309">ACS</span></span>
* <span data-ttu-id="15ad5-2310">Befehl `install-connector` zum Festlegen des AKS-Master-FQDN geändert</span><span class="sxs-lookup"><span data-stu-id="15ad5-2310">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="15ad5-2311">Erstellen der Rollenzuweisung für „vnet-subnet-id“ (wenn kein Dienstprinzipal angegeben wurde) und „skip-role-assignment“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-2311">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="15ad5-2312">AppService</span><span class="sxs-lookup"><span data-stu-id="15ad5-2312">AppService</span></span>

* <span data-ttu-id="15ad5-2313">Unterstützung für WebJobs-Vorgangsverwaltung hinzugefügt (kontinuierlich/ausgelöst)</span><span class="sxs-lookup"><span data-stu-id="15ad5-2313">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="15ad5-2314">„az webapp config set“ unterstützt die Eigenschaft „--fts-state“; Unterstützung für „az functionapp config set/show“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2314">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="15ad5-2315">Unterstützung für Bring Your Own Storage für Web-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2315">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="15ad5-2316">Unterstützung für das Auflisten und Wiederherstellen gelöschter Web-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2316">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="15ad5-2317">Batch</span><span class="sxs-lookup"><span data-stu-id="15ad5-2317">Batch</span></span>
* <span data-ttu-id="15ad5-2318">Hinzufügen von Aufgaben über `--json-file` geändert, um die AddTaskCollectionParameter-Syntax zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="15ad5-2318">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="15ad5-2319">Dokumentation akzeptierter `--json-file`-Formate aktualisiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-2319">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="15ad5-2320">`--max-tasks-per-node-option` zu `batch pool create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2320">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="15ad5-2321">Verhalten von `batch account` geändert, um das aktuell angemeldete Konto anzuzeigen, wenn keine Optionen angegeben wurden</span><span class="sxs-lookup"><span data-stu-id="15ad5-2321">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="15ad5-2322">Batch KI</span><span class="sxs-lookup"><span data-stu-id="15ad5-2322">Batch AI</span></span> 
* <span data-ttu-id="15ad5-2323">Fehler bei der automatischen Speicherkontoerstellung im Befehl `batchai cluster create` behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-2323">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="15ad5-2324">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="15ad5-2324">Cognitive Services</span></span>
* <span data-ttu-id="15ad5-2325">Vervollständigung für die Argumente `--sku`, `--kind` und `--location` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2325">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="15ad5-2326">Befehl `cognitiveservices account list-usage` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2326">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="15ad5-2327">Befehl `cognitiveservices account list-kinds` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2327">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="15ad5-2328">Befehl `cognitiveservices account list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2328">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="15ad5-2329">`cognitiveservices list` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-2329">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="15ad5-2330">`--name` geändert (ist jetzt optional für `cognitiveservices account list-skus`)</span><span class="sxs-lookup"><span data-stu-id="15ad5-2330">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="15ad5-2331">Container</span><span class="sxs-lookup"><span data-stu-id="15ad5-2331">Container</span></span>
* <span data-ttu-id="15ad5-2332">Möglichkeit zum Neustarten und Beenden einer ausgeführten Containergruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2332">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="15ad5-2333">`--network-profile` zum Übergeben eines Netzwerkprofils hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2333">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="15ad5-2334">`--subnet` und `--vnet_name` hinzugefügt, um das Erstellen von Containergruppen in einem VNET zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="15ad5-2334">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="15ad5-2335">Tabellenausgabe geändert, sodass der Status der Containergruppe angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="15ad5-2335">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="15ad5-2336">Data Lake</span><span class="sxs-lookup"><span data-stu-id="15ad5-2336">Datalake</span></span>
* <span data-ttu-id="15ad5-2337">Befehle für VNET-Regeln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2337">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="15ad5-2338">Interaktive Shell</span><span class="sxs-lookup"><span data-stu-id="15ad5-2338">Interactive Shell</span></span>
* <span data-ttu-id="15ad5-2339">Fehler in Windows behoben, durch den Befehle nicht ordnungsgemäß ausgeführt wurden</span><span class="sxs-lookup"><span data-stu-id="15ad5-2339">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="15ad5-2340">Durch veraltete Objekte verursachtes Problem beim Laden von Befehlen im interaktiven Modus behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-2340">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="15ad5-2341">IoT</span><span class="sxs-lookup"><span data-stu-id="15ad5-2341">IoT</span></span>
* <span data-ttu-id="15ad5-2342">Routingunterstützung für IoT Hubs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2342">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="15ad5-2343">Key Vault</span><span class="sxs-lookup"><span data-stu-id="15ad5-2343">Key Vault</span></span>
* <span data-ttu-id="15ad5-2344">Key Vault-Schlüsselimport für RSA-Schlüssel korrigiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-2344">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="15ad5-2345">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="15ad5-2345">Network</span></span>
* <span data-ttu-id="15ad5-2346">Befehle vom Typ `network public-ip prefix` hinzugefügt, um Präfixe von öffentlichen IP-Adressen zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="15ad5-2346">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="15ad5-2347">Befehle vom Typ `network service-endpoint` hinzugefügt, um Dienstendpunktrichtlinien-Features zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="15ad5-2347">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="15ad5-2348">Befehle vom Typ `network lb outbound-rule` hinzugefügt, um die Erstellung von Ausgangsregeln für Load Balancer Standard zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="15ad5-2348">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="15ad5-2349">`--public-ip-prefix` zu `network lb frontend-ip create/update` hinzugefügt, um Front-End-IP-Konfigurationen mit Präfixen von öffentlichen IP-Adressen zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="15ad5-2349">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="15ad5-2350">`--enable-tcp-reset` zu `network lb rule/inbound-nat-rule/inbound-nat-pool create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2350">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="15ad5-2351">`--disable-outbound-snat` zu `network lb rule create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2351">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="15ad5-2352">Verwendung von `network watcher flow-log show/configure` mit klassischen NSGs ermöglicht</span><span class="sxs-lookup"><span data-stu-id="15ad5-2352">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="15ad5-2353">Hinzufügen des `network watcher run-configuration-diagnostic`-Befehls</span><span class="sxs-lookup"><span data-stu-id="15ad5-2353">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="15ad5-2354">Befehl `network watcher test-connectivity` korrigiert und Eigenschaften `--method`, `--valid-status-codes` und `--headers` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2354">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="15ad5-2355">`network express-route create/update`: Flag `--allow-global-reach` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2355">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="15ad5-2356">`network vnet subnet create/update`: Unterstützung für `--delegation` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2356">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="15ad5-2357">Befehl `network vnet subnet list-available-delegations` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2357">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="15ad5-2358">`network traffic-manager profile create/update`: Unterstützung für `--interval`, `--timeout` und `--max-failures` für die Überwachungskonfiguration hinzugefügt; Optionen `--monitor-path`, `--monitor-port` und `--monitor-protocol` zugunsten von `--path`, `--port` und `--protocol` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-2358">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="15ad5-2359">`network lb frontend-ip create/update`: Logik für das Festlegen der Zuweisungsmethode für private IP-Adressen korrigiert. Bei Angabe einer privaten IP-Adresse ist die Zuweisung statisch. Wird keine private IP-Adresse (oder eine leere Zeichenfolge für die private IP-Adresse) angegeben, erfolgt eine dynamische Zuweisung.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2359">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="15ad5-2360">`dns record-set * create/update`: Unterstützung für `--target-resource` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2360">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="15ad5-2361">Befehle vom Typ `network interface-endpoint` hinzugefügt, um Schnittstellenendpunkt-Objekte abzufragen</span><span class="sxs-lookup"><span data-stu-id="15ad5-2361">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="15ad5-2362">`network profile show/list/delete` für die partielle Verwaltung von Netzwerkprofilen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2362">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="15ad5-2363">Befehle vom Typ `network express-route peering connection` für die Verwaltung von Peeringverbindungen zwischen ExpressRoute-Instanzen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2363">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="15ad5-2364">RDBMS</span><span class="sxs-lookup"><span data-stu-id="15ad5-2364">RDBMS</span></span>
* <span data-ttu-id="15ad5-2365">Unterstützung für den MariaDB-Dienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2365">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="15ad5-2366">Reservierung</span><span class="sxs-lookup"><span data-stu-id="15ad5-2366">Reservation</span></span>
* <span data-ttu-id="15ad5-2367">Cosmos DB im Enumerationstyp für reservierte Ressourcen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2367">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="15ad5-2368">Namenseigenschaft im Patchmodell hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2368">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="15ad5-2369">App-Verwaltung</span><span class="sxs-lookup"><span data-stu-id="15ad5-2369">Manage App</span></span>
* <span data-ttu-id="15ad5-2370">Fehler in `managedapp create --kind MarketPlace` korrigiert, der zum Absturz der Instanzerstellung einer verwalteten Marketplace-App führte</span><span class="sxs-lookup"><span data-stu-id="15ad5-2370">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="15ad5-2371">Befehle vom Typ `feature` geändert, um sie auf unterstützte Profile zu beschränken</span><span class="sxs-lookup"><span data-stu-id="15ad5-2371">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="15ad5-2372">Role</span><span class="sxs-lookup"><span data-stu-id="15ad5-2372">Role</span></span>
* <span data-ttu-id="15ad5-2373">Unterstützung für das Auflisten der Gruppenmitgliedschaften des Benutzers hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2373">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="15ad5-2374">SignalR</span><span class="sxs-lookup"><span data-stu-id="15ad5-2374">SignalR</span></span>
* <span data-ttu-id="15ad5-2375">Erste Version</span><span class="sxs-lookup"><span data-stu-id="15ad5-2375">First release</span></span>

### <a name="storage"></a><span data-ttu-id="15ad5-2376">Storage</span><span class="sxs-lookup"><span data-stu-id="15ad5-2376">Storage</span></span>
* <span data-ttu-id="15ad5-2377">Parameter `--auth-mode login` für die Verwendung der Anmeldeinformationen des Benutzers für die Blob- und Warteschlangenautorisierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2377">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="15ad5-2378">`storage container immutability-policy/legal-hold` für die Verwaltung von unveränderlichem Speicher hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2378">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="15ad5-2379">VM</span><span class="sxs-lookup"><span data-stu-id="15ad5-2379">VM</span></span>
* <span data-ttu-id="15ad5-2380">Problem behoben, das dazu führte, dass die Datei mit dem privaten Schlüssel durch `vm create --generate-ssh-keys` überschrieben wird, wenn die Datei mit dem privaten Schlüssel fehlt (Nr. 4725, 6780)</span><span class="sxs-lookup"><span data-stu-id="15ad5-2380">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="15ad5-2381">Unterstützung für den gemeinsamen Image-Katalog über `az sig` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2381">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="15ad5-2382">28. August 2018</span><span class="sxs-lookup"><span data-stu-id="15ad5-2382">August 28, 2018</span></span>

<span data-ttu-id="15ad5-2383">Version 2.0.45</span><span class="sxs-lookup"><span data-stu-id="15ad5-2383">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="15ad5-2384">Core</span><span class="sxs-lookup"><span data-stu-id="15ad5-2384">Core</span></span>

* <span data-ttu-id="15ad5-2385">Das Problem, aufgrund dessen eine leere Konfigurationsdatei geladen wurde, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2385">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="15ad5-2386">Unterstützung für Profil `2018-03-01-hybrid` für Azure Stack hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2386">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="15ad5-2387">ACR</span><span class="sxs-lookup"><span data-stu-id="15ad5-2387">ACR</span></span>

* <span data-ttu-id="15ad5-2388">Problemumgehung für Laufzeitvorgänge ohne ARM-Anforderungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2388">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="15ad5-2389">Änderung vorgenommen, um im Befehl `build` Versionskontrolldateien (etwa „.git“ und „.gitignore“) standardmäßig aus der TAR-Datei auszuschließen</span><span class="sxs-lookup"><span data-stu-id="15ad5-2389">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="15ad5-2390">ACS</span><span class="sxs-lookup"><span data-stu-id="15ad5-2390">ACS</span></span>

* <span data-ttu-id="15ad5-2391">`aks create` geändert, dass standardmäßig virtuelle Computer vom Typ `Standard_DS2_v2` erstellt werden</span><span class="sxs-lookup"><span data-stu-id="15ad5-2391">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="15ad5-2392">`aks get-credentials` geändert, um nun neue APIs zum Abrufen der Clusteranmeldeinformationen aufzurufen</span><span class="sxs-lookup"><span data-stu-id="15ad5-2392">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="15ad5-2393">AppService</span><span class="sxs-lookup"><span data-stu-id="15ad5-2393">AppService</span></span>

* <span data-ttu-id="15ad5-2394">Unterstützung für CORS in „functionapp“ und „webapp“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2394">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="15ad5-2395">ARM-Tagunterstützung in Erstellungsbefehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2395">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="15ad5-2396">`[webapp|functionapp] identity show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="15ad5-2396">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="15ad5-2397">Backup</span><span class="sxs-lookup"><span data-stu-id="15ad5-2397">Backup</span></span>

* <span data-ttu-id="15ad5-2398">`backup vault backup-properties show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="15ad5-2398">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="15ad5-2399">Botdienst</span><span class="sxs-lookup"><span data-stu-id="15ad5-2399">Bot Service</span></span>

* <span data-ttu-id="15ad5-2400">Anfängliches Release der Botdienst-CLI</span><span class="sxs-lookup"><span data-stu-id="15ad5-2400">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="15ad5-2401">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="15ad5-2401">Cognitive Services</span></span>

* <span data-ttu-id="15ad5-2402">Neuer Parameter `--api-properties,` hinzugefügt, der zum Erstellen einiger Dienste erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="15ad5-2402">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="15ad5-2403">IoT</span><span class="sxs-lookup"><span data-stu-id="15ad5-2403">IoT</span></span>

* <span data-ttu-id="15ad5-2404">Problem mit dem Zuweisen verknüpfter Hubs behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-2404">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="15ad5-2405">Überwachen</span><span class="sxs-lookup"><span data-stu-id="15ad5-2405">Monitor</span></span>

* <span data-ttu-id="15ad5-2406">`monitor metrics alert`-Befehle für Metrikwarnungen nahezu in Echtzeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2406">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="15ad5-2407">`monitor alert`-Befehle als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-2407">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="15ad5-2408">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="15ad5-2408">Network</span></span>

* <span data-ttu-id="15ad5-2409">`network application-gateway ssl-policy predefined show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="15ad5-2409">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="15ad5-2410">Resource</span><span class="sxs-lookup"><span data-stu-id="15ad5-2410">Resource</span></span>

* <span data-ttu-id="15ad5-2411">`provider operation show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="15ad5-2411">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="15ad5-2412">Storage</span><span class="sxs-lookup"><span data-stu-id="15ad5-2412">Storage</span></span>

* <span data-ttu-id="15ad5-2413">`storage share policy show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="15ad5-2413">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="15ad5-2414">VM</span><span class="sxs-lookup"><span data-stu-id="15ad5-2414">VM</span></span>

* <span data-ttu-id="15ad5-2415">`vm/vmss identity show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="15ad5-2415">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="15ad5-2416">`--storage-caching` für `vm create` eingestellt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2416">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="15ad5-2417">14. August 2018</span><span class="sxs-lookup"><span data-stu-id="15ad5-2417">Auguest 14, 2018</span></span>

<span data-ttu-id="15ad5-2418">Version 2.0.44</span><span class="sxs-lookup"><span data-stu-id="15ad5-2418">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="15ad5-2419">Core</span><span class="sxs-lookup"><span data-stu-id="15ad5-2419">Core</span></span>

* <span data-ttu-id="15ad5-2420">Numerische Anzeige in `table`-Ausgabe korrigiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-2420">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="15ad5-2421">YAML-Ausgabeformat hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2421">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="15ad5-2422">Telemetrie</span><span class="sxs-lookup"><span data-stu-id="15ad5-2422">Telemetry</span></span>

* <span data-ttu-id="15ad5-2423">Verbesserte Berichterstellung für Telemetriedaten</span><span class="sxs-lookup"><span data-stu-id="15ad5-2423">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="15ad5-2424">ACR</span><span class="sxs-lookup"><span data-stu-id="15ad5-2424">ACR</span></span>

* <span data-ttu-id="15ad5-2425">Befehle vom Typ `content-trust policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2425">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="15ad5-2426">Problem behoben, aufgrund dessen `.dockerignore` nicht richtig verarbeitet wurde</span><span class="sxs-lookup"><span data-stu-id="15ad5-2426">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="15ad5-2427">ACS</span><span class="sxs-lookup"><span data-stu-id="15ad5-2427">ACS</span></span>

* <span data-ttu-id="15ad5-2428">`az acs/aks install-cli` für die Installation in `%USERPROFILE%\.azure-kubectl` unter Windows geändert</span><span class="sxs-lookup"><span data-stu-id="15ad5-2428">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="15ad5-2429">`az aks install-connector` geändert, um zu ermitteln, ob der Cluster über RBAC verfügt, und um den ACI-Connector entsprechend zu konfigurieren</span><span class="sxs-lookup"><span data-stu-id="15ad5-2429">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="15ad5-2430">Geändert in Rollenzuweisung zum Subnetz bei entsprechender Angabe</span><span class="sxs-lookup"><span data-stu-id="15ad5-2430">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="15ad5-2431">Neue Option zum Überspringen der Rollenzuweisung für Subnetz hinzugefügt, wenn dieses angegeben ist</span><span class="sxs-lookup"><span data-stu-id="15ad5-2431">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="15ad5-2432">Geändert, um Rollenzuweisung zum Subnetz zu überspringen, wenn bereits eine Zuweisung vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="15ad5-2432">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="15ad5-2433">AppService</span><span class="sxs-lookup"><span data-stu-id="15ad5-2433">AppService</span></span>

* <span data-ttu-id="15ad5-2434">Fehler behoben, der das Erstellen einer Funktions-App mithilfe von Speicherkonten in externen Ressourcengruppen verhinderte</span><span class="sxs-lookup"><span data-stu-id="15ad5-2434">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="15ad5-2435">Absturz bei ZIP-Bereitstellung behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-2435">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="15ad5-2436">Batch AI</span><span class="sxs-lookup"><span data-stu-id="15ad5-2436">BatchAI</span></span>

* <span data-ttu-id="15ad5-2437">Protokollierungsausgabe für die automatische Speicherkontoerstellung geändert, sodass nun „Ressourcen*gruppe*“ angegeben wird</span><span class="sxs-lookup"><span data-stu-id="15ad5-2437">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="15ad5-2438">Container</span><span class="sxs-lookup"><span data-stu-id="15ad5-2438">Container</span></span>

* <span data-ttu-id="15ad5-2439">`--secure-environment-variables` zum Übergeben sicherer Umgebungsvariablen an einen Container hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2439">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="15ad5-2440">IoT</span><span class="sxs-lookup"><span data-stu-id="15ad5-2440">IoT</span></span>

* <span data-ttu-id="15ad5-2441">[BREAKING CHANGE] Veraltete Befehle entfernt, die in die IoT-Erweiterung verschoben wurden</span><span class="sxs-lookup"><span data-stu-id="15ad5-2441">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="15ad5-2442">Elemente aktualisiert, um nicht die Domäne `azure-devices.net` anzunehmen</span><span class="sxs-lookup"><span data-stu-id="15ad5-2442">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="15ad5-2443">Iot Central</span><span class="sxs-lookup"><span data-stu-id="15ad5-2443">Iot Central</span></span>

* <span data-ttu-id="15ad5-2444">Erstes Release des IoT Central-Moduls</span><span class="sxs-lookup"><span data-stu-id="15ad5-2444">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="15ad5-2445">KeyVault</span><span class="sxs-lookup"><span data-stu-id="15ad5-2445">KeyVault</span></span>


* <span data-ttu-id="15ad5-2446">Befehle zum Verwalten von Speicherkonten und SAS-Definitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2446">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="15ad5-2447">Befehle für Netzwerkregeln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2447">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="15ad5-2448">Parameter `--id` zu Geheimnis-, Schlüssel- und Zertifikatvorgängen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2448">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="15ad5-2449">Unterstützung für Version mit mehreren APIs zur Schlüsseltresorverwaltung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2449">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="15ad5-2450">Unterstützung für Version mit mehreren APIs zur Schlüsseltresordatenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2450">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="15ad5-2451">Relay</span><span class="sxs-lookup"><span data-stu-id="15ad5-2451">Relay</span></span>

* <span data-ttu-id="15ad5-2452">Erste Veröffentlichung</span><span class="sxs-lookup"><span data-stu-id="15ad5-2452">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="15ad5-2453">Sql</span><span class="sxs-lookup"><span data-stu-id="15ad5-2453">Sql</span></span>

* <span data-ttu-id="15ad5-2454">Befehle vom Typ `sql failover-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2454">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="15ad5-2455">Storage</span><span class="sxs-lookup"><span data-stu-id="15ad5-2455">Storage</span></span>

* <span data-ttu-id="15ad5-2456">[BREAKING CHANGE]`storage account show-usage` geändert, um Parameter `--location` erforderlich zu machen. Auflistung nach Region</span><span class="sxs-lookup"><span data-stu-id="15ad5-2456">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="15ad5-2457">Parameter `--resource-group` geändert, sodass er für `storage account`-Befehle optional ist</span><span class="sxs-lookup"><span data-stu-id="15ad5-2457">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="15ad5-2458">Warnungen vom Typ „Fehler bei Vorbedingung“ für einzelne Fehler in Batch-Befehlen für eine aggregiert Nachricht entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2458">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="15ad5-2459">`[blob|file] delete-batch`-Befehle geändert, sodass kein Array mit Null-Werten mehr ausgegeben wird</span><span class="sxs-lookup"><span data-stu-id="15ad5-2459">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="15ad5-2460">`blob [download|upload|delete-batch]`-Befehle geändert, um SAS-Token aus Container-URL zu lesen</span><span class="sxs-lookup"><span data-stu-id="15ad5-2460">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="15ad5-2461">VM</span><span class="sxs-lookup"><span data-stu-id="15ad5-2461">VM</span></span>

* <span data-ttu-id="15ad5-2462">Allgemeine Filter zu `vm list-skus` für höhere Benutzerfreundlichkeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2462">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="15ad5-2463">31. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="15ad5-2463">July 31, 2018</span></span>

<span data-ttu-id="15ad5-2464">Version 2.0.43</span><span class="sxs-lookup"><span data-stu-id="15ad5-2464">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="15ad5-2465">ACR</span><span class="sxs-lookup"><span data-stu-id="15ad5-2465">ACR</span></span>

* <span data-ttu-id="15ad5-2466">Flag `--with-secure-properties` zum Befehl `acr build-task show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2466">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="15ad5-2467">Befehl `acr build-task update-build` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2467">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="15ad5-2468">ACS</span><span class="sxs-lookup"><span data-stu-id="15ad5-2468">ACS</span></span>

* <span data-ttu-id="15ad5-2469">Änderung, um 0 (Erfolg) zurückzugeben, wenn `az aks browse` durch Drücken von [STRG+C] beendet wird</span><span class="sxs-lookup"><span data-stu-id="15ad5-2469">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="15ad5-2470">Batch</span><span class="sxs-lookup"><span data-stu-id="15ad5-2470">Batch</span></span>

* <span data-ttu-id="15ad5-2471">Korrektur eines Fehlers bei der Anzeige des AAD-Tokens in Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="15ad5-2471">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="15ad5-2472">Container</span><span class="sxs-lookup"><span data-stu-id="15ad5-2472">Container</span></span>

* <span data-ttu-id="15ad5-2473">Voraussetzung von `--log-analytics-workspace-key` für Name oder ID im festgelegten Abonnement entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2473">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="15ad5-2474">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="15ad5-2474">Network</span></span>

* <span data-ttu-id="15ad5-2475">DNS-Unterstützung zu „2017-03-09-profile“ für Azure Stack hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2475">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="15ad5-2476">Resource</span><span class="sxs-lookup"><span data-stu-id="15ad5-2476">Resource</span></span>

* <span data-ttu-id="15ad5-2477">`--rollback-on-error` zu `group deployment create` hinzugefügt, um bei einem Fehler eine als funktionierend bekannte Bereitstellung auszuführen</span><span class="sxs-lookup"><span data-stu-id="15ad5-2477">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="15ad5-2478">Problem behoben, aufgrund dessen `--parameters {}` mit `group deployment create` zu einem Fehler führte</span><span class="sxs-lookup"><span data-stu-id="15ad5-2478">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="15ad5-2479">Role</span><span class="sxs-lookup"><span data-stu-id="15ad5-2479">Role</span></span>

* <span data-ttu-id="15ad5-2480">Unterstützung für das Stack-Profil „2017-03-09-profile“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2480">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="15ad5-2481">Problem behoben, aufgrund dessen das generische Update von Parametern auf `app update` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="15ad5-2481">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="15ad5-2482">Suchen,</span><span class="sxs-lookup"><span data-stu-id="15ad5-2482">Search</span></span>

* <span data-ttu-id="15ad5-2483">Befehle für Azure Search-Dienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2483">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="15ad5-2484">Service Bus</span><span class="sxs-lookup"><span data-stu-id="15ad5-2484">Service Bus</span></span>

* <span data-ttu-id="15ad5-2485">Migrationsbefehlsgruppe hinzugefügt, um einen Namespace von Service Bus Standard zu Premium zu migrieren</span><span class="sxs-lookup"><span data-stu-id="15ad5-2485">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="15ad5-2486">Neue optionale Eigenschaften zu Service Bus-Warteschlange und -Abonnement hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2486">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="15ad5-2487">`--enable-batched-operations` und `--enable-dead-lettering-on-message-expiration` in `queue`</span><span class="sxs-lookup"><span data-stu-id="15ad5-2487">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="15ad5-2488">`--dead-letter-on-filter-exceptions` in `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="15ad5-2488">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="15ad5-2489">Storage</span><span class="sxs-lookup"><span data-stu-id="15ad5-2489">Storage</span></span>

* <span data-ttu-id="15ad5-2490">Unterstützung für den Download großer Dateien über eine einzelne Verbindung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2490">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="15ad5-2491">`show`-Befehle konvertiert, bei denen im Falle einer fehlenden Ressource kein Fehler mit dem Exitcode 3 ausgelöst wurde</span><span class="sxs-lookup"><span data-stu-id="15ad5-2491">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="15ad5-2492">VM</span><span class="sxs-lookup"><span data-stu-id="15ad5-2492">VM</span></span>

* <span data-ttu-id="15ad5-2493">Unterstützung zum Auflisten von Verfügbarkeitsgruppen nach Abonnement hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2493">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="15ad5-2494">Unterstützung für `StandardSSD_LRS` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2494">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="15ad5-2495">Unterstützung für Anwendungssicherheitsgruppe beim Erstellen einer VM-Skalierungsgruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2495">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="15ad5-2496">[BREAKING CHANGE]`[vm|vmss] create`, `[vm|vmss] identity assign` und `[vm|vmss] identity remove` wurden geändert, um vom Benutzer zugewiesene Identitäten im Wörterbuchformat auszugeben.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2496">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="15ad5-2497">18. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="15ad5-2497">July 18, 2018</span></span>

<span data-ttu-id="15ad5-2498">Version 2.0.42</span><span class="sxs-lookup"><span data-stu-id="15ad5-2498">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="15ad5-2499">Core</span><span class="sxs-lookup"><span data-stu-id="15ad5-2499">Core</span></span>

* <span data-ttu-id="15ad5-2500">Unterstützung für browserbasierte Anmeldung WSL-Bash-Fenster hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2500">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="15ad5-2501">`--force-string`-Flag für alle generischen Updatebefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2501">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="15ad5-2502">[BREAKING CHANGE] Befehle vom Typ „show“ so geändert, dass die Fehlermeldung protokolliert wird und der Vorgang bei einer fehlenden Ressource mit dem Exitcode 3 fehlschlägt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2502">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="15ad5-2503">ACR</span><span class="sxs-lookup"><span data-stu-id="15ad5-2503">ACR</span></span>

* <span data-ttu-id="15ad5-2504">[BREAKING CHANGE] „--no-push“ in Befehl „acr build“ in reines Flag geändert</span><span class="sxs-lookup"><span data-stu-id="15ad5-2504">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="15ad5-2505">Befehle `show` und `update` unter Gruppe `acr repository` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2505">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="15ad5-2506">`--detail`-Flag für `show-manifests` und `show-tags` hinzugefügt, um ausführlichere Informationen anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="15ad5-2506">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="15ad5-2507">Parameter `--image` zur Unterstützung des Abrufs von Builddetails oder Protokollen anhand eines Images hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2507">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="15ad5-2508">ACS</span><span class="sxs-lookup"><span data-stu-id="15ad5-2508">ACS</span></span>

* <span data-ttu-id="15ad5-2509">`az aks create` so geändert, dass mit Fehler beendet wird, wenn `--max-pods` kleiner als 5 ist</span><span class="sxs-lookup"><span data-stu-id="15ad5-2509">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="15ad5-2510">AppService</span><span class="sxs-lookup"><span data-stu-id="15ad5-2510">AppService</span></span>

* <span data-ttu-id="15ad5-2511">Unterstützung für PremiumV2-SKUs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2511">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="15ad5-2512">Batch</span><span class="sxs-lookup"><span data-stu-id="15ad5-2512">Batch</span></span>

* <span data-ttu-id="15ad5-2513">Korrektur eines Fehlers bei der Verwendung von Anmeldeinformationen im Cloud Shell-Modus</span><span class="sxs-lookup"><span data-stu-id="15ad5-2513">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="15ad5-2514">JSON-Eingabe so geändert, dass Groß-/Kleinschreibung nicht beachtet wird</span><span class="sxs-lookup"><span data-stu-id="15ad5-2514">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="15ad5-2515">Batch KI</span><span class="sxs-lookup"><span data-stu-id="15ad5-2515">Batch AI</span></span>

* <span data-ttu-id="15ad5-2516">Befehl `az batchai job exec` korrigiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-2516">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="15ad5-2517">Container</span><span class="sxs-lookup"><span data-stu-id="15ad5-2517">Container</span></span>

* <span data-ttu-id="15ad5-2518">Anforderung von Benutzername und Kennwort für Nicht-DockerHub-Registrierungen entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2518">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="15ad5-2519">Fehler beim Erstellen von Containergruppen aus YAML-Datei behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-2519">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="15ad5-2520">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="15ad5-2520">Network</span></span>

* <span data-ttu-id="15ad5-2521">Unterstützung für `--no-wait` zu `network nic [create|update|delete]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2521">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="15ad5-2522">`network nic wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2522">Added `network nic wait`</span></span>
* <span data-ttu-id="15ad5-2523">`--ids`-Argument für `network vnet [subnet|peering] list` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-2523">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="15ad5-2524">`--include-default`-Flag hinzugefügt, um Standardsicherheitsregeln in die Ausgabe von `network nsg rule list` aufzunehmen</span><span class="sxs-lookup"><span data-stu-id="15ad5-2524">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="15ad5-2525">Resource</span><span class="sxs-lookup"><span data-stu-id="15ad5-2525">Resource</span></span>

* <span data-ttu-id="15ad5-2526">Unterstützung für `--no-wait` zu `group deployment delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2526">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="15ad5-2527">Unterstützung für `--no-wait` zu `deployment delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2527">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="15ad5-2528">Befehl `deployment wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2528">Added `deployment wait` command</span></span>
* <span data-ttu-id="15ad5-2529">Problem behoben, aufgrund dessen die `az deployment`-Befehle auf Abonnementebene fälschlicherweise für Profil „2017-03-09-profile“ angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="15ad5-2529">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="15ad5-2530">SQL</span><span class="sxs-lookup"><span data-stu-id="15ad5-2530">SQL</span></span>

* <span data-ttu-id="15ad5-2531">Fehler „Der angegebene Ressourcengruppenname ... entsprach nicht dem Namen in der URL“ beim Angeben des Namens des Pools für elastische Datenbanken für `sql db copy`-und `sql db replica create`-Befehle behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-2531">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="15ad5-2532">Konfigurieren des Standard-SQL Servers durch Ausführen von `az configure --defaults sql-server=<name>` zulässig</span><span class="sxs-lookup"><span data-stu-id="15ad5-2532">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="15ad5-2533">Tabellenformatierer für Befehle `sql server`, `sql server firewall-rule`, `sql list-usages` und `sql show-usage` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2533">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="15ad5-2534">Storage</span><span class="sxs-lookup"><span data-stu-id="15ad5-2534">Storage</span></span>

* <span data-ttu-id="15ad5-2535">`pageRanges`-Eigenschaft zu `storage blob show`-Ausgabe hinzugefügt, die für Seitenblobs ausgefüllt wird</span><span class="sxs-lookup"><span data-stu-id="15ad5-2535">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="15ad5-2536">VM</span><span class="sxs-lookup"><span data-stu-id="15ad5-2536">VM</span></span>

* <span data-ttu-id="15ad5-2537">[BREAKING CHANGE]`vmss create` so geändert, dass `Standard_DS1_v2` als standardmäßige Instanzgröße verwendet wird</span><span class="sxs-lookup"><span data-stu-id="15ad5-2537">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="15ad5-2538">Unterstützung für `--no-wait` zu `vm extension [set|delete]` und `vmss extension [set|delete]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2538">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="15ad5-2539">`vm extension wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2539">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="15ad5-2540">3\. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="15ad5-2540">July 3, 2018</span></span>

<span data-ttu-id="15ad5-2541">Version 2.0.41</span><span class="sxs-lookup"><span data-stu-id="15ad5-2541">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="15ad5-2542">AKS</span><span class="sxs-lookup"><span data-stu-id="15ad5-2542">AKS</span></span>

* <span data-ttu-id="15ad5-2543">Überwachung geändert, sodass Abonnement-ID verwendet wird</span><span class="sxs-lookup"><span data-stu-id="15ad5-2543">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="15ad5-2544">3\. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="15ad5-2544">July 3, 2018</span></span>

<span data-ttu-id="15ad5-2545">Version 2.0.40</span><span class="sxs-lookup"><span data-stu-id="15ad5-2545">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="15ad5-2546">Core</span><span class="sxs-lookup"><span data-stu-id="15ad5-2546">Core</span></span>

* <span data-ttu-id="15ad5-2547">Neuer Autorisierungscode-Flow für interaktive Anmeldung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2547">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="15ad5-2548">ACR</span><span class="sxs-lookup"><span data-stu-id="15ad5-2548">ACR</span></span>

* <span data-ttu-id="15ad5-2549">Abruf-Buildstatus hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2549">Added polling build status</span></span>
* <span data-ttu-id="15ad5-2550">Unterstützung für Enumerationswerte ohne Berücksichtigung von Groß-/Kleinschreibung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2550">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="15ad5-2551">Parameter `--top` und `--orderby` für `show-manifests` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2551">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="15ad5-2552">ACS</span><span class="sxs-lookup"><span data-stu-id="15ad5-2552">ACS</span></span>

* <span data-ttu-id="15ad5-2553">[BREAKING CHANGE] Standardmäßiges Aktivieren der rollenbasierten Zugriffssteuerung für Kubernetes</span><span class="sxs-lookup"><span data-stu-id="15ad5-2553">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="15ad5-2554">Argument `--disable-rbac` hinzugefügt und `--enable-rbac` als veraltet festgelegt, da es nun der Standard ist</span><span class="sxs-lookup"><span data-stu-id="15ad5-2554">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="15ad5-2555">Optionen für Befehl `aks browse` wurden aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2555">Updated options for `aks browse` command.</span></span> <span data-ttu-id="15ad5-2556">Unterstützung für `--listen-port` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2556">Added `--listen-port` support</span></span>
* <span data-ttu-id="15ad5-2557">Standardmäßiges Helm-Diagrammpaket für Befehl `aks install-connector` wurde aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2557">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="15ad5-2558">Verwenden von „virtual-kubelet-for-aks-latest.tgz“</span><span class="sxs-lookup"><span data-stu-id="15ad5-2558">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="15ad5-2559">Befehle `aks enable-addons` und `aks disable-addons` zum Aktualisieren eines vorhandenen Clusters hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2559">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="15ad5-2560">AppService</span><span class="sxs-lookup"><span data-stu-id="15ad5-2560">AppService</span></span>

* <span data-ttu-id="15ad5-2561">Unterstützung für das Deaktivieren der Identität über `webapp identity remove` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2561">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="15ad5-2562">`preview`-Tag für Identitätsfunktion entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2562">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="15ad5-2563">Backup</span><span class="sxs-lookup"><span data-stu-id="15ad5-2563">Backup</span></span>

* <span data-ttu-id="15ad5-2564">Moduldefinition aktualisiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-2564">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="15ad5-2565">Batch AI</span><span class="sxs-lookup"><span data-stu-id="15ad5-2565">BatchAI</span></span>

* <span data-ttu-id="15ad5-2566">Tabellenausgabe für Befehle `batchai cluster node list` und `batchai job node list` korrigiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-2566">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="15ad5-2567">Cloud</span><span class="sxs-lookup"><span data-stu-id="15ad5-2567">Cloud</span></span>

* <span data-ttu-id="15ad5-2568">Serversuffix `acr login` zu Cloudkonfiguration hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2568">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="15ad5-2569">Container</span><span class="sxs-lookup"><span data-stu-id="15ad5-2569">Container</span></span>

* <span data-ttu-id="15ad5-2570">`container create` zu Standard für Vorgang mit langer Ausführungsdauer geändert</span><span class="sxs-lookup"><span data-stu-id="15ad5-2570">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="15ad5-2571">Log Analytics-Parameter `--log-analytics-workspace` und `--log-analytics-workspace-key` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2571">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="15ad5-2572">Parameter `--protocol` zum Festlegen des zu verwendenden Netzwerkprotokolls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2572">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="15ad5-2573">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="15ad5-2573">Extension</span></span>

* <span data-ttu-id="15ad5-2574">`extension list-available` geändert, sodass nur mit der CLI-Version kompatible Erweiterungen angezeigt werden</span><span class="sxs-lookup"><span data-stu-id="15ad5-2574">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="15ad5-2575">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="15ad5-2575">Network</span></span>

* <span data-ttu-id="15ad5-2576">Problem behoben, aufgrund dessen bei Datensatztypen die Groß-/Kleinschreibung beachtet werden musste ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="15ad5-2576">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="15ad5-2577">Rdbms</span><span class="sxs-lookup"><span data-stu-id="15ad5-2577">Rdbms</span></span>

* <span data-ttu-id="15ad5-2578">Befehle vom Typ `[postgres|myql] server vnet-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2578">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="15ad5-2579">Resource</span><span class="sxs-lookup"><span data-stu-id="15ad5-2579">Resource</span></span>

* <span data-ttu-id="15ad5-2580">Neue Vorgangsgruppe `deployment` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2580">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="15ad5-2581">VM</span><span class="sxs-lookup"><span data-stu-id="15ad5-2581">VM</span></span>

* <span data-ttu-id="15ad5-2582">Unterstützung für das Entfernen der vom System zugewiesenen Identität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2582">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="15ad5-2583">25. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="15ad5-2583">June 25, 2018</span></span>

<span data-ttu-id="15ad5-2584">Version 2.0.39</span><span class="sxs-lookup"><span data-stu-id="15ad5-2584">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="15ad5-2585">Befehlszeilenschnittstelle (CLI)</span><span class="sxs-lookup"><span data-stu-id="15ad5-2585">CLI</span></span>

* <span data-ttu-id="15ad5-2586">Dateieinschränkung in MSI-Installer aktualisiert, um Problem mit der Erweiterungsinstallation zu beheben</span><span class="sxs-lookup"><span data-stu-id="15ad5-2586">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="15ad5-2587">19. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="15ad5-2587">June 19, 2018</span></span>

<span data-ttu-id="15ad5-2588">Version 2.0.38</span><span class="sxs-lookup"><span data-stu-id="15ad5-2588">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="15ad5-2589">Core</span><span class="sxs-lookup"><span data-stu-id="15ad5-2589">Core</span></span>

* <span data-ttu-id="15ad5-2590">Globale Unterstützung für `--subscription` zu den meisten Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2590">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="15ad5-2591">ACR</span><span class="sxs-lookup"><span data-stu-id="15ad5-2591">ACR</span></span>

* <span data-ttu-id="15ad5-2592">`azure-storage-blob` als Abhängigkeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2592">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="15ad5-2593">CPU-Standardkonfiguration für `acr build-task create` geändert, sodass zwei Kerne verwendet werden</span><span class="sxs-lookup"><span data-stu-id="15ad5-2593">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="15ad5-2594">ACS</span><span class="sxs-lookup"><span data-stu-id="15ad5-2594">ACS</span></span>

* <span data-ttu-id="15ad5-2595">Optionen des Befehls `aks use-dev-spaces` wurden aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2595">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="15ad5-2596">Unterstützung für `--update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2596">Added `--update` support</span></span>
* <span data-ttu-id="15ad5-2597">`aks get-credentials --admin` geändert, sodass der Benutzerkontext in `$HOME/.kube/config` ersetzt wird</span><span class="sxs-lookup"><span data-stu-id="15ad5-2597">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="15ad5-2598">Schreibgeschützte `nodeResourceGroup`-Eigenschaft in verwalteten Clustern verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="15ad5-2598">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="15ad5-2599">Befehlsfehler `acs browse` korrigiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-2599">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="15ad5-2600">`--connector-name` für `aks install-connector`, `aks upgrade-connector` und `aks remove-connector` als optional festgelegt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2600">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="15ad5-2601">Neue Azure Container Instances-Regionen für `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2601">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="15ad5-2602">Normalisierter Speicherort im Helm-Versionsnamen und Knotenname zu `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2602">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="15ad5-2603">AppService</span><span class="sxs-lookup"><span data-stu-id="15ad5-2603">AppService</span></span>

* <span data-ttu-id="15ad5-2604">Unterstützung für neuere Versionen von „urllib“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2604">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="15ad5-2605">Unterstützung der Verwendung eines App Service-Plans aus externen Ressourcengruppen zu `functionapp create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2605">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="15ad5-2606">Batch</span><span class="sxs-lookup"><span data-stu-id="15ad5-2606">Batch</span></span>

* <span data-ttu-id="15ad5-2607">`azure-batch-extensions`-Abhängigkeit entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2607">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="15ad5-2608">Batch KI</span><span class="sxs-lookup"><span data-stu-id="15ad5-2608">Batch AI</span></span>

* <span data-ttu-id="15ad5-2609">Unterstützung für Arbeitsbereiche wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2609">Added support for workspaces.</span></span> <span data-ttu-id="15ad5-2610">Arbeitsbereiche ermöglichen das Zusammenfassen von Clustern, Dateiservern und Experimenten in Gruppen ohne Beschränkung der Anzahl von Ressourcen, die erstellt werden können.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2610">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="15ad5-2611">Unterstützung für Experimente wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2611">Added support for experiments.</span></span> <span data-ttu-id="15ad5-2612">Experimente ermöglichen das Zusammenfassen von Aufträgen in Sammlungen ohne Beschränkung der Anzahl von erstellten Aufträgen.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2612">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="15ad5-2613">Unterstützung für das Konfigurieren von `/dev/shm` für Aufträge hinzugefügt, die in einem Docker-Container ausgeführt werden</span><span class="sxs-lookup"><span data-stu-id="15ad5-2613">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="15ad5-2614">Die Befehle `batchai cluster node exec` und `batchai job node exec` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2614">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="15ad5-2615">Diese Befehle ermöglichen die Ausführung aller Befehle direkt auf Knoten und bieten Funktionen zur Portweiterleitung.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2615">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="15ad5-2616">Unterstützung für `--ids` zu `batchai`-Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2616">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="15ad5-2617">[BREAKING CHANGE] Alle Cluster und Dateiserver müssen unter Arbeitsbereichen erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2617">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="15ad5-2618">[BREAKING CHANGE] Aufträge müssen unter Experimenten erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2618">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="15ad5-2619">[BREAKING CHANGE]`--nfs-resource-group` wurde aus den Befehlen `cluster create` und `job create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2619">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="15ad5-2620">Geben Sie zum Bereitstellen eines NFS, das einem anderen Arbeitsbereich/einer anderen Ressourcengruppe angehört, die ARM-ID des Dateiservers über die Option `--nfs` an.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2620">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="15ad5-2621">[BREAKING CHANGE]`--cluster-resource-group` wurde aus dem Befehl `job create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2621">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="15ad5-2622">Geben Sie zum Übermitteln eines Auftrags, der einem anderen Arbeitsbereich/einer anderen Ressourcengruppe angehört, die ARM-ID des Clusters über die Option `--cluster` an.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2622">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="15ad5-2623">[BREAKING CHANGE] Attribut `location` wurde aus Aufträgen, Clustern und Dateiservern entfernt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2623">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="15ad5-2624">„Location“ ist jetzt ein Attribut eines Arbeitsbereichs.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2624">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="15ad5-2625">[BREAKING CHANGE]`--location` wurde aus den Befehlen `job create`, `cluster create` und `file-server create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2625">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="15ad5-2626">[BREAKING CHANGE] Namen von Kurzoptionen wurden geändert, um die Schnittstelle konsistenter zu machen:</span><span class="sxs-lookup"><span data-stu-id="15ad5-2626">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="15ad5-2627">[`--config`, `-c`] in [`--config-file`, `-f`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2627">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="15ad5-2628">[`--cluster`, `-r`] in [`--cluster`, `-c`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2628">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="15ad5-2629">[`--cluster`, `-n`] in [`--cluster`, `-c`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2629">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="15ad5-2630">[`--job`, `-n`] in [`--job`, `-j`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2630">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="15ad5-2631">Karten</span><span class="sxs-lookup"><span data-stu-id="15ad5-2631">Maps</span></span>

* <span data-ttu-id="15ad5-2632">[BREAKING CHANGE]`maps account create` wurde so geändert, dass Nutzungsbedingungen entweder durch interaktive Eingabeaufforderung oder `--accept-tos`-Flag akzeptiert werden müssen.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2632">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="15ad5-2633">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="15ad5-2633">Network</span></span>

* <span data-ttu-id="15ad5-2634">Unterstützung für `https` zu `network lb probe create` hinzugefügt [Nr. 6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="15ad5-2634">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="15ad5-2635">Problem behoben, aufgrund dessen die Groß-/Kleinschreibung von `--endpoint-status` berücksichtigt wurde.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2635">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="15ad5-2636">#6502</span><span class="sxs-lookup"><span data-stu-id="15ad5-2636">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="15ad5-2637">Reservations</span><span class="sxs-lookup"><span data-stu-id="15ad5-2637">Reservations</span></span>

* <span data-ttu-id="15ad5-2638">[BREAKING CHANGE] Erforderlicher Parameter `ReservedResourceType` zu `reservations catalog show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2638">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="15ad5-2639">Parameter `Location` zu `reservations catalog show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2639">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="15ad5-2640">[BREAKING CHANGE]`kind` aus `ReservationProperties` entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2640">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="15ad5-2641">[BREAKING CHANGE]`capabilities` wurde in `Catalog` in `sku_properties` umbenannt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2641">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="15ad5-2642">[BREAKING CHANGE] Eigenschaften `size` und `tier` aus `Catalog` entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2642">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="15ad5-2643">Parameter `InstanceFlexibility` zu `reservations reservation update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2643">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="15ad5-2644">Role</span><span class="sxs-lookup"><span data-stu-id="15ad5-2644">Role</span></span>

* <span data-ttu-id="15ad5-2645">Fehlerbehandlung verbessert</span><span class="sxs-lookup"><span data-stu-id="15ad5-2645">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="15ad5-2646">SQL</span><span class="sxs-lookup"><span data-stu-id="15ad5-2646">SQL</span></span>

* <span data-ttu-id="15ad5-2647">Verwirrender Fehler behoben, der beim Ausführen von `az sql db list-editions` für einen Ort auftrat, der für Ihr Abonnement nicht verfügbar ist</span><span class="sxs-lookup"><span data-stu-id="15ad5-2647">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="15ad5-2648">Storage</span><span class="sxs-lookup"><span data-stu-id="15ad5-2648">Storage</span></span>

* <span data-ttu-id="15ad5-2649">Lesbarkeit der Tabellenausgabe für `storage blob download` verbessert</span><span class="sxs-lookup"><span data-stu-id="15ad5-2649">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="15ad5-2650">VM</span><span class="sxs-lookup"><span data-stu-id="15ad5-2650">VM</span></span>

* <span data-ttu-id="15ad5-2651">Verbesserte Einschränkung der VM-Größenüberprüfung für Unterstützung von beschleunigten Netzwerken in `vm create`</span><span class="sxs-lookup"><span data-stu-id="15ad5-2651">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="15ad5-2652">Warnung für `vmss create` hinzugefügt, dass die VM-Standardgröße von `Standard_D1_v2` auf `Standard_DS1_v2` umgestellt wird</span><span class="sxs-lookup"><span data-stu-id="15ad5-2652">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="15ad5-2653">`--force-update` zu `[vm|vmss] extension set` hinzugefügt, um die Erweiterung auch dann zu aktualisieren, wenn die Konfiguration nicht geändert wurde</span><span class="sxs-lookup"><span data-stu-id="15ad5-2653">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="15ad5-2654">13. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="15ad5-2654">June 13, 2018</span></span>

<span data-ttu-id="15ad5-2655">Version 2.0.37</span><span class="sxs-lookup"><span data-stu-id="15ad5-2655">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="15ad5-2656">Core</span><span class="sxs-lookup"><span data-stu-id="15ad5-2656">Core</span></span>

* <span data-ttu-id="15ad5-2657">Verbesserte interaktive Telemetrie</span><span class="sxs-lookup"><span data-stu-id="15ad5-2657">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="15ad5-2658">13. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="15ad5-2658">June 13, 2018</span></span>

<span data-ttu-id="15ad5-2659">Version 2.0.36</span><span class="sxs-lookup"><span data-stu-id="15ad5-2659">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="15ad5-2660">AKS</span><span class="sxs-lookup"><span data-stu-id="15ad5-2660">AKS</span></span>

* <span data-ttu-id="15ad5-2661">Zusätzliche erweiterte Netzwerkoptionen zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2661">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="15ad5-2662">Argumente zu `aks create` zum Aktivieren der Überwachung und HTTP-Routing hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2662">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="15ad5-2663">Argument `--no-ssh-key` zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2663">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="15ad5-2664">Argument `--enable-rbac` zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2664">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="15ad5-2665">[VORSCHAUVERSION] Unterstützung für Azure Active Directory-Authentifizierung zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2665">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="15ad5-2666">AppService</span><span class="sxs-lookup"><span data-stu-id="15ad5-2666">AppService</span></span>

* <span data-ttu-id="15ad5-2667">Problem mit inkompatiblen urllib-Versionen behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-2667">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="15ad5-2668">5\. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="15ad5-2668">June 5, 2018</span></span>

<span data-ttu-id="15ad5-2669">Version 2.0.35</span><span class="sxs-lookup"><span data-stu-id="15ad5-2669">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="15ad5-2670">Interactive</span><span class="sxs-lookup"><span data-stu-id="15ad5-2670">Interactive</span></span>

* <span data-ttu-id="15ad5-2671">Grenzwerte für die Abhängigkeiten des interaktiven Modus hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2671">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="15ad5-2672">5\. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="15ad5-2672">June 5, 2018</span></span>

<span data-ttu-id="15ad5-2673">Version 2.0.34</span><span class="sxs-lookup"><span data-stu-id="15ad5-2673">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="15ad5-2674">Core</span><span class="sxs-lookup"><span data-stu-id="15ad5-2674">Core</span></span>

* <span data-ttu-id="15ad5-2675">Unterstützung für mandantenübergreifende Ressourcenverweise hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2675">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="15ad5-2676">Verbesserte Zuverlässigkeit bei Telemetrieuploads</span><span class="sxs-lookup"><span data-stu-id="15ad5-2676">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="15ad5-2677">ACR</span><span class="sxs-lookup"><span data-stu-id="15ad5-2677">ACR</span></span>

* <span data-ttu-id="15ad5-2678">Unterstützung für VSTS als Remotequellort hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2678">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="15ad5-2679">Befehl `acr import` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2679">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="15ad5-2680">AKS</span><span class="sxs-lookup"><span data-stu-id="15ad5-2680">AKS</span></span>

* <span data-ttu-id="15ad5-2681">`aks get-credentials` wurde geändert, um die Kube-Konfigurationsdatei mit sichereren Dateisystemberechtigungen zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2681">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="15ad5-2682">Batch</span><span class="sxs-lookup"><span data-stu-id="15ad5-2682">Batch</span></span>

* <span data-ttu-id="15ad5-2683">Fehler bei der Formatierung der Poollistentabelle behoben [[Problem 4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="15ad5-2683">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="15ad5-2684">IoT</span><span class="sxs-lookup"><span data-stu-id="15ad5-2684">IOT</span></span>

* <span data-ttu-id="15ad5-2685">Unterstützung für das Erstellen von IoT Hub-Instanzen im Tarif „Basic“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2685">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="15ad5-2686">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="15ad5-2686">Network</span></span>

* <span data-ttu-id="15ad5-2687">`network vnet peering` wurde verbessert.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2687">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="15ad5-2688">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="15ad5-2688">Policy Insights</span></span>

* <span data-ttu-id="15ad5-2689">Erstrelease</span><span class="sxs-lookup"><span data-stu-id="15ad5-2689">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="15ad5-2690">ARM</span><span class="sxs-lookup"><span data-stu-id="15ad5-2690">ARM</span></span>

* <span data-ttu-id="15ad5-2691">Befehle vom Typ `account management-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2691">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="15ad5-2692">SQL</span><span class="sxs-lookup"><span data-stu-id="15ad5-2692">SQL</span></span>

* <span data-ttu-id="15ad5-2693">Neue Befehle für verwaltete Instanzen hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="15ad5-2693">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="15ad5-2694">Neue Befehle für verwaltete Datenbanken hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="15ad5-2694">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="15ad5-2695">Storage</span><span class="sxs-lookup"><span data-stu-id="15ad5-2695">Storage</span></span>

* <span data-ttu-id="15ad5-2696">Zusätzliche MimeTypes für JSON und JavaScript hinzugefügt (abzuleiten aus Dateierweiterungen)</span><span class="sxs-lookup"><span data-stu-id="15ad5-2696">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="15ad5-2697">VM</span><span class="sxs-lookup"><span data-stu-id="15ad5-2697">VM</span></span>

* <span data-ttu-id="15ad5-2698">`vm list-skus` wurde geändert, um feste Spalten zu verwenden und eine Warnung hinzuzufügen, dass `Tier` und `Size` entfernt werden.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2698">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="15ad5-2699">Option `--accelerated-networking` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2699">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="15ad5-2700">`--tags` zu `identity create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2700">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="15ad5-2701">22. Mai 2018</span><span class="sxs-lookup"><span data-stu-id="15ad5-2701">May 22, 2018</span></span>

<span data-ttu-id="15ad5-2702">Version 2.0.33</span><span class="sxs-lookup"><span data-stu-id="15ad5-2702">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="15ad5-2703">Core</span><span class="sxs-lookup"><span data-stu-id="15ad5-2703">Core</span></span>

* <span data-ttu-id="15ad5-2704">Unterstützung für das Erweitern von `@` in Dateinamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2704">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="15ad5-2705">ACS</span><span class="sxs-lookup"><span data-stu-id="15ad5-2705">ACS</span></span>

* <span data-ttu-id="15ad5-2706">Neue Dev Spaces-Befehle `aks use-dev-spaces` und `aks remove-dev-spaces` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2706">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="15ad5-2707">Tippfehler in Hilfemeldung korrigiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-2707">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="15ad5-2708">AppService</span><span class="sxs-lookup"><span data-stu-id="15ad5-2708">AppService</span></span>

* <span data-ttu-id="15ad5-2709">Verbesserte generische Aktualisierungsbefehle</span><span class="sxs-lookup"><span data-stu-id="15ad5-2709">Improved generic update commands</span></span>
* <span data-ttu-id="15ad5-2710">Asynchrone Unterstützung für `webapp deployment source config-zip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2710">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="15ad5-2711">Container</span><span class="sxs-lookup"><span data-stu-id="15ad5-2711">Container</span></span>

* <span data-ttu-id="15ad5-2712">Unterstützung für das Exportieren einer Containergruppe im YAML-Format hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2712">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="15ad5-2713">Unterstützung für die Verwendung einer YAML-Datei zum Erstellen/Aktualisieren einer Containergruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2713">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="15ad5-2714">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="15ad5-2714">Extension</span></span>

* <span data-ttu-id="15ad5-2715">Verbesserte Entfernung von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="15ad5-2715">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="15ad5-2716">Interactive</span><span class="sxs-lookup"><span data-stu-id="15ad5-2716">Interactive</span></span>

* <span data-ttu-id="15ad5-2717">Protokollierung geändert, um Parser für Abschlüsse zu deaktivieren</span><span class="sxs-lookup"><span data-stu-id="15ad5-2717">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="15ad5-2718">Verbesserte Verarbeitung beschädigter Hilfscaches</span><span class="sxs-lookup"><span data-stu-id="15ad5-2718">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="15ad5-2719">KeyVault</span><span class="sxs-lookup"><span data-stu-id="15ad5-2719">KeyVault</span></span>

* <span data-ttu-id="15ad5-2720">keyvault-Befehle wurden korrigiert, damit sie in Cloud Shell oder auf virtuellen Computern mit Identität verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2720">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="15ad5-2721">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="15ad5-2721">Network</span></span>

* <span data-ttu-id="15ad5-2722">Problem behoben, aufgrund dessen `network watcher show-topology` nicht mit einem VNET und/oder Subnetznamen verwendet werden konnte ([#6326](https://github.com/Azure/azure-cli/issues/6326))</span><span class="sxs-lookup"><span data-stu-id="15ad5-2722">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="15ad5-2723">Problem behoben, aufgrund dessen einige `network watcher`-Befehle fälschlicherweise angaben, dass Network Watcher nicht für bestimmte Regionen aktiviert ist ([#6264](https://github.com/Azure/azure-cli/issues/6264))</span><span class="sxs-lookup"><span data-stu-id="15ad5-2723">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="15ad5-2724">SQL</span><span class="sxs-lookup"><span data-stu-id="15ad5-2724">SQL</span></span>

* <span data-ttu-id="15ad5-2725">[BREAKING CHANGE] Von den Befehlen `db` und `dw` zurückgegebene Antwortobjekte geändert:</span><span class="sxs-lookup"><span data-stu-id="15ad5-2725">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="15ad5-2726">Eigenschaft `serviceLevelObjective` in `currentServiceObjectiveName` umbenannt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2726">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="15ad5-2727">Eigenschaften `currentServiceObjectiveId` und `requestedServiceObjectiveId` entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2727">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="15ad5-2728">Eigenschaft `maxSizeBytes` geändert (ist nun keine Zeichenfolge mehr, sondern ein Ganzzahlwert)</span><span class="sxs-lookup"><span data-stu-id="15ad5-2728">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="15ad5-2729">[BREAKING CHANGE] Die folgenden `db`- und `dw`-Eigenschaften wurden geändert und sind jetzt schreibgeschützt:</span><span class="sxs-lookup"><span data-stu-id="15ad5-2729">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="15ad5-2730">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2730">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="15ad5-2731">Verwenden Sie zum Aktualisieren den Parameter `--service-objective`, oder legen Sie die Eigenschaft `sku.name` fest.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2731">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="15ad5-2732">`edition`.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2732">`edition`.</span></span> <span data-ttu-id="15ad5-2733">Verwenden Sie zum Aktualisieren den Parameter `--edition`, oder legen Sie die Eigenschaft `sku.tier` fest.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2733">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="15ad5-2734">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2734">`elasticPoolName`.</span></span> <span data-ttu-id="15ad5-2735">Verwenden Sie zum Aktualisieren den Parameter `--elastic-pool`, oder legen Sie die Eigenschaft `elasticPoolId` fest.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2735">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="15ad5-2736">[BREAKING CHANGE] Die folgenden `elastic-pool`-Eigenschaften wurden geändert und sind jetzt schreibgeschützt:</span><span class="sxs-lookup"><span data-stu-id="15ad5-2736">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="15ad5-2737">`edition`.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2737">`edition`.</span></span> <span data-ttu-id="15ad5-2738">Verwenden Sie zum Aktualisieren den Parameter `--edition`.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2738">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="15ad5-2739">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2739">`dtu`.</span></span> <span data-ttu-id="15ad5-2740">Verwenden Sie zum Aktualisieren den Parameter `--capacity`.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2740">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="15ad5-2741">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2741">`databaseDtuMin`.</span></span> <span data-ttu-id="15ad5-2742">Verwenden Sie zum Aktualisieren den Parameter `--db-min-capacity`.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2742">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="15ad5-2743">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2743">`databaseDtuMax`.</span></span> <span data-ttu-id="15ad5-2744">Verwenden Sie zum Aktualisieren den Parameter `--db-max-capacity`.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2744">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="15ad5-2745">Die Parameter `--family` und `--capacity` wurden zu den `db`-, `dw`- und `elastic-pool`-Befehlen hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2745">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="15ad5-2746">Den `db`-, `dw`- und `elastic-pool`-Befehlen wurden Tabellenformatierer hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2746">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="15ad5-2747">Storage</span><span class="sxs-lookup"><span data-stu-id="15ad5-2747">Storage</span></span>

* <span data-ttu-id="15ad5-2748">Vervollständigung für das Argument `--account-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2748">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="15ad5-2749">Problem mit `storage entity query` behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-2749">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="15ad5-2750">VM</span><span class="sxs-lookup"><span data-stu-id="15ad5-2750">VM</span></span>

* <span data-ttu-id="15ad5-2751">[BREAKING CHANGE]`--write-accelerator` aus `vm create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2751">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="15ad5-2752">Die gleiche Unterstützung kann über `vm update` oder `vm disk attach` erzielt werden.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2752">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="15ad5-2753">Erweiterungsimageabgleich in `[vm|vmss] extension` korrigiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-2753">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="15ad5-2754">`--boot-diagnostics-storage` zu `vm create` zur Erfassung des Startprotokolls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2754">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="15ad5-2755">`--license-type` zu `[vm|vmss] update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2755">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="15ad5-2756">7\. Mai 2018</span><span class="sxs-lookup"><span data-stu-id="15ad5-2756">May 7, 2018</span></span>

<span data-ttu-id="15ad5-2757">Version 2.0.32</span><span class="sxs-lookup"><span data-stu-id="15ad5-2757">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="15ad5-2758">Core</span><span class="sxs-lookup"><span data-stu-id="15ad5-2758">Core</span></span>

* <span data-ttu-id="15ad5-2759">Ein Ausnahmefehler wurde behoben, der beim Abrufen von Geheimnissen aus einem Dienstprinzipalkonto mit Zertifikat auftrat.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2759">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="15ad5-2760">Eingeschränkte Unterstützung für positionelle Argumente hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2760">Added limited support for positional arguments</span></span>
* <span data-ttu-id="15ad5-2761">Problem behoben, aufgrund dessen `--query` nicht mit `--ids` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="15ad5-2761">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="15ad5-2762">#5591</span><span class="sxs-lookup"><span data-stu-id="15ad5-2762">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="15ad5-2763">Pipingszenarien von Befehlen bei Verwendung von `--ids` verbessert</span><span class="sxs-lookup"><span data-stu-id="15ad5-2763">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="15ad5-2764">Unterstützt `-o tsv` mit angegebener Abfrage bzw. `-o json` ohne angegeben Abfrage</span><span class="sxs-lookup"><span data-stu-id="15ad5-2764">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="15ad5-2765">Befehlsvorschläge bei Fehler hinzugefügt, wenn Befehle Tippfehler enthielten</span><span class="sxs-lookup"><span data-stu-id="15ad5-2765">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="15ad5-2766">Fehler bei der Eingabe von `az ''` behandelt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2766">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="15ad5-2767">Unterstützung für benutzerdefinierte Ressourcentypen für Befehlsmodule und -erweiterungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2767">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="15ad5-2768">ACR</span><span class="sxs-lookup"><span data-stu-id="15ad5-2768">ACR</span></span>

* <span data-ttu-id="15ad5-2769">ACR Build-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2769">Added ACR Build commands</span></span>
* <span data-ttu-id="15ad5-2770">Fehlermeldungen vom Typ „Ressource nicht gefunden.“ verbessert</span><span class="sxs-lookup"><span data-stu-id="15ad5-2770">Improved resource not found error messages</span></span>
* <span data-ttu-id="15ad5-2771">Höhere Leistung bei der Ressourcenerstellung und optimierte Fehlerbehandlung</span><span class="sxs-lookup"><span data-stu-id="15ad5-2771">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="15ad5-2772">ACR-Anmeldung bei nicht standardmäßigen Konsolen und WSL optimiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-2772">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="15ad5-2773">Fehlermeldungen zu Repositorybefehlen optimiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-2773">Improved repository commands error messages</span></span>
* <span data-ttu-id="15ad5-2774">Tabellenspalten und -reihenfolge aktualisiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-2774">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="15ad5-2775">ACS</span><span class="sxs-lookup"><span data-stu-id="15ad5-2775">ACS</span></span>

* <span data-ttu-id="15ad5-2776">Warnung hinzugefügt, dass `az aks` eine Vorschauversion des Diensts ist</span><span class="sxs-lookup"><span data-stu-id="15ad5-2776">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="15ad5-2777">Berechtigungsproblem in `aks install-connector` behoben, wenn `--aci-resource-group` nicht angegeben wird</span><span class="sxs-lookup"><span data-stu-id="15ad5-2777">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="15ad5-2778">AMS</span><span class="sxs-lookup"><span data-stu-id="15ad5-2778">AMS</span></span>

* <span data-ttu-id="15ad5-2779">Erste Version: Verwalten von Azure Media Services-Ressourcen</span><span class="sxs-lookup"><span data-stu-id="15ad5-2779">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="15ad5-2780">AppService</span><span class="sxs-lookup"><span data-stu-id="15ad5-2780">Appservice</span></span>

* <span data-ttu-id="15ad5-2781">Ein Problem in `webapp delete` wurde behoben, das bei Angabe von `--slot` auftrat.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2781">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="15ad5-2782">`--runtime-version` aus `webapp auth update` entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2782">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="15ad5-2783">Unterstützung für „min\_tls\_version“ und „https2.0“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2783">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="15ad5-2784">Unterstützung für mehrere Container hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2784">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="15ad5-2785">Batch KI</span><span class="sxs-lookup"><span data-stu-id="15ad5-2785">Batch AI</span></span>

* <span data-ttu-id="15ad5-2786">`batchai create cluster` wurde geändert, um die in der Konfigurationsdatei des Clusters konfigurierte VM-Priorität zu berücksichtigen.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2786">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="15ad5-2787">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="15ad5-2787">Cognitive Services</span></span>

* <span data-ttu-id="15ad5-2788">Tippfehler im Beispiel für `cognitiveservices account create` behoben [Nr. 5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="15ad5-2788">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="15ad5-2789">Nutzung</span><span class="sxs-lookup"><span data-stu-id="15ad5-2789">Consumption</span></span>

* <span data-ttu-id="15ad5-2790">Neue Befehle für Budget-API hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2790">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="15ad5-2791">Container</span><span class="sxs-lookup"><span data-stu-id="15ad5-2791">Container</span></span>

* <span data-ttu-id="15ad5-2792">`--registry-server` muss nicht mehr für `container create` angegeben werden, wenn ein Registrierungsserver im Imagenamen enthalten ist.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2792">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="15ad5-2793">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="15ad5-2793">Cosmos DB</span></span>

* <span data-ttu-id="15ad5-2794">VNET-Unterstützung für Azure CLI eingeführt: Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="15ad5-2794">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="15ad5-2795">DMS</span><span class="sxs-lookup"><span data-stu-id="15ad5-2795">DMS</span></span>

* <span data-ttu-id="15ad5-2796">Erste Version: Die Migration von SQL zu Azure SQL wird nun unterstützt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2796">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="15ad5-2797">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="15ad5-2797">Extension</span></span>

* <span data-ttu-id="15ad5-2798">Fehler behoben, aufgrund dessen Erweiterungsmetadaten nicht mehr angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="15ad5-2798">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="15ad5-2799">Interactive</span><span class="sxs-lookup"><span data-stu-id="15ad5-2799">Interactive</span></span>

* <span data-ttu-id="15ad5-2800">Interaktive Vervollständigung funktioniert nun auch mit positionellen Argumenten.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2800">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="15ad5-2801">Benutzerfreundlichere Ausgabe bei der Eingabe von '\'</span><span class="sxs-lookup"><span data-stu-id="15ad5-2801">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="15ad5-2802">Abschlüsse für Parameter ohne Hilfe korrigiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-2802">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="15ad5-2803">Beschreibungen für Befehlsgruppen korrigiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-2803">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="15ad5-2804">Labor</span><span class="sxs-lookup"><span data-stu-id="15ad5-2804">Lab</span></span>

* <span data-ttu-id="15ad5-2805">Regressionen aus Knack-Umwandlung korrigiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-2805">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="15ad5-2806">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="15ad5-2806">Network</span></span>

* <span data-ttu-id="15ad5-2807">[BREAKING CHANGE] Parameter `--ids` entfernt für:</span><span class="sxs-lookup"><span data-stu-id="15ad5-2807">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="15ad5-2808">Profil</span><span class="sxs-lookup"><span data-stu-id="15ad5-2808">Profile</span></span>

* <span data-ttu-id="15ad5-2809">Quellerkennung für `disk create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-2809">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="15ad5-2810">[BREAKING CHANGE]`--msi-port` und `--identity-port` entfernt, da sie nicht mehr verwendet werden</span><span class="sxs-lookup"><span data-stu-id="15ad5-2810">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="15ad5-2811">Tippfehler in kurzer Zusammenfassung für `account get-access-token` korrigiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-2811">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="15ad5-2812">Redis</span><span class="sxs-lookup"><span data-stu-id="15ad5-2812">Redis</span></span>

* <span data-ttu-id="15ad5-2813">`redis patch-schedule patch-schedule show` wurde durch `redis patch-schedule show` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2813">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="15ad5-2814">`redis list-all` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-2814">Deprecated `redis list-all`.</span></span> <span data-ttu-id="15ad5-2815">Diese Funktion wurde in `redis list` integriert.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2815">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="15ad5-2816">`redis import-method` wurde durch `redis import` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2816">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="15ad5-2817">Unterstützung für `--ids` zu verschiedenen Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2817">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="15ad5-2818">Role</span><span class="sxs-lookup"><span data-stu-id="15ad5-2818">Role</span></span>

* <span data-ttu-id="15ad5-2819">[BREAKING CHANGE] Veralteter Befehl `ad sp reset-credentials` entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2819">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="15ad5-2820">Storage</span><span class="sxs-lookup"><span data-stu-id="15ad5-2820">Storage</span></span>

* <span data-ttu-id="15ad5-2821">Zulassen, dass das Ziel-SAS-Token für die Blobkopie auf die Quelle angewendet wird, wenn Quell-SAS und Kontoschlüssel nicht angegeben werden</span><span class="sxs-lookup"><span data-stu-id="15ad5-2821">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="15ad5-2822">Verfügbar gemacht: Socket-Timeout für Blobuploads und -downloads</span><span class="sxs-lookup"><span data-stu-id="15ad5-2822">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="15ad5-2823">Blobnamen, die mit Pfadtrennzeichen beginnen, als relative Pfade behandeln</span><span class="sxs-lookup"><span data-stu-id="15ad5-2823">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="15ad5-2824">Zulassen, dass `storage blob copy --source-sas` mit dem Abfragezeichen „?“ beginnt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2824">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="15ad5-2825">`storage entity query --marker` korrigiert, um Liste von Schlüsselwerten zu akzeptieren</span><span class="sxs-lookup"><span data-stu-id="15ad5-2825">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="15ad5-2826">VM</span><span class="sxs-lookup"><span data-stu-id="15ad5-2826">VM</span></span>

* <span data-ttu-id="15ad5-2827">Ungültige Erkennungslogik für nicht verwalteten Blob-URI korrigiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-2827">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="15ad5-2828">Unterstützung für Datenträgerverschlüsselung ohne vom Benutzer bereitgestellte Dienstprinzipale hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2828">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="15ad5-2829">[BREAKING CHANGE] Verwenden Sie nicht „ManagedIdentityExtension“ des virtuellen Computers für MSI-Unterstützung.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2829">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="15ad5-2830">Unterstützung für Entfernungsrichtlinie zu `vmss` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2830">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="15ad5-2831">[BREAKING CHANGE]`--ids` entfernt aus:</span><span class="sxs-lookup"><span data-stu-id="15ad5-2831">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="15ad5-2832">Unterstützung für Schreibbeschleunigung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2832">Added write accelerator support</span></span>
* <span data-ttu-id="15ad5-2833">`vmss perform-maintenance` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2833">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="15ad5-2834">`vm diagnostics set` korrigiert, um zuverlässig den Betriebssystemtyp des virtuellen Computers zu erkennen</span><span class="sxs-lookup"><span data-stu-id="15ad5-2834">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="15ad5-2835">`vm resize` geändert, um zu überprüfen, ob die angeforderte Größe von der derzeit festgelegten Größe abweicht, und nur bei einer Änderung eine Aktualisierung auszuführen</span><span class="sxs-lookup"><span data-stu-id="15ad5-2835">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="15ad5-2836">10. April 2018</span><span class="sxs-lookup"><span data-stu-id="15ad5-2836">April 10, 2018</span></span>

<span data-ttu-id="15ad5-2837">Version 2.0.31</span><span class="sxs-lookup"><span data-stu-id="15ad5-2837">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="15ad5-2838">ACR</span><span class="sxs-lookup"><span data-stu-id="15ad5-2838">ACR</span></span>

* <span data-ttu-id="15ad5-2839">Verbesserte Fehlerbehandlung für wincred-Fallback</span><span class="sxs-lookup"><span data-stu-id="15ad5-2839">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="15ad5-2840">ACS</span><span class="sxs-lookup"><span data-stu-id="15ad5-2840">ACS</span></span>

* <span data-ttu-id="15ad5-2841">Gültigkeit von per AKS erstellten SPNs in fünf Jahre geändert</span><span class="sxs-lookup"><span data-stu-id="15ad5-2841">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="15ad5-2842">AppService</span><span class="sxs-lookup"><span data-stu-id="15ad5-2842">Appservice</span></span>

* [BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="15ad5-2844">Nicht abgefangene Ausnahme für nicht vorhandene Web-App-Pläne behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-2844">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="15ad5-2845">Batch AI</span><span class="sxs-lookup"><span data-stu-id="15ad5-2845">BatchAI</span></span>

* <span data-ttu-id="15ad5-2846">Unterstützung für API 2018-03-01 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2846">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="15ad5-2847">Bereitstellung auf Auftragsebene</span><span class="sxs-lookup"><span data-stu-id="15ad5-2847">Job level mounting</span></span>
  - <span data-ttu-id="15ad5-2848">Umgebungsvariablen mit Geheimniswerten</span><span class="sxs-lookup"><span data-stu-id="15ad5-2848">Environment variables with secret values</span></span>
  - <span data-ttu-id="15ad5-2849">Einstellungen von Leistungsindikatoren</span><span class="sxs-lookup"><span data-stu-id="15ad5-2849">Performance counters settings</span></span>
  - <span data-ttu-id="15ad5-2850">Berichtstellung für auftragsspezifisches Pfadsegment</span><span class="sxs-lookup"><span data-stu-id="15ad5-2850">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="15ad5-2851">Unterstützung für Unterordner in Listendateien-API</span><span class="sxs-lookup"><span data-stu-id="15ad5-2851">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="15ad5-2852">Berichterstellung zur Nutzung und zu Grenzwerten</span><span class="sxs-lookup"><span data-stu-id="15ad5-2852">Usage and limits reporting</span></span>
  - <span data-ttu-id="15ad5-2853">Zulassen der Angabe des Cachetyps für NFS-Server</span><span class="sxs-lookup"><span data-stu-id="15ad5-2853">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="15ad5-2854">Unterstützung für benutzerdefinierte Images</span><span class="sxs-lookup"><span data-stu-id="15ad5-2854">Support for custom images</span></span>
  - <span data-ttu-id="15ad5-2855">Unterstützung für pyTorch-Toolkit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2855">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="15ad5-2856">Befehl `job wait` hinzugefügt, der das Warten auf die Auftragsfertigstellung ermöglicht und den Code für die Auftragsbeendigung meldet</span><span class="sxs-lookup"><span data-stu-id="15ad5-2856">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="15ad5-2857">Befehl `usage show` hinzugefügt, mit dem die aktuelle Nutzung von Batch KI-Ressourcen und die Grenzwerte für verschiedene Regionen aufgelistet werden</span><span class="sxs-lookup"><span data-stu-id="15ad5-2857">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="15ad5-2858">Nationale Clouds werden unterstützt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2858">National clouds are supported</span></span>
* <span data-ttu-id="15ad5-2859">Befehlszeilenargumente für Aufträge hinzugefügt, um das Bereitstellen von Dateisystemen auf Auftragsebene zusätzlich zu Konfigurationsdateien zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="15ad5-2859">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="15ad5-2860">Weitere Optionen zum Anpassen von Clustern hinzugefügt – VM-Priorität, Subnetz, anfängliche Knotenanzahl für Cluster mit automatischer Skalierung, Angeben eines benutzerdefinierten Images</span><span class="sxs-lookup"><span data-stu-id="15ad5-2860">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="15ad5-2861">Befehlszeilenoption zum Angeben des Cachetyps für NFS mit Verwaltung per Batch KI hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2861">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="15ad5-2862">Angeben der Bereitstellung von Dateisystemen in Konfigurationsdateien vereinfacht.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2862">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="15ad5-2863">Weglassen von Anmeldeinformationen für Azure-Dateifreigaben und Azure-Blobcontainer ist jetzt möglich. Die CLI füllt fehlende Anmeldeinformationen auf, indem der Speicherkontoschlüssel verwendet wird, der über Befehlszeilenparameter oder per Umgebungsvariable angegeben wird, oder der Schlüssel wird über Azure Storage abgefragt (sofern das Speicherkonto zum aktuellen Abonnement gehört).</span><span class="sxs-lookup"><span data-stu-id="15ad5-2863">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="15ad5-2864">Der Befehl zum Streamen von Auftragsdateien wird jetzt automatisch abgeschlossen, nachdem der Auftrag beendet ist (Erfolg, Fehler, Beendigung oder Löschung)</span><span class="sxs-lookup"><span data-stu-id="15ad5-2864">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="15ad5-2865">Verbesserte `table`-Ausgabe für `show`-Vorgänge</span><span class="sxs-lookup"><span data-stu-id="15ad5-2865">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="15ad5-2866">Option `--use-auto-storage` für die Clustererstellung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2866">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="15ad5-2867">Diese Option erleichtert die Verwaltung von Speicherkonten und die Bereitstellung von Azure-Dateifreigaben und Azure-Blobcontainern in Clustern.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2867">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="15ad5-2868">`--generate-ssh-keys` für `cluster create` und `file-server create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2868">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="15ad5-2869">Möglichkeit zum Angeben der Knotensetupaufgabe über die Befehlszeile</span><span class="sxs-lookup"><span data-stu-id="15ad5-2869">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="15ad5-2870">[BREAKING CHANGE] Befehl `job stream-file` und `job list-files` in die Gruppe `job file` verschoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-2870">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="15ad5-2871">[BREAKING CHANGE]`--admin-user-name` im Befehl `file-server create` in `--user-name` umbenannt, um Einheitlichkeit mit dem Befehl `cluster create` zu erzielen</span><span class="sxs-lookup"><span data-stu-id="15ad5-2871">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="15ad5-2872">Abrechnung</span><span class="sxs-lookup"><span data-stu-id="15ad5-2872">Billing</span></span>

* <span data-ttu-id="15ad5-2873">Registrierungskontobefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2873">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="15ad5-2874">Nutzung</span><span class="sxs-lookup"><span data-stu-id="15ad5-2874">Consumption</span></span>

* <span data-ttu-id="15ad5-2875">Befehle vom Typ `marketplace` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2875">Added `marketplace` commands</span></span>
* <span data-ttu-id="15ad5-2876">[BREAKING CHANGE]`reservations summaries` in `reservation summary` umbenannt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2876">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="15ad5-2877">[BREAKING CHANGE]`reservations details` in `reservation detail` umbenannt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2877">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="15ad5-2878">[BREAKING CHANGE] Kurzoptionen `--reservation-order-id` und `--reservation-id` für `reservation`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2878">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="15ad5-2879">[BREAKING CHANGE]`--grain`-Kurzoptionen für `reservation summary`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2879">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="15ad5-2880">[BREAKING CHANGE]`--include-meter-details`-Kurzoptionen für `pricesheet`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2880">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="15ad5-2881">Container</span><span class="sxs-lookup"><span data-stu-id="15ad5-2881">Container</span></span>

* <span data-ttu-id="15ad5-2882">Parameter für die Volumebereitstellung für das Git-Repository hinzugefügt: `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` und `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="15ad5-2882">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="15ad5-2883">[#5926](https://github.com/Azure/azure-cli/issues/5926) behoben: Fehler bei `az container exec`, wenn „--container-name“ angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="15ad5-2883">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="15ad5-2884">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="15ad5-2884">Extension</span></span>

* <span data-ttu-id="15ad5-2885">Meldung für Distributionsüberprüfung in Debugebene geändert</span><span class="sxs-lookup"><span data-stu-id="15ad5-2885">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="15ad5-2886">Interactive</span><span class="sxs-lookup"><span data-stu-id="15ad5-2886">Interactive</span></span>

* <span data-ttu-id="15ad5-2887">Geändert: Verhinderung des Abschlusses bei nicht erkannten Befehlen</span><span class="sxs-lookup"><span data-stu-id="15ad5-2887">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="15ad5-2888">Ereignishooks vor und nach der Erstellung der Teilstruktur von Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2888">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="15ad5-2889">Abschluss für `--ids`-Parameter hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2889">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="15ad5-2890">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="15ad5-2890">Network</span></span>

* <span data-ttu-id="15ad5-2891">[#5936](https://github.com/Azure/azure-cli/issues/5936) behoben: `application-gateway create`-Tags konnten nicht festgelegt werden</span><span class="sxs-lookup"><span data-stu-id="15ad5-2891">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="15ad5-2892">Argument `--auth-certs` zum Anfügen von Authentifizierungszertifikaten für `application-gateway http-settings [create|update]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2892">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="15ad5-2893">#4910</span><span class="sxs-lookup"><span data-stu-id="15ad5-2893">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="15ad5-2894">`ddos-protection`-Befehle zum Erstellen von DDoS-Schutzplänen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2894">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="15ad5-2895">Unterstützung von `--ddos-protection-plan` für `vnet [create|update]` hinzugefügt, um das Zuordnen eines VNET zu einem DDoS-Schutzplan zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="15ad5-2895">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="15ad5-2896">Problem mit `--disable-bgp-route-propagation`-Flag in `network route-table [create|update]` behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-2896">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="15ad5-2897">Dummy-Argumente `--public-ip-address-type` und `--subnet-type` für `network lb [create|update]` entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2897">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="15ad5-2898">Unterstützung für TXT-Datensätze mit RFC 1035-Escapesequenzen für `network dns zone [import|export]` und `network dns record-set txt add-record` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2898">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="15ad5-2899">Profil</span><span class="sxs-lookup"><span data-stu-id="15ad5-2899">Profile</span></span>

* <span data-ttu-id="15ad5-2900">Unterstützung für klassische Azure-Konten in `account list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2900">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="15ad5-2901">[BREAKING CHANGE]`--msi` & `--msi-port`-Argumente entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2901">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="15ad5-2902">RDBMS</span><span class="sxs-lookup"><span data-stu-id="15ad5-2902">RDBMS</span></span>

* <span data-ttu-id="15ad5-2903">Befehl `georestore` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2903">Added `georestore` command</span></span>
* <span data-ttu-id="15ad5-2904">Speichergrößenbeschränkung aus Befehl `create` entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2904">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="15ad5-2905">Resource</span><span class="sxs-lookup"><span data-stu-id="15ad5-2905">Resource</span></span>

* <span data-ttu-id="15ad5-2906">Unterstützung für `--metadata` zu `policy definition create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2906">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="15ad5-2907">Unterstützung von `--metadata`, `--set`, `--add`, `--remove` für `policy definition update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2907">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="15ad5-2908">SQL</span><span class="sxs-lookup"><span data-stu-id="15ad5-2908">SQL</span></span>

* <span data-ttu-id="15ad5-2909">`sql elastic-pool op list` und `sql elastic-pool op cancel` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2909">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="15ad5-2910">Storage</span><span class="sxs-lookup"><span data-stu-id="15ad5-2910">Storage</span></span>

* <span data-ttu-id="15ad5-2911">Fehlermeldungen für falsch formatierte Verbindungszeichenfolgen verbessert</span><span class="sxs-lookup"><span data-stu-id="15ad5-2911">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="15ad5-2912">VM</span><span class="sxs-lookup"><span data-stu-id="15ad5-2912">VM</span></span>

* <span data-ttu-id="15ad5-2913">Unterstützung für die Konfiguration der Plattform-Fehlerdomänenanzahl für `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2913">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="15ad5-2914">`vmss create` geändert, damit standardmäßig „Standard LB“ für zonales, großes oder per einzelner Platzierungsgruppe deaktiviertes Scale Set festgelegt wird</span><span class="sxs-lookup"><span data-stu-id="15ad5-2914">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret`
* <span data-ttu-id="15ad5-2916">Unterstützung für SKU mit öffentlicher IP für `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2916">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="15ad5-2917">Argumente `--keyvault` und `--resource-group` für `vm secret format` hinzugefügt, um Szenarien zu unterstützen, bei denen der Befehl die Tresor-ID nicht auflösen kann.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2917">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="15ad5-2918">#5718</span><span class="sxs-lookup"><span data-stu-id="15ad5-2918">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="15ad5-2919">Bessere Fehler für `[vm|vmss create]`, wenn der Standort einer Ressourcengruppe keine Zonenunterstützung aufweist</span><span class="sxs-lookup"><span data-stu-id="15ad5-2919">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="15ad5-2920">27. März 2018</span><span class="sxs-lookup"><span data-stu-id="15ad5-2920">March 27, 2018</span></span>

<span data-ttu-id="15ad5-2921">Version 2.0.30</span><span class="sxs-lookup"><span data-stu-id="15ad5-2921">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="15ad5-2922">Core</span><span class="sxs-lookup"><span data-stu-id="15ad5-2922">Core</span></span>

* <span data-ttu-id="15ad5-2923">Anzeigen einer Meldung für Erweiterungen, die in der Hilfe als Vorschauversion gekennzeichnet sind</span><span class="sxs-lookup"><span data-stu-id="15ad5-2923">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="15ad5-2924">ACS</span><span class="sxs-lookup"><span data-stu-id="15ad5-2924">ACS</span></span>

* <span data-ttu-id="15ad5-2925">Behebung eines Fehlers bei der SSL-Zertifikatprüfung für `aks install-cli` in Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="15ad5-2925">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="15ad5-2926">AppService</span><span class="sxs-lookup"><span data-stu-id="15ad5-2926">Appservice</span></span>

* <span data-ttu-id="15ad5-2927">Unterstützung nur von HTTPS zu `webapp update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2927">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="15ad5-2928">Unterstützung für Slots zu `az webapp identity [assign|show]` und `az functionapp identity [assign|show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2928">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="15ad5-2929">Backup</span><span class="sxs-lookup"><span data-stu-id="15ad5-2929">Backup</span></span>

* <span data-ttu-id="15ad5-2930">Neuer Befehl `az backup protection isenabled-for-vm` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2930">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="15ad5-2931">Mit diesem Befehl kann überprüft werden, ob ein virtueller Computer von einem beliebigen Tresor im Abonnement gesichert wird.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2931">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="15ad5-2932">Azure-Objekt-IDs für Parameter `--resource-group` und `--vault-name` für die folgenden Befehle aktiviert:</span><span class="sxs-lookup"><span data-stu-id="15ad5-2932">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="15ad5-2933">`--name`-Parameter wurden geändert, um das Ausgabeformat von `backup ... show`-Befehlen zu akzeptieren.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2933">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="15ad5-2934">Container</span><span class="sxs-lookup"><span data-stu-id="15ad5-2934">Container</span></span>

* <span data-ttu-id="15ad5-2935">Befehl `container exec` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2935">Added `container exec` command.</span></span> <span data-ttu-id="15ad5-2936">Ausführung von Befehlen in einem Container für eine ausgeführte Containergruppe</span><span class="sxs-lookup"><span data-stu-id="15ad5-2936">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="15ad5-2937">Zulassen der Tabellenausgabe zum Erstellen und Aktualisieren einer Containergruppe</span><span class="sxs-lookup"><span data-stu-id="15ad5-2937">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="15ad5-2938">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="15ad5-2938">Extension</span></span>

* <span data-ttu-id="15ad5-2939">Meldung für `extension add` hinzugefügt, wenn sich die Erweiterung in der Vorschauphase befindet</span><span class="sxs-lookup"><span data-stu-id="15ad5-2939">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="15ad5-2940">`extension list-available` geändert, um vollständige Erweiterungsdaten mit `--show-details` anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="15ad5-2940">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="15ad5-2941">[BREAKING CHANGE]`extension list-available` geändert, um standardmäßig vereinfachte Erweiterungsdaten anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="15ad5-2941">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="15ad5-2942">Interactive</span><span class="sxs-lookup"><span data-stu-id="15ad5-2942">Interactive</span></span>

* <span data-ttu-id="15ad5-2943">Vervollständigungen wurden geändert und werden jetzt aktiviert, sobald das Laden der Befehlstabelle abgeschlossen ist.</span><span class="sxs-lookup"><span data-stu-id="15ad5-2943">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="15ad5-2944">Fehler bei der Verwendung des Parameters `--style` behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-2944">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="15ad5-2945">Interaktiver Lexer nach Befehlstabellensicherung instanziiert (sofern nicht vorhanden)</span><span class="sxs-lookup"><span data-stu-id="15ad5-2945">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="15ad5-2946">Verbesserte Unterstützung der Vervollständigung</span><span class="sxs-lookup"><span data-stu-id="15ad5-2946">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="15ad5-2947">Labor</span><span class="sxs-lookup"><span data-stu-id="15ad5-2947">Lab</span></span>

* <span data-ttu-id="15ad5-2948">Probleme mit Befehl `create environment` behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-2948">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="15ad5-2949">Überwachen</span><span class="sxs-lookup"><span data-stu-id="15ad5-2949">Monitor</span></span>

* <span data-ttu-id="15ad5-2950">Unterstützung für `--top`, `--orderby` und `--namespace` zu `metrics list` hinzugefügt [Nr. 5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="15ad5-2950">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="15ad5-2951">[#4529](https://github.com/Azure/azure-cli/issues/5785) behoben: `metrics list` akzeptiert eine durch Leerzeichen getrennte Liste von abzurufenden Metriken</span><span class="sxs-lookup"><span data-stu-id="15ad5-2951">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="15ad5-2952">Unterstützung für `--namespace` zu `metrics list-definitions` hinzugefügt [Nr. 5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="15ad5-2952">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="15ad5-2953">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="15ad5-2953">Network</span></span>

* <span data-ttu-id="15ad5-2954">Unterstützung für private DNS-Zonen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2954">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="15ad5-2955">Profil</span><span class="sxs-lookup"><span data-stu-id="15ad5-2955">Profile</span></span>

* <span data-ttu-id="15ad5-2956">Warnung für `--identity-port` und `--msi-port` zu `login` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2956">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="15ad5-2957">RDBMS</span><span class="sxs-lookup"><span data-stu-id="15ad5-2957">RDBMS</span></span>

* <span data-ttu-id="15ad5-2958">GA-API-Version 2017-12-01 (Geschäftsmodell) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2958">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="15ad5-2959">Resource</span><span class="sxs-lookup"><span data-stu-id="15ad5-2959">Resource</span></span>

* [BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="15ad5-2961">Role</span><span class="sxs-lookup"><span data-stu-id="15ad5-2961">Role</span></span>

* <span data-ttu-id="15ad5-2962">Unterstützung für erforderliche Zugriffskonfigurationen und native Clients zu `az ad app create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2962">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="15ad5-2963">`rbac`-Befehle geändert, um maximal 1.000 IDs für Objektauflösung zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="15ad5-2963">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="15ad5-2964">Befehle zur Verwaltung von Anmeldeinformationen (`ad sp credential [reset|list|delete]`) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2964">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="15ad5-2965">[BREAKING CHANGE] „properties“ aus `az role assignment [list|show]`-Ausgabe entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2965">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="15ad5-2966">Unterstützung für `dataActions`- und `notDataActions`-Berechtigungen zu `role definition` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2966">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="15ad5-2967">Storage</span><span class="sxs-lookup"><span data-stu-id="15ad5-2967">Storage</span></span>

* <span data-ttu-id="15ad5-2968">Problem beim Hochladen von Dateien mit einer Größe von 195 GB bis 200 GB behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-2968">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="15ad5-2969">[#4049](https://github.com/Azure/azure-cli/issues/4049) behoben: Probleme bei Uploads von Anfügeblobs behoben, die ein Ignorieren der Bedingungsparameter verursacht haben</span><span class="sxs-lookup"><span data-stu-id="15ad5-2969">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="15ad5-2970">VM</span><span class="sxs-lookup"><span data-stu-id="15ad5-2970">VM</span></span>

* <span data-ttu-id="15ad5-2971">Warnung für anstehende BREAKING CHANGEen für Sätze mit mehr als 100 Instanzen zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2971">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="15ad5-2972">Unterstützung der Zonenresilienz zu `vm [snapshot|image]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2972">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="15ad5-2973">Datenträgerinstanzansicht geändert, um besseren Verschlüsselungsstatus zu melden</span><span class="sxs-lookup"><span data-stu-id="15ad5-2973">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="15ad5-2974">[BREAKING CHANGE]`vm extension delete` geändert, um keine Ausgabe mehr zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="15ad5-2974">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="15ad5-2975">13. März 2018</span><span class="sxs-lookup"><span data-stu-id="15ad5-2975">March 13, 2018</span></span>

<span data-ttu-id="15ad5-2976">Version 2.0.29</span><span class="sxs-lookup"><span data-stu-id="15ad5-2976">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="15ad5-2977">ACR</span><span class="sxs-lookup"><span data-stu-id="15ad5-2977">ACR</span></span>

* <span data-ttu-id="15ad5-2978">Unterstützung für den Parameter `--image` zu `repository delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2978">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="15ad5-2979">Parameter `--manifest` und `--tag` des Befehls `repository delete` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-2979">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="15ad5-2980">Befehl `repository untag` zum Entfernen eines Tags ohne das Löschen von Daten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2980">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="15ad5-2981">ACS</span><span class="sxs-lookup"><span data-stu-id="15ad5-2981">ACS</span></span>

* <span data-ttu-id="15ad5-2982">Befehl `aks upgrade-connector` zum Aktualisieren eines vorhandenen Connectors hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2982">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="15ad5-2983">`kubectl`-Konfigurationsdateien zur Verwendung von besser lesbarem YAML im Blockstil geändert</span><span class="sxs-lookup"><span data-stu-id="15ad5-2983">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="15ad5-2984">Advisor</span><span class="sxs-lookup"><span data-stu-id="15ad5-2984">Advisor</span></span>

* <span data-ttu-id="15ad5-2985">[BREAKING CHANGE]`advisor configuration get` in `advisor configuration list` umbenannt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2985">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="15ad5-2986">[BREAKING CHANGE]`advisor configuration set` in `advisor configuration update` umbenannt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2986">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="15ad5-2987">[BREAKING CHANGE]`advisor recommendation generate` entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2987">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="15ad5-2988">Parameter `--refresh` zu `advisor recommendation list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2988">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="15ad5-2989">Befehl `advisor recommendation show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2989">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="15ad5-2990">AppService</span><span class="sxs-lookup"><span data-stu-id="15ad5-2990">Appservice</span></span>

* <span data-ttu-id="15ad5-2991">`[webapp|functionapp] assign-identity` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-2991">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="15ad5-2992">Befehle `webapp identity [assign|show]` und `functionapp identity [assign|show]` für verwaltete Identität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2992">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="15ad5-2993">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="15ad5-2993">Eventhubs</span></span>

* <span data-ttu-id="15ad5-2994">Erste Veröffentlichung</span><span class="sxs-lookup"><span data-stu-id="15ad5-2994">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="15ad5-2995">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="15ad5-2995">Extension</span></span>

* <span data-ttu-id="15ad5-2996">Überprüfung zum Warnen von Benutzern hinzugefügt, wenn sich die verwendete Distribution von der in der Paketquelldatei gespeicherten Distribution unterscheidet, da dies Fehlern führen kann</span><span class="sxs-lookup"><span data-stu-id="15ad5-2996">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="15ad5-2997">Interactive</span><span class="sxs-lookup"><span data-stu-id="15ad5-2997">Interactive</span></span>

* <span data-ttu-id="15ad5-2998">[#5625](https://github.com/Azure/azure-cli/issues/5625) behoben: Verlauf über verschiedene Sitzungen hinweg beibehalten</span><span class="sxs-lookup"><span data-stu-id="15ad5-2998">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="15ad5-2999">[#3016](https://github.com/Azure/azure-cli/issues/3016) behoben: Verlauf nicht aufgezeichnet, obwohl er innerhalb des Bereichs liegt</span><span class="sxs-lookup"><span data-stu-id="15ad5-2999">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="15ad5-3000">[#5688](https://github.com/Azure/azure-cli/issues/5688) behoben: Abschlüsse wurden nicht angezeigt, wenn beim Laden der Befehlstabelle eine Ausnahme aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="15ad5-3000">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="15ad5-3001">Statusanzeige für lang ausgeführte Vorgänge korrigiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-3001">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="15ad5-3002">Überwachen</span><span class="sxs-lookup"><span data-stu-id="15ad5-3002">Monitor</span></span>

* <span data-ttu-id="15ad5-3003">`monitor autoscale-settings`-Befehle als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-3003">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="15ad5-3004">Befehle vom Typ `monitor autoscale` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3004">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="15ad5-3005">Befehle vom Typ `monitor autoscale profile` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3005">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="15ad5-3006">Befehle vom Typ `monitor autoscale rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3006">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="15ad5-3007">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="15ad5-3007">Network</span></span>

* <span data-ttu-id="15ad5-3008">[BREAKING CHANGE] Parameter `--tags` aus `route-filter rule create` entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3008">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="15ad5-3009">Einige fehlerhafte Standardwerte für die folgenden Befehle entfernt:</span><span class="sxs-lookup"><span data-stu-id="15ad5-3009">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="15ad5-3010">`network watcher connection-monitor`-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3010">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="15ad5-3011">Parameter `--vnet` und `--subnet` zu `network watcher show-topology` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3011">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="15ad5-3012">Profil</span><span class="sxs-lookup"><span data-stu-id="15ad5-3012">Profile</span></span>

* <span data-ttu-id="15ad5-3013">Parameter `--msi` für `az login` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-3013">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="15ad5-3014">Parameter `--identity` für `az login` als Ersatz vor `--msi` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3014">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="15ad5-3015">RDBMS</span><span class="sxs-lookup"><span data-stu-id="15ad5-3015">RDBMS</span></span>

* <span data-ttu-id="15ad5-3016">[VORSCHAU] Geändert, sodass die API „2017-12-01-preview“ verwendet wird</span><span class="sxs-lookup"><span data-stu-id="15ad5-3016">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="15ad5-3017">Service Bus</span><span class="sxs-lookup"><span data-stu-id="15ad5-3017">Service Bus</span></span>

* <span data-ttu-id="15ad5-3018">Erste Veröffentlichung</span><span class="sxs-lookup"><span data-stu-id="15ad5-3018">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="15ad5-3019">Storage</span><span class="sxs-lookup"><span data-stu-id="15ad5-3019">Storage</span></span>

* <span data-ttu-id="15ad5-3020">[#4971](https://github.com/Azure/azure-cli/issues/4971) behoben: `storage blob copy` unterstützt jetzt andere Azure-Clouds.</span><span class="sxs-lookup"><span data-stu-id="15ad5-3020">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="15ad5-3021">[#5286](https://github.com/Azure/azure-cli/issues/5286) behoben: Batchbefehle `storage blob [delete-batch|download-batch|upload-batch]` lösen bei Vorbedingungsfehlern keinen Fehler mehr aus</span><span class="sxs-lookup"><span data-stu-id="15ad5-3021">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="15ad5-3022">VM</span><span class="sxs-lookup"><span data-stu-id="15ad5-3022">VM</span></span>

* <span data-ttu-id="15ad5-3023">`[vm|vmss] create` unterstützt jetzt das Anfügen nicht verwalteter Datenträger und das Konfigurieren der Zwischenspeicherung.</span><span class="sxs-lookup"><span data-stu-id="15ad5-3023">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="15ad5-3024">`[vm|vmss] assign-identity` und `[vm|vmss] remove-identity` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-3024">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="15ad5-3025">Befehle `vm identity [assign|remove|show]` und `vmss identity [assign|remove|show]` als Ersatz für veraltete Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3025">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="15ad5-3026">Standardpriorität in `vmss create` auf „Keine“ geändert</span><span class="sxs-lookup"><span data-stu-id="15ad5-3026">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="15ad5-3027">27. Februar 2018</span><span class="sxs-lookup"><span data-stu-id="15ad5-3027">February 27, 2018</span></span>

<span data-ttu-id="15ad5-3028">Version 2.0.28</span><span class="sxs-lookup"><span data-stu-id="15ad5-3028">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="15ad5-3029">Core</span><span class="sxs-lookup"><span data-stu-id="15ad5-3029">Core</span></span>

* <span data-ttu-id="15ad5-3030">[#5184](https://github.com/Azure/azure-cli/issues/5184) behoben: Problem beim Installieren von Homebrew</span><span class="sxs-lookup"><span data-stu-id="15ad5-3030">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="15ad5-3031">Unterstützung für Erweiterungstelemetrie mit benutzerdefinierten Schlüsseln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3031">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="15ad5-3032">HTTP-Protokollierung zu `--debug` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3032">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="15ad5-3033">ACS</span><span class="sxs-lookup"><span data-stu-id="15ad5-3033">ACS</span></span>

* <span data-ttu-id="15ad5-3034">Geändert, sodass für `aks install-connector` standardmäßig das Helm-Diagramm `virtual-kubelet-for-aks` verwendet wird</span><span class="sxs-lookup"><span data-stu-id="15ad5-3034">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="15ad5-3035">Problem behoben: Unzureichende Berechtigungen für Dienstprinzipale zum Erstellen einer ACI-Containergruppe</span><span class="sxs-lookup"><span data-stu-id="15ad5-3035">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="15ad5-3036">Parameter `--aci-container-group`, `--location` und `--image-tag` zu `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3036">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="15ad5-3037">Veraltungshinweis aus `aks get-versions` entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3037">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="15ad5-3038">AppService</span><span class="sxs-lookup"><span data-stu-id="15ad5-3038">Appservice</span></span>

* <span data-ttu-id="15ad5-3039">Updates für die neue SDK-Version (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="15ad5-3039">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="15ad5-3040">[5538](https://github.com/Azure/azure-cli/issues/5538) behoben: `Free` wurde als ungültige SKU gemeldet.</span><span class="sxs-lookup"><span data-stu-id="15ad5-3040">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="15ad5-3041">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="15ad5-3041">Cognitive Services</span></span>

* <span data-ttu-id="15ad5-3042">Hinweis beim Erstellen eines neuen Cognitive Services-Kontos aktualisiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-3042">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="15ad5-3043">Nutzung</span><span class="sxs-lookup"><span data-stu-id="15ad5-3043">Consumption</span></span>

* <span data-ttu-id="15ad5-3044">Neue Befehle für PriceSheet-API hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3044">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="15ad5-3045">Vorhandene Formate für Nutzungsdetails und Reservierungsdetails aktualisiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-3045">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="15ad5-3046">Container</span><span class="sxs-lookup"><span data-stu-id="15ad5-3046">Container</span></span>

* <span data-ttu-id="15ad5-3047">Argumente `--secrets` und `--secrets-mount-path` zu `container create` hinzugefügt, um Geheimnisse in ACI verwenden zu können</span><span class="sxs-lookup"><span data-stu-id="15ad5-3047">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="15ad5-3048">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="15ad5-3048">Network</span></span>

* <span data-ttu-id="15ad5-3049">[#5559](https://github.com/Azure/azure-cli/issues/5559) behoben: Fehlender Client in `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="15ad5-3049">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="15ad5-3050">Resource</span><span class="sxs-lookup"><span data-stu-id="15ad5-3050">Resource</span></span>

* <span data-ttu-id="15ad5-3051">`group deployment export` geändert, um eine partielle Vorlage und ggf. Fehler anzuzeigen, wenn der Vorgang nicht erfolgreich war</span><span class="sxs-lookup"><span data-stu-id="15ad5-3051">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="15ad5-3052">Role</span><span class="sxs-lookup"><span data-stu-id="15ad5-3052">Role</span></span>

* <span data-ttu-id="15ad5-3053">`role assignment list-changelogs` hinzugefügt, um die Überprüfung von Dienstprinzipalrollen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="15ad5-3053">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="15ad5-3054">SQL</span><span class="sxs-lookup"><span data-stu-id="15ad5-3054">SQL</span></span>

* <span data-ttu-id="15ad5-3055">Zonenredundanzunterstützung für Datenbanken und Pools für elastische Datenbanken hinzugefügt (bei Erstellung und Aktualisierung)</span><span class="sxs-lookup"><span data-stu-id="15ad5-3055">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="15ad5-3056">Storage</span><span class="sxs-lookup"><span data-stu-id="15ad5-3056">Storage</span></span>

* <span data-ttu-id="15ad5-3057">Angabe von Zielpfad/Präfix für `storage blob [upload-batch|download-batch]` ermöglicht</span><span class="sxs-lookup"><span data-stu-id="15ad5-3057">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="15ad5-3058">VM</span><span class="sxs-lookup"><span data-stu-id="15ad5-3058">VM</span></span>

* <span data-ttu-id="15ad5-3059">Unterstützung für das Anfügen/Trennen von Datenträgern für eine einzelne VMSS-Instanz hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3059">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="15ad5-3060">13. Februar 2018</span><span class="sxs-lookup"><span data-stu-id="15ad5-3060">February 13, 2018</span></span>

<span data-ttu-id="15ad5-3061">Version 2.0.27</span><span class="sxs-lookup"><span data-stu-id="15ad5-3061">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="15ad5-3062">Core</span><span class="sxs-lookup"><span data-stu-id="15ad5-3062">Core</span></span>

* <span data-ttu-id="15ad5-3063">Authentifizierung für Abonnement-ID und Namen bei der MSI-Anmeldung in Authentifizierung mit Schlüssel geändert</span><span class="sxs-lookup"><span data-stu-id="15ad5-3063">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="15ad5-3064">ACS</span><span class="sxs-lookup"><span data-stu-id="15ad5-3064">ACS</span></span>

* <span data-ttu-id="15ad5-3065">[BREAKING CHANGE]`aks get-versions` aus Gründen der Genauigkeit in `aks get-upgrades` umbenannt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3065">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="15ad5-3066">`aks get-versions` zur Anzeige der verfügbaren Kubernetes-Versionen für `aks create` geändert</span><span class="sxs-lookup"><span data-stu-id="15ad5-3066">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="15ad5-3067">Standardwerte von `aks create` in Auswahl der Kubernetes-Version durch den Server geändert</span><span class="sxs-lookup"><span data-stu-id="15ad5-3067">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="15ad5-3068">Hilfemeldungen zu dem von AKS generierten Dienstprinzipal aktualisiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-3068">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="15ad5-3069">Standardknotengrößen für `aks create` von „Standard\_D1\_v2“ in „Standard\_DS1\_v2“ geändert</span><span class="sxs-lookup"><span data-stu-id="15ad5-3069">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="15ad5-3070">Zuverlässigkeit der Suche nach dem Dashboardpod für `az aks browse` verbessert</span><span class="sxs-lookup"><span data-stu-id="15ad5-3070">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="15ad5-3071">`aks get-credentials` korrigiert, um Unicode-Fehler beim Laden von Kubernetes-Konfigurationsdateien zu behandeln</span><span class="sxs-lookup"><span data-stu-id="15ad5-3071">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="15ad5-3072">Meldung zu `az aks install-cli` hinzugefügt, um das Abrufen von `kubectl` in `$PATH` zu erleichtern</span><span class="sxs-lookup"><span data-stu-id="15ad5-3072">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="15ad5-3073">AppService</span><span class="sxs-lookup"><span data-stu-id="15ad5-3073">Appservice</span></span>

* <span data-ttu-id="15ad5-3074">Problem behoben, das zu einem Fehler von `webapp [backup|restore]` aufgrund eines Nullverweises führte</span><span class="sxs-lookup"><span data-stu-id="15ad5-3074">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="15ad5-3075">Unterstützung für Standard-App Service-Pläne durch `az configure --defaults appserviceplan=my-asp` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3075">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="15ad5-3076">CDN</span><span class="sxs-lookup"><span data-stu-id="15ad5-3076">CDN</span></span>

* <span data-ttu-id="15ad5-3077">Befehle vom Typ `cdn custom-domain [enable-https|disable-https]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3077">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="15ad5-3078">Container</span><span class="sxs-lookup"><span data-stu-id="15ad5-3078">Container</span></span>

* <span data-ttu-id="15ad5-3079">Option `--follow` zu `az container logs` für Streamingprotokolle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3079">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="15ad5-3080">Befehl `container attach` hinzugefügt, der die lokale Standardausgabe und Fehlerdatenströme an einen Container in einer Containergruppe angefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3080">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="15ad5-3081">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="15ad5-3081">CosmosDB</span></span>

* <span data-ttu-id="15ad5-3082">Unterstützung für Einstellungsfunktionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3082">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="15ad5-3083">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="15ad5-3083">Extension</span></span>

* <span data-ttu-id="15ad5-3084">Unterstützung für den Parameter `--pip-proxy` zu Befehlen vom Typ `az extension [add|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3084">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="15ad5-3085">Unterstützung für das Argument `--pip-extra-index-urls` zu Befehlen vom Typ `az extension [add|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3085">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="15ad5-3086">Feedback</span><span class="sxs-lookup"><span data-stu-id="15ad5-3086">Feedback</span></span>

* <span data-ttu-id="15ad5-3087">Erweiterungsinformationen zu Telemetriedaten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3087">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="15ad5-3088">Interactive</span><span class="sxs-lookup"><span data-stu-id="15ad5-3088">Interactive</span></span>

* <span data-ttu-id="15ad5-3089">Problem behoben, aufgrund dessen der Benutzer bei Verwendung des interaktiven Modus in Cloud Shell zur Anmeldung aufgefordert wird</span><span class="sxs-lookup"><span data-stu-id="15ad5-3089">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="15ad5-3090">Regression mit fehlenden Parametervervollständigungen korrigiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-3090">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="15ad5-3091">IoT</span><span class="sxs-lookup"><span data-stu-id="15ad5-3091">IoT</span></span>

* <span data-ttu-id="15ad5-3092">Problem behoben, aufgrund dessen `iot dps access policy [create|update]` bei erfolgreicher Ausführung einen Fehler „nicht gefunden“ zurückgibt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3092">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="15ad5-3093">Problem behoben, aufgrund dessen `iot dps linked-hub [create|update]` bei erfolgreicher Ausführung einen Fehler „nicht gefunden“ zurückgibt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3093">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="15ad5-3094">Unterstützung für `--no-wait` zu `iot dps access policy [create|update]` und `iot dps linked-hub [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3094">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="15ad5-3095">`iot hub create` geändert, um die Angabe der Anzahl von Partitionen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="15ad5-3095">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="15ad5-3096">Überwachen</span><span class="sxs-lookup"><span data-stu-id="15ad5-3096">Monitor</span></span>

* <span data-ttu-id="15ad5-3097">Befehl `az monitor log-profiles create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-3097">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="15ad5-3098">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="15ad5-3098">Network</span></span>

* <span data-ttu-id="15ad5-3099">Option `--tags` für folgende Befehle korrigiert:</span><span class="sxs-lookup"><span data-stu-id="15ad5-3099">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="15ad5-3100">Profil</span><span class="sxs-lookup"><span data-stu-id="15ad5-3100">Profile</span></span>

* <span data-ttu-id="15ad5-3101">`az login` im interaktiven Modus aktiviert</span><span class="sxs-lookup"><span data-stu-id="15ad5-3101">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="15ad5-3102">Resource</span><span class="sxs-lookup"><span data-stu-id="15ad5-3102">Resource</span></span>

* <span data-ttu-id="15ad5-3103">`feature show` wieder hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3103">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="15ad5-3104">Role</span><span class="sxs-lookup"><span data-stu-id="15ad5-3104">Role</span></span>

* <span data-ttu-id="15ad5-3105">Argument `--available-to-other-tenants` zu `ad app update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3105">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="15ad5-3106">SQL</span><span class="sxs-lookup"><span data-stu-id="15ad5-3106">SQL</span></span>

* <span data-ttu-id="15ad5-3107">Befehle vom Typ `sql server dns-alias` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3107">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="15ad5-3108">`sql db rename` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3108">Added `sql db rename`</span></span>
* <span data-ttu-id="15ad5-3109">Unterstützung für das Argument `--ids` für alle SQL-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3109">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="15ad5-3110">Storage</span><span class="sxs-lookup"><span data-stu-id="15ad5-3110">Storage</span></span>

* <span data-ttu-id="15ad5-3111">Befehle `storage blob service-properties delete-policy` und `storage blob undelete` hinzugefügt, um vorläufiges Löschen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="15ad5-3111">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="15ad5-3112">VM</span><span class="sxs-lookup"><span data-stu-id="15ad5-3112">VM</span></span>

* <span data-ttu-id="15ad5-3113">Absturz bei unvollständiger Initialisierung der VM-Verschlüsselung behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-3113">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="15ad5-3114">Prinzipal-ID-Ausgabe beim Aktivieren von MSI hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3114">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="15ad5-3115">`vm boot-diagnostics get-boot-log` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="15ad5-3115">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="15ad5-3116">31. Januar 2018</span><span class="sxs-lookup"><span data-stu-id="15ad5-3116">January 31, 2018</span></span>

<span data-ttu-id="15ad5-3117">Version 2.0.26</span><span class="sxs-lookup"><span data-stu-id="15ad5-3117">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="15ad5-3118">Core</span><span class="sxs-lookup"><span data-stu-id="15ad5-3118">Core</span></span>

* <span data-ttu-id="15ad5-3119">Unterstützung für das Abrufen von unformatierten Token im MSI-Kontext hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3119">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="15ad5-3120">Abrufindikator-Zeichenfolge nach Fertigstellung von LRO für die Windows-Datei „cmd.exe“ entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3120">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="15ad5-3121">Warnung hinzugefügt, die angezeigt wird, wenn ein konfigurierter Standardwert in einen Eintrag auf INFO-Ebene geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="15ad5-3121">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="15ad5-3122">`--verbose` zum Anzeigen verwenden.</span><span class="sxs-lookup"><span data-stu-id="15ad5-3122">Use `--verbose` to see</span></span>
* <span data-ttu-id="15ad5-3123">Statusanzeige für Wait-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3123">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="15ad5-3124">ACS</span><span class="sxs-lookup"><span data-stu-id="15ad5-3124">ACS</span></span>

* <span data-ttu-id="15ad5-3125">Argument `--disable-browser` erläutert</span><span class="sxs-lookup"><span data-stu-id="15ad5-3125">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="15ad5-3126">Vervollständigung mit der TAB-TASTE für Argumente vom Typ `--vm-size` verbessert</span><span class="sxs-lookup"><span data-stu-id="15ad5-3126">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="15ad5-3127">AppService</span><span class="sxs-lookup"><span data-stu-id="15ad5-3127">Appservice</span></span>

* <span data-ttu-id="15ad5-3128">`webapp log [tail|download]` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="15ad5-3128">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="15ad5-3129">Überprüfung `kind` für Web-Apps und Funktionen entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3129">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="15ad5-3130">CDN</span><span class="sxs-lookup"><span data-stu-id="15ad5-3130">CDN</span></span>

* <span data-ttu-id="15ad5-3131">Problem mit fehlendem Client für `cdn custom-domain create` behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-3131">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="15ad5-3132">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="15ad5-3132">CosmosDB</span></span>

* <span data-ttu-id="15ad5-3133">Parameterbeschreibung für Failoverrichtlinien korrigiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-3133">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="15ad5-3134">Interactive</span><span class="sxs-lookup"><span data-stu-id="15ad5-3134">Interactive</span></span>

* <span data-ttu-id="15ad5-3135">Problem behoben, aufgrund dessen Vervollständigungen von Befehlsoptionen nicht mehr angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="15ad5-3135">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="15ad5-3136">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="15ad5-3136">Network</span></span>

* <span data-ttu-id="15ad5-3137">Schutz für `--cert-password` zu `application-gateway create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3137">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="15ad5-3138">Problem mit `application-gateway update` behoben, aufgrund dessen `--sku` fälschlicherweise einen Standardwert anwendete</span><span class="sxs-lookup"><span data-stu-id="15ad5-3138">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="15ad5-3139">Schutz für `--shared-key` und `--authorization-key` zu `vpn-connection create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3139">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="15ad5-3140">Problem mit fehlendem Client für `asg create` behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-3140">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="15ad5-3141">Parameter `--file-name / -f` für exportierte Namen zu `dns zone export` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3141">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="15ad5-3142">Folgende Probleme mit `dns zone export` behoben:</span><span class="sxs-lookup"><span data-stu-id="15ad5-3142">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="15ad5-3143">Problem behoben, aufgrund dessen lange TXT-Einträge nicht korrekt exportiert wurden</span><span class="sxs-lookup"><span data-stu-id="15ad5-3143">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="15ad5-3144">Problem behoben, aufgrund dessen TXT-Einträge in Anführungszeichen fälschlich ohne Anführungszeichen in Escapezeichen exportiert wurden</span><span class="sxs-lookup"><span data-stu-id="15ad5-3144">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="15ad5-3145">Problem behoben, aufgrund dessen bestimmte Datensätze zweimal mit `dns zone import` importiert wurden</span><span class="sxs-lookup"><span data-stu-id="15ad5-3145">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="15ad5-3146">Befehle `vnet-gateway root-cert` und `vnet-gateway revoked-cert` wiederhergestellt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3146">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="15ad5-3147">Profil</span><span class="sxs-lookup"><span data-stu-id="15ad5-3147">Profile</span></span>

* <span data-ttu-id="15ad5-3148">`get-access-token` zur Verwendung auf einer VM mit Identität korrigiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-3148">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="15ad5-3149">Resource</span><span class="sxs-lookup"><span data-stu-id="15ad5-3149">Resource</span></span>

* <span data-ttu-id="15ad5-3150">Fehler mit `deployment [create|validate]` korrigiert, aufgrund dessen fälschlich eine Warnung angezeigt wurde, wenn ein Vorlagenfeld „Typ“ Werte in Großbuchstaben enthielt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3150">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="15ad5-3151">Storage</span><span class="sxs-lookup"><span data-stu-id="15ad5-3151">Storage</span></span>

* <span data-ttu-id="15ad5-3152">Problem mit der Migration von Storage V1-Konten zu Storage V2 behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-3152">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="15ad5-3153">Statusberichterstellung für alle Upload-/Downloadbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3153">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="15ad5-3154">Fehler korrigiert, der die Verwendung der arg-Option „-n“ mit `storage account check-name` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="15ad5-3154">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="15ad5-3155">Spalte „Momentaufnahme“ zur Tabellenausgabe für `blob [list|show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3155">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="15ad5-3156">Fehler mit verschiedenen Parametern korrigiert, die als Int-Typen analysiert werden mussten</span><span class="sxs-lookup"><span data-stu-id="15ad5-3156">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="15ad5-3157">VM</span><span class="sxs-lookup"><span data-stu-id="15ad5-3157">VM</span></span>

* <span data-ttu-id="15ad5-3158">Befehl `vm image accept-terms` hinzugefügt, um die Erstellung von VMs aus Images mit zusätzlichen Gebühren zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="15ad5-3158">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="15ad5-3159">`[vm|vmss create]` korrigiert, um sicherzustellen, dass Befehle unter einem Proxy mit nicht signierten Zertifikaten ausgeführt werden können</span><span class="sxs-lookup"><span data-stu-id="15ad5-3159">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="15ad5-3160">[VORSCHAU] Unterstützung für „niedrige“ Priorität zu VMSS hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3160">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="15ad5-3161">Schutz für `--admin-password` zu `[vm|vmss] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3161">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="15ad5-3162">17. Januar 2018</span><span class="sxs-lookup"><span data-stu-id="15ad5-3162">January 17, 2018</span></span>

<span data-ttu-id="15ad5-3163">Version 2.0.25</span><span class="sxs-lookup"><span data-stu-id="15ad5-3163">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="15ad5-3164">ACR</span><span class="sxs-lookup"><span data-stu-id="15ad5-3164">ACR</span></span>

* <span data-ttu-id="15ad5-3165">Fallback auf ACR-Anmeldung bei Fehlern mit Windows-Anmeldeinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3165">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="15ad5-3166">Registrierungsprotokolle aktiviert</span><span class="sxs-lookup"><span data-stu-id="15ad5-3166">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="15ad5-3167">ACS</span><span class="sxs-lookup"><span data-stu-id="15ad5-3167">ACS</span></span>

* <span data-ttu-id="15ad5-3168">Befehl `get-credentials` korrigiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-3168">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="15ad5-3169">SPN-Rollenanforderung entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3169">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="15ad5-3170">AppService</span><span class="sxs-lookup"><span data-stu-id="15ad5-3170">Appservice</span></span>

* <span data-ttu-id="15ad5-3171">Fehler mit `config ssl upload` behoben, bei dem `hosting_environment_profile` NULL war</span><span class="sxs-lookup"><span data-stu-id="15ad5-3171">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="15ad5-3172">Unterstützung benutzerdefinierter URLs zu `browse` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3172">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="15ad5-3173">Slotunterstützung für `log tail` korrigiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-3173">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="15ad5-3174">Backup</span><span class="sxs-lookup"><span data-stu-id="15ad5-3174">Backup</span></span>

* <span data-ttu-id="15ad5-3175">Option `--container-name` von `backup item list` geändert (ist jetzt optional)</span><span class="sxs-lookup"><span data-stu-id="15ad5-3175">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="15ad5-3176">Speicherkontooptionen zu `backup restore restore-disks` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3176">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="15ad5-3177">Standortüberprüfung in `backup protection enable-for-vm` korrigiert (Groß-/Kleinschreibung wird jetzt nicht mehr beachtet)</span><span class="sxs-lookup"><span data-stu-id="15ad5-3177">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="15ad5-3178">Problem behoben, durch das bei Befehlen mit ungültigem Containernamen ein Fehler auftrat</span><span class="sxs-lookup"><span data-stu-id="15ad5-3178">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="15ad5-3179">`backup item list` geändert (Integritätsstatus jetzt standardmäßig enthalten)</span><span class="sxs-lookup"><span data-stu-id="15ad5-3179">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="15ad5-3180">Batch</span><span class="sxs-lookup"><span data-stu-id="15ad5-3180">Batch</span></span>

* <span data-ttu-id="15ad5-3181">`batch login` geändert, um Authentifizierungsdetails zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="15ad5-3181">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="15ad5-3182">Cloud</span><span class="sxs-lookup"><span data-stu-id="15ad5-3182">Cloud</span></span>

* <span data-ttu-id="15ad5-3183">Beim Festlegen von `--profile` für eine Cloud werden nun keine Endpunkte mehr benötigt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-3183">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="15ad5-3184">Nutzung</span><span class="sxs-lookup"><span data-stu-id="15ad5-3184">Consumption</span></span>

* <span data-ttu-id="15ad5-3185">Neue Befehle für Reservierungen hinzugefügt: `consumption reservations summaries` und `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="15ad5-3185">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="15ad5-3186">Event Grid</span><span class="sxs-lookup"><span data-stu-id="15ad5-3186">Event Grid</span></span>

* <span data-ttu-id="15ad5-3187">[BREAKING CHANGE] Die Befehle vom Typ `az eventgrid topic event-subscription` wurden in `eventgrid event-subscription` verschoben.</span><span class="sxs-lookup"><span data-stu-id="15ad5-3187">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="15ad5-3188">[BREAKING CHANGE] Die Befehle vom Typ `az eventgrid resource event-subscription` wurden in `eventgrid event-subscription` verschoben.</span><span class="sxs-lookup"><span data-stu-id="15ad5-3188">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="15ad5-3189">[BREAKING CHANGE] Der Befehl `eventgrid event-subscription show-endpoint-url` wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-3189">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="15ad5-3190">Verwenden Sie stattdessen `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="15ad5-3190">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="15ad5-3191">Befehl `eventgrid topic update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3191">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="15ad5-3192">Befehl `eventgrid event-subscription update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3192">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="15ad5-3193">Parameter `--ids` für Befehle vom Typ `eventgrid topic` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3193">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="15ad5-3194">Unterstützung der Vervollständigung mit der TAB-TASTE für Themennamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3194">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="15ad5-3195">Interactive</span><span class="sxs-lookup"><span data-stu-id="15ad5-3195">Interactive</span></span>

* <span data-ttu-id="15ad5-3196">Problem behoben, das dazu führte, dass der interaktive Modus nicht mit Python 2.x verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="15ad5-3196">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="15ad5-3197">Fehler beim Start behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-3197">Fixed errors on startup</span></span>
* <span data-ttu-id="15ad5-3198">Problem behoben, das dazu führte, dass einige Befehle nicht im interaktiven Modus ausgeführt werden konnten</span><span class="sxs-lookup"><span data-stu-id="15ad5-3198">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="15ad5-3199">IoT</span><span class="sxs-lookup"><span data-stu-id="15ad5-3199">IoT</span></span>

* <span data-ttu-id="15ad5-3200">Unterstützung für Gerätebereitstellungsdienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3200">Added support for device provisioning service</span></span>
* <span data-ttu-id="15ad5-3201">Benachrichtigungen zu veralteten Elementen in Befehlen und in der Befehlshilfe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3201">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="15ad5-3202">IoT-Überprüfung hinzugefügt, um Benutzer über die IoT-Erweiterung zu informieren</span><span class="sxs-lookup"><span data-stu-id="15ad5-3202">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="15ad5-3203">Überwachen</span><span class="sxs-lookup"><span data-stu-id="15ad5-3203">Monitor</span></span>

* <span data-ttu-id="15ad5-3204">Unterstützung mehrerer Diagnoseeinstellung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-3204">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="15ad5-3205">Der Parameter `--name` ist nun für `az monitor diagnostic-settings create` erforderlich.</span><span class="sxs-lookup"><span data-stu-id="15ad5-3205">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="15ad5-3206">Befehl `monitor diagnostic-settings categories` zum Abrufen der Diagnoseeinstellungskategorie hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3206">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="15ad5-3207">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="15ad5-3207">Network</span></span>

* <span data-ttu-id="15ad5-3208">Problem behoben, das beim Ändern des aktiven Standbymodus mit `vnet-gateway update` auftrat</span><span class="sxs-lookup"><span data-stu-id="15ad5-3208">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="15ad5-3209">Unterstützung für HTTP2 zu `application-gateway [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3209">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="15ad5-3210">Profil</span><span class="sxs-lookup"><span data-stu-id="15ad5-3210">Profile</span></span>

* <span data-ttu-id="15ad5-3211">Unterstützung für die Anmeldung mit durch Benutzer zugewiesenen Identitäten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3211">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="15ad5-3212">Role</span><span class="sxs-lookup"><span data-stu-id="15ad5-3212">Role</span></span>

* <span data-ttu-id="15ad5-3213">Argument `--assignee-object-id` zu `role assignment create` hinzugefügt, um Graph-Abfrage zu umgehen</span><span class="sxs-lookup"><span data-stu-id="15ad5-3213">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="15ad5-3214">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="15ad5-3214">Service Fabric</span></span>

* <span data-ttu-id="15ad5-3215">Ausführliche Fehler zur Überprüfungsantwort bei der Clustererstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3215">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="15ad5-3216">Problem mit fehlendem Client für verschiedene Befehle behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-3216">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="15ad5-3217">VM</span><span class="sxs-lookup"><span data-stu-id="15ad5-3217">VM</span></span>

* <span data-ttu-id="15ad5-3218">[VORSCHAUVERSION] Zonenübergreifende Unterstützung für `vmss`</span><span class="sxs-lookup"><span data-stu-id="15ad5-3218">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="15ad5-3219">[BREAKING CHANGE] Standard für Einzelzone (`vmss`) in Standardlastenausgleich geändert</span><span class="sxs-lookup"><span data-stu-id="15ad5-3219">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="15ad5-3220">[BREAKING CHANGE]`externalIdentities` in `userAssignedIdentities` geändert für EMSI</span><span class="sxs-lookup"><span data-stu-id="15ad5-3220">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="15ad5-3221">[VORSCHAUVERSION] Unterstützung für Austausch des Betriebssystemdatenträgers hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3221">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="15ad5-3222">Unterstützung der Verwendung von VM-Images aus anderen Abonnements hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3222">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="15ad5-3223">Argumente `--plan-name`, `--plan-product`, `--plan-promotion-code` und `--plan-publisher` zu `[vm|vmss] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3223">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="15ad5-3224">Fehlerbedingte Probleme mit `[vm|vmss] create` behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-3224">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="15ad5-3225">Übermäßige Ressourcenverwendung durch `vm image list --all` behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-3225">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="15ad5-3226">19. Dezember 2017</span><span class="sxs-lookup"><span data-stu-id="15ad5-3226">December 19, 2017</span></span>

<span data-ttu-id="15ad5-3227">Version 2.0.23</span><span class="sxs-lookup"><span data-stu-id="15ad5-3227">Version 2.0.23</span></span>

* <span data-ttu-id="15ad5-3228">Unterstützung für die Anmeldung mit durch Benutzer zugewiesenen Identitäten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3228">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="15ad5-3229">Container</span><span class="sxs-lookup"><span data-stu-id="15ad5-3229">Container</span></span>

* <span data-ttu-id="15ad5-3230">Falsche Reihenfolge der Parameter für Containerprotokolle behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-3230">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="15ad5-3231">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="15ad5-3231">Network</span></span>

* <span data-ttu-id="15ad5-3232">Argument `--disable-bgp-route-propagation` zu `route-table [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3232">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="15ad5-3233">Argument `--ip-tags` zu `public-ip [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3233">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="15ad5-3234">Storage</span><span class="sxs-lookup"><span data-stu-id="15ad5-3234">Storage</span></span>

* <span data-ttu-id="15ad5-3235">Unterstützung für Storage V2 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3235">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="15ad5-3236">VM</span><span class="sxs-lookup"><span data-stu-id="15ad5-3236">VM</span></span>

* <span data-ttu-id="15ad5-3237">[VORSCHAUVERSION] Unterstützung für durch Benutzer zugewiesene Identitäten für virtuelle Computer und VMSSs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3237">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="15ad5-3238">5\. Dezember 2017</span><span class="sxs-lookup"><span data-stu-id="15ad5-3238">December 5, 2017</span></span>

<span data-ttu-id="15ad5-3239">Version 2.0.22</span><span class="sxs-lookup"><span data-stu-id="15ad5-3239">Version 2.0.22</span></span>

* <span data-ttu-id="15ad5-3240">`az component`-Befehle wurden entfernt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-3240">Removed `az component` commands.</span></span> <span data-ttu-id="15ad5-3241">Verwenden Sie stattdessen `az extension`.</span><span class="sxs-lookup"><span data-stu-id="15ad5-3241">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="15ad5-3242">Core</span><span class="sxs-lookup"><span data-stu-id="15ad5-3242">Core</span></span>
* <span data-ttu-id="15ad5-3243">Der `AZURE_US_GOV_CLOUD`-Autoritätsendpunkt von AAD wurde von „login.microsoftonline.com“ in „login.microsoftonline.us“ geändert.</span><span class="sxs-lookup"><span data-stu-id="15ad5-3243">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="15ad5-3244">Problem behoben, aufgrund dessen Telemetriedaten fortlaufend neu gesendet wurden</span><span class="sxs-lookup"><span data-stu-id="15ad5-3244">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="15ad5-3245">ACS</span><span class="sxs-lookup"><span data-stu-id="15ad5-3245">ACS</span></span>

* <span data-ttu-id="15ad5-3246">Die Befehle `aks install-connector` und `aks remove-connector` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-3246">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="15ad5-3247">Verbesserte Fehlerberichterstellung für `acs create`</span><span class="sxs-lookup"><span data-stu-id="15ad5-3247">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="15ad5-3248">Feste Verwendung von `aks get-credentials -f` ohne vollqualifizierten Pfad</span><span class="sxs-lookup"><span data-stu-id="15ad5-3248">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="15ad5-3249">Advisor</span><span class="sxs-lookup"><span data-stu-id="15ad5-3249">Advisor</span></span>

* <span data-ttu-id="15ad5-3250">Erste Veröffentlichung</span><span class="sxs-lookup"><span data-stu-id="15ad5-3250">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="15ad5-3251">AppService</span><span class="sxs-lookup"><span data-stu-id="15ad5-3251">Appservice</span></span>

* <span data-ttu-id="15ad5-3252">Erstellung feststehender Zertifikatnamen mit `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="15ad5-3252">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="15ad5-3253">`webapp [list|show]` und `functionapp [list|show]` wurden verbessert, um die richtigen Apps anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="15ad5-3253">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="15ad5-3254">Standardwert für `WEBSITE_NODE_DEFAULT_VERSION` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3254">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="15ad5-3255">Nutzung</span><span class="sxs-lookup"><span data-stu-id="15ad5-3255">Consumption</span></span>

* <span data-ttu-id="15ad5-3256">Unterstützung für API-Version 2017-11-30 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3256">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="15ad5-3257">Container</span><span class="sxs-lookup"><span data-stu-id="15ad5-3257">Container</span></span>

* <span data-ttu-id="15ad5-3258">Feste Regression für Standardports</span><span class="sxs-lookup"><span data-stu-id="15ad5-3258">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="15ad5-3259">Überwachen</span><span class="sxs-lookup"><span data-stu-id="15ad5-3259">Monitor</span></span>

* <span data-ttu-id="15ad5-3260">Unterstützung mehrerer Dimensionen zu Metrikbefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3260">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="15ad5-3261">Resource</span><span class="sxs-lookup"><span data-stu-id="15ad5-3261">Resource</span></span>

* <span data-ttu-id="15ad5-3262">Argument `--include-response-body` zu `resource show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3262">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="15ad5-3263">Role</span><span class="sxs-lookup"><span data-stu-id="15ad5-3263">Role</span></span>

* <span data-ttu-id="15ad5-3264">Anzeige von Standardzuweisungen für „klassische“ Administratoren zu `role assignment list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3264">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="15ad5-3265">Unterstützung für das Hinzufügen (anstelle der Überschreibung) von Anmeldeinformationen zu `ad sp reset-credentials` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3265">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="15ad5-3266">Verbesserte Fehlerberichterstellung für `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="15ad5-3266">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="15ad5-3267">SQL</span><span class="sxs-lookup"><span data-stu-id="15ad5-3267">SQL</span></span>

* <span data-ttu-id="15ad5-3268">Die Befehle `sql db list-usages` und `sql db show-usage` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-3268">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="15ad5-3269">Die Befehle `sql server conn-policy show` und `sql server conn-policy update` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-3269">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="15ad5-3270">VM</span><span class="sxs-lookup"><span data-stu-id="15ad5-3270">VM</span></span>

* <span data-ttu-id="15ad5-3271">Zoneninformationen zu `az vm list-skus` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3271">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="15ad5-3272">14. November 2017</span><span class="sxs-lookup"><span data-stu-id="15ad5-3272">November 14, 2017</span></span>

<span data-ttu-id="15ad5-3273">Version 2.0.21</span><span class="sxs-lookup"><span data-stu-id="15ad5-3273">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="15ad5-3274">ACR</span><span class="sxs-lookup"><span data-stu-id="15ad5-3274">ACR</span></span>

* <span data-ttu-id="15ad5-3275">Unterstützung für das Erstellen von Webhooks in Replikationsregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3275">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="15ad5-3276">ACS</span><span class="sxs-lookup"><span data-stu-id="15ad5-3276">ACS</span></span>

* <span data-ttu-id="15ad5-3277">Formulierung in AKS von „Agent“ in „Knoten“ geändert</span><span class="sxs-lookup"><span data-stu-id="15ad5-3277">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="15ad5-3278">Option `--orchestrator-release` für `acs create` als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="15ad5-3278">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="15ad5-3279">VM-Standardgröße für AKS in `Standard_D1_v2` geändert</span><span class="sxs-lookup"><span data-stu-id="15ad5-3279">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="15ad5-3280">`az aks browse` für Windows korrigiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-3280">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="15ad5-3281">`az aks get-credentials` für Windows korrigiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-3281">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="15ad5-3282">AppService</span><span class="sxs-lookup"><span data-stu-id="15ad5-3282">Appservice</span></span>

* <span data-ttu-id="15ad5-3283">Bereitstellungsquelle `config-zip` für Web-Apps und Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3283">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="15ad5-3284">Option `--docker-container-logging` zu `az webapp log config` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3284">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="15ad5-3285">Option `storage` aus dem Parameter `--web-server-logging` von `az webapp log config` entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3285">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="15ad5-3286">Fehlermeldungen für `deployment user set` verbessert</span><span class="sxs-lookup"><span data-stu-id="15ad5-3286">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="15ad5-3287">Unterstützung für das Erstellen von Linux-Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3287">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="15ad5-3288">`list-locations` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="15ad5-3288">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="15ad5-3289">Batch</span><span class="sxs-lookup"><span data-stu-id="15ad5-3289">Batch</span></span>

* <span data-ttu-id="15ad5-3290">Fehler im Poolerstellungsbefehl korrigiert, der bei Verwendung einer Ressourcen-ID mit dem Flag `--image` aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="15ad5-3290">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="15ad5-3291">BatchAI</span><span class="sxs-lookup"><span data-stu-id="15ad5-3291">Batchai</span></span>

* <span data-ttu-id="15ad5-3292">Kurzoption (`-s`) für `--vm-size` zur Angabe der VM-Größe im Befehl `file-server create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3292">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="15ad5-3293">Argumente für Speicherkontoname und -schlüssel zum Parameter `cluster create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3293">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="15ad5-3294">Dokumentation für `job list-files` und `job stream-file` korrigiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-3294">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="15ad5-3295">Kurzoption (`-r`) für `--cluster-name` zur Angabe des Clusternamens im Befehl `job create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3295">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="15ad5-3296">Cloud</span><span class="sxs-lookup"><span data-stu-id="15ad5-3296">Cloud</span></span>

* <span data-ttu-id="15ad5-3297">`cloud [register|update]` geändert, um die Registrierung von Clouds ohne erforderliche Endpunkte zu verhindern</span><span class="sxs-lookup"><span data-stu-id="15ad5-3297">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="15ad5-3298">Container</span><span class="sxs-lookup"><span data-stu-id="15ad5-3298">Container</span></span>

* <span data-ttu-id="15ad5-3299">Unterstützung für das Öffnen mehrerer Ports hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3299">Added support to open multiple ports</span></span>
* <span data-ttu-id="15ad5-3300">Neustartrichtlinie für Containergruppen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3300">Added container group restart policy</span></span>
* <span data-ttu-id="15ad5-3301">Unterstützung zum Einbinden einer Azure-Dateifreigabe als Volume hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3301">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="15ad5-3302">Hilfedokumente aktualisiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-3302">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="15ad5-3303">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="15ad5-3303">Data Lake Analytics</span></span>

* <span data-ttu-id="15ad5-3304">`[job|account] list` geändert, um präzisere Informationen zu erhalten</span><span class="sxs-lookup"><span data-stu-id="15ad5-3304">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="15ad5-3305">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="15ad5-3305">Data Lake Store</span></span>

* <span data-ttu-id="15ad5-3306">`account list` geändert, um präzisere Informationen zu erhalten</span><span class="sxs-lookup"><span data-stu-id="15ad5-3306">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="15ad5-3307">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="15ad5-3307">Extension</span></span>

* <span data-ttu-id="15ad5-3308">`extension list-available` hinzugefügt, um das Auflisten offizieller Microsoft-Erweiterungen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="15ad5-3308">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="15ad5-3309">`--name` zu `extension [add|update]` hinzugefügt, um das Installieren von Erweiterungen nach Name zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="15ad5-3309">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="15ad5-3310">IoT</span><span class="sxs-lookup"><span data-stu-id="15ad5-3310">IoT</span></span>

* <span data-ttu-id="15ad5-3311">Unterstützung für Zertifizierungsstellen (CAs) und Zertifikatketten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3311">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="15ad5-3312">Überwachen</span><span class="sxs-lookup"><span data-stu-id="15ad5-3312">Monitor</span></span>

* <span data-ttu-id="15ad5-3313">Befehle vom Typ `activity-log alert` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3313">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="15ad5-3314">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="15ad5-3314">Network</span></span>

* <span data-ttu-id="15ad5-3315">Unterstützung für CAA-DNS-Einträge hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3315">Added support for CAA DNS records</span></span>
* <span data-ttu-id="15ad5-3316">Problem behoben, durch das Endpunkte nicht mit `traffic-manager profile update` aktualisiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="15ad5-3316">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="15ad5-3317">Problem behoben, durch das `vnet update --dns-servers` je nach VNet-Erstellungsmethode nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="15ad5-3317">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="15ad5-3318">Problem behoben, durch das relative DNS-Namen durch `dns zone import` nicht korrekt importiert wurden</span><span class="sxs-lookup"><span data-stu-id="15ad5-3318">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="15ad5-3319">Reservations</span><span class="sxs-lookup"><span data-stu-id="15ad5-3319">Reservations</span></span>

* <span data-ttu-id="15ad5-3320">Erste Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="15ad5-3320">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="15ad5-3321">Resource</span><span class="sxs-lookup"><span data-stu-id="15ad5-3321">Resource</span></span>

* <span data-ttu-id="15ad5-3322">Unterstützung für Ressourcen-IDs zum Parameter `--resource` und Sperren auf Ressourcenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3322">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="15ad5-3323">SQL</span><span class="sxs-lookup"><span data-stu-id="15ad5-3323">SQL</span></span>

* <span data-ttu-id="15ad5-3324">Parameter `--ignore-missing-vnet-service-endpoint` zu `sql server vnet-rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3324">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="15ad5-3325">Storage</span><span class="sxs-lookup"><span data-stu-id="15ad5-3325">Storage</span></span>

* <span data-ttu-id="15ad5-3326">`storage account create` geändert, sodass die SKU `Standard_RAGRS` als Standard verwendet wird</span><span class="sxs-lookup"><span data-stu-id="15ad5-3326">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="15ad5-3327">Fehler im Zusammenhang mit Datei-/Blobnamen korrigiert, die ASCII-fremde Zeichen enthalten</span><span class="sxs-lookup"><span data-stu-id="15ad5-3327">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="15ad5-3328">Fehler korrigiert, der die Verwendung von `--source-uri` mit `storage [blob|file] copy start-batch` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="15ad5-3328">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="15ad5-3329">Befehle zum Globalisieren und Löschen mehrerer Objekte mit `storage [blob|file] delete-batch` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3329">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="15ad5-3330">Problem beim Aktivieren von Metriken mit `storage metrics update` behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-3330">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="15ad5-3331">Problem mit Dateien über 200 GB bei Verwendung von `storage blob upload-batch` behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-3331">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="15ad5-3332">Problem behoben, durch das `--bypass` und `--default-action` von `storage account [create|update]` ignoriert wurden</span><span class="sxs-lookup"><span data-stu-id="15ad5-3332">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="15ad5-3333">VM</span><span class="sxs-lookup"><span data-stu-id="15ad5-3333">VM</span></span>

* <span data-ttu-id="15ad5-3334">Fehler mit `vmss create` korrigiert, der die Verwendung der Größenebene `Basic` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="15ad5-3334">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="15ad5-3335">`--plan`-Argumente zu `[vm|vmss] create` für benutzerdefinierte Images mit Abrechnungsinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3335">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="15ad5-3336">Befehle hinzugefügt: `vm secret `[add|remove|list]</span><span class="sxs-lookup"><span data-stu-id="15ad5-3336">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="15ad5-3337">`vm format-secret` in `vm secret format` umbenannt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3337">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="15ad5-3338">Argument `--encrypt format` zu `vm encryption enable` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3338">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="15ad5-3339">24. Oktober 2017</span><span class="sxs-lookup"><span data-stu-id="15ad5-3339">October 24, 2017</span></span>

<span data-ttu-id="15ad5-3340">Version 2.0.20</span><span class="sxs-lookup"><span data-stu-id="15ad5-3340">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="15ad5-3341">Core</span><span class="sxs-lookup"><span data-stu-id="15ad5-3341">Core</span></span>

* <span data-ttu-id="15ad5-3342">Aktualisierung von `2017-03-09-profile` zur Verwendung von Version `2016-01-01` der `MGMT_STORAGE`-API</span><span class="sxs-lookup"><span data-stu-id="15ad5-3342">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="15ad5-3343">ACR</span><span class="sxs-lookup"><span data-stu-id="15ad5-3343">ACR</span></span>

* <span data-ttu-id="15ad5-3344">Die Ressourcenverwaltung wurde aktualisiert und verweist nun auf die API-Version `2017-10-01`.</span><span class="sxs-lookup"><span data-stu-id="15ad5-3344">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="15ad5-3345">SKU „Bring Your Own Storage“ wurde in „Klassisch“ geändert.</span><span class="sxs-lookup"><span data-stu-id="15ad5-3345">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="15ad5-3346">Die Registrierungs-SKUs wurden in „Basic“, „Standard“ und „Premium“ umbenannt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-3346">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="15ad5-3347">ACS</span><span class="sxs-lookup"><span data-stu-id="15ad5-3347">ACS</span></span>

* <span data-ttu-id="15ad5-3348">[VORSCHAUVERSION] Befehle vom Typ `az aks` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3348">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="15ad5-3349">Problem mit `get-credentials` in Kubernetes behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-3349">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="15ad5-3350">AppService</span><span class="sxs-lookup"><span data-stu-id="15ad5-3350">Appservice</span></span>

* <span data-ttu-id="15ad5-3351">Problem behoben, aufgrund dessen heruntergeladene `webapp`-Protokolle unter Umständen ungültig waren</span><span class="sxs-lookup"><span data-stu-id="15ad5-3351">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="15ad5-3352">Komponente</span><span class="sxs-lookup"><span data-stu-id="15ad5-3352">Component</span></span>

* <span data-ttu-id="15ad5-3353">Deutlichere Meldung zur Einstellung für alle Installer und für Bestätigungsaufforderung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3353">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="15ad5-3354">Überwachen</span><span class="sxs-lookup"><span data-stu-id="15ad5-3354">Monitor</span></span>

* <span data-ttu-id="15ad5-3355">Befehle vom Typ `action-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3355">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="15ad5-3356">Resource</span><span class="sxs-lookup"><span data-stu-id="15ad5-3356">Resource</span></span>

* <span data-ttu-id="15ad5-3357">Inkompatibilität mit der aktuellen Version der msrest-Abhängigkeit in `group export` behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-3357">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="15ad5-3358">Problem mit `policy assignment create` behoben, sodass der Befehl mit integrierten Richtliniendefinitionen und Richtliniensatzdefinitionen verwendet werden kann</span><span class="sxs-lookup"><span data-stu-id="15ad5-3358">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="15ad5-3359">VM</span><span class="sxs-lookup"><span data-stu-id="15ad5-3359">VM</span></span>

* <span data-ttu-id="15ad5-3360">Argument `--accelerated-networking` zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3360">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="15ad5-3361">9\. Oktober 2017</span><span class="sxs-lookup"><span data-stu-id="15ad5-3361">October 9, 2017</span></span>

<span data-ttu-id="15ad5-3362">Version 2.0.19</span><span class="sxs-lookup"><span data-stu-id="15ad5-3362">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="15ad5-3363">Core</span><span class="sxs-lookup"><span data-stu-id="15ad5-3363">Core</span></span>

* <span data-ttu-id="15ad5-3364">Verarbeitung von ADFS-Autoritäts-URLs wurde mit einem nachgestellten Schrägstrich zu Azure Stack hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-3364">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="15ad5-3365">AppService</span><span class="sxs-lookup"><span data-stu-id="15ad5-3365">Appservice</span></span>

* <span data-ttu-id="15ad5-3366">Mit dem neuen Befehl `webapp update` wurde ein allgemeines Update hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-3366">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="15ad5-3367">Batch</span><span class="sxs-lookup"><span data-stu-id="15ad5-3367">Batch</span></span>

* <span data-ttu-id="15ad5-3368">Aktualisierung auf Batch SDK 4.0.0</span><span class="sxs-lookup"><span data-stu-id="15ad5-3368">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="15ad5-3369">Die Option `--image` von „VirtualMachineConfiguration“ wurde aktualisiert, um zusätzlich zu „publish:offer:sku:version“ ARM-Imageverweise zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="15ad5-3369">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="15ad5-3370">Unterstützung für das neue CLI-Erweiterungsmodell für Batch-Erweiterungsbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3370">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="15ad5-3371">Batch-Unterstützung aus dem Komponentenmodell entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3371">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="15ad5-3372">BatchAI</span><span class="sxs-lookup"><span data-stu-id="15ad5-3372">Batchai</span></span>

* <span data-ttu-id="15ad5-3373">Erste Version des Batch KI-Moduls</span><span class="sxs-lookup"><span data-stu-id="15ad5-3373">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="15ad5-3374">KeyVault</span><span class="sxs-lookup"><span data-stu-id="15ad5-3374">Keyvault</span></span>

* <span data-ttu-id="15ad5-3375">Key Vault-Authentifizierungsproblem behoben, das bei Verwendung von ADFS in Azure Stack auftrat.</span><span class="sxs-lookup"><span data-stu-id="15ad5-3375">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="15ad5-3376">(#4448)</span><span class="sxs-lookup"><span data-stu-id="15ad5-3376">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="15ad5-3377">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="15ad5-3377">Network</span></span>

* <span data-ttu-id="15ad5-3378">Das Argument `--server` von `application-gateway address-pool create` ist nun optional, sodass leere Adresspools zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="15ad5-3378">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="15ad5-3379">`traffic-manager` wurde aktualisiert, um aktuelle Features zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="15ad5-3379">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="15ad5-3380">Resource</span><span class="sxs-lookup"><span data-stu-id="15ad5-3380">Resource</span></span>

* <span data-ttu-id="15ad5-3381">Zusätzliche Unterstützung für `--resource-group/-g`-Optionen für Ressourcengruppennamen zu `group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3381">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="15ad5-3382">Befehle für `account lock` hinzugefügt, um die Verwendung mit Sperren auf Abonnementebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="15ad5-3382">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="15ad5-3383">Befehle für `group lock` hinzugefügt, um die Verwendung mit Sperren auf Gruppenebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="15ad5-3383">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="15ad5-3384">Befehle für `resource lock` hinzugefügt, um die Verwendung mit Sperren auf Ressourcenebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="15ad5-3384">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="15ad5-3385">Sql</span><span class="sxs-lookup"><span data-stu-id="15ad5-3385">Sql</span></span>

* <span data-ttu-id="15ad5-3386">Unterstützung für SQL Transparent Data Encryption (TDE) und TDE für Bring Your Own Key-Szenarien hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3386">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="15ad5-3387">Der Befehl `db list-deleted` und der Parameter `db restore --deleted-time` wurden hinzugefügt, um die Ermittlung und Wiederherstellung gelöschter Datenbanken zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="15ad5-3387">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="15ad5-3388">`db op list` und `db op cancel` wurden hinzugefügt, um das Auflisten und Abbrechen ausgeführter Vorgänge für eine Datenbank zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="15ad5-3388">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="15ad5-3389">Storage</span><span class="sxs-lookup"><span data-stu-id="15ad5-3389">Storage</span></span>

* <span data-ttu-id="15ad5-3390">Unterstützung für Momentaufnahme von Dateifreigaben hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3390">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="15ad5-3391">VM</span><span class="sxs-lookup"><span data-stu-id="15ad5-3391">Vm</span></span>

* <span data-ttu-id="15ad5-3392">Korrektur eines Fehlers in `vm show`, bei dem die Verwendung von `-d` in Verbindung mit fehlenden privaten IP-Adressen einen Absturz verursachte</span><span class="sxs-lookup"><span data-stu-id="15ad5-3392">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="15ad5-3393">[VORSCHAUVERSION] Unterstützung für paralleles Upgrade zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3393">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="15ad5-3394">Unterstützung für das Aktualisieren der Verschlüsselungseinstellungen mit `vm encryption enable` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3394">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="15ad5-3395">Parameter `--os-disk-size-gb` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3395">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="15ad5-3396">Parameter `--license-type` für Windows zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3396">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="15ad5-3397">22. September 2017</span><span class="sxs-lookup"><span data-stu-id="15ad5-3397">September 22, 2017</span></span>

<span data-ttu-id="15ad5-3398">Version 2.0.18</span><span class="sxs-lookup"><span data-stu-id="15ad5-3398">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="15ad5-3399">Resource</span><span class="sxs-lookup"><span data-stu-id="15ad5-3399">Resource</span></span>

* <span data-ttu-id="15ad5-3400">Unterstützung für das Anzeigen integrierter Richtliniendefinitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3400">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="15ad5-3401">Unterstützungsmodusparameter zum Erstellen von Richtliniendefinitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3401">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="15ad5-3402">Unterstützung für UI-Definitionen und -Vorlagen zu `managedapp definition create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3402">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="15ad5-3403">[BREAKING CHANGE] Der Ressourcentyp `managedapp` wurde von `appliances` in `applications` und von `applianceDefinitions` in `applicationDefinitions` geändert.</span><span class="sxs-lookup"><span data-stu-id="15ad5-3403">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="15ad5-3404">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="15ad5-3404">Network</span></span>

* <span data-ttu-id="15ad5-3405">Unterstützung für Verfügbarkeitszone zu Unterbefehlen `network lb` und `network public-ip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3405">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="15ad5-3406">Unterstützung für IPv6-Microsoft-Peering zu `express-route` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3406">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="15ad5-3407">Befehle für Anwendungssicherheitsgruppe `asg` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3407">Added `asg` application security group commands</span></span>
* <span data-ttu-id="15ad5-3408">Argument `--application-security-groups` zu `nic [create|ip-config create|ip-config update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3408">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="15ad5-3409">Argumente `--source-asgs` und `--destination-asgs` zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3409">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="15ad5-3410">Argumente `--ddos-protection` und `--vm-protection` zu `vnet [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3410">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="15ad5-3411">Befehle vom Typ `network [vnet-gateway|vpn-client|show-url]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3411">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="15ad5-3412">Storage</span><span class="sxs-lookup"><span data-stu-id="15ad5-3412">Storage</span></span>

* <span data-ttu-id="15ad5-3413">Problem behoben, das nach der Aktualisierung des SDK unter Umständen einen Fehler der `storage account network-rule`-Befehle zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="15ad5-3413">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="15ad5-3414">Eventgrid</span><span class="sxs-lookup"><span data-stu-id="15ad5-3414">Eventgrid</span></span>

* <span data-ttu-id="15ad5-3415">Azure Event Grid Python SDK für die Verwendung der neueren API-Version „2017-09-15-preview“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-3415">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="15ad5-3416">SQL</span><span class="sxs-lookup"><span data-stu-id="15ad5-3416">SQL</span></span>

* <span data-ttu-id="15ad5-3417">`sql server list`-Argument `--resource-group` geändert, sodass es nun optional ist.</span><span class="sxs-lookup"><span data-stu-id="15ad5-3417">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="15ad5-3418">Wird es nicht angegeben, werden alle SQL Server-Instanzen im Abonnement zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="15ad5-3418">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="15ad5-3419">Parameter `--no-wait` zu `db [create|copy|restore|update|replica create|create|update]` und `dw [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3419">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="15ad5-3420">KeyVault</span><span class="sxs-lookup"><span data-stu-id="15ad5-3420">Keyvault</span></span>

* <span data-ttu-id="15ad5-3421">Unterstützung für die Keyvault-Befehlsausführung hinter einem Proxy hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3421">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="15ad5-3422">VM</span><span class="sxs-lookup"><span data-stu-id="15ad5-3422">VM</span></span>

* <span data-ttu-id="15ad5-3423">Unterstützung für Verfügbarkeitszone zu `[vm|vmss|disk] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3423">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="15ad5-3424">Problem behoben, das bei Verwendung von `--app-gateway ID` mit `vmss create` einen Fehler zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="15ad5-3424">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="15ad5-3425">Argument `--asgs` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3425">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="15ad5-3426">Unterstützung für die Ausführung von Befehlen auf virtuellen Computern mit `vm run-command` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3426">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="15ad5-3427">[VORSCHAU] Unterstützung für VMSS-Datenträgerverschlüsselung mit `vmss encryption` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3427">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="15ad5-3428">Unterstützung für die Durchführung der Wartung auf virtuellen Computern mit `vm perform-maintenance` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3428">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="15ad5-3429">ACS</span><span class="sxs-lookup"><span data-stu-id="15ad5-3429">ACS</span></span>

* <span data-ttu-id="15ad5-3430">[VORSCHAU] Argument `--orchestrator-release` zu `acs create` für ACS-Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3430">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="15ad5-3431">AppService</span><span class="sxs-lookup"><span data-stu-id="15ad5-3431">Appservice</span></span>

* <span data-ttu-id="15ad5-3432">Neue Möglichkeit zum Aktualisieren und Anzeigen der Authentifizierungseinstellungen mit `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="15ad5-3432">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="15ad5-3433">Backup</span><span class="sxs-lookup"><span data-stu-id="15ad5-3433">Backup</span></span>

* <span data-ttu-id="15ad5-3434">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="15ad5-3434">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="15ad5-3435">11. September 2017</span><span class="sxs-lookup"><span data-stu-id="15ad5-3435">September 11, 2017</span></span>

<span data-ttu-id="15ad5-3436">Version 2.0.17</span><span class="sxs-lookup"><span data-stu-id="15ad5-3436">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="15ad5-3437">Core</span><span class="sxs-lookup"><span data-stu-id="15ad5-3437">Core</span></span>

* <span data-ttu-id="15ad5-3438">Festlegung einer eigenen Korrelations-ID in Telemetrie durch das Befehlsmodul aktiviert</span><span class="sxs-lookup"><span data-stu-id="15ad5-3438">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="15ad5-3439">Ein Problem mit der JSON-Sicherungsdatei wurde behoben, das beim Festlegen des Diagnosemodus für Telemetrie auftrat</span><span class="sxs-lookup"><span data-stu-id="15ad5-3439">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="15ad5-3440">ACS</span><span class="sxs-lookup"><span data-stu-id="15ad5-3440">Acs</span></span>

* <span data-ttu-id="15ad5-3441">Befehl `acs list-locations` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3441">Added `acs list-locations` command</span></span>
* <span data-ttu-id="15ad5-3442">`ssh-key-file` wird mit dem erwarteten Standardwert versehen.</span><span class="sxs-lookup"><span data-stu-id="15ad5-3442">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="15ad5-3443">AppService</span><span class="sxs-lookup"><span data-stu-id="15ad5-3443">Appservice</span></span>

* <span data-ttu-id="15ad5-3444">Neue Möglichkeit zum Erstellen einer Web-App in einer anderen Ressourcengruppe als der des aktiven Diensttarifs</span><span class="sxs-lookup"><span data-stu-id="15ad5-3444">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="15ad5-3445">CDN</span><span class="sxs-lookup"><span data-stu-id="15ad5-3445">CDN</span></span>

* <span data-ttu-id="15ad5-3446">Der Fehler bei `cdn custom-domain create`, dass „CustomDomain“ nicht wiederholbar ist, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="15ad5-3446">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="15ad5-3447">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="15ad5-3447">Extension</span></span>

* <span data-ttu-id="15ad5-3448">Erstrelease</span><span class="sxs-lookup"><span data-stu-id="15ad5-3448">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="15ad5-3449">KeyVault</span><span class="sxs-lookup"><span data-stu-id="15ad5-3449">Keyvault</span></span>

* <span data-ttu-id="15ad5-3450">Problem behoben, aufgrund dessen bei den Berechtigungen für `keyvault set-policy` die Groß-/Kleinschreibung beachtet werden musste</span><span class="sxs-lookup"><span data-stu-id="15ad5-3450">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="15ad5-3451">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="15ad5-3451">Network</span></span>

* <span data-ttu-id="15ad5-3452">`vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3452">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="15ad5-3453">Das Argument `--private-access-services` wurde für `vnet subnet create/update` in `--service-endpoints` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-3453">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="15ad5-3454">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3454">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="15ad5-3455">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3455">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="15ad5-3456">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3456">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="15ad5-3457">Resource</span><span class="sxs-lookup"><span data-stu-id="15ad5-3457">Resource</span></span>

* <span data-ttu-id="15ad5-3458">Übergabe von Parameterdefinitionen für Ressourcenrichtlinien in `policy definition create` und `policy definition update` zulassen</span><span class="sxs-lookup"><span data-stu-id="15ad5-3458">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="15ad5-3459">Übergabe von Parameterwerten für `policy assignment create` zulassen</span><span class="sxs-lookup"><span data-stu-id="15ad5-3459">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="15ad5-3460">Übergabe von JSON-Code oder einer Datei für alle Parameter zulassen</span><span class="sxs-lookup"><span data-stu-id="15ad5-3460">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="15ad5-3461">Inkrementierte API-Version</span><span class="sxs-lookup"><span data-stu-id="15ad5-3461">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="15ad5-3462">SQL</span><span class="sxs-lookup"><span data-stu-id="15ad5-3462">SQL</span></span>

* <span data-ttu-id="15ad5-3463">Befehle vom Typ `sql server vnet-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3463">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="15ad5-3464">VM</span><span class="sxs-lookup"><span data-stu-id="15ad5-3464">VM</span></span>

* <span data-ttu-id="15ad5-3465">Behoben: Zugriff nur zuweisen, wenn `--scope` angegeben wird</span><span class="sxs-lookup"><span data-stu-id="15ad5-3465">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="15ad5-3466">Behoben: Gleiche Erweiterungsbenennung wie Portal verwenden</span><span class="sxs-lookup"><span data-stu-id="15ad5-3466">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="15ad5-3467">`subscription` aus der Ausgabe von `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3467">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="15ad5-3468">Behoben: Speicher-SKU vom Typ `[vm|vmss] create` wird nicht auf Datenträger mit einem Image angewendet.</span><span class="sxs-lookup"><span data-stu-id="15ad5-3468">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="15ad5-3469">Behoben: `vm format-secret --secrets` akzeptierte keine durch neue Zeilen getrennte IDs.</span><span class="sxs-lookup"><span data-stu-id="15ad5-3469">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="15ad5-3470">31. August 2017</span><span class="sxs-lookup"><span data-stu-id="15ad5-3470">August 31, 2017</span></span>

<span data-ttu-id="15ad5-3471">Version 2.0.16</span><span class="sxs-lookup"><span data-stu-id="15ad5-3471">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="15ad5-3472">KeyVault</span><span class="sxs-lookup"><span data-stu-id="15ad5-3472">Keyvault</span></span>

* <span data-ttu-id="15ad5-3473">Fehler behoben, der beim Versuch auftrat, die Geheimniscodierung mit `secret download` automatisch aufzulösen</span><span class="sxs-lookup"><span data-stu-id="15ad5-3473">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="15ad5-3474">Sf</span><span class="sxs-lookup"><span data-stu-id="15ad5-3474">Sf</span></span>

* <span data-ttu-id="15ad5-3475">Alle Befehle wurden durch die Service Fabric-Befehlszeilenschnittstelle (sfctl) ersetzt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-3475">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="15ad5-3476">Storage</span><span class="sxs-lookup"><span data-stu-id="15ad5-3476">Storage</span></span>

* <span data-ttu-id="15ad5-3477">Problem behoben, aufgrund dessen Speicherkonten nicht in Regionen erstellt werden konnten, die die NetworkACLs-Funktion nicht unterstützen</span><span class="sxs-lookup"><span data-stu-id="15ad5-3477">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="15ad5-3478">Festlegen des Inhaltstyps und der Inhaltscodierung während Blob- und Dateiuploads, wenn weder Inhaltstyp noch Inhaltscodierung angegeben sind</span><span class="sxs-lookup"><span data-stu-id="15ad5-3478">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="15ad5-3479">28. August 2017</span><span class="sxs-lookup"><span data-stu-id="15ad5-3479">August 28, 2017</span></span>

<span data-ttu-id="15ad5-3480">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="15ad5-3480">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="15ad5-3481">Befehlszeilenschnittstelle (CLI)</span><span class="sxs-lookup"><span data-stu-id="15ad5-3481">CLI</span></span>

* <span data-ttu-id="15ad5-3482">Rechtlichen Hinweis zu `--version` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3482">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="15ad5-3483">ACS</span><span class="sxs-lookup"><span data-stu-id="15ad5-3483">ACS</span></span>

* <span data-ttu-id="15ad5-3484">Vorschauregionen korrigiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-3484">Corrected preview regions</span></span>
* <span data-ttu-id="15ad5-3485">Standardmäßiges DNS-Namenspräfix (`dns_name_prefix`) ordnungsgemäß formatiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-3485">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="15ad5-3486">ACS-Befehlsausgabe optimiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-3486">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="15ad5-3487">AppService</span><span class="sxs-lookup"><span data-stu-id="15ad5-3487">Appservice</span></span>

* <span data-ttu-id="15ad5-3488">[BREAKING CHANGE] Inkonsistenzen in der Ausgabe von `az webapp config appsettings [delete|set]` behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-3488">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="15ad5-3489">Neuen Alias (`-i`) für `az webapp config container set --docker-custom-image-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3489">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="15ad5-3490">`az webapp log show` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="15ad5-3490">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="15ad5-3491">Neue Argumente aus `az webapp delete` verfügbar gemacht, um App Service-Plan, Metriken oder DNS-Registrierung beizubehalten</span><span class="sxs-lookup"><span data-stu-id="15ad5-3491">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="15ad5-3492">Behoben: Korrekte Erkennung der Sloteinstellungen</span><span class="sxs-lookup"><span data-stu-id="15ad5-3492">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="15ad5-3493">IoT</span><span class="sxs-lookup"><span data-stu-id="15ad5-3493">IoT</span></span>

* <span data-ttu-id="15ad5-3494">#3934 behoben: Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="15ad5-3494">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="15ad5-3495">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="15ad5-3495">Network</span></span>

* <span data-ttu-id="15ad5-3496">[BREAKING CHANGE]`vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3496">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="15ad5-3497">[BREAKING CHANGE] Option `--private-access-services` für `--service-endpoints` in `vnet subnet [create|update]` umbenannt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3497">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="15ad5-3498">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3498">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="15ad5-3499">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3499">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="15ad5-3500">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3500">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="15ad5-3501">Profil</span><span class="sxs-lookup"><span data-stu-id="15ad5-3501">Profile</span></span>

* <span data-ttu-id="15ad5-3502">`--msi` und `--msi-port` für die Anmeldung mit der Identität eines virtuellen Computers verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="15ad5-3502">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="15ad5-3503">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="15ad5-3503">Service Fabric</span></span>

* <span data-ttu-id="15ad5-3504">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="15ad5-3504">Preview release</span></span>
* <span data-ttu-id="15ad5-3505">Registrierungsbenutzer-/-kennwortregeln für Befehl vereinfacht</span><span class="sxs-lookup"><span data-stu-id="15ad5-3505">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="15ad5-3506">Kennwortanforderung für Benutzer trotz Parameterübergabe behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-3506">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="15ad5-3507">Unterstützung für leere Registrierungsanmeldeinformationen (`registry_cred`) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3507">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="15ad5-3508">Storage</span><span class="sxs-lookup"><span data-stu-id="15ad5-3508">Storage</span></span>

* <span data-ttu-id="15ad5-3509">Festlegen des Blobtarifs ermöglicht</span><span class="sxs-lookup"><span data-stu-id="15ad5-3509">Enabled setting blob tier</span></span>
* <span data-ttu-id="15ad5-3510">Argumente `--bypass` und `--default-action` zur Unterstützung von Diensttunneling zu `storage account [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3510">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="15ad5-3511">Befehle zum Hinzufügen von VNet-Regeln und IP-basierten Regeln zu `storage account network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3511">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="15ad5-3512">Dienstverschlüsselung durch vom Kunden verwalteten Schlüssel ermöglicht</span><span class="sxs-lookup"><span data-stu-id="15ad5-3512">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="15ad5-3513">[BREAKING CHANGE] Option `--encryption` für Befehl `az storage account create and az storage account update` in `--encryption-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3513">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="15ad5-3514">Behoben (4220): `az storage account update encryption` – Syntaxkonflikt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3514">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="15ad5-3515">VM</span><span class="sxs-lookup"><span data-stu-id="15ad5-3515">VM</span></span>

* <span data-ttu-id="15ad5-3516">Problem behoben, aufgrund dessen bei Verwendung von `--instance-id *` zusätzliche, fehlerhafte Informationen für `vmss get-instance-view` angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="15ad5-3516">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="15ad5-3517">Unterstützung für `--lb-sku` zu `vmss create` hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="15ad5-3517">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="15ad5-3518">Menschliche Namen aus der Administratornamen-Blacklist für `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3518">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="15ad5-3519">Problem behoben, aufgrund dessen `[vm|vmss] create` einen Fehler ausgelöst hat, wenn aus einem Image keine Tarifinformationen extrahiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="15ad5-3519">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="15ad5-3520">Absturzproblem beim Erstellen einer VMMS-Skalierungsgruppe mit einem internen Lastenausgleich behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-3520">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="15ad5-3521">Problem behoben, aufgrund dessen das Argument `--no-wait` nicht mit `vm availability-set create` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="15ad5-3521">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="15ad5-3522">15. August 2017</span><span class="sxs-lookup"><span data-stu-id="15ad5-3522">August 15, 2017</span></span>

<span data-ttu-id="15ad5-3523">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="15ad5-3523">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="15ad5-3524">ACS</span><span class="sxs-lookup"><span data-stu-id="15ad5-3524">ACS</span></span>

* <span data-ttu-id="15ad5-3525">sshMaster0-Portnummer für Kubernetes korrigiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-3525">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="15ad5-3526">AppService</span><span class="sxs-lookup"><span data-stu-id="15ad5-3526">Appservice</span></span>

* <span data-ttu-id="15ad5-3527">Ausnahme beim Erstellen einer neuen Git-basierten Linux-Web-App behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-3527">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="15ad5-3528">Event Grid</span><span class="sxs-lookup"><span data-stu-id="15ad5-3528">Event Grid</span></span>

* <span data-ttu-id="15ad5-3529">SDK-Abhängigkeiten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3529">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="15ad5-3530">11. August 2017</span><span class="sxs-lookup"><span data-stu-id="15ad5-3530">August 11, 2017</span></span>

<span data-ttu-id="15ad5-3531">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="15ad5-3531">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="15ad5-3532">ACS</span><span class="sxs-lookup"><span data-stu-id="15ad5-3532">ACS</span></span>

* <span data-ttu-id="15ad5-3533">Weitere Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3533">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="15ad5-3534">Batch</span><span class="sxs-lookup"><span data-stu-id="15ad5-3534">Batch</span></span>

* <span data-ttu-id="15ad5-3535">Auf Batch SDK 3.1.0 und Batch Management SDK 4.1.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-3535">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="15ad5-3536">Neuen Befehl zum Anzeigen der Aufgabenanzahl eines Auftrags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3536">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="15ad5-3537">Fehler in der SAS-URL-Verarbeitung der Ressourcendatei behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-3537">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="15ad5-3538">Batch-Kontoendpunkt unterstützt nun optionales Präfix „https://“</span><span class="sxs-lookup"><span data-stu-id="15ad5-3538">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="15ad5-3539">Unterstützung für das Hinzufügen von Listen mit mehr als 100 Aufgaben zu einem Auftrag</span><span class="sxs-lookup"><span data-stu-id="15ad5-3539">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="15ad5-3540">Debugprotokollierung für das Laden des Erweiterungsbefehlsmoduls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3540">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="15ad5-3541">Komponente</span><span class="sxs-lookup"><span data-stu-id="15ad5-3541">Component</span></span>

* <span data-ttu-id="15ad5-3542">Warnung für veraltete Befehle vom Typ „az component“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3542">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="15ad5-3543">Container</span><span class="sxs-lookup"><span data-stu-id="15ad5-3543">Container</span></span>

* <span data-ttu-id="15ad5-3544">`create`: Problem behoben, aufgrund dessen das Gleichheitszeichen innerhalb einer Umgebungsvariablen nicht zulässig war</span><span class="sxs-lookup"><span data-stu-id="15ad5-3544">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="15ad5-3545">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="15ad5-3545">Data Lake Store</span></span>

* <span data-ttu-id="15ad5-3546">Fortschrittsüberwachung ermöglicht</span><span class="sxs-lookup"><span data-stu-id="15ad5-3546">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="15ad5-3547">Event Grid</span><span class="sxs-lookup"><span data-stu-id="15ad5-3547">Event Grid</span></span>

* <span data-ttu-id="15ad5-3548">Erste Veröffentlichung</span><span class="sxs-lookup"><span data-stu-id="15ad5-3548">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="15ad5-3549">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="15ad5-3549">Network</span></span>

* <span data-ttu-id="15ad5-3550">`lb`: Problem behoben, aufgrund dessen bestimmte Namen untergeordneter Ressourcen bei Auslassung nicht richtig aufgelöst wurden</span><span class="sxs-lookup"><span data-stu-id="15ad5-3550">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="15ad5-3551">`application-gateway {subresource} delete`: Problem behoben, aufgrund dessen `--no-wait` nicht berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="15ad5-3551">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="15ad5-3552">`application-gateway http-settings update`: Problem behoben, aufgrund dessen `--connection-draining-timeout` nicht deaktiviert werden konnte</span><span class="sxs-lookup"><span data-stu-id="15ad5-3552">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="15ad5-3553">Fehler behoben: Unerwartetes Schlüsselwortargument `sa_data_size_kilobyes` bei `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="15ad5-3553">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="15ad5-3554">Profil</span><span class="sxs-lookup"><span data-stu-id="15ad5-3554">Profile</span></span>

* <span data-ttu-id="15ad5-3555">`account list`: `--refresh` hinzugefügt, um die neuesten Abonnements vom Server zu synchronisieren</span><span class="sxs-lookup"><span data-stu-id="15ad5-3555">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="15ad5-3556">Storage</span><span class="sxs-lookup"><span data-stu-id="15ad5-3556">Storage</span></span>

* <span data-ttu-id="15ad5-3557">Aktualisieren des Speicherkontos mit vom System zugewiesener Identität ermöglicht</span><span class="sxs-lookup"><span data-stu-id="15ad5-3557">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="15ad5-3558">VM</span><span class="sxs-lookup"><span data-stu-id="15ad5-3558">VM</span></span>

* <span data-ttu-id="15ad5-3559">`availability-set`: Fehlerdomänenanzahl bei Konvertierung verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="15ad5-3559">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="15ad5-3560">Befehl `list-skus` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="15ad5-3560">Exposed `list-skus` command</span></span>
* <span data-ttu-id="15ad5-3561">Unterstützung der Identitätszuweisung ohne Erstellung von Rollenzuweisungen</span><span class="sxs-lookup"><span data-stu-id="15ad5-3561">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="15ad5-3562">Anwenden von Speicher-SKU beim Anfügen von Datenträgern</span><span class="sxs-lookup"><span data-stu-id="15ad5-3562">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="15ad5-3563">Standardmäßiger Betriebssystemdatenträger-Name und Speicher-SKU bei Verwendung verwalteter Datenträger entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3563">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="15ad5-3564">28. Juli 2017</span><span class="sxs-lookup"><span data-stu-id="15ad5-3564">July 28, 2017</span></span>

<span data-ttu-id="15ad5-3565">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="15ad5-3565">Version 2.0.12</span></span>

* <span data-ttu-id="15ad5-3566">Containerbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3566">Added container commands</span></span>
* <span data-ttu-id="15ad5-3567">Abrechnungs- und Nutzungsmodule hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3567">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="15ad5-3568">Core</span><span class="sxs-lookup"><span data-stu-id="15ad5-3568">Core</span></span>

* <span data-ttu-id="15ad5-3569">Ausgabe von SDK-Authentifizierungsinformationen für Dienstprinzipale mit Zertifikaten</span><span class="sxs-lookup"><span data-stu-id="15ad5-3569">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="15ad5-3570">Ausnahmen beim Bereitstellungsfortschritt behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-3570">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="15ad5-3571">Verwendung des ARM-Endpunkts aus der aktuellen Cloud für die Erstellung des Abonnementclients</span><span class="sxs-lookup"><span data-stu-id="15ad5-3571">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="15ad5-3572">Gleichzeitige Verarbeitung der Datei „clouds.config“ verbessert (3636)</span><span class="sxs-lookup"><span data-stu-id="15ad5-3572">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="15ad5-3573">Aktualisierung der Clientanforderungs-ID für jede Befehlsausführung</span><span class="sxs-lookup"><span data-stu-id="15ad5-3573">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="15ad5-3574">Erstellung von Abonnementclients mit richtigem SDK-Profil (3635)</span><span class="sxs-lookup"><span data-stu-id="15ad5-3574">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="15ad5-3575">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="15ad5-3575">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="15ad5-3576">Unterstützung für Auswahl von Tabellenausgabefeldern über jmespath Abfrage hinzugefügt (3581)</span><span class="sxs-lookup"><span data-stu-id="15ad5-3576">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="15ad5-3577">Stummschaltung von Analyseargumenten und Anfügeverlauf mit Gesten verbessert (3434)</span><span class="sxs-lookup"><span data-stu-id="15ad5-3577">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="15ad5-3578">Erstellung von Abonnementclients mit richtigem SDK-Profil</span><span class="sxs-lookup"><span data-stu-id="15ad5-3578">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="15ad5-3579">Verschiebung aller vorhandenen Erfassungsdateien in den neuesten Ordner</span><span class="sxs-lookup"><span data-stu-id="15ad5-3579">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="15ad5-3580">Idempotenz für VM-/VMSS-Erstellung behoben (3586)</span><span class="sxs-lookup"><span data-stu-id="15ad5-3580">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="15ad5-3581">Bei Befehlspfaden wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="15ad5-3581">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="15ad5-3582">Bei bestimmten booleschen Parametern wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="15ad5-3582">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="15ad5-3583">Unterstützung der Anmeldung bei lokalem AD FS-Server wie Azure Stack</span><span class="sxs-lookup"><span data-stu-id="15ad5-3583">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="15ad5-3584">Gleichzeitige Schreibvorgänge in „clouds.config“ behoben (3255)</span><span class="sxs-lookup"><span data-stu-id="15ad5-3584">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="15ad5-3585">ACR</span><span class="sxs-lookup"><span data-stu-id="15ad5-3585">ACR</span></span>

* <span data-ttu-id="15ad5-3586">Befehl `show-usage` für verwaltete Registrierungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3586">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="15ad5-3587">Unterstützung der SKU-Aktualisierung für verwaltete Registrierungen</span><span class="sxs-lookup"><span data-stu-id="15ad5-3587">Support SKU update for managed registries</span></span>
* <span data-ttu-id="15ad5-3588">Verwaltete Registrierungen mit verwalteter SKU hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3588">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="15ad5-3589">Webhooks für verwaltete Registrierungen mit ACR-Webhook-Befehlsmodul hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3589">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="15ad5-3590">AAD-Authentifizierung mit ACR-Anmeldebefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3590">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="15ad5-3591">Löschbefehl für Docker-Repositorys, Manifeste und Tags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3591">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="15ad5-3592">ACS</span><span class="sxs-lookup"><span data-stu-id="15ad5-3592">ACS</span></span>

* <span data-ttu-id="15ad5-3593">Unterstützung der API-Version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="15ad5-3593">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="15ad5-3594">AppService</span><span class="sxs-lookup"><span data-stu-id="15ad5-3594">Appservice</span></span>

* <span data-ttu-id="15ad5-3595">Fehler behoben, aufgrund dessen die Auflistung der Linux-Web-App keine Werte zurückgegeben hat</span><span class="sxs-lookup"><span data-stu-id="15ad5-3595">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="15ad5-3596">Unterstützung für das Abrufen von Anmeldeinformationen aus dem ACR</span><span class="sxs-lookup"><span data-stu-id="15ad5-3596">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="15ad5-3597">Entfernung aller Befehle unter `appservice web`</span><span class="sxs-lookup"><span data-stu-id="15ad5-3597">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="15ad5-3598">Maskierung von Docker-Registrierungskennwörtern aus der Befehlsausgabe (3656)</span><span class="sxs-lookup"><span data-stu-id="15ad5-3598">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="15ad5-3599">Gewährleistung der fehlerfreien Verwendung des Standardbrowsers unter macOS (3623)</span><span class="sxs-lookup"><span data-stu-id="15ad5-3599">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="15ad5-3600">Verbesserung des Nutzens von `webapp log tail` und `webapp log download` (3624)</span><span class="sxs-lookup"><span data-stu-id="15ad5-3600">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="15ad5-3601">Befehl `traffic-routing` zum Konfigurieren des statischen Routings verfügbar gemacht (3566)</span><span class="sxs-lookup"><span data-stu-id="15ad5-3601">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="15ad5-3602">Zuverlässigkeit beim Konfigurieren der Quellcodeverwaltung verbessert (3245)</span><span class="sxs-lookup"><span data-stu-id="15ad5-3602">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="15ad5-3603">Nicht unterstütztes Argument `--node-version` aus `webapp config update` für Windows-Web-Apps entfernt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-3603">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="15ad5-3604">Verwenden Sie stattdessen `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="15ad5-3604">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="15ad5-3605">Batch</span><span class="sxs-lookup"><span data-stu-id="15ad5-3605">Batch</span></span>

* <span data-ttu-id="15ad5-3606">Auf Batch SDK 3.0.0 mit Unterstützung virtueller Computer mit niedriger Priorität in Pools aktualisiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-3606">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="15ad5-3607">`pool create`-Option `--target-dedicated` in `--target-dedicated-nodes` umbenannt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3607">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="15ad5-3608">`pool create`-Optionen `--target-low-priority-nodes` und `--application-licenses` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3608">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="15ad5-3609">CDN</span><span class="sxs-lookup"><span data-stu-id="15ad5-3609">CDN</span></span>

* <span data-ttu-id="15ad5-3610">Besser verständliche Fehlermeldung für `cdn endpoint list`, wenn das von `--profile-name` angegebene Profil nicht vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="15ad5-3610">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="15ad5-3611">Cloud</span><span class="sxs-lookup"><span data-stu-id="15ad5-3611">Cloud</span></span>

* <span data-ttu-id="15ad5-3612">API-Version des Cloudmetadaten-Endpunkts in das Format JJJJ-MM-TT umgewandelt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3612">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="15ad5-3613">Katalogendpunkt nicht erforderlich</span><span class="sxs-lookup"><span data-stu-id="15ad5-3613">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="15ad5-3614">Unterstützung für die Cloudregistrierung nur mit ARM-Endpunkt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3614">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="15ad5-3615">Option für `cloud set` bereitgestellt, um beim Auswählen der aktuellen Cloud das Profil auswählen zu können</span><span class="sxs-lookup"><span data-stu-id="15ad5-3615">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="15ad5-3616">`endpoint_vm_image_alias_doc` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="15ad5-3616">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="15ad5-3617">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="15ad5-3617">CosmosDB</span></span>

* <span data-ttu-id="15ad5-3618">Möglichkeit zum Erstellen einer Auflistung mit benutzerdefiniertem Partitionsschlüssel behoben</span><span class="sxs-lookup"><span data-stu-id="15ad5-3618">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="15ad5-3619">Unterstützung für Auflistungs-Standardgültigkeitsdauer hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3619">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="15ad5-3620">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="15ad5-3620">Data Lake Analytics</span></span>

* <span data-ttu-id="15ad5-3621">Zusätzliche Befehle für Compute-Richtlinienverwaltung unter der Überschrift `dla account compute-policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3621">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="15ad5-3622">`dla job pipeline show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3622">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="15ad5-3623">`dla job recurrence list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3623">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="15ad5-3624">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="15ad5-3624">Data Lake Store</span></span>

* <span data-ttu-id="15ad5-3625">Unterstützung für vom Benutzer verwaltete Schlüsseltresor-Schlüsselrotation in `dls account update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3625">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="15ad5-3626">Zugrunde liegende SDK-Version des Data Lake Store-Dateisystems aktualisiert, um ein Leistungsproblem zu behandeln</span><span class="sxs-lookup"><span data-stu-id="15ad5-3626">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="15ad5-3627">Befehl `dls enable-key-vault` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-3627">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="15ad5-3628">Dieser Befehl versucht, eine vom Benutzer angegebene Key Vault-Instanz zur Verschlüsselung der Daten in einem Data Lake Store-Konto zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="15ad5-3628">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="15ad5-3629">Interactive</span><span class="sxs-lookup"><span data-stu-id="15ad5-3629">Interactive</span></span>

* <span data-ttu-id="15ad5-3630">Startzeit durch Verwendung zwischengespeicherter Befehle verbessert</span><span class="sxs-lookup"><span data-stu-id="15ad5-3630">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="15ad5-3631">Testabdeckung verbessert</span><span class="sxs-lookup"><span data-stu-id="15ad5-3631">Increased test coverage</span></span>
* <span data-ttu-id="15ad5-3632">?-Geste erweitert, sodass sie auch in den nächsten Befehl eingefügt wird</span><span class="sxs-lookup"><span data-stu-id="15ad5-3632">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="15ad5-3633">Interaktive Fehler mit dem Profil „2017-03-09-profile-preview“ behoben (3587)</span><span class="sxs-lookup"><span data-stu-id="15ad5-3633">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="15ad5-3634">`--version` als Parameter für den interaktiven Modus zugelassen (3645)</span><span class="sxs-lookup"><span data-stu-id="15ad5-3634">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="15ad5-3635">Beseitigung von Fehlern im interaktiven Modus beim Abschluss von Überprüfungen (3570)</span><span class="sxs-lookup"><span data-stu-id="15ad5-3635">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="15ad5-3636">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="15ad5-3636">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="15ad5-3637">Flag `--progress` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3637">Added `--progress` flag</span></span>
* <span data-ttu-id="15ad5-3638">`--debug` und `--verbose` aus Abschlüssen entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3638">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="15ad5-3639">`interactive` aus Abschlüssen entfernt (3324)</span><span class="sxs-lookup"><span data-stu-id="15ad5-3639">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="15ad5-3640">IoT</span><span class="sxs-lookup"><span data-stu-id="15ad5-3640">IoT</span></span>

* <span data-ttu-id="15ad5-3641">Behoben: Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="15ad5-3641">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="15ad5-3642">(3934)</span><span class="sxs-lookup"><span data-stu-id="15ad5-3642">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="15ad5-3643">Schlüsseltresor</span><span class="sxs-lookup"><span data-stu-id="15ad5-3643">Key vault</span></span>

* <span data-ttu-id="15ad5-3644">Befehle für Schlüsseltresor-Wiederherstellungsfeatures hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="15ad5-3644">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="15ad5-3645">`keyvault`-Unterbefehle: `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="15ad5-3645">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="15ad5-3646">`keyvault secret`-Unterbefehle: `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="15ad5-3646">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="15ad5-3647">`keyvault certificate`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="15ad5-3647">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="15ad5-3648">`keyvault key`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="15ad5-3648">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="15ad5-3649">Dienstprinzipal-Schlüsseltresorintegration hinzugefügt (3133)</span><span class="sxs-lookup"><span data-stu-id="15ad5-3649">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="15ad5-3650">Schlüsseltresor-Datenebene auf 0.3.2. aktualisiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-3650">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="15ad5-3651">(3307)</span><span class="sxs-lookup"><span data-stu-id="15ad5-3651">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="15ad5-3652">Labor</span><span class="sxs-lookup"><span data-stu-id="15ad5-3652">Lab</span></span>

* <span data-ttu-id="15ad5-3653">Unterstützung für Übernahme eines beliebigen virtuellen Computers im Labor über `az lab vm claim` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3653">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="15ad5-3654">Tabellenausgabeformatierer für `az lab vm list` und `az lab vm show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3654">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="15ad5-3655">Überwachen</span><span class="sxs-lookup"><span data-stu-id="15ad5-3655">Monitor</span></span>

* <span data-ttu-id="15ad5-3656">Korrektur für Vorlagendatei mit Befehl `monitor autoscale-settings get-parameters-template` (3349)</span><span class="sxs-lookup"><span data-stu-id="15ad5-3656">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="15ad5-3657">`monitor alert-rule-incidents list` in `monitor alert list-incidents` umbenannt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3657">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="15ad5-3658">`monitor alert-rule-incidents show` in `monitor alert show-incident` umbenannt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3658">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="15ad5-3659">`monitor metric-defintions list` in `monitor metrics list-definitions` umbenannt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3659">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="15ad5-3660">`monitor alert-rules` in `monitor alert` umbenannt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3660">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="15ad5-3661">`monitor alert create` geändert:</span><span class="sxs-lookup"><span data-stu-id="15ad5-3661">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="15ad5-3662">Unterbefehle vom Typ `condition` und `action` akzeptieren keinen JSON-Code mehr.</span><span class="sxs-lookup"><span data-stu-id="15ad5-3662">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="15ad5-3663">Hinzufügung zahlreicher Parameter zur Vereinfachung der Regelerstellung</span><span class="sxs-lookup"><span data-stu-id="15ad5-3663">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="15ad5-3664">`location` nicht mehr erforderlich</span><span class="sxs-lookup"><span data-stu-id="15ad5-3664">`location` no longer required</span></span>
  * <span data-ttu-id="15ad5-3665">Hinzufügung von Namen- und ID-Unterstützung für Ziel</span><span class="sxs-lookup"><span data-stu-id="15ad5-3665">Add name and ID support for target</span></span>
  * <span data-ttu-id="15ad5-3666">Entfernung von `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="15ad5-3666">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="15ad5-3667">Umbenennung von `is-enabled` in `enabled` (nicht mehr erforderlich)</span><span class="sxs-lookup"><span data-stu-id="15ad5-3667">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="15ad5-3668">`description` wird nun abhängig von der angegebenen Bedingung auf einen Standardwert festgelegt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-3668">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="15ad5-3669">Hinzufügung von Beispielen zur Verdeutlichung des neuen Formats</span><span class="sxs-lookup"><span data-stu-id="15ad5-3669">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="15ad5-3670">Unterstützung von Namen oder IDs für Befehle vom Typ `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="15ad5-3670">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="15ad5-3671">Komfortargumente und Beispiele zu `monitor alert rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3671">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="15ad5-3672">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="15ad5-3672">Network</span></span>

* <span data-ttu-id="15ad5-3673">Befehl `list-private-access-services` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3673">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="15ad5-3674">Argument `--private-access-services` zu `vnet subnet create` und `vnet subnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3674">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="15ad5-3675">Problem behoben, das einen Fehler für `application-gateway redirect-config create` zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="15ad5-3675">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="15ad5-3676">Problem behoben, aufgrund dessen `application-gateway redirect-config update` nicht mit `--no-wait` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="15ad5-3676">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="15ad5-3677">Fehler behoben, der bei der Verwendung des Arguments `--servers` mit `application-gateway address-pool create` und `application-gateway address-pool update` aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="15ad5-3677">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="15ad5-3678">Befehle vom Typ `application-gateway redirect-config` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3678">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="15ad5-3679">Befehle zu `application-gateway ssl-policy` hinzugefügt: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="15ad5-3679">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="15ad5-3680">Argumente zu `application-gateway ssl-policy set` hinzugefügt: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="15ad5-3680">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="15ad5-3681">Argumente zu `application-gateway http-settings create` und `application-gateway http-settings update` hinzugefügt: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="15ad5-3681">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="15ad5-3682">Argumente zu `application-gateway url-path-map create` und `application-gateway url-path-map update` hinzugefügt: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="15ad5-3682">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="15ad5-3683">Argument `--redirect-config` zu `application-gateway url-path-map rule create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3683">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="15ad5-3684">Unterstützung für `--no-wait` zu `application-gateway url-path-map rule delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3684">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="15ad5-3685">Argumente zu `application-gateway probe create` und `application-gateway probe update` hinzugefügt: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="15ad5-3685">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="15ad5-3686">Argument `--redirect-config` zu `application-gateway rule create` und `application-gateway rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3686">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="15ad5-3687">Unterstützung für `--accelerated-networking` zu `nic create` und `nic update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3687">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="15ad5-3688">Argument `--internal-dns-name-suffix` von `nic create` entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3688">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="15ad5-3689">Unterstützung für `--dns-servers` zu `nic update` und `nic create` hinzugefügt: Hinzufügung von Unterstützung für --dns-servers</span><span class="sxs-lookup"><span data-stu-id="15ad5-3689">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="15ad5-3690">Fehler korrigiert, aufgrund dessen `--local-address-prefixes` von `local-gateway create` ignoriert wurde</span><span class="sxs-lookup"><span data-stu-id="15ad5-3690">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="15ad5-3691">Unterstützung für `--dns-servers` zu `vnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3691">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="15ad5-3692">Fehler beim Erstellen eines Peerings ohne Routenfilterung mit `express-route peering create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-3692">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="15ad5-3693">Fehler korrigiert, aufgrund dessen die Argumente `--provider` und `--bandwidth` nicht mit `express-route update` verwendet werden konnten</span><span class="sxs-lookup"><span data-stu-id="15ad5-3693">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="15ad5-3694">Fehler mit Standardlogik von `network watcher show-topology` korrigiert</span><span class="sxs-lookup"><span data-stu-id="15ad5-3694">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="15ad5-3695">Ausgabeformatierung für `network list-usages` verbessert</span><span class="sxs-lookup"><span data-stu-id="15ad5-3695">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="15ad5-3696">Verwendung der standardmäßigen Front-End-IP-Adresse für `application-gateway http-listener create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="15ad5-3696">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="15ad5-3697">Verwendung des Standardadresspools, der HTTP-Standardeinstellungen und des HTTP-Standardlisteners für `application-gateway rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="15ad5-3697">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="15ad5-3698">Verwendung der standardmäßigen Front-End-IP-Adresse und des standardmäßigen Back-End-Pools für `lb rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="15ad5-3698">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="15ad5-3699">Verwendung der standardmäßigen Front-End-IP-Adresse für `lb inbound-nat-rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="15ad5-3699">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="15ad5-3700">Profil</span><span class="sxs-lookup"><span data-stu-id="15ad5-3700">Profile</span></span>

* <span data-ttu-id="15ad5-3701">Unterstützung der Anmeldung innerhalb eines virtuellen Computers mit einer verwalteten Identität</span><span class="sxs-lookup"><span data-stu-id="15ad5-3701">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="15ad5-3702">Unterstützung der Ausgabe für `account show` im SDK-Authentifizierungsdateiformat</span><span class="sxs-lookup"><span data-stu-id="15ad5-3702">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="15ad5-3703">Anzeige von Warnungen für veraltete Befehle bei Verwendung von „--expanded-view“</span><span class="sxs-lookup"><span data-stu-id="15ad5-3703">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="15ad5-3704">Befehl `get-access-token` für die Bereitstellung eines unformatierten AAD-Tokens hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3704">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="15ad5-3705">Unterstützung der Anmeldung mit einem Benutzerkonto ohne zugeordnete Abonnements</span><span class="sxs-lookup"><span data-stu-id="15ad5-3705">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="15ad5-3706">RDBMS</span><span class="sxs-lookup"><span data-stu-id="15ad5-3706">RDBMS</span></span>

* <span data-ttu-id="15ad5-3707">Unterstützung der abonnementübergreifenden Auflistung von Servern (3417)</span><span class="sxs-lookup"><span data-stu-id="15ad5-3707">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="15ad5-3708">Behoben: `%s` wird aufgrund von fehlendem `% server_type` nicht verarbeitet (3393)</span><span class="sxs-lookup"><span data-stu-id="15ad5-3708">Fixed `%s` not processed because of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="15ad5-3709">Dokumentquellenzuordnung behoben und CI-Aufgabe zur Überprüfung hinzugefügt (3361)</span><span class="sxs-lookup"><span data-stu-id="15ad5-3709">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="15ad5-3710">MySQL- und PostgreSQL-Hilfe korrigiert (3369)</span><span class="sxs-lookup"><span data-stu-id="15ad5-3710">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="15ad5-3711">Resource</span><span class="sxs-lookup"><span data-stu-id="15ad5-3711">Resource</span></span>

* <span data-ttu-id="15ad5-3712">Eingabeaufforderungen bei fehlenden Parametern für `group deployment create` verbessert</span><span class="sxs-lookup"><span data-stu-id="15ad5-3712">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="15ad5-3713">Analyse der Syntax `--parameters KEY=VALUE` verbessert</span><span class="sxs-lookup"><span data-stu-id="15ad5-3713">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="15ad5-3714">Probleme behoben, durch die Parameterdateien von `group deployment create` bei Verwendung der Syntax `@<file>` nicht mehr erkannt wurden</span><span class="sxs-lookup"><span data-stu-id="15ad5-3714">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="15ad5-3715">Unterstützung des Arguments `--ids` für Befehle vom Typ `resource` und `managedapp`</span><span class="sxs-lookup"><span data-stu-id="15ad5-3715">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="15ad5-3716">Einige Analyse- und Fehlermeldungen korrigiert (3584)</span><span class="sxs-lookup"><span data-stu-id="15ad5-3716">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="15ad5-3717">Analyse vom Typ `--resource-type` für den Befehl `lock` korrigiert, sodass `<resource-namespace>` und `<resource-type>` akzeptiert werden</span><span class="sxs-lookup"><span data-stu-id="15ad5-3717">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="15ad5-3718">Parameterüberprüfung für Vorlagenlinkvorlagen hinzugefügt (3629)</span><span class="sxs-lookup"><span data-stu-id="15ad5-3718">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="15ad5-3719">Unterstützung für die Angabe von Bereitstellungsparametern mit der Syntax `KEY=VALUE` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3719">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="15ad5-3720">Role</span><span class="sxs-lookup"><span data-stu-id="15ad5-3720">Role</span></span>

* <span data-ttu-id="15ad5-3721">Unterstützung der Ausgabe im SDK-Authentifizierungsdateiformat für `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="15ad5-3721">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="15ad5-3722">Rollenzuweisungen und dazugehörige AAD-Anwendung beim Löschen eines Dienstprinzipals bereinigt (3610)</span><span class="sxs-lookup"><span data-stu-id="15ad5-3722">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="15ad5-3723">Einbeziehung des Zeitformats in Beschreibungen vom Typ `--start-date` und `--end-date` für `app create`-Argumente</span><span class="sxs-lookup"><span data-stu-id="15ad5-3723">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="15ad5-3724">Anzeige von Warnungen für veraltete Befehle bei Verwendung von `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="15ad5-3724">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="15ad5-3725">Schlüsseltresorintegration zu den Befehlen `create-for-rbac` und `reset-credentials` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3725">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="15ad5-3726">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="15ad5-3726">Service Fabric</span></span>
* <span data-ttu-id="15ad5-3727">Problem behoben, aufgrund dessen große Dateien in Anwendungen beim Hochladen gekürzt wurden (3666)</span><span class="sxs-lookup"><span data-stu-id="15ad5-3727">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="15ad5-3728">Tests für Service Fabric-Befehle hinzugefügt (3424)</span><span class="sxs-lookup"><span data-stu-id="15ad5-3728">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="15ad5-3729">Zahlreiche Service Fabric-Befehle korrigiert (3234)</span><span class="sxs-lookup"><span data-stu-id="15ad5-3729">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="15ad5-3730">SQL</span><span class="sxs-lookup"><span data-stu-id="15ad5-3730">SQL</span></span>

* <span data-ttu-id="15ad5-3731">Fehlerhafte1 Parameter `--identity` für `sql server create` entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3731">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="15ad5-3732">Kennwortwerte aus der Befehlsausgabe von `sql server create` und `sql server update` entfernt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3732">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="15ad5-3733">Befehle `sql db list-editions` und `sql elastic-pool list-editions` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3733">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="15ad5-3734">Storage</span><span class="sxs-lookup"><span data-stu-id="15ad5-3734">Storage</span></span>

* <span data-ttu-id="15ad5-3735">Option `--marker` für die Befehle `storage blob list`, `storage container list` und `storage share list` entfernt (3745)</span><span class="sxs-lookup"><span data-stu-id="15ad5-3735">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="15ad5-3736">Erstellung eines reinen HTTPS-Speicherkontos ermöglicht</span><span class="sxs-lookup"><span data-stu-id="15ad5-3736">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="15ad5-3737">Speichermetriken, Protokollierung und CORS-Befehle aktualisiert (3495)</span><span class="sxs-lookup"><span data-stu-id="15ad5-3737">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="15ad5-3738">Ausnahmemeldung von „cors add“ umformuliert (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="15ad5-3738">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="15ad5-3739">Generator im Probelaufmodus des Downloadbatchbefehls in eine Liste konvertiert (3592)</span><span class="sxs-lookup"><span data-stu-id="15ad5-3739">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="15ad5-3740">Problem bei Probelauf des Blobdownloadbatchs behoben (3640) (3592)</span><span class="sxs-lookup"><span data-stu-id="15ad5-3740">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="15ad5-3741">VM</span><span class="sxs-lookup"><span data-stu-id="15ad5-3741">VM</span></span>

* <span data-ttu-id="15ad5-3742">Unterstützung der NSG-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="15ad5-3742">Support configuring nsg</span></span>
* <span data-ttu-id="15ad5-3743">Fehler behoben, aufgrund dessen der DNS-Server nicht ordnungsgemäß konfiguriert wurde</span><span class="sxs-lookup"><span data-stu-id="15ad5-3743">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="15ad5-3744">Unterstützung verwalteter Dienstidentitäten</span><span class="sxs-lookup"><span data-stu-id="15ad5-3744">Support managed service identities</span></span>
* <span data-ttu-id="15ad5-3745">Problem behoben, aufgrund dessen `cmss create` mit einem vorhandenen Lastenausgleich `--backend-pool-name` benötigte</span><span class="sxs-lookup"><span data-stu-id="15ad5-3745">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="15ad5-3746">Festlegung, dass die LUN von mit `vm image create` erstellten Datenträgern mit 0 beginnt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3746">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="15ad5-3747">10. Mai 2017</span><span class="sxs-lookup"><span data-stu-id="15ad5-3747">May 10, 2017</span></span>

<span data-ttu-id="15ad5-3748">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="15ad5-3748">Version 2.0.6</span></span>

* <span data-ttu-id="15ad5-3749">Umbenennen von „documentdb“ in „cosmosdb“</span><span class="sxs-lookup"><span data-stu-id="15ad5-3749">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="15ad5-3750">Hinzufügen von rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="15ad5-3750">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="15ad5-3751">Einbeziehen der Data Lake Analytics- und Data Lake Store-Module</span><span class="sxs-lookup"><span data-stu-id="15ad5-3751">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="15ad5-3752">Einbeziehen des Cognitive Services-Moduls</span><span class="sxs-lookup"><span data-stu-id="15ad5-3752">Include Cognitive Services module</span></span>
* <span data-ttu-id="15ad5-3753">Einbeziehen des Service Fabric-Moduls</span><span class="sxs-lookup"><span data-stu-id="15ad5-3753">Include Service Fabric module</span></span>
* <span data-ttu-id="15ad5-3754">Einbeziehen des interaktiven Moduls (Umbenennen von „az-shell“)</span><span class="sxs-lookup"><span data-stu-id="15ad5-3754">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="15ad5-3755">Hinzufügen von Unterstützung für CDN-Befehle</span><span class="sxs-lookup"><span data-stu-id="15ad5-3755">Add support for CDN commands</span></span>
* <span data-ttu-id="15ad5-3756">Entfernen des Containermoduls</span><span class="sxs-lookup"><span data-stu-id="15ad5-3756">Remove Container module</span></span>
* <span data-ttu-id="15ad5-3757">Hinzufügen von „az -v“ als Verknüpfung für „az --version“ ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="15ad5-3757">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="15ad5-3758">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="15ad5-3758">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="15ad5-3759">Core</span><span class="sxs-lookup"><span data-stu-id="15ad5-3759">Core</span></span>

* <span data-ttu-id="15ad5-3760">Core: Erfassen von Ausnahmen, die durch einen nicht registrierten Anbieter verursacht werden, und automatische Registrierung</span><span class="sxs-lookup"><span data-stu-id="15ad5-3760">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="15ad5-3761">Leistung: Dauerhaftes Speichern des ADAL-Tokencaches im Arbeitsspeicher bis zum Prozessende ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="15ad5-3761">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="15ad5-3762">Korrigieren der vom hexadezimalen Fingerabdruck -o tsv zurückgegebenen Bytes ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="15ad5-3762">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="15ad5-3763">Verbessern des Downloads des Schlüsseltresorzertifikats und der AAD-SP-Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="15ad5-3763">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="15ad5-3764">Hinzufügen des Python-Speicherorts zu „az –version“ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="15ad5-3764">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="15ad5-3765">Anmeldung: Unterstützung der Anmeldung, wenn keine Abonnements vorhanden sind ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="15ad5-3765">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="15ad5-3766">Core: Beheben eines Fehlers bei zweimaliger Verwendung eines Dienstprinzipals bei der Anmeldung ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="15ad5-3766">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="15ad5-3767">Core: Ermöglichen der Konfiguration des Dateipfads von „accessTokens.json“ über eine Umgebungsvariable ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="15ad5-3767">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="15ad5-3768">Core: Zulassen der Anwendung konfigurierter Standardwerte auf optionale Argumente ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="15ad5-3768">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="15ad5-3769">Core: Verbesserte Leistung</span><span class="sxs-lookup"><span data-stu-id="15ad5-3769">core: Improved performance</span></span>
* <span data-ttu-id="15ad5-3770">Core: Zertifikate von benutzerdefinierter Zertifizierungsstelle – Unterstützung für das Festlegen der REQUESTS_CA_BUNDLE-Umgebungsvariablen</span><span class="sxs-lookup"><span data-stu-id="15ad5-3770">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="15ad5-3771">Core: Cloudkonfiguration – Verwenden des Endpunkts „resource manager“, wenn Endpunkt „management“ nicht festgelegt ist</span><span class="sxs-lookup"><span data-stu-id="15ad5-3771">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="15ad5-3772">ACS</span><span class="sxs-lookup"><span data-stu-id="15ad5-3772">ACS</span></span>

* <span data-ttu-id="15ad5-3773">Korrigieren der Master- und Agentanzahl als ganze Zahl statt Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="15ad5-3773">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="15ad5-3774">Verfügbarmachen von „az acs create --no-wait“ und „az acs wait“ für die asynchrone Erstellung</span><span class="sxs-lookup"><span data-stu-id="15ad5-3774">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="15ad5-3775">Verfügbarmachen von „az acs create --validate“ für Probelaufüberprüfungen</span><span class="sxs-lookup"><span data-stu-id="15ad5-3775">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="15ad5-3776">Entfernen von Windows-Profil vor PUT-Aufruf für Skalierungsbefehl ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="15ad5-3776">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="15ad5-3777">AppService</span><span class="sxs-lookup"><span data-stu-id="15ad5-3777">AppService</span></span>

* <span data-ttu-id="15ad5-3778">functionapp: Hinzufügen der vollständigen functionapp-Unterstützung, einschließlich Erstellen, Anzeigen, Auflisten, Löschen, Hostname, SSL usw.</span><span class="sxs-lookup"><span data-stu-id="15ad5-3778">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="15ad5-3779">Hinzufügen von Team Services (vsts) als Continuous Delivery-Option zu „appservice web source-control config“</span><span class="sxs-lookup"><span data-stu-id="15ad5-3779">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="15ad5-3780">Erstellen von „az webapp“ als Ersatz für „az appservice web“ (für Abwärtskompatibilität bleibt „az appservice web“ für 2 weitere Releases erhalten)</span><span class="sxs-lookup"><span data-stu-id="15ad5-3780">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="15ad5-3781">Verfügbarmachen von Argumenten zum Konfigurieren von Bereitstellung und Laufzeitstapeln beim Erstellen von Web-Apps</span><span class="sxs-lookup"><span data-stu-id="15ad5-3781">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="15ad5-3782">Verfügbarmachen von „webapp list-runtimes“</span><span class="sxs-lookup"><span data-stu-id="15ad5-3782">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="15ad5-3783">Unterstützen der Konfiguration von Verbindungszeichenfolgen ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="15ad5-3783">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="15ad5-3784">Unterstützen des Slottauschs mit Vorschau</span><span class="sxs-lookup"><span data-stu-id="15ad5-3784">support slot swap with preview</span></span>
* <span data-ttu-id="15ad5-3785">Beheben von Fehlern in appservice-Befehlen ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="15ad5-3785">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="15ad5-3786">Verwenden der Ressourcengruppe des App Service-Plans für Zertifizierungsvorgänge ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="15ad5-3786">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="15ad5-3787">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="15ad5-3787">CosmosDB</span></span>

* <span data-ttu-id="15ad5-3788">Umbenennen des documentdb-Moduls in cosmosdb</span><span class="sxs-lookup"><span data-stu-id="15ad5-3788">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="15ad5-3789">Zusätzliche Unterstützung für documentdb-APIs auf Datenebene: Datenbank- und Sammlungsverwaltung</span><span class="sxs-lookup"><span data-stu-id="15ad5-3789">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="15ad5-3790">Zusätzliche Unterstützung für das Aktivieren des automatischen Failovers für Datenbankkonten</span><span class="sxs-lookup"><span data-stu-id="15ad5-3790">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="15ad5-3791">Zusätzliche Unterstützung für die neue ConsistentPrefix-Konsistenzrichtlinie</span><span class="sxs-lookup"><span data-stu-id="15ad5-3791">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="15ad5-3792">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="15ad5-3792">Data Lake Analytics</span></span>

* <span data-ttu-id="15ad5-3793">Beheben eines Fehlers, bei dem das Filtern von Auftragslisten nach Ergebnis und Status einen Fehler auslöst</span><span class="sxs-lookup"><span data-stu-id="15ad5-3793">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="15ad5-3794">Hinzufügen von Unterstützung für den neuen Katalogelementtyp „Paket“</span><span class="sxs-lookup"><span data-stu-id="15ad5-3794">Add support for new catalog item type: package.</span></span> <span data-ttu-id="15ad5-3795">Zugriff über: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="15ad5-3795">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="15ad5-3796">Ermöglichen der Auflistung folgender Katalogelemente innerhalb einer Datenbank (keine Schemaspezifikation erforderlich):</span><span class="sxs-lookup"><span data-stu-id="15ad5-3796">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="15ad5-3797">Tabelle</span><span class="sxs-lookup"><span data-stu-id="15ad5-3797">Table</span></span>
  * <span data-ttu-id="15ad5-3798">Tabellenwertfunktion</span><span class="sxs-lookup"><span data-stu-id="15ad5-3798">Table valued function</span></span>
  * <span data-ttu-id="15ad5-3799">Sicht</span><span class="sxs-lookup"><span data-stu-id="15ad5-3799">View</span></span>
  * <span data-ttu-id="15ad5-3800">Tabellenstatistiken.</span><span class="sxs-lookup"><span data-stu-id="15ad5-3800">Table Statistics.</span></span> <span data-ttu-id="15ad5-3801">Können auch mit einem Schema, jedoch ohne Angabe eines Tabellennamens aufgelistet werden.</span><span class="sxs-lookup"><span data-stu-id="15ad5-3801">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="15ad5-3802">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="15ad5-3802">Data Lake Store</span></span>

* <span data-ttu-id="15ad5-3803">Aktualisieren der Version des zugrunde liegenden Dateisystem-SDK, wodurch eine bessere Unterstützung für die Verarbeitung von Drosselungsszenarien auf Serverseite gewährt wird</span><span class="sxs-lookup"><span data-stu-id="15ad5-3803">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="15ad5-3804">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="15ad5-3804">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="15ad5-3805">Fehlende Hilfe für Zugriffsanzeige</span><span class="sxs-lookup"><span data-stu-id="15ad5-3805">missed help for access show.</span></span> <span data-ttu-id="15ad5-3806">hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="15ad5-3806">adding it.</span></span> <span data-ttu-id="15ad5-3807">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="15ad5-3807">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="15ad5-3808">Suchen</span><span class="sxs-lookup"><span data-stu-id="15ad5-3808">Find</span></span>

* <span data-ttu-id="15ad5-3809">Verbessern von Suchergebnissen und Ermöglichen der Versionsverwaltung des Suchindex</span><span class="sxs-lookup"><span data-stu-id="15ad5-3809">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="15ad5-3810">KeyVault</span><span class="sxs-lookup"><span data-stu-id="15ad5-3810">KeyVault</span></span>

* <span data-ttu-id="15ad5-3811">BC:`az keyvault certificate download` Ändern von „-e“ von Zeichenfolge oder Binärdatentyp in PEM oder DER zur besseren Darstellung der Optionen</span><span class="sxs-lookup"><span data-stu-id="15ad5-3811">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="15ad5-3812">BC: Entfernen von „--expires“ und „--not-before“ aus `keyvault certificate create`, da diese Parameter nicht vom Dienst unterstützt werden</span><span class="sxs-lookup"><span data-stu-id="15ad5-3812">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="15ad5-3813">Hinzufügen des Parameters „--validity“ zu `keyvault certificate create`, um gezielt den Wert in „--policy“ zu überschreiben</span><span class="sxs-lookup"><span data-stu-id="15ad5-3813">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="15ad5-3814">Beheben des Problems in `keyvault certificate get-default-policy`, bei dem „expires“ und „not_before“ verfügbar gemacht wurden, „validity_in_months“ hingegen nicht</span><span class="sxs-lookup"><span data-stu-id="15ad5-3814">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="15ad5-3815">Keyvault-Korrektur für den Import von PEM und PFX ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="15ad5-3815">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="15ad5-3816">Labor</span><span class="sxs-lookup"><span data-stu-id="15ad5-3816">Lab</span></span>

* <span data-ttu-id="15ad5-3817">Hinzufügen der Befehle „create“, „show“, „delete“ und „list“ für die Laborumgebung</span><span class="sxs-lookup"><span data-stu-id="15ad5-3817">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="15ad5-3818">Hinzufügen der Befehle „show“ und „list“ zur Anzeige von ARM-Vorlagen im Labor</span><span class="sxs-lookup"><span data-stu-id="15ad5-3818">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="15ad5-3819">Hinzufügen des Kennzeichens „--environment“ in `az lab vm list`, um virtuelle Computer nach Umgebung im Labor zu filtern</span><span class="sxs-lookup"><span data-stu-id="15ad5-3819">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="15ad5-3820">Hinzufügen des benutzerfreundlichen Befehls `az lab formula export-artifacts` zum Exportieren des Artefaktgerüsts innerhalb der Formel eines Labors</span><span class="sxs-lookup"><span data-stu-id="15ad5-3820">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="15ad5-3821">Hinzufügen von Befehlen zum Verwalten von Geheimnissen in einem Labor</span><span class="sxs-lookup"><span data-stu-id="15ad5-3821">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="15ad5-3822">Überwachen</span><span class="sxs-lookup"><span data-stu-id="15ad5-3822">Monitor</span></span>

* <span data-ttu-id="15ad5-3823">Fehlerbehebung: Modellieren von `--actions` von `az alert-rules create` zum Verarbeiten von JSON-Zeichenfolgen ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="15ad5-3823">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="15ad5-3824">Programmfehlerbehebung: Beim Erstellen von Diagnoseeinstellungen werden Protokolle/Metriken aus Anzeigebefehlen nicht akzeptiert ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="15ad5-3824">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="15ad5-3825">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="15ad5-3825">Network</span></span>

* <span data-ttu-id="15ad5-3826">Hinzufügen des `network watcher test-connectivity`-Befehls</span><span class="sxs-lookup"><span data-stu-id="15ad5-3826">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="15ad5-3827">Hinzufügen von Unterstützung für den `--filters`-Parameter für `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="15ad5-3827">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="15ad5-3828">Hinzufügen von Unterstützung für den Application Gateway-Verbindungsausgleich</span><span class="sxs-lookup"><span data-stu-id="15ad5-3828">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="15ad5-3829">Hinzufügen von Unterstützung für die Konfiguration von Application Gateway-WAF-Regelsätzen</span><span class="sxs-lookup"><span data-stu-id="15ad5-3829">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="15ad5-3830">Hinzufügen von Unterstützung für ExpressRoute-Routenfilter und -Regeln</span><span class="sxs-lookup"><span data-stu-id="15ad5-3830">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="15ad5-3831">Hinzufügen von Unterstützung für geografisches TrafficManager-Routing</span><span class="sxs-lookup"><span data-stu-id="15ad5-3831">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="15ad5-3832">Hinzufügen von Unterstützung für richtlinienbasierte Datenverkehrsselektoren für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="15ad5-3832">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="15ad5-3833">Hinzufügen von Unterstützung für IPSec-Richtlinien für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="15ad5-3833">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="15ad5-3834">Korrektur eines Fehlers bei `vpn-connection create` bei Verwendung der Parameter `--no-wait` oder `--validate`</span><span class="sxs-lookup"><span data-stu-id="15ad5-3834">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="15ad5-3835">Hinzufügen von Unterstützung für Aktiv/Aktiv-VNET-Gateways</span><span class="sxs-lookup"><span data-stu-id="15ad5-3835">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="15ad5-3836">Entfernen von NULL-Werten aus der Ausgabe von `network vpn-connection list/show`-Befehlen</span><span class="sxs-lookup"><span data-stu-id="15ad5-3836">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="15ad5-3837">BC: Korrektur eines Fehlers in der Ausgabe von `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="15ad5-3837">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="15ad5-3838">Korrektur eines Fehlers, bei dem das Argument „--key-length“ von „vpn-connection create“ nicht ordnungsgemäß analysiert wurde</span><span class="sxs-lookup"><span data-stu-id="15ad5-3838">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="15ad5-3839">Korrektur eines Fehlers in `dns zone import`, bei dem Datensätze nicht ordnungsgemäß importiert wurden</span><span class="sxs-lookup"><span data-stu-id="15ad5-3839">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="15ad5-3840">Korrektur eines Fehlers, bei dem `traffic-manager endpoint update` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="15ad5-3840">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="15ad5-3841">Hinzufügen von Network Watcher-Vorschaubefehlen</span><span class="sxs-lookup"><span data-stu-id="15ad5-3841">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="15ad5-3842">Profil</span><span class="sxs-lookup"><span data-stu-id="15ad5-3842">Profile</span></span>

* <span data-ttu-id="15ad5-3843">Unterstützung der Anmeldung, wenn keine Abonnements gefunden werden ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="15ad5-3843">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="15ad5-3844">Unterstützung für kurze Parameternamen in „az account set --subscription“ ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="15ad5-3844">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="15ad5-3845">Redis</span><span class="sxs-lookup"><span data-stu-id="15ad5-3845">Redis</span></span>

* <span data-ttu-id="15ad5-3846">Hinzufügen des Updatebefehls, durch den auch die Möglichkeit zum Skalieren für Redis Cache hinzugefügt wird</span><span class="sxs-lookup"><span data-stu-id="15ad5-3846">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="15ad5-3847">Verwerfen des Befehls „update-settings“</span><span class="sxs-lookup"><span data-stu-id="15ad5-3847">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="15ad5-3848">Resource</span><span class="sxs-lookup"><span data-stu-id="15ad5-3848">Resource</span></span>

* <span data-ttu-id="15ad5-3849">Hinzufügen der Befehle „managedapp“ und „managedapp definition“ ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="15ad5-3849">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="15ad5-3850">Unterstützung für die „provider operation“-Befehle ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="15ad5-3850">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="15ad5-3851">Unterstützung für die Erstellung generischer Ressourcen ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="15ad5-3851">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="15ad5-3852">Korrigieren der Ressourcenanalyse und der API-Versionssuche</span><span class="sxs-lookup"><span data-stu-id="15ad5-3852">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="15ad5-3853">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="15ad5-3853">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="15ad5-3854">Hinzufügen von Dokumenten für „az lock update“</span><span class="sxs-lookup"><span data-stu-id="15ad5-3854">Add docs for az lock update.</span></span> <span data-ttu-id="15ad5-3855">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="15ad5-3855">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="15ad5-3856">Beenden mit Fehler bei dem Versuch, Ressourcen für eine nicht vorhandene Gruppe aufzulisten</span><span class="sxs-lookup"><span data-stu-id="15ad5-3856">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="15ad5-3857">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="15ad5-3857">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="15ad5-3858">[Compute] Beheben von Problemen mit dem Update von VMSS- und VM-Verfügbarkeitsgruppen</span><span class="sxs-lookup"><span data-stu-id="15ad5-3858">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="15ad5-3859">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="15ad5-3859">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="15ad5-3860">Korrigieren des Erstellungs- und Löschvorgangs für Sperren, wenn „parent-resource-path“ auf „None“ festgelegt ist ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="15ad5-3860">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="15ad5-3861">Role</span><span class="sxs-lookup"><span data-stu-id="15ad5-3861">Role</span></span>

* <span data-ttu-id="15ad5-3862">create-for-rbac: Sicherstellen, dass das SP-Enddatum nicht das Ablaufdatum des Zertifikats überschreitet ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="15ad5-3862">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="15ad5-3863">RBAC: Hinzufügen vollständiger Unterstützung für „ad group“ ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="15ad5-3863">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="15ad5-3864">Rolle: Beheben von Probleme beim Rollendefinitionsupdate ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="15ad5-3864">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="15ad5-3865">create-for-rbac: Sicherstellen, dass das angegebene Benutzerkennwort übernommen wird</span><span class="sxs-lookup"><span data-stu-id="15ad5-3865">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="15ad5-3866">SQL</span><span class="sxs-lookup"><span data-stu-id="15ad5-3866">SQL</span></span>

* <span data-ttu-id="15ad5-3867">Hinzufügen der Befehle „az sql server list-usages“ und „az sql db list-usages“</span><span class="sxs-lookup"><span data-stu-id="15ad5-3867">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="15ad5-3868">SQL: Möglichkeit zur direkten Verbindung mit Ressourcenanbieter ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="15ad5-3868">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="15ad5-3869">Storage</span><span class="sxs-lookup"><span data-stu-id="15ad5-3869">Storage</span></span>

* <span data-ttu-id="15ad5-3870">Festlegen des Ressourcengruppenstandorts als Standardstandort für `storage account create`</span><span class="sxs-lookup"><span data-stu-id="15ad5-3870">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="15ad5-3871">Hinzufügen von Unterstützung für das inkrementelle Kopieren von Blobs</span><span class="sxs-lookup"><span data-stu-id="15ad5-3871">Add support for incremental blob copy</span></span>
* <span data-ttu-id="15ad5-3872">Hinzufügen von Unterstützung für den Upload umfangreicher Blockblobs</span><span class="sxs-lookup"><span data-stu-id="15ad5-3872">Add support for large block blob upload</span></span>
* <span data-ttu-id="15ad5-3873">Ändern der Blockgröße auf 100 MB, wenn die hochzuladende Datei größer als 200 GB ist</span><span class="sxs-lookup"><span data-stu-id="15ad5-3873">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="15ad5-3874">VM</span><span class="sxs-lookup"><span data-stu-id="15ad5-3874">VM</span></span>

* <span data-ttu-id="15ad5-3875">avail-set: Festlegen der UD- und FD-Domänenanzahl als optional</span><span class="sxs-lookup"><span data-stu-id="15ad5-3875">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="15ad5-3876">Hinweis: VM-Befehle in unabhängigen Clouds: Vermeiden Sie Features im Zusammenhang mit verwalteten Datenträgern, einschließlich der folgenden:</span><span class="sxs-lookup"><span data-stu-id="15ad5-3876">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="15ad5-3877">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="15ad5-3877">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="15ad5-3878">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="15ad5-3878">az vm/vmss disk</span></span>
  3. <span data-ttu-id="15ad5-3879">Verwenden Sie in „az vm/vmss create“ den Befehl „—use-unmanaged-disk“, um verwaltete Datenträger zu vermeiden. Andere Befehle sollten funktionieren.</span><span class="sxs-lookup"><span data-stu-id="15ad5-3879">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="15ad5-3880">vm/vmss: Verbessern des Warnungstexts beim Generieren von SSH-Schlüsselpaaren</span><span class="sxs-lookup"><span data-stu-id="15ad5-3880">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="15ad5-3881">vm/vmss: Unterstützen der Erstellung über ein Marketplace-Image, für das Planinformationen erforderlich sind ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="15ad5-3881">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="15ad5-3882">3\. April 2017</span><span class="sxs-lookup"><span data-stu-id="15ad5-3882">April 3, 2017</span></span>

<span data-ttu-id="15ad5-3883">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="15ad5-3883">Version 2.0.2</span></span>

<span data-ttu-id="15ad5-3884">In dieser Version wurden die Komponenten ACR, Batch, KeyVault und SQL eingeführt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-3884">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="15ad5-3885">Core</span><span class="sxs-lookup"><span data-stu-id="15ad5-3885">Core</span></span>

* <span data-ttu-id="15ad5-3886">Hinzufügen der Module „acr“, „lab“, „monitor“ und „find“ zur Standardliste</span><span class="sxs-lookup"><span data-stu-id="15ad5-3886">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="15ad5-3887">Anmeldung: Überspringen des fehlerhaften Mandanten ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="15ad5-3887">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="15ad5-3888">Anmeldung: Festlegen des Standardabonnements auf ein Abonnement mit dem Status „Enabled“ ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="15ad5-3888">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="15ad5-3889">Hinzufügen von wait-Befehlen und Unterstützung von „--no-wait“ für mehr Befehle ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="15ad5-3889">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="15ad5-3890">Core: Unterstützen der Anmeldung per Dienstprinzipal mit einem Zertifikat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="15ad5-3890">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="15ad5-3891">Hinzufügen der Meldung zu fehlenden Vorlagenparametern</span><span class="sxs-lookup"><span data-stu-id="15ad5-3891">Add prompting for missing template parameters.</span></span> <span data-ttu-id="15ad5-3892">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="15ad5-3892">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="15ad5-3893">Unterstützen des Festlegens von Standardwerten für häufig verwendete Argumente, z.B. Standardressourcengruppe, Standardweb und Standard-VM</span><span class="sxs-lookup"><span data-stu-id="15ad5-3893">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="15ad5-3894">Unterstützen der Anmeldung an einem bestimmten Mandanten</span><span class="sxs-lookup"><span data-stu-id="15ad5-3894">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="15ad5-3895">ACS</span><span class="sxs-lookup"><span data-stu-id="15ad5-3895">ACS</span></span>

* <span data-ttu-id="15ad5-3896">[ACS] Hinzufügen von Unterstützung für die Konfiguration eines ACS-Standardclusters ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="15ad5-3896">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="15ad5-3897">Hinzufügen von Unterstützung der Aufforderung zur Kennworteingabe für SSH-Schlüssel</span><span class="sxs-lookup"><span data-stu-id="15ad5-3897">Add support for ssh key password prompting.</span></span> <span data-ttu-id="15ad5-3898">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="15ad5-3898">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="15ad5-3899">Hinzufügen von Unterstützung für Windows-Cluster</span><span class="sxs-lookup"><span data-stu-id="15ad5-3899">Add support for windows clusters.</span></span> <span data-ttu-id="15ad5-3900">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="15ad5-3900">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="15ad5-3901">Wechseln von der Rolle „Besitzer“ zur Rolle „Mitwirkender“</span><span class="sxs-lookup"><span data-stu-id="15ad5-3901">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="15ad5-3902">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="15ad5-3902">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="15ad5-3903">AppService</span><span class="sxs-lookup"><span data-stu-id="15ad5-3903">AppService</span></span>

* <span data-ttu-id="15ad5-3904">appservice: Unterstützung für das Abrufen der externen IP-Adresse für DNS A-Einträge ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="15ad5-3904">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="15ad5-3905">appservice: Unterstützung der Bindung von Platzhalterzertifikaten ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="15ad5-3905">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="15ad5-3906">appservice: Unterstützung von Veröffentlichungsprofilen für Listen ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="15ad5-3906">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="15ad5-3907">AppService: Auslösen der Synchronisierung der Quellcodeverwaltung nach der Konfiguration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="15ad5-3907">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="15ad5-3908">DataLake</span><span class="sxs-lookup"><span data-stu-id="15ad5-3908">DataLake</span></span>

* <span data-ttu-id="15ad5-3909">Erste Version des Data Lake Analytics-Moduls</span><span class="sxs-lookup"><span data-stu-id="15ad5-3909">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="15ad5-3910">Erste Version des Data Lake Store-Moduls</span><span class="sxs-lookup"><span data-stu-id="15ad5-3910">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="15ad5-3911">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="15ad5-3911">DocuemntDB</span></span>

* <span data-ttu-id="15ad5-3912">DocumentDB: Hinzufügen von Unterstützung für das Auflisten von Verbindungszeichenfolgen ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="15ad5-3912">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="15ad5-3913">VM</span><span class="sxs-lookup"><span data-stu-id="15ad5-3913">VM</span></span>

* <span data-ttu-id="15ad5-3914">[Compute] Hinzufügen von AppGateway-Unterstützung für Erstellung von VM-Skalierungsgruppen ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="15ad5-3914">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="15ad5-3915">[VM/VMSS] Verbesserte Unterstützung für die Datenträgerzwischenspeicherung ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="15ad5-3915">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="15ad5-3916">VM/VMSS: Einbinden der vom Portal verwendeten Logik zur Überprüfung von Anmeldeinformationen ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="15ad5-3916">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="15ad5-3917">Hinzufügen von wait-Befehlen und Unterstützung für „--no-wait“ ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="15ad5-3917">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="15ad5-3918">VM-Skalierungsgruppe: Unterstützung von „\*“ zum Auflisten der übergreifenden Instanzansicht für VMs ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="15ad5-3918">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="15ad5-3919">Hinzufügen – Geheimnisse für virtuellen Computer und VM-Skalierungsgruppe ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="15ad5-3919">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="15ad5-3920">Zulassen der VM-Erstellung mit spezialisierter VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="15ad5-3920">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="15ad5-3921">27. Februar 2017</span><span class="sxs-lookup"><span data-stu-id="15ad5-3921">February 27, 2017</span></span>

<span data-ttu-id="15ad5-3922">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="15ad5-3922">Version 2.0.0</span></span>

<span data-ttu-id="15ad5-3923">Diese Version der Azure CLI 2.0 ist die erste „allgemein verfügbare“ Version. Die allgemeine Verfügbarkeit gilt für die folgenden Befehlsmodule:</span><span class="sxs-lookup"><span data-stu-id="15ad5-3923">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="15ad5-3924">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="15ad5-3924">Container Service (acs)</span></span>
- <span data-ttu-id="15ad5-3925">Compute (einschließlich Resource Manager, VM, VM-Skalierungsgruppen, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="15ad5-3925">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="15ad5-3926">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="15ad5-3926">Networking</span></span>
- <span data-ttu-id="15ad5-3927">Storage</span><span class="sxs-lookup"><span data-stu-id="15ad5-3927">Storage</span></span>

<span data-ttu-id="15ad5-3928">Diese Befehlsmodule können in der Produktion verwendet werden und verfügen über Unterstützung durch eine Standard-SLA von Microsoft. Sie können Anfragen zu Problemen direkt beim Microsoft-Support oder in der [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/) öffnen. Sie haben die Möglichkeit, Fragen in [StackOverflow mit dem Tag „azure-cli“](http://stackoverflow.com/questions/tagged/azure-cli) zu stellen oder sich unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) an das Produktteam zu wenden. Außerdem können Sie über die Befehlszeile mit dem Befehl `az feedback` Feedback senden.</span><span class="sxs-lookup"><span data-stu-id="15ad5-3928">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="15ad5-3929">Die Befehle in diesen Modulen sind stabil, und es ist nicht zu erwarten, dass sich die Syntax in den anstehenden Veröffentlichungen dieser Version der Azure CLI ändern.</span><span class="sxs-lookup"><span data-stu-id="15ad5-3929">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="15ad5-3930">Verwenden Sie zum Überprüfen der Version der CLI den Befehl `az --version`. In der Ausgabe werden die Version der CLI selbst (für diese Veröffentlichung 2.0.0), die einzelnen Befehlsmodule und die von Ihnen genutzten Versionen von Python und GCC aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-3930">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="15ad5-3931">Einige Befehlsmodule verfügen über das Postfix „b*n*“ oder „rc*n*“. Diese Befehlsmodule befinden sich noch in der Vorschauphase und werden später die allgemeine Verfügbarkeit erlangen.</span><span class="sxs-lookup"><span data-stu-id="15ad5-3931">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="15ad5-3932">Außerdem werden jeden Abend Vorschaubuilds der CLI bereitgestellt. Informationen hierzu finden Sie in der [Anleitung zum Abrufen der abendlichen Builds](https://github.com/Azure/azure-cli#nightly-builds) und im Abschnitt zum [Setup für Entwickler und Beitragen von Code](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="15ad5-3932">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="15ad5-3933">Sie können für die abendlichen Vorschaubuilds wie folgt Probleme melden:</span><span class="sxs-lookup"><span data-stu-id="15ad5-3933">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="15ad5-3934">Über die [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="15ad5-3934">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="15ad5-3935">Per Kontaktaufnahme mit dem Produktteam unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="15ad5-3935">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="15ad5-3936">Senden von Feedback über die Befehlszeile mit dem Befehl `az feedback`</span><span class="sxs-lookup"><span data-stu-id="15ad5-3936">Provide feedback from the command line with the `az feedback` command</span></span>

# <a name="beta-release-notes"></a>[<span data-ttu-id="15ad5-3937">Versionshinweise zur Betaversion</span><span class="sxs-lookup"><span data-stu-id="15ad5-3937">Beta release notes</span></span>](#tab/azure-cli-beta)

<span data-ttu-id="15ad5-3938">Die Azure CLI-Betaversion ist eine Migration der Authentifizierungsmethode der AAD-Plattform (v1.0) zu [Microsoft Identity Platform (v2.0)](/azure/active-directory/develop/v2-overview).</span><span class="sxs-lookup"><span data-stu-id="15ad5-3938">The Azure CLI beta release is a migration from the authentican method of AAD platform (v1.0) to [Microsoft Identity platform (v2.0)](/azure/active-directory/develop/v2-overview).</span></span>

## <a name="june-23-2020"></a><span data-ttu-id="15ad5-3939">23. Juni 2020</span><span class="sxs-lookup"><span data-stu-id="15ad5-3939">June 23, 2020</span></span>

### <a name="things-to-know-about-the-new-azure-cli-beta-release"></a><span data-ttu-id="15ad5-3940">Wissenswertes über die neue Azure CLI-Betaversion</span><span class="sxs-lookup"><span data-stu-id="15ad5-3940">Things to know about the new Azure CLI beta release</span></span>

-   <span data-ttu-id="15ad5-3941">Die Betaversion der Azure CLI unterstützt alle CLI-Befehle, die in der aktuellen veröffentlichten Version verfügbar sind.</span><span class="sxs-lookup"><span data-stu-id="15ad5-3941">The beta version of the Azure CLI supports all CLI commands that you will find in the current released version.</span></span>
-   <span data-ttu-id="15ad5-3942">Nach der Installation der Betaversion ist eine erneute Anmeldung erforderlich.</span><span class="sxs-lookup"><span data-stu-id="15ad5-3942">Relogin is required after install the beta version.</span></span>
-   <span data-ttu-id="15ad5-3943">Die Betaversion unterstützt nur die Windows-Plattform.</span><span class="sxs-lookup"><span data-stu-id="15ad5-3943">The beta release only supports the Windows platform.</span></span>
-   <span data-ttu-id="15ad5-3944">Azure Stack wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-3944">The Azure Stack is not supported.</span></span>
-   <span data-ttu-id="15ad5-3945">Parameter `--use-cert-sn-issuer` wird nicht unterstützt, wenn für die Authentifizierung ein Dienstprinzipalschlüssel verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="15ad5-3945">`--use-cert-sn-issuer` parameter is not supported when using service principal key to authenticate.</span></span>
-   <span data-ttu-id="15ad5-3946">Das Überspringen der SSL-Überprüfung über die Umgebung `ADAL_PYTHON_SSL_NO_VERIFY` wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="15ad5-3946">Skip SSL verification via environment `ADAL_PYTHON_SSL_NO_VERIFY` is not supported.</span></span>

<span data-ttu-id="15ad5-3947">Sollten Probleme in der Betaversion auftreten, können Sie auf [GitHub](https://github.com/Azure/azure-cli/issues/new/choose) gerne Kommentare für das Azure CLI-Entwicklungsteam hinterlassen.</span><span class="sxs-lookup"><span data-stu-id="15ad5-3947">If you find any issues in the beta release, the Azure CLI engineering team welcomes your comments on [GitHub](https://github.com/Azure/azure-cli/issues/new/choose).</span></span>

---

---
title: Versionshinweise für die Azure CLI
description: Enthält Informationen zu den aktuellen Updates der Azure CLI.
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 08/06/2020
ms.topic: article
ms.service: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: f81f5a69bd5806d2081a8eaa9b62a5b00b56edf9
ms.sourcegitcommit: 04d3b43d7c960ff0e6188c9672d27046b45da6ed
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/06/2020
ms.locfileid: "87855932"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="0bba9-103">Versionshinweise für die Azure CLI</span><span class="sxs-lookup"><span data-stu-id="0bba9-103">Azure CLI release notes</span></span>

# <a name="current-release-notes"></a>[<span data-ttu-id="0bba9-104">Aktuelle Versionshinweise</span><span class="sxs-lookup"><span data-stu-id="0bba9-104">Current release notes</span></span>](#tab/azure-cli)

## <a name="august-11-2020"></a><span data-ttu-id="0bba9-105">11. August 2020</span><span class="sxs-lookup"><span data-stu-id="0bba9-105">August 11, 2020</span></span>

<span data-ttu-id="0bba9-106">Version 2.10.1</span><span class="sxs-lookup"><span data-stu-id="0bba9-106">Version 2.10.1</span></span>

### <a name="app-service"></a><span data-ttu-id="0bba9-107">App Service</span><span class="sxs-lookup"><span data-stu-id="0bba9-107">App Service</span></span>

* <span data-ttu-id="0bba9-108">Behebung Nr. 9887: webapp und functionapp, Unterstützung für das Zuweisen/Entfernen einer benutzerseitig verwalteten Identität</span><span class="sxs-lookup"><span data-stu-id="0bba9-108">Fix #9887 webapp and functionapp, support assigning/removing user managed identity</span></span>
* <span data-ttu-id="0bba9-109">Behebung Nr. 1382, Nr. 14055: Fehlermeldungen für „az webapp create“ und „az webapp config container set“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-109">Fix #1382, #14055: Update error messages for az webapp create and az webapp config container set</span></span>
* <span data-ttu-id="0bba9-110">`az webapp up`: Standardmäßige ASP-Auswahllogik korrigiert, wenn der Parameter „--plan“ nicht angegeben wird</span><span class="sxs-lookup"><span data-stu-id="0bba9-110">`az webapp up`: Fix default ASP selection logic when --plan parameter is not provided</span></span>

### <a name="appconfig"></a><span data-ttu-id="0bba9-111">AppConfig</span><span class="sxs-lookup"><span data-stu-id="0bba9-111">AppConfig</span></span>

* <span data-ttu-id="0bba9-112">Unterstützung für die Aktivierung/Deaktivierung von PublicNetworkAccess während der Speichererstellung</span><span class="sxs-lookup"><span data-stu-id="0bba9-112">Support enabling/disabling PublicNetworkAccess during store creation</span></span>

### <a name="compute"></a><span data-ttu-id="0bba9-113">Compute</span><span class="sxs-lookup"><span data-stu-id="0bba9-113">Compute</span></span>

* <span data-ttu-id="0bba9-114">Unterstützung für das Zuordnen einer Datenträgerzugriffsressource für Datenträger und Momentaufnahmen</span><span class="sxs-lookup"><span data-stu-id="0bba9-114">Support associating disk and snapshot with a disk-access resource</span></span>

### <a name="lab"></a><span data-ttu-id="0bba9-115">Labor</span><span class="sxs-lookup"><span data-stu-id="0bba9-115">Lab</span></span>

* <span data-ttu-id="0bba9-116">Fehlerbehebung Nr. 7904: Fehler bei der Datumsüberprüfung bei der Lab-VM-Erstellung</span><span class="sxs-lookup"><span data-stu-id="0bba9-116">Fix for issue #7904 date validation bug in lab vm creation</span></span>

### <a name="storage"></a><span data-ttu-id="0bba9-117">Storage</span><span class="sxs-lookup"><span data-stu-id="0bba9-117">Storage</span></span>

* <span data-ttu-id="0bba9-118">`az storage blob upload-batch`: Problembehebung Nr. 14660 mit nicht positionellen Argumenten</span><span class="sxs-lookup"><span data-stu-id="0bba9-118">`az storage blob upload-batch`: Fix issue #14660 with unpositional arguments</span></span>

## <a name="august-04-2020"></a><span data-ttu-id="0bba9-119">04. August 2020</span><span class="sxs-lookup"><span data-stu-id="0bba9-119">August 04, 2020</span></span>

<span data-ttu-id="0bba9-120">Version 2.10.0</span><span class="sxs-lookup"><span data-stu-id="0bba9-120">Version 2.10.0</span></span>

### <a name="aks"></a><span data-ttu-id="0bba9-121">AKS</span><span class="sxs-lookup"><span data-stu-id="0bba9-121">AKS</span></span>

* <span data-ttu-id="0bba9-122">`az aks update`: Argument „--enable-aad“ geändert, um einen RBAC-fähigen AAD-fremden Cluster zu einem von AKS-verwalteten AAD-Cluster zu migrieren</span><span class="sxs-lookup"><span data-stu-id="0bba9-122">`az aks update`: Change --enable-aad argument to migrate a RBAC-enabled non-AAD cluster to a AKS-managed AAD cluster</span></span>
* <span data-ttu-id="0bba9-123">`az aks install-cli`: Argumente „--kubelogin-version“ und „--kubelogin-install-location“ zum Installieren von kubelogin hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-123">`az aks install-cli`: Add --kubelogin-version and --kubelogin-install-location arguments to install kubelogin</span></span>
* <span data-ttu-id="0bba9-124">Befehl „az aks nodepool get-upgrades“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-124">Add az aks nodepool get-upgrades command</span></span>

### <a name="ams"></a><span data-ttu-id="0bba9-125">AMS</span><span class="sxs-lookup"><span data-stu-id="0bba9-125">AMS</span></span>

* <span data-ttu-id="0bba9-126">Korrektur 14021: „az ams account sp“ ist nicht idempotent.</span><span class="sxs-lookup"><span data-stu-id="0bba9-126">Fix #14021: az ams account sp is not idempotent</span></span>

### <a name="apim"></a><span data-ttu-id="0bba9-127">APIM</span><span class="sxs-lookup"><span data-stu-id="0bba9-127">APIM</span></span>

* <span data-ttu-id="0bba9-128">APIM-API-Import: API-Importunterstützung und Erweiterung anderer CLI-Befehle auf der API-Ebene</span><span class="sxs-lookup"><span data-stu-id="0bba9-128">apim api import: support API import and enchance other api level cli commands</span></span>

### <a name="app-service"></a><span data-ttu-id="0bba9-129">App Service</span><span class="sxs-lookup"><span data-stu-id="0bba9-129">App Service</span></span>

* <span data-ttu-id="0bba9-130">Korrektur 13035: Zugriffsbeschränkungsüberprüfung für „az webapp config“ hinzugefügt, um Duplikate zu vermeiden</span><span class="sxs-lookup"><span data-stu-id="0bba9-130">Fix #13035: Add validation for az webapp config access-restriction to avoid adding duplicates</span></span>

### <a name="appconfig"></a><span data-ttu-id="0bba9-131">AppConfig</span><span class="sxs-lookup"><span data-stu-id="0bba9-131">AppConfig</span></span>

* <span data-ttu-id="0bba9-132">Bei fehlender Angabe wird die Standard-SKU verwendet.</span><span class="sxs-lookup"><span data-stu-id="0bba9-132">Default to standard sku if not specified</span></span>
* <span data-ttu-id="0bba9-133">[BREAKING CHANGE] Einstellungen mit JSON-Inhaltstyp werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-133">[BREAKING CHANGE] Support settings with JSON content type</span></span>

### <a name="arm"></a><span data-ttu-id="0bba9-134">ARM</span><span class="sxs-lookup"><span data-stu-id="0bba9-134">ARM</span></span>

* <span data-ttu-id="0bba9-135">`az resource tag`: Fehler im Zusammenhang mit managedApp-Kennzeichnung sowie einige damit zusammenhängende Testprobleme behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-135">`az resource tag`: Fix the bug of managedApp tagging and some related test issues</span></span>
* <span data-ttu-id="0bba9-136">`az deployment mg/tenant what-if`: Unterstützung für die Bereitstellung auf Verwaltungsgruppen- und Mandantenebene hinzugefügt (Was-wäre-wenn)</span><span class="sxs-lookup"><span data-stu-id="0bba9-136">`az deployment mg/tenant what-if`: Add support to management group and tenant level deployment What-If</span></span>
* <span data-ttu-id="0bba9-137">`az deployment mg/tenant create`: Parameter „--confirm-with-what-if/-c“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-137">`az deployment mg/tenant create`: Add --confirm-with-what-if/-c parameter.</span></span>
* <span data-ttu-id="0bba9-138">`az deployment mg/tenant create`: Parameter „--what-if-result-format/-r“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-138">`az deployment mg/tenant create`: Add --what-if-result-format/-r parameter.</span></span>
* <span data-ttu-id="0bba9-139">`az deployment mg/tenant create`: Parameter „--what-if-exclude-change-types/-x“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-139">`az deployment mg/tenant create`: Add --what-if-exclude-change-types/-x parameter.</span></span>
* <span data-ttu-id="0bba9-140">`az tag`: Unterstützung von „az tag“ für Ressourcen-ID-Parameter</span><span class="sxs-lookup"><span data-stu-id="0bba9-140">`az tag`: az tag support for resource id parameter</span></span>

### <a name="backup"></a><span data-ttu-id="0bba9-141">Backup</span><span class="sxs-lookup"><span data-stu-id="0bba9-141">Backup</span></span>

* <span data-ttu-id="0bba9-142">Auslösung von AFS-Container-/Elementerkennung nur bei Bedarf</span><span class="sxs-lookup"><span data-stu-id="0bba9-142">Trigger AFS container/item discovery only when needed</span></span>

### <a name="cdn"></a><span data-ttu-id="0bba9-143">CDN</span><span class="sxs-lookup"><span data-stu-id="0bba9-143">CDN</span></span>

* <span data-ttu-id="0bba9-144">Private Link-Felder zu Ursprung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-144">Add private link fields to origin</span></span>

### <a name="compute"></a><span data-ttu-id="0bba9-145">Compute</span><span class="sxs-lookup"><span data-stu-id="0bba9-145">Compute</span></span>

* <span data-ttu-id="0bba9-146">`az vm/vmss create`: Wahl eines gültigen Benutzernamens für den Benutzer bei ungültigem Standardbenutzernamen</span><span class="sxs-lookup"><span data-stu-id="0bba9-146">`az vm/vmss create`: Select a valid username for user if the default username is invalid</span></span>
* <span data-ttu-id="0bba9-147">`az vm update`: Unterstützung mandantenübergreifender Images</span><span class="sxs-lookup"><span data-stu-id="0bba9-147">`az vm update`: support cross tenant image</span></span>
* <span data-ttu-id="0bba9-148">`az disk-access`: Neue Befehlsgruppe für die Verwendung der Datenträgerzugriffsressource hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-148">`az disk-access`: Add new command group to operate disk access resource</span></span>
* <span data-ttu-id="0bba9-149">Unterstützung der automatischen Platzierung dedizierter Hostgruppen</span><span class="sxs-lookup"><span data-stu-id="0bba9-149">Support dedicated host group automatic placement</span></span>
* <span data-ttu-id="0bba9-150">Unterstützung von PPG und SPG im VMSS-Orchestrierungsmodus</span><span class="sxs-lookup"><span data-stu-id="0bba9-150">Support ppg and spg in VMSS orchestration mode</span></span>

### <a name="config"></a><span data-ttu-id="0bba9-151">Config</span><span class="sxs-lookup"><span data-stu-id="0bba9-151">Config</span></span>

* <span data-ttu-id="0bba9-152">`az config`: Neuer Befehl (`config`) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-152">`az config`: Add new `config` command module</span></span>

### <a name="extension"></a><span data-ttu-id="0bba9-153">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="0bba9-153">Extension</span></span>

* <span data-ttu-id="0bba9-154">Unterstützung der automatischen Installation einer Erweiterung, wenn die Erweiterung eines Befehls nicht installiert ist</span><span class="sxs-lookup"><span data-stu-id="0bba9-154">Support automatically installing an extension if the extension of a command is not installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="0bba9-155">HDInsight</span><span class="sxs-lookup"><span data-stu-id="0bba9-155">HDInsight</span></span>

* <span data-ttu-id="0bba9-156">Drei Parameter zum Befehl `az hdinsight create` hinzugefügt, um Private Link und Verschlüsselung während der Übertragung zu unterstützen:</span><span class="sxs-lookup"><span data-stu-id="0bba9-156">Add 3 parameters to the command `az hdinsight create` to support private link and encryption in transit feature:</span></span>

### <a name="iot-hub"></a><span data-ttu-id="0bba9-157">IoT Hub</span><span class="sxs-lookup"><span data-stu-id="0bba9-157">Iot Hub</span></span>

* <span data-ttu-id="0bba9-158">Korrektur 7792: „iot hub create“ ist nicht idempotent.</span><span class="sxs-lookup"><span data-stu-id="0bba9-158">Fix #7792: IoT Hub Create is not idempotent</span></span>

### <a name="iot-central"></a><span data-ttu-id="0bba9-159">IoT Central</span><span class="sxs-lookup"><span data-stu-id="0bba9-159">IoT Central</span></span>

* <span data-ttu-id="0bba9-160">Parameteroptionenliste für IoT Central hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-160">Add paramater option list for iot central</span></span>

### <a name="keyvault"></a><span data-ttu-id="0bba9-161">KeyVault</span><span class="sxs-lookup"><span data-stu-id="0bba9-161">KeyVault</span></span>

* <span data-ttu-id="0bba9-162">`az keyvault key encrypt/decrypt`: Parameter `--data-type` zum expliziten Angeben der Art von Originaldaten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-162">`az keyvault key encrypt/decrypt`: add parameter `--data-type` for explicitly specifing the type of original data</span></span>

### <a name="monitor"></a><span data-ttu-id="0bba9-163">Überwachen</span><span class="sxs-lookup"><span data-stu-id="0bba9-163">Monitor</span></span>

* <span data-ttu-id="0bba9-164">`az monitor log-analytics workspace data-export`: Unterstützung des Event Hub-Namespace als Ziel</span><span class="sxs-lookup"><span data-stu-id="0bba9-164">`az monitor log-analytics workspace data-export`: support event hub namespace as the destination.</span></span>
* <span data-ttu-id="0bba9-165">`az monitor autoscale`: Unterstützung von Namespace und Dimensionen für „--condition“</span><span class="sxs-lookup"><span data-stu-id="0bba9-165">`az monitor autoscale`: support namespace and dimensions for --condition</span></span>

### <a name="netappfiles"></a><span data-ttu-id="0bba9-166">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="0bba9-166">NetAppFiles</span></span>

* <span data-ttu-id="0bba9-167">`az volume revert`:  Volumewiederherstellung hinzugefügt, um ein Volume auf eine der zugehörigen Momentaufnahmen zurückzusetzen</span><span class="sxs-lookup"><span data-stu-id="0bba9-167">`az volume revert`:  Add Volume Revert to revert a volume to one of its snapshots.</span></span>
* <span data-ttu-id="0bba9-168">[BREAKING CHANGE] `az netappfiles mount-target` entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-168">[BREAKING CHANGE] Remove `az netappfiles mount-target`.</span></span>
* <span data-ttu-id="0bba9-169">`az volume show`: Standort zu Active Directory-Eigenschaften hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-169">`az volume show`: Add site to Active Directory Properties</span></span>

### <a name="network"></a><span data-ttu-id="0bba9-170">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0bba9-170">Network</span></span>

* <span data-ttu-id="0bba9-171">`az application-gateway private-link add`: Unterstützung der Angabe eines vorhandenen Subnetzes nach ID</span><span class="sxs-lookup"><span data-stu-id="0bba9-171">`az application-gateway private-link add`: support to specify an existing subnet by ID</span></span>
* <span data-ttu-id="0bba9-172">`az network application-gateway waf-policy create`: Unterstützung von Version und Typ</span><span class="sxs-lookup"><span data-stu-id="0bba9-172">`az network application-gateway waf-policy create`: support version and type</span></span>

### <a name="storage"></a><span data-ttu-id="0bba9-173">Storage</span><span class="sxs-lookup"><span data-stu-id="0bba9-173">Storage</span></span>

* <span data-ttu-id="0bba9-174">Korrektur 10302: Unterstützung der Ermittlung des wahrscheinlichen Inhaltstyps beim Synchronisieren von Dateien</span><span class="sxs-lookup"><span data-stu-id="0bba9-174">Fix #10302: Support guess content-type when synchronizing files</span></span>
* <span data-ttu-id="0bba9-175">`az storage blob lease`: Neue API-Version für Blobleasevorgänge angewendet</span><span class="sxs-lookup"><span data-stu-id="0bba9-175">`az storage blob lease`: Apply new api version for blob lease operations</span></span>
* <span data-ttu-id="0bba9-176">`az storage fs access`: Unterstützung von AAD-Anmeldeinformationen bei der Verwaltung der Zugriffssteuerung für das ADLS Gen2-Konto</span><span class="sxs-lookup"><span data-stu-id="0bba9-176">`az storage fs access`: Support AAD credential in managing access control for ADLS Gen2 account</span></span>
* <span data-ttu-id="0bba9-177">`az storage share-rm create/update`: „--access-tier“ hinzugefügt, um die Zugriffsebene zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="0bba9-177">`az storage share-rm create/update`: add --access-tier to support access tier</span></span>

## <a name="july-16-2020"></a><span data-ttu-id="0bba9-178">16. Juli 2020</span><span class="sxs-lookup"><span data-stu-id="0bba9-178">July 16, 2020</span></span>

<span data-ttu-id="0bba9-179">Version 2.9.1</span><span class="sxs-lookup"><span data-stu-id="0bba9-179">Version 2.9.1</span></span>

### <a name="aks"></a><span data-ttu-id="0bba9-180">AKS</span><span class="sxs-lookup"><span data-stu-id="0bba9-180">AKS</span></span>

* <span data-ttu-id="0bba9-181">Explizite Einstellung von VMSS im Windows-Beispielbefehl entfernt, da dies jetzt die Standardeinstellung ist</span><span class="sxs-lookup"><span data-stu-id="0bba9-181">Remove explicit setting of VMSS in Windows example command since it is now default</span></span>

### <a name="iot"></a><span data-ttu-id="0bba9-182">IoT</span><span class="sxs-lookup"><span data-stu-id="0bba9-182">IoT</span></span>

* <span data-ttu-id="0bba9-183">[BREAKING CHANGE] `az iot pnp`: IoT-PNP-Vorschaubefehle aus Core-CLI entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-183">[BREAKING CHANGE] `az iot pnp`: Remove IoT PNP preview commands from core CLI</span></span>

### <a name="rest"></a><span data-ttu-id="0bba9-184">REST</span><span class="sxs-lookup"><span data-stu-id="0bba9-184">REST</span></span>

* <span data-ttu-id="0bba9-185">Behebung Nr. 14152: `az rest`: ARM-URLs ohne Abonnement-ID werden nun akzeptiert.</span><span class="sxs-lookup"><span data-stu-id="0bba9-185">Fix #14152: `az rest`: Accept ARM URLs without subscription ID</span></span>

### <a name="storage"></a><span data-ttu-id="0bba9-186">Storage</span><span class="sxs-lookup"><span data-stu-id="0bba9-186">Storage</span></span>

* <span data-ttu-id="0bba9-187">Behebung Nr. 14138: Einige Berechtigungen sind nun optional.</span><span class="sxs-lookup"><span data-stu-id="0bba9-187">Fix #14138: Make some permissions optional</span></span>

## <a name="july-14-2020"></a><span data-ttu-id="0bba9-188">14. Juli 2020</span><span class="sxs-lookup"><span data-stu-id="0bba9-188">July 14, 2020</span></span>

<span data-ttu-id="0bba9-189">Version 2.9.0</span><span class="sxs-lookup"><span data-stu-id="0bba9-189">Version 2.9.0</span></span>

### <a name="acr"></a><span data-ttu-id="0bba9-190">ACR</span><span class="sxs-lookup"><span data-stu-id="0bba9-190">ACR</span></span>

* <span data-ttu-id="0bba9-191">Verarbeiten des Protokollartefaktlinks aus der Registrierung zum Streamen von Protokollen</span><span class="sxs-lookup"><span data-stu-id="0bba9-191">Handle log artifact link from Registry to stream logs</span></span>
* <span data-ttu-id="0bba9-192">Helm2-Befehle als veraltet kennzeichnen</span><span class="sxs-lookup"><span data-stu-id="0bba9-192">Deprecate helm2 commands</span></span>

### <a name="aks"></a><span data-ttu-id="0bba9-193">AKS</span><span class="sxs-lookup"><span data-stu-id="0bba9-193">AKS</span></span>

* <span data-ttu-id="0bba9-194">`az aks create`: Argument „--enable-aad“ hinzufügen</span><span class="sxs-lookup"><span data-stu-id="0bba9-194">`az aks create`: add --enable-aad argument</span></span>
* <span data-ttu-id="0bba9-195">`az aks update`: Argument „--enable-aad“ hinzufügen</span><span class="sxs-lookup"><span data-stu-id="0bba9-195">`az aks update`: add --enable-aad argument</span></span>

### <a name="apim"></a><span data-ttu-id="0bba9-196">APIM</span><span class="sxs-lookup"><span data-stu-id="0bba9-196">APIM</span></span>

* <span data-ttu-id="0bba9-197">Allgemeine Befehle vom Typ „az apim api“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-197">Added general az apim api commands</span></span>

### <a name="appconfig"></a><span data-ttu-id="0bba9-198">AppConfig</span><span class="sxs-lookup"><span data-stu-id="0bba9-198">AppConfig</span></span>

* <span data-ttu-id="0bba9-199">Beispiel für die Verwendung von „--fields“ in AppConfig-Revision hinzufügen</span><span class="sxs-lookup"><span data-stu-id="0bba9-199">Add example for using --fields in appconfig revision</span></span>

### <a name="appservice"></a><span data-ttu-id="0bba9-200">AppService</span><span class="sxs-lookup"><span data-stu-id="0bba9-200">AppService</span></span>

* <span data-ttu-id="0bba9-201">`az functionapp create`: Unterstützung für Java 11 und PowerShell 7 hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-201">`az functionapp create`: Added support for Java 11 and Powershell 7.</span></span> <span data-ttu-id="0bba9-202">Unterstützung für Stapel-API hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-202">Added Stacks API Support.</span></span>
* <span data-ttu-id="0bba9-203">Behebung von Nr. 14208: Erstellen einer App mit mehreren Containern erzeugt einen Fehler</span><span class="sxs-lookup"><span data-stu-id="0bba9-203">Fix #14208 multi-container app creation fails</span></span>
* <span data-ttu-id="0bba9-204">Korrektur von „az webapp create“ – hartcodierte Laufzeitstapel verwenden</span><span class="sxs-lookup"><span data-stu-id="0bba9-204">Fix az webapp create - use hardcoded runtime stacks</span></span>

### <a name="arm"></a><span data-ttu-id="0bba9-205">ARM</span><span class="sxs-lookup"><span data-stu-id="0bba9-205">ARM</span></span>

* <span data-ttu-id="0bba9-206">`az resource tag`: Behebung des Problems beim Taggen von Ressourcen mit dem Ressourcentyp `Microsoft.ContainerInstance/containerGroups`</span><span class="sxs-lookup"><span data-stu-id="0bba9-206">`az resource tag`: Fix the problem of tagging resources with resource type `Microsoft.ContainerInstance/containerGroups`</span></span>

### <a name="compute"></a><span data-ttu-id="0bba9-207">Compute</span><span class="sxs-lookup"><span data-stu-id="0bba9-207">Compute</span></span>

* <span data-ttu-id="0bba9-208">Datenträgerversion aktualisieren 2020-05-01, Compute 2020-06-01</span><span class="sxs-lookup"><span data-stu-id="0bba9-208">Bump version disks 2020-05-01, compute 2020-06-01</span></span>
* <span data-ttu-id="0bba9-209">Doppelte Verschlüsselung des Datenträgerverschlüsselungssatzes</span><span class="sxs-lookup"><span data-stu-id="0bba9-209">Double encryption of disk encryption set</span></span>
* <span data-ttu-id="0bba9-210">`az vmss update`: Unterstützung für das Angeben eines mandantenübergreifendes Image.</span><span class="sxs-lookup"><span data-stu-id="0bba9-210">`az vmss update`: support specify cross tenant image.</span></span>
* <span data-ttu-id="0bba9-211">`az sig image-version create`: Unterstützung für das Angeben eines mandantenübergreifendes Image.</span><span class="sxs-lookup"><span data-stu-id="0bba9-211">`az sig image-version create`: support specify cross tenant image.</span></span>
* <span data-ttu-id="0bba9-212">vm/vmss create: Verschlüsselung von Cache und Daten während der Übertragung für (Betriebssystem-)Datenträger und temporäre Datenträger für VM und VMSS</span><span class="sxs-lookup"><span data-stu-id="0bba9-212">vm/vmss create: Encryption of cache & data-in-transit for OS/Data disks and temp disks for VM & VMSS</span></span>
* <span data-ttu-id="0bba9-213">Vorgang „simulate-eviction“ für VM und VMSS hinzufügen</span><span class="sxs-lookup"><span data-stu-id="0bba9-213">Add simulate-eviction operation for VM and VMSS</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="0bba9-214">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="0bba9-214">CosmosDB</span></span>

* <span data-ttu-id="0bba9-215">Aktuelle Features: Autoscale, IpRules, EnableFreeTier und EnableAnalyticalStorage</span><span class="sxs-lookup"><span data-stu-id="0bba9-215">Recent features: Autoscale, IpRules, EnableFreeTier and EnableAnalyticalStorage</span></span>

### <a name="eventgrid"></a><span data-ttu-id="0bba9-216">EventGrid</span><span class="sxs-lookup"><span data-stu-id="0bba9-216">EventGrid</span></span>

* <span data-ttu-id="0bba9-217">CLI-Unterstützung für 2020-04-01-preview hinzufügen und Previewfunktionen mit „is_Preview=True“ kennzeichnen</span><span class="sxs-lookup"><span data-stu-id="0bba9-217">Add CLI support for 2020-04-01-preview and mark preview features with is_Preview=True</span></span>

### <a name="find"></a><span data-ttu-id="0bba9-218">Suchen</span><span class="sxs-lookup"><span data-stu-id="0bba9-218">Find</span></span>

* <span data-ttu-id="0bba9-219">Behebung von Nr. 14094 „az find“: Abfragen schlagen fehl, wenn nicht angemeldet und Telemetrie deaktiviert</span><span class="sxs-lookup"><span data-stu-id="0bba9-219">Fix #14094 az find Fix Queries failing when not logged in and when telemetry is disabled</span></span>

### <a name="hdinsight"></a><span data-ttu-id="0bba9-220">HDInsight</span><span class="sxs-lookup"><span data-stu-id="0bba9-220">HDInsight</span></span>

* <span data-ttu-id="0bba9-221">Zwei Befehle zur Unterstützung der Neustartfunktion für HDInsight-Knoten hinzufügen</span><span class="sxs-lookup"><span data-stu-id="0bba9-221">Add two commands to support hdinsight node reboot feature</span></span>

### <a name="monitor"></a><span data-ttu-id="0bba9-222">Überwachen</span><span class="sxs-lookup"><span data-stu-id="0bba9-222">Monitor</span></span>

* <span data-ttu-id="0bba9-223">Vorschaukennzeichnung für Befehle unter Log Analytics-Arbeitsbereich entfernen</span><span class="sxs-lookup"><span data-stu-id="0bba9-223">Remove preview flag for commands under Log Analytics workspace</span></span>
* <span data-ttu-id="0bba9-224">`az monitor diagnostic-settings subscription`: Diagnoseeinstellungen für Abonnement unterstützen</span><span class="sxs-lookup"><span data-stu-id="0bba9-224">`az monitor diagnostic-settings subscription`: Support diagnositc settings for subscription</span></span>
* <span data-ttu-id="0bba9-225">`az monitor metrics`: „,“ und „|“ in Metrikname unterstützen</span><span class="sxs-lookup"><span data-stu-id="0bba9-225">`az monitor metrics`: support ',' and '|' in metric name</span></span>
* <span data-ttu-id="0bba9-226">`az monitor log-analytics workspace data-export`: Log Analytics-Datenexport unterstützen</span><span class="sxs-lookup"><span data-stu-id="0bba9-226">`az monitor log-analytics workspace data-export`: support log analytics data export</span></span>

### <a name="network"></a><span data-ttu-id="0bba9-227">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0bba9-227">Network</span></span>

* <span data-ttu-id="0bba9-228">`az network application-gateway frontend-ip update`: Parameter „--public-ip-address“ als veraltet markieren</span><span class="sxs-lookup"><span data-stu-id="0bba9-228">`az network application-gateway frontend-ip update`: Deprecating the --public-ip-address parameter</span></span>
* <span data-ttu-id="0bba9-229">„azure-mgmt-network“ auf 11.0.0 aktualisieren</span><span class="sxs-lookup"><span data-stu-id="0bba9-229">Bump azure-mgmt-network to 11.0.0</span></span>
* <span data-ttu-id="0bba9-230">`az network express-route gateway connection`: Routingkonfiguration unterstützen</span><span class="sxs-lookup"><span data-stu-id="0bba9-230">`az network express-route gateway connection`: support routing configuration</span></span>
* <span data-ttu-id="0bba9-231">`az network virtual-appliance`: Virtuelle Azure-Netzwerkgerät unterstützen.</span><span class="sxs-lookup"><span data-stu-id="0bba9-231">`az network virtual-appliance`: Support Azure network virtual appliance.</span></span>
* <span data-ttu-id="0bba9-232">Application Gateway-Unterstützung der Funktion für private Links</span><span class="sxs-lookup"><span data-stu-id="0bba9-232">Application Gateway support private link feature</span></span>

### <a name="policyinsights"></a><span data-ttu-id="0bba9-233">PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="0bba9-233">PolicyInsights</span></span>

* <span data-ttu-id="0bba9-234">`az policy state`: Befehl „trigger-scan“ zu Auswertungen der Compliance von Auslöserrichtinien hinzufügen</span><span class="sxs-lookup"><span data-stu-id="0bba9-234">`az policy state`: add trigger-scan command to trigger policy compliance evaluations</span></span>
* <span data-ttu-id="0bba9-235">`az policy state list`: Versionen von Richtlinienentitäten in jedem Compliancedatensatz verfügbar machen</span><span class="sxs-lookup"><span data-stu-id="0bba9-235">`az policy state list`: expose versions of policy entities in each compliance record</span></span>

### <a name="profile"></a><span data-ttu-id="0bba9-236">Profil</span><span class="sxs-lookup"><span data-stu-id="0bba9-236">Profile</span></span>

* <span data-ttu-id="0bba9-237">`az account get-access-token`: „expiresOn“ für verwaltete Identität anzeigen</span><span class="sxs-lookup"><span data-stu-id="0bba9-237">`az account get-access-token`: Show expiresOn for Managed Identity</span></span>

### <a name="rdbms"></a><span data-ttu-id="0bba9-238">RDBMS</span><span class="sxs-lookup"><span data-stu-id="0bba9-238">RDBMS</span></span>

* <span data-ttu-id="0bba9-239">TLS-Mindestversion unterstützen</span><span class="sxs-lookup"><span data-stu-id="0bba9-239">Support Minimum TLS version</span></span>
* <span data-ttu-id="0bba9-240">Infrastrukturverschlüsselung für Azure Postgres und MySQL hinzufügen</span><span class="sxs-lookup"><span data-stu-id="0bba9-240">Add Infrastructure Encryption for Azure Postgres and MySQL</span></span>

### <a name="security"></a><span data-ttu-id="0bba9-241">Sicherheit</span><span class="sxs-lookup"><span data-stu-id="0bba9-241">Security</span></span>

* <span data-ttu-id="0bba9-242">Befehl „allowed_connections“ hinzufügen</span><span class="sxs-lookup"><span data-stu-id="0bba9-242">Add allowed_connections commands</span></span>
* <span data-ttu-id="0bba9-243">Befehle für adaptive Netzwerkhärtung hinzufügen</span><span class="sxs-lookup"><span data-stu-id="0bba9-243">Add Adaptive network hardeningss commands</span></span>
* <span data-ttu-id="0bba9-244">Befehle vom Typ „adaptive_application_controls“ hinzufügen</span><span class="sxs-lookup"><span data-stu-id="0bba9-244">Add adaptive_application_controls commands</span></span>
* <span data-ttu-id="0bba9-245">Hinzufügen von „az security iot-solution“/„iot-alerts“/„iot-recommendations“/„iot-analytics“ REST zu Azure CLI</span><span class="sxs-lookup"><span data-stu-id="0bba9-245">Addition of az security iot-solution/ iot-alerts/iot-recommendations/iot-analytics REST to Azure CLI</span></span>
* <span data-ttu-id="0bba9-246">CLI für Einhaltung gesetzlicher Bestimmungen hinzufügen</span><span class="sxs-lookup"><span data-stu-id="0bba9-246">Add regulatory compliance CLI</span></span>

### <a name="signalr"></a><span data-ttu-id="0bba9-247">SignalR</span><span class="sxs-lookup"><span data-stu-id="0bba9-247">SignalR</span></span>

* <span data-ttu-id="0bba9-248">Features einschließlich der Verwaltung privater Endpunktverbindungen, Netzwerkregeln und Upstream hinzufügen</span><span class="sxs-lookup"><span data-stu-id="0bba9-248">Add features including managing private endpoint connections, network rules and upstream</span></span>

### <a name="sql"></a><span data-ttu-id="0bba9-249">SQL</span><span class="sxs-lookup"><span data-stu-id="0bba9-249">SQL</span></span>

* <span data-ttu-id="0bba9-250">`az sql mi create`, `az sql mi update`: Parameter `--tags` zur Unterstützung von Ressourcenkennzeichnung hinzufügen</span><span class="sxs-lookup"><span data-stu-id="0bba9-250">`az sql mi create`, `az sql mi update`: Add `--tags` parameter to support resource tagging</span></span>
* <span data-ttu-id="0bba9-251">`az sql mi failover`: Failover vom primären oder sekundären Punkt unterstützen</span><span class="sxs-lookup"><span data-stu-id="0bba9-251">`az sql mi failover`: Support failover from primary or secondary point</span></span>

### <a name="storage"></a><span data-ttu-id="0bba9-252">Storage</span><span class="sxs-lookup"><span data-stu-id="0bba9-252">Storage</span></span>

* <span data-ttu-id="0bba9-253">`az storage account create/update`: „--allow-blob-public-access“ hinzufügen, um den öffentlichen Zugriff für Blob und Container zuzulassen oder zu unterbinden</span><span class="sxs-lookup"><span data-stu-id="0bba9-253">`az storage account create/update`: Add --allow-blob-public-access to allow or disallow public access for blob and containers</span></span>
* <span data-ttu-id="0bba9-254">`az storage account create/update`: `--min-tls-version` hinzufügen, um das Festlegen der TLS-Mindestversion für Anforderungen an den Speicher zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="0bba9-254">`az storage account create/update`: Add `--min-tls-version` to support setting the minimum TLS version to be permitted on requests to storage.</span></span>
* <span data-ttu-id="0bba9-255">Token-Anmeldeinformationen zum Einchecken entfernen</span><span class="sxs-lookup"><span data-stu-id="0bba9-255">Remove check in token credential</span></span>
* <span data-ttu-id="0bba9-256">Namen des Speicherkontos in Beispielen korrigieren</span><span class="sxs-lookup"><span data-stu-id="0bba9-256">Fix the storage account name in examples</span></span>

### <a name="webapp"></a><span data-ttu-id="0bba9-257">Webapp</span><span class="sxs-lookup"><span data-stu-id="0bba9-257">Webapp</span></span>

* <span data-ttu-id="0bba9-258">Fehlerbehebung: „az webapp log deployment show -“ gibt Bereitstellungsprotokolle anstatt von Protokollmetadaten zurück</span><span class="sxs-lookup"><span data-stu-id="0bba9-258">Bugfix: az webapp log deployment show - return deployment logs instead of log metadata</span></span>
* <span data-ttu-id="0bba9-259">Fehlerbehebung: „az webapp vnet-integration“ hinzufügen – Fehlerbehandlung korrigieren bei ungültigem VNET-Namen, VNET-Ressourcen-ID unterstützen</span><span class="sxs-lookup"><span data-stu-id="0bba9-259">Bugfix: az webapp vnet-integration add - fix error handling if bad vnet name, support vnet resource ID</span></span>

## <a name="june-23-2020"></a><span data-ttu-id="0bba9-260">23. Juni 2020</span><span class="sxs-lookup"><span data-stu-id="0bba9-260">June 23, 2020</span></span>

<span data-ttu-id="0bba9-261">Version 2.8.0</span><span class="sxs-lookup"><span data-stu-id="0bba9-261">Version 2.8.0</span></span>

### <a name="acr"></a><span data-ttu-id="0bba9-262">ACR</span><span class="sxs-lookup"><span data-stu-id="0bba9-262">ACR</span></span>

* <span data-ttu-id="0bba9-263">Unterstützung für Deaktivierung des Regionsendpunkts/Routings hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-263">Add support for region endpoint disable / routing disable</span></span>
* <span data-ttu-id="0bba9-264">[BREAKING CHANGE] `az acr login --expose-token` akzeptiert Benutzername und Kennwort nicht.</span><span class="sxs-lookup"><span data-stu-id="0bba9-264">[BREAKING CHANGE] `az acr login --expose-token` does not accept username and password</span></span>

### <a name="acs"></a><span data-ttu-id="0bba9-265">ACS</span><span class="sxs-lookup"><span data-stu-id="0bba9-265">ACS</span></span>

* <span data-ttu-id="0bba9-266">Privater Cluster und API „2019-10-27-preview“ entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-266">Remove private cluster and 2019-10-27-preview API</span></span>

### <a name="aks"></a><span data-ttu-id="0bba9-267">AKS</span><span class="sxs-lookup"><span data-stu-id="0bba9-267">AKS</span></span>

* <span data-ttu-id="0bba9-268">Unterstützung: Ja, für „az aks upgrade“</span><span class="sxs-lookup"><span data-stu-id="0bba9-268">Support --yes for az aks upgrade</span></span>
* <span data-ttu-id="0bba9-269">„Änderung der Standard-VM-SKU in Standard_D2s_v3 (Nr. 13541)“ wiederhergestellt</span><span class="sxs-lookup"><span data-stu-id="0bba9-269">Revert "change default vm sku to Standard_D2s_v3 (#13541)"</span></span>
* <span data-ttu-id="0bba9-270">„az aks update --uptime-sla“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-270">Add "az aks update --uptime-sla"</span></span>
* <span data-ttu-id="0bba9-271">Tippfehler im Befehl „az aks update“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-271">Fix typo in az aks update command</span></span>
* <span data-ttu-id="0bba9-272">Änderung, um einen Agentpool mit 0 Knoten zu unterstützen und die manuelle Skalierung für einen Pool mit CAS-Aktivierung zu blockieren</span><span class="sxs-lookup"><span data-stu-id="0bba9-272">Change to support 0 node agent pool and block manual scale for CAS enabled pool</span></span>
* <span data-ttu-id="0bba9-273">Tippfehler in VirtualMachineScaleSets korrigiert und Verweise auf Kubernetes-Versionen aktualisiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-273">Fix typo on VirtualMachineScaleSets and update references to Kubernetes versions</span></span>

### <a name="ams"></a><span data-ttu-id="0bba9-274">AMS</span><span class="sxs-lookup"><span data-stu-id="0bba9-274">AMS</span></span>

* <span data-ttu-id="0bba9-275">ÄNDERUNG: Hilfetext für Parameter „--expiry“</span><span class="sxs-lookup"><span data-stu-id="0bba9-275">CHANGE help text for "--expiry" parameter.</span></span>

### <a name="appservice"></a><span data-ttu-id="0bba9-276">AppService</span><span class="sxs-lookup"><span data-stu-id="0bba9-276">AppService</span></span>

* <span data-ttu-id="0bba9-277">`az webapp log deployment show`: Anzeigen des aktuellen Bereitstellungsprotokolls oder der Bereitstellungsprotokolle einer bestimmten Bereitstellung, wenn die Bereitstellungs-ID angegeben ist</span><span class="sxs-lookup"><span data-stu-id="0bba9-277">`az webapp log deployment show`: Show the latest deployment log, or the deployment logs of a specific deployment if deployment-id is specified</span></span>
* <span data-ttu-id="0bba9-278">`az webapp log deployment list`: Liste der verfügbaren Bereitstellungsprotokolle</span><span class="sxs-lookup"><span data-stu-id="0bba9-278">`az webapp log deployment list`: List of deployment logs available</span></span>
* <span data-ttu-id="0bba9-279">Behebung: Oberflächenfehler bei Angabe eines ungültigen Web-App-Namens</span><span class="sxs-lookup"><span data-stu-id="0bba9-279">Fix: Surface error when invalid webapp name provided</span></span>
* <span data-ttu-id="0bba9-280">Nr. 13261 korrigiert: „az webapp list-runtimes“ nutzt eine statische Liste, bis die neue API für verfügbare Stapel zur Verfügung steht</span><span class="sxs-lookup"><span data-stu-id="0bba9-280">Fix #13261 az webapp list-runtimes use static list until new Available Stacks API is available</span></span>
* <span data-ttu-id="0bba9-281">`az appservice ase create`: Erstellungsproblem behoben (Nr. 13361)</span><span class="sxs-lookup"><span data-stu-id="0bba9-281">`az appservice ase create`: Fix create issue #13361</span></span>
* <span data-ttu-id="0bba9-282">`az appservice ase list-addresses`: SDK-Änderung korrigiert (Nr. 13140)</span><span class="sxs-lookup"><span data-stu-id="0bba9-282">`az appservice ase list-addresses`: Fix change of SDK #13140.</span></span>
* <span data-ttu-id="0bba9-283">Web-App-/Sloterstellung für Windows-Container korrigiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-283">Fix webapp/slot creation for Windows Containers</span></span>
* <span data-ttu-id="0bba9-284">`az webapp auth update`: Optionaler Parameter zum Aktualisieren der Laufzeitversion hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-284">`az webapp auth update`: Add optional parameter to update runtime-version</span></span>
* <span data-ttu-id="0bba9-285">Unterstützung für das Auflisten, Löschen, Genehmigen und Ablehnen der Verbindung mit privatem Endpunkt für eine Web-App in der CLI</span><span class="sxs-lookup"><span data-stu-id="0bba9-285">Support list, delete, approve and reject private endpoint connection for webapp in CLI</span></span>
* <span data-ttu-id="0bba9-286">Behebung Nr. 13888: Unterstützung für Static Web Apps hinzugefügt: Befehle zum Abrufen, Auflisten und Erstellen</span><span class="sxs-lookup"><span data-stu-id="0bba9-286">Fix #13888 : Add support for Static WebApps: get, list, create commands</span></span>
* <span data-ttu-id="0bba9-287">Fehlermeldungen für die SSH-Tunnelverbindung verbessert</span><span class="sxs-lookup"><span data-stu-id="0bba9-287">Improved error messages for SSH Tunnel Connection</span></span>

### <a name="arm"></a><span data-ttu-id="0bba9-288">ARM</span><span class="sxs-lookup"><span data-stu-id="0bba9-288">ARM</span></span>

* <span data-ttu-id="0bba9-289">`az tag`: Beispiele für „-h“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-289">`az tag`: Add examples for -h</span></span>
* <span data-ttu-id="0bba9-290">`az deployment group/sub what-if`: Parameter „--exclude-change-types/-x“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-290">`az deployment group/sub what-if`: Add --exclude-change-types/-x parameter.</span></span>
* <span data-ttu-id="0bba9-291">`az deployment group/sub/mg/tenant create`: Parameter „--what-if-exclude-change-types/-x“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-291">`az deployment group/sub/mg/tenant create`: Add --what-if-exclude-change-types/-x parameter.</span></span>
* <span data-ttu-id="0bba9-292">`az deployment group/sub/mg/tenant validate`: Anzeigen von Fehlermeldungen in einem besseren Format</span><span class="sxs-lookup"><span data-stu-id="0bba9-292">`az deployment group/sub/mg/tenant validate`: Show error messages in a better format.</span></span>
* <span data-ttu-id="0bba9-293">`az group export`: Neue Parameter `--skip-resource-name-params` und `--skip-all-params` hinzugefügt, um das Überspringen der Parametrisierung zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="0bba9-293">`az group export`: Add new parameters `--skip-resource-name-params` and `--skip-all-params` to support skip parameterization</span></span>
* <span data-ttu-id="0bba9-294">API „az feature unregister“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-294">Add az feature unregister api</span></span>

### <a name="aro"></a><span data-ttu-id="0bba9-295">ARO</span><span class="sxs-lookup"><span data-stu-id="0bba9-295">ARO</span></span>

* <span data-ttu-id="0bba9-296">„Public“/„Private“ zu Parametern zur Unterstützung bei Eingangs-/APIServer-Sichtbarkeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-296">Add Public, Private to params for help with ingress/apiserver visibility</span></span>

### <a name="batch"></a><span data-ttu-id="0bba9-297">Batch</span><span class="sxs-lookup"><span data-stu-id="0bba9-297">Batch</span></span>

* <span data-ttu-id="0bba9-298">`az batch account create`: Neuer Parameter `--public-network-access` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-298">`az batch account create`: Add new parameter `--public-network-access`</span></span>
* <span data-ttu-id="0bba9-299">`az batch account create`: Neuer Parameter `--identity-type` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-299">`az batch account create`: Add new parameter `--identity-type`</span></span>
* <span data-ttu-id="0bba9-300">`az batch account set`: Neuer Parameter `--identity-type` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-300">`az batch account set`: Add new parameter `--identity-type`</span></span>
* <span data-ttu-id="0bba9-301">[BREAKING CHANGE] az batch pool create: Bei der Erstellung eines Pools mithilfe eines benutzerdefinierten Images kann die Eigenschaft „--image“ nun ausschließlich auf ein Shared Image Gallery-Image verweisen.</span><span class="sxs-lookup"><span data-stu-id="0bba9-301">[BREAKING CHANGE] az batch pool create: When creating a pool using a custom image, the --image property of can now only refer to a Shared Image Gallery image.</span></span>
* <span data-ttu-id="0bba9-302">[BREAKING CHANGE] az batch pool create: Bei der Erstellung eines Pools mit der Option „--json-file“ und Angabe einer Netzwerkkonfiguration (networkConfiguration) wurde die Eigenschaft „publicIPs“ in die neue Eigenschaft „publicIPAddressConfiguration“ verschoben.</span><span class="sxs-lookup"><span data-stu-id="0bba9-302">[BREAKING CHANGE] az batch pool create: When creating a pool with --json-file option and specifying a networkConfiguration, the publicIPs property has moved in to a new property publicIPAddressConfiguration.</span></span> <span data-ttu-id="0bba9-303">Diese neue Eigenschaft unterstützt außerdem die neue Eigenschaft „ipAddressProvisioningType“. Diese gibt an, wie der Pool IP-Adressen und die Eigenschaft „publicIPs“ zuordnen muss, um die Konfiguration einer Liste mit PublicIP-Ressourcen zu ermöglichen, die bei der Festlegung von „ipAddressProvisioningType“ auf „UserManaged“ verwendet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="0bba9-303">This new property also supports a new ipAddressProvisioningType property which specifies how the pool should allocate IP's and a publicIPs property which allows for configuration of a list of PublicIP resources to use in the case ipAddressProvisioningType is set to UserManaged</span></span>
* <span data-ttu-id="0bba9-304">`az network private-link-resource`: Unterstützung für die Microsoft.Batch-Ressource „batchAccount“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-304">`az network private-link-resource`: Add support for the Microsoft.Batch batchAccount resource</span></span>
* <span data-ttu-id="0bba9-305">`az network private-endpoint-connection`: Unterstützung für die Microsoft.Batch-Ressource „batchAccount“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-305">`az network private-endpoint-connection`: Add support for the Microsoft.Batch batchAccount resource</span></span>

### <a name="cdn"></a><span data-ttu-id="0bba9-306">CDN</span><span class="sxs-lookup"><span data-stu-id="0bba9-306">CDN</span></span>

* <span data-ttu-id="0bba9-307">`az cdn custom-domain enable-https`: Unterstützung für BYOC hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-307">`az cdn custom-domain enable-https`: Add BYOC support.</span></span>
* <span data-ttu-id="0bba9-308">`az cdn custom-domain enable-https`: Aktivierung von benutzerdefiniertem HTTPS mit CDN-verwalteten Zertifikaten für die SKUs Standard_Verizon und Standard_Microsoft korrigiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-308">`az cdn custom-domain enable-https`: Fix enabling custom HTTPS with CDN managed certificates for Standard_Verizon and Standard_Microsoft SKUs.</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="0bba9-309">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="0bba9-309">Cognitive Services</span></span>

* <span data-ttu-id="0bba9-310">[BREAKING CHANGE] `az cognitiveservices account` besitzt nun eine einheitliche Struktur für alle Befehle.</span><span class="sxs-lookup"><span data-stu-id="0bba9-310">[BREAKING CHANGE] `az cognitiveservices account` now have a unified structure for all commands.</span></span>
* <span data-ttu-id="0bba9-311">`az cognitiveservices account identity`: Identitätsverwaltung für Cognitive Services hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-311">`az cognitiveservices account identity`: Add identity management for Cognitive Services.</span></span>

### <a name="compute"></a><span data-ttu-id="0bba9-312">Compute</span><span class="sxs-lookup"><span data-stu-id="0bba9-312">Compute</span></span>

* <span data-ttu-id="0bba9-313">`az image builder`: API-Version auf 2020-02-14 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-313">`az image builder`: Upgrade API version to 2020-02-14</span></span>
* <span data-ttu-id="0bba9-314">`az image builder create`: `--identity` zur Unterstützung der Identitätskonfiguration hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-314">`az image builder create`: Add `--identity` to support identity configuration</span></span>
* <span data-ttu-id="0bba9-315">`az image builder customizer add`: Unterstützung für Windows Update-Anpassung</span><span class="sxs-lookup"><span data-stu-id="0bba9-315">`az image builder customizer add`: Support Windows update customizer</span></span>
* <span data-ttu-id="0bba9-316">Neuer Befehl `az image builder cancel`</span><span class="sxs-lookup"><span data-stu-id="0bba9-316">New command `az image builder cancel`</span></span>
* <span data-ttu-id="0bba9-317">Anzeigen einer Warnung, wenn ein Benutzer eine VMSS bereitstellt, die an eine bestimmte (und nicht an die neueste) Imageversion angeheftet ist</span><span class="sxs-lookup"><span data-stu-id="0bba9-317">Show a warning when a user deploys a VMSS pinned to a specific image version rather than latest</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="0bba9-318">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="0bba9-318">Cosmos DB</span></span>

* <span data-ttu-id="0bba9-319">`az cosmosdb`: Befehl „exists“ zu Datenbank- und Containergruppen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-319">`az cosmosdb`: Add exists command to database and container groups</span></span>
* <span data-ttu-id="0bba9-320">Zulassen der Erstellung fester Sammlungen</span><span class="sxs-lookup"><span data-stu-id="0bba9-320">Allow creating fixed collections</span></span>

### <a name="eventhub"></a><span data-ttu-id="0bba9-321">EventHub</span><span class="sxs-lookup"><span data-stu-id="0bba9-321">EventHub</span></span>

* <span data-ttu-id="0bba9-322">`az eventhubs namespace create` : Parameter für verwaltete Identität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-322">`az eventhubs namespace create` : Add managed identity parameters</span></span>

### <a name="extension"></a><span data-ttu-id="0bba9-323">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="0bba9-323">Extension</span></span>

* <span data-ttu-id="0bba9-324">„--version“ hinzugefügt, um die Installation über eine bestimmte Version zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="0bba9-324">Add --version to support to install from a specific version</span></span>
* <span data-ttu-id="0bba9-325">CLI-Erweiterungen dürfen nun Pakete im Namespace „azure“ enthalten.</span><span class="sxs-lookup"><span data-stu-id="0bba9-325">Enable CLI extensions to include packages in the 'azure' namespace</span></span>

### <a name="iot-hub"></a><span data-ttu-id="0bba9-326">IoT Hub</span><span class="sxs-lookup"><span data-stu-id="0bba9-326">Iot Hub</span></span>

* <span data-ttu-id="0bba9-327">[BREAKING CHANGE] az iot hub job: Veraltete job-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-327">[BREAKING CHANGE] az iot hub job: Remove deprecated job commands</span></span>

### <a name="keyvault"></a><span data-ttu-id="0bba9-328">KeyVault</span><span class="sxs-lookup"><span data-stu-id="0bba9-328">KeyVault</span></span>

* <span data-ttu-id="0bba9-329">`az keyvault key import`: Unterstützt das Importieren aus Zeichenfolgen über zwei neue Parameter.</span><span class="sxs-lookup"><span data-stu-id="0bba9-329">`az keyvault key import`: Supports importing from strings via two new parameters.</span></span>
* <span data-ttu-id="0bba9-330">Unterstützung der Ver- und Entschlüsselung von Zeichenfolgen/Bytes mit gespeicherten Schlüsseln</span><span class="sxs-lookup"><span data-stu-id="0bba9-330">Support string/bytes encryption and decryption with stored keys</span></span>

### <a name="monitor"></a><span data-ttu-id="0bba9-331">Überwachen</span><span class="sxs-lookup"><span data-stu-id="0bba9-331">Monitor</span></span>

* <span data-ttu-id="0bba9-332">Unterstützung für „no wait“ bei der Clustererstellung</span><span class="sxs-lookup"><span data-stu-id="0bba9-332">Support no wait for cluster creation</span></span>
* <span data-ttu-id="0bba9-333">`az monitor log-analytics workspace saved-search`: Unterstützung neuer Befehle für gespeicherte Suche</span><span class="sxs-lookup"><span data-stu-id="0bba9-333">`az monitor log-analytics workspace saved-search`: Support new commands for saved search</span></span>

### <a name="network"></a><span data-ttu-id="0bba9-334">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0bba9-334">Network</span></span>

* <span data-ttu-id="0bba9-335">`az network application-gateway address-pool update`: Hilfenachricht optimiert und Beispiele hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-335">`az network application-gateway address-pool update`: Refine help message and add examples.</span></span>
* <span data-ttu-id="0bba9-336">`az network vnet create`: Unterstützung für das Argument „--nsg“</span><span class="sxs-lookup"><span data-stu-id="0bba9-336">`az network vnet create`: Support --nsg argument</span></span>
* <span data-ttu-id="0bba9-337">`az network lb address-pool`: Unterstützung für das Erstellen eines Back-End-Pools des Lastenausgleichs mit Back-End-Adresse</span><span class="sxs-lookup"><span data-stu-id="0bba9-337">`az network lb address-pool`: Support create lb backend pool with backend address.</span></span>
* <span data-ttu-id="0bba9-338">`az network application-gateway address-pool`: Korrektur für das Argument „--add“</span><span class="sxs-lookup"><span data-stu-id="0bba9-338">`az network application-gateway address-pool`: Fix for --add argument</span></span>

### <a name="rbac"></a><span data-ttu-id="0bba9-339">RBAC</span><span class="sxs-lookup"><span data-stu-id="0bba9-339">RBAC</span></span>

* <span data-ttu-id="0bba9-340">`az ad sp create-for-rabc`: Unterstützung von Namen mit Leerzeichen, Schrägstrich und umgekehrtem Schrägstrich</span><span class="sxs-lookup"><span data-stu-id="0bba9-340">`az ad sp create-for-rabc`: Support name with space, slash and back slash</span></span>
* <span data-ttu-id="0bba9-341">`az ad sp create-for-rbac`: Fehlermeldung optimiert, die angezeigt wird, wenn Benutzer einen ungültigen Bereich angeben</span><span class="sxs-lookup"><span data-stu-id="0bba9-341">`az ad sp create-for-rbac`: Refine error message when user specify an invalid scope</span></span>

### <a name="security"></a><span data-ttu-id="0bba9-342">Sicherheit</span><span class="sxs-lookup"><span data-stu-id="0bba9-342">Security</span></span>

* <span data-ttu-id="0bba9-343">Befehle für Sicherheitsbewertungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-343">Add security assessment commands</span></span>

### <a name="sql"></a><span data-ttu-id="0bba9-344">SQL</span><span class="sxs-lookup"><span data-stu-id="0bba9-344">SQL</span></span>

* <span data-ttu-id="0bba9-345">`az sql db ltr-policy/ltr-backup`: Aktualisieren/Anzeigen der Richtlinie zur langfristigen Aufbewahrung, Anzeigen/Löschen von Sicherungen zur langfristigen Aufbewahrung, Wiederherstellen von Sicherungen zur langfristigen Aufbewahrung</span><span class="sxs-lookup"><span data-stu-id="0bba9-345">`az sql db ltr-policy/ltr-backup`: update/show long term retention policy, show/delete long term retention backups, restore long term retention backup</span></span>

### <a name="storage"></a><span data-ttu-id="0bba9-346">Storage</span><span class="sxs-lookup"><span data-stu-id="0bba9-346">Storage</span></span>

* <span data-ttu-id="0bba9-347">Authentifizierungsproblem behoben, um das Abrufen eines Tokens für „--subscription“ zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="0bba9-347">Fix authentication issue to support get token for --subscription</span></span>
* <span data-ttu-id="0bba9-348">`az storage remove`: Problem Nr. 13459 behoben, um eine Ausnahme bei einem Vorgangsfehler auszulösen</span><span class="sxs-lookup"><span data-stu-id="0bba9-348">`az storage remove`: Fix issue #13459 to raise exception for operation failure</span></span>
* <span data-ttu-id="0bba9-349">Probleme Nr. 13012, 13632 und 13657 behoben, um nicht verwendete Argumente für Befehle im Zusammenhang mit „generate-sas“ zu entfernen</span><span class="sxs-lookup"><span data-stu-id="0bba9-349">Fix issues #13012, #13632 and #13657 to remove unused arguments for generate-sas related commands</span></span>
* <span data-ttu-id="0bba9-350">`az storage logging update`: Überprüfung für Protokollierungsversion hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-350">`az storage logging update`: Add check for logging version</span></span>
* <span data-ttu-id="0bba9-351">`az storage blob show`: Weitere Eigenschaften für Blob mit Track 2 SDK hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-351">`az storage blob show`: Add more properties for blob with track 2 SDK</span></span>
* <span data-ttu-id="0bba9-352">Behebung Nr. 13708: Warnmeldung für Anmeldeinformationen optimiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-352">Fix #13708: Refine warning message for credential</span></span>
* <span data-ttu-id="0bba9-353">`az storage share-rm create/update`: Unterstützung für NFS-Protokoll und Root-Squash hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-353">`az storage share-rm create/update`: Add NFS protocol and root squash support</span></span>
* <span data-ttu-id="0bba9-354">`az storage account create`: Unterstützung für doppelte Verschlüsselung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-354">`az storage account create`: Add support for double encryption</span></span>
* <span data-ttu-id="0bba9-355">[BREAKING CHANGE] `az storage blob/container/file/share/table/queue generate-sas`: „--expiry“ und „--permissions“ als erforderlich festgelegt</span><span class="sxs-lookup"><span data-stu-id="0bba9-355">[BREAKING CHANGE] `az storage blob/container/file/share/table/queue generate-sas`: make --expiry and --permissions required</span></span>
* <span data-ttu-id="0bba9-356">`az storage blob set-tier`: Migration zu Track 2, um das Festlegen der Aktivierungspriorität zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="0bba9-356">`az storage blob set-tier`: Migrate to Track 2 to support setting rehydrate priority</span></span>

## <a name="june-02-2020"></a><span data-ttu-id="0bba9-357">2\. Juni 2020</span><span class="sxs-lookup"><span data-stu-id="0bba9-357">June 02, 2020</span></span>

<span data-ttu-id="0bba9-358">Version 2.7.0</span><span class="sxs-lookup"><span data-stu-id="0bba9-358">Version 2.7.0</span></span>

### <a name="acr"></a><span data-ttu-id="0bba9-359">ACR</span><span class="sxs-lookup"><span data-stu-id="0bba9-359">ACR</span></span>

* <span data-ttu-id="0bba9-360">Tippfehler in einer Fehlermeldung der Tokenerstellung korrigiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-360">Fix a typo in an error message of token creation</span></span>

### <a name="aks"></a><span data-ttu-id="0bba9-361">AKS</span><span class="sxs-lookup"><span data-stu-id="0bba9-361">AKS</span></span>

* <span data-ttu-id="0bba9-362">Standard-VM-SKU in „Standard_D2s_v3“ geändert</span><span class="sxs-lookup"><span data-stu-id="0bba9-362">Change default vm sku to Standard_D2s_v3</span></span>
* <span data-ttu-id="0bba9-363">Erstellung der Rollenzuweisung für MSI-Cluster plus benutzerdefiniertes Subnetz korrigiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-363">Fix creating role assignment for MSI clsuter plus custom subnet</span></span>

### <a name="appservice"></a><span data-ttu-id="0bba9-364">AppService</span><span class="sxs-lookup"><span data-stu-id="0bba9-364">AppService</span></span>

* <span data-ttu-id="0bba9-365">Fehlerbehebung Nr. 12739: Von „az appservice list-locations“ werden einige ungültige Standorte zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0bba9-365">Fix #12739 az appservice list-locations returns some invalid locations</span></span>

### <a name="arm"></a><span data-ttu-id="0bba9-366">ARM</span><span class="sxs-lookup"><span data-stu-id="0bba9-366">ARM</span></span>

* <span data-ttu-id="0bba9-367">`az deployment`: Fehlerbehebung Nr. 13159 der fehlerhaften JSON-Meldung nach dem Entfernen von Kommentaren und nach dem Komprimieren</span><span class="sxs-lookup"><span data-stu-id="0bba9-367">`az deployment`: Fix issue #13159 of incorrect message of JSON after removing comments and compressing</span></span>
* <span data-ttu-id="0bba9-368">`az resource tag`: Fehlerbehebung Nr. 13255 für das Markieren von Ressourcen mit dem Ressourcentyp `Microsoft.ContainerRegistry/registries/webhooks`</span><span class="sxs-lookup"><span data-stu-id="0bba9-368">`az resource tag`: Fix issue #13255 of tagging resources with resource type `Microsoft.ContainerRegistry/registries/webhooks`</span></span>
* <span data-ttu-id="0bba9-369">Beispiele für das Ressourcenmodul verbessert</span><span class="sxs-lookup"><span data-stu-id="0bba9-369">Improve the examples for the resource module</span></span>

### <a name="aro"></a><span data-ttu-id="0bba9-370">ARO</span><span class="sxs-lookup"><span data-stu-id="0bba9-370">ARO</span></span>

* <span data-ttu-id="0bba9-371">CLIError in das richtige Flag für „--worker-vm-disk-size-gb“ geändert</span><span class="sxs-lookup"><span data-stu-id="0bba9-371">Change CLIError to correct flag for --worker-vm-disk-size-gb</span></span>

### <a name="eventhub"></a><span data-ttu-id="0bba9-372">EventHub</span><span class="sxs-lookup"><span data-stu-id="0bba9-372">EventHub</span></span>

* <span data-ttu-id="0bba9-373">Fehlerbehebung Nr. 12406: „intervalInSeconds“ wird von Argument „--capture-interval“ nicht aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="0bba9-373">Fix for issue #12406 Argument --capture-interval does not update the "intervalInSeconds"</span></span>

### <a name="hdinsight"></a><span data-ttu-id="0bba9-374">HDInsight</span><span class="sxs-lookup"><span data-stu-id="0bba9-374">HDInsight</span></span>

* <span data-ttu-id="0bba9-375">„get_json_object“ in „shell_safe_json_parse“ geändert</span><span class="sxs-lookup"><span data-stu-id="0bba9-375">Change get_json_object to shell_safe_json_parse</span></span>

### <a name="monitor"></a><span data-ttu-id="0bba9-376">Überwachen</span><span class="sxs-lookup"><span data-stu-id="0bba9-376">Monitor</span></span>

* <span data-ttu-id="0bba9-377">`az monitor metrics alert`: Verschiedene Hilfemeldungen optimiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-377">`az monitor metrics alert`: refine several help messages</span></span>
* <span data-ttu-id="0bba9-378">`az monitor diagnostic-settings create`: Unterstützung für das Argument „--export-to-resource-specific“</span><span class="sxs-lookup"><span data-stu-id="0bba9-378">`az monitor diagnostic-settings create`: support --export-to-resource-specific argument</span></span>
* <span data-ttu-id="0bba9-379">Unterstützung für die Wiederherstellung von LA-Arbeitsbereichen</span><span class="sxs-lookup"><span data-stu-id="0bba9-379">Support LA workspace recover</span></span>

### <a name="network"></a><span data-ttu-id="0bba9-380">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0bba9-380">Network</span></span>

* <span data-ttu-id="0bba9-381">`az network dns zone`: Unterstützung des Bindestrichs (-)</span><span class="sxs-lookup"><span data-stu-id="0bba9-381">`az network dns zone`: support - character</span></span>
* <span data-ttu-id="0bba9-382">`az network vpn-connection ipsec-policy`: „--sa-lifetime“ und „--sa-max-size“ im Beispiel in höhere Werte geändert</span><span class="sxs-lookup"><span data-stu-id="0bba9-382">`az network vpn-connection ipsec-policy`: change the --sa-lifetime and --sa-max-size to larger values in example</span></span>
* <span data-ttu-id="0bba9-383">Netzwerk auf 2020-04-01 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-383">Bump network to 2020-04-01</span></span>
* <span data-ttu-id="0bba9-384">`az network private-endpoint-connection`: Unterstützung von Event Grid</span><span class="sxs-lookup"><span data-stu-id="0bba9-384">`az network private-endpoint-connection`: support event grid</span></span>
* <span data-ttu-id="0bba9-385">`az network express-route list-route-tables`: Fehler behoben, der dazu führte, dass Routen nicht als Tabelle aufgeführt werden konnten</span><span class="sxs-lookup"><span data-stu-id="0bba9-385">`az network express-route list-route-tables`: fix bug that cannot list routes as table</span></span>

### <a name="packaging"></a><span data-ttu-id="0bba9-386">Verpackung</span><span class="sxs-lookup"><span data-stu-id="0bba9-386">Packaging</span></span>

* <span data-ttu-id="0bba9-387">Ubuntu-Paket (Focal) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-387">Add Ubuntu Focal Package</span></span>

### <a name="rbac"></a><span data-ttu-id="0bba9-388">RBAC</span><span class="sxs-lookup"><span data-stu-id="0bba9-388">RBAC</span></span>

* <span data-ttu-id="0bba9-389">`az ad sp credential reset`: Erstellung von Anmeldeinformationen geändert, um problematische Sonderzeichen zu vermeiden</span><span class="sxs-lookup"><span data-stu-id="0bba9-389">`az ad sp credential reset`: modify credential generation to avoid troublesome special characters</span></span>

### <a name="redis"></a><span data-ttu-id="0bba9-390">Redis</span><span class="sxs-lookup"><span data-stu-id="0bba9-390">Redis</span></span>

* <span data-ttu-id="0bba9-391">Fehlerbehebung Nr. 13529: Dokumentation des Parameters „enable_non_ssl_port“ geändert</span><span class="sxs-lookup"><span data-stu-id="0bba9-391">Fix #13529: Change documentation of parameter enable_non_ssl_port</span></span>

### <a name="storage"></a><span data-ttu-id="0bba9-392">Storage</span><span class="sxs-lookup"><span data-stu-id="0bba9-392">Storage</span></span>

* <span data-ttu-id="0bba9-393">`az storage copy`: Parameter `--follow-symlinks` zur Unterstützung von symbolischen Verknüpfungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-393">`az storage copy`: Add parameter `--follow-symlinks` to support symlinks</span></span>
* <span data-ttu-id="0bba9-394">Lokaler Kontext für Speicherkonto aktiviert</span><span class="sxs-lookup"><span data-stu-id="0bba9-394">Enable local context for storage account</span></span>
* <span data-ttu-id="0bba9-395">`az storage logging`: Fehlerbehebung Nr. 11969: Fehlermeldung optimiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-395">`az storage logging`: Fix issue #11969 to refine error message</span></span>

## <a name="may-19-2020"></a><span data-ttu-id="0bba9-396">19. Mai 2020</span><span class="sxs-lookup"><span data-stu-id="0bba9-396">May 19, 2020</span></span>

<span data-ttu-id="0bba9-397">Version 2.6.0</span><span class="sxs-lookup"><span data-stu-id="0bba9-397">Version 2.6.0</span></span>

### <a name="acr"></a><span data-ttu-id="0bba9-398">ACR</span><span class="sxs-lookup"><span data-stu-id="0bba9-398">ACR</span></span>

* <span data-ttu-id="0bba9-399">Standardtimeout von fünf Minuten für jede an ACR gesendete Anforderung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-399">Add default timeout of 5 minutes for any requests to ACR</span></span>
* <span data-ttu-id="0bba9-400">Unterstützung für das Deaktivieren des Zugriffs auf das öffentliche Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0bba9-400">Support disable public network access</span></span>
* <span data-ttu-id="0bba9-401">`az acr token create`: Argument „--days“ verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="0bba9-401">`az acr token create`: expose --days argument</span></span>
* <span data-ttu-id="0bba9-402">`az acr import`: Akzeptiert Werte für das Argument „--source“, bei denen der Servername einen Anmeldenamen enthält (mittels clientseitiger Korrektur)</span><span class="sxs-lookup"><span data-stu-id="0bba9-402">`az acr import`: accept --source argument values which contain login in server name through client end correction</span></span>

### <a name="acs"></a><span data-ttu-id="0bba9-403">ACS</span><span class="sxs-lookup"><span data-stu-id="0bba9-403">ACS</span></span>

* <span data-ttu-id="0bba9-404">Fehlerbehebung: Felderbereinigung für Felder entfernt, die nicht mehr vorhanden sind</span><span class="sxs-lookup"><span data-stu-id="0bba9-404">Bug fix: remove fields cleanup for fields that no longer exist</span></span>

### <a name="aks"></a><span data-ttu-id="0bba9-405">AKS</span><span class="sxs-lookup"><span data-stu-id="0bba9-405">AKS</span></span>

* <span data-ttu-id="0bba9-406">Hilfekontext des Befehls „uptime-sla“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-406">Update uptime-sla command help context</span></span>
* <span data-ttu-id="0bba9-407">Bereichsüberprüfung für die Aktualisierung der Mindestanzahl für die Autoskalierung entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-407">Remove range check for updating min count for autoscaler</span></span>
* <span data-ttu-id="0bba9-408">Hotfix, der bewirkt, dass bei der CLI kein Fehler auftritt, wenn der Benutzer nur das Windows-Kennwort angibt</span><span class="sxs-lookup"><span data-stu-id="0bba9-408">Fix that cli doe not fail when user only specifies Windows password</span></span>

### <a name="ams"></a><span data-ttu-id="0bba9-409">AMS</span><span class="sxs-lookup"><span data-stu-id="0bba9-409">AMS</span></span>

* <span data-ttu-id="0bba9-410">`az ams transform create`: Funktion zum Erstellen einer Transformation mit einer FaceDetector-Voreinstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-410">`az ams transform create`: Add ability to create a transform with a FaceDetector preset</span></span>
* <span data-ttu-id="0bba9-411">`az ams content-key-policy create` : Funktion zum Erstellen einer FairPlay-Inhaltsschlüsselrichtlinie mit einer Konfiguration für die Offlinemiete hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-411">`az ams content-key-policy create` : Add ability to create a FairPlay content key policy with an offline rental configuration</span></span>

### <a name="appconfig"></a><span data-ttu-id="0bba9-412">AppConfig</span><span class="sxs-lookup"><span data-stu-id="0bba9-412">AppConfig</span></span>

* <span data-ttu-id="0bba9-413">Fehlerbehebung für die Schlüsselauflistungswerte mit Feldern</span><span class="sxs-lookup"><span data-stu-id="0bba9-413">Bug fix for list key values with fields</span></span>

### <a name="appservice"></a><span data-ttu-id="0bba9-414">AppService</span><span class="sxs-lookup"><span data-stu-id="0bba9-414">AppService</span></span>

* <span data-ttu-id="0bba9-415">`az functionapp create`: AzureWebJobsDashboard wird nur festgelegt, wenn AppInsights deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="0bba9-415">`az functionapp create`: AzureWebJobsDashboard will only be set if AppInsights is disabled</span></span>
* <span data-ttu-id="0bba9-416">Fehlerbehebung Nr. 10664: VNET-Integration – Standortüberprüfungsfehler und Fehlerbehebung Nr. 13257: Fehler bei „az webapp up“, wenn eine Ressourcengruppe erstellt werden muss</span><span class="sxs-lookup"><span data-stu-id="0bba9-416">Fix #10664- VNet Integration - Location Check Issue & fix #13257- az webapp up failing when RG needs to be created</span></span>
* <span data-ttu-id="0bba9-417">`az webapp|functionapp config ssl import`: Ressourcengruppenübergreifende Suche des Schlüsseltresors im Abonnement und verbesserte Hilfe und Beispiele</span><span class="sxs-lookup"><span data-stu-id="0bba9-417">`az webapp|functionapp config ssl import`: Lookup key vault across resources groups in subscription and improve help and examples.</span></span>
* <span data-ttu-id="0bba9-418">Lokaler Kontext für App Service integriert</span><span class="sxs-lookup"><span data-stu-id="0bba9-418">Onboard local context for app service</span></span>

### <a name="arm"></a><span data-ttu-id="0bba9-419">ARM</span><span class="sxs-lookup"><span data-stu-id="0bba9-419">ARM</span></span>

* <span data-ttu-id="0bba9-420">`az deployment`: Problem behoben, das dazu führte, dass templateLink beim Bereitstellen oder Überprüfen von „template-uri“ nicht zurückgegeben wurde</span><span class="sxs-lookup"><span data-stu-id="0bba9-420">`az deployment`: Fix the problem that the templateLink will not be returned when deploying or validating template-uri</span></span>
* <span data-ttu-id="0bba9-421">`az deployment`: Problem behoben, das dazu führte, dass speziell codierte Zeichen von der Bereitstellung/Überprüfung nicht unterstützt wurden</span><span class="sxs-lookup"><span data-stu-id="0bba9-421">`az deployment`: Fix the problem that deployment/validate does not support specially encoded character</span></span>
* <span data-ttu-id="0bba9-422">`az deployment sub/group what-if`: Arrayausrichtung und Fehlerbehandlung korrigiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-422">`az deployment sub/group what-if`: Fix array alignment and error handling</span></span>
* <span data-ttu-id="0bba9-423">`az deployment operation`: Veraltete Informationen angepasst</span><span class="sxs-lookup"><span data-stu-id="0bba9-423">`az deployment operation`: Modify the deprecate information</span></span>

### <a name="aro"></a><span data-ttu-id="0bba9-424">ARO</span><span class="sxs-lookup"><span data-stu-id="0bba9-424">ARO</span></span>

* <span data-ttu-id="0bba9-425">Beispiele zu folgenden Befehlen hinzugefügt: az aro create, list, list-credentials, show, delete</span><span class="sxs-lookup"><span data-stu-id="0bba9-425">Add examples to az aro create, list, list-credentials, show, delete</span></span>
* <span data-ttu-id="0bba9-426">Funktion „generate_random_id“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-426">Add generate_random_id function</span></span>

### <a name="backup"></a><span data-ttu-id="0bba9-427">Backup</span><span class="sxs-lookup"><span data-stu-id="0bba9-427">Backup</span></span>

* <span data-ttu-id="0bba9-428">FriendlyName im Befehl zum Aktivieren des Schutzes für AzureFileShare zulässig</span><span class="sxs-lookup"><span data-stu-id="0bba9-428">Allow FriendlyName in enable protection for AzureFileShare command</span></span>
* <span data-ttu-id="0bba9-429">Korrektur im IaasVM-Befehl „restore-disks“</span><span class="sxs-lookup"><span data-stu-id="0bba9-429">Fix in IaasVM restore-disks Command</span></span>
* <span data-ttu-id="0bba9-430">BackupManagementType „MAB“ zum Befehl zum Auflisten der Elemente hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-430">Add "MAB" BackupManagementType to item list command</span></span>
* <span data-ttu-id="0bba9-431">Unterstützung für die Wiederholung des Richtlinienupdates für fehlerhafte Elemente hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-431">Add support for retrying policy update for failed items.</span></span>
* <span data-ttu-id="0bba9-432">Funktion zum Fortsetzen des Schutzes für virtuelle Azure-Computer hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-432">Add Resume Protection functionality for Azure Virtual Machine</span></span>
* <span data-ttu-id="0bba9-433">Unterstützung zum Angeben der Ressourcengruppe zum Speichern von instantRP beim Erstellen oder Ändern der Richtlinie hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-433">Add support to specify ResourceGroup for storing instantRP during Create or Modify Policy</span></span>

### <a name="ci"></a><span data-ttu-id="0bba9-434">CI</span><span class="sxs-lookup"><span data-stu-id="0bba9-434">CI</span></span>

* <span data-ttu-id="0bba9-435">Unterstützung für flake8 3.8.0</span><span class="sxs-lookup"><span data-stu-id="0bba9-435">Support flake8 3.8.0</span></span>

### <a name="compute"></a><span data-ttu-id="0bba9-436">Compute</span><span class="sxs-lookup"><span data-stu-id="0bba9-436">Compute</span></span>

* <span data-ttu-id="0bba9-437">Neuer Befehl: az vm auto-shutdown</span><span class="sxs-lookup"><span data-stu-id="0bba9-437">New command az vm auto-shutdown</span></span>
* <span data-ttu-id="0bba9-438">`az vm list-skus`: Verhalten von „--zone“aktualisiert. Jetzt werden alle SKU-Typen zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0bba9-438">`az vm list-skus`: Update --zone behavior, return all type skus now</span></span>

### <a name="core"></a><span data-ttu-id="0bba9-439">Core</span><span class="sxs-lookup"><span data-stu-id="0bba9-439">Core</span></span>

* <span data-ttu-id="0bba9-440">Aktivierungsstatus aus dem lokalen Kontext für globale Benutzerebene aktualisiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-440">Update local context on/off status to global user level</span></span>

### <a name="extension"></a><span data-ttu-id="0bba9-441">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="0bba9-441">Extension</span></span>

* <span data-ttu-id="0bba9-442">`az extension add`: „--system“ hinzugefügt, um die Installation von Erweiterungen in einem Systempfad zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="0bba9-442">`az extension add`: Add --system to enable installing extensions in a system path</span></span>
* <span data-ttu-id="0bba9-443">Unterstützung für „.egg-info“ zum Speichern der Metadaten für die Radtyperweiterung</span><span class="sxs-lookup"><span data-stu-id="0bba9-443">Support .egg-info to store wheel type extension metadata</span></span>

### <a name="iot"></a><span data-ttu-id="0bba9-444">IoT</span><span class="sxs-lookup"><span data-stu-id="0bba9-444">IoT</span></span>

* <span data-ttu-id="0bba9-445">`az iot`: Nachricht des IoT-Befehlsmoduls mit dem Hinweis auf die Erweiterung für die erste Ausführung aktualisiert, sodass sie anstelle der veralteten ID die korrekte moderne ID (`azure-iot`) enthält</span><span class="sxs-lookup"><span data-stu-id="0bba9-445">`az iot`: Update the IoT command module first run extension awareness message to the accurate, non-deprecated modern Id `azure-iot`.</span></span>

### <a name="iot-hub"></a><span data-ttu-id="0bba9-446">IoT Hub</span><span class="sxs-lookup"><span data-stu-id="0bba9-446">IoT Hub</span></span>

* <span data-ttu-id="0bba9-447">Unterstützung für API- und Netzwerkisolationsbefehle für 2020-03-01</span><span class="sxs-lookup"><span data-stu-id="0bba9-447">Support for 2020-03-01 API and Network Isolation commands</span></span>

### <a name="netappfiles"></a><span data-ttu-id="0bba9-448">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="0bba9-448">NetAppFiles</span></span>

* <span data-ttu-id="0bba9-449">`az volume create`: „snapshot-id“ als Parameter zum Erstellen eines Volumes hinzugefügt. Ermöglicht Benutzern das Erstellen eines Volumes auf der Grundlage einer vorhandenen Momentaufnahme.</span><span class="sxs-lookup"><span data-stu-id="0bba9-449">`az volume create`: Adds snapshot-id as a parameter to create volume this will allow users to create a volume from existing snapshot.</span></span>

### <a name="network"></a><span data-ttu-id="0bba9-450">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0bba9-450">Network</span></span>

* <span data-ttu-id="0bba9-451">TTL-Wert korrigiert, der für „dns add-record“ unbeabsichtigt geändert wurde</span><span class="sxs-lookup"><span data-stu-id="0bba9-451">Fix ttl value changed unintended for dns add-record</span></span>
* <span data-ttu-id="0bba9-452">`az network public-ip create`: Kunden über einen bevorstehenden Breaking Change informiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-452">`az network public-ip create`: Inform customers of a coming breaking change</span></span>
* <span data-ttu-id="0bba9-453">Unterstützung von generischen Befehlen für Private Link-Szenario</span><span class="sxs-lookup"><span data-stu-id="0bba9-453">Support generic commands for private link scenario</span></span>
* <span data-ttu-id="0bba9-454">`az network private-endpoint-connection`: Unterstützung für MySQL-, Postgre- und MariaDB-Typen</span><span class="sxs-lookup"><span data-stu-id="0bba9-454">`az network private-endpoint-connection`: Support mysql, postgre and mariadb types</span></span>
* <span data-ttu-id="0bba9-455">`az network private-endpoint-connection`: Unterstützung von CosmosDB-Typen</span><span class="sxs-lookup"><span data-stu-id="0bba9-455">`az network private-endpoint-connection`: Support cosmosdb types</span></span>
* <span data-ttu-id="0bba9-456">`az network private-endpoint`: „--group-ids“ und Umleitung an „--group-id“ als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="0bba9-456">`az network private-endpoint`: deprecate --group-ids and redirect to --group-id</span></span>

### <a name="output"></a><span data-ttu-id="0bba9-457">Output</span><span class="sxs-lookup"><span data-stu-id="0bba9-457">Output</span></span>

* <span data-ttu-id="0bba9-458">Anzeigen der Updateanweisung bei der Suche, beim Feedback und in „--help“</span><span class="sxs-lookup"><span data-stu-id="0bba9-458">Show update instruction in find, feedback and --help</span></span>

### <a name="packaging"></a><span data-ttu-id="0bba9-459">Verpackung</span><span class="sxs-lookup"><span data-stu-id="0bba9-459">Packaging</span></span>

* <span data-ttu-id="0bba9-460">Erstellen von MSI-/Homebrew-Paketen mit Abhängigkeiten, die aus „requirements.txt“ aufgelöst werden</span><span class="sxs-lookup"><span data-stu-id="0bba9-460">Build MSI/Homebrew packages with dependecies resolved from requirements.txt</span></span>

### <a name="rbac"></a><span data-ttu-id="0bba9-461">RBAC</span><span class="sxs-lookup"><span data-stu-id="0bba9-461">RBAC</span></span>

* <span data-ttu-id="0bba9-462">`az ad sp credential reset`: Erstellung unsicherer Anmeldeinformationen korrigiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-462">`az ad sp credential reset`: fix weak credential generation</span></span>

### <a name="storage"></a><span data-ttu-id="0bba9-463">Storage</span><span class="sxs-lookup"><span data-stu-id="0bba9-463">Storage</span></span>

* <span data-ttu-id="0bba9-464">`az storage account file-service-properties update/show`: Unterstützung für Dateieigenschaften für Speicherkonto hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-464">`az storage account file-service-properties update/show`: Add File Properties Support for Storage Account</span></span>
* <span data-ttu-id="0bba9-465">`az storage container create`: Fehlerbehebung Nr. 13373 durch Hinzufügen eines Validierungssteuerelements für öffentlichen Zugriff</span><span class="sxs-lookup"><span data-stu-id="0bba9-465">`az storage container create`: Fix #13373 by adding validator for public access</span></span>
* <span data-ttu-id="0bba9-466">Unterstützung für ADLS Gen2 (track2) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-466">Add ADLS Gen2 track2 support</span></span>
* <span data-ttu-id="0bba9-467">`az storage blob sync`: Unterstützung für `--connection-string`</span><span class="sxs-lookup"><span data-stu-id="0bba9-467">`az storage blob sync`: Support `--connection-string`</span></span>
* <span data-ttu-id="0bba9-468">`az storage blob sync`: Falsche Fehlermeldung korrigiert, die angezeigt wird, wenn der Installationsspeicherort von „azcopy“ nicht gefunden wird</span><span class="sxs-lookup"><span data-stu-id="0bba9-468">`az storage blob sync`: Fix the incorrect error message when azcopy cannot find the installation location</span></span>

## <a name="april-30-2020"></a><span data-ttu-id="0bba9-469">30. April 2020</span><span class="sxs-lookup"><span data-stu-id="0bba9-469">April 30, 2020</span></span>

<span data-ttu-id="0bba9-470">Version 2.5.1</span><span class="sxs-lookup"><span data-stu-id="0bba9-470">Version 2.5.1</span></span>

### <a name="acr"></a><span data-ttu-id="0bba9-471">ACR</span><span class="sxs-lookup"><span data-stu-id="0bba9-471">ACR</span></span>

* <span data-ttu-id="0bba9-472">`az acr check-health`: „DOCKER_PULL_ERROR“ unter Windows behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-472">`az acr check-health`: Fix "DOCKER_PULL_ERROR" on Windows</span></span>

### <a name="compute"></a><span data-ttu-id="0bba9-473">Compute</span><span class="sxs-lookup"><span data-stu-id="0bba9-473">Compute</span></span>

* <span data-ttu-id="0bba9-474">`az vm list-ip-addresses`: Fehlerbehandlung</span><span class="sxs-lookup"><span data-stu-id="0bba9-474">`az vm list-ip-addresses`: Error handling</span></span>
* <span data-ttu-id="0bba9-475">Fehler behoben, der bei der VM-Erstellung auftrat, wenn „endpoint_vm_image_alias_doc“ im Cloudprofil nicht festgelegt war</span><span class="sxs-lookup"><span data-stu-id="0bba9-475">Fix a bug of vm create if endpoint_vm_image_alias_doc is not set in cloud profile</span></span>
* <span data-ttu-id="0bba9-476">`az vmss create`: „--os-disk-size-gb“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-476">`az vmss create`: Add --os-disk-size-gb</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="0bba9-477">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="0bba9-477">Cosmos DB</span></span>

* <span data-ttu-id="0bba9-478">`az cosmosdb create/update`: Unterstützung für „--enable-public-network“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-478">`az cosmosdb create/update`: add --enable-public-network support</span></span>

### <a name="extension"></a><span data-ttu-id="0bba9-479">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="0bba9-479">Extension</span></span>

* <span data-ttu-id="0bba9-480">Laden der falschen Metadaten für die Radtyperweiterung korrigiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-480">Fix loading wrong metadata for wheel type extension</span></span>

### <a name="packaging"></a><span data-ttu-id="0bba9-481">Verpackung</span><span class="sxs-lookup"><span data-stu-id="0bba9-481">Packaging</span></span>

* <span data-ttu-id="0bba9-482">Az-Skript für Git Bash/Cygwin unter Windows hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-482">Add az script for Git Bash/Cygwin on Windows</span></span>

### <a name="sql"></a><span data-ttu-id="0bba9-483">SQL</span><span class="sxs-lookup"><span data-stu-id="0bba9-483">SQL</span></span>

* <span data-ttu-id="0bba9-484">`az sql instance-pool`: Befehlsgruppe für Instanzpools hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-484">`az sql instance-pool`: Add instance pools command group</span></span>

### <a name="storage"></a><span data-ttu-id="0bba9-485">Storage</span><span class="sxs-lookup"><span data-stu-id="0bba9-485">Storage</span></span>

* <span data-ttu-id="0bba9-486">Paket „azure-multiapi-storage“ auf 0.3.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-486">Upgrade package azure-multiapi-storage to 0.3.0</span></span>
* <span data-ttu-id="0bba9-487">Unterstützung von GZRS für Speicherkontoerstellung und -aktualisierung</span><span class="sxs-lookup"><span data-stu-id="0bba9-487">Support GZRS for storage account creation and update</span></span>
* <span data-ttu-id="0bba9-488">`az storage account failover`: Unterstützung für das Failover von GRS/GZRS-Speicherkonten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-488">`az storage account failover`: Add support for grs/gzrs storage account failover</span></span>
* <span data-ttu-id="0bba9-489">`az storage blob upload`: Parameter „--encryption-scope“ hinzugefügt, um die Angabe von Informationen zum Verschlüsselungsbereich zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="0bba9-489">`az storage blob upload`: Add --encryption-scope parameter to support specifying encryption scope information</span></span>

## <a name="april-28-2020"></a><span data-ttu-id="0bba9-490">28. April 2020</span><span class="sxs-lookup"><span data-stu-id="0bba9-490">April 28, 2020</span></span>

<span data-ttu-id="0bba9-491">Version 2.5.0</span><span class="sxs-lookup"><span data-stu-id="0bba9-491">Version 2.5.0</span></span>

### <a name="acs"></a><span data-ttu-id="0bba9-492">ACS</span><span class="sxs-lookup"><span data-stu-id="0bba9-492">ACS</span></span>

* <span data-ttu-id="0bba9-493">[BREAKING CHANGE] az openshift create: Parameter „--vnet-peer“ entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-493">[BREAKING CHANGE] az openshift create: remove --vnet-peer parameter.</span></span>
* <span data-ttu-id="0bba9-494">`az openshift create`: Flags zur Unterstützung des privaten Clusters hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-494">`az openshift create`: add flags to support private cluster.</span></span>
* <span data-ttu-id="0bba9-495">`az openshift`: Upgrade auf API-Version `2019-10-27-preview`</span><span class="sxs-lookup"><span data-stu-id="0bba9-495">`az openshift`: upgrade to `2019-10-27-preview` API version.</span></span>
* <span data-ttu-id="0bba9-496">`az openshift`: Befehl `update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-496">`az openshift`: add `update` command.</span></span>

### <a name="aks"></a><span data-ttu-id="0bba9-497">AKS</span><span class="sxs-lookup"><span data-stu-id="0bba9-497">AKS</span></span>

* <span data-ttu-id="0bba9-498">`az aks create`: Unterstützung für Windows hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-498">`az aks create`: Add support for Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="0bba9-499">AppService</span><span class="sxs-lookup"><span data-stu-id="0bba9-499">AppService</span></span>

* <span data-ttu-id="0bba9-500">`az webapp deployment source config-zip`: Energiesparmodus nach „request.get()“ entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-500">`az webapp deployment source config-zip`: remove sleep after request.get()</span></span>

### <a name="arm"></a><span data-ttu-id="0bba9-501">ARM</span><span class="sxs-lookup"><span data-stu-id="0bba9-501">ARM</span></span>

* <span data-ttu-id="0bba9-502">Was-wäre-wenn-Befehle für Vorlagenbereitstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-502">Add template deployment What-If commands</span></span>

### <a name="aro"></a><span data-ttu-id="0bba9-503">ARO</span><span class="sxs-lookup"><span data-stu-id="0bba9-503">ARO</span></span>

* <span data-ttu-id="0bba9-504">`az aro`: Tabellenausgabe korrigiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-504">`az aro`: Fix table output</span></span>

### <a name="ci"></a><span data-ttu-id="0bba9-505">CI</span><span class="sxs-lookup"><span data-stu-id="0bba9-505">CI</span></span>

* <span data-ttu-id="0bba9-506">pytest integriert und nose für Automatisierungstest als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="0bba9-506">Onboard pytest and deprecate nose for Automation Test</span></span>

### <a name="compute"></a><span data-ttu-id="0bba9-507">Compute</span><span class="sxs-lookup"><span data-stu-id="0bba9-507">Compute</span></span>

* <span data-ttu-id="0bba9-508">`az vmss disk detach`: Datenträgerfehler „NoneType“ behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-508">`az vmss disk detach`: fix data disk NoneType issue</span></span>
* <span data-ttu-id="0bba9-509">`az vm availability-set list`: Unterstützung zum Anzeigen der VM-Liste</span><span class="sxs-lookup"><span data-stu-id="0bba9-509">`az vm availability-set list`: Support showing VM list</span></span>
* <span data-ttu-id="0bba9-510">`az vm list-skus`: Anzeigeproblem des Tabellenformats behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-510">`az vm list-skus`: Fix display problem of table format</span></span>

### <a name="keyvault"></a><span data-ttu-id="0bba9-511">KeyVault</span><span class="sxs-lookup"><span data-stu-id="0bba9-511">KeyVault</span></span>

* <span data-ttu-id="0bba9-512">Neuer Parameter `--enable-rbac-authorization` bei Erstellung oder Aktualisierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-512">Add new parameter `--enable-rbac-authorization` during creating or updating</span></span>

### <a name="monitor"></a><span data-ttu-id="0bba9-513">Überwachen</span><span class="sxs-lookup"><span data-stu-id="0bba9-513">Monitor</span></span>

* <span data-ttu-id="0bba9-514">Unterstützung der CMK-Features für LA-Cluster</span><span class="sxs-lookup"><span data-stu-id="0bba9-514">Support LA cluster CMK features</span></span>
* <span data-ttu-id="0bba9-515">`az monitor log-analytics workspace linked-storage`: Unterstützung für BYOS-Features</span><span class="sxs-lookup"><span data-stu-id="0bba9-515">`az monitor log-analytics workspace linked-storage`: supports BYOS features</span></span>

### <a name="network"></a><span data-ttu-id="0bba9-516">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0bba9-516">Network</span></span>

* <span data-ttu-id="0bba9-517">`az network security-partner`: Unterstützung des Sicherheitspartneranbieters</span><span class="sxs-lookup"><span data-stu-id="0bba9-517">`az network security-partner`: support security partner provider</span></span>

### <a name="privatedns"></a><span data-ttu-id="0bba9-518">PrivateDNS</span><span class="sxs-lookup"><span data-stu-id="0bba9-518">Privatedns</span></span>

* <span data-ttu-id="0bba9-519">Funktion in privater DNS-Zone zum Importieren der Exportzonendatei hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-519">Add feature in private DNS zone to import export zone file</span></span>

## <a name="april-21-2020"></a><span data-ttu-id="0bba9-520">21. April 2020</span><span class="sxs-lookup"><span data-stu-id="0bba9-520">April 21, 2020</span></span>

<span data-ttu-id="0bba9-521">Version 2.4.0</span><span class="sxs-lookup"><span data-stu-id="0bba9-521">Version 2.4.0</span></span>

### <a name="acr"></a><span data-ttu-id="0bba9-522">ACR</span><span class="sxs-lookup"><span data-stu-id="0bba9-522">ACR</span></span>

* <span data-ttu-id="0bba9-523">`az acr run --cmd`: Deaktivieren der Arbeitsverzeichnisaußerkraftsetzung</span><span class="sxs-lookup"><span data-stu-id="0bba9-523">`az acr run --cmd`: disable working directory override</span></span>
* <span data-ttu-id="0bba9-524">Unterstützung dedizierter Datenendpunkte</span><span class="sxs-lookup"><span data-stu-id="0bba9-524">Support dedicated data endpoint</span></span>

### <a name="aks"></a><span data-ttu-id="0bba9-525">AKS</span><span class="sxs-lookup"><span data-stu-id="0bba9-525">AKS</span></span>

* <span data-ttu-id="0bba9-526">`az aks list -o table` sollte „privateFqdn“ als FQDN für private Cluster anzeigen</span><span class="sxs-lookup"><span data-stu-id="0bba9-526">`az aks list -o table` should show privateFqdn as fqdn for private clusters</span></span>
* <span data-ttu-id="0bba9-527">„--uptime-sla“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-527">Add --uptime-sla</span></span>
* <span data-ttu-id="0bba9-528">containerservice-Paket aktualisiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-528">Update containerservice package</span></span>
* <span data-ttu-id="0bba9-529">Unterstützung für öffentliche IP-Adressen für Knoten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-529">Add node public IP support</span></span>
* <span data-ttu-id="0bba9-530">Tippfehler im help-Befehl korrigiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-530">Fix typo in the help command</span></span>

### <a name="appconfig"></a><span data-ttu-id="0bba9-531">AppConfig</span><span class="sxs-lookup"><span data-stu-id="0bba9-531">AppConfig</span></span>

* <span data-ttu-id="0bba9-532">Schlüsseltresorverweis für die Befehle „kv list“ und „kv export“ aufgelöst</span><span class="sxs-lookup"><span data-stu-id="0bba9-532">Resolve key vault reference for kv list and export commands</span></span>
* <span data-ttu-id="0bba9-533">Fehlerbehebung für die Werte für das Auflisten von Schlüsseln</span><span class="sxs-lookup"><span data-stu-id="0bba9-533">Bug fix for list key values</span></span>

### <a name="appservice"></a><span data-ttu-id="0bba9-534">AppService</span><span class="sxs-lookup"><span data-stu-id="0bba9-534">AppService</span></span>

* <span data-ttu-id="0bba9-535">`az functionapp create`: Vorgehensweise zum Festlegen von „linuxFxVersion“ für Linux-Funktions-Apps (.NET) geändert.</span><span class="sxs-lookup"><span data-stu-id="0bba9-535">`az functionapp create`: Changed the way linuxFxVersion was being set for dotnet linux function apps.</span></span> <span data-ttu-id="0bba9-536">Dadurch sollte der Fehler behoben sein, der die Erstellung von Linux-Verbrauchs-Apps (.NET) verhindert hat.</span><span class="sxs-lookup"><span data-stu-id="0bba9-536">This should fix a bug that was preventing dotnet linux consumption apps from being created</span></span>
* <span data-ttu-id="0bba9-537">[BREAKING CHANGE] `az webapp create`: Korrektur vorgenommen, um vorhandene App-Einstellungen (AppSettings) für „az webapp create“ beizubehalten</span><span class="sxs-lookup"><span data-stu-id="0bba9-537">[BREAKING CHANGE] `az webapp create`: fix to keep existing AppSettings with az webapp create</span></span>
* <span data-ttu-id="0bba9-538">[BREAKING CHANGE] `az webapp up`: Korrektur vorgenommen, um bei Verwendung des Flags „-g“ eine RG für den Befehl „az webapp up“ zu erstellen</span><span class="sxs-lookup"><span data-stu-id="0bba9-538">[BREAKING CHANGE] `az webapp up`: fix to create RG for az webapp up command when using -g flag</span></span>
* <span data-ttu-id="0bba9-539">[BREAKING CHANGE] `az webapp config`: Korrektur vorgenommen, um Werte für Nicht-JSON-Ausgaben mit „az webapp config connection-string list“ anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="0bba9-539">[BREAKING CHANGE] `az webapp config`: fix to show values for non-JSON output with az webapp config connection-string list</span></span>

### <a name="arm"></a><span data-ttu-id="0bba9-540">ARM</span><span class="sxs-lookup"><span data-stu-id="0bba9-540">ARM</span></span>

* <span data-ttu-id="0bba9-541">`az deployment create/validate`: Parameter `--no-prompt` hinzugefügt, um das Überspringen der Eingabeaufforderung für fehlende Parameter für die ARM-Vorlage zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="0bba9-541">`az deployment create/validate`: Add parameter `--no-prompt` to support skipping the prompt of missing parameters for ARM template</span></span>
* <span data-ttu-id="0bba9-542">`az deployment group/mg/sub/tenant validate`: Unterstützung von Kommentaren in der Bereitstellungsparameterdatei</span><span class="sxs-lookup"><span data-stu-id="0bba9-542">`az deployment group/mg/sub/tenant validate`: Support comments in deployment parameter file</span></span>
* <span data-ttu-id="0bba9-543">`az deployment`: `is_preview` für Parameter `--handle-extended-json-format` entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-543">`az deployment`: Remove `is_preview` for parameter `--handle-extended-json-format`</span></span>
* <span data-ttu-id="0bba9-544">`az deployment group/mg/sub/tenant cancel`: Unterstützung für den Abbruch der Bereitstellung für ARM-Vorlagen</span><span class="sxs-lookup"><span data-stu-id="0bba9-544">`az deployment group/mg/sub/tenant cancel`: Support cancel deployment for ARM template</span></span>
* <span data-ttu-id="0bba9-545">`az deployment group/mg/sub/tenant validate`: Fehlermeldung bei einem Fehler der Bereitstellungsüberprüfung verbessert</span><span class="sxs-lookup"><span data-stu-id="0bba9-545">`az deployment group/mg/sub/tenant validate`: Improve the error message when deployment verification fails</span></span>
* <span data-ttu-id="0bba9-546">`az deployment-scripts`: Neue Befehle für DeploymentScripts hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-546">`az deployment-scripts`: Add new commands for DeploymentScripts</span></span>
* <span data-ttu-id="0bba9-547">`az resource tag`: Parameter `--is-incremental` hinzugefügt, um das inkrementelle Hinzufügen von Tags zur Ressource zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="0bba9-547">`az resource tag`: Add parameter `--is-incremental` to support adding tags to resource incrementally</span></span>

### <a name="aro"></a><span data-ttu-id="0bba9-548">ARO</span><span class="sxs-lookup"><span data-stu-id="0bba9-548">ARO</span></span>

* <span data-ttu-id="0bba9-549">`az aro`:  ARO-Befehlsmodul von Azure RedHat OpenShift V4 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-549">`az aro`:  Add Azure RedHat OpenShift V4 aro command module</span></span>

### <a name="batch"></a><span data-ttu-id="0bba9-550">Batch</span><span class="sxs-lookup"><span data-stu-id="0bba9-550">Batch</span></span>

* <span data-ttu-id="0bba9-551">Batch-API aktualisiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-551">Update Batch API</span></span>

### <a name="compute"></a><span data-ttu-id="0bba9-552">Compute</span><span class="sxs-lookup"><span data-stu-id="0bba9-552">Compute</span></span>

* <span data-ttu-id="0bba9-553">`az sig image-version create`: Speicherkontotyp „Premium_LRS“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-553">`az sig image-version create`: Add storage account type Premium_LRS</span></span>
* <span data-ttu-id="0bba9-554">`az vmss update`: Problem behoben, das beim Aktualisieren der Beendigungsbenachrichtigung auftrat</span><span class="sxs-lookup"><span data-stu-id="0bba9-554">`az vmss update`: Fix terminate notification update issue</span></span>
* <span data-ttu-id="0bba9-555">`az vm/vmss create`: Unterstützung für spezialisierte Imageversion hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-555">`az vm/vmss create`: Add support for specialized image version</span></span>
* <span data-ttu-id="0bba9-556">SIG-API-Version 2019-12-01</span><span class="sxs-lookup"><span data-stu-id="0bba9-556">SIG API Version 2019-12-01</span></span>
* <span data-ttu-id="0bba9-557">`az sig image-version create`: „--target-region-encryption“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-557">`az sig image-version create`: Add --target-region-encryption</span></span>
* <span data-ttu-id="0bba9-558">Fehler bei Serientestausführung behoben, der auf die Duplizierung des Schlüsseltresornamens im globalen In-Memory-Cache zurückzuführen war.</span><span class="sxs-lookup"><span data-stu-id="0bba9-558">Fix tests fail when running in serial due to keyvault name is duplicated in global in-momery cache</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="0bba9-559">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="0bba9-559">CosmosDB</span></span>

* <span data-ttu-id="0bba9-560">Unterstützung für `az cosmosdb private-link-resource/private-endpoint-connection`</span><span class="sxs-lookup"><span data-stu-id="0bba9-560">Support `az cosmosdb private-link-resource/private-endpoint-connection`</span></span>

### <a name="iot-central"></a><span data-ttu-id="0bba9-561">IoT Central</span><span class="sxs-lookup"><span data-stu-id="0bba9-561">IoT Central</span></span>

* <span data-ttu-id="0bba9-562">`az iotcentral` als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="0bba9-562">Deprecate `az iotcentral`</span></span>
* <span data-ttu-id="0bba9-563">Befehlsmodul `az iot central` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-563">Add `az iot central` command module</span></span>

### <a name="monitor"></a><span data-ttu-id="0bba9-564">Überwachen</span><span class="sxs-lookup"><span data-stu-id="0bba9-564">Monitor</span></span>

* <span data-ttu-id="0bba9-565">Unterstützung eines Private Link-Szenarios für die Überwachung</span><span class="sxs-lookup"><span data-stu-id="0bba9-565">Support private link scenario for monitor</span></span>
* <span data-ttu-id="0bba9-566">Falsche Simulationsmethode in „test_monitor_general_operations.py“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-566">Fix wrong mocking way in test_monitor_general_operations.py</span></span>

### <a name="network"></a><span data-ttu-id="0bba9-567">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0bba9-567">Network</span></span>

* <span data-ttu-id="0bba9-568">SKU für den Befehl zur Aktualisierung der öffentlichen IP-Adresse als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="0bba9-568">Deprecate sku for public ip update command</span></span>
* <span data-ttu-id="0bba9-569">`az network private-endpoint`: Unterstützung für private DNS-Zonengruppe</span><span class="sxs-lookup"><span data-stu-id="0bba9-569">`az network private-endpoint`: Support private dns zone group</span></span>
* <span data-ttu-id="0bba9-570">Feature für lokalen Kontext für VNET-/Subnetzparameter aktiviert</span><span class="sxs-lookup"><span data-stu-id="0bba9-570">Enable local context feature for vnet/subnet parameter</span></span>
* <span data-ttu-id="0bba9-571">Falsches Verwendungsbeispiel in „test_nw_flow_log_delete“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-571">Fix wrong usage example in test_nw_flow_log_delete</span></span>

### <a name="packaging"></a><span data-ttu-id="0bba9-572">Verpackung</span><span class="sxs-lookup"><span data-stu-id="0bba9-572">Packaging</span></span>

* <span data-ttu-id="0bba9-573">Unterstützung für Ubuntu-/Disco-Paket eingestellt</span><span class="sxs-lookup"><span data-stu-id="0bba9-573">Drop support for Ubuntu/Disco package</span></span>

### <a name="rbac"></a><span data-ttu-id="0bba9-574">RBAC</span><span class="sxs-lookup"><span data-stu-id="0bba9-574">RBAC</span></span>

* <span data-ttu-id="0bba9-575">`az ad app create/update`: Unterstützung von „--optional-claims“ als Parameter</span><span class="sxs-lookup"><span data-stu-id="0bba9-575">`az ad app create/update`: support --optional-claims as a parameter</span></span>

### <a name="rdbms"></a><span data-ttu-id="0bba9-576">RDBMS</span><span class="sxs-lookup"><span data-stu-id="0bba9-576">RDBMS</span></span>

* <span data-ttu-id="0bba9-577">Azure Active Directory-Administratorbefehle für PostgreSQL und MySQL hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-577">Add Azure active directory administrator commands for PostgreSQL and MySQL</span></span>

### <a name="service-fabric"></a><span data-ttu-id="0bba9-578">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="0bba9-578">Service Fabric</span></span>

* <span data-ttu-id="0bba9-579">Fehlerbehebung Nr. 12891: `az sf application update --application-parameters` entfernt alte Parameter, die nicht in der Anforderung enthalten sind.</span><span class="sxs-lookup"><span data-stu-id="0bba9-579">Fix #12891: `az sf application update --application-parameters` removes old parameters that are not in the request</span></span>
* <span data-ttu-id="0bba9-580">Fehlerbehebung Nr. 12470: az sf create cluster: Fehler im Zusammenhang mit der Dauerhaftigkeit und Zuverlässigkeit von Updates sowie im Zusammenhang mit der codebasierten Suche der VMSS unter Angabe eines bestimmten Knotentypnamens behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-580">Fix #12470 az sf create cluster, fix bugs in update durability and reliability and find vmss correctly through the code given a node type name</span></span>

### <a name="sql"></a><span data-ttu-id="0bba9-581">SQL</span><span class="sxs-lookup"><span data-stu-id="0bba9-581">SQL</span></span>

* <span data-ttu-id="0bba9-582">`az sql mi op list`, `az sql mi op get`, `az sql mi op cancel` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-582">Add `az sql mi op list`, `az sql mi op get`, `az sql mi op cancel`</span></span>
* <span data-ttu-id="0bba9-583">`az sql midb`: Aktualisieren/Anzeigen der Richtlinie zur langfristigen Aufbewahrung, Anzeigen/Löschen von Sicherungen zur langfristigen Aufbewahrung, Wiederherstellen von Sicherungen zur langfristigen Aufbewahrung</span><span class="sxs-lookup"><span data-stu-id="0bba9-583">`az sql midb`: update/show long term retention policy,  show/delete long term retention backups, restore long term retention backup</span></span>

### <a name="storage"></a><span data-ttu-id="0bba9-584">Storage</span><span class="sxs-lookup"><span data-stu-id="0bba9-584">Storage</span></span>

* <span data-ttu-id="0bba9-585">„azure-mgmt-storage“ auf 9.0.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-585">Upgrade azure-mgmt-storage to 9.0.0</span></span>
* <span data-ttu-id="0bba9-586">`az storage logging off`: Unterstützung für das Ausschalten der Protokollierung für ein Speicherkonto</span><span class="sxs-lookup"><span data-stu-id="0bba9-586">`az storage logging off`: Support turning off logging for a storage account</span></span>
* <span data-ttu-id="0bba9-587">`az storage account update`: Automatische Rotation von Schlüsseln für CMK aktiviert</span><span class="sxs-lookup"><span data-stu-id="0bba9-587">`az storage account update`: Enable key auto-rotated for CMK</span></span>
* <span data-ttu-id="0bba9-588">`az storage account encryption-scope create/update/list/show`: Unterstützung zum Anpassen des Verschlüsselungsbereichs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-588">`az storage account encryption-scope create/update/list/show`: Add support to customize encryption scope</span></span>
* <span data-ttu-id="0bba9-589">`az storage container create`: „--default-encryption-scope“ und „--deny-encryption-scope-override“ hinzugefügt, um den Verschlüsselungsbereich für die Containerebene festzulegen</span><span class="sxs-lookup"><span data-stu-id="0bba9-589">`az storage container create`: Add --default-encryption-scope and --deny-encryption-scope-override to set encryption scope for container level</span></span>

### <a name="survey"></a><span data-ttu-id="0bba9-590">Umfrage</span><span class="sxs-lookup"><span data-stu-id="0bba9-590">Survey</span></span>

* <span data-ttu-id="0bba9-591">Switch zum Deaktivieren des Umfragelinks hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-591">Add switch to turn off survey link</span></span>

## <a name="april-01-2020"></a><span data-ttu-id="0bba9-592">01. April 2020</span><span class="sxs-lookup"><span data-stu-id="0bba9-592">April 01, 2020</span></span>

<span data-ttu-id="0bba9-593">Version 2.3.1</span><span class="sxs-lookup"><span data-stu-id="0bba9-593">Version 2.3.1</span></span>

### <a name="acr"></a><span data-ttu-id="0bba9-594">ACR</span><span class="sxs-lookup"><span data-stu-id="0bba9-594">ACR</span></span>

* <span data-ttu-id="0bba9-595">Falsche Version von „azure-mgmt-containerregistry“ für Linux korrigiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-595">Fix wrong version of azure-mgmt-containerregistry for Linux</span></span>

### <a name="profile"></a><span data-ttu-id="0bba9-596">Profil</span><span class="sxs-lookup"><span data-stu-id="0bba9-596">Profile</span></span>

* <span data-ttu-id="0bba9-597">az login: Anmeldefehler behoben, der auftrat, wenn nicht das Cloudprofil `latest` verwendet wurde</span><span class="sxs-lookup"><span data-stu-id="0bba9-597">az login: Fix login failure with cloud profiles other than `latest`</span></span>

## <a name="march-31-2020"></a><span data-ttu-id="0bba9-598">31. März 2020</span><span class="sxs-lookup"><span data-stu-id="0bba9-598">March 31, 2020</span></span>

<span data-ttu-id="0bba9-599">Version 2.3.0</span><span class="sxs-lookup"><span data-stu-id="0bba9-599">Version 2.3.0</span></span>

### <a name="acr"></a><span data-ttu-id="0bba9-600">ACR</span><span class="sxs-lookup"><span data-stu-id="0bba9-600">ACR</span></span>

* <span data-ttu-id="0bba9-601">„az acr task update“: NULL-Zeiger-Ausnahme</span><span class="sxs-lookup"><span data-stu-id="0bba9-601">'az acr task update': null pointer exception</span></span>
* <span data-ttu-id="0bba9-602">`az acr import`: Hilfe und Fehlermeldung geändert, um die Verwendung von „--source“ und „--registry“ zu verdeutlichen</span><span class="sxs-lookup"><span data-stu-id="0bba9-602">`az acr import`: Modify help and error message to clarify the usage of --source and --registry</span></span>
* <span data-ttu-id="0bba9-603">Überprüfung für das Argument „registry_name“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-603">Add a validator for argument 'registry_name'</span></span>
* <span data-ttu-id="0bba9-604">`az acr login`: Vorschauflag für „--expose-token“ entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-604">`az acr login`:Remove the preview flag on '--expose-token'</span></span>
* <span data-ttu-id="0bba9-605">[BREAKING CHANGE] Branch-Parameter „az acr task create/update“ entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-605">[BREAKING CHANGE] 'az acr task create/update' Branch parameter is removed</span></span>
* <span data-ttu-id="0bba9-606">„az acr task update“: Kunde kann nun Kontext, Git-Token und/oder Trigger einzeln aktualisieren</span><span class="sxs-lookup"><span data-stu-id="0bba9-606">'az acr task update' Customer now can update context, git-token, and or triggers individually</span></span>
* <span data-ttu-id="0bba9-607">„az acr agentpool“: Neues Feature</span><span class="sxs-lookup"><span data-stu-id="0bba9-607">'az acr agentpool': new feature</span></span>

### <a name="aks"></a><span data-ttu-id="0bba9-608">AKS</span><span class="sxs-lookup"><span data-stu-id="0bba9-608">AKS</span></span>

* <span data-ttu-id="0bba9-609">„apiServerAccessProfile“ bei der Aktualisierung von „--api-server-authorized-ip-ranges“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-609">Fix apiServerAccessProfile when updating --api-server-authorized-ip-ranges</span></span>
* <span data-ttu-id="0bba9-610">aks update: Überschreibung ausgehender IP-Adressen mit Eingabewerten bei der Aktualisierung</span><span class="sxs-lookup"><span data-stu-id="0bba9-610">aks update: Override outbound IPs with input values when update</span></span>
* <span data-ttu-id="0bba9-611">Keine SPN-Erstellung für MSI-Cluster sowie Unterstützung der Anfügung von ACR an MSI-Cluster</span><span class="sxs-lookup"><span data-stu-id="0bba9-611">Do not create SPN for MSI clusters and support attach acr to MSI clusters</span></span>

### <a name="ams"></a><span data-ttu-id="0bba9-612">AMS</span><span class="sxs-lookup"><span data-stu-id="0bba9-612">AMS</span></span>

* <span data-ttu-id="0bba9-613">Fix 12469: Hinzufügen von „content-key-policy“ für Fairplay aufgrund von Problemen mit dem Parameter „ask“ nicht erfolgreich</span><span class="sxs-lookup"><span data-stu-id="0bba9-613">Fix #12469: adding Fairplay content-key-policy fails due to problems with 'ask' parameter</span></span>

### <a name="appconfig"></a><span data-ttu-id="0bba9-614">AppConfig</span><span class="sxs-lookup"><span data-stu-id="0bba9-614">AppConfig</span></span>

* <span data-ttu-id="0bba9-615">„--skip-keyvault“ für „kv export“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-615">Add --skip-keyvault for kv export</span></span>

### <a name="appservice"></a><span data-ttu-id="0bba9-616">AppService</span><span class="sxs-lookup"><span data-stu-id="0bba9-616">AppService</span></span>

* <span data-ttu-id="0bba9-617">Fix 12509: Tag für „az webapp up“ standardmäßig entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-617">Fix #12509: Remove the tag to az webapp up by default</span></span>
* <span data-ttu-id="0bba9-618">az functionapp create: Hilfemenü für „--runtime-version“ aktualisiert und Warnung hinzugefügt, wenn der Benutzer „--runtime-version“ für .NET angibt</span><span class="sxs-lookup"><span data-stu-id="0bba9-618">az functionapp create: Updated --runtime-version help menu and added warning when user specifies --runtime-version for dotnet</span></span>
* <span data-ttu-id="0bba9-619">az functionapp create: Methode zum Festlegen von „javaVersion“ für Windows-Funktions-Apps aktualisiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-619">az functionapp create: Updated the way javaVersion was being set for Windows function apps</span></span>

### <a name="arm"></a><span data-ttu-id="0bba9-620">ARM</span><span class="sxs-lookup"><span data-stu-id="0bba9-620">ARM</span></span>

* <span data-ttu-id="0bba9-621">az deployment create/validate: Standardmäßige Verwendung von „--handle-extended-json-format“</span><span class="sxs-lookup"><span data-stu-id="0bba9-621">az deployment create/validate: Use --handle-extended-json-format by default</span></span>
* <span data-ttu-id="0bba9-622">az lock create: Beispiele für die Erstellung einer Unterressource in der Hilfedokumentation hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-622">az lock create: Add examples of creating subresource in the help documentation</span></span>
* <span data-ttu-id="0bba9-623">az deployment {group/mg/sub/tenant} list: Unterstützung der provisioningState-Filterung</span><span class="sxs-lookup"><span data-stu-id="0bba9-623">az deployment {group/mg/sub/tenant} list: Support provisioningState filtering</span></span>
* <span data-ttu-id="0bba9-624">az deployment: Analysefehler für Kommentar unter letztem Argument behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-624">az deployment: Fix the parse bug for comment under the last argument</span></span>

### <a name="backup"></a><span data-ttu-id="0bba9-625">Backup</span><span class="sxs-lookup"><span data-stu-id="0bba9-625">Backup</span></span>

* <span data-ttu-id="0bba9-626">Mehrere Dateiwiederherstellungsfunktionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-626">Added multiple files restore capabilities</span></span>
* <span data-ttu-id="0bba9-627">Unterstützung der ausschließlichen Sicherung von Betriebssystemdatenträgern hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-627">Added support for Backing up OS Disks only</span></span>
* <span data-ttu-id="0bba9-628">Parameter „restore-as-unmanaged-disk“ für die Angabe einer nicht verwalteten Wiederherstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-628">Added restore-as-unmanaged-disk parameter to specify unmanaged restore</span></span>

### <a name="compute"></a><span data-ttu-id="0bba9-629">Compute</span><span class="sxs-lookup"><span data-stu-id="0bba9-629">Compute</span></span>

* <span data-ttu-id="0bba9-630">az vm create: Option „NONE“ von „--nsg-rule“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-630">az vm create: Add NONE option of --nsg-rule</span></span>
* <span data-ttu-id="0bba9-631">az vmss create/update: Vorschautag für automatische VMSS-Reparaturen entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-631">az vmss create/update: remove vmss automatic repairs preview tag</span></span>
* <span data-ttu-id="0bba9-632">az vm update: Unterstützung von „--workspace“</span><span class="sxs-lookup"><span data-stu-id="0bba9-632">az vm update: Support --workspace</span></span>
* <span data-ttu-id="0bba9-633">Fehler im VirtualMachineScaleSetExtension-Initialisierungscode behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-633">Fix a bug in VirtualMachineScaleSetExtension initialization code</span></span>
* <span data-ttu-id="0bba9-634">Upgrade der VMAccessAgent-Version auf 2.4 durchgeführt</span><span class="sxs-lookup"><span data-stu-id="0bba9-634">Upgrade VMAccessAgent version to 2.4</span></span>
* <span data-ttu-id="0bba9-635">az vmss set-orchestration-service-state: Unterstützung zum Festlegen des Orchestrierungdienstzustands für VMSS</span><span class="sxs-lookup"><span data-stu-id="0bba9-635">az vmss set-orchestration-service-state: support vmss set orchestration service state</span></span>
* <span data-ttu-id="0bba9-636">Upgrade der Datenträger-API-Version auf 2019-11-01 durchgeführt</span><span class="sxs-lookup"><span data-stu-id="0bba9-636">Upgrade disk API version to 2019-11-01</span></span>
* <span data-ttu-id="0bba9-637">az disk create: add --disk-iops-read-only, --disk-mbps-read-only, --max-shares, --image-reference, --image-reference-lun, --gallery-image-reference, --gallery-image-reference-lun</span><span class="sxs-lookup"><span data-stu-id="0bba9-637">az disk create: add --disk-iops-read-only, --disk-mbps-read-only, --max-shares, --image-reference, --image-reference-lun, --gallery-image-reference, --gallery-image-reference-lun</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="0bba9-638">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="0bba9-638">Cosmos DB</span></span>

* <span data-ttu-id="0bba9-639">Fehlende Option „--type“ für Veraltungsumleitungen korrigiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-639">Fix missing --type option for deprecation redirections</span></span>

### <a name="docker"></a><span data-ttu-id="0bba9-640">Docker</span><span class="sxs-lookup"><span data-stu-id="0bba9-640">Docker</span></span>

* <span data-ttu-id="0bba9-641">Update auf Alpine 3.11 und Python 3.6.10 durchgeführt</span><span class="sxs-lookup"><span data-stu-id="0bba9-641">Update to Alpine 3.11 and Python 3.6.10</span></span>

### <a name="extension"></a><span data-ttu-id="0bba9-642">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="0bba9-642">Extension</span></span>

* <span data-ttu-id="0bba9-643">Laden von Erweiterungen im Systempfad mittels Paketen ermöglicht</span><span class="sxs-lookup"><span data-stu-id="0bba9-643">Allow to load extensions in the system path via packages</span></span>

### <a name="hdinsight"></a><span data-ttu-id="0bba9-644">HDInsight</span><span class="sxs-lookup"><span data-stu-id="0bba9-644">HDInsight</span></span>

* <span data-ttu-id="0bba9-645">(az hdinsight create:) Unterstützung der Angabe der unterstützten TLS-Mindestversion durch Kunden unter Verwendung des Parameters `--minimal-tls-version`.</span><span class="sxs-lookup"><span data-stu-id="0bba9-645">(az hdinsight create:) Support customers specify minimal supported tls version by using parameter `--minimal-tls-version`.</span></span> <span data-ttu-id="0bba9-646">Zulässiger Wert: 1.0,1.1,1.2</span><span class="sxs-lookup"><span data-stu-id="0bba9-646">The allowed value is 1.0,1.1,1.2</span></span>

### <a name="iot"></a><span data-ttu-id="0bba9-647">IoT</span><span class="sxs-lookup"><span data-stu-id="0bba9-647">IoT</span></span>

* <span data-ttu-id="0bba9-648">Codebesitzer hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-648">Add codeowner</span></span>
* <span data-ttu-id="0bba9-649">az iot hub create: Standard-SKU von F1 in S1 geändert</span><span class="sxs-lookup"><span data-stu-id="0bba9-649">az iot hub create : Change default sku to S1 from F1</span></span>
* <span data-ttu-id="0bba9-650">iot hub: Unterstützung von „IotHub“ im Profil „2019-03-01-hybrid“</span><span class="sxs-lookup"><span data-stu-id="0bba9-650">iot hub: Support IotHub in the profile of 2019-03-01-hybrid</span></span>

### <a name="iotcentral"></a><span data-ttu-id="0bba9-651">IoTCentral</span><span class="sxs-lookup"><span data-stu-id="0bba9-651">IoTCentral</span></span>

* <span data-ttu-id="0bba9-652">Fehlerdetails sowie Standardanwendungsvorlage und Aufforderungsmeldung aktualisiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-652">Update error details, update default application template and prompt message</span></span>

### <a name="keyvault"></a><span data-ttu-id="0bba9-653">KeyVault</span><span class="sxs-lookup"><span data-stu-id="0bba9-653">KeyVault</span></span>

* <span data-ttu-id="0bba9-654">Unterstützung von Zertifikatsicherung/-wiederherstellung</span><span class="sxs-lookup"><span data-stu-id="0bba9-654">Support certificate backup/restore</span></span>
* <span data-ttu-id="0bba9-655">keyvault create/update: Unterstützung von „--retention-days“</span><span class="sxs-lookup"><span data-stu-id="0bba9-655">keyvault create/update: Support --retention-days</span></span>
* <span data-ttu-id="0bba9-656">Keine Anzeige von verwalteten Schlüsseln/Geheimnissen bei der Auflistung mehr</span><span class="sxs-lookup"><span data-stu-id="0bba9-656">No longer display managed keys/secrets while listing</span></span>
* <span data-ttu-id="0bba9-657">az keyvault create: Unterstützung von `--network-acls`, `--network-acls-ips` und `--network-acls-vnets` zur Angabe von Netzwerkregeln bei der Tresorerstellung</span><span class="sxs-lookup"><span data-stu-id="0bba9-657">az keyvault create: support `--network-acls`, `--network-acls-ips` and `--network-acls-vnets` for specifying network rules while creating vault</span></span>

### <a name="lock"></a><span data-ttu-id="0bba9-658">Sperre</span><span class="sxs-lookup"><span data-stu-id="0bba9-658">Lock</span></span>

* <span data-ttu-id="0bba9-659">Fehlerbehebung für „az lock delete“: „az lock delete“ funktioniert für „Microsoft.DocumentDB“ nicht.</span><span class="sxs-lookup"><span data-stu-id="0bba9-659">az lock delete fix bug: az lock delete does not work on Microsoft.DocumentDB</span></span>

### <a name="monitor"></a><span data-ttu-id="0bba9-660">Überwachen</span><span class="sxs-lookup"><span data-stu-id="0bba9-660">Monitor</span></span>

* <span data-ttu-id="0bba9-661">az monitor clone: Unterstützung des Klonens von Metrikregeln zwischen Ressourcen</span><span class="sxs-lookup"><span data-stu-id="0bba9-661">az monitor clone: support clone metric rules from one resource to another</span></span>
* <span data-ttu-id="0bba9-662">Fix IcM179210086: Erstellung einer benutzerdefinierten Metrikwarnung für die Application Insights-Metrik nicht möglich</span><span class="sxs-lookup"><span data-stu-id="0bba9-662">Fix IcM179210086: unable to create custom metric alert for their Application Insights metric</span></span>

### <a name="netappfiles"></a><span data-ttu-id="0bba9-663">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="0bba9-663">NetAppFiles</span></span>

* <span data-ttu-id="0bba9-664">az volume create: Datenschutzvolumes zum Hinzufügen von Replikationsvorgängen zugelassen: Genehmigen, Aussetzen, Fortsetzen, Status, Entfernen</span><span class="sxs-lookup"><span data-stu-id="0bba9-664">az volume create: Allow data protection volumes adding replication operations: approve, suspend, resume, status, remove</span></span>

### <a name="network"></a><span data-ttu-id="0bba9-665">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0bba9-665">Network</span></span>

* <span data-ttu-id="0bba9-666">az network application-gateway waf-policy managed-rule rule-set add: Unterstützung von „ Microsoft_BotManagerRuleSet“</span><span class="sxs-lookup"><span data-stu-id="0bba9-666">az network application-gateway waf-policy managed-rule rule-set add: support Microsoft_BotManagerRuleSet</span></span>
* <span data-ttu-id="0bba9-667">network watcher flow-log show: Falsche Veraltungsinformationen behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-667">network watcher flow-log show: fix wrong deprecating info</span></span>
* <span data-ttu-id="0bba9-668">Unterstützung von Hostnamen im Application Gateway-Listener</span><span class="sxs-lookup"><span data-stu-id="0bba9-668">support host names in application gateway listener</span></span>
* <span data-ttu-id="0bba9-669">az network nat gateway: Unterstützung der Erstellung einer leeren Ressource ohne öffentliche IP-Adresse oder Präfix für öffentliche IP-Adressen</span><span class="sxs-lookup"><span data-stu-id="0bba9-669">az network nat gateway: support create empty resource without public ip or public ip prefix</span></span>
* <span data-ttu-id="0bba9-670">Unterstützung der VPN-Gateway-Generierung</span><span class="sxs-lookup"><span data-stu-id="0bba9-670">Support vpn gateway generation</span></span>
* <span data-ttu-id="0bba9-671">Unterstützung von `--if-none-match` in `az network dns record-set {} add-record`</span><span class="sxs-lookup"><span data-stu-id="0bba9-671">Support `--if-none-match` in `az network dns record-set {} add-record`</span></span>

### <a name="packaging"></a><span data-ttu-id="0bba9-672">Verpackung</span><span class="sxs-lookup"><span data-stu-id="0bba9-672">Packaging</span></span>

* <span data-ttu-id="0bba9-673">Unterstützung von Python 3.5 eingestellt</span><span class="sxs-lookup"><span data-stu-id="0bba9-673">Drop support for python 3.5</span></span>

### <a name="profile"></a><span data-ttu-id="0bba9-674">Profil</span><span class="sxs-lookup"><span data-stu-id="0bba9-674">Profile</span></span>

* <span data-ttu-id="0bba9-675">az login: Warnung für MFA-Fehler</span><span class="sxs-lookup"><span data-stu-id="0bba9-675">az login: Show warning for MFA error</span></span>

### <a name="rdbms"></a><span data-ttu-id="0bba9-676">RDBMS</span><span class="sxs-lookup"><span data-stu-id="0bba9-676">RDBMS</span></span>

* <span data-ttu-id="0bba9-677">Befehle zur Verwaltung von Verschlüsselungsschlüsseln für Serverdaten für PostgreSQL und MySQL hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-677">Add server data encryption key management commands for PostgreSQL and MySQL</span></span>

## <a name="march-10-2020"></a><span data-ttu-id="0bba9-678">10. März 2020</span><span class="sxs-lookup"><span data-stu-id="0bba9-678">March 10, 2020</span></span>

<span data-ttu-id="0bba9-679">Version 2.2.0</span><span class="sxs-lookup"><span data-stu-id="0bba9-679">Version 2.2.0</span></span>

### <a name="acr"></a><span data-ttu-id="0bba9-680">ACR</span><span class="sxs-lookup"><span data-stu-id="0bba9-680">ACR</span></span>

* <span data-ttu-id="0bba9-681">Fix: `az acr login` löst fälschlicherweise Fehler aus</span><span class="sxs-lookup"><span data-stu-id="0bba9-681">Fix: `az acr login` wrongly raise error</span></span>
* <span data-ttu-id="0bba9-682">Neuer Befehl `az acr helm install-cli` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-682">Add new command `az acr helm install-cli`</span></span>
* <span data-ttu-id="0bba9-683">Privater Link und CMK-Unterstützung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-683">Add private link and CMK support</span></span>
* <span data-ttu-id="0bba9-684">Befehl „private-link-resource list“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-684">add 'private-link-resource list' command</span></span>

### <a name="aks"></a><span data-ttu-id="0bba9-685">AKS</span><span class="sxs-lookup"><span data-stu-id="0bba9-685">AKS</span></span>

* <span data-ttu-id="0bba9-686">Durchsuchen von AKS in Cloud-Shell korrigiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-686">fix the aks browse in cloud shell</span></span>
* <span data-ttu-id="0bba9-687">az aks: NoneType-Fehler beim Überwachen von „addon“ und „agentpool“ behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-687">az aks: Fix monitoring addon and agentpool NoneType errors</span></span>
* <span data-ttu-id="0bba9-688">„--nodepool-tags“ zum Knotenpool beim Erstellen von Azure-Kubernetes-Clustern hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-688">Add --nodepool-tags to node pool when creating azure kubernetes cluster</span></span>
* <span data-ttu-id="0bba9-689">„--tags“ beim Hinzufügen oder Aktualisieren eines Knotenpool in einem Cluster hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-689">Add --tags when adding or updating a nodepool to cluster</span></span>
* <span data-ttu-id="0bba9-690">aks create: `--enable-private-cluster` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-690">aks create: add `--enable-private-cluster`</span></span>
* <span data-ttu-id="0bba9-691">„--nodepool-labels“ beim Erstellen von Azure-Kubernetes-Clustern hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-691">add --nodepool-labels when creating azure kubernetes cluster</span></span>
* <span data-ttu-id="0bba9-692">„--labels“ beim Hinzufügen eines neuen Knotenpools zu einem Azure-Kubernetes-Cluster hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-692">add --labels when adding a new nodepool to azure kubernetes cluster</span></span>
* <span data-ttu-id="0bba9-693">Fehlender Schrägstrich (/) in der Dashboard-URL hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-693">add missing / in the dashboard url</span></span>
* <span data-ttu-id="0bba9-694">Unterstützung der Erstellung von AKS-Clustern, sodass verwaltete Identitäten möglich sind</span><span class="sxs-lookup"><span data-stu-id="0bba9-694">Support create aks clusters enabling managed identity</span></span>
* <span data-ttu-id="0bba9-695">az aks: Überprüfen, ob das Netzwerk-Plug-In entweder „azure“ oder „kubenet“ ist</span><span class="sxs-lookup"><span data-stu-id="0bba9-695">az aks: Validate network plugin to be either "azure" or "kubenet"</span></span>
* <span data-ttu-id="0bba9-696">az aks: Unterstützung für AAD-Sitzungsschlüssel hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-696">az aks: Add aad session key support</span></span>
* <span data-ttu-id="0bba9-697">[BREAKING CHANGE] az aks: Unterstützung von MSI-Änderungen für GF und BF für omsagent (Containerüberwachung)(#1)</span><span class="sxs-lookup"><span data-stu-id="0bba9-697">[BREAKING CHANGE] az aks: support msi changes for GF and BF for omsagent (Container monitoring)(#1)</span></span>
* <span data-ttu-id="0bba9-698">az aks use-dev-spaces: Endpunkt-Typoption zum Befehl „use-dev-spaces“, hinzugefügt, um den auf einem Azure Dev Spaces-Controller erstellten Endpunkt anzupassen</span><span class="sxs-lookup"><span data-stu-id="0bba9-698">az aks use-dev-spaces: Adding endpoint type option to the use-dev-spaces command to customize the endpoint created on an Azure Dev Spaces controller</span></span>

### <a name="appconfig"></a><span data-ttu-id="0bba9-699">AppConfig</span><span class="sxs-lookup"><span data-stu-id="0bba9-699">AppConfig</span></span>

* <span data-ttu-id="0bba9-700">Verwendung von „kv set“ entsperrt, um Schlüsseltresorverweis und -funktion hinzuzufügen …</span><span class="sxs-lookup"><span data-stu-id="0bba9-700">Unblock using "kv set" to add keyvault reference and feature …</span></span>

### <a name="appservice"></a><span data-ttu-id="0bba9-701">AppService</span><span class="sxs-lookup"><span data-stu-id="0bba9-701">AppService</span></span>

* <span data-ttu-id="0bba9-702">az webapp create : Beheben eines Problems beim Ausführen des Befehls mit „--runtime“</span><span class="sxs-lookup"><span data-stu-id="0bba9-702">az webapp create : Fix issue when running the command with --runtime</span></span>
* <span data-ttu-id="0bba9-703">az functionapp deployment source config-zip: Fehlermeldung hinzugefügt, wenn der Ressourcengruppen- oder Funktionsname ungültig oder nicht vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="0bba9-703">az functionapp deployment source config-zip: Add an error message if resource group or function name are invalid/don't exist</span></span>
* <span data-ttu-id="0bba9-704">functionapp create: Warnmeldung korrigiert, die derzeit mit `functionapp create` angezeigt wird und ein `--functions_version`-Flag angibt, aber irrtümlich ein `_` anstelle eines `-` im Flagnamen verwendet</span><span class="sxs-lookup"><span data-stu-id="0bba9-704">functionapp create: Fix the warning message that appears with `functionapp create` today which cites a `--functions_version` flag but erroneously uses a `_` instead of a `-` in the flag name</span></span>
* <span data-ttu-id="0bba9-705">az functionapp create: Es wurde aktualisiert, wie linuxFxVersion und der Containerimagename für Linux-Funktions-Apps festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="0bba9-705">az functionapp create: Updated the way linuxFxVersion and container image name were being set for linux function apps</span></span>
* <span data-ttu-id="0bba9-706">az functionapp deployment source config-zip: Problems behoben, das durch die Racebedingung für die Änderung von App-Einstellungen während der ZIP-Bereitstellung verursacht wird und während der Bereitstellung 5xx-Fehler ausgibt</span><span class="sxs-lookup"><span data-stu-id="0bba9-706">az functionapp deployment source config-zip: Fix an issue caused by app settings change racing condition during zip deploy, giving 5xx errors during deployment</span></span>
* <span data-ttu-id="0bba9-707">Fix #5720946: „az webapp backup“ legt Namen nicht fest</span><span class="sxs-lookup"><span data-stu-id="0bba9-707">Fix #5720946: az webapp backup fails to set name</span></span>

### <a name="arm"></a><span data-ttu-id="0bba9-708">ARM</span><span class="sxs-lookup"><span data-stu-id="0bba9-708">ARM</span></span>

* <span data-ttu-id="0bba9-709">az resource: Beispiele für das Ressourcenmodul verbessert</span><span class="sxs-lookup"><span data-stu-id="0bba9-709">az resource: Improve the examples of the resource module</span></span>
* <span data-ttu-id="0bba9-710">az policy assignment list: Unterstützung für das Auflisten von Richtlinienzuweisungen im Verwaltungsgruppenbereich</span><span class="sxs-lookup"><span data-stu-id="0bba9-710">az policy assignment list: Support listing policy assignments at Management Group scope</span></span>
* <span data-ttu-id="0bba9-711">`az deployment group` und `az deployment operation group` für Vorlagenbereitstellung in Ressourcengruppen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-711">Add `az deployment group` and `az deployment operation group` for template deployment at resource groups.</span></span> <span data-ttu-id="0bba9-712">Dies ist ein Duplikat von `az group deployment` und `az group deployment operation`.</span><span class="sxs-lookup"><span data-stu-id="0bba9-712">This is a duplicate of `az group deployment` and `az group deployment operation`</span></span>
* <span data-ttu-id="0bba9-713">`az deployment sub` und `az deployment operation sub` für Vorlagenbereitstellung im Abonnementbereich hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-713">Add `az deployment sub` and `az deployment operation sub` for template deployment at subscription scope.</span></span> <span data-ttu-id="0bba9-714">Dies ist ein Duplikat von `az deployment` und `az deployment operation`.</span><span class="sxs-lookup"><span data-stu-id="0bba9-714">This is a duplicate of `az deployment` and `az deployment operation`</span></span>
* <span data-ttu-id="0bba9-715">`az deployment mg` und `az deployment operation mg` für Vorlagenbereitstellung in Verwaltungsgruppen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-715">Add `az deployment mg` and `az deployment operation mg` for template deployment at management groups</span></span>
* <span data-ttu-id="0bba9-716">`az deployment tenant` und `az deployment operation tenant` für Vorlagenbereitstellung im Mandantenbereich hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-716">Add `az deployment tenant` and `az deployment operation tenant` for template deployment at tenant scope</span></span>
* <span data-ttu-id="0bba9-717">az policy assignment create: Beschreibung zu Parameter `--location` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-717">az policy assignment create: Add a description to the `--location` parameter</span></span>
* <span data-ttu-id="0bba9-718">az group deployment create: Parameter `--aux-tenants` zur mandantenübergreifenden Unterstützung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-718">az group deployment create: Add parameter `--aux-tenants` to support cross tenants</span></span>

### <a name="cdn"></a><span data-ttu-id="0bba9-719">CDN</span><span class="sxs-lookup"><span data-stu-id="0bba9-719">CDN</span></span>

* <span data-ttu-id="0bba9-720">CDN-WAF-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-720">Add CDN WAF commands</span></span>

### <a name="compute"></a><span data-ttu-id="0bba9-721">Compute</span><span class="sxs-lookup"><span data-stu-id="0bba9-721">Compute</span></span>

* <span data-ttu-id="0bba9-722">az sig image-version: „--data-snapshot-luns“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-722">az sig image-version: add --data-snapshot-luns</span></span>
* <span data-ttu-id="0bba9-723">az ppg show: „--colocation-status“ hinzugefügt, um das Abrufen des Zusammenstellungsstatus aller Ressourcen in der Näherungsplatzierungsgruppe zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="0bba9-723">az ppg show: add --colocation-status to enable fetching the colocation status of all the resources in the proximity placement group</span></span>
* <span data-ttu-id="0bba9-724">az vmss create/update: Unterstützung automatischer Reparaturen</span><span class="sxs-lookup"><span data-stu-id="0bba9-724">az vmss create/update: support automatic repairs</span></span>
* <span data-ttu-id="0bba9-725">[BREAKING CHANGE] az image template: „template“ in „builder“ umbenannt</span><span class="sxs-lookup"><span data-stu-id="0bba9-725">[BREAKING CHANGE] az image template: rename template to builder</span></span>
* <span data-ttu-id="0bba9-726">az image builder create: „--image-template“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-726">az image builder create: add --image-template</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="0bba9-727">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="0bba9-727">Cosmos DB</span></span>

* <span data-ttu-id="0bba9-728">Gespeicherte Prozedur „Add Sql“, udf- und trigger-Cmdlets hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-728">Add Sql stored procedure, udf and trigger cmdlets</span></span>
* <span data-ttu-id="0bba9-729">az cosmosdb create: „--key-uri“ hinzugefügt, um das Hinzufügen von Schlüsseltresor-Verschlüsselungsinformationen zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="0bba9-729">az cosmosdb create: add --key-uri to support adding key vault encryption information</span></span>

### <a name="keyvault"></a><span data-ttu-id="0bba9-730">KeyVault</span><span class="sxs-lookup"><span data-stu-id="0bba9-730">KeyVault</span></span>

* <span data-ttu-id="0bba9-731">keyvault create: „soft-delete“ standardmäßig aktiviert</span><span class="sxs-lookup"><span data-stu-id="0bba9-731">keyvault create: enable soft-delete by default</span></span>

### <a name="monitor"></a><span data-ttu-id="0bba9-732">Überwachen</span><span class="sxs-lookup"><span data-stu-id="0bba9-732">Monitor</span></span>

* <span data-ttu-id="0bba9-733">az monitor metrics alert create: Unterstützung von `~` in `--condition`</span><span class="sxs-lookup"><span data-stu-id="0bba9-733">az monitor metrics alert create: support `~` in `--condition`</span></span>

### <a name="network"></a><span data-ttu-id="0bba9-734">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0bba9-734">Network</span></span>

* <span data-ttu-id="0bba9-735">az network application-gateway rewrite-rule create: Unterstützung der URL-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="0bba9-735">az network application-gateway rewrite-rule create: support url configuration</span></span>
* <span data-ttu-id="0bba9-736">az network dns zone import: Bei „--zone-name“ wird die Groß-/Kleinschreibung künftig nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="0bba9-736">az network dns zone import: --zone-name will be case insensitive in the future</span></span>
* <span data-ttu-id="0bba9-737">az network private-endpoint/private-link-service: Vorschaubezeichnung entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-737">az network private-endpoint/private-link-service: remove preview label</span></span>
* <span data-ttu-id="0bba9-738">az network bastion: Unterstützung von „bastion“</span><span class="sxs-lookup"><span data-stu-id="0bba9-738">az network bastion: support bastion</span></span>
* <span data-ttu-id="0bba9-739">az network vnet list-available-ips: Unterstützung für das Auflisten verfügbarer IPs in einem VNET</span><span class="sxs-lookup"><span data-stu-id="0bba9-739">az network vnet list-available-ips: support list available ips in a vnet</span></span>
* <span data-ttu-id="0bba9-740">az network watcher flow-log create/list/delete/update: neue Befehle hinzugefügt, um Watcher-Datenflussprotokolle zu verwalten und „--location“ zur expliziten Identifizierung von Watcher verfügbar zu machen</span><span class="sxs-lookup"><span data-stu-id="0bba9-740">az network watcher flow-log create/list/delete/update: add new commands to manage watcher flow log and exposing --location to identify watcher explicitly</span></span>
* <span data-ttu-id="0bba9-741">az network watcher flow-log configure: veraltet</span><span class="sxs-lookup"><span data-stu-id="0bba9-741">az network watcher flow-log configure: deprecated</span></span>
* <span data-ttu-id="0bba9-742">az network watcher flow-log show: Unterstützung von „--location“ und „--name“, um ein ARM-formatiertes Ergebnis zu erhalten; alte formatierte Ausgabe als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-742">az network watcher flow-log show: support --location and --name to get ARM-formatted result, deprecated old formatted output</span></span>

### <a name="policy"></a><span data-ttu-id="0bba9-743">Richtlinie</span><span class="sxs-lookup"><span data-stu-id="0bba9-743">Policy</span></span>

* <span data-ttu-id="0bba9-744">az policy assignment create: Fehler behoben, dass automatisch generierter Name der Richtlinienzuweisung den Grenzwert überschreitet</span><span class="sxs-lookup"><span data-stu-id="0bba9-744">az policy assignment create: Fix the bug that automatically generated name of policy assignment exceeds the limit</span></span>

### <a name="rbac"></a><span data-ttu-id="0bba9-745">RBAC</span><span class="sxs-lookup"><span data-stu-id="0bba9-745">RBAC</span></span>

* <span data-ttu-id="0bba9-746">az ad group show: Problem behoben, dass „--group“-Wert als regulärer Ausdruck behandelt wurde</span><span class="sxs-lookup"><span data-stu-id="0bba9-746">az ad group show: fix --group value treated as regex problem</span></span>

### <a name="rdbms"></a><span data-ttu-id="0bba9-747">RDBMS</span><span class="sxs-lookup"><span data-stu-id="0bba9-747">RDBMS</span></span>

* <span data-ttu-id="0bba9-748">SDK-Version von „azure-mgmt-rdbms“ auf 2.0.0 festgelegt</span><span class="sxs-lookup"><span data-stu-id="0bba9-748">Bump the azure-mgmt-rdbms SDK version to 2.0.0</span></span>
* <span data-ttu-id="0bba9-749">az postgres private-endpoint-connection: Verwalten von Verbindungen mit privatem Postgres-Endpunkt</span><span class="sxs-lookup"><span data-stu-id="0bba9-749">az postgres private-endpoint-connection: manage postgres private endpoint connections</span></span>
* <span data-ttu-id="0bba9-750">az postgres private-link-resource: Verwalten von privaten Postgres-Linkressourcen</span><span class="sxs-lookup"><span data-stu-id="0bba9-750">az postgres private-link-resource: manage postgres private link resources</span></span>
* <span data-ttu-id="0bba9-751">az mysql private-endpoint-connection: Verwalten von Verbindungen mit privatem MySQL-Endpunkt</span><span class="sxs-lookup"><span data-stu-id="0bba9-751">az mysql private-endpoint-connection: manage mysql private endpoint connections</span></span>
* <span data-ttu-id="0bba9-752">az mysql private-link-resource: Verwalten von privaten MySQL-Linkressourcen</span><span class="sxs-lookup"><span data-stu-id="0bba9-752">az mysql private-link-resource: manage mysql private link resources</span></span>
* <span data-ttu-id="0bba9-753">az mariadb private-endpoint-connection: Verwalten von Verbindungen mit privatem MariaDB-Endpunkt</span><span class="sxs-lookup"><span data-stu-id="0bba9-753">az mariadb private-endpoint-connection: manage mariadb private endpoint connections</span></span>
* <span data-ttu-id="0bba9-754">az mariadb private-link-resource: Verwalten von privaten MariaDB-Linkressourcen</span><span class="sxs-lookup"><span data-stu-id="0bba9-754">az mariadb private-link-resource: manage mariadb private link resources</span></span>
* <span data-ttu-id="0bba9-755">Aktualisieren von Tests von privaten RDBMS-Endpunkten</span><span class="sxs-lookup"><span data-stu-id="0bba9-755">Updating RDBMS Private Endpoint Tests</span></span>

### <a name="sql"></a><span data-ttu-id="0bba9-756">SQL</span><span class="sxs-lookup"><span data-stu-id="0bba9-756">SQL</span></span>

* <span data-ttu-id="0bba9-757">Sql midb: list-deleted, show-deleted, update-retention, show-retention hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-757">Sql midb Add: list-deleted, show-deleted, update-retention, show-retention</span></span>
* <span data-ttu-id="0bba9-758">(sql server create:) Optionales Flag „Enable“/„Disable“ für public-network-access zu „sql server create“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-758">(sql server create:) Add optional public-network-access 'Enable'/'Disable' flag to sql server create</span></span>
* <span data-ttu-id="0bba9-759">(sql server update): kundenorientierte Änderung vorgenommen</span><span class="sxs-lookup"><span data-stu-id="0bba9-759">(sql server update:) make some customer-facing change</span></span>
* <span data-ttu-id="0bba9-760">Eigenschaft „minimal_tls_version“ für MI und SQL-Datenbank hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-760">Add minimal_tls_version property for MI and SQL DB</span></span>

### <a name="storage"></a><span data-ttu-id="0bba9-761">Storage</span><span class="sxs-lookup"><span data-stu-id="0bba9-761">Storage</span></span>

* <span data-ttu-id="0bba9-762">az storage blob delete-batch: Flag `--dryrun` mit Fehlverhalten</span><span class="sxs-lookup"><span data-stu-id="0bba9-762">az storage blob delete-batch: Misbehaving `--dryrun` flag</span></span>
* <span data-ttu-id="0bba9-763">az storage account network-rule hinzugefügt (Fehlerbehebung): Hinzufügen von Vorgängen muss idempotent sein</span><span class="sxs-lookup"><span data-stu-id="0bba9-763">az storage account network-rule add (bug fix): add operation should be idempotent</span></span>
* <span data-ttu-id="0bba9-764">az storage account create/update: Unterstützung für Routingpräferenz hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-764">az storage account create/update: Add Routing Preference support</span></span>
* <span data-ttu-id="0bba9-765">„azure-mgmt-storage“ auf Version 8.0.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-765">Upgrade azure-mgmt-storage version to 8.0.0</span></span>
* <span data-ttu-id="0bba9-766">az storage container immutability create: Parameter „--allow-protected-append-write“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-766">az storage container immutability create: add --allow-protected-append-write parameter</span></span>
* <span data-ttu-id="0bba9-767">az storage account private-link-resource list: Unterstützung zum Auflisten privater Linkressourcen für Speicherkonto hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-767">az storage account private-link-resource list: Add support to list private link resources for storage account</span></span>
* <span data-ttu-id="0bba9-768">az storage account private-endpoint-connection approve/reject/show/delete: Unterstützung der Verwaltung von Verbindungen mit privaten Endpunkten</span><span class="sxs-lookup"><span data-stu-id="0bba9-768">az storage account private-endpoint-connection approve/reject/show/delete: Support to manage private endpoint connections</span></span>
* <span data-ttu-id="0bba9-769">az storage account blob-service-properties update: „--enable-restore-policy“ und „--restore-days“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-769">az storage account blob-service-properties update: add --enable-restore-policy and --restore-days</span></span>
* <span data-ttu-id="0bba9-770">az storage blob restore: Unterstützung für die Wiederherstellung von Blobbereichen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-770">az storage blob restore: Add support to restore blob ranges</span></span>

## <a name="february-18-2020"></a><span data-ttu-id="0bba9-771">18. Februar 2020</span><span class="sxs-lookup"><span data-stu-id="0bba9-771">February 18, 2020</span></span>

<span data-ttu-id="0bba9-772">Version 2.1.0</span><span class="sxs-lookup"><span data-stu-id="0bba9-772">Version 2.1.0</span></span>

### <a name="acr"></a><span data-ttu-id="0bba9-773">ACR</span><span class="sxs-lookup"><span data-stu-id="0bba9-773">ACR</span></span>

* <span data-ttu-id="0bba9-774">Neues Argument `--expose-token` für `az acr login` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-774">Add a new argument `--expose-token` for `az acr login`</span></span>
* <span data-ttu-id="0bba9-775">Falsche Ausgabe für `az acr task identity show -n Name -r Registry -o table` korrigiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-775">Fix the incorrect output of `az acr task identity show -n Name -r Registry -o table`</span></span>
* <span data-ttu-id="0bba9-776">az acr login: Auslösen von „CLIError“, wenn vom Docker-Befehl Fehler zurückgegeben werden</span><span class="sxs-lookup"><span data-stu-id="0bba9-776">az acr login: Throw a CLIError if there are errors returned by docker command</span></span>

### <a name="acs"></a><span data-ttu-id="0bba9-777">ACS</span><span class="sxs-lookup"><span data-stu-id="0bba9-777">ACS</span></span>

* <span data-ttu-id="0bba9-778">aks create/update: Validierung für `--vnet-subnet-id` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-778">aks create/update: add `--vnet-subnet-id` validation</span></span>

### <a name="aladdin"></a><span data-ttu-id="0bba9-779">Aladdin</span><span class="sxs-lookup"><span data-stu-id="0bba9-779">Aladdin</span></span>

* <span data-ttu-id="0bba9-780">Analysieren der generierten Beispiele in „_help.py“ der Befehle</span><span class="sxs-lookup"><span data-stu-id="0bba9-780">Parse generated examples into commands' _help.py</span></span>

### <a name="ams"></a><span data-ttu-id="0bba9-781">AMS</span><span class="sxs-lookup"><span data-stu-id="0bba9-781">AMS</span></span>

* <span data-ttu-id="0bba9-782">az ams ist jetzt allgemein verfügbar.</span><span class="sxs-lookup"><span data-stu-id="0bba9-782">az ams is GA now</span></span>

### <a name="appconfig"></a><span data-ttu-id="0bba9-783">AppConfig</span><span class="sxs-lookup"><span data-stu-id="0bba9-783">AppConfig</span></span>

* <span data-ttu-id="0bba9-784">Hilfenachricht überarbeitet, um nicht unterstützte Schlüssel-/Bezeichnungsfilter auszuschließen</span><span class="sxs-lookup"><span data-stu-id="0bba9-784">Revise help message to exclude unsupported key/label filter</span></span>
* <span data-ttu-id="0bba9-785">Vorschautag für die meisten Befehle entfernt (mit Ausnahme der Flags für verwaltete Identitäten und Features)</span><span class="sxs-lookup"><span data-stu-id="0bba9-785">Remove preview tag for most commands excluding managed identity and feature flags</span></span>
* <span data-ttu-id="0bba9-786">Kundenseitig verwalteter Schlüssel beim Aktualisieren der Speicher hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-786">Add customer managed key when updating stores</span></span>

### <a name="appservice"></a><span data-ttu-id="0bba9-787">AppService</span><span class="sxs-lookup"><span data-stu-id="0bba9-787">AppService</span></span>

* <span data-ttu-id="0bba9-788">az webapp list-runtimes: Fehler bei „list-runtimes“ behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-788">az webapp list-runtimes: Fix the bug for list-runtimes</span></span>
* <span data-ttu-id="0bba9-789">„az webapp|functionapp config ssl create“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-789">Add az webapp|functionapp config ssl create</span></span>
* <span data-ttu-id="0bba9-790">Unterstützung für v3-Funktions-Apps und Node 12</span><span class="sxs-lookup"><span data-stu-id="0bba9-790">Add support for v3 function apps and node 12</span></span>

### <a name="arm"></a><span data-ttu-id="0bba9-791">ARM</span><span class="sxs-lookup"><span data-stu-id="0bba9-791">ARM</span></span>

* <span data-ttu-id="0bba9-792">az policy assignment create: Fehlermeldung korrigiert, die angezeigt wird, wenn der Parameter `--policy` ungültig ist</span><span class="sxs-lookup"><span data-stu-id="0bba9-792">az policy assignment create: Fix the error message when the `--policy` parameter is invalid</span></span>
* <span data-ttu-id="0bba9-793">az group deployment create: Fehler „stat: path too long for Windows" korrigiert, der angezeigt wird, wenn eine zu große Datei vom Typ „parameters.json“ verwendet wird</span><span class="sxs-lookup"><span data-stu-id="0bba9-793">az group deployment create: Fix "stat: path too long for Windows" error when using large parameters.json file</span></span>

### <a name="backup"></a><span data-ttu-id="0bba9-794">Backup</span><span class="sxs-lookup"><span data-stu-id="0bba9-794">Backup</span></span>

* <span data-ttu-id="0bba9-795">Korrektur des Wiederherstellungsflows auf Elementebene am ursprünglichen Speicherort</span><span class="sxs-lookup"><span data-stu-id="0bba9-795">Fix for item level recovery flow in OLR</span></span>
* <span data-ttu-id="0bba9-796">Unterstützung von „Als Dateien wiederherstellen“ für SQL- und SAP-Datenbanken hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-796">Add restore as files support for SQL and SAP Databases</span></span>

### <a name="compute"></a><span data-ttu-id="0bba9-797">Compute</span><span class="sxs-lookup"><span data-stu-id="0bba9-797">Compute</span></span>

* <span data-ttu-id="0bba9-798">vm/vmss/availability-set update: „--ppg“ hinzugefügt, um die Aktualisierung von „ProximityPlacementGroup“ zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="0bba9-798">vm/vmss/availability-set update: add --ppg to allowing updating ProximityPlacementGroup</span></span>
* <span data-ttu-id="0bba9-799">vmss create: „--data-disk-iops“ und „--data-disk-mbps“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-799">vmss create: add --data-disk-iops and --data-disk-mbps</span></span>
* <span data-ttu-id="0bba9-800">az vm host: Vorschautag für `vm host` und `vm host group` entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-800">az vm host: remove preview tag for `vm host` and `vm host group`</span></span>
* <span data-ttu-id="0bba9-801">[BREAKING CHANGE] Behebung Nr. 10728: `az vm create`: Automatisches Erstellen des Subnetzes, wenn das VNET angegeben wird und das Subnetz nicht vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="0bba9-801">[BREAKING CHANGE] Fix #10728: `az vm create`: create subnet automatically if vnet is specified and subnet not exists</span></span>
* <span data-ttu-id="0bba9-802">Erhöhen der Stabilität von „vm image list“</span><span class="sxs-lookup"><span data-stu-id="0bba9-802">Increase robustness of vm image list</span></span>

### <a name="eventhub"></a><span data-ttu-id="0bba9-803">Eventhub</span><span class="sxs-lookup"><span data-stu-id="0bba9-803">Eventhub</span></span>

* <span data-ttu-id="0bba9-804">Azure Stack-Unterstützung für Profil „2019-03-01-hybrid“</span><span class="sxs-lookup"><span data-stu-id="0bba9-804">Azure Stack support for 2019-03-01-hybrid profile</span></span>

### <a name="keyvault"></a><span data-ttu-id="0bba9-805">KeyVault</span><span class="sxs-lookup"><span data-stu-id="0bba9-805">KeyVault</span></span>

* <span data-ttu-id="0bba9-806">az keyvault key create: neuer Wert `import` für Parameter `--ops` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-806">az keyvault key create: add a new value `import` for parameter `--ops`</span></span>
* <span data-ttu-id="0bba9-807">az keyvault key list-versions: Unterstützung des Parameters `--id` für die Angabe von Schlüsseln</span><span class="sxs-lookup"><span data-stu-id="0bba9-807">az keyvault key list-versions: support parameter `--id` for specifying keys</span></span>
* <span data-ttu-id="0bba9-808">Unterstützung für Verbindungen mit privaten Endpunkten</span><span class="sxs-lookup"><span data-stu-id="0bba9-808">Support private endpoint connections</span></span>

### <a name="network"></a><span data-ttu-id="0bba9-809">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0bba9-809">Network</span></span>

* <span data-ttu-id="0bba9-810">Geändert in „azure-mgmt-network 9.0.0“</span><span class="sxs-lookup"><span data-stu-id="0bba9-810">Bump to azure-mgmt-network 9.0.0</span></span>
* <span data-ttu-id="0bba9-811">az network private-link-service update/create: Unterstützung von „--enable-proxy-protocol“</span><span class="sxs-lookup"><span data-stu-id="0bba9-811">az network private-link-service update/create: support --enable-proxy-protocol</span></span>
* <span data-ttu-id="0bba9-812">Feature für Version 2 von Verbindungsmonitor hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-812">Add connection Monitor V2 feature</span></span>

### <a name="packaging"></a><span data-ttu-id="0bba9-813">Verpackung</span><span class="sxs-lookup"><span data-stu-id="0bba9-813">Packaging</span></span>

* <span data-ttu-id="0bba9-814">[BREAKING CHANGE] Unterstützung für Python 2.7 eingestellt</span><span class="sxs-lookup"><span data-stu-id="0bba9-814">[BREAKING CHANGE] Drop support for Python 2.7</span></span>

### <a name="profile"></a><span data-ttu-id="0bba9-815">Profil</span><span class="sxs-lookup"><span data-stu-id="0bba9-815">Profile</span></span>

* <span data-ttu-id="0bba9-816">Vorschau: Neue Attribute `homeTenantId` und `managedByTenants` zu Abonnementkonten hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-816">Preview: Add new attributes `homeTenantId` and `managedByTenants` to subscription accounts.</span></span> <span data-ttu-id="0bba9-817">Führen Sie `az login` erneut aus, damit die Änderungen wirksam werden.</span><span class="sxs-lookup"><span data-stu-id="0bba9-817">Please re-run `az login` for the changes to take effect</span></span>
* <span data-ttu-id="0bba9-818">az login: Eine Warnung wird angezeigt, wenn ein Abonnement von mehren Mandanten aufgeführt wird und der erste als Standard festgelegt wird.</span><span class="sxs-lookup"><span data-stu-id="0bba9-818">az login: Show a warning when a subscription is listed from more than one tenants and default to the first one.</span></span> <span data-ttu-id="0bba9-819">Fügen Sie `--tenant` in `az login` ein, um beim Zugreifen auf dieses Abonnement einen bestimmten Mandanten auszuwählen.</span><span class="sxs-lookup"><span data-stu-id="0bba9-819">To select a specific tenant when accessing this subscription, please include `--tenant` in `az login`</span></span>

### <a name="role"></a><span data-ttu-id="0bba9-820">Role</span><span class="sxs-lookup"><span data-stu-id="0bba9-820">Role</span></span>

* <span data-ttu-id="0bba9-821">az role assignment create: Problem behoben, das beim Zuweisen einer Rolle zu einem Dienstprinzipal nach Anzeigename einen Fehler vom Typ „HTTP 400“ verursachte</span><span class="sxs-lookup"><span data-stu-id="0bba9-821">az role assignment create: Fix the error that assigning a role to a service principal by display name yields a HTTP 400</span></span>

### <a name="sql"></a><span data-ttu-id="0bba9-822">SQL</span><span class="sxs-lookup"><span data-stu-id="0bba9-822">SQL</span></span>

* <span data-ttu-id="0bba9-823">Cmdlet `az sql mi update` der verwalteten SQL-Instanz mit zwei neuen Parametern aktualisiert: tier und family</span><span class="sxs-lookup"><span data-stu-id="0bba9-823">Update SQL Managed Instance cmdlet `az sql mi update` with two new parameters: tier and family</span></span>

### <a name="storage"></a><span data-ttu-id="0bba9-824">Storage</span><span class="sxs-lookup"><span data-stu-id="0bba9-824">Storage</span></span>

* <span data-ttu-id="0bba9-825">[BREAKING CHANGE] `az storage account create`: Art des Standardspeicherkontos in StorageV2 geändert</span><span class="sxs-lookup"><span data-stu-id="0bba9-825">[BREAKING CHANGE] `az storage account create`: Change default storage account kind to StorageV2</span></span>

## <a name="february-04-2020"></a><span data-ttu-id="0bba9-826">04. Februar 2020</span><span class="sxs-lookup"><span data-stu-id="0bba9-826">February 04, 2020</span></span>

<span data-ttu-id="0bba9-827">Version 2.0.81</span><span class="sxs-lookup"><span data-stu-id="0bba9-827">Version 2.0.81</span></span>

### <a name="acs"></a><span data-ttu-id="0bba9-828">ACS</span><span class="sxs-lookup"><span data-stu-id="0bba9-828">ACS</span></span>

* <span data-ttu-id="0bba9-829">Unterstützung für das Festlegen zugeordneter Ausgangsports und Leerlauftimeouts für Load Balancer Standard hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-829">Add support to set outbound allocated ports and idle timeouts on standard load balancer</span></span>
* <span data-ttu-id="0bba9-830">Aktualisierung auf API-Version 2019-11-01</span><span class="sxs-lookup"><span data-stu-id="0bba9-830">Update to API Version 2019-11-01</span></span>

### <a name="acr"></a><span data-ttu-id="0bba9-831">ACR</span><span class="sxs-lookup"><span data-stu-id="0bba9-831">ACR</span></span>

* <span data-ttu-id="0bba9-832">[BREAKING CHANGE] `az acr delete` löst eine Eingabeaufforderung aus.</span><span class="sxs-lookup"><span data-stu-id="0bba9-832">[BREAKING CHANGE] `az acr delete` will prompt</span></span>
* <span data-ttu-id="0bba9-833">[BREAKING CHANGE] „az acr task delete“ löst eine Eingabeaufforderung aus.</span><span class="sxs-lookup"><span data-stu-id="0bba9-833">[BREAKING CHANGE] 'az acr task delete' will prompt</span></span>
* <span data-ttu-id="0bba9-834">Neue Befehlsgruppe „az acr taskrun show/list/delete“ für die Aufgabenausführungsverwaltung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-834">Add a new command group 'az acr taskrun show/list/delete' for taskrun management</span></span>

### <a name="aks"></a><span data-ttu-id="0bba9-835">AKS</span><span class="sxs-lookup"><span data-stu-id="0bba9-835">AKS</span></span>

* <span data-ttu-id="0bba9-836">Jeder Cluster erhält einen separaten Dienstprinzipal zur Verbesserung der Isolation.</span><span class="sxs-lookup"><span data-stu-id="0bba9-836">Each cluster gets a separate service principal to improve isolation</span></span>

### <a name="appconfig"></a><span data-ttu-id="0bba9-837">AppConfig</span><span class="sxs-lookup"><span data-stu-id="0bba9-837">AppConfig</span></span>

* <span data-ttu-id="0bba9-838">Unterstützung für den Import/Export von KeyVault-Verweisen in/aus AppService</span><span class="sxs-lookup"><span data-stu-id="0bba9-838">Support import/export of keyvault references from/to appservice</span></span>
* <span data-ttu-id="0bba9-839">Unterstützung für den Import/Export aller Bezeichnungen in appconfig und aus appconfig</span><span class="sxs-lookup"><span data-stu-id="0bba9-839">Support import/export of all labels from appconfig to appconfig</span></span>
* <span data-ttu-id="0bba9-840">Überprüfen der Schlüssel- und Featurenamen vor dem Festlegen und Importieren</span><span class="sxs-lookup"><span data-stu-id="0bba9-840">Validate key and feature names before setting and importing</span></span>
* <span data-ttu-id="0bba9-841">Verfügbarmachen der SKU-Änderung für den Konfigurationsspeicher</span><span class="sxs-lookup"><span data-stu-id="0bba9-841">Expose sku modification for configuration store.</span></span>
* <span data-ttu-id="0bba9-842">Befehlsgruppe für die verwaltete Identität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-842">Add command group for managed identity.</span></span>

### <a name="appservice"></a><span data-ttu-id="0bba9-843">AppService</span><span class="sxs-lookup"><span data-stu-id="0bba9-843">AppService</span></span>

* <span data-ttu-id="0bba9-844">Azure Stack: Oberflächenbefehle im Profil „2019-03-01-hybrid“</span><span class="sxs-lookup"><span data-stu-id="0bba9-844">Azure Stack: surface commands under the profile of 2019-03-01-hybrid</span></span>
* <span data-ttu-id="0bba9-845">functionapp: Funktion zum Erstellen von Java-Funktions-Apps in Linux hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-845">functionapp: Add ability to create Java function apps in Linux</span></span>

### <a name="arm"></a><span data-ttu-id="0bba9-846">ARM</span><span class="sxs-lookup"><span data-stu-id="0bba9-846">ARM</span></span>

* <span data-ttu-id="0bba9-847">Behebung von Problem Nr. 10246: `az resource tag` stürzt ab, wenn der übergebene Parameter `--ids` der Ressourcengruppen-ID entspricht.</span><span class="sxs-lookup"><span data-stu-id="0bba9-847">Fix issue #10246: `az resource tag` crashes when the parameter `--ids` passed in is resource group ID</span></span>
* <span data-ttu-id="0bba9-848">Behebung von Problem Nr. 11658: Der Befehl `az group export` unterstützt die Parameter `--query` und `--output` nicht.</span><span class="sxs-lookup"><span data-stu-id="0bba9-848">Fix issue #11658: `az group export` command does not support `--query` and `--output` parameters</span></span>
* <span data-ttu-id="0bba9-849">Behebung von Problem Nr. 10279: Der Exitcode von `az group deployment validate` ist 0, wenn bei der Überprüfung ein Fehler auftritt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-849">Fix issue #10279: The exit code of `az group deployment validate` is 0 when the verification fails</span></span>
* <span data-ttu-id="0bba9-850">Behebung von Problem Nr. 9916: Fehlermeldung des Konflikts zwischen Tag und anderen Filterbedingungen für Befehl `az resource list` verbessert</span><span class="sxs-lookup"><span data-stu-id="0bba9-850">Fix issue #9916: Improve the error message of the conflict between tag and other filter conditions for `az resource list` command</span></span>
* <span data-ttu-id="0bba9-851">Neuer Parameter `--managed-by` hinzugefügt, um das Hinzufügen der Informationen vom Typ „managedBy“ für Befehl `az group create` zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="0bba9-851">Add new parameter `--managed-by` to support adding managedBy information for command `az group create`</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="0bba9-852">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="0bba9-852">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="0bba9-853">Untergruppe `monitor` hinzugefügt, um Log Analytics-Überwachung im Azure Red Hat OpenShift-Cluster zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="0bba9-853">Add `monitor` subgroup to manage Log Analytics monitoring in Azure Red Hat OpensShift cluster</span></span>

### <a name="botservice"></a><span data-ttu-id="0bba9-854">BotService</span><span class="sxs-lookup"><span data-stu-id="0bba9-854">BotService</span></span>

* <span data-ttu-id="0bba9-855">Behebung von Problem Nr. 11697: `az bot create` ist nicht idempotent.</span><span class="sxs-lookup"><span data-stu-id="0bba9-855">Fix issue #11697: `az bot create` is not idempotent</span></span>
* <span data-ttu-id="0bba9-856">Tests zur Namenskorrektur geändert, sodass sie nur im Livemodus ausgeführt werden</span><span class="sxs-lookup"><span data-stu-id="0bba9-856">Change name-correcting tests to run in Live-mode only</span></span>

### <a name="cdn"></a><span data-ttu-id="0bba9-857">CDN</span><span class="sxs-lookup"><span data-stu-id="0bba9-857">CDN</span></span>

* <span data-ttu-id="0bba9-858">Unterstützung für das rulesEngine-Feature hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-858">Add support for rulesEngine feature</span></span>
* <span data-ttu-id="0bba9-859">Neue Befehlsgruppe „cdn endpoint rule“ zum Verwalten von Regeln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-859">Add new commands group 'cdn endpoint rule' to manage rules</span></span>
* <span data-ttu-id="0bba9-860">azure-mgmt-cdn-Version auf 4.0.0 aktualisiert, um API-Version 2019-04-15 zu verwenden</span><span class="sxs-lookup"><span data-stu-id="0bba9-860">Update azure-mgmt-cdn version to 4.0.0 to use api version 2019-04-15</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="0bba9-861">Bereitstellungs-Manager</span><span class="sxs-lookup"><span data-stu-id="0bba9-861">Deployment Manager</span></span>

* <span data-ttu-id="0bba9-862">Auflistungsvorgang für alle Ressourcen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-862">Add list operation for all resources.</span></span>
* <span data-ttu-id="0bba9-863">Schrittressource für neuen Schritttyp optimiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-863">Enhance step resource for new step type.</span></span>
* <span data-ttu-id="0bba9-864">Paket „azure-mgmt-deploymentmanager“ zur Verwendung von Version 0.2.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-864">Update azure-mgmt-deploymentmanager package to use version 0.2.0.</span></span>

### <a name="iot"></a><span data-ttu-id="0bba9-865">IoT</span><span class="sxs-lookup"><span data-stu-id="0bba9-865">IoT</span></span>

* <span data-ttu-id="0bba9-866">Befehle vom Typ „IoT hub Job“ als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="0bba9-866">Deprecate 'IoT hub Job' commands.</span></span>

### <a name="iot-central"></a><span data-ttu-id="0bba9-867">IoT Central</span><span class="sxs-lookup"><span data-stu-id="0bba9-867">IoT Central</span></span>

* <span data-ttu-id="0bba9-868">Unterstützung der App-Erstellung/-Aktualisierung mit neuem SKU-Namen ST0, ST1, ST2</span><span class="sxs-lookup"><span data-stu-id="0bba9-868">Support app creation/update with the new sku name ST0, ST1, ST2.</span></span>

### <a name="key-vault"></a><span data-ttu-id="0bba9-869">Key Vault</span><span class="sxs-lookup"><span data-stu-id="0bba9-869">Key Vault</span></span>

* <span data-ttu-id="0bba9-870">Neuer Befehl `az keyvault key download` zum Herunterladen von Schlüsseln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-870">Add a new command `az keyvault key download` for downloading keys.</span></span>

### <a name="misc"></a><span data-ttu-id="0bba9-871">Sonstiges</span><span class="sxs-lookup"><span data-stu-id="0bba9-871">Misc</span></span>

* <span data-ttu-id="0bba9-872">Behebung Nr. 6371: Unterstützung für die Vervollständigung von Dateinamen und Umgebungsvariablen in Bash</span><span class="sxs-lookup"><span data-stu-id="0bba9-872">Fix #6371: Support filename and environment variable completion in Bash</span></span>

### <a name="network"></a><span data-ttu-id="0bba9-873">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0bba9-873">Network</span></span>

* <span data-ttu-id="0bba9-874">Behebung Nr. 2092: az network dns record-set add/remove: Warnung hinzugefügt, wenn Datensatzgruppe nicht gefunden wurde.</span><span class="sxs-lookup"><span data-stu-id="0bba9-874">Fix #2092: az network dns record-set add/remove: add warning when record-set is not found.</span></span> <span data-ttu-id="0bba9-875">In Zukunft wird ein zusätzliches Argument unterstützt, um diese automatische Erstellung zu bestätigen.</span><span class="sxs-lookup"><span data-stu-id="0bba9-875">In the future, an extra argument will be supported to confirm this auto creation.</span></span>

### <a name="policy"></a><span data-ttu-id="0bba9-876">Richtlinie</span><span class="sxs-lookup"><span data-stu-id="0bba9-876">Policy</span></span>

* <span data-ttu-id="0bba9-877">Neuer Befehl `az policy metadata` hinzugefügt, um umfangreiche Richtlinienmetadatenressourcen abzurufen</span><span class="sxs-lookup"><span data-stu-id="0bba9-877">Add new command `az policy metadata` to retrieve rich policy metadata resources</span></span>
* <span data-ttu-id="0bba9-878">`az policy remediation create`: Geben Sie mit dem Parameter `--resource-discovery-mode` an, ob die Konformität vor der Wartung neu bewertet werden soll.</span><span class="sxs-lookup"><span data-stu-id="0bba9-878">`az policy remediation create`: Specify whether compliance should be re-evaluated prior to remediation with the `--resource-discovery-mode` parameter</span></span>

### <a name="profile"></a><span data-ttu-id="0bba9-879">Profil</span><span class="sxs-lookup"><span data-stu-id="0bba9-879">Profile</span></span>

* <span data-ttu-id="0bba9-880">`az account get-access-token`: Parameter `--tenant` hinzugefügt, um das Token für den Mandanten direkt abzurufen. Es muss kein Abonnement angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="0bba9-880">`az account get-access-token`: Add `--tenant` parameter to acquire token for the tenant directly, needless to specify a subscription</span></span>

### <a name="rbac"></a><span data-ttu-id="0bba9-881">RBAC</span><span class="sxs-lookup"><span data-stu-id="0bba9-881">RBAC</span></span>

* <span data-ttu-id="0bba9-882">[BREAKING CHANGE] Behebung Nr. 11883: `az role assignment create`: Bei leerem Bereich wird ein Fehler ausgegeben.</span><span class="sxs-lookup"><span data-stu-id="0bba9-882">[BREAKING CHANGE] Fix #11883: `az role assignment create`: empty scope will prompt error</span></span>

### <a name="security"></a><span data-ttu-id="0bba9-883">Sicherheit</span><span class="sxs-lookup"><span data-stu-id="0bba9-883">Security</span></span>

* <span data-ttu-id="0bba9-884">Neue Befehle `az atp show` und `az atp update` hinzugefügt, um erweiterte Einstellungen für den Bedrohungsschutz für Speicherkonten anzuzeigen und zu verwalten</span><span class="sxs-lookup"><span data-stu-id="0bba9-884">Add new commands `az atp show` and `az atp update` to view and manage advanced threat protection settings for storage accounts.</span></span>

### <a name="sql"></a><span data-ttu-id="0bba9-885">SQL</span><span class="sxs-lookup"><span data-stu-id="0bba9-885">SQL</span></span>

* <span data-ttu-id="0bba9-886">`sql dw create`: Parameter `--zone-redundant` und `--read-replica-count` als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="0bba9-886">`sql dw create`: deprecate `--zone-redundant` and `--read-replica-count` parameters.</span></span> <span data-ttu-id="0bba9-887">Diese Parameter gelten nicht für Datawarehouse.</span><span class="sxs-lookup"><span data-stu-id="0bba9-887">These parameters do not apply to DataWarehouse.</span></span>
* <span data-ttu-id="0bba9-888">[BREAKING CHANGE] `az sql db create`: „WideWorldImportersStd“ und „WideWorldImportersFull“ als dokumentierte zulässige Werte für „az sql db create --sample-name“ entfernt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-888">[BREAKING CHANGE] `az sql db create`: Remove "WideWorldImportersStd" and "WideWorldImportersFull" as documented allowed values for "az sql db create --sample-name".</span></span> <span data-ttu-id="0bba9-889">Diese Beispieldatenbanken führen immer zu einem Fehler bei der Erstellung.</span><span class="sxs-lookup"><span data-stu-id="0bba9-889">These sample databases would always cause creation to fail.</span></span>
* <span data-ttu-id="0bba9-890">Neue Befehle `sql db classification show/list/update/delete` und `sql db classification recommendation list/enable/disable` zur Verwaltung von Vertraulichkeitsklassifizierungen für SQL-Datenbanken hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-890">Add New commands `sql db classification show/list/update/delete` and `sql db classification recommendation list/enable/disable` to manage sensitivity classifications for SQL databases.</span></span>
* <span data-ttu-id="0bba9-891">`az sql db audit-policy`: Behebung für leere Überwachungsaktionen und -gruppen</span><span class="sxs-lookup"><span data-stu-id="0bba9-891">`az sql db audit-policy`: Fix for empty audit actions and groups</span></span>

### <a name="storage"></a><span data-ttu-id="0bba9-892">Storage</span><span class="sxs-lookup"><span data-stu-id="0bba9-892">Storage</span></span>

* <span data-ttu-id="0bba9-893">Neue Befehlsgruppe `az storage share-rm` hinzugefügt, um den Ressourcenanbieter „Microsoft.Storage“ für Verwaltungsvorgänge der Azure-Dateifreigabe zu verwenden</span><span class="sxs-lookup"><span data-stu-id="0bba9-893">Add a new command group `az storage share-rm` to use the Microsoft.Storage resource provider for Azure file share management operations.</span></span>
* <span data-ttu-id="0bba9-894">Behebung für Problem Nr. 11415: Berechtigungsfehler für `az storage blob update`</span><span class="sxs-lookup"><span data-stu-id="0bba9-894">Fix issue #11415: permission error for `az storage blob update`</span></span>
* <span data-ttu-id="0bba9-895">Integration von Azcopy 10.3.3 und Unterstützung von Win32</span><span class="sxs-lookup"><span data-stu-id="0bba9-895">Integrate Azcopy 10.3.3 and support Win32.</span></span>
* <span data-ttu-id="0bba9-896">`az storage copy`: Parameter `--include-path`, `--include-pattern`, `--exclude-path` und`--exclude-pattern` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-896">`az storage copy`: Add `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="0bba9-897">`az storage remove`: Parameter `--inlcude` und `--exclude` in Parameter `--include-path`, `--include-pattern`, `--exclude-path` und`--exclude-pattern` geändert</span><span class="sxs-lookup"><span data-stu-id="0bba9-897">`az storage remove`: Change `--inlcude` and `--exclude` parameters to `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="0bba9-898">`az storage sync`: Parameter `--include-pattern`, `--exclude-path` und`--exclude-pattern` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-898">`az storage sync`: Add `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>

### <a name="servicefabric"></a><span data-ttu-id="0bba9-899">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="0bba9-899">ServiceFabric</span></span>

* <span data-ttu-id="0bba9-900">Neue Befehle zum Verwalten von Anwendung und Diensten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-900">Add new commands to manage appliaction and services.</span></span>

## <a name="january-13-2020"></a><span data-ttu-id="0bba9-901">13. Januar 2020</span><span class="sxs-lookup"><span data-stu-id="0bba9-901">January 13, 2020</span></span>

<span data-ttu-id="0bba9-902">Version 2.0.80</span><span class="sxs-lookup"><span data-stu-id="0bba9-902">Version 2.0.80</span></span>

### <a name="compute"></a><span data-ttu-id="0bba9-903">Compute</span><span class="sxs-lookup"><span data-stu-id="0bba9-903">Compute</span></span>

* <span data-ttu-id="0bba9-904">Datenträgeraktualisierung: „--disk-encryption-set“ und „--encryption-type“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-904">disk update: Add --disk-encryption-set and --encryption-type</span></span>
* <span data-ttu-id="0bba9-905">Momentaufnahmeerstellung/-aktualisierung: „--disk-encryption-set“ und „--encryption-type“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-905">snapshot create/update: Add --disk-encryption-set and --encryption-type</span></span>

### <a name="storage"></a><span data-ttu-id="0bba9-906">Storage</span><span class="sxs-lookup"><span data-stu-id="0bba9-906">Storage</span></span>

* <span data-ttu-id="0bba9-907">„azure-mgmt-storage“ auf Version 7.1.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-907">Upgrade azure-mgmt-storage version to 7.1.0</span></span>
* <span data-ttu-id="0bba9-908">`az storage account create`: `--encryption-key-type-for-table` und `--encryption-key-type-for-queue` zur Unterstützung des Tabellen- und Warteschlangenverschlüsselungsdiensts hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-908">`az storage account create`: Add `--encryption-key-type-for-table` and `--encryption-key-type-for-queue` to support Table and Queue Encryption Service</span></span>

## <a name="january-07-2020"></a><span data-ttu-id="0bba9-909">7\. Januar 2020</span><span class="sxs-lookup"><span data-stu-id="0bba9-909">January 07, 2020</span></span>

<span data-ttu-id="0bba9-910">Version 2.0.79</span><span class="sxs-lookup"><span data-stu-id="0bba9-910">Version 2.0.79</span></span>

### <a name="acr"></a><span data-ttu-id="0bba9-911">ACR</span><span class="sxs-lookup"><span data-stu-id="0bba9-911">ACR</span></span>

* <span data-ttu-id="0bba9-912">[BREAKING CHANGE] Parameter „--os“ für „acr build“, „acr task create/update“, „acr run“ und „acr pack“ wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-912">[BREAKING CHANGE] Remove '--os' parameter for 'acr build', 'acr task create/update', 'acr run', and 'acr pack'.</span></span> <span data-ttu-id="0bba9-913">Verwenden Sie stattdessen „--platform“.</span><span class="sxs-lookup"><span data-stu-id="0bba9-913">Use '--platform' instead.</span></span>

### <a name="appconfig"></a><span data-ttu-id="0bba9-914">AppConfig</span><span class="sxs-lookup"><span data-stu-id="0bba9-914">AppConfig</span></span>

* <span data-ttu-id="0bba9-915">Unterstützung für das Importieren/Exportieren von Featureflags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-915">Add support for importing/exporting feature flags</span></span>
* <span data-ttu-id="0bba9-916">Neuer Befehl „az appconfig kv set-keyvault“ für das Erstellen einer KeyVault-Referenz hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-916">Add new command 'az appconfig kv set-keyvault' for creating keyvault reference</span></span>
* <span data-ttu-id="0bba9-917">Unterstützung verschiedener Benennungskonventionen beim Exportieren von Featureflags in eine Datei</span><span class="sxs-lookup"><span data-stu-id="0bba9-917">Support various naming conventions when exporting feature flags to file</span></span>

### <a name="appservice"></a><span data-ttu-id="0bba9-918">AppService</span><span class="sxs-lookup"><span data-stu-id="0bba9-918">AppService</span></span>

* <span data-ttu-id="0bba9-919">Behebung von Problem Nr. 7154: Aktualisierung der Dokumentation für Befehl „<>“, sodass Backticks anstelle von einfachen Anführungszeichen verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="0bba9-919">Fix issue #7154: Updating documentation for command <> to use back ticks instead of single quotes</span></span>
* <span data-ttu-id="0bba9-920">Behebung von Problem Nr. 11287: „webapp up“: Für die mit „up“ erstellte App muss standardmäßig SSL aktiviert sein.</span><span class="sxs-lookup"><span data-stu-id="0bba9-920">Fix issue #11287: webapp up: By default make the app created using up 'should be 'SSL enabled'</span></span>
* <span data-ttu-id="0bba9-921">Behebung von Problem Nr. 11592: Flag „az webapp up“ für statische HTML-Websites hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-921">Fix issue #11592: Add az webapp up flag for html static sites</span></span>

### <a name="arm"></a><span data-ttu-id="0bba9-922">ARM</span><span class="sxs-lookup"><span data-stu-id="0bba9-922">ARM</span></span>

* <span data-ttu-id="0bba9-923">Behebung `az resource tag`: Recovery Services-Tresor-Tags können nicht aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="0bba9-923">Fix `az resource tag`: Recovery Services Vault tags cannot be updated</span></span>

### <a name="backup"></a><span data-ttu-id="0bba9-924">Backup</span><span class="sxs-lookup"><span data-stu-id="0bba9-924">Backup</span></span>

* <span data-ttu-id="0bba9-925">Neuer Befehl „backup protection undelete“ hinzugefügt, um die Funktion zum vorläufigen Löschen für IaasVM-Workloads zu aktivieren</span><span class="sxs-lookup"><span data-stu-id="0bba9-925">Added new command 'backup protection undelete' to enable soft-delete feature for IaasVM workload</span></span>
* <span data-ttu-id="0bba9-926">Neuer Parameter „--soft-delete-feature-state“ hinzugefügt, um den Befehl „backup-properties“ festzulegen</span><span class="sxs-lookup"><span data-stu-id="0bba9-926">Added new parameter '--soft-delete-feature-state' to set backup-properties command</span></span>
* <span data-ttu-id="0bba9-927">Unterstützung für den Ausschluss von Datenträgern für IaasVM-Workload hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-927">Added disk exclusion support for IaasVM workload</span></span>

### <a name="compute"></a><span data-ttu-id="0bba9-928">Compute</span><span class="sxs-lookup"><span data-stu-id="0bba9-928">Compute</span></span>

* <span data-ttu-id="0bba9-929">Fehler `vm create` in Azure Stack-Profil behoben.</span><span class="sxs-lookup"><span data-stu-id="0bba9-929">Fix `vm create` failure in Azure Stack profile.</span></span>
* <span data-ttu-id="0bba9-930">vm monitor metrics tail/list-definitions: Unterstützung einer Abfragemetrik und von Listendefinitionen für eine VM.</span><span class="sxs-lookup"><span data-stu-id="0bba9-930">vm monitor metrics tail/list-definitions: support query metric and list definitions for a vm.</span></span>
* <span data-ttu-id="0bba9-931">Neue Aktion des Befehls zum erneuten Anwenden für „az vm“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-931">Add new reapply command action for az vm</span></span>

### <a name="hdinsight"></a><span data-ttu-id="0bba9-932">HDInsight</span><span class="sxs-lookup"><span data-stu-id="0bba9-932">HDInsight</span></span>

* <span data-ttu-id="0bba9-933">Unterstützung für das Erstellen eines Kafka-Clusters mit Kafka-REST-Proxy</span><span class="sxs-lookup"><span data-stu-id="0bba9-933">Support for creating a Kafka cluster with Kafka Rest Proxy</span></span>
* <span data-ttu-id="0bba9-934">„azure-mgmt-hdinsight“ auf 1.3.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-934">Upgrade azure-mgmt-hdinsight to 1.3.0</span></span>

### <a name="misc"></a><span data-ttu-id="0bba9-935">Verschiedenes:</span><span class="sxs-lookup"><span data-stu-id="0bba9-935">Misc.</span></span>

* <span data-ttu-id="0bba9-936">Vorschaubefehl `az version show` hinzugefügt, um die Versionen der Azure CLI-Module und Erweiterungen standardmäßig im JSON-Format oder im mit „--output“ konfigurierten Format anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="0bba9-936">Add preview command `az version show` to show the versions of Azure CLI modules and extensions in JSON format by default or format configured by --output</span></span>

### <a name="event-hubs"></a><span data-ttu-id="0bba9-937">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="0bba9-937">Event Hubs</span></span>

* <span data-ttu-id="0bba9-938">[BREAKING CHANGE] Statusoption „ReceiveDisabled“ aus „az eventhubs eventhub update“ und „az eventhubs eventhub create“ entfernt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-938">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az eventhubs eventhub update' and 'az eventhubs eventhub create'.</span></span> <span data-ttu-id="0bba9-939">Diese Option ist für Event Hub-Entitäten nicht gültig.</span><span class="sxs-lookup"><span data-stu-id="0bba9-939">This option is not valid for Event Hub entities.</span></span>

### <a name="service-bus"></a><span data-ttu-id="0bba9-940">Service Bus</span><span class="sxs-lookup"><span data-stu-id="0bba9-940">Service Bus</span></span>

* <span data-ttu-id="0bba9-941">[BREAKING CHANGE] Statusoption „ReceiveDisabled“ aus Befehlen „az servicebus topic create“, „az servicebus topic update“, „az servicebus queue create“ und „az servicebus queue update“ entfernt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-941">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az servicebus topic create', 'az servicebus topic update', 'az servicebus queue create', and 'az servicebus queue update'.</span></span> <span data-ttu-id="0bba9-942">Diese Option ist für Service Bus-Themen und -Warteschlangen nicht gültig.</span><span class="sxs-lookup"><span data-stu-id="0bba9-942">This option is not valid for Service Bus topics and queues.</span></span>

### <a name="rbac"></a><span data-ttu-id="0bba9-943">RBAC</span><span class="sxs-lookup"><span data-stu-id="0bba9-943">RBAC</span></span>

* <span data-ttu-id="0bba9-944">Behebung Nr. 11712: `az ad app/sp show` gibt nicht den Exitcode 3 zurück, wenn die Anwendung oder der Dienstprinzipal nicht vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="0bba9-944">Fix #11712: `az ad app/sp show` does not return exit code 3 when the application or service principal does not exist</span></span>

### <a name="storage"></a><span data-ttu-id="0bba9-945">Storage</span><span class="sxs-lookup"><span data-stu-id="0bba9-945">Storage</span></span>

* <span data-ttu-id="0bba9-946">`az storage account create`: Vorschaukennzeichnung für Parameter „--enable-hierarchical-namespace“ entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-946">`az storage account create`: Remove preview flag for --enable-hierarchical-namespace parameter</span></span>
* <span data-ttu-id="0bba9-947">azure-mgmt-storage-Version auf 7.0.0 aktualisiert, um API-Version 2019-06-01 zu verwenden</span><span class="sxs-lookup"><span data-stu-id="0bba9-947">Update azure-mgmt-storage version to 7.0.0 to use api version 2019-06-01</span></span>
* <span data-ttu-id="0bba9-948">Neue Parameter `--enable-delete-retention` und `--delete-retention-days` hinzugefügt, um die Verwaltung der Aufbewahrungsrichtlinie für Löschen für „blob-service-properties“ von Speicherkonten zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="0bba9-948">Add new parameters `--enable-delete-retention` and `--delete-retention-days` to support managing delete retention policy for storage account blob-service-properties.</span></span>

## <a name="december-17-2019"></a><span data-ttu-id="0bba9-949">17. Dezember 2019</span><span class="sxs-lookup"><span data-stu-id="0bba9-949">December 17, 2019</span></span>

<span data-ttu-id="0bba9-950">2.0.78</span><span class="sxs-lookup"><span data-stu-id="0bba9-950">2.0.78</span></span>

### <a name="acr"></a><span data-ttu-id="0bba9-951">ACR</span><span class="sxs-lookup"><span data-stu-id="0bba9-951">ACR</span></span>

* <span data-ttu-id="0bba9-952">Unterstützung für lokalen Kontext in „acr task run“</span><span class="sxs-lookup"><span data-stu-id="0bba9-952">Added support Local context in acr task run</span></span>

### <a name="acs"></a><span data-ttu-id="0bba9-953">ACS</span><span class="sxs-lookup"><span data-stu-id="0bba9-953">ACS</span></span>

* <span data-ttu-id="0bba9-954">[BREAKING CHANGE] az openshift create: `--workspace-resource-id` in `--workspace-id` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-954">[BREAKING CHANGE]az openshift create: rename `--workspace-resource-id` to `--workspace-id`.</span></span>

### <a name="ams"></a><span data-ttu-id="0bba9-955">AMS</span><span class="sxs-lookup"><span data-stu-id="0bba9-955">AMS</span></span>

* <span data-ttu-id="0bba9-956">Befehle zum Anzeigen aktualisiert, sodass 3 zurückgegeben wird, wenn die Ressource nicht gefunden wurde</span><span class="sxs-lookup"><span data-stu-id="0bba9-956">Updated show commands to return 3 when resource not found</span></span>

### <a name="appconfig"></a><span data-ttu-id="0bba9-957">AppConfig</span><span class="sxs-lookup"><span data-stu-id="0bba9-957">AppConfig</span></span>

* <span data-ttu-id="0bba9-958">Fehler beim Anhängen der API-Version an die Anforderungs-URL korrigiert.</span><span class="sxs-lookup"><span data-stu-id="0bba9-958">Fixed bug when appending api-version to request url.</span></span> <span data-ttu-id="0bba9-959">Die vorhandene Lösung funktioniert nicht mit Paginierung.</span><span class="sxs-lookup"><span data-stu-id="0bba9-959">The existing solution doesn't work with pagination.</span></span>
* <span data-ttu-id="0bba9-960">Unterstützung für die Anzeige von weiteren Sprachen neben Englisch hinzugefügt, da der Back-End-Dienst Unicode für die Globalisierung unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-960">Added support for showing languages besides English as our backend service support unicode for globalization.</span></span>

### <a name="appservice"></a><span data-ttu-id="0bba9-961">AppService</span><span class="sxs-lookup"><span data-stu-id="0bba9-961">AppService</span></span>

* <span data-ttu-id="0bba9-962">Problem Nr. 11217 behoben: Web-App: „az webapp config ssl upload“ muss Slot-Parameter unterstützen.</span><span class="sxs-lookup"><span data-stu-id="0bba9-962">Fixed issue #11217: webapp: az webapp config ssl upload should support slot parameter</span></span>
* <span data-ttu-id="0bba9-963">Problem Nr. 10965 behoben: Error: Der Name darf nicht leer sein.</span><span class="sxs-lookup"><span data-stu-id="0bba9-963">Fixed issue #10965: Error: Name cannot be empty.</span></span> <span data-ttu-id="0bba9-964">Entfernen anhand von „ip_address“ und „subnet“ zulassen</span><span class="sxs-lookup"><span data-stu-id="0bba9-964">Allow remove by ip_address and subnet</span></span>
* <span data-ttu-id="0bba9-965">Unterstützung des Imports von Zertifikaten aus Key Vault hinzugefügt `az webapp config ssl import`</span><span class="sxs-lookup"><span data-stu-id="0bba9-965">Added support for importing certificates from Key Vault `az webapp config ssl import`</span></span>

### <a name="arm"></a><span data-ttu-id="0bba9-966">ARM</span><span class="sxs-lookup"><span data-stu-id="0bba9-966">ARM</span></span>

* <span data-ttu-id="0bba9-967">Paket „azure-mgmt-resource“ auf die Verwendung von 6.0.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-967">Updated azure-mgmt-resource package to use 6.0.0</span></span>
* <span data-ttu-id="0bba9-968">Mandantenübergreifende Unterstützung für Befehl `az group deployment create` durch Hinzufügen des neuen Parameters `--aux-subs`</span><span class="sxs-lookup"><span data-stu-id="0bba9-968">Cross Tenant Support for `az group deployment create` command by adding new parameter `--aux-subs`</span></span>
* <span data-ttu-id="0bba9-969">Neuer Parameter `--metadata` hinzugefügt, um das Hinzufügen von Metadateninformationen für Richtliniensatzdefinitionen zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="0bba9-969">Added new parameter `--metadata` to support adding metadata information for policy set definitions.</span></span>

### <a name="backup"></a><span data-ttu-id="0bba9-970">Backup</span><span class="sxs-lookup"><span data-stu-id="0bba9-970">Backup</span></span>

* <span data-ttu-id="0bba9-971">Unterstützung der Sicherung für SQL- und SAP Hana-Workloads hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-971">Added Backup support for SQL and SAP Hana workload.</span></span>

### <a name="botservice"></a><span data-ttu-id="0bba9-972">BotService</span><span class="sxs-lookup"><span data-stu-id="0bba9-972">BotService</span></span>

* <span data-ttu-id="0bba9-973">[Breaking Change] Flag „--version“ aus Vorschaubefehl „az bot create“ entfernt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-973">[Breaking change] Remove '--version' flag from preview command 'az bot create'.</span></span> <span data-ttu-id="0bba9-974">Nur v4-SDK-Bots werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-974">Only v4 SDK bots are supported.</span></span>
* <span data-ttu-id="0bba9-975">Überprüfung der Namensverfügbarkeit für „az bot create“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-975">Added name availability check for 'az bot create'.</span></span>
* <span data-ttu-id="0bba9-976">Unterstützung für das Aktualisieren der Symbol-URL für einen Bot über „az bot update“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-976">Added support for updating the icon URL for a bot via 'az bot update'.</span></span>
* <span data-ttu-id="0bba9-977">Unterstützung für das Aktualisieren eines Direct Line-Kanals über „az bot directline update“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-977">Added support for updating a Direct Line channel via 'az bot directline update'.</span></span>
* <span data-ttu-id="0bba9-978">Unterstützung für Flag „--enable-enhanced-auth“ zu „az bot directline create“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-978">Added '--enable-enhanced-auth' flag support to 'az bot directline create'.</span></span>
* <span data-ttu-id="0bba9-979">Die folgenden Befehlsgruppen sind allgemein verfügbar und befinden sich nicht in der Vorschau: „az bot authsetting“.</span><span class="sxs-lookup"><span data-stu-id="0bba9-979">The following command groups are GA and not in preview: 'az bot authsetting'.</span></span>
* <span data-ttu-id="0bba9-980">Die folgenden Befehle in „az bot“ sind allgemein verfügbar und befinden sich nicht in der Vorschau: „create“, „prepare-deploy“, „show“, „delete“, „update“.</span><span class="sxs-lookup"><span data-stu-id="0bba9-980">The following commands in 'az bot' are GA and not in preview: 'create', 'prepare-deploy', 'show', 'delete', 'update'.</span></span>
* <span data-ttu-id="0bba9-981">„az bot prepare-deploy“ korrigiert, indem der Wert voon „--proj-file-path“ in Kleinschreibung geändert wurde (z. B. „Test.csproj“ in „test.csproj“).</span><span class="sxs-lookup"><span data-stu-id="0bba9-981">Fixed 'az bot prepare-deploy' changing '--proj-file-path' value to lower case (e.g. "Test.csproj" to "test.csproj").</span></span>

### <a name="compute"></a><span data-ttu-id="0bba9-982">Compute</span><span class="sxs-lookup"><span data-stu-id="0bba9-982">Compute</span></span>

* <span data-ttu-id="0bba9-983">vmss create/update: „--scale-in-policy“ hinzugefügt, womit entschieden wird, welche virtuellen Computer beim horizontalen Herunterskalieren einer VM-Skalierungsgruppe zum Entfernen ausgewählt werden.</span><span class="sxs-lookup"><span data-stu-id="0bba9-983">vmss create/update: Added --scale-in-policy, which decides which virtual machines are chosen for removal when a VMSS is scaled-in.</span></span>
* <span data-ttu-id="0bba9-984">vm/vmss update: „--priority“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-984">vm/vmss update: Added --priority.</span></span>
* <span data-ttu-id="0bba9-985">vm/vmss update: „--max-price“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-985">vm/vmss update: Added --max-price.</span></span>
* <span data-ttu-id="0bba9-986">Befehlsgruppe „disk-encryption-set“ hinzugefügt (create, show, update, delete, list).</span><span class="sxs-lookup"><span data-stu-id="0bba9-986">Added disk-encryption-set command group (create, show, update, delete, list).</span></span>
* <span data-ttu-id="0bba9-987">disk create: „--encryption-type“ und „--disk-encryption-set“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-987">disk create: Added --encryption-type and --disk-encryption-set.</span></span>
* <span data-ttu-id="0bba9-988">vm/vmss create: „--os-disk-encryption-set“ und „--data-disk-encryption-sets“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-988">vm/vmss create: Added --os-disk-encryption-set and --data-disk-encryption-sets.</span></span>

### <a name="core"></a><span data-ttu-id="0bba9-989">Core</span><span class="sxs-lookup"><span data-stu-id="0bba9-989">Core</span></span>

* <span data-ttu-id="0bba9-990">Unterstützung für Python 3.4 entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-990">Removed support for Python 3.4</span></span>
* <span data-ttu-id="0bba9-991">Plug-In für HaTS-Umfrage in mehreren Befehlen</span><span class="sxs-lookup"><span data-stu-id="0bba9-991">Plug in HaTS survey in multiple commands</span></span>

### <a name="dls"></a><span data-ttu-id="0bba9-992">DLS</span><span class="sxs-lookup"><span data-stu-id="0bba9-992">DLS</span></span>

* <span data-ttu-id="0bba9-993">ADLS-SDK-Version aktualisiert (0.0.48).</span><span class="sxs-lookup"><span data-stu-id="0bba9-993">Updated ADLS sdk version (0.0.48).</span></span>

### <a name="install"></a><span data-ttu-id="0bba9-994">Installieren</span><span class="sxs-lookup"><span data-stu-id="0bba9-994">Install</span></span>

* <span data-ttu-id="0bba9-995">Installationsskript unterstützt Python 3.8</span><span class="sxs-lookup"><span data-stu-id="0bba9-995">Install script support python 3.8</span></span>

### <a name="iot"></a><span data-ttu-id="0bba9-996">IoT</span><span class="sxs-lookup"><span data-stu-id="0bba9-996">IOT</span></span>

* <span data-ttu-id="0bba9-997">[BREAKING CHANGE] Parameter „--failover-region“ aus „manual-failover“ entfernt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-997">[BREAKING CHANGE] Removed --failover-region parameter from manual-failover.</span></span> <span data-ttu-id="0bba9-998">Das Failover erfolgt jetzt in eine zugewiesene, geografisch gekoppelte sekundäre Region.</span><span class="sxs-lookup"><span data-stu-id="0bba9-998">Now it will failover to assigned geo-paired secondary region.</span></span>

### <a name="key-vault"></a><span data-ttu-id="0bba9-999">Key Vault</span><span class="sxs-lookup"><span data-stu-id="0bba9-999">Key Vault</span></span>

* <span data-ttu-id="0bba9-1000">Nr. 8095 behoben: `az keyvault storage remove`: Hilfemeldung verbessert</span><span class="sxs-lookup"><span data-stu-id="0bba9-1000">Fixed #8095: `az keyvault storage remove`: improve the help message</span></span>
* <span data-ttu-id="0bba9-1001">Nr. 8921 behoben: `az keyvault key/secret/certificate list/list-deleted/list-versions`: Validierungsfehler in Parameter `--maxresults` behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-1001">Fixed #8921: `az keyvault key/secret/certificate list/list-deleted/list-versions`: fix the validation bug on parameter `--maxresults`</span></span>
* <span data-ttu-id="0bba9-1002">Nr. 10512 behoben: `az keyvault set-policy`: Fehlermeldung verbessert, wenn weder `--object-id`, `--spn` noch `--upn` angegeben ist</span><span class="sxs-lookup"><span data-stu-id="0bba9-1002">Fixed #10512: `az keyvault set-policy`: improve the error message when none of `--object-id`, `--spn` or `--upn` is specified</span></span>
* <span data-ttu-id="0bba9-1003">Nr. 10846 behoben: `az keyvault secret show-deleted`: Wenn `--id` angegeben ist, ist `--name/-n` nicht erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1003">Fixed #10846: `az keyvault secret show-deleted`: when `--id` is specified, `--name/-n` is not required</span></span>
* <span data-ttu-id="0bba9-1004">Nr. 11084 behoben: `az keyvault secret download`: Hilfemeldung von Parameter `--encoding` verbessert</span><span class="sxs-lookup"><span data-stu-id="0bba9-1004">Fixed #11084: `az keyvault secret download`: improve the help message of parameter `--encoding`</span></span>

### <a name="network"></a><span data-ttu-id="0bba9-1005">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0bba9-1005">Network</span></span>

* <span data-ttu-id="0bba9-1006">az network application-gateway probe: Unterstützung für Option „--port“ hinzugefügt, um einen Port zum Prüfen von Back-End-Servern beim Erstellen und Aktualisieren anzugeben</span><span class="sxs-lookup"><span data-stu-id="0bba9-1006">az network application-gateway probe: Added support --port option to specify a port for probing backend servers when create and update</span></span>
* <span data-ttu-id="0bba9-1007">az network application-gateway url-path-map create/update: Fehlerbehebung für `--waf-policy`</span><span class="sxs-lookup"><span data-stu-id="0bba9-1007">az network application-gateway url-path-map create/update: bug fix for `--waf-policy`</span></span>
* <span data-ttu-id="0bba9-1008">az network application-gateway: Unterstützung für `--rewrite-rule-set` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1008">az network application-gateway: Added support `--rewrite-rule-set`</span></span>
* <span data-ttu-id="0bba9-1009">az network list-service-aliases: Unterstützung für Listendienstaliase hinzugefügt, die für Dienstendpunktrichtlinien verwendet werden können</span><span class="sxs-lookup"><span data-stu-id="0bba9-1009">az network list-service-aliases: Added support list service aliases which can be used for Service Endpoint Policies</span></span>
* <span data-ttu-id="0bba9-1010">az network dns zone import: Unterstützung für „.@“ in Datensatzname hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1010">az network dns zone import: Added support .@ in record name</span></span>

### <a name="packaging"></a><span data-ttu-id="0bba9-1011">Verpackung</span><span class="sxs-lookup"><span data-stu-id="0bba9-1011">Packaging</span></span>

* <span data-ttu-id="0bba9-1012">Back-Edge-Builds für PIP-Installation hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1012">Added back edge builds for pip install</span></span>
* <span data-ttu-id="0bba9-1013">Ubuntu-Eoan-Paket hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1013">Added Ubuntu eoan package</span></span>

### <a name="policy"></a><span data-ttu-id="0bba9-1014">Richtlinie</span><span class="sxs-lookup"><span data-stu-id="0bba9-1014">Policy</span></span>

* <span data-ttu-id="0bba9-1015">Unterstützung für Version 2019-09-01 der Richtlinien-API hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1015">Added support for Policy API version 2019-09-01.</span></span>
* <span data-ttu-id="0bba9-1016">az policy set-definition: Unterstützung der Gruppierung innerhalb von Richtliniensatzdefinitionen mit `--definition-groups`-Parameter hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1016">az policy set-definition: Added support grouping within policy set definitions with `--definition-groups` parameter</span></span>

### <a name="redis"></a><span data-ttu-id="0bba9-1017">Redis</span><span class="sxs-lookup"><span data-stu-id="0bba9-1017">Redis</span></span>

* <span data-ttu-id="0bba9-1018">Vorschauparameter `--replicas-per-master` zu Befehl `az redis create`hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1018">Added preview param `--replicas-per-master` to `az redis create` command</span></span>
* <span data-ttu-id="0bba9-1019">„azure-mgmt-redis“ von 6.0.0 auf 7.0.0rc1 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-1019">Updated azure-mgmt-redis from 6.0.0 to 7.0.0rc1</span></span>

### <a name="servicefabric"></a><span data-ttu-id="0bba9-1020">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="0bba9-1020">ServiceFabric</span></span>

* <span data-ttu-id="0bba9-1021">Hinzufügen von Logik in Knotentyp korrigiert, einschließlich Nr. 10963: Beim Hinzufügen eines neuen Knotentyps mit Dauerhaftigkeitsstufe „Gold“ wird immer ein CLI-Fehler ausgegeben.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1021">Fixed in node-type add logic including #10963: Adding new node type with durability level Gold will always throw CLI error</span></span>
* <span data-ttu-id="0bba9-1022">ServiceFabricNodeVmExt-Version in Erstellungsvorlage auf 1.1 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-1022">Updated ServiceFabricNodeVmExt version to 1.1 in creation template</span></span>

### <a name="sql"></a><span data-ttu-id="0bba9-1023">SQL</span><span class="sxs-lookup"><span data-stu-id="0bba9-1023">SQL</span></span>

* <span data-ttu-id="0bba9-1024">Parameter „--read-scale“ und „--read-replicas“ zu Befehlen „sql db create“ und „sql db update“ hinzugefügt, um Leseskalierungsverwaltung zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1024">Added "--read-scale" and "--read-replicas" parameters to sql db create and update commands, to support read scale management.</span></span>

### <a name="storage"></a><span data-ttu-id="0bba9-1025">Storage</span><span class="sxs-lookup"><span data-stu-id="0bba9-1025">Storage</span></span>

* <span data-ttu-id="0bba9-1026">Allgemein verfügbares Release – Eigenschaft „Large File Shares“ für Befehle „storage account create“ und „storage account update“</span><span class="sxs-lookup"><span data-stu-id="0bba9-1026">GA Release Large File Shares property for storage account create and update command</span></span>
* <span data-ttu-id="0bba9-1027">Allgemein verfügbares Release – Unterstützung von SAS-Token für die Benutzerdelegierung</span><span class="sxs-lookup"><span data-stu-id="0bba9-1027">GA Release User Delegation SAS token Support</span></span>
* <span data-ttu-id="0bba9-1028">Neue Befehle `az storage account blob-service-properties show` und `az storage account blob-service-properties update --enable-change-feed` hinzugefügt, um Blob-Diensteigenschaften für das Speicherkonto zu verwalten.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1028">Added new commands `az storage account blob-service-properties show` and `az storage account blob-service-properties update --enable-change-feed` to manage blob service properties for storage account.</span></span>
* <span data-ttu-id="0bba9-1029">[BEVORSTEHENDER BREAKING CHANGE] `az storage copy`: Das Zeichen `*` wird nicht mehr als Platzhalter in der URL, es werden jedoch die neuen Parameter „--include-pattern“ und „--exclude-pattern“ mit Unterstützung des Platzhalters `*` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1029">[COMING BREAKING CHANGE] `az storage copy`: `*` character is no longer supported as a wildcard in URL, but new parameters --include-pattern and --exclude-pattern will be added with `*` wildcard support.</span></span>
* <span data-ttu-id="0bba9-1030">Problem Nr. 11043 behoben: Unterstützung für das Entfernen des gesamten Containers/der gesamten Freigabe in `az storage remove` Befehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1030">Fixed issue #11043: Added support to remove whole container/share in `az storage remove` command</span></span>

## <a name="november-26-2019"></a><span data-ttu-id="0bba9-1031">26. November 2019</span><span class="sxs-lookup"><span data-stu-id="0bba9-1031">November 26, 2019</span></span>

<span data-ttu-id="0bba9-1032">Version 2.0.77</span><span class="sxs-lookup"><span data-stu-id="0bba9-1032">Version 2.0.77</span></span>

### <a name="acr"></a><span data-ttu-id="0bba9-1033">ACR</span><span class="sxs-lookup"><span data-stu-id="0bba9-1033">ACR</span></span>

* <span data-ttu-id="0bba9-1034">Parameter `--branch` in „acr task create/update“ als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-1034">Deprecated parameter `--branch` from acr task create/update</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="0bba9-1035">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="0bba9-1035">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="0bba9-1036">`--workspace-resource-id`-Flag hinzugefügt, um die Erstellung eines Azure Red Hat OpenShift-Clusters mit Überwachung zuzulassen</span><span class="sxs-lookup"><span data-stu-id="0bba9-1036">Added `--workspace-resource-id` flag to allow creation of Azure Red Hat Openshift cluster with monitoring</span></span>
* <span data-ttu-id="0bba9-1037">`monitor_profile`-Flag hinzugefügt, um einen Azure Red Hat OpenShift-Clusters mit Überwachung zu erstellen</span><span class="sxs-lookup"><span data-stu-id="0bba9-1037">Added `monitor_profile` to create Azure Red Hat OpenShift cluster with monitoring</span></span>

### <a name="aks"></a><span data-ttu-id="0bba9-1038">AKS</span><span class="sxs-lookup"><span data-stu-id="0bba9-1038">AKS</span></span>

* <span data-ttu-id="0bba9-1039">Unterstützung des Rotationsvorgangs für Clusterzertifikate mithilfe von für Cluster Zertifikat Rotation mit „az aks rotate-certs“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1039">Added support cluster certificate rotation operation using "az aks rotate-certs".</span></span>

### <a name="appconfig"></a><span data-ttu-id="0bba9-1040">AppConfig</span><span class="sxs-lookup"><span data-stu-id="0bba9-1040">AppConfig</span></span>

* <span data-ttu-id="0bba9-1041">Unterstützung für die Verwendung von „:“ für `as az appconfig kv import`-Trennzeichen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1041">Added support for using ":" for `as az appconfig kv import` separator</span></span>
* <span data-ttu-id="0bba9-1042">Problem beim Auflisten von Schlüsselwerten mit mehreren Bezeichnungen, einschließlich NULL-Bezeichnung, behoben.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1042">Fixed issue for listing key values with multiple labels including null label.</span></span> 
* <span data-ttu-id="0bba9-1043">Verwaltungsebenen-SDK, „azure-mgmt-appconfiguration“, auf Version 0.3.0 aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1043">Updated management plane sdk, azure-mgmt-appconfiguration, to version 0.3.0.</span></span> 

### <a name="appservice"></a><span data-ttu-id="0bba9-1044">AppService</span><span class="sxs-lookup"><span data-stu-id="0bba9-1044">AppService</span></span>

* <span data-ttu-id="0bba9-1045">Problem Nr. 11100 behoben AttributeError für „az webapp up“ beim Erstellen eines Dienstplans</span><span class="sxs-lookup"><span data-stu-id="0bba9-1045">Fixed issue #11100: AttributeError for az webapp up when create service plan</span></span>
* <span data-ttu-id="0bba9-1046">az webapp up: Erzwingen der Erstellung oder Bereitstellung auf einer Website für unterstützte Sprachen, es werden keine Standardeinstellungen verwendet.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1046">az webapp up: Forcing the creation or deployment to a site for supported languages, no defaults used.</span></span>
* <span data-ttu-id="0bba9-1047">Unterstützung für App Service-Umgebung hinzugefügt: az appservice ase show | list | list-addresses | list-plans | create | update | delete</span><span class="sxs-lookup"><span data-stu-id="0bba9-1047">Added support for App Service Environment: az appservice ase show | list | list-addresses | list-plans | create | update | delete</span></span>

### <a name="backup"></a><span data-ttu-id="0bba9-1048">Backup</span><span class="sxs-lookup"><span data-stu-id="0bba9-1048">Backup</span></span>

* <span data-ttu-id="0bba9-1049">Problem in Az-Sicherungsrichtlinie „list-associated-items“ behoben.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1049">Fixed issue in az backup policy list-associated-items.</span></span> <span data-ttu-id="0bba9-1050">Optionaler Parameter „BackupManagementType“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1050">Added optional BackupManagementType parameter.</span></span>

### <a name="compute"></a><span data-ttu-id="0bba9-1051">Compute</span><span class="sxs-lookup"><span data-stu-id="0bba9-1051">Compute</span></span>

* <span data-ttu-id="0bba9-1052">API-Version von Compute, Datenträger, Momentaufnahmen auf 2019-07-01 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-1052">Upgraded API version of compute, disks, snapshots to 2019-07-01</span></span>
* <span data-ttu-id="0bba9-1053">vmss create: Verbesserung für – Orchestrierungsmodus</span><span class="sxs-lookup"><span data-stu-id="0bba9-1053">vmss create: Improvement for --orchestration-mode</span></span>
* <span data-ttu-id="0bba9-1054">sig image-definition create: „--os-state“ hinzugefügt, um die Angabe zu ermöglichen, ob die unter diesem Image erstellten virtuellen Computer „generalisiert“ oder „spezialisiert“ sind</span><span class="sxs-lookup"><span data-stu-id="0bba9-1054">sig image-definition create: Added --os-state to allow specifying whether the virtual machines created under this image are 'Generalized' or 'Specialized'</span></span>
* <span data-ttu-id="0bba9-1055">sig image-definition create: „--hyper-v-generation“ hinzugefügt, um die Angabe der Hypervisorgeneration zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="0bba9-1055">sig image-definition create: Added --hyper-v-generation to allow specifying the hypervisor generation</span></span>
* <span data-ttu-id="0bba9-1056">sig image-version create: Unterstützung für „--os-snapshot“ und „--data-snapshots“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1056">sig image-version create: Added support --os-snapshot and --data-snapshots</span></span>
* <span data-ttu-id="0bba9-1057">image create: „--data-disk-caching“ hinzugefügt, um die Angabe der Zwischenspeicherungseinstellung von Datenträger zu ermöflichen</span><span class="sxs-lookup"><span data-stu-id="0bba9-1057">image create: Added --data-disk-caching to allow specifying caching setting of data disks</span></span>
* <span data-ttu-id="0bba9-1058">Upgrade des Python-Compute-SDK auf 10.0.0</span><span class="sxs-lookup"><span data-stu-id="0bba9-1058">Upgraded Python Compute SDK to 10.0.0</span></span>
* <span data-ttu-id="0bba9-1059">vm/vmss create: „Spot“ zu Aufzählungseigenschaft „Priority“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1059">vm/vmss create: Added 'Spot' to 'Priority' enum property</span></span>
* <span data-ttu-id="0bba9-1060">[Breaking Change] Parameter „--max-billing“ für sowohl VM als auch VMSS in „--max-price“ umbenannt, um die Konsistenz mit Swagger- und PowerShell-Cmdlets sicherzustellen</span><span class="sxs-lookup"><span data-stu-id="0bba9-1060">[Breaking change] Renamed '--max-billing' parameter to '--max-price', for both VM and VMSS, to be consistent with Swagger and Powershell cmdlets</span></span>
* <span data-ttu-id="0bba9-1061">vm monitor log show: Unterstützung für das Abfragen von Protokollen über verknüpften Protokollanalyse-Arbeitsbereich hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1061">vm monitor log show: Added support for querying log over linked log analytics workspace.</span></span>

### <a name="iot"></a><span data-ttu-id="0bba9-1062">IoT</span><span class="sxs-lookup"><span data-stu-id="0bba9-1062">IOT</span></span>

* <span data-ttu-id="0bba9-1063">Behebung Nr. 2531: Argumente für Benutzerfreundlichkeit für Hub-Update hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1063">Fix #2531: Added convenience arguments for hub update.</span></span>
* <span data-ttu-id="0bba9-1064">Behebung Nr. 8323: Fehlende Parameter zum Erstellen eines benutzerdefinierten Speicherendpunkts hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1064">Fix #8323: Added missing parameters to create storage custom endpoint.</span></span>
* <span data-ttu-id="0bba9-1065">Regressionsfehler behoben: Die Änderungen wurden rückgängig gemacht, sodass der standardmäßige Speicherendpunkt überschrieben wurde.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1065">Fix regression bug: Reverted the changes which overrides the default storage endpoint.</span></span>

### <a name="key-vault"></a><span data-ttu-id="0bba9-1066">Key Vault</span><span class="sxs-lookup"><span data-stu-id="0bba9-1066">Key Vault</span></span>

* <span data-ttu-id="0bba9-1067">Nr. 11121 behoben: Bei der Verwendung von `az keyvault certificate list` erfordert die Übergabe von `--include-pending` jetzt nicht mehr den Wert `true` oder `false`.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1067">Fixed #11121: When using `az keyvault certificate list`, passing `--include-pending` now doesn't require a value of `true` or `false`</span></span>

### <a name="netappfiles"></a><span data-ttu-id="0bba9-1068">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="0bba9-1068">NetAppFiles</span></span>

* <span data-ttu-id="0bba9-1069">Upgrade von „azure-mgmt-netapp“ auf Version 0.7.0, die einige zusätzliche Volumeeigenschaften enthält, die bevorstehenden Replikationsvorgängen zugeordnet sind</span><span class="sxs-lookup"><span data-stu-id="0bba9-1069">Upgraded azure-mgmt-netapp to 0.7.0 which includes some additional volume properties associated with upcoming replication operations</span></span>

### <a name="network"></a><span data-ttu-id="0bba9-1070">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0bba9-1070">Network</span></span>

* <span data-ttu-id="0bba9-1071">application-gateway waf-config: veraltet</span><span class="sxs-lookup"><span data-stu-id="0bba9-1071">application-gateway waf-config: deprecated</span></span>
* <span data-ttu-id="0bba9-1072">application-gateway waf-policy: Untergruppe „managed-rules“ zur Verwaltung von verwalteten Regelsätzen und Ausschlussregeln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1072">application-gateway waf-policy: Added subgroup managed-rules to manage managed rule sets and exclusion rules</span></span>
* <span data-ttu-id="0bba9-1073">application-gateway waf-policy: Untergruppe „policy-setting“ zur Verwaltung der globalen Konfiguration von „waf-policy“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1073">application-gateway waf-policy: Added subgroup policy-setting to manage global configuration of a waf-policy</span></span>
* <span data-ttu-id="0bba9-1074">[BREAKING CHANGE] application-gateway waf-policy: Untergruppenregel in „custom-rule“ umbenannt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1074">[BREAKING CHANGE] application-gateway waf-policy: Renamed subgroup rule to custom-rule</span></span>
* <span data-ttu-id="0bba9-1075">application-gateway http-listener: „--firewall-policy“ beim Erstellen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1075">application-gateway http-listener: Added --firewall-policy when create</span></span>
* <span data-ttu-id="0bba9-1076">application-gateway url-path-map rule: „--firewall-policy“ beim Erstellen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1076">application-gateway url-path-map rule: Added --firewall-policy when create</span></span>

### <a name="packaging"></a><span data-ttu-id="0bba9-1077">Verpackung</span><span class="sxs-lookup"><span data-stu-id="0bba9-1077">Packaging</span></span>

* <span data-ttu-id="0bba9-1078">Az-Wrapper in Python neu geschrieben</span><span class="sxs-lookup"><span data-stu-id="0bba9-1078">Rewrote the az wrapper in Python</span></span>
* <span data-ttu-id="0bba9-1079">Unterstützung für Python 3.8 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1079">Added support for Python 3.8</span></span>
* <span data-ttu-id="0bba9-1080">Für RPM-Paket in Python 3 geändert</span><span class="sxs-lookup"><span data-stu-id="0bba9-1080">Changed to Python 3 for RPM package</span></span>

### <a name="profile"></a><span data-ttu-id="0bba9-1081">Profil</span><span class="sxs-lookup"><span data-stu-id="0bba9-1081">Profile</span></span>

* <span data-ttu-id="0bba9-1082">Fehler beim Ausführen von `az login -u {} -p {}` mit Microsoft-Konto entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1082">Polished error when running `az login -u {} -p {}` with Microsoft account</span></span>
* <span data-ttu-id="0bba9-1083">`SSLError` beim Ausführen von `az login` hinter einem Proxy mit einem selbstsignierten Stammzertifikat entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1083">Polished `SSLError` when running `az login` behind a proxy with self-signed root certificate</span></span>
* <span data-ttu-id="0bba9-1084">Nr. 10578 behoben: `az login` hängt, wenn mehrere Instanzen gleichzeitig unter Windows oder WSL gestartet werden.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1084">Fixed #10578: `az login` hangs when more than one instances are launched at the same time on Windows or WSL</span></span>
* <span data-ttu-id="0bba9-1085">Nr. 11059 behoben: `az login --allow-no-subscriptions` schlägt fehl, wenn Abonnements im Mandanten vorhanden sind.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1085">Fixed #11059: `az login --allow-no-subscriptions` fails if there are subscriptions in the tenant</span></span>
* <span data-ttu-id="0bba9-1086">Nr. 11238 behoben: Nach dem Umbenennen eines Abonnements führt die Anmeldung mit MSI dazu, dass das gleiche Abonnement zweimal angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1086">Fixed #11238: After renaming a subscription, logging in with MSI will result in the same subscription appearing twice</span></span>

### <a name="rbac"></a><span data-ttu-id="0bba9-1087">RBAC</span><span class="sxs-lookup"><span data-stu-id="0bba9-1087">RBAC</span></span>

* <span data-ttu-id="0bba9-1088">Nr. 10996 behoben: Fehler für `--force-change-password-next-login` in `az ad user update` entfernt, wenn `--password` nicht angegeben ist</span><span class="sxs-lookup"><span data-stu-id="0bba9-1088">Fixed #10996: Polish error for `--force-change-password-next-login` in `az ad user update` when `--password` is not specified</span></span>

### <a name="redis"></a><span data-ttu-id="0bba9-1089">Redis</span><span class="sxs-lookup"><span data-stu-id="0bba9-1089">Redis</span></span>

* <span data-ttu-id="0bba9-1090">Nr. 2902 behoben: Festlegen von Speicherkonfigurationen beim Aktualisieren des Basic-SKU-Cache vermeiden</span><span class="sxs-lookup"><span data-stu-id="0bba9-1090">Fixed #2902: Avoid setting memory configs while updating Basic SKU cache</span></span>

### <a name="reservations"></a><span data-ttu-id="0bba9-1091">Reservations</span><span class="sxs-lookup"><span data-stu-id="0bba9-1091">Reservations</span></span>

* <span data-ttu-id="0bba9-1092">SDK-Version auf 0.6.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-1092">Upgraded SDK Version to 0.6.0</span></span>
* <span data-ttu-id="0bba9-1093">Abrechnungsplandetails nach dem Aufrufen von „Get-Gatalogs“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1093">Added billingplan details info after calling Get-Gatalogs</span></span>
* <span data-ttu-id="0bba9-1094">Neuer Befehl `az reservations reservation-order calculate` zum Berechnen des Preises für eine Reservierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1094">Added new command `az reservations reservation-order calculate` to calculate the price for a reservation</span></span>
* <span data-ttu-id="0bba9-1095">Neuer Befehl `az reservations reservation-order purchase` zum Erwerb einer neuen Reservierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1095">Added new command `az reservations reservation-order purchase` to purchase a new reservation</span></span>

### <a name="rest"></a><span data-ttu-id="0bba9-1096">REST</span><span class="sxs-lookup"><span data-stu-id="0bba9-1096">Rest</span></span>
* <span data-ttu-id="0bba9-1097">`az rest` in allgemeine Verfügbarkeit geändert</span><span class="sxs-lookup"><span data-stu-id="0bba9-1097">Changed `az rest` to GA</span></span>

### <a name="sql"></a><span data-ttu-id="0bba9-1098">SQL</span><span class="sxs-lookup"><span data-stu-id="0bba9-1098">SQL</span></span>

* <span data-ttu-id="0bba9-1099">„azure-mgmt-sql“ auf Version 0.15.0 aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1099">Updated azure-mgmt-sql to version 0.15.0.</span></span>

### <a name="storage"></a><span data-ttu-id="0bba9-1100">Storage</span><span class="sxs-lookup"><span data-stu-id="0bba9-1100">Storage</span></span>

* <span data-ttu-id="0bba9-1101">storage account create: „--enable-hierarchical-namespace“ hinzugefügt, um Dateisystemsemantik in Blobdienst zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1101">storage account create: Added --enable-hierarchical-namespace to support filesystem semantics in blob service.</span></span>
* <span data-ttu-id="0bba9-1102">Ausnahme ohne Zusammenhang aus Fehlermeldung entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1102">Removed unrelated exception from error message</span></span>
* <span data-ttu-id="0bba9-1103">Probleme mit falscher Fehlermeldung „Sie verfügen nicht über die erforderlichen Berechtigungen zum Ausführen dieses Vorgangs“ behoben.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1103">Fixed issues with incorrect error message "You do not have the required permissions needed to perform this operation."</span></span> <span data-ttu-id="0bba9-1104">bei Blockierung durch Netzwerkregeln oder bei „AuthenticationFailed“.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1104">when blocked by network rules or AuthenticationFailed.</span></span>

## <a name="november-4-2019"></a><span data-ttu-id="0bba9-1105">4\. November 2019</span><span class="sxs-lookup"><span data-stu-id="0bba9-1105">November 4, 2019</span></span>

<span data-ttu-id="0bba9-1106">Version 2.0.76</span><span class="sxs-lookup"><span data-stu-id="0bba9-1106">Version 2.0.76</span></span>

### <a name="acr"></a><span data-ttu-id="0bba9-1107">ACR</span><span class="sxs-lookup"><span data-stu-id="0bba9-1107">ACR</span></span>

* <span data-ttu-id="0bba9-1108">Vorschauparameter `--pack-image-tag` wurde dem Befehl `az acr pack build` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1108">Added a preview parameter `--pack-image-tag` to command `az acr pack build`.</span></span>
* <span data-ttu-id="0bba9-1109">Unterstützung der Aktivierung der Überwachung beim Erstellen einer Registrierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1109">Added support for enabling auditing on creating a registry</span></span>
* <span data-ttu-id="0bba9-1110">Unterstützung von RBAC mit Repositoryumfang hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1110">Added support for Repository-scoped RBAC</span></span>

### <a name="aks"></a><span data-ttu-id="0bba9-1111">AKS</span><span class="sxs-lookup"><span data-stu-id="0bba9-1111">AKS</span></span>

* <span data-ttu-id="0bba9-1112">`--enable-cluster-autoscaler`, `--min-count` und `--max-count` wurden dem Befehl `az aks create` hinzugefügt, sodass die automatische Clusterskalierung für den Knotenpool aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1112">Added `--enable-cluster-autoscaler`, `--min-count` and `--max-count` to the `az aks create` command, which enables cluster autoscaler for the node pool.</span></span>
* <span data-ttu-id="0bba9-1113">Die obigen Flags sowie `--update-cluster-autoscaler` und `--disable-cluster-autoscaler` wurden dem Befehl `az aks update` hinzugefügt, sodass Updates der automatischen Clusterskalierung zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1113">Added the above flags as well as `--update-cluster-autoscaler` and `--disable-cluster-autoscaler` to the `az aks update` command, allowing updates to cluster autoscaler.</span></span>

### <a name="appconfig"></a><span data-ttu-id="0bba9-1114">AppConfig</span><span class="sxs-lookup"><span data-stu-id="0bba9-1114">AppConfig</span></span>

* <span data-ttu-id="0bba9-1115">Befehlsgruppe der AppConfig-Funktion zum Verwalten von in einer App Configuration-Instanz gespeicherten Featureflags wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1115">Added appconfig feature command group to manage feature flags stored in an App Configuration.</span></span>
* <span data-ttu-id="0bba9-1116">Geringfügiger Programmfehler für Befehl „appconfig kv export to file“ wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1116">Fixed minor bug for appconfig kv export to file command.</span></span> <span data-ttu-id="0bba9-1117">Das Lesen der Zieldateiinhalte wird während des Exports angehalten.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1117">Stop reading dest file contents during export.</span></span>

### <a name="appservice"></a><span data-ttu-id="0bba9-1118">AppService</span><span class="sxs-lookup"><span data-stu-id="0bba9-1118">AppService</span></span>

* <span data-ttu-id="0bba9-1119">`az appservice plan create`: Unterstützung für das Festlegen von „persitescalung“ beim Erstellen eines App-Serviceplans wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1119">`az appservice plan create`: Added support to set 'persitescaling' on appservice plan create.</span></span>
* <span data-ttu-id="0bba9-1120">Ein Problem wurde behoben, aufgrund dessen der Vorgang „webapp config ssl bind“ vorhandene Tags aus der Ressource entfernt hat.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1120">Fixed an issue where webapp config ssl bind operation was removing existing tags from the resource</span></span>
* <span data-ttu-id="0bba9-1121">Flag `--build-remote` wurde für `az functionapp deployment source config-zip` hinzugefügt, um die Remotebuildaktion während der Funktions-App-Bereitstellung zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1121">Added `--build-remote` flag for `az functionapp deployment source config-zip` to support remote build action during function app deployment.</span></span>
* <span data-ttu-id="0bba9-1122">Die Standardknotenversion in Funktions-Apps wurde für Windows in ~ 10 geändert.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1122">Changed default node version on function apps to ~10 for Windows</span></span>
* <span data-ttu-id="0bba9-1123">`--runtime-version`-Eigenschaft zu `az functionapp create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1123">Added `--runtime-version` property to `az functionapp create`</span></span>

### <a name="arm"></a><span data-ttu-id="0bba9-1124">ARM</span><span class="sxs-lookup"><span data-stu-id="0bba9-1124">ARM</span></span>

* <span data-ttu-id="0bba9-1125">`az deployment/group deployment validate`: Parameter `--handle-extended-json-format` wurde hinzugefügt, um bei der Bereitstellung mehrere Zeilen und Kommentare in der JSON-Vorlage zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1125">`az deployment/group deployment validate`: Added `--handle-extended-json-format` parameter to support multiline and comments in json template when deployment.</span></span>
* <span data-ttu-id="0bba9-1126">„azure-mgmt-resource“ auf „2019-07-01“ festgelegt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1126">Bumped azure-mgmt-resource to 2019-07-01</span></span>

### <a name="backup"></a><span data-ttu-id="0bba9-1127">Backup</span><span class="sxs-lookup"><span data-stu-id="0bba9-1127">Backup</span></span>

* <span data-ttu-id="0bba9-1128">Unterstützung für AzureFiles-Sicherung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1128">Added AzureFiles backup support</span></span>

### <a name="compute"></a><span data-ttu-id="0bba9-1129">Compute</span><span class="sxs-lookup"><span data-stu-id="0bba9-1129">Compute</span></span>

* <span data-ttu-id="0bba9-1130">`az vm create`: Beim gleichzeitigen Festlegen von beschleunigtem Netzwerkbetrieb und einer vorhandenen NIC wurde eine Warnung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1130">`az vm create`: Added warning when specifying accelerated networking and an existing NIC together.</span></span>
* <span data-ttu-id="0bba9-1131">`az vm create`: `--vmss` hinzugefügt, um eine vorhandene VM-Skalierungsgruppe anzugeben, welcher der virtuelle Computer zugewiesen werden soll.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1131">`az vm create`: Added `--vmss` to specify an existing virtual machine scale set that the virtual machine should be assigned to.</span></span>
* <span data-ttu-id="0bba9-1132">`az vm/vmss create`: Eine lokale Kopie der Imagealiasdatei wurde hinzugefügt, sodass in einer eingeschränkten Netzwerkumgebung darauf zugegriffen werden kann.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1132">`az vm/vmss create`: Added a local copy of image alias file so that it can be accessed in a restricted network environment.</span></span>
* <span data-ttu-id="0bba9-1133">`az vmss create`: `--orchestration-mode` hinzugefügt, um anzugeben, wie virtuelle Computer von der Skalierungsgruppe verwaltet werden.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1133">`az vmss create`: Added `--orchestration-mode` to specify how virtual machines are managed by the scale set.</span></span>
* <span data-ttu-id="0bba9-1134">`az vm/vmss update`: `--ultra-ssd-enabled` hinzugefügt, um das Aktualisieren der SSD-Einstellung zuzulassen.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1134">`az vm/vmss update`: Added `--ultra-ssd-enabled` to allow updating ultra SSD setting.</span></span>
* <span data-ttu-id="0bba9-1135">[BREAKING CHANGE] `az vm extension set`: Ein Fehler wurde behoben, aufgrund dessen Benutzer mit `--ids` keine Erweiterung auf einem virtuellen Computer festlegen konnten.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1135">[BREAKING CHANGE] `az vm extension set`: Fixed bug where users could not set an extension on a VM with `--ids`.</span></span>
* <span data-ttu-id="0bba9-1136">Neue Befehle wurden zu `az vm image terms accept/cancel/show` hinzugefügt , um Azure Marketplace-Imagebedingungen zu verwalten.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1136">Added new commands `az vm image terms accept/cancel/show` to manage Azure Marketplace image terms.</span></span>
* <span data-ttu-id="0bba9-1137">VMAccessForLinux auf Version 1.5 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-1137">Updated VMAccessForLinux to version 1.5</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="0bba9-1138">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="0bba9-1138">CosmosDB</span></span>

* <span data-ttu-id="0bba9-1139">[BREAKING CHANGE] `az sql container create`: `--partition-key-path` in erforderlichen Parameter geändert</span><span class="sxs-lookup"><span data-stu-id="0bba9-1139">[BREAKING CHANGE] `az sql container create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="0bba9-1140">[BREAKING CHANGE] `az gremlin graph create`: `--partition-key-path` in erforderlichen Parameter geändert</span><span class="sxs-lookup"><span data-stu-id="0bba9-1140">[BREAKING CHANGE] `az gremlin graph create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="0bba9-1141">`az sql container create`: `--unique-key-policy` und `--conflict-resolution-policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1141">`az sql container create`: Added `--unique-key-policy` and `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="0bba9-1142">`az sql container create/update`: Aktualisierung des `--idx`-Standardschemas</span><span class="sxs-lookup"><span data-stu-id="0bba9-1142">`az sql container create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="0bba9-1143">`gremlin graph create`: `--conflict-resolution-policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1143">`gremlin graph create`: Added `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="0bba9-1144">`gremlin graph create/update`: Aktualisierung des `--idx`-Standardschemas</span><span class="sxs-lookup"><span data-stu-id="0bba9-1144">`gremlin graph create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="0bba9-1145">Tippfehler in Hilfemeldung korrigiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-1145">Fixed typo in help message</span></span>
* <span data-ttu-id="0bba9-1146">Datenbank: Informationen zur eingestellten Unterstützung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1146">database: Added deprecation information</span></span>
* <span data-ttu-id="0bba9-1147">Auflistung: Informationen zur eingestellten Unterstützung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1147">collection: Added deprecation information</span></span>

### <a name="iot"></a><span data-ttu-id="0bba9-1148">IoT</span><span class="sxs-lookup"><span data-stu-id="0bba9-1148">IoT</span></span>

* <span data-ttu-id="0bba9-1149">Neuer Routingquelltyp hinzugefügt: DigitalTwinChangeEvents</span><span class="sxs-lookup"><span data-stu-id="0bba9-1149">Added new routing source type: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="0bba9-1150">Fehlende Features in `az iot hub create` behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-1150">Fixed missing features in `az iot hub create`</span></span>

### <a name="key-vault"></a><span data-ttu-id="0bba9-1151">Key Vault</span><span class="sxs-lookup"><span data-stu-id="0bba9-1151">Key Vault</span></span>

* <span data-ttu-id="0bba9-1152">Ein unerwarteter Fehler wurde behoben, bei dem keine Zertifikatdatei vorhanden war.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1152">Fixed an unexpected error when certificate file does not exist</span></span>
* <span data-ttu-id="0bba9-1153">Funktionsunfähigkeit von `az keyvault recover/purge` behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-1153">Fixed `az keyvault recover/purge` not working</span></span>

### <a name="netappfiles"></a><span data-ttu-id="0bba9-1154">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="0bba9-1154">NetAppFiles</span></span>

* <span data-ttu-id="0bba9-1155">„azure-mgmt-netapp“ wurde auf 0.6.0 aktualisiert, um API-Version 2019-07-01 zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1155">Upgraded azure-mgmt-netapp to 0.6.0 to use API version 2019-07-01.</span></span> <span data-ttu-id="0bba9-1156">Diese neue API-Version umfasst:</span><span class="sxs-lookup"><span data-stu-id="0bba9-1156">This new API version includes:</span></span>

    - <span data-ttu-id="0bba9-1157">Volumeerstellung `--protocol-types` akzeptiert jetzt „NFSv4.1“ anstelle von „NFSv4“.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1157">Volume creation `--protocol-types` accepts now "NFSv4.1" not "NFSv4"</span></span>
    - <span data-ttu-id="0bba9-1158">Die Richtlinie der Volumeexportrichtlinie heißt jetzt „nfsv41“ anstelle von „nfsv4“.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1158">Volume export policy property now named 'nfsv41' not 'nfsv4'</span></span>
    - <span data-ttu-id="0bba9-1159">Volume `--creation-token` wurde in `--file-path` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1159">Volume `--creation-token` renamed to `--file-path`</span></span>
    - <span data-ttu-id="0bba9-1160">Das Erstellungsdatum einer Momentaufnahme heißt jetzt einfach „erstellt“.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1160">Snapshot creation date now named just 'created'</span></span>

### <a name="network"></a><span data-ttu-id="0bba9-1161">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0bba9-1161">Network</span></span>

* <span data-ttu-id="0bba9-1162">`az network private-dns link vnet create/update`: Unterstützung für mandantenübergreifende Verknüpfung virtueller Netzwerke.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1162">`az network private-dns link vnet create/update`: Support cross-tenant virtual network linking.</span></span>
* <span data-ttu-id="0bba9-1163">[BREAKING CHANGE] `az network vnet subnet list`: `--resource-group` und `--vnet-name` wurden geändert und sind jetzt erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1163">[BREAKING CHANGE] `az network vnet subnet list`: Changed `--resource-group` and `--vnet-name` to be required now.</span></span>
* <span data-ttu-id="0bba9-1164">`az network public-ip prefix create`: Unterstützung der Angabe der IP-Adressversion (IPv4, IPv6) bei der Erstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1164">`az network public-ip prefix create`: Added support to specify IP address version (IPv4, IPv6) when creation</span></span>
* <span data-ttu-id="0bba9-1165">„azure-mgmt-network“ auf 7.0.0 und „api-version“ auf 2019-09-01 festgelegt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1165">Bumped azure-mgmt-network to 7.0.0 and api-version to 2019-09-01</span></span>
* <span data-ttu-id="0bba9-1166">`az network vrouter`: Unterstützung für neuen virtuellen Dienstrouter und virtuelles Routerpeering hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1166">`az network vrouter`: Added support for new service virtual router and virtual router peering</span></span>
* <span data-ttu-id="0bba9-1167">`az network express-route gateway connection`: Unterstützung für `--internet-security` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1167">`az network express-route gateway connection`: Added support for `--internet-security`</span></span>

### <a name="profile"></a><span data-ttu-id="0bba9-1168">Profil</span><span class="sxs-lookup"><span data-stu-id="0bba9-1168">Profile</span></span>

* <span data-ttu-id="0bba9-1169">Funktionsunfähigkeit von `az account get-access-token --resource-type ms-graph` behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-1169">Fixed `az account get-access-token --resource-type ms-graph` not working</span></span>
* <span data-ttu-id="0bba9-1170">Warnung aus `az login` entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1170">Removed warning from `az login`</span></span>

### <a name="rbac"></a><span data-ttu-id="0bba9-1171">RBAC</span><span class="sxs-lookup"><span data-stu-id="0bba9-1171">RBAC</span></span>

* <span data-ttu-id="0bba9-1172">Funktionsunfähigkeit von `az ad app update --id {} --display-name {}` behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-1172">Fixed `az ad app update --id {} --display-name {}` doesn't work</span></span>

### <a name="servicefabric"></a><span data-ttu-id="0bba9-1173">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="0bba9-1173">ServiceFabric</span></span>

* <span data-ttu-id="0bba9-1174">`az sf cluster create`: Ein Problem wurde behoben, indem die Compute-VMSS von „template.json“ für Service Fabric unter Linux und Windows von Standarddatenträgern auf verwaltete Datenträger umgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1174">`az sf cluster create`: Fixed an issue by modifying service fabric linux and windows template.json compute vmss from standard to managed disks</span></span>

### <a name="sql"></a><span data-ttu-id="0bba9-1175">SQL</span><span class="sxs-lookup"><span data-stu-id="0bba9-1175">SQL</span></span>

* <span data-ttu-id="0bba9-1176">Die Parameter `--compute-model`, `--auto-pause-delay` und `--min-capacity` wurden hinzugefügt, um CRUD-Vorgänge für das neue SQL-Datenbank-Angebot zu unterstützen: Serverloses Computemodell.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1176">Added `--compute-model`, `--auto-pause-delay`, and `--min-capacity` parameters to support CRUD operations for new SQL Database offering: Serverless compute model.</span></span>

### <a name="storage"></a><span data-ttu-id="0bba9-1177">Storage</span><span class="sxs-lookup"><span data-stu-id="0bba9-1177">Storage</span></span>

* <span data-ttu-id="0bba9-1178">`az storage account create/update`: Parameter „--enable-files-adds“ und Azure Active Directory-Eigenschaftenargumentgruppe hinzugefügt, um Active Directory Domain-Dienstauthentifizierung für Azure Files zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1178">`az storage account create/update`: Added --enable-files-adds parameter and Azure Active Directory Properties Argument group to support Azure Files Active Directory Domain Service Authentication</span></span>
* <span data-ttu-id="0bba9-1179">`az storage account keys list/renew` wurde erweitert, um die Auflistung oder erneute Generierung von Kerberos-Schlüsseln des Speicherkontos zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1179">Expanded `az storage account keys list/renew` to support listing or regenerating Kerberos keys of storage account.</span></span>

## <a name="october-15-2019"></a><span data-ttu-id="0bba9-1180">15. Oktober 2019</span><span class="sxs-lookup"><span data-stu-id="0bba9-1180">October 15, 2019</span></span>

<span data-ttu-id="0bba9-1181">Version 2.0.75</span><span class="sxs-lookup"><span data-stu-id="0bba9-1181">Version 2.0.75</span></span>

### <a name="aks"></a><span data-ttu-id="0bba9-1182">AKS</span><span class="sxs-lookup"><span data-stu-id="0bba9-1182">AKS</span></span>

* <span data-ttu-id="0bba9-1183">Standardwert `--load-balancer-sku` in `standard` geändert, sofern von der Kubernetes-Version unterstützt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1183">Changed `--load-balancer-sku` default value to `standard` if supported by the kubernetes version</span></span>
* <span data-ttu-id="0bba9-1184">Standardwert `--vm-set-type` in `virtualmachinescalesets` geändert, sofern von der Kubernetes-Version unterstützt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1184">Changed `--vm-set-type` default value to `virtualmachinescalesets` if supported by the kubernetes version</span></span>

### <a name="ams"></a><span data-ttu-id="0bba9-1185">AMS</span><span class="sxs-lookup"><span data-stu-id="0bba9-1185">AMS</span></span>

* <span data-ttu-id="0bba9-1186">[BREAKING CHANGE] Name von `job start` in `job create` geändert</span><span class="sxs-lookup"><span data-stu-id="0bba9-1186">[BREAKING CHANGE] Changed the name of `job start` to `job create`</span></span>
* <span data-ttu-id="0bba9-1187">[BREAKING CHANGE] Parameter `--ask` von `content-key-policy create` geändert, sodass eine hexadezimale Zeichenfolge mit 32 Zeichen anstelle von UTF8 verwendet wird</span><span class="sxs-lookup"><span data-stu-id="0bba9-1187">[BREAKING CHANGE] Changed the `--ask` parameter of `content-key-policy create` to use a 32-character hex string instead of UTF8</span></span>

### <a name="appservice"></a><span data-ttu-id="0bba9-1188">AppService</span><span class="sxs-lookup"><span data-stu-id="0bba9-1188">AppService</span></span>

* <span data-ttu-id="0bba9-1189">Befehle vom Typ `webapp config access-restriction show|set|add|remove` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1189">Added commands `webapp config access-restriction show|set|add|remove`</span></span>
* <span data-ttu-id="0bba9-1190">Bessere Fehlerbehandlung zu `webapp up` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1190">Added better error handling to `webapp up`</span></span>
* <span data-ttu-id="0bba9-1191">Unterstützung für SKU `Isolated` zu `appservice plan update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1191">Added support for `Isolated` SKU to `appservice plan update`</span></span>

### <a name="arm"></a><span data-ttu-id="0bba9-1192">ARM</span><span class="sxs-lookup"><span data-stu-id="0bba9-1192">ARM</span></span>

* <span data-ttu-id="0bba9-1193">Parameter `--handle-extended-json-format` zu `deployment create` hinzugefügt, um mehrere Zeilen und Kommentare in der JSON-Vorlage zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="0bba9-1193">Added `--handle-extended-json-format` parameter `deployment create` to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="0bba9-1194">Compute</span><span class="sxs-lookup"><span data-stu-id="0bba9-1194">Compute</span></span>

* <span data-ttu-id="0bba9-1195">Parameter `--enable-agent` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1195">Added `--enable-agent` parameter to `vm create`</span></span>
* <span data-ttu-id="0bba9-1196">`vm create` geändert, um bei der Verwendung von Zonen die SKU „Standard“ für die öffentliche IP-Adresse zu verwenden</span><span class="sxs-lookup"><span data-stu-id="0bba9-1196">Changed `vm create` to use standard public IP SKU automatically when using zones</span></span>
* <span data-ttu-id="0bba9-1197">`vm create` geändert, um automatisch einen gültigen Computernamen für eine VM zu erstellen, falls keiner angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="0bba9-1197">Changed `vm create` to automatically create a valid computer name for a VM if none is provided</span></span>
* <span data-ttu-id="0bba9-1198">Parameter `--computer-name-prefix` zu `vmss create` hinzugefügt, um das benutzerdefinierte Computernamenspräfix virtueller Computer in VMSS zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="0bba9-1198">Added `--computer-name-prefix` parameter to `vmss create` to support custom computer name prefix of virtual machines in the VMSS</span></span>
* <span data-ttu-id="0bba9-1199">Parameter `--workspace` zu `vm create` hinzugefügt, um automatisch einen Log Analytics-Arbeitsbereich zu aktivieren</span><span class="sxs-lookup"><span data-stu-id="0bba9-1199">Add `--workspace` parameter to `vm create` to enable log analytics workspace automatically</span></span>
* <span data-ttu-id="0bba9-1200">API-Version für Kataloge auf 2019-07-01 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-1200">Updated galleries API version to 2019-07-01</span></span>

### <a name="core"></a><span data-ttu-id="0bba9-1201">Core</span><span class="sxs-lookup"><span data-stu-id="0bba9-1201">Core</span></span>

* <span data-ttu-id="0bba9-1202">Syntaxprüfung für Parameter `--set` im generischen Updatebefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1202">Added syntax check for `--set` parameter in generic update command</span></span>

### <a name="iot"></a><span data-ttu-id="0bba9-1203">IoT</span><span class="sxs-lookup"><span data-stu-id="0bba9-1203">IoT</span></span>

* <span data-ttu-id="0bba9-1204">Problem behoben, bei dem für `iot hub show` der Fehler „Ressource nicht gefunden.“ zurückgegeben wurde</span><span class="sxs-lookup"><span data-stu-id="0bba9-1204">Fixed an issue where `iot hub show` would incorrectly error with "resource not found"</span></span>

### <a name="monitor"></a><span data-ttu-id="0bba9-1205">Überwachen</span><span class="sxs-lookup"><span data-stu-id="0bba9-1205">Monitor</span></span>

* <span data-ttu-id="0bba9-1206">Unterstützung für CRUD zu `monitor log-analytics workspace` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1206">Added support for CRUD to `monitor log-analytics workspace`</span></span>

### <a name="network"></a><span data-ttu-id="0bba9-1207">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0bba9-1207">Network</span></span>

* <span data-ttu-id="0bba9-1208">Unterstützung für mandantenübergreifende virtuelle Verbindung zu `network private-dns link vnet [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1208">Added support for cross-tenant virtual linking to `network private-dns link vnet [create|update]`</span></span>
* <span data-ttu-id="0bba9-1209">[BREAKING CHANGE]`network vnet subnet list` geändert, um Parameter `--resource-group` und `--vnet-name` vorauszusetzen</span><span class="sxs-lookup"><span data-stu-id="0bba9-1209">[BREAKING CHANGE] Changed `network vnet subnet list` to require `--resource-group` and `--vnet-name` parameters</span></span>

### <a name="sql"></a><span data-ttu-id="0bba9-1210">SQL</span><span class="sxs-lookup"><span data-stu-id="0bba9-1210">SQL</span></span>

* <span data-ttu-id="0bba9-1211">Befehle zu `sql mi ad-admin` hinzugefügt, die das Festlegen eines AAD-Administrators für verwaltete Instanzen unterstützen</span><span class="sxs-lookup"><span data-stu-id="0bba9-1211">Added commands to `sql mi ad-admin` that support setting an AAD administrator on managed instances</span></span>

### <a name="storage"></a><span data-ttu-id="0bba9-1212">Storage</span><span class="sxs-lookup"><span data-stu-id="0bba9-1212">Storage</span></span>

* <span data-ttu-id="0bba9-1213">Parameter `--preserve-s2s-access-tier` zu `storage copy` hinzugefügt, um die Zugriffsebene beim Kopieren von Dienst zu Dienst beizubehalten</span><span class="sxs-lookup"><span data-stu-id="0bba9-1213">Added `--preserve-s2s-access-tier` parameter `storage copy` to preserve access tier during service to service copy</span></span>
* <span data-ttu-id="0bba9-1214">Parameter `--enable-large-file-share` zu `storage account [create|update]` hinzugefügt, um große Dateifreigaben für ein Speicherkonto zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="0bba9-1214">Added `--enable-large-file-share` parameter to `storage account [create|update]` to support large file shares for storage account</span></span>

## <a name="september-24-2019"></a><span data-ttu-id="0bba9-1215">24. September 2019</span><span class="sxs-lookup"><span data-stu-id="0bba9-1215">September 24, 2019</span></span>

<span data-ttu-id="0bba9-1216">Version 2.0.74</span><span class="sxs-lookup"><span data-stu-id="0bba9-1216">Version 2.0.74</span></span>

### <a name="acr"></a><span data-ttu-id="0bba9-1217">ACR</span><span class="sxs-lookup"><span data-stu-id="0bba9-1217">ACR</span></span>

* <span data-ttu-id="0bba9-1218">Erforderlicher Parameter `--type` zu `acr config retention update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1218">Added a required `--type` parameter to `acr config retention update`</span></span>
* <span data-ttu-id="0bba9-1219">[BREAKING CHANGE] Umbenannter Parameter `--name -n` in `--registry -r ` für Befehlsgruppe `acr config` geändert</span><span class="sxs-lookup"><span data-stu-id="0bba9-1219">[BREAKING CHANGE] Renamed parameter `--name -n` changed to `--registry -r ` for `acr config` command group</span></span>

### <a name="aks"></a><span data-ttu-id="0bba9-1220">AKS</span><span class="sxs-lookup"><span data-stu-id="0bba9-1220">AKS</span></span>

* <span data-ttu-id="0bba9-1221">Parameter `--load-balancer-sku` zum Befehl `aks create` hinzugefügt, um die Erstellung von AKS-Clustern mit SLB zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="0bba9-1221">Added `--load-balancer-sku` parameter to `aks create` command, which allows for creating AKS cluster with SLB</span></span>
* <span data-ttu-id="0bba9-1222">Parameter `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` und `--load-balancer-outbound-ip-prefixes` zu den Befehlen `aks [create|update]` hinzugefügt,um die Aktualisierung des Lastenausgleichsprofils eines AKS-Clusters mit SLB zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="0bba9-1222">Added `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` and `--load-balancer-outbound-ip-prefixes` parameters to `aks [create|update]` commands, which allow for updating load balancer profile of an AKS cluster with SLB</span></span>
* <span data-ttu-id="0bba9-1223">Parameter `--vm-set-type` zum Befehl `aks create` hinzugefügt, um die Angabe von VM-Typen eines AKS-Clusters (vmas oder vmss) zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="0bba9-1223">Added `--vm-set-type` parameter to `aks create` command, which allows to specify vm types of an AKS Cluster (vmas or vmss)</span></span>

### <a name="arm"></a><span data-ttu-id="0bba9-1224">ARM</span><span class="sxs-lookup"><span data-stu-id="0bba9-1224">ARM</span></span>

* <span data-ttu-id="0bba9-1225">Parameter `--handle-extended-json-format` zum Befehl `group deployment create` hinzugefügt, um mehrere Zeilen und Kommentare in der JSON-Vorlage zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="0bba9-1225">Added `--handle-extended-json-format` parameter to `group deployment create` command to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="0bba9-1226">Compute</span><span class="sxs-lookup"><span data-stu-id="0bba9-1226">Compute</span></span>

* <span data-ttu-id="0bba9-1227">Parameter `--terminate-notification-time` zu den Befehlen `vmss [create|update]` hinzugefügt, um die Konfigurierbarkeit der Beendigung geplanter Ereignisse zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="0bba9-1227">Added `--terminate-notification-time` parameter to `vmss [create|update]` commands to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="0bba9-1228">Parameter `--enable-terminate-notification` zu den Befehlen `vmss update` hinzugefügt, um die Konfigurierbarkeit der Beendigung geplanter Ereignisse zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="0bba9-1228">Added `--enable-terminate-notification` parameter to `vmss update` command to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="0bba9-1229">Parameter `--priority,` `--eviction-policy,` `--max-billing` zu `[vm|vmss] create`-Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1229">Added `--priority,` `--eviction-policy,` `--max-billing` parameters to `[vm|vmss] create` commands</span></span>
* <span data-ttu-id="0bba9-1230">`disk create` geändert, um die Angabe der genauen Größe des Datenträgeruploads zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="0bba9-1230">Changed `disk create` to allow specifying the exact size of the disk upload</span></span>
* <span data-ttu-id="0bba9-1231">Unterstützung für inkrementelle Momentaufnahmen für verwaltete Datenträger zu `snapshot create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1231">Added support for incremental snapshots for managed disks to `snapshot create`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="0bba9-1232">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="0bba9-1232">Cosmos DB</span></span>

* <span data-ttu-id="0bba9-1233">Parameter `--type <key-type>` zum Befehl `cosmosdb keys list` hinzugefügt, um Schlüssel, schreibgeschützte Schlüssel oder Verbindungszeichenfolgen anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="0bba9-1233">Added `--type <key-type>` parameter to `cosmosdb keys list` command to show key, read only keys or connection strings</span></span>
* <span data-ttu-id="0bba9-1234">Befehl `cosmosdb keys regenerate` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1234">Added `cosmosdb keys regenerate` command</span></span>
* <span data-ttu-id="0bba9-1235">[VERALTET] Befehle `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` und `cosmosdb list-read-only-keys` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-1235">[DEPRECATED] Deprecated `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` and `cosmosdb list-read-only-keys` commands</span></span>

### <a name="eventgrid"></a><span data-ttu-id="0bba9-1236">EventGrid</span><span class="sxs-lookup"><span data-stu-id="0bba9-1236">EventGrid</span></span>

* <span data-ttu-id="0bba9-1237">Endpunkthilfetext korrigiert, um auf den richtigen Parameter zu verweisen</span><span class="sxs-lookup"><span data-stu-id="0bba9-1237">Fixed the endpoint help text to refer to the right parameter</span></span>

### <a name="key-vault"></a><span data-ttu-id="0bba9-1238">Key Vault</span><span class="sxs-lookup"><span data-stu-id="0bba9-1238">Key Vault</span></span>

* <span data-ttu-id="0bba9-1239">Problem behoben, aufgrund dessen die Anmeldung mit einem Mandanten (`login -t`) unter Umständen zu einem Fehler von `keyvault create` führte</span><span class="sxs-lookup"><span data-stu-id="0bba9-1239">Fixed issue where logging in with a tenant (`login -t`) could cause `keyvault create` to fail</span></span>

### <a name="monitor"></a><span data-ttu-id="0bba9-1240">Überwachen</span><span class="sxs-lookup"><span data-stu-id="0bba9-1240">Monitor</span></span>

* <span data-ttu-id="0bba9-1241">Problem behoben, aufgrund dessen das Zeichen `:` in `--condition` für `monitor metrics alert create` nicht zulässig war</span><span class="sxs-lookup"><span data-stu-id="0bba9-1241">Fixed issue where `:` character was not allowed in `--condition` argument to `monitor metrics alert create`</span></span>

### <a name="policy"></a><span data-ttu-id="0bba9-1242">Richtlinie</span><span class="sxs-lookup"><span data-stu-id="0bba9-1242">Policy</span></span>

* <span data-ttu-id="0bba9-1243">Unterstützung für Policy-API-Version 2019-06-01 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1243">Added support for Policy API version 2019-06-01</span></span>
* <span data-ttu-id="0bba9-1244">Parameter `--enforcement-mode` zum Befehl `policy assignment create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1244">Added `--enforcement-mode` parameter to `policy assignment create` command</span></span>

### <a name="storage"></a><span data-ttu-id="0bba9-1245">Storage</span><span class="sxs-lookup"><span data-stu-id="0bba9-1245">Storage</span></span>

* <span data-ttu-id="0bba9-1246">Parameter `--blob-type` zum Befehl `az storage copy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1246">Added `--blob-type` parameter to `az storage copy` command</span></span>

## <a name="september-10-2019"></a><span data-ttu-id="0bba9-1247">10. September 2019</span><span class="sxs-lookup"><span data-stu-id="0bba9-1247">September 10, 2019</span></span>

### <a name="acr"></a><span data-ttu-id="0bba9-1248">ACR</span><span class="sxs-lookup"><span data-stu-id="0bba9-1248">ACR</span></span>

* <span data-ttu-id="0bba9-1249">Befehlsgruppe `acr config retention` zum Konfigurieren der Aufbewahrungsrichtlinie hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1249">Added command group `acr config retention` to configure retention policy</span></span>

### <a name="aks"></a><span data-ttu-id="0bba9-1250">AKS</span><span class="sxs-lookup"><span data-stu-id="0bba9-1250">AKS</span></span>

* <span data-ttu-id="0bba9-1251">Unterstützung für die ACR-Integration mit den folgenden Befehlen hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="0bba9-1251">Added support for ACR integration with the following commands:</span></span>
  * <span data-ttu-id="0bba9-1252">Parameter `--attach-acr` zu `aks [create|update]` hinzugefügt, um einen ACR an einen AKS-Cluster anzufügen</span><span class="sxs-lookup"><span data-stu-id="0bba9-1252">Added `--attach-acr` parameter to `aks [create|update]` to attach an ACR to an AKS cluster</span></span>
  * <span data-ttu-id="0bba9-1253">Parameter `--detach-acr` zu `aks update` hinzugefügt, um den ACR von einem AKS-Cluster zu trennen</span><span class="sxs-lookup"><span data-stu-id="0bba9-1253">Added `--detach-acr` parameter to `aks update` to detach the ACR from an AKS cluster</span></span>

### <a name="arm"></a><span data-ttu-id="0bba9-1254">ARM</span><span class="sxs-lookup"><span data-stu-id="0bba9-1254">ARM</span></span>

* <span data-ttu-id="0bba9-1255">Zur Verwendung der API-Version 2019-05-10 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-1255">Updated to use API version 2019-05-10</span></span>

### <a name="batch"></a><span data-ttu-id="0bba9-1256">Batch</span><span class="sxs-lookup"><span data-stu-id="0bba9-1256">Batch</span></span>

* <span data-ttu-id="0bba9-1257">Neue JSON-Konfigurationseinstellungen für `batch pool create` zu `--json-file` hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="0bba9-1257">Added new JSON configuration settings to `--json-file` for `batch pool create`:</span></span>
  * <span data-ttu-id="0bba9-1258">`MountConfigurations` für Dateisystemeinbindungen hinzugefügt (Details siehe https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body )</span><span class="sxs-lookup"><span data-stu-id="0bba9-1258">Added `MountConfigurations` for file system mounts (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
  * <span data-ttu-id="0bba9-1259">Optionale Eigenschaft `publicIPs` in `NetworkConfiguration` für öffentliche IP-Adressen für Pools hinzugefügt (Details siehe https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body )</span><span class="sxs-lookup"><span data-stu-id="0bba9-1259">Added optional property `publicIPs` on `NetworkConfiguration` for public IPs on pools (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
* <span data-ttu-id="0bba9-1260">Unterstützung für Kataloge mit freigegebenen Images zu `--image` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1260">Added support for shared image galleries to `--image`</span></span>
* <span data-ttu-id="0bba9-1261">[BREAKING CHANGE] Standardwert von `--start-task-wait-for-success` für `batch pool create` in `true` geändert</span><span class="sxs-lookup"><span data-stu-id="0bba9-1261">[BREAKING CHANGE] Changed default value of `--start-task-wait-for-success` on `batch pool create` to be `true`</span></span>
* <span data-ttu-id="0bba9-1262">[BREAKING CHANGE] Standardwert von `Scope` für `AutoUserSpecification` geändert, damit immer „Pool“ verwendet wird (vormals `Task` für Windows-Knoten bzw. `Pool` für Linux-Knoten)</span><span class="sxs-lookup"><span data-stu-id="0bba9-1262">[BREAKING CHANGE] Changed default value for `Scope` on `AutoUserSpecification` to always be Pool (was `Task` on Windows nodes, `Pool` on Linux nodes)</span></span>
  * <span data-ttu-id="0bba9-1263">Dieses Argument kann nur über eine JSON-Konfiguration mit `--json-file` festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1263">This argument can only be set from a JSON configuration with `--json-file`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="0bba9-1264">HDInsight</span><span class="sxs-lookup"><span data-stu-id="0bba9-1264">HDInsight</span></span>

* <span data-ttu-id="0bba9-1265">Allgemein verfügbares Release</span><span class="sxs-lookup"><span data-stu-id="0bba9-1265">GA release</span></span>
* <span data-ttu-id="0bba9-1266">[BREAKING CHANGE] Parameter `--workernode-count/-c` von `az hdinsight resize` in erforderlich geändert</span><span class="sxs-lookup"><span data-stu-id="0bba9-1266">[BREAKING CHANGE] Changed parameter `--workernode-count/-c` of `az hdinsight resize` to be required.</span></span>

### <a name="key-vault"></a><span data-ttu-id="0bba9-1267">Key Vault</span><span class="sxs-lookup"><span data-stu-id="0bba9-1267">Key Vault</span></span>

* <span data-ttu-id="0bba9-1268">Problem behoben, aufgrund dessen Subnetze nicht aus Netzwerkregeln gelöscht werden konnten</span><span class="sxs-lookup"><span data-stu-id="0bba9-1268">Fixed issue where subnets couldn't be deleted from network rules</span></span>
* <span data-ttu-id="0bba9-1269">Problem behoben, aufgrund dessen doppelte Subnetze und IP-Adressen zu Netzwerkregeln hinzugefügt werden konnten</span><span class="sxs-lookup"><span data-stu-id="0bba9-1269">Fixed issue where duplicated subnets and IP addresses could be added to network rules</span></span>

### <a name="network"></a><span data-ttu-id="0bba9-1270">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0bba9-1270">Network</span></span>

* <span data-ttu-id="0bba9-1271">Parameter `--interval` zu `network watcher flow-log` hinzugefügt, um den Wert für das Intervall der Datenverkehrsanalyse festzulegen</span><span class="sxs-lookup"><span data-stu-id="0bba9-1271">Added `--interval` parameter to `network watcher flow-log` to set traffic analysis interval value</span></span>
* <span data-ttu-id="0bba9-1272">`network application-gateway identity` zum Verwalten der Gatewayidentität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1272">Added `network application-gateway identity` to manage gateway identity</span></span>
* <span data-ttu-id="0bba9-1273">Unterstützung zum Festlegen der Key Vault-ID zu `network application-gateway ssl-cert` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1273">Added support for setting Key Vault ID to `network application-gateway ssl-cert`</span></span>
* <span data-ttu-id="0bba9-1274">`network express-route peering peer-connection [show|list]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1274">Added `network express-route peering peer-connection [show|list]`</span></span>

### <a name="policy"></a><span data-ttu-id="0bba9-1275">Richtlinie</span><span class="sxs-lookup"><span data-stu-id="0bba9-1275">Policy</span></span>

* <span data-ttu-id="0bba9-1276">Zur Verwendung der API-Version 2019-01-01 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-1276">Updated to use API version 2019-01-01</span></span>

## <a name="august-27-2019"></a><span data-ttu-id="0bba9-1277">27. August 2019</span><span class="sxs-lookup"><span data-stu-id="0bba9-1277">August 27, 2019</span></span>

<span data-ttu-id="0bba9-1278">Version 2.0.72</span><span class="sxs-lookup"><span data-stu-id="0bba9-1278">Version 2.0.72</span></span>

### <a name="acr"></a><span data-ttu-id="0bba9-1279">ACR</span><span class="sxs-lookup"><span data-stu-id="0bba9-1279">ACR</span></span>

* <span data-ttu-id="0bba9-1280">[BREAKING CHANGE] Unterstützung für SKU `classic` entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1280">[BREAKING CHANGE] Removed support for the `classic` SKU</span></span>

### <a name="api-management"></a><span data-ttu-id="0bba9-1281">API Management</span><span class="sxs-lookup"><span data-stu-id="0bba9-1281">API Management</span></span>

* <span data-ttu-id="0bba9-1282">[VORSCHAU] Befehlsgruppe `apim` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1282">[PREVIEW] Added `apim` command group</span></span>

### <a name="appservice"></a><span data-ttu-id="0bba9-1283">AppService</span><span class="sxs-lookup"><span data-stu-id="0bba9-1283">AppService</span></span>

* <span data-ttu-id="0bba9-1284">Problem mit dem Befehl `webapp webjob continuous start` bei Angabe eines Slots behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-1284">Fixed issue with `webapp webjob continuous start` command when specifying a slot</span></span>
* <span data-ttu-id="0bba9-1285">`webapp up` geändert, um den Ordner `env` zu erkennen und aus der für die Bereitstellung verwendeten Datei zu entfernen</span><span class="sxs-lookup"><span data-stu-id="0bba9-1285">Changed `webapp up` to detect `env` folder and remove it from the file used for deployment</span></span>

### <a name="keyvault"></a><span data-ttu-id="0bba9-1286">KeyVault</span><span class="sxs-lookup"><span data-stu-id="0bba9-1286">Keyvault</span></span>

* <span data-ttu-id="0bba9-1287">Fehler in `keyvault secret set` behoben, aufgrund dessen das Argument `--expires` ignoriert wurde</span><span class="sxs-lookup"><span data-stu-id="0bba9-1287">Fixed a bug in `keyvault secret set` that igored the `--expires` argument</span></span>

### <a name="network"></a><span data-ttu-id="0bba9-1288">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0bba9-1288">Network</span></span>

* <span data-ttu-id="0bba9-1289">Unterstützung für IPv6-Adressen zu Argumenten vom Typ `--private-ip-address-version` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1289">Added support for IPv6 addresses to `--private-ip-address-version` arguments</span></span>
* <span data-ttu-id="0bba9-1290">Neue Befehle vom Typ `network private-endpoint [create|update|list-types]` für die Verwaltung privater Endpunkte hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1290">Added new commands `network private-endpoint [create|update|list-types]` for private endpoint management</span></span>
* <span data-ttu-id="0bba9-1291">Befehlsgruppe `network private-link-service` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1291">Added command group `network private-link-service`</span></span>
* <span data-ttu-id="0bba9-1292">Argumente `--private-endpoint-network-policies` und `--private-link-service-network-policies` zu `network vnet subnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1292">Added `--private-endpoint-network-policies` and `--private-link-service-network-policies` arguments to `network vnet subnet update`</span></span>

### <a name="rbac"></a><span data-ttu-id="0bba9-1293">RBAC</span><span class="sxs-lookup"><span data-stu-id="0bba9-1293">RBAC</span></span>

* <span data-ttu-id="0bba9-1294">Problem mit `ad app update --homepage` behoben, aufgrund dessen die Startseite nicht aktualisiert wurde</span><span class="sxs-lookup"><span data-stu-id="0bba9-1294">Fixed issue with `ad app update --homepage` where homepage would not be updated</span></span>

### <a name="servicefabric"></a><span data-ttu-id="0bba9-1295">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="0bba9-1295">ServiceFabric</span></span>

* <span data-ttu-id="0bba9-1296">Unterstützung für Key Vault-Namen mit Groß- und Kleinschreibung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1296">Added support for mixed-case Key Vault names</span></span>
* <span data-ttu-id="0bba9-1297">Problem bei der Verwendung von Zertifikaten in Key Vault behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-1297">Fixed issue when using certificates in Key Vault</span></span>
* <span data-ttu-id="0bba9-1298">Problem bei der Verwendung von PFX-Zertifikatdateien behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-1298">Fixed issue with using PFX certificate files</span></span>
* <span data-ttu-id="0bba9-1299">Problem mit `sf cluster certificate add` behoben, wenn keine Key Vault-Ressourcengruppe angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="0bba9-1299">Fixed issue with `sf cluster certificate add` when Key Vault resource group wasn't specified</span></span>
* <span data-ttu-id="0bba9-1300">Problem behoben, aufgrund dessen `sf cluster set` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="0bba9-1300">Fixed issue with `sf cluster set` not working</span></span>

### <a name="signalr"></a><span data-ttu-id="0bba9-1301">SignalR</span><span class="sxs-lookup"><span data-stu-id="0bba9-1301">SignalR</span></span>

* <span data-ttu-id="0bba9-1302">Neue Befehle hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="0bba9-1302">Added new commands:</span></span>
  * <span data-ttu-id="0bba9-1303">`signalr cors`: Verwalten von CORS für SignalR</span><span class="sxs-lookup"><span data-stu-id="0bba9-1303">`signalr cors`: Manage SignalR CORS</span></span>
  * <span data-ttu-id="0bba9-1304">`signalr restart`: Starten eines SignalR-Diensts</span><span class="sxs-lookup"><span data-stu-id="0bba9-1304">`signalr restart`: Restart a SignalR service</span></span>
  * <span data-ttu-id="0bba9-1305">`signalr update`: Aktualisieren eines SignalR-Diensts</span><span class="sxs-lookup"><span data-stu-id="0bba9-1305">`signalr update`: Update a SignalR service</span></span>
* <span data-ttu-id="0bba9-1306">Argument `--service-mode` zu `signalr create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1306">Added `--service-mode` argument to `signalr create`</span></span>

### <a name="storage"></a><span data-ttu-id="0bba9-1307">Storage</span><span class="sxs-lookup"><span data-stu-id="0bba9-1307">Storage</span></span>

* <span data-ttu-id="0bba9-1308">Befehl `storage account revoke-delegation-keys` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1308">Added `storage account revoke-delegation-keys` command</span></span>

## <a name="august-13-2019"></a><span data-ttu-id="0bba9-1309">13. August 2019</span><span class="sxs-lookup"><span data-stu-id="0bba9-1309">August 13, 2019</span></span>

<span data-ttu-id="0bba9-1310">Version 2.0.71</span><span class="sxs-lookup"><span data-stu-id="0bba9-1310">Version 2.0.71</span></span>

### <a name="appservice"></a><span data-ttu-id="0bba9-1311">AppService</span><span class="sxs-lookup"><span data-stu-id="0bba9-1311">AppService</span></span>

* <span data-ttu-id="0bba9-1312">Problem behoben, aufgrund dessen bei Befehlen vom Typ `webapp webjob continuous` für Slots Fehler auftraten</span><span class="sxs-lookup"><span data-stu-id="0bba9-1312">Fixed issue where `webapp webjob continuous` commands were failing for slots</span></span>

### <a name="botservice"></a><span data-ttu-id="0bba9-1313">BotService</span><span class="sxs-lookup"><span data-stu-id="0bba9-1313">BotService</span></span>

* <span data-ttu-id="0bba9-1314">[BREAKING CHANGE] Unterstützung für die Erstellung von Bots der Version 3 entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1314">[BREAKING CHANGE] Removed support for creating v3 SDK bots</span></span>

### <a name="cognitiveservices"></a><span data-ttu-id="0bba9-1315">CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="0bba9-1315">CognitiveServices</span></span>

* <span data-ttu-id="0bba9-1316">Befehle vom Typ `cognitiveservices account network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1316">Added `cognitiveservices account network-rule` commands</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="0bba9-1317">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="0bba9-1317">Cosmos DB</span></span>

* <span data-ttu-id="0bba9-1318">Beim Aktualisieren mehrerer Schreibstandorte wurde eine Warnung entfernt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1318">Removed warning when updating multiple write locations</span></span>
* <span data-ttu-id="0bba9-1319">CRUD-Befehle für CosmosDB SQL-, MongoDB-, Cassandra-, Gremlin- und Tabellenressourcen sowie den Ressourcendurchsatz hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1319">Added CRUD commands for CosmosDB SQL, MongoDB, Cassandra, Gremlin and Table resources and resource's throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="0bba9-1320">HDInsight</span><span class="sxs-lookup"><span data-stu-id="0bba9-1320">HDInsight</span></span>

<span data-ttu-id="0bba9-1321">Dieses Release enthält zahlreiche wichtige Änderungen.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1321">This release contains a large number of breaking changes.</span></span>

* <span data-ttu-id="0bba9-1322">[BREAKING CHANGE] Parameter für `hdinsight create` umbenannt:</span><span class="sxs-lookup"><span data-stu-id="0bba9-1322">[BREAKING CHANGE] Renamed parameters for `hdinsight create`:</span></span>
  * <span data-ttu-id="0bba9-1323">`--storage-default-container` in `--storage-container` umbenannt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1323">Renamed `--storage-default-container` to `--storage-container`</span></span>
  * <span data-ttu-id="0bba9-1324">`--storage-default-filesystem` in `--storage-filesystem` umbenannt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1324">Renamed `--storage-default-filesystem` to `--storage-filesystem`</span></span>
* <span data-ttu-id="0bba9-1325">[BREAKING CHANGE] Das Argument `--name` von `application create` wurde so geändert, dass es den Anwendungsnamen anstelle des Clusternamens darstellt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1325">[BREAKING CHANGE] Changed the `--name` argument of `application create` to represent the application name instead of the cluster name</span></span>
* <span data-ttu-id="0bba9-1326">Argument `--cluster-name` zu `application create` hinzugefügt, um die alte Funktion `--name` zu ersetzen</span><span class="sxs-lookup"><span data-stu-id="0bba9-1326">Added `--cluster-name` argument to `application create` to replace old `--name` functionality</span></span>
* <span data-ttu-id="0bba9-1327">[BREAKING CHANGE] Parameter für `application create` umbenannt:</span><span class="sxs-lookup"><span data-stu-id="0bba9-1327">[BREAKING CHANGE] Renamed parameters for `application create`:</span></span>
  * <span data-ttu-id="0bba9-1328">`--application-type` in `--type` umbenannt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1328">Renamed `--application-type` to `--type`</span></span>
  * <span data-ttu-id="0bba9-1329">`--marketplace-identifier` in `--marketplace-id` umbenannt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1329">Renamed `--marketplace-identifier` to `--marketplace-id`</span></span>
  * <span data-ttu-id="0bba9-1330">`--https-endpoint-access-mode` in `--access-mode` umbenannt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1330">Renamed `--https-endpoint-access-mode` to `--access-mode`</span></span>
  * <span data-ttu-id="0bba9-1331">`--https-endpoint-destination-port` in `--destination-port` umbenannt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1331">Renamed  `--https-endpoint-destination-port` to `--destination-port`</span></span>
* <span data-ttu-id="0bba9-1332">[BREAKING CHANGE] Parameter für `application create` entfernt:</span><span class="sxs-lookup"><span data-stu-id="0bba9-1332">[BREAKING CHANGE] Removed parameters for `application create`:</span></span>
  * `--https-endpoint-location`
  * `--https-endpoint-public-port`
  * `--ssh-endpoint-destination-port`
  * `--ssh-endpoint-location`
  * `--ssh-endpoint-public-port`
* <span data-ttu-id="0bba9-1333">[WICHTIGE ÄNDERUNG] `--target-instance-count` für `hdinsight resize` in `--workernode-count` umbenannt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1333">[BREAKING CHNAGE] Renamed `--target-instance-count` to `--workernode-count` for `hdinsight resize`</span></span>
* <span data-ttu-id="0bba9-1334">[BREAKING CHANGE] Alle Befehle in der Gruppe `hdinsight script-action` wurden so geändert, dass sie den Parameter `--name` als Namen der Skriptaktion verwenden.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1334">[BREAKING CHANGE] Changed all commands in the `hdinsight script-action` group to use the `--name` parameter as the name of the script action.</span></span>
* <span data-ttu-id="0bba9-1335">Argument `--cluster-name` zu allen Befehlen vom Typ `hdinsight script-action` hinzugefügt, um die alte Funktion `--name` zu ersetzen</span><span class="sxs-lookup"><span data-stu-id="0bba9-1335">Added `--cluster-name` argument to all `hdinsight script-action` commands to replace old `--name` functionality</span></span>
* <span data-ttu-id="0bba9-1336">[BREAKING CHANGE]`--script-execution-id` für alle Befehle vom Typ `hdinsight script-action` in `--execution-id` umbenannt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1336">[BREAKING CHANGE] Renamed `--script-execution-id` to `--execution-id` for all `hdinsight script-action` commands</span></span>
* <span data-ttu-id="0bba9-1337">[BREAKING CHANGE]`hdinsight script-action show` in `hdinsight script-action show-execution-details` umbenannt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1337">[BREAKING CHANGE] Renamed `hdinsight script-action show` to `hdinsight script-action show-execution-details`</span></span>
* <span data-ttu-id="0bba9-1338">[WICHTIGE ÄNDERUNG] Parameter in `hdinsight script-action execute --roles` geändert, sodass sie durch Leerzeichen anstelle von Kommas getrennt sind</span><span class="sxs-lookup"><span data-stu-id="0bba9-1338">[BREAKING CHNAGE] Changed parameters to `hdinsight script-action execute --roles` to be space-separated instead of comma-separated</span></span>
* <span data-ttu-id="0bba9-1339">[BREAKING CHANGE] Parameter `--persisted` für `hdinsight script-action list` entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1339">[BREAKING CHANGE] Removed the `--persisted` parameter of `hdinsight script-action list`</span></span>
* <span data-ttu-id="0bba9-1340">Der Parameter `hdinsight create --cluster-configurations` wurde so geändert, dass er einen Pfad zu einer lokalen JSON-Datei oder JSON-Zeichenfolge akzeptiert.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1340">Changed the `hdinsight create --cluster-configurations` parameter to accept a path to a local JSON file or a JSON string</span></span>
* <span data-ttu-id="0bba9-1341">Befehl `hdinsight script-action list-execution-history` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1341">Added command `hdinsight script-action list-execution-history`</span></span>
* <span data-ttu-id="0bba9-1342">`hdinsight monitor enable --workspace` geändert, um die ID oder den Namen eines Log Analytics-Arbeitsbereichs zu akzeptieren</span><span class="sxs-lookup"><span data-stu-id="0bba9-1342">Changed `hdinsight monitor enable --workspace` to accept a Log Analytics workspace ID or workspace name</span></span>
* <span data-ttu-id="0bba9-1343">Argument `hdinsight monitor enable --primary-key` hinzugefügt. Dieses Argument wird benötigt, wenn eine Arbeitsbereichs-ID als Parameter angegeben wird.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1343">Added the `hdinsight monitor enable --primary-key` argument, which is needed if a workspace ID is provided as the parameter</span></span>
* <span data-ttu-id="0bba9-1344">Weitere Beispiele und aktualisierte Beschreibungen für Hilfemeldungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1344">Added more examples and updated descriptions for help messages</span></span>

### <a name="interactive"></a><span data-ttu-id="0bba9-1345">Interactive</span><span class="sxs-lookup"><span data-stu-id="0bba9-1345">Interactive</span></span>

* <span data-ttu-id="0bba9-1346">Ladefehler behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-1346">Fixed a loading error</span></span>

### <a name="kubernetes"></a><span data-ttu-id="0bba9-1347">Kubernetes</span><span class="sxs-lookup"><span data-stu-id="0bba9-1347">Kubernetes</span></span>

* <span data-ttu-id="0bba9-1348">Änderung, um `https` zu verwenden, wenn der Dashboardcontainerport `https` verwendet</span><span class="sxs-lookup"><span data-stu-id="0bba9-1348">Changed to use `https` if dashboard container port is using `https`</span></span>

### <a name="network"></a><span data-ttu-id="0bba9-1349">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0bba9-1349">Network</span></span>

* <span data-ttu-id="0bba9-1350">Argument `--yes` hinzugefügt zu `network dns record-set cname delete`</span><span class="sxs-lookup"><span data-stu-id="0bba9-1350">Added `--yes` argument `network dns record-set cname delete`</span></span>

### <a name="profile"></a><span data-ttu-id="0bba9-1351">Profil</span><span class="sxs-lookup"><span data-stu-id="0bba9-1351">Profile</span></span>

* <span data-ttu-id="0bba9-1352">Argument `--resource-type` zu `account get-access-token` zum Abrufen von Ressourcenzugriffstoken hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1352">Added `--resource-type` argument to `account get-access-token` to get resource access tokens</span></span>

### <a name="servicefabric"></a><span data-ttu-id="0bba9-1353">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="0bba9-1353">ServiceFabric</span></span>

* <span data-ttu-id="0bba9-1354">Alle unterstützten Betriebssystemversionen für „sf cluster create“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1354">Added all supported os version for sf cluster create</span></span>
* <span data-ttu-id="0bba9-1355">Fehler beim Überprüfen des primären Zertifikats behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-1355">Fixed primary certificate validation bug</span></span>

### <a name="storage"></a><span data-ttu-id="0bba9-1356">Storage</span><span class="sxs-lookup"><span data-stu-id="0bba9-1356">Storage</span></span>

* <span data-ttu-id="0bba9-1357">Befehl `storage copy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1357">Added command `storage copy`</span></span>

## <a name="july-30-2019"></a><span data-ttu-id="0bba9-1358">30. Juli 2019</span><span class="sxs-lookup"><span data-stu-id="0bba9-1358">July 30, 2019</span></span>

<span data-ttu-id="0bba9-1359">Version 2.0.70</span><span class="sxs-lookup"><span data-stu-id="0bba9-1359">Version 2.0.70</span></span>

### <a name="acr"></a><span data-ttu-id="0bba9-1360">ACR</span><span class="sxs-lookup"><span data-stu-id="0bba9-1360">ACR</span></span>

* <span data-ttu-id="0bba9-1361">Problem #9952 behoben (Regression im Befehl `acr pack build`)</span><span class="sxs-lookup"><span data-stu-id="0bba9-1361">Fixed issue #9952 (a regression in the `acr pack build` command)</span></span>
* <span data-ttu-id="0bba9-1362">Standardname des Generatorimages in `acr pack build` entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1362">Removed the default builder image name in `acr pack build`</span></span>

### <a name="appservice"></a><span data-ttu-id="0bba9-1363">AppService</span><span class="sxs-lookup"><span data-stu-id="0bba9-1363">Appservice</span></span>

* <span data-ttu-id="0bba9-1364">`webapp config ssl` geändert, um eine Meldung anzuzeigen, wenn eine Ressource nicht gefunden wurde</span><span class="sxs-lookup"><span data-stu-id="0bba9-1364">Changed `webapp config ssl` to show a message if a resource is not found</span></span>
* <span data-ttu-id="0bba9-1365">Problem behoben, aufgrund dessen `functionapp create` den Speicherkontotypen `Standard_RAGRS` nicht akzeptiert hat</span><span class="sxs-lookup"><span data-stu-id="0bba9-1365">Fixed issue where `functionapp create` does not accept `Standard_RAGRS` storage account type</span></span>
* <span data-ttu-id="0bba9-1366">Problem behoben, aufgrund dessen für `webapp up` ein Fehler auftrat, wenn für die Ausführung ältere Python-Versionen verwendet wurden</span><span class="sxs-lookup"><span data-stu-id="0bba9-1366">Fixed an issue where `webapp up` would fail if run using older versions of python</span></span>

### <a name="network"></a><span data-ttu-id="0bba9-1367">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0bba9-1367">Network</span></span>

* <span data-ttu-id="0bba9-1368">Ungültiger Parameter `--ids` aus `network nic ip-config add` entfernt (Fehlerbehebungen #9861)</span><span class="sxs-lookup"><span data-stu-id="0bba9-1368">Removed invalid parameter `--ids` from `network nic ip-config add` (fixes #9861)</span></span>
* <span data-ttu-id="0bba9-1369">Fehlerbehebungen #9604.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1369">Fixes #9604.</span></span> <span data-ttu-id="0bba9-1370">Parameter `--root-certs` zu `network application-gateway http-settings [create|update]` hinzugefügt, um vom Benutzer zugewiesene vertrauenswürdige Stammzertifikate zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1370">Added `--root-certs` parameter to `network application-gateway http-settings [create|update]` to support user associate trusted root certificates.</span></span>
* <span data-ttu-id="0bba9-1371">Argument `--subscription` für `network dns record-set ns create` korrigiert (#9965)</span><span class="sxs-lookup"><span data-stu-id="0bba9-1371">Fixed arguent `--subscription` for `network dns record-set ns create` (#9965)</span></span>

### <a name="rbac"></a><span data-ttu-id="0bba9-1372">RBAC</span><span class="sxs-lookup"><span data-stu-id="0bba9-1372">RBAC</span></span>

* <span data-ttu-id="0bba9-1373">Befehl `user update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1373">Added `user update` command</span></span>
* <span data-ttu-id="0bba9-1374">[VERALTET]`--upn-or-object-id` in benutzerbezogenen Befehlen als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-1374">[DEPRECATED] Deprecated `--upn-or-object-id` from user-related commands</span></span>
    * <span data-ttu-id="0bba9-1375">Verwenden Sie das Ersatzargument `--id`.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1375">Use replacement argument `--id`</span></span>
* <span data-ttu-id="0bba9-1376">Argument `--id` zu benutzerbezogenen Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1376">Added `--id` argument to user-related commands</span></span>

### <a name="sql"></a><span data-ttu-id="0bba9-1377">SQL</span><span class="sxs-lookup"><span data-stu-id="0bba9-1377">SQL</span></span>

* <span data-ttu-id="0bba9-1378">Verwaltungsbefehle für Schlüssel verwalteter Instanzen und TDE-Schutzvorrichtung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1378">Added management commands for managed instance keys and TDE protector</span></span>

### <a name="storage"></a><span data-ttu-id="0bba9-1379">Storage</span><span class="sxs-lookup"><span data-stu-id="0bba9-1379">Storage</span></span>

* <span data-ttu-id="0bba9-1380">Befehl `storage remove` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1380">Added `storage remove` command</span></span>
* <span data-ttu-id="0bba9-1381">Problem mit `storage blob update` behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-1381">Fixed an issue with `storage blob update`</span></span>

### <a name="vm"></a><span data-ttu-id="0bba9-1382">VM</span><span class="sxs-lookup"><span data-stu-id="0bba9-1382">VM</span></span>

* <span data-ttu-id="0bba9-1383">`list-skus` wurde geändert, um eine neuere API-Version für die Ausgabe von Zonendetails zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1383">Changed `list-skus` to use newer api-version to output zone details</span></span>
* <span data-ttu-id="0bba9-1384">Standardwert `--single-placement-group` für `vmss create` in `false` geändert</span><span class="sxs-lookup"><span data-stu-id="0bba9-1384">Changed default of `--single-placement-group` to `false` for `vmss create`</span></span>
* <span data-ttu-id="0bba9-1385">Möglichkeit zum Auswählen von ZRS-Speicher-SKUs für `[snapshot|disk] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1385">Added ability to select ZRS storage SKUs for `[snapshot|disk] create`</span></span>
* <span data-ttu-id="0bba9-1386">Neue Befehlsgruppe `vm host` zur Unterstützung dedizierter Hosts hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1386">Added new command group `vm host` to support dedicated hosts</span></span>
* <span data-ttu-id="0bba9-1387">Parameter `--host` und `--host-group` für `vm create` hinzugefügt, um den dedizierten VM-Host festzulegen</span><span class="sxs-lookup"><span data-stu-id="0bba9-1387">Added parameters `--host` and `--host-group` on `vm create` to set VM dedicated host</span></span>

## <a name="july-16-2019"></a><span data-ttu-id="0bba9-1388">16. Juli 2019</span><span class="sxs-lookup"><span data-stu-id="0bba9-1388">July 16, 2019</span></span>

<span data-ttu-id="0bba9-1389">Version 2.0.69</span><span class="sxs-lookup"><span data-stu-id="0bba9-1389">Version 2.0.69</span></span>

### <a name="appservice"></a><span data-ttu-id="0bba9-1390">AppService</span><span class="sxs-lookup"><span data-stu-id="0bba9-1390">Appservice</span></span>

* <span data-ttu-id="0bba9-1391">`webapp identity`-Befehle geändert, um eine korrekte Fehlermeldung zurückzugeben, wenn „ResourceGroupName“ oder der App-Name ungültig sind</span><span class="sxs-lookup"><span data-stu-id="0bba9-1391">Changed `webapp identity` commands to return a proper error message if ResourceGroupName or App name are invalid</span></span>
* <span data-ttu-id="0bba9-1392">`webapp list` korrigiert, sodass der korrekte Wert für „numberOfSites“ zurückgegeben wird, wenn „ResourceGroup“ nicht angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="0bba9-1392">Fixed `webapp list` to return the correct value for numberOfSites if no ResourceGroup was provided</span></span>
* <span data-ttu-id="0bba9-1393">Nebeneffekte von `appservice plan create` und `webapp create` behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-1393">Fixed side-effects of `appservice plan create` and `webapp create`</span></span>

### <a name="core"></a><span data-ttu-id="0bba9-1394">Core</span><span class="sxs-lookup"><span data-stu-id="0bba9-1394">Core</span></span>

* <span data-ttu-id="0bba9-1395">Problem behoben, aufgrund dessen `--subscription` angezeigt wurde, obwohl nicht anwendbar</span><span class="sxs-lookup"><span data-stu-id="0bba9-1395">Fixed issue where `--subscription` would appear despite being not applicable</span></span>

### <a name="batch"></a><span data-ttu-id="0bba9-1396">Batch</span><span class="sxs-lookup"><span data-stu-id="0bba9-1396">Batch</span></span>

* <span data-ttu-id="0bba9-1397">[BREAKING CHANGE]`batch pool node-agent-skus list` durch `batch pool supported-images list` ersetzt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1397">[BREAKING CHANGE] Replaced `batch pool node-agent-skus list` with `batch pool supported-images list`</span></span>
* <span data-ttu-id="0bba9-1398">Unterstützung für Sicherheitsregeln hinzugefügt, die den Netzwerkzugriff auf einen Pool basierend auf dem Quellport des Datenverkehrs blockieren, wenn die Option `--json-file` von `batch pool create network` verwendet wird</span><span class="sxs-lookup"><span data-stu-id="0bba9-1398">Added support for security rules blocking network access to a pool based on the source port of the traffic when using the `--json-file` option of `batch pool create network`</span></span>
* <span data-ttu-id="0bba9-1399">Unterstützung für die Ausführung der Aufgabe im Arbeitsverzeichnis des Containers oder der Batch-Aufgabe hinzugefügt, wenn die Option `--json-file` von `batch task create` verwendet wird</span><span class="sxs-lookup"><span data-stu-id="0bba9-1399">Added support for executing the task in the container working directory or in the Batch task working directory when using the `--json-file` option of `batch task create`</span></span>
* <span data-ttu-id="0bba9-1400">Fehler in Option `--application-package-references` von `batch pool create` behoben, aufgrund dessen nur Standardeinstellungen möglich waren</span><span class="sxs-lookup"><span data-stu-id="0bba9-1400">Fixed error in `--application-package-references` option of `batch pool create` where it would only work with defaults</span></span>

### <a name="eventhubs"></a><span data-ttu-id="0bba9-1401">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="0bba9-1401">Eventhubs</span></span>

* <span data-ttu-id="0bba9-1402">Validierung für Parameter `--rights` von `authorizationrule`-Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1402">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="rdbms"></a><span data-ttu-id="0bba9-1403">RDBMS</span><span class="sxs-lookup"><span data-stu-id="0bba9-1403">RDBMS</span></span>

* <span data-ttu-id="0bba9-1404">Optionaler Parameter zum Angeben der Replikat-SKU für den Befehl zum Erstellen von Replikaten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1404">Added optional parameter to specify replica SKU for create replica command</span></span>
* <span data-ttu-id="0bba9-1405">Problem mit CI-Testfehler bei der Erstellung von MySQL-Replikaten behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-1405">Fixed the issue with CI test failure with creating MySQL replica</span></span>

### <a name="relay"></a><span data-ttu-id="0bba9-1406">Relay</span><span class="sxs-lookup"><span data-stu-id="0bba9-1406">Relay</span></span>

* <span data-ttu-id="0bba9-1407">Problem mit Hybridverbindung behoben, wenn die Client-Autorisierung deaktiviert ist [#8775](https://github.com/azure/azure-cli/issues/8775)</span><span class="sxs-lookup"><span data-stu-id="0bba9-1407">Fixed issue with hybrid connection when client authroization disabled [#8775](https://github.com/azure/azure-cli/issues/8775)</span></span>
* <span data-ttu-id="0bba9-1408">Parameter `--requires-transport-security` zu `relay wcfrelay create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1408">Added parameter `--requires-transport-security` to `relay wcfrelay create`</span></span>

### <a name="servicebus"></a><span data-ttu-id="0bba9-1409">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="0bba9-1409">Servicebus</span></span>

* <span data-ttu-id="0bba9-1410">Validierung für Parameter `--rights` von `authorizationrule`-Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1410">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="storage"></a><span data-ttu-id="0bba9-1411">Storage</span><span class="sxs-lookup"><span data-stu-id="0bba9-1411">Storage</span></span>

* <span data-ttu-id="0bba9-1412">AADDS für Files für Speicherkontoaktualisierung aktiviert</span><span class="sxs-lookup"><span data-stu-id="0bba9-1412">Enable Files AADDS for storage account update</span></span>
* <span data-ttu-id="0bba9-1413">Problem `storage blob service-properties update --set` behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-1413">Fixed issue `storage blob service-properties update --set`</span></span>

## <a name="july-2-2019"></a><span data-ttu-id="0bba9-1414">2\. Juli 2019</span><span class="sxs-lookup"><span data-stu-id="0bba9-1414">July 2, 2019</span></span>

<span data-ttu-id="0bba9-1415">Version 2.0.68</span><span class="sxs-lookup"><span data-stu-id="0bba9-1415">Version 2.0.68</span></span>

### <a name="core"></a><span data-ttu-id="0bba9-1416">Core</span><span class="sxs-lookup"><span data-stu-id="0bba9-1416">Core</span></span>

* <span data-ttu-id="0bba9-1417">Befehlsmodule sind jetzt in einer einzelnen verteilbaren Python-Komponente zusammengefasst.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1417">Command modules are now consolidated into a single Python distributable.</span></span> <span data-ttu-id="0bba9-1418">Die direkte Verwendung zahlreicher Pakete vom Typ `azure-cli-` in PyPI ist daher veraltet.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1418">This deprecates direct use of many `azure-cli-` packages on PyPI.</span></span>
  <span data-ttu-id="0bba9-1419">Dadurch sollte sich die Installationsgröße reduzieren. Darüber hinaus sollte es nur Benutzer betreffen, die eine direkte Installation über `pip` ausgeführt haben.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1419">This should reduce install size and only affect users who have directly installed via `pip`.</span></span>

### <a name="acr"></a><span data-ttu-id="0bba9-1420">ACR</span><span class="sxs-lookup"><span data-stu-id="0bba9-1420">ACR</span></span>

* <span data-ttu-id="0bba9-1421">Unterstützung für Trigger mit Timer zu Aufgabe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1421">Added support for Timer Triggers to Task</span></span>

### <a name="appservice"></a><span data-ttu-id="0bba9-1422">AppService</span><span class="sxs-lookup"><span data-stu-id="0bba9-1422">Appservice</span></span>

* <span data-ttu-id="0bba9-1423">`functionapp create` wurde so geändert, das Application Insights standardmäßig aktiviert wird.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1423">Changed `functionapp create` to enable application insights by default</span></span>
* <span data-ttu-id="0bba9-1424">[BREAKING CHANGE] Veralteter Befehl `functionapp devops-build` entfernt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1424">[BREAKING CHANGE] Removed deprecated `functionapp devops-build` command.</span></span>
  *  <span data-ttu-id="0bba9-1425">Verwenden Sie stattdessen den neuen Befehl `az functionapp devops-pipeline`.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1425">Use the new command `az functionapp devops-pipeline` instead</span></span>
* <span data-ttu-id="0bba9-1426">Unterstützung des Funktions-App-Plans für Linux-Verbrauch zu `functionapp deployment config-zip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1426">Added Linux Consumption function app plan support to `functionapp deployment config-zip`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="0bba9-1427">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="0bba9-1427">Cosmos DB</span></span>

* <span data-ttu-id="0bba9-1428">Unterstützung für das Deaktivieren von TTL hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1428">Added support for disabling TTL</span></span>

### <a name="dls"></a><span data-ttu-id="0bba9-1429">DLS</span><span class="sxs-lookup"><span data-stu-id="0bba9-1429">DLS</span></span>

* <span data-ttu-id="0bba9-1430">Aktualisierte ADLS-Version (0.0.45)</span><span class="sxs-lookup"><span data-stu-id="0bba9-1430">Updated ADLS version (0.0.45)</span></span>

### <a name="feedback"></a><span data-ttu-id="0bba9-1431">Feedback</span><span class="sxs-lookup"><span data-stu-id="0bba9-1431">Feedback</span></span>

* <span data-ttu-id="0bba9-1432">Wird ein fehlgeschlagener Erweiterungsbefehl gemeldet, versucht `az feedback` nun, über den Index die Projekt-/Repository-URL der Erweiterung im Browser zu öffnen.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1432">When reporting a failed extension command, `az feedback` now attempts to open the browser to the project/repo url of the extension from the index</span></span>

### <a name="hdinsight"></a><span data-ttu-id="0bba9-1433">HDInsight</span><span class="sxs-lookup"><span data-stu-id="0bba9-1433">HDInsight</span></span>

* <span data-ttu-id="0bba9-1434">[BREAKING CHANGE] Der Befehlsgruppenname `oms` wurde in `monitor` geändert.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1434">[BREAKING CHANGE] Changed `oms` command group name to `monitor`</span></span>
* <span data-ttu-id="0bba9-1435">[BREAKING CHANGE]`--http-password/-p` als erforderlicher Parameter festgelegt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1435">[BREAKING CHANGE] Made `--http-password/-p` a required parameter</span></span> 
* <span data-ttu-id="0bba9-1436">Vervollständigungen für `--cluster-admin-account` und `cluster-users-group-dns` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1436">Added completers for `--cluster-admin-account` and `cluster-users-group-dns` parameters completer</span></span> 
* <span data-ttu-id="0bba9-1437">Parameter `cluster-users-group-dns` so geändert, dass er erforderlich ist, wenn `—esp` vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="0bba9-1437">Changed `cluster-users-group-dns` parameter to be required when `—esp` is present</span></span>
* <span data-ttu-id="0bba9-1438">Timeout für alle vorhandenen automatischen Argumentvervollständigungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1438">Added a timeout for all existing argument auto-completers</span></span>
* <span data-ttu-id="0bba9-1439">Timeout für das Transformieren des Ressourcennamens in eine Ressourcen-ID hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1439">Added a timeout for transforming resource name to resource id</span></span>
* <span data-ttu-id="0bba9-1440">Die automatischen Vervollständigungen wurden so geändert, dass Ressourcen aus einer beliebigen Ressourcengruppe ausgewählt werden.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1440">Changed Auto-completers to select resources from any resource group.</span></span> <span data-ttu-id="0bba9-1441">Dabei kann es sich um eine andere Ressourcengruppe als die mit `-g` angegebene Gruppe handeln.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1441">It can be a different resource group than the one specified with `-g`</span></span>
* <span data-ttu-id="0bba9-1442">Unterstützung für die Parameter `--sub-domain-suffix` und `--disable_gateway_auth` im Befehl `hdinsight application create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1442">Added support for `--sub-domain-suffix` and `--disable_gateway_auth` parameters in the `hdinsight application create` command</span></span>

### <a name="managed-services"></a><span data-ttu-id="0bba9-1443">Verwaltete Dienste</span><span class="sxs-lookup"><span data-stu-id="0bba9-1443">Managed Services</span></span>

* <span data-ttu-id="0bba9-1444">Befehlsmodul für verwaltete Dienste als Vorschau eingeführt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1444">Introducing managed service command module in preview</span></span>

### <a name="profile"></a><span data-ttu-id="0bba9-1445">Profil</span><span class="sxs-lookup"><span data-stu-id="0bba9-1445">Profile</span></span>
* <span data-ttu-id="0bba9-1446">Argument `--subscription` für Abmeldebefehl unterdrückt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1446">Suppress `--subscription` argument for logout command</span></span>

### <a name="rbac"></a><span data-ttu-id="0bba9-1447">RBAC</span><span class="sxs-lookup"><span data-stu-id="0bba9-1447">RBAC</span></span>

* <span data-ttu-id="0bba9-1448">[BREAKING CHANGE] Argument `--password` für `create-for-rbac` entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1448">[BREAKING CHANGE] Removed `--password` argument for `create-for-rbac`</span></span>
* <span data-ttu-id="0bba9-1449">Parameter `--assignee-principal-type` zum Befehl `create` hinzugefügt, um zeitweilige Fehler zu vermeiden, die durch die Replikationswartezeit des AAD-Graph-Servers verursacht werden</span><span class="sxs-lookup"><span data-stu-id="0bba9-1449">Added `--assignee-principal-type` parameter to `create` command to avoid intermittent failures caused by AAD graph server replication latency</span></span>
* <span data-ttu-id="0bba9-1450">Absturz in `ad signed-in-user` beim Auflisten von in Besitz befindlichen Objekten behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-1450">Fixed a crash in `ad signed-in-user` when listing owned objects</span></span>
* <span data-ttu-id="0bba9-1451">Problem behoben, aufgrund dessen `ad sp` nicht die richtige Anwendung über einen Dienstprinzipal fand</span><span class="sxs-lookup"><span data-stu-id="0bba9-1451">Fixed issue where `ad sp` would not find the right application from a service principal</span></span>

### <a name="rdbms"></a><span data-ttu-id="0bba9-1452">RDBMS</span><span class="sxs-lookup"><span data-stu-id="0bba9-1452">RDBMS</span></span>

* <span data-ttu-id="0bba9-1453">Unterstützung für die Replikation für MariaDB hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1453">Added support for replication for MariaDB</span></span>

### <a name="sql"></a><span data-ttu-id="0bba9-1454">SQL</span><span class="sxs-lookup"><span data-stu-id="0bba9-1454">SQL</span></span>

* <span data-ttu-id="0bba9-1455">Zulässige Werte für `sql db create --sample-name` dokumentiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-1455">Documented allowed values for `sql db create --sample-name`</span></span>

### <a name="storage"></a><span data-ttu-id="0bba9-1456">Storage</span><span class="sxs-lookup"><span data-stu-id="0bba9-1456">Storage</span></span>

* <span data-ttu-id="0bba9-1457">Unterstützung von SAS-Token für die Benutzerdelegierung mit `--as-user` zu `storage blob generate-sas` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1457">Added user delegation SAS token support with `--as-user` to `storage blob generate-sas`</span></span> 
* <span data-ttu-id="0bba9-1458">Unterstützung von SAS-Token für die Benutzerdelegierung mit `--as-user` zu `storage container generate-sas` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1458">Added user delegation SAS token support with `--as-user` to `storage container generate-sas`</span></span> 

### <a name="vm"></a><span data-ttu-id="0bba9-1459">VM</span><span class="sxs-lookup"><span data-stu-id="0bba9-1459">VM</span></span>

* <span data-ttu-id="0bba9-1460">Fehler behoben, aufgrund dessen `vmss create` bei der Ausführung mit `--no-wait` eine Fehlermeldung zurückgab</span><span class="sxs-lookup"><span data-stu-id="0bba9-1460">Fixed bug where `vmss create` returns an error message when run with `--no-wait`</span></span>
* <span data-ttu-id="0bba9-1461">Die clientseitige Validierung für `vmss create --single-placement-group` wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1461">Removed client-side validation for `vmss create --single-placement-group`.</span></span> <span data-ttu-id="0bba9-1462">Es tritt kein Fehler auf, wenn `--single-placement-group` auf `true` und für `--instance-count` ein größerer Wert als 100 festgelegt wird oder wenn Verfügbarkeitszonen angegeben werden. Diese Validierung wird jedoch dem Computedienst überlassen.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1462">Does not fail if `--single-placement-group` is set to `true` and`--instance-count` is greater than 100 or availability zones are specified, but leaves this validation to the compute service</span></span>
* <span data-ttu-id="0bba9-1463">Problem behoben, aufgrund dessen bei der Verwendung von `--latest` für `[vm|vmss] extension image list` ein Fehler auftrat</span><span class="sxs-lookup"><span data-stu-id="0bba9-1463">Fixed bug where `[vm|vmss] extension image list` fails when used with `--latest`</span></span>


## <a name="june-18-2019"></a><span data-ttu-id="0bba9-1464">18. Juni 2019</span><span class="sxs-lookup"><span data-stu-id="0bba9-1464">June 18, 2019</span></span>

<span data-ttu-id="0bba9-1465">Version 2.0.67</span><span class="sxs-lookup"><span data-stu-id="0bba9-1465">Version 2.0.67</span></span>

### <a name="core"></a><span data-ttu-id="0bba9-1466">Core</span><span class="sxs-lookup"><span data-stu-id="0bba9-1466">Core</span></span>

<span data-ttu-id="0bba9-1467">In diesem Release wird das neue [Preview]-Tag eingeführt, um Kunden gegenüber deutlich zu machen, dass sich eine Befehlsgruppe, ein Befehl oder ein Argument in der Vorschauphase befindet.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1467">This release introduces a new [Preview] tag to more clearly communicate to customers when a command group, command or argument is in preview status.</span></span> <span data-ttu-id="0bba9-1468">Diese Information war zuvor im Hilfetext oder implizit durch die Versionsnummer des Befehlsmoduls angegeben.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1468">This was previously called out in help text or communicated implicitly by the command module version number.</span></span>
<span data-ttu-id="0bba9-1469">Die Befehlszeilenschnittstelle wird künftig Versionsnummern für einzelne Pakete entfernen.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1469">The CLI will be removing version numbers for individual packages in the future.</span></span> <span data-ttu-id="0bba9-1470">Wenn sich ein Befehl in der Vorschauphase befindet, gilt dies auch für alle seine Argumente.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1470">If a command is in preview, all of its arguments are as well.</span></span> <span data-ttu-id="0bba9-1471">Wenn eine Befehlsgruppe als Vorschau gekennzeichnet ist, befinden sich auch alle Befehle und Argumente in der Vorschauphase.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1471">If a command group is labeled as being in preview, then all commands and arguments are considered to be in preview as well.</span></span>

<span data-ttu-id="0bba9-1472">Infolge dieser Änderung befinden sich in diesem Release verschiedene Befehlsgruppen anscheinend „plötzlich“ in der Vorschauphase.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1472">As a result of this change, several command groups may seem to "suddenly" appear to be in a preview status with this release.</span></span> <span data-ttu-id="0bba9-1473">Tatsächlich ist es jedoch so, dass sich die meisten Pakete in der Vorschauphase befanden, in diesem Release jedoch als allgemein verfügbar gelten.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1473">What actually happened is that most packages were in a preview status, but are being deemed GA with this release</span></span>

### <a name="acr"></a><span data-ttu-id="0bba9-1474">ACR</span><span class="sxs-lookup"><span data-stu-id="0bba9-1474">ACR</span></span>
* <span data-ttu-id="0bba9-1475">Befehl „acr check-health“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1475">Added 'acr check-health' command</span></span>
* <span data-ttu-id="0bba9-1476">Verbesserte Fehlerbehandlung für AAD-Token und für das Abrufen externer Befehle</span><span class="sxs-lookup"><span data-stu-id="0bba9-1476">Improved error handling for AAD tokens and for retrieving external commands</span></span>

### <a name="acs"></a><span data-ttu-id="0bba9-1477">ACS</span><span class="sxs-lookup"><span data-stu-id="0bba9-1477">ACS</span></span>
* <span data-ttu-id="0bba9-1478">Veraltete ACS-Befehle werden jetzt in der Hilfeansicht ausgeblendet.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1478">Deprecated ACS commands are now hidden from help view</span></span>

### <a name="ams"></a><span data-ttu-id="0bba9-1479">AMS</span><span class="sxs-lookup"><span data-stu-id="0bba9-1479">AMS</span></span>
* <span data-ttu-id="0bba9-1480">[BREAKING CHANGE] Änderung, damit ISO 8601-Zeitzeichenfolgen für „archive-window-length“ und „key-frame-interval-duration“ zurückgegeben werden</span><span class="sxs-lookup"><span data-stu-id="0bba9-1480">[BREAKING CHANGE] Changed to return ISO 8601 time strings for archive-window-length and key-frame-interval-duration</span></span>

### <a name="appservice"></a><span data-ttu-id="0bba9-1481">AppService</span><span class="sxs-lookup"><span data-stu-id="0bba9-1481">AppService</span></span>
* <span data-ttu-id="0bba9-1482">Standortbasiertes Routing für `webapp deleted list` und `webapp deleted restore` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1482">Added location based routing for `webapp deleted list` and `webapp deleted restore`</span></span>
* <span data-ttu-id="0bba9-1483">Problem behoben, aufgrund dessen in Azure Cloud Shell nicht auf die von einer Web-App protokollierte Ziel-URL („Sie können die App starten unter...“) geklickt werden konnte</span><span class="sxs-lookup"><span data-stu-id="0bba9-1483">Fixed issue where webapp up logged target URL ("You can launch the app at...") was not clickable in Azure Cloud Shell</span></span>
* <span data-ttu-id="0bba9-1484">Problem behoben, aufgrund dessen beim Erstellen von Apps bei einigen SKUs ein AlwaysOn-Fehler auftrat</span><span class="sxs-lookup"><span data-stu-id="0bba9-1484">Fixed an issue where creating apps with the some SKUs was failing with an AlwaysOn error</span></span>
* <span data-ttu-id="0bba9-1485">Vorabüberprüfung zu `[appservice|webapp] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1485">Added pre-validation to `[appservice|webapp] create`</span></span>
* <span data-ttu-id="0bba9-1486">`[webapp|functionapp] traffic-routing` korrigiert, damit der richtige actionHostName-Wert verwendet wird</span><span class="sxs-lookup"><span data-stu-id="0bba9-1486">Fixed `[webapp|functionapp] traffic-routing` to use the correct actionHostName</span></span>
* <span data-ttu-id="0bba9-1487">Slotunterstützung zu `functionapp`-Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1487">Added slot support to `functionapp` commands</span></span>

### <a name="batch"></a><span data-ttu-id="0bba9-1488">Batch</span><span class="sxs-lookup"><span data-stu-id="0bba9-1488">Batch</span></span>
* <span data-ttu-id="0bba9-1489">AAD-Authentifizierungsregression korrigiert, die von übermäßiger Berichterstellung für Authentifizierung mit gemeinsam verwendetem Schlüssel verursacht wurde</span><span class="sxs-lookup"><span data-stu-id="0bba9-1489">Fixed AAD auth regression caused by over-aggressive error reporting for Shared Key Auth</span></span>

### <a name="batchai"></a><span data-ttu-id="0bba9-1490">Batch AI</span><span class="sxs-lookup"><span data-stu-id="0bba9-1490">BatchAI</span></span>
* <span data-ttu-id="0bba9-1491">BatchAI-Befehle sind jetzt veraltet und ausgeblendet.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1491">BatchAI commands are now deprecated and hidden</span></span>

### <a name="botservice"></a><span data-ttu-id="0bba9-1492">BotService</span><span class="sxs-lookup"><span data-stu-id="0bba9-1492">BotService</span></span>
* <span data-ttu-id="0bba9-1493">Für Befehle, die Version 3 des SDK unterstützen, wurden die Warnmeldungen „Support eingestellt“/„Wartungsmodus“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1493">Added "discontinued support"/"maintenance mode" warning messages for commands that support the v3 SDK</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="0bba9-1494">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="0bba9-1494">CosmosDB</span></span>
* <span data-ttu-id="0bba9-1495">[VERALTET] Der Befehl `cosmosdb list-keys` wurde als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1495">[DEPRECATED] Deprecated the `cosmosdb list-keys` command</span></span>
* <span data-ttu-id="0bba9-1496">Befehl `cosmosdb keys list` hinzugefügt, er ersetzt `cosmosdb list-keys`.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1496">Added the `cosmosdb keys list` command - replaces `cosmosdb list-keys`</span></span>
* <span data-ttu-id="0bba9-1497">`cosmsodb create/update`: Neues Format für „--location“ hinzugefügt, um das Festlegen der Eigenschaft „isZoneRedundant“ zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="0bba9-1497">`cosmsodb create/update`: Added new format for --location to allow setting "isZoneRedundant" property.</span></span> <span data-ttu-id="0bba9-1498">Das alte Format wurde als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1498">Deprecated old format</span></span>

### <a name="eventgrid"></a><span data-ttu-id="0bba9-1499">EventGrid</span><span class="sxs-lookup"><span data-stu-id="0bba9-1499">EventGrid</span></span>
* <span data-ttu-id="0bba9-1500">`eventgrid domain`-Befehle für CRUD-Vorgänge für Domänen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1500">Added `eventgrid domain` commands for domain CRUD operations</span></span>
* <span data-ttu-id="0bba9-1501">`eventgrid domain topic`-Befehle für CRUD-Vorgänge für Domänenthemen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1501">Added `eventgrid domain topic` commands for domain topics CRUD operations</span></span>
* <span data-ttu-id="0bba9-1502">Argument `--odata-query` zu `eventgrid [topic|event-subscription] list` zum Filtern der Ergebnisse mithilfe von OData-Syntax hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1502">Added `--odata-query` argument to `eventgrid [topic|event-subscription] list` for filtering results using OData syntax</span></span>
* <span data-ttu-id="0bba9-1503">`event-subscription create/update`: „servicebusqueue“ als neue Werte für den Parameter `--endpoint-type` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1503">`event-subscription create/update`: Added servicebusqueue as new values for the `--endpoint-type` parameter</span></span>
* <span data-ttu-id="0bba9-1504">[BREAKING CHANGE] Unterstützung für `--included-event-types All` mit `eventgrid event-subscription [create|update]` entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1504">[BREAKING CHANGE] Removed support for `--included-event-types All` with `eventgrid event-subscription [create|update]`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="0bba9-1505">HDInsight</span><span class="sxs-lookup"><span data-stu-id="0bba9-1505">HDInsight</span></span>
* <span data-ttu-id="0bba9-1506">Unterstützung für den Parameter `--ssh-public-key` im Befehl vom Typ `hdinsight create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1506">Added support for `--ssh-public-key` parameter in `hdinsight create` command</span></span>

### <a name="iot"></a><span data-ttu-id="0bba9-1507">IoT</span><span class="sxs-lookup"><span data-stu-id="0bba9-1507">IoT</span></span>
* <span data-ttu-id="0bba9-1508">Unterstützung für das erneute Generieren von Autorisierungsrichtlinienschlüsseln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1508">Added support to regenerate authorization policy keys</span></span>
* <span data-ttu-id="0bba9-1509">SDK und Unterstützung für den Bereitstellungsdienst des DigitalTwin-Repositorys hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1509">Added SDK and support for DigitalTwin Repository Provisioning Service</span></span>

### <a name="network"></a><span data-ttu-id="0bba9-1510">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0bba9-1510">Network</span></span>
* <span data-ttu-id="0bba9-1511">Zonenunterstützung für NAT Gateway hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1511">Added Zone support for Nat Gateway</span></span>
* <span data-ttu-id="0bba9-1512">Befehl `network list-service-tags` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1512">Added command `network list-service-tags`</span></span>
* <span data-ttu-id="0bba9-1513">Problem mit `dns zone import` behoben, aufgrund dessen Benutzer keine A-Platzhaltereinträge importieren konnten</span><span class="sxs-lookup"><span data-stu-id="0bba9-1513">Fixed issue with `dns zone import` where users could not import wildcard A records</span></span>
* <span data-ttu-id="0bba9-1514">Problem mit `watcher flow-log configure` behoben, aufgrund dessen die Flowprotokollierung in bestimmten Regionen nicht aktiviert werden konnte</span><span class="sxs-lookup"><span data-stu-id="0bba9-1514">Fixed issue with `watcher flow-log configure` where flow logging could not be enabled in certain regions</span></span>

### <a name="resource"></a><span data-ttu-id="0bba9-1515">Resource</span><span class="sxs-lookup"><span data-stu-id="0bba9-1515">Resource</span></span>
* <span data-ttu-id="0bba9-1516">Befehl `az rest` zum Ausführen von REST-Aufrufen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1516">Added `az rest` command for making REST calls</span></span>
* <span data-ttu-id="0bba9-1517">Fehler behoben, der bei Verwendung von `policy assignment list` mit `--scope` auf Ressourcengruppen- oder Abonnementebene auftrat</span><span class="sxs-lookup"><span data-stu-id="0bba9-1517">Fixed error when using `policy assignment list` with a resource group or subscription level `--scope`</span></span>

### <a name="servicebus"></a><span data-ttu-id="0bba9-1518">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="0bba9-1518">ServiceBus</span></span>
* <span data-ttu-id="0bba9-1519">Problem mit `servicebus topic create --max-size` behoben [Nr. 9319](https://github.com/azure/azure-cli/issues/9319)</span><span class="sxs-lookup"><span data-stu-id="0bba9-1519">Fixed issue with `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span></span>

### <a name="sql"></a><span data-ttu-id="0bba9-1520">SQL</span><span class="sxs-lookup"><span data-stu-id="0bba9-1520">SQL</span></span>
* <span data-ttu-id="0bba9-1521">`--location` wurde geändert und ist nun für `sql [server|mi] create` optional. Ohne Angabe wird der Ressourcengruppenstandort verwendet.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1521">Changed `--location` to be optional for `sql [server|mi] create` - uses resource group location if not specified</span></span>
* <span data-ttu-id="0bba9-1522">Der Fehler, dass das Objekt „NoneType“ nicht wiederholbar ist, wurde für `sql db list-editions --available` behoben.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1522">Fixed "'NoneType' object is not iterable" error for `sql db list-editions --available`</span></span>

### <a name="sqlvm"></a><span data-ttu-id="0bba9-1523">SQLVm</span><span class="sxs-lookup"><span data-stu-id="0bba9-1523">SQLVm</span></span>
* <span data-ttu-id="0bba9-1524">[WICHTIGE ÄNDERUNG] `sql vm create` wurde geändert und erfordert nun den Parameter `--license-type`.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1524">[BREAKING CHNAGE] Changed `sql vm create` to require `--license-type` parameter</span></span>
* <span data-ttu-id="0bba9-1525">Änderung, um beim Erstellen oder Aktualisieren einer SQL-VM das Festlegen der SQL-Image-SKU zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="0bba9-1525">Changed to allow setting SQL image SKU when creating or updating a sql vm</span></span>

### <a name="storage"></a><span data-ttu-id="0bba9-1526">Storage</span><span class="sxs-lookup"><span data-stu-id="0bba9-1526">Storage</span></span>
* <span data-ttu-id="0bba9-1527">Problem mit fehlendem Kontoschlüssel für `storage container generate-sas` behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-1527">Fixed issue with missing account key for `storage container generate-sas`</span></span>
* <span data-ttu-id="0bba9-1528">Problem mit `storage blob sync` unter Linux behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-1528">Fixed issue with `storage blob sync` on Linux</span></span>

### <a name="vm"></a><span data-ttu-id="0bba9-1529">VM</span><span class="sxs-lookup"><span data-stu-id="0bba9-1529">VM</span></span>
* <span data-ttu-id="0bba9-1530">[VORSCHAU] Befehle vom Typ `vm image template` zum Erstellen von VM-Images hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1530">[PREVIEW] Added `vm image template` commands to build VM images</span></span>

## <a name="june-4-2019"></a><span data-ttu-id="0bba9-1531">4\. Juni 2019</span><span class="sxs-lookup"><span data-stu-id="0bba9-1531">June 4, 2019</span></span>

<span data-ttu-id="0bba9-1532">Version 2.0.66</span><span class="sxs-lookup"><span data-stu-id="0bba9-1532">Version 2.0.66</span></span>

### <a name="core"></a><span data-ttu-id="0bba9-1533">Core</span><span class="sxs-lookup"><span data-stu-id="0bba9-1533">Core</span></span>
* <span data-ttu-id="0bba9-1534">Fehler behoben, aufgrund dessen bei Befehlen ein Fehler auftrat, wenn `--output yaml` mit `--query` verwendet wurde</span><span class="sxs-lookup"><span data-stu-id="0bba9-1534">Fixed bug where commands fail if `--output yaml` is used with `--query`</span></span>

### <a name="acr"></a><span data-ttu-id="0bba9-1535">ACR</span><span class="sxs-lookup"><span data-stu-id="0bba9-1535">ACR</span></span>
* <span data-ttu-id="0bba9-1536">Befehlsgruppe „acr pack“ zum Erstellen von Aufgaben zur Schnellerstellung mit Buildpacks hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1536">Added 'acr pack' command group for creating quick build Tasks using Buildpacks.</span></span>

### <a name="acs"></a><span data-ttu-id="0bba9-1537">ACS</span><span class="sxs-lookup"><span data-stu-id="0bba9-1537">ACS</span></span>
* <span data-ttu-id="0bba9-1538">Zulassen der Aktivierung/Deaktivierung des AKS-Add-Ons für das Kube-Dashboard</span><span class="sxs-lookup"><span data-stu-id="0bba9-1538">Allow enabling/disabling AKS kube-dashboard addon</span></span>
* <span data-ttu-id="0bba9-1539">Ausgeben einer benutzerfreundlichen Nachricht, wenn das Abonnement nicht in der Whitelist zur Verwendung von Azure Red Hat OpenShift enthalten ist</span><span class="sxs-lookup"><span data-stu-id="0bba9-1539">Print a friendly message when the subscription is not whitelisted to use Azure Red Hat OpenShift</span></span>

### <a name="batch"></a><span data-ttu-id="0bba9-1540">Batch</span><span class="sxs-lookup"><span data-stu-id="0bba9-1540">Batch</span></span>
* <span data-ttu-id="0bba9-1541">Bessere Fehlerbehandlung, wenn der Benutzer nicht bei einem Konto angemeldet ist \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span><span class="sxs-lookup"><span data-stu-id="0bba9-1541">Improved error handling when not logged in to an account \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span></span>

### <a name="iot"></a><span data-ttu-id="0bba9-1542">IoT</span><span class="sxs-lookup"><span data-stu-id="0bba9-1542">IoT</span></span>
* <span data-ttu-id="0bba9-1543">Unterstützung für manuelles Failover hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1543">Added support for manual failover</span></span>

### <a name="network"></a><span data-ttu-id="0bba9-1544">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0bba9-1544">Network</span></span>
* <span data-ttu-id="0bba9-1545">Befehle vom Typ `network application-gateway waf-policy` hinzugefügt, um benutzerdefinierte WAF-Regeln zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="0bba9-1545">Added `network application-gateway waf-policy` commands to support custom WAF rules.</span></span>
* <span data-ttu-id="0bba9-1546">Argumente `--waf-policy` und `--max-capacity` zu `network application-gateway [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1546">Added `--waf-policy` and `--max-capacity` arguments to `network application-gateway [create|update]`</span></span> 

### <a name="resource"></a><span data-ttu-id="0bba9-1547">Resource</span><span class="sxs-lookup"><span data-stu-id="0bba9-1547">Resource</span></span>
* <span data-ttu-id="0bba9-1548">Verbesserte Fehlermeldungen aus `deployment create`, wenn TTY nicht verfügbar ist</span><span class="sxs-lookup"><span data-stu-id="0bba9-1548">Improved error message from `deployment create` when there is no TTY available</span></span>

### <a name="role"></a><span data-ttu-id="0bba9-1549">Role</span><span class="sxs-lookup"><span data-stu-id="0bba9-1549">Role</span></span>
* <span data-ttu-id="0bba9-1550">Hilfetext aktualisiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-1550">Updated help text.</span></span>

### <a name="compute"></a><span data-ttu-id="0bba9-1551">Compute</span><span class="sxs-lookup"><span data-stu-id="0bba9-1551">Compute</span></span>
* <span data-ttu-id="0bba9-1552">Unterstützung zu `vm create` für virtuelle Computer aus einem verwalteten Image mit Datenträger-LUNs hinzugefügt, die nicht bei 0 beginnen oder die Nummern überspringen</span><span class="sxs-lookup"><span data-stu-id="0bba9-1552">Added support to `vm create` for VMs from a managed image with data-disk luns that do not start from 0 or that skip numbers</span></span>

## <a name="may-21-2019"></a><span data-ttu-id="0bba9-1553">21. Mai 2019</span><span class="sxs-lookup"><span data-stu-id="0bba9-1553">May 21, 2019</span></span>

<span data-ttu-id="0bba9-1554">Version 2.0.65</span><span class="sxs-lookup"><span data-stu-id="0bba9-1554">Version 2.0.65</span></span>

### <a name="core"></a><span data-ttu-id="0bba9-1555">Core</span><span class="sxs-lookup"><span data-stu-id="0bba9-1555">Core</span></span>
* <span data-ttu-id="0bba9-1556">Besseres Feedback für Authentifizierungsfehler hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1556">Added better feedback for authentication errors</span></span>
* <span data-ttu-id="0bba9-1557">Problem behoben, aufgrund dessen die CLI Erweiterungen lädt, die nicht mit der Core-Version kompatibel waren</span><span class="sxs-lookup"><span data-stu-id="0bba9-1557">Fixed issue where the CLI would load extensions that were not compatible with its core version</span></span>
* <span data-ttu-id="0bba9-1558">Problem beim Starten behoben, wenn `clouds.config` beschädigt ist</span><span class="sxs-lookup"><span data-stu-id="0bba9-1558">Fixed issue with launching when `clouds.config` is corrupted</span></span>

### <a name="acr"></a><span data-ttu-id="0bba9-1559">ACR</span><span class="sxs-lookup"><span data-stu-id="0bba9-1559">ACR</span></span>
* <span data-ttu-id="0bba9-1560">Unterstützung für verwaltete Identitäten zu Aufgaben hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1560">Added support for Managed Identities to Tasks</span></span>

### <a name="acs"></a><span data-ttu-id="0bba9-1561">ACS</span><span class="sxs-lookup"><span data-stu-id="0bba9-1561">ACS</span></span>
* <span data-ttu-id="0bba9-1562">`openshift create`-Befehl bei der Verwendung mit dem AAD-Kundenclient korrigiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-1562">Fixed `openshift create` command when used with customer AAD client</span></span>

### <a name="appservice"></a><span data-ttu-id="0bba9-1563">AppService</span><span class="sxs-lookup"><span data-stu-id="0bba9-1563">AppService</span></span>
* <span data-ttu-id="0bba9-1564">[VERALTET] Befehl `functionapp devops-build` als veraltet gekennzeichnet – wird in der nächsten Version entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1564">[DEPRECATED] Deprecated `functionapp devops-build` command - will be removed in next release</span></span>
* <span data-ttu-id="0bba9-1565">`functionapp devops-pipeline` geändert, um das Buildprotokoll von Azure DevOps im ausführlichen Modus abzurufen</span><span class="sxs-lookup"><span data-stu-id="0bba9-1565">Changed `functionapp devops-pipeline` to fetch build log from Azure DevOps in verbose mode</span></span>
* <span data-ttu-id="0bba9-1566">[BREAKING CHANGE] Flag `--use_local_settings` aus dem Befehl `functionapp devops-pipeline` entfernt – kein Vorgang wurde ausgeführt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1566">[BREAKING CHANGE] Removed `--use_local_settings` flag from `functionapp devops-pipeline` command - was a no-op</span></span>
* <span data-ttu-id="0bba9-1567">`webapp up` geändert, sodass die JSON-Ausgabe zurückgegeben wird, wenn `--logs` nicht verwendet wird</span><span class="sxs-lookup"><span data-stu-id="0bba9-1567">Changed `webapp up` to return JSON output if `--logs` is not used</span></span>
* <span data-ttu-id="0bba9-1568">Unterstützung hinzugefügt zum Schreiben von Standardressourcen in die lokale Konfiguration für `webapp up`</span><span class="sxs-lookup"><span data-stu-id="0bba9-1568">Added support for writing default resources to local config for `webapp up`</span></span>
* <span data-ttu-id="0bba9-1569">Unterstützung zu `webapp up` hinzugefügt für die erneute Bereitstellung einer App ohne Verwendung des `--location`-Arguments</span><span class="sxs-lookup"><span data-stu-id="0bba9-1569">Added support to `webapp up` for redeploying an app without using the `--location` argument</span></span>
* <span data-ttu-id="0bba9-1570">Problem behoben, bei dem für die ASP-Erstellung der Linux-SKU „Free“ der SKU-Wert „Free“ nicht funktioniert hat</span><span class="sxs-lookup"><span data-stu-id="0bba9-1570">Fixed an issue where for Linux Free SKU ASP creation use Free as SKU value was not working</span></span>

### <a name="botservice"></a><span data-ttu-id="0bba9-1571">BotService</span><span class="sxs-lookup"><span data-stu-id="0bba9-1571">BotService</span></span>
* <span data-ttu-id="0bba9-1572">Geändert, sodass Groß-/Kleinschreibung für `--lang`-Parameter für Befehle zulässig ist</span><span class="sxs-lookup"><span data-stu-id="0bba9-1572">Changed to allow all casing for `--lang` parameters for commands</span></span>
* <span data-ttu-id="0bba9-1573">Beschreibung für das Befehlsmodul aktualisiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-1573">Updated description for command module</span></span>

### <a name="consumption"></a><span data-ttu-id="0bba9-1574">Nutzung</span><span class="sxs-lookup"><span data-stu-id="0bba9-1574">Consumption</span></span>
* <span data-ttu-id="0bba9-1575">Fehlende erforderliche Parameter bei der Ausführung von `consumption usage list --billing-period-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1575">Added missing required parameter when running `consumption usage list --billing-period-name`</span></span>

### <a name="iot"></a><span data-ttu-id="0bba9-1576">IoT</span><span class="sxs-lookup"><span data-stu-id="0bba9-1576">IoT</span></span>
* <span data-ttu-id="0bba9-1577">Unterstützung für das Auflisten aller Schlüssel hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1577">Added support to list all keys</span></span>

### <a name="network"></a><span data-ttu-id="0bba9-1578">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0bba9-1578">Network</span></span>
* [BREAKING CHANGE]: Removed `network interface-endpoints` command group - use `network private-endpoints` 
* <span data-ttu-id="0bba9-1580">`--nat-gateway`-Argument zu `network vnet subnet [create|update]` für das Anfügen an ein NAT-Gateway hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1580">Added `--nat-gateway` argument to `network vnet subnet [create|update]` for attaching to a NAT gateway</span></span>
* <span data-ttu-id="0bba9-1581">Problem mit `dns zone import` behoben, aufgrund dessen Eintragsnamen keinem Datensatztyp entsprochen haben</span><span class="sxs-lookup"><span data-stu-id="0bba9-1581">Fixed issue with `dns zone import` where record names could not match a record type</span></span>

### <a name="rdbms"></a><span data-ttu-id="0bba9-1582">RDBMS</span><span class="sxs-lookup"><span data-stu-id="0bba9-1582">RDBMS</span></span>
* <span data-ttu-id="0bba9-1583">Postgres- und MySLQ-Unterstützung für die Georeplikation hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1583">Added postgres and mysql support for geo replication</span></span>

### <a name="rbac"></a><span data-ttu-id="0bba9-1584">RBAC</span><span class="sxs-lookup"><span data-stu-id="0bba9-1584">RBAC</span></span>
* <span data-ttu-id="0bba9-1585">Unterstützung für den Verwaltungsgruppenumfang zu `role assignment` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1585">Added support for management group scope to `role assignment`</span></span>

### <a name="storage"></a><span data-ttu-id="0bba9-1586">Storage</span><span class="sxs-lookup"><span data-stu-id="0bba9-1586">Storage</span></span>
* <span data-ttu-id="0bba9-1587">`storage blob sync`: Synchronisierungsbefehl für Speicherblob hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1587">`storage blob sync`: add sync command for storage blob</span></span>

### <a name="compute"></a><span data-ttu-id="0bba9-1588">Compute</span><span class="sxs-lookup"><span data-stu-id="0bba9-1588">Compute</span></span>
* <span data-ttu-id="0bba9-1589">`--computer-name` zu `vm create` zum Festlegen des Computernamens eines virtuellen Computers hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1589">Added `--computer-name` to `vm create` for setting a VM's computer name</span></span>
* <span data-ttu-id="0bba9-1590">`--ssh-key-value` umbenannt in `--ssh-key-values` für `[vm|vmss] create`: Jetzt können mehrere öffentliche SSH-Schlüsselwerte oder -pfade akzeptiert werden.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1590">Renamed `--ssh-key-value` renamed to `--ssh-key-values` for `[vm|vmss] create` - can now accept multiple ssh public key values or paths</span></span>
  * <span data-ttu-id="0bba9-1591">__Hinweis__: Dies ist **kein** Breaking Change: `--ssh-key-value` wird korrekt analysiert, da nur eine Übereinstimmung mit `--ssh-key-values` besteht.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1591">__Note__: This is **not** a breaking change - `--ssh-key-value` will be parsed correctly as it matches only `--ssh-key-values`</span></span>
* <span data-ttu-id="0bba9-1592">`--type`-Argument von `ppg create` in optionales Argument geändert</span><span class="sxs-lookup"><span data-stu-id="0bba9-1592">Changed the `--type` argument of `ppg create` to be optional</span></span>

## <a name="may-6-2019"></a><span data-ttu-id="0bba9-1593">6\. Mai 2019</span><span class="sxs-lookup"><span data-stu-id="0bba9-1593">May 6, 2019</span></span>

<span data-ttu-id="0bba9-1594">Version 2.0.64</span><span class="sxs-lookup"><span data-stu-id="0bba9-1594">Version 2.0.64</span></span>

### <a name="acs"></a><span data-ttu-id="0bba9-1595">ACS</span><span class="sxs-lookup"><span data-stu-id="0bba9-1595">ACS</span></span>
* <span data-ttu-id="0bba9-1596">[BREAKING CHANGE] Flag `--fqdn` aus den `openshift`-Befehlen entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1596">[BREAKING CHANGE] Removed `--fqdn` flag on `openshift` commands</span></span>
* <span data-ttu-id="0bba9-1597">Geändert, sodass die allgemein verfügbare Azure Red Hat Openshift-API-Version verwendet wird</span><span class="sxs-lookup"><span data-stu-id="0bba9-1597">Changed to use Azure Red Hat Openshift GA API Version</span></span>
* <span data-ttu-id="0bba9-1598">Flag `customer-admin-group-id` wurde zu `openshift create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1598">Added `customer-admin-group-id` flag to `openshift create`</span></span>
* <span data-ttu-id="0bba9-1599">[ALLGEMEIN VERFÜGBAR] `(PREVIEW)` aus der `aks create`-Option `--network-policy` entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1599">[GA] Removed `(PREVIEW)` from `aks create` option `--network-policy`</span></span>

### <a name="appservice"></a><span data-ttu-id="0bba9-1600">AppService</span><span class="sxs-lookup"><span data-stu-id="0bba9-1600">Appservice</span></span>
* <span data-ttu-id="0bba9-1601">[VERALTET] Befehl `functionapp devops-build` als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="0bba9-1601">[DEPRECATED] Deprecated `functionapp devops-build` command</span></span>
  * <span data-ttu-id="0bba9-1602">Umbenannt in `functionapp devops-pipeline`</span><span class="sxs-lookup"><span data-stu-id="0bba9-1602">Renamed to `functionapp devops-pipeline`</span></span>
* <span data-ttu-id="0bba9-1603">Fehler beim Abrufen des richtigen Benutzernamens für Cloud Shell behoben, der einen Fehler von `webapp up` verursachte</span><span class="sxs-lookup"><span data-stu-id="0bba9-1603">Fixed getting the correct username for cloudshell which was causing `webapp up` to fail</span></span>
* <span data-ttu-id="0bba9-1604">Dokumentation von `appservice plan --sku` mit den unterstützten App Service-Plänen aktualisiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-1604">Updated `appservice plan --sku` documentation updated to reflect the supported appserviceplans</span></span>
* <span data-ttu-id="0bba9-1605">Optionale Argumente für Ressourcengruppe und Plan zu `webapp up` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1605">Added optional arguments for resource group and plan to `webapp up`</span></span>
* <span data-ttu-id="0bba9-1606">Unterstützung zur Berücksichtigung der Umgebungsvariablen `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` zu `webapp ssh` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1606">Added support to `webapp ssh` to respect `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>
* <span data-ttu-id="0bba9-1607">Unterstützung für `appserviceplan create` für die kostenlose Linux-SKU hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1607">Added `appserviceplan create` support for Linux Free SKU</span></span>
* <span data-ttu-id="0bba9-1608">`webapp up` geändert, um nach dem Festlegen der App-Einstellung `SCM_DO_BUILD_DURING_DEPLOYMENT=true` zum Verarbeiten des Kudu-Kaltstarts für 30 Sekunden in den Energiesparmodus zu wechseln</span><span class="sxs-lookup"><span data-stu-id="0bba9-1608">Changed `webapp up` to have a 30s sleep after setting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` appsetting to handle kudu cold start</span></span>
* <span data-ttu-id="0bba9-1609">Unterstützung für die `powershell`-Runtime zu `functionapp create` unter Windows hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1609">Added support for `powershell` runtime to `functionapp create` on Windows</span></span>
* <span data-ttu-id="0bba9-1610">Befehl `create-remote-connection` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1610">Added `create-remote-connection` command</span></span>

### <a name="batch"></a><span data-ttu-id="0bba9-1611">Batch</span><span class="sxs-lookup"><span data-stu-id="0bba9-1611">Batch</span></span>
* <span data-ttu-id="0bba9-1612">Fehler im Validierungssteuerelement für `--application-package-references`-Optionen korrigiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-1612">Fixed bug in validator for `--application-package-references` options</span></span>

### <a name="botservice"></a><span data-ttu-id="0bba9-1613">Botservice</span><span class="sxs-lookup"><span data-stu-id="0bba9-1613">Botservice</span></span>
* <span data-ttu-id="0bba9-1614">[BREAKING CHANGE]`bot create -v v4 -k webapp` geändert, sodass standardmäßig eine leerer Web-App-Bot erstellt wird (d. h. kein Bot wird in App Service bereitgestellt)</span><span class="sxs-lookup"><span data-stu-id="0bba9-1614">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to create an empty Web App Bot by default (i.e. no bot is deployed to the App Service)</span></span>
* <span data-ttu-id="0bba9-1615">`--echo`-Flag zu `bot create` hinzugefügt, sodass das alte Verhalten mit `-v v4` verwendet wird</span><span class="sxs-lookup"><span data-stu-id="0bba9-1615">Added `--echo` flag to `bot create` to use the old behavior with `-v v4`</span></span>
* <span data-ttu-id="0bba9-1616">[BREAKING CHANGE] Standardwert von `--version` in `v4` geändert</span><span class="sxs-lookup"><span data-stu-id="0bba9-1616">[BREAKING CHANGE] Changed the default value of  `--version` to `v4`</span></span>
  * <span data-ttu-id="0bba9-1617">__HINWEIS:__ `bot prepare-publish` verwendet weiterhin den alten Standard.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1617">__NOTE:__ `bot prepare-publish` still uses the its old default</span></span>
* <span data-ttu-id="0bba9-1618">[BREAKING CHANGE]`--lang` geändert, sodass der Standard nicht mehr `Csharp` ist.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1618">[BREAKING CHANGE] Changed `--lang` to no longer default to `Csharp`.</span></span> <span data-ttu-id="0bba9-1619">Wenn der Befehl `--lang` erfordert und dies nicht angegeben ist, wird der Befehl nun mit Fehler beendet.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1619">If the command requires `--lang` and it is not provided, the command will now error out</span></span>
* <span data-ttu-id="0bba9-1620">[BREAKING CHANGE]`--appid`- und `--password`-Argumente für `bot create` in erforderlich geändert, sie können jetzt über `ad app create` erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1620">[BREAKING CHANGE] Changed the `--appid` and `--password` args for `bot create` to be required and can now be created via `ad app create`</span></span>
* <span data-ttu-id="0bba9-1621">`--appid`- und `--password`-Validierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1621">Added `--appid` and `--password` validation</span></span>
* <span data-ttu-id="0bba9-1622">[BREAKING CHANGE]`bot create -v v4` geändert, sodass kein Speicherkonto bzw. keine Application Insights-Instanz erstellt oder verwendet wird</span><span class="sxs-lookup"><span data-stu-id="0bba9-1622">[BREAKING CHANGE] Changed `bot create -v v4` to not create or use a Storage Account or Application Insights</span></span>
* <span data-ttu-id="0bba9-1623">[BREAKING CHANGE]`bot create -v v3` geändert, sodass eine Region erforderlich ist, in der Application Insights verfügbar ist</span><span class="sxs-lookup"><span data-stu-id="0bba9-1623">[BREAKING CHANGE] Changed `bot create -v v3` to require a region where Application Insights is available</span></span>
* <span data-ttu-id="0bba9-1624">[BREAKING CHANGE]`bot update` geändert, sodass es sich jetzt nur auf spezifische Eigenschaften eines Bots auswirkt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1624">[BREAKING CHANGE] Changed `bot update` to now affect only specific properties of a bot</span></span>
* <span data-ttu-id="0bba9-1625">[BREAKING CHANGE]`--lang`-Flags geändert, sodass `Javascript` anstelle von `Node` akzeptiert wird</span><span class="sxs-lookup"><span data-stu-id="0bba9-1625">[BREAKING CHANGE] Changed `--lang` flags to accept `Javascript` instead of `Node`</span></span>
* <span data-ttu-id="0bba9-1626">[BREAKING CHANGE]`Node` als zulässiger `--lang`-Wert entfernt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1626">[BREAKING CHANGE] Removed `Node` as an allowed `--lang` value</span></span>
* <span data-ttu-id="0bba9-1627">[BREAKING CHANGE]`bot create -v v4 -k webapp` geändert, sodass `SCM_DO_BUILD_DURING_DEPLOYMENT` nicht mehr auf TRUE festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1627">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to no longer set `SCM_DO_BUILD_DURING_DEPLOYMENT` to true.</span></span> <span data-ttu-id="0bba9-1628">Alle Bereitstellungen über Kudu fungieren ihrem Standardverhalten entsprechend.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1628">All deployments through Kudu will act according to their default behavior</span></span>
* <span data-ttu-id="0bba9-1629">`bot download` für Bots ohne `.bot`-Dateien geändert, sodass die sprachspezifische Konfigurationsdatei mit Werten aus den Anwendungseinstellungen für den Bot erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1629">Changed `bot download` for bots without `.bot` files to create the language-specific configuration file with values from the Application Settings for the bot</span></span>
* <span data-ttu-id="0bba9-1630">Unterstützung für `Typescript` zu `bot prepare-deploy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1630">Added `Typescript` support to `bot prepare-deploy`</span></span>
* <span data-ttu-id="0bba9-1631">Warnmeldung zu `bot prepare-deploy` für `Javascript`- und `Typescript`-Bots hinzugefügt, wenn `package.json` in `--code-dir` nicht enthalten ist</span><span class="sxs-lookup"><span data-stu-id="0bba9-1631">Added warning message to `bot prepare-deploy` for `Javascript` and `Typescript` bots for when `--code-dir` does not contain `package.json`</span></span>
* <span data-ttu-id="0bba9-1632">`bot prepare-deploy` geändert, sodass bei Erfolg `true` zurückgegeben wird</span><span class="sxs-lookup"><span data-stu-id="0bba9-1632">Changed `bot prepare-deploy` to return `true` if successful</span></span>
* <span data-ttu-id="0bba9-1633">Ausführliche Protokollierung zu `bot prepare-deploy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1633">Added verbose logging to `bot prepare-deploy`</span></span>
* <span data-ttu-id="0bba9-1634">Mehr verfügbare Application Insights-Regionen zu `az bot create -v v3` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1634">Added more available Application Insights regions to `az bot create -v v3`</span></span>

### <a name="configure"></a><span data-ttu-id="0bba9-1635">Konfigurieren</span><span class="sxs-lookup"><span data-stu-id="0bba9-1635">Configure</span></span>
* <span data-ttu-id="0bba9-1636">Unterstützung für die ordnerbasierte Argument-Standardwertkonfigurationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1636">Added support for folder based argument default value configurations</span></span>

### <a name="eventhubs"></a><span data-ttu-id="0bba9-1637">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="0bba9-1637">Eventhubs</span></span>
* <span data-ttu-id="0bba9-1638">Befehle vom Typ `namespace network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1638">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="0bba9-1639">`--default-action`-Argument für Netzwerkregeln zu `namespace [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1639">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="0bba9-1640">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0bba9-1640">Network</span></span>
* <span data-ttu-id="0bba9-1641">[BREAKING CHANGE]`--cache`-Argument mit `--defer` für `vnet [create|update]` ersetzt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1641">[BREAKING CHANGE] Replaced `--cache` arugment with `--defer` for `vnet [create|update]`</span></span> 

### <a name="policy-insights"></a><span data-ttu-id="0bba9-1642">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="0bba9-1642">Policy Insights</span></span>
* <span data-ttu-id="0bba9-1643">Unterstützung für `--expand PolicyEvaluationDetails` hinzugefügt, sodass Richtlinienauswertungsdetails von der Ressource abgefragt werden</span><span class="sxs-lookup"><span data-stu-id="0bba9-1643">Added support for `--expand PolicyEvaluationDetails` to query policy evaluation details on the resource</span></span>

### <a name="role"></a><span data-ttu-id="0bba9-1644">Role</span><span class="sxs-lookup"><span data-stu-id="0bba9-1644">Role</span></span>
* <span data-ttu-id="0bba9-1645">[VERALTET]: Ausblenden des „--password"-Arguments von `create-for-rbac` geändert; Unterstützung wird im Mai 2019 entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1645">[DEPRECATED] Changed `create-for-rbac` hide '--password' argument - support will be removed in May 2019</span></span>

### <a name="service-bus"></a><span data-ttu-id="0bba9-1646">Service Bus</span><span class="sxs-lookup"><span data-stu-id="0bba9-1646">Service Bus</span></span>
* <span data-ttu-id="0bba9-1647">Befehle vom Typ `namespace network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1647">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="0bba9-1648">`--default-action`-Argument für Netzwerkregeln zu `namespace [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1648">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>
* <span data-ttu-id="0bba9-1649">`topic [create|update]` korrigiert, sodass `--max-size`-Unterstützung für 10-, 20-, 40- und 80-GB-Werte mit Premium-SKU zulässig ist</span><span class="sxs-lookup"><span data-stu-id="0bba9-1649">Fixed `topic [create|update]` to allow `--max-size` support for 10, 20, 40 and 80GB values with premium SKU</span></span>

### <a name="sql"></a><span data-ttu-id="0bba9-1650">SQL</span><span class="sxs-lookup"><span data-stu-id="0bba9-1650">SQL</span></span>
* <span data-ttu-id="0bba9-1651">Befehle vom Typ `sql virtual-cluster [list|show|delete]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1651">Added `sql virtual-cluster [list|show|delete]` commands</span></span>

### <a name="vm"></a><span data-ttu-id="0bba9-1652">VM</span><span class="sxs-lookup"><span data-stu-id="0bba9-1652">VM</span></span>
* <span data-ttu-id="0bba9-1653">`--protect-from-scale-in` und `--protect-from-scale-set-actions` zu `vmss update` hinzugefügt, sodass Aktualisierungen der Schutzrichtlinie von VMSS-VM-Instanzen aktiviert sind</span><span class="sxs-lookup"><span data-stu-id="0bba9-1653">Added `--protect-from-scale-in` and `--protect-from-scale-set-actions` to `vmss update` to enable updates to the protection policy of VMSS VM instances</span></span>
* <span data-ttu-id="0bba9-1654">`--instance-id` zu `vmss update` hinzugefügt, sodass allgemeine Aktualisierungen von VMSS-VM-Instanzen aktiviert sind</span><span class="sxs-lookup"><span data-stu-id="0bba9-1654">Added `--instance-id` to `vmss update` to enable generic update of VMSS VM instances</span></span>
* <span data-ttu-id="0bba9-1655">`--instance-id` zu `vmss wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1655">Added `--instance-id` to `vmss wait`</span></span>
* <span data-ttu-id="0bba9-1656">Neue `ppg`-Befehlsgruppe für die Verwaltung von Näherungsplatzierungsgruppen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1656">Added new `ppg` command group for managing Proximity Placement Groups</span></span>
* <span data-ttu-id="0bba9-1657">`--ppg` zu `[vm|vmss] create` und `vm availability-set create` für die Verwaltung von PPGs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1657">Added `--ppg` to `[vm|vmss] create` and `vm availability-set create` for managing PPGs</span></span>
* <span data-ttu-id="0bba9-1658">Parameter `--hyper-v-generation` zu `image create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1658">Added `--hyper-v-generation` parameter to `image create`</span></span>

## <a name="april-23-2019"></a><span data-ttu-id="0bba9-1659">23. April 2019</span><span class="sxs-lookup"><span data-stu-id="0bba9-1659">April 23, 2019</span></span>

<span data-ttu-id="0bba9-1660">Version 2.0.63</span><span class="sxs-lookup"><span data-stu-id="0bba9-1660">Version 2.0.63</span></span>

### <a name="acs"></a><span data-ttu-id="0bba9-1661">ACS</span><span class="sxs-lookup"><span data-stu-id="0bba9-1661">ACS</span></span>
* <span data-ttu-id="0bba9-1662">`aks get-credentials` zur Anzeige einer Eingabeaufforderung zum Überschreiben doppelter Werte geändert</span><span class="sxs-lookup"><span data-stu-id="0bba9-1662">Changed `aks get-credentials` to prompt to overwrite duplicated values</span></span>
* <span data-ttu-id="0bba9-1663">`(PREVIEW)` aus Dev Spaces-Befehlen „aks use-dev-spaces“ und „aks remove-dev-spaces“ entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1663">Removed `(PREVIEW)` from Dev Spaces commands "aks use-dev-spaces" and "aks remove-dev-spaces"</span></span>

### <a name="ams"></a><span data-ttu-id="0bba9-1664">AMS</span><span class="sxs-lookup"><span data-stu-id="0bba9-1664">AMS</span></span>
* <span data-ttu-id="0bba9-1665">Fehler bei der Objekt- und Kontofilteraktualisierung behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-1665">Fixed bug with asset and account filters update</span></span>

### <a name="appservice"></a><span data-ttu-id="0bba9-1666">AppService</span><span class="sxs-lookup"><span data-stu-id="0bba9-1666">AppService</span></span>
* <span data-ttu-id="0bba9-1667">Unterstützung für die App Service-Umgebung (App Service Environment, ASE) und Zeitlimit zu `webapp ssh` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1667">Added support for ASE and timeout to `webapp ssh`</span></span>
* <span data-ttu-id="0bba9-1668">Unterstützung für die Einrichtung von CI/CD für eine Azure DevOps-Pipeline aus einem GitHub-Repository zu Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1668">Added support for establishing CI CD to an Azure DevOps pipeline from a Github repository to Function apps</span></span>
* <span data-ttu-id="0bba9-1669">`--github-pat`-Argument zu `functionapp devops-build create` hinzugefügt, um persönliche GitHub-Zugriffstoken zu akzeptieren</span><span class="sxs-lookup"><span data-stu-id="0bba9-1669">Added `--github-pat` argument to `functionapp devops-build create` to accept Github personal access token</span></span>
* <span data-ttu-id="0bba9-1670">`--github-repository`-Argument zu `functionapp devops-build create` hinzugefügt, um das GitHub-Repository mit dem Quellcode einer Funktions-App zu akzeptieren</span><span class="sxs-lookup"><span data-stu-id="0bba9-1670">Added `--github-repository` argument to `functionapp devops-build create` to accept Github repository that contains a functionapp source code</span></span>
* <span data-ttu-id="0bba9-1671">Problem behoben, aufgrund dessen bei `az webapp up --logs` ein Fehler auftrat und die .NET Core-Standardversion auf 2.1 aktualisiert wurde</span><span class="sxs-lookup"><span data-stu-id="0bba9-1671">Fixed issue where `az webapp up --logs` was failing with a error and updating default .NETCORE version to 2.1</span></span>
* <span data-ttu-id="0bba9-1672">Unnötige Funktions-App-Einstellungen beim Erstellen einer Funktions-App mit Verbrauchsplan entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1672">Removed unnecessary functionapp settings when creating a function app with consumption plan</span></span>
* <span data-ttu-id="0bba9-1673">`webapp up` geändert, sodass die ASP-Standardzeichenfolge jetzt eine Zahl am Ende anfügt, um einen neuen ASP basierend auf SKU-Optionen zu erstellen</span><span class="sxs-lookup"><span data-stu-id="0bba9-1673">Changed `webapp up` so the default asp string now appends number at the end to create a new ASP based on SKU options</span></span>
* <span data-ttu-id="0bba9-1674">`-b` als Option für `webapp up` hinzugefügt, um die App im Browser zu starten</span><span class="sxs-lookup"><span data-stu-id="0bba9-1674">Added `-b` as an option to `webapp up` to launch the app in the browser</span></span>
* <span data-ttu-id="0bba9-1675">`webapp deployment source config zip` geändert, um die `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`-Umgebungsvariable zu behandeln</span><span class="sxs-lookup"><span data-stu-id="0bba9-1675">Changed `webapp deployment source config zip` to handle `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="0bba9-1676">Bereitstellungs-Manager</span><span class="sxs-lookup"><span data-stu-id="0bba9-1676">Deployment Manager</span></span>
* <span data-ttu-id="0bba9-1677">[VORSCHAUVERSIPN] Erstellen und Verwalten von Artefakten, die Rollouts unterstützen</span><span class="sxs-lookup"><span data-stu-id="0bba9-1677">[PREVIEW] Create and manage artifacts that support rollouts</span></span>

### <a name="lab"></a><span data-ttu-id="0bba9-1678">Labor</span><span class="sxs-lookup"><span data-stu-id="0bba9-1678">Lab</span></span>
* <span data-ttu-id="0bba9-1679">Fehler behoben, der zu einer vorzeitigen Beendigung führen würde</span><span class="sxs-lookup"><span data-stu-id="0bba9-1679">Fixed bug which would cause an early exit</span></span>

### <a name="network"></a><span data-ttu-id="0bba9-1680">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0bba9-1680">Network</span></span>
* <span data-ttu-id="0bba9-1681">Automatische Delegierung des Namenservers im übergeordneten Element während der Erstellung der untergeordneten Zone zu `dns zone create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1681">Added auto name server delegation to `dns zone create` in parent during child zone creation</span></span>

### <a name="resource"></a><span data-ttu-id="0bba9-1682">Resource</span><span class="sxs-lookup"><span data-stu-id="0bba9-1682">Resource</span></span>
* <span data-ttu-id="0bba9-1683">[VERALTET]: Argumente `--link-id`, `--target-id` und `--filter-string` von `resource link` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-1683">[DEPRECATED] Deprecated `--link-id`, `--target-id` and `--filter-string` arguments of `resource link`</span></span>
  * <span data-ttu-id="0bba9-1684">Verwenden Sie stattdessen die Argumente `--link`, `--target` und `--filter`.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1684">Use the arguments `--link`, `--target`, and `--filter` instead</span></span>
* <span data-ttu-id="0bba9-1685">Problem behoben, aufgrund dessen `resource link [create|update]`-Befehle nicht verwendet werden konnten</span><span class="sxs-lookup"><span data-stu-id="0bba9-1685">Fixed issue where `resource link [create|update]` commands would not work</span></span>
* <span data-ttu-id="0bba9-1686">Problem behoben, aufgrund dessen das Löschen anhand einer Ressourcen-ID bei einem Fehler zu einem Absturz führen konnte</span><span class="sxs-lookup"><span data-stu-id="0bba9-1686">Fixed an issue where deleting using a resource ID could crash on error</span></span>

### <a name="sql"></a><span data-ttu-id="0bba9-1687">SQL</span><span class="sxs-lookup"><span data-stu-id="0bba9-1687">SQL</span></span>
* <span data-ttu-id="0bba9-1688">Unterstützung für benutzerdefinierte Zeitzonen auf verwalteten Instanzen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1688">Added support for custom time zone on managed instances</span></span>
* <span data-ttu-id="0bba9-1689">Geändert, um die Verwendung des Namens eines Pools für elastische Datenbanken mit `sql db update` zuzulassen</span><span class="sxs-lookup"><span data-stu-id="0bba9-1689">Changed to allow elastic pool name to be used with `sql db update`</span></span>
* <span data-ttu-id="0bba9-1690">Unterstützung für `--no-wait` zu `sql server [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1690">Added `--no-wait` support to `sql server [create|update]`</span></span>
* <span data-ttu-id="0bba9-1691">Befehl `sql server wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1691">Added command `sql server wait`</span></span>

### <a name="storage"></a><span data-ttu-id="0bba9-1692">Storage</span><span class="sxs-lookup"><span data-stu-id="0bba9-1692">Storage</span></span>
* <span data-ttu-id="0bba9-1693">Problem mit doppelt codierten SAS-Token in `storage blob generate-sas` behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-1693">Fixed issue with double-encoded SAS tokens in `storage blob generate-sas`</span></span>

### <a name="vm"></a><span data-ttu-id="0bba9-1694">VM</span><span class="sxs-lookup"><span data-stu-id="0bba9-1694">VM</span></span>
* <span data-ttu-id="0bba9-1695">`--skip-shutdown`-Flag zum Ausschalten von VMs ohne Herunterfahren zu `vm|vmss stop` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1695">Added `--skip-shutdown` flag to `vm|vmss stop` to power-off VMs without shutdown</span></span>
* <span data-ttu-id="0bba9-1696">`--storage-account-type`-Argument zum Festlegen des Kontotyps des Veröffentlichungsprofils zu `sig image-version create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1696">Added `--storage-account-type` argument to `sig image-version create` to set the publishing profile's account type</span></span>
* <span data-ttu-id="0bba9-1697">`--target-regions`-Argument zu `sig image-version create` hinzugefügt, um das Festlegen von regionsspezifischen Speicherkontotypen zuzulassen</span><span class="sxs-lookup"><span data-stu-id="0bba9-1697">Added `--target-regions` argument to `sig image-version create` to allow setting region-specific storage account types</span></span>

## <a name="april-9-2019"></a><span data-ttu-id="0bba9-1698">9\. April 2019</span><span class="sxs-lookup"><span data-stu-id="0bba9-1698">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="0bba9-1699">Core</span><span class="sxs-lookup"><span data-stu-id="0bba9-1699">Core</span></span>
* <span data-ttu-id="0bba9-1700">Problem behoben, aufgrund dessen einige Erweiterungen mit der Version `Unknown` angezeigt wurden und nicht aktualisiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="0bba9-1700">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="0bba9-1701">ACR</span><span class="sxs-lookup"><span data-stu-id="0bba9-1701">ACR</span></span>
* <span data-ttu-id="0bba9-1702">Unterstützung für die kontextlose Ausführung eines Images hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1702">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="0bba9-1703">AMS</span><span class="sxs-lookup"><span data-stu-id="0bba9-1703">AMS</span></span>
* [VERALTET]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
[DEPRECATED]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [BREAKING CHANGE]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="0bba9-1706">Unterstützung für neue Verschlüsselungsparameter in `ams streaming-policy create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1706">Added new encryption parameters support in `ams streaming-policy create`</span></span>
* <span data-ttu-id="0bba9-1707">Neuer Parameter `--filters` zu `ams streaming-locator create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1707">Added new paramter `--filters` to `ams streaming-locator create`</span></span>

### <a name="appservice"></a><span data-ttu-id="0bba9-1708">AppService</span><span class="sxs-lookup"><span data-stu-id="0bba9-1708">AppService</span></span>
* <span data-ttu-id="0bba9-1709">Unterstützung für `--logs` zu `webapp up` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1709">Added `--logs` support to `webapp up`</span></span>
* <span data-ttu-id="0bba9-1710">Probleme bei der Generierung von `azure-pipelines.yml` beim Befehl `functionapp devops-build create` behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-1710">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="0bba9-1711">Fehlerbehandlung und Indikatoren für `unctionapp devops-build create` verbessert</span><span class="sxs-lookup"><span data-stu-id="0bba9-1711">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="0bba9-1712">[BREAKING CHANGE] Flag `--local-git` für den Befehl `devops-build` entfernt; lokale Git-Erkennung und -Verarbeitung sind zum Erstellen von Azure DevOps-Pipelines obligatorisch</span><span class="sxs-lookup"><span data-stu-id="0bba9-1712">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="0bba9-1713">Unterstützung für das Erstellen von Linux-Functions-Plänen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1713">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="0bba9-1714">Möglichkeit zum Wechseln eines Plans unter einer Funktions-App mit `functionapp update --plan` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1714">Added ability to switch a plan underneath a function app using `functionapp update --plan`</span></span>
* <span data-ttu-id="0bba9-1715">Unterstützung für Einstellungen zum Aufskalieren für den Azure Functions-Premium-Plan hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1715">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="0bba9-1716">CDN</span><span class="sxs-lookup"><span data-stu-id="0bba9-1716">CDN</span></span>
* <span data-ttu-id="0bba9-1717">Unterstützung hinzugefügt für `Microsoft_Standard` und `Standard_ChinaCdn`</span><span class="sxs-lookup"><span data-stu-id="0bba9-1717">Added support for `Microsoft_Standard` and `Standard_ChinaCdn`</span></span>

### <a name="feedback"></a><span data-ttu-id="0bba9-1718">Feedback</span><span class="sxs-lookup"><span data-stu-id="0bba9-1718">Feedback</span></span>
* <span data-ttu-id="0bba9-1719">`feedback` zur Anzeige von Metadaten zu den zuletzt ausgeführten Befehlen geändert</span><span class="sxs-lookup"><span data-stu-id="0bba9-1719">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="0bba9-1720">`feedback` geändert, um den Benutzer zur Unterstützung beim Issueerstellungsprozess aufzufordern (durch Öffnen eines Browsers und Verwenden einer Issuevorlage)</span><span class="sxs-lookup"><span data-stu-id="0bba9-1720">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="0bba9-1721">`feedback` geändert, um den Issuetext bei der Ausführung mit „--verbose“ auszugeben</span><span class="sxs-lookup"><span data-stu-id="0bba9-1721">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="0bba9-1722">Überwachen</span><span class="sxs-lookup"><span data-stu-id="0bba9-1722">Monitor</span></span>
* <span data-ttu-id="0bba9-1723">Problem behoben, aufgrund dessen „Count“ kein zulässiger Wert für `metrics alert [create|update]` war</span><span class="sxs-lookup"><span data-stu-id="0bba9-1723">Fixed issue where "count" was not a permitted value with `metrics alert [create|update]`</span></span> 

### <a name="network"></a><span data-ttu-id="0bba9-1724">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0bba9-1724">Network</span></span>
* <span data-ttu-id="0bba9-1725">Problem behoben, aufgrund dessen das Tabellenformat mit `vnet-gateway list-bgp-peer-status` nicht angezeigt wurde</span><span class="sxs-lookup"><span data-stu-id="0bba9-1725">Fixed table format not displaying with `vnet-gateway list-bgp-peer-status`</span></span>
* <span data-ttu-id="0bba9-1726">Befehle `list-request-headers` und `list-response-headers` zu `application-gateway rewrite-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1726">Added `list-request-headers` and `list-response-headers` commands to `application-gateway rewrite-rule`</span></span>
* <span data-ttu-id="0bba9-1727">Befehl `list-server-variables` zu `application-gateway rewrite-rule condition` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1727">Added `list-server-variables` command to `application-gateway rewrite-rule condition`</span></span>
* <span data-ttu-id="0bba9-1728">Problem behoben, aufgrund dessen durch das Aktualisieren des Linkstatus für einen ExpressRoute-Port eine Ausnahme vom Typ „unbekanntes Attribut“ ausgelöst wurde: `express-route port update`</span><span class="sxs-lookup"><span data-stu-id="0bba9-1728">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception `express-route port update`</span></span>

### <a name="privatedns"></a><span data-ttu-id="0bba9-1729">PrivateDNS</span><span class="sxs-lookup"><span data-stu-id="0bba9-1729">PrivateDNS</span></span>
* <span data-ttu-id="0bba9-1730">`network private-dns` für private DNS-Zonen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1730">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="0bba9-1731">Resource</span><span class="sxs-lookup"><span data-stu-id="0bba9-1731">Resource</span></span>
* <span data-ttu-id="0bba9-1732">Problem mit `deployment create` und `group deployment create` behoben, aufgrund dessen eine Parameterdatei mit leerem Parametersatz nicht verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="0bba9-1732">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="0bba9-1733">Role</span><span class="sxs-lookup"><span data-stu-id="0bba9-1733">Role</span></span>
* <span data-ttu-id="0bba9-1734">`create-for-rbac` korrigiert, um `--years` korrekt zu verarbeiten</span><span class="sxs-lookup"><span data-stu-id="0bba9-1734">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="0bba9-1735">[BREAKING CHANGE]`role assignment delete` geändert, um eine Eingabeaufforderung anzuzeigen, wenn alle Zuweisungen im Abonnement ohne Bedingungen gelöscht werden</span><span class="sxs-lookup"><span data-stu-id="0bba9-1735">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="0bba9-1736">SQL</span><span class="sxs-lookup"><span data-stu-id="0bba9-1736">SQL</span></span>
* <span data-ttu-id="0bba9-1737">`sql mi [create|update]` mit den Eigenschaften „proxyOverride“ und „publicDataEndpointEnabled“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-1737">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="0bba9-1738">Storage</span><span class="sxs-lookup"><span data-stu-id="0bba9-1738">Storage</span></span>
* <span data-ttu-id="0bba9-1739">[BREAKING CHANGE] Ergebnis von `storage blob delete` entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1739">[BREAKING CHANGE] Removed result of `storage blob delete`</span></span>
* <span data-ttu-id="0bba9-1740">`--full-uri` zu `storage blob generate-sas` hinzugefügt, um den vollständigen URI für das Blob mit SAS zu erstellen</span><span class="sxs-lookup"><span data-stu-id="0bba9-1740">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="0bba9-1741">`--file-snapshot` zu `storage file copy start` hinzugefügt, um die Datei aus der Momentaufnahme zu kopieren</span><span class="sxs-lookup"><span data-stu-id="0bba9-1741">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="0bba9-1742">`storage blob copy cancel` geändert, um anstelle der Ausnahme für „NoPendingCopyOperation“ nur den Fehler anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="0bba9-1742">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="0bba9-1743">26. März 2019</span><span class="sxs-lookup"><span data-stu-id="0bba9-1743">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="0bba9-1744">Core</span><span class="sxs-lookup"><span data-stu-id="0bba9-1744">Core</span></span>
* <span data-ttu-id="0bba9-1745">Probleme mit der Inkompatibilität der Entwicklungserweiterung behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-1745">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="0bba9-1746">Die Fehlerbehandlung verweist Kunden jetzt auf die Problemseite.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1746">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="0bba9-1747">Cloud</span><span class="sxs-lookup"><span data-stu-id="0bba9-1747">Cloud</span></span>
* <span data-ttu-id="0bba9-1748">Fehler „Abonnement nicht gefunden“ in `cloud set` behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-1748">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="0bba9-1749">ACR</span><span class="sxs-lookup"><span data-stu-id="0bba9-1749">ACR</span></span>
* <span data-ttu-id="0bba9-1750">Redundante Quellen im Imageimport korrigiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-1750">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="0bba9-1751">`--auth-mode` wurde den Befehlen `acr build`, `acr run`, `acr task create` und `acr task update` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1751">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="0bba9-1752">Befehlsgruppe „acr task credential“ zum Verwalten von Anmeldeinformationen für eine Aufgabe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1752">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="0bba9-1753">„--no-wait“ zum Befehl `acr build` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1753">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="0bba9-1754">AppService</span><span class="sxs-lookup"><span data-stu-id="0bba9-1754">AppService</span></span>
* <span data-ttu-id="0bba9-1755">Problem behoben, das dazu führte, dass die Ausführung aus einem leeren Verzeichnis oder ein Szenario mit unbekannten Code von `webapp up` nicht korrekt behandelt wurde</span><span class="sxs-lookup"><span data-stu-id="0bba9-1755">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="0bba9-1756">Problem behoben, aufgrund dessen Slots für `[webapp|functionapp] config ssl bind` nicht verwendet werden konnten</span><span class="sxs-lookup"><span data-stu-id="0bba9-1756">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="0bba9-1757">Bot Service</span><span class="sxs-lookup"><span data-stu-id="0bba9-1757">BOT Service</span></span>
* <span data-ttu-id="0bba9-1758">`bot prepare-deploy` hinzugefügt, um die Bereitstellung von Bots über `webapp` vorzubereiten</span><span class="sxs-lookup"><span data-stu-id="0bba9-1758">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="0bba9-1759">`bot create --kind registration` geändert, um das Kennwort anzuzeigen, falls kein Kennwort angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="0bba9-1759">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="0bba9-1760">[BREAKING CHANGE]`--endpoint` wurde in `bot create --kind registration` geändert, sodass nun standardmäßig eine leere Zeichenfolge verwendet wird, anstatt eine Angabe zu erfordern.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1760">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="0bba9-1761">`SCM_DO_BUILD_DURING_DEPLOYMENT` zu den Anwendungseinstellungen der ARM-Vorlage für Web-App-Bot (v4) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1761">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="0bba9-1762">CDN</span><span class="sxs-lookup"><span data-stu-id="0bba9-1762">CDN</span></span>
* <span data-ttu-id="0bba9-1763">Unterstützung für `--no-wait` zu `cdn endpoint [create|update|start|stop|delete|load|purge]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1763">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* <span data-ttu-id="0bba9-1764">[BREAKING CHANGE] Das standardmäßige Zwischenspeicherverhalten für Abfragezeichenfolgen von `cdn endpoint create` wurde geändert.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1764">[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour.</span></span> <span data-ttu-id="0bba9-1765">Es wird nicht mehr standardmäßig „IgnoreQueryString“ festgelegt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1765">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="0bba9-1766">Er wird jetzt vom Dienst festgelegt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1766">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="0bba9-1767">Cosmosdb</span><span class="sxs-lookup"><span data-stu-id="0bba9-1767">Cosmosdb</span></span>
* <span data-ttu-id="0bba9-1768">Unterstützung für `--enable-multiple-write-locations` bei Kontoaktualisierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1768">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="0bba9-1769">Untergruppe `network-rule` mit Befehlen `add`, `remove` und `list` zum Verwalten von VNET-Regeln eines Cosmos DB-Kontos hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1769">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="0bba9-1770">Interactive</span><span class="sxs-lookup"><span data-stu-id="0bba9-1770">Interactive</span></span>
* <span data-ttu-id="0bba9-1771">Inkompatibilität mit der über azdev installierten interaktiven Erweiterung korrigiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-1771">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="0bba9-1772">Überwachen</span><span class="sxs-lookup"><span data-stu-id="0bba9-1772">Monitor</span></span>
* <span data-ttu-id="0bba9-1773">Geändert, sodass der Dimensionswert `*` für `monitor metrics alert [create|update]` zulässig ist</span><span class="sxs-lookup"><span data-stu-id="0bba9-1773">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="0bba9-1774">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0bba9-1774">Network</span></span>
* <span data-ttu-id="0bba9-1775">Befehlsgruppe `rewrite-rule` zu `application-gateway` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1775">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="0bba9-1776">Profil</span><span class="sxs-lookup"><span data-stu-id="0bba9-1776">Profile</span></span>
* <span data-ttu-id="0bba9-1777">Kontounterstützung auf Mandantenebene für verwaltete Dienstidentität zu `login` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1777">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="0bba9-1778">Postgres</span><span class="sxs-lookup"><span data-stu-id="0bba9-1778">Postgres</span></span> 
* <span data-ttu-id="0bba9-1779">postgresql-Befehle vom Typ `replica` und Befehl `restart server` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1779">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="0bba9-1780">Änderungen vorgenommen, um den Standardspeicherort aus der Ressourcengruppe abzurufen, wenn er für die Erstellung von Servern nicht angegeben wurde, und um eine Überprüfung für die Aufbewahrungstage hinzuzufügen</span><span class="sxs-lookup"><span data-stu-id="0bba9-1780">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="0bba9-1781">Resource</span><span class="sxs-lookup"><span data-stu-id="0bba9-1781">Resource</span></span>
* <span data-ttu-id="0bba9-1782">Verbesserte Tabellenausgabe für `deployment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="0bba9-1782">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="0bba9-1783">Problem mit `deployment [create|validate]` behoben, aufgrund dessen der Typ „secureObject“ nicht erkannt wurde</span><span class="sxs-lookup"><span data-stu-id="0bba9-1783">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="0bba9-1784">Graph</span><span class="sxs-lookup"><span data-stu-id="0bba9-1784">Graph</span></span>
* <span data-ttu-id="0bba9-1785">Unterstützung für `--end-date` zu `ad [app|sp] credential reset` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1785">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="0bba9-1786">Unterstützung für das Hinzufügen von Berechtigungen mit `ad app permission add` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1786">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="0bba9-1787">Fehler mit `ad app permission list` behoben, wenn keine Berechtigungen vorlagen</span><span class="sxs-lookup"><span data-stu-id="0bba9-1787">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="0bba9-1788">Änderung an `ad sp delete` vorgenommen, um das Entfernen einer Rollenzuweisung zu überspringen, wenn das aktuelle Konto kein Abonnement enthält</span><span class="sxs-lookup"><span data-stu-id="0bba9-1788">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="0bba9-1789">`ad app create` geändert, sodass ohne Angabe für `--identifier-uris` standardmäßig eine leere Liste verwendet wird</span><span class="sxs-lookup"><span data-stu-id="0bba9-1789">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="0bba9-1790">storage</span><span class="sxs-lookup"><span data-stu-id="0bba9-1790">storage</span></span>
* <span data-ttu-id="0bba9-1791">`--snapshot` zu `storage file download-batch` für den Download von einer Freigabemomentaufnahme hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1791">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="0bba9-1792">Statusanzeige für `storage blob [download-batch|upload-batch]` geändert, damit sie weniger ausführlich dargestellt wird und das aktuelle Blob angibt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1792">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="0bba9-1793">Problem mit `storage account update` behoben, das beim Aktualisieren von Verschlüsselungsparametern auftrat</span><span class="sxs-lookup"><span data-stu-id="0bba9-1793">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="0bba9-1794">Problem behoben, bei dem für `storage blob show` ein Fehler auftrat, wenn oauth (`--auth-mode=login`) verwendet wurde</span><span class="sxs-lookup"><span data-stu-id="0bba9-1794">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="0bba9-1795">VM</span><span class="sxs-lookup"><span data-stu-id="0bba9-1795">VM</span></span>
* <span data-ttu-id="0bba9-1796">Befehl `image update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1796">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="0bba9-1797">12. März 2019</span><span class="sxs-lookup"><span data-stu-id="0bba9-1797">March 12, 2019</span></span>

<span data-ttu-id="0bba9-1798">Version 2.0.60</span><span class="sxs-lookup"><span data-stu-id="0bba9-1798">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="0bba9-1799">Core</span><span class="sxs-lookup"><span data-stu-id="0bba9-1799">Core</span></span>

* <span data-ttu-id="0bba9-1800">Falsche Fehlermeldung in `cloud set` zu nicht gefundenem Abonnement korrigiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-1800">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="0bba9-1801">ACR</span><span class="sxs-lookup"><span data-stu-id="0bba9-1801">ACR</span></span>

* <span data-ttu-id="0bba9-1802">Redundante Quellen im Imageimport korrigiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-1802">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="0bba9-1803">ACS</span><span class="sxs-lookup"><span data-stu-id="0bba9-1803">ACS</span></span>

* <span data-ttu-id="0bba9-1804">Änderung vorgenommen, um den Parameter `--listen-address` für `aks browse` zu ignorieren, wenn er nicht von kubectl unterstützt wird</span><span class="sxs-lookup"><span data-stu-id="0bba9-1804">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="0bba9-1805">AppService</span><span class="sxs-lookup"><span data-stu-id="0bba9-1805">AppService</span></span>

* <span data-ttu-id="0bba9-1806">`[webapp|functionapp] deployment list-publishing-credentials` hinzugefügt, um die Kudu-Veröffentlichungs-URL und die entsprechenden Anmeldeinformationen abzurufen</span><span class="sxs-lookup"><span data-stu-id="0bba9-1806">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="0bba9-1807">Fehlerhafte Ausgabeanweisung für `webapp auth update` entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1807">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="0bba9-1808">`functionapp` korrigiert, um das korrekte Image für die Runtime in App Service-Plänen unter Linux festzulegen</span><span class="sxs-lookup"><span data-stu-id="0bba9-1808">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="0bba9-1809">Vorschau-Tag für `webapp up` entfernt und Verbesserungen am Befehl implementiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-1809">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="0bba9-1810">Botservice</span><span class="sxs-lookup"><span data-stu-id="0bba9-1810">Botservice</span></span>

* <span data-ttu-id="0bba9-1811">`SCM_DO_BUILD_DURING_DEPLOYMENT` zu den Anwendungseinstellungen der ARM-Vorlage für Web-App-Bot (v4) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1811">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="0bba9-1812">`Microsoft-BotFramework-AppId` und `Microsoft-BotFramework-AppPassword` zu den Anwendungseinstellungen der ARM-Vorlage für Web-App-Bot (v4) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1812">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="0bba9-1813">Einfache Anführungszeichen aus der Befehlsausgabe von `bot publish` am Ende von `bot create` entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1813">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="0bba9-1814">`bot publish` wurde geändert und ist jetzt asynchron.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1814">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="0bba9-1815">Container</span><span class="sxs-lookup"><span data-stu-id="0bba9-1815">Container</span></span>

* <span data-ttu-id="0bba9-1816">Argument `--no-wait` zu `container [start|restart]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1816">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="0bba9-1817">EventHub</span><span class="sxs-lookup"><span data-stu-id="0bba9-1817">EventHub</span></span>

* <span data-ttu-id="0bba9-1818">Flag `--skip-empty-archives` zu `eventhub create|update` hinzugefügt, um leere Archive in der Aufzeichnung zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="0bba9-1818">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="0bba9-1819">Suchen</span><span class="sxs-lookup"><span data-stu-id="0bba9-1819">Find</span></span>

* <span data-ttu-id="0bba9-1820">Umfangreiches Funktionsupdate</span><span class="sxs-lookup"><span data-stu-id="0bba9-1820">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="0bba9-1821">HDInsight</span><span class="sxs-lookup"><span data-stu-id="0bba9-1821">HDInsight</span></span>

* <span data-ttu-id="0bba9-1822">Parameter `--storage-account-managed-identity` zu `hdinsight create` hinzugefügt, um MSI in ADLS Gen2 zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="0bba9-1822">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="0bba9-1823">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0bba9-1823">Network</span></span>

* <span data-ttu-id="0bba9-1824">Problem mit `vpn-connection update` behoben, aufgrund dessen die Aktualisierung einer VPN-Verbindung zwischen Gateways in verschiedenen Abonnements fehlschlug</span><span class="sxs-lookup"><span data-stu-id="0bba9-1824">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="0bba9-1825">Rdbms</span><span class="sxs-lookup"><span data-stu-id="0bba9-1825">Rdbms</span></span>

* <span data-ttu-id="0bba9-1826">Kleinere Korrekturen, um den Standardspeicherort aus der Ressourcengruppe abzurufen, wenn er für die Erstellung von Servern nicht angegeben wurde, und um eine Überprüfung für die Aufbewahrungstage hinzuzufügen</span><span class="sxs-lookup"><span data-stu-id="0bba9-1826">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="0bba9-1827">Role</span><span class="sxs-lookup"><span data-stu-id="0bba9-1827">Role</span></span>

* <span data-ttu-id="0bba9-1828">`role definition update` wurde korrigiert und nutzt nun die ID, um die Definition korrekt aufzulösen.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1828">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="0bba9-1829">`ad app credential reset` geändert, um die Annahme zu entfernen, dass der Dienstprinzipal der App stets vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="0bba9-1829">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="0bba9-1830">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="0bba9-1830">Service Fabric</span></span>

* <span data-ttu-id="0bba9-1831">Das Problem, dass `sf cluster list` nicht wiederholbar war, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1831">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="0bba9-1832">26. Februar 2019</span><span class="sxs-lookup"><span data-stu-id="0bba9-1832">February 26, 2019</span></span>

<span data-ttu-id="0bba9-1833">Version 2.0.59</span><span class="sxs-lookup"><span data-stu-id="0bba9-1833">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="0bba9-1834">Core</span><span class="sxs-lookup"><span data-stu-id="0bba9-1834">Core</span></span>

* <span data-ttu-id="0bba9-1835">Problem behoben, aufgrund dessen die Verwendung von `--subscription NAME` in einigen Instanzen eine Ausnahme ausgelöst hat</span><span class="sxs-lookup"><span data-stu-id="0bba9-1835">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="0bba9-1836">ACR</span><span class="sxs-lookup"><span data-stu-id="0bba9-1836">ACR</span></span>

* <span data-ttu-id="0bba9-1837">Parameter `--target` für die Befehle `acr build`, `acr task create` und `acr task update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1837">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="0bba9-1838">Verbesserte Fehlerbehandlung für Runtimebefehle, wenn keine Anmeldung bei Azure besteht</span><span class="sxs-lookup"><span data-stu-id="0bba9-1838">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="0bba9-1839">ACS</span><span class="sxs-lookup"><span data-stu-id="0bba9-1839">ACS</span></span>

* <span data-ttu-id="0bba9-1840">Option `--listen-address` zu `aks port-forward` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1840">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="0bba9-1841">AppService</span><span class="sxs-lookup"><span data-stu-id="0bba9-1841">AppService</span></span>

* <span data-ttu-id="0bba9-1842">Befehl `functionapp devops-build` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1842">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="0bba9-1843">Batch</span><span class="sxs-lookup"><span data-stu-id="0bba9-1843">Batch</span></span>
* <span data-ttu-id="0bba9-1844">[BREAKING CHANGE] Befehl `batch pool upgrade os` entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1844">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="0bba9-1845">[BREAKING CHANGE]`Pacakges`-Eigenschaft aus `Application`-Antworten entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1845">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="0bba9-1846">Befehl `batch application package list` zum Auflisten von Paketen einer Anwendung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1846">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="0bba9-1847">[BREAKING CHANGE]`--application-id` in allen `batch application`-Befehlen in `--application-name` geändert</span><span class="sxs-lookup"><span data-stu-id="0bba9-1847">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="0bba9-1848">Argument `--json-file` für Befehle zum Anfordern der unformatierten API-Antwort hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1848">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="0bba9-1849">Validierung aktualisiert, sodass das `https://`-Element automatisch in alle Endpunkte aufgenommen wird, wenn es fehlt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1849">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="0bba9-1850">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="0bba9-1850">CosmosDB</span></span>

* <span data-ttu-id="0bba9-1851">Untergruppe `network-rule` mit Befehlen `add`, `remove` und `list` zum Verwalten von VNET-Regeln eines Cosmos DB-Kontos hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1851">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="0bba9-1852">Kusto</span><span class="sxs-lookup"><span data-stu-id="0bba9-1852">Kusto</span></span>

* <span data-ttu-id="0bba9-1853">[BREAKING CHANGE] Typen `hot_cache_period` und `soft_delete_period` für Datenbank in Format der Zeitspanne nach ISO8601 geändert</span><span class="sxs-lookup"><span data-stu-id="0bba9-1853">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="0bba9-1854">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0bba9-1854">Network</span></span>

* <span data-ttu-id="0bba9-1855">Argument `--express-route-gateway-bypass` zu `vpn-connection [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1855">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="0bba9-1856">Befehlsgruppen aus `express-route`-Erweiterungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1856">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="0bba9-1857">Befehlsgruppen `express-route gateway` und `express-route port` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1857">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="0bba9-1858">Argument `--legacy-mode` zu `express-route peering [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1858">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="0bba9-1859">Argumente `--allow-classic-operations` und `--express-route-port` zu `express-route [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1859">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="0bba9-1860">Argument `--gateway-default-site` zu `vnet-gateway [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1860">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="0bba9-1861">Befehle vom Typ `ipsec-policy` zu `vnet-gateway` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1861">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="0bba9-1862">Resource</span><span class="sxs-lookup"><span data-stu-id="0bba9-1862">Resource</span></span>

* <span data-ttu-id="0bba9-1863">Problem mit `deployment create` behoben, aufgrund dessen beim Feld „Typ“ die Groß-/Kleinschreibung beachtet wurde</span><span class="sxs-lookup"><span data-stu-id="0bba9-1863">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="0bba9-1864">Unterstützung für URI-basierte Parameterdatei zu `policy assignment create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1864">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="0bba9-1865">Unterstützung für URI-basierte Parameter und Definitionen zu `policy set-definition update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1865">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="0bba9-1866">Verarbeitung von Parametern und Regeln für `policy definition update` korrigiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-1866">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="0bba9-1867">Problem mit `resource show/update/delete/tag/invoke-action` behoben, aufgrund dessen bei abonnementübergreifenden IDs die Abonnement-ID nicht ordnungsgemäß berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="0bba9-1867">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="0bba9-1868">Role</span><span class="sxs-lookup"><span data-stu-id="0bba9-1868">Role</span></span>

* <span data-ttu-id="0bba9-1869">Unterstützung für App-Rollen zu `ad app [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1869">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="0bba9-1870">VM</span><span class="sxs-lookup"><span data-stu-id="0bba9-1870">VM</span></span>

* <span data-ttu-id="0bba9-1871">Problem mit `vm create where ` behoben, aufgrund dessen der beschleunigte Netzwerkbetrieb für Ubuntu 18.0 nicht standardmäßig aktiviert war</span><span class="sxs-lookup"><span data-stu-id="0bba9-1871">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="0bba9-1872">12. Februar 2019</span><span class="sxs-lookup"><span data-stu-id="0bba9-1872">February 12, 2019</span></span>

<span data-ttu-id="0bba9-1873">Version 2.0.58</span><span class="sxs-lookup"><span data-stu-id="0bba9-1873">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="0bba9-1874">Core</span><span class="sxs-lookup"><span data-stu-id="0bba9-1874">Core</span></span>

* <span data-ttu-id="0bba9-1875">`az --version` zeigt jetzt eine Benachrichtigung an, wenn Sie Pakete haben, für die ein Update verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1875">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="0bba9-1876">Die Regression, dass `--ids` nicht mehr mit JSON-Ausgaben verwendet werden konnte, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1876">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="0bba9-1877">ACR</span><span class="sxs-lookup"><span data-stu-id="0bba9-1877">ACR</span></span>
* <span data-ttu-id="0bba9-1878">[BREAKING CHANGE] Die Befehlsgruppe `acr build-task` wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1878">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="0bba9-1879">[BREAKING CHANGE] Die Optionen `--tag` und `--manifest` wurden aus `acr repository delete` entfernt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1879">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="0bba9-1880">ACS</span><span class="sxs-lookup"><span data-stu-id="0bba9-1880">ACS</span></span>
* <span data-ttu-id="0bba9-1881">Unterstützung für Namen ohne Berücksichtigung von Groß-/Kleinschreibung wurde zu `aks [enable-addons|disable-addons]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1881">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="0bba9-1882">Unterstützung für Azure Active Directory-Aktualisierungsvorgang mithilfe von `aks update-credentials --reset-aad` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1882">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="0bba9-1883">Die Information, dass `--output` für `aks get-credentials` ignoriert wird, wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1883">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="0bba9-1884">AMS</span><span class="sxs-lookup"><span data-stu-id="0bba9-1884">AMS</span></span>
* <span data-ttu-id="0bba9-1885">Befehle vom Typ `ams streaming-endpoint [start | stop | create | update] wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1885">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="0bba9-1886">Befehle vom Typ `ams live-event [create | start | stop | reset] wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1886">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="0bba9-1887">AppService</span><span class="sxs-lookup"><span data-stu-id="0bba9-1887">Appservice</span></span>
* <span data-ttu-id="0bba9-1888">Die Möglichkeit zum Erstellen und Konfigurieren von Funktionen mithilfe von ACR-Containern wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1888">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="0bba9-1889">Unterstützung für das Aktualisieren von Web-App-Konfigurationen über JSON wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1889">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="0bba9-1890">Die Hilfe für `appservice-plan-update` wurde verbessert.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1890">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="0bba9-1891">Unterstützung für App-Erkenntnisse beim Erstellen von Funktions-Apps wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1891">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="0bba9-1892">Probleme mit der Web-App SSH wurden behoben.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1892">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="0bba9-1893">Botservice</span><span class="sxs-lookup"><span data-stu-id="0bba9-1893">Botservice</span></span>
* <span data-ttu-id="0bba9-1894">Die Benutzeroberfläche für `bot publish` wurde verbessert.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1894">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="0bba9-1895">Eine Warnung für Zeitlimit bei der Ausführung von `npm install` während `az bot publish` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1895">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="0bba9-1896">Ungültiges char-Element wurde `.` aus `--name` in `az bot create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1896">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="0bba9-1897">Eine Änderung wurde vorgenommen, um die zufällige Zuordnung von Ressourcennamen beim Erstellen von Azure Storage-Instanzen, App Service-Plänen, Funktions-/Web-Apps und Application Insights-Instanzen zu verhindern.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1897">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="0bba9-1898">[VERALTET] Argument `--proj-name` zugunsten von `--proj-file-path` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-1898">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="0bba9-1899">`az bot publish` wurde geändert, um abgerufene IIS-Bereitstellungsdateien vom Typ „Node.js“ zu entfernen, wenn sie nicht bereits vorhanden waren.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1899">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="0bba9-1900">Das `--keep-node-modules` Argument wurde zu `az bot publish` hinzugefügt, damit der Ordner `node_modules` in App Service nicht gelöscht wird.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1900">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="0bba9-1901">Das Schlüssel-Wert-Paar `"publishCommand"` wurde der Ausgabe von `az bot create` beim Erstellen einer Funktions-App oder eines Web-App-Bots hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1901">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="0bba9-1902">Der Wert von `"publishCommand"` ist ein `az bot publish`-Befehl, der bereits die erforderlichen Parameter zum Veröffentlichen des neu erstellten Bots enthält.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1902">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="0bba9-1903">`"WEBSITE_NODE_DEFAULT_VERSION"` in der ARM-Vorlage wurde so aktualisiert, dass v4-SDK-Bots 10.14.1 anstelle von 8.9.4 verwenden.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1903">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="0bba9-1904">Key Vault</span><span class="sxs-lookup"><span data-stu-id="0bba9-1904">Key Vault</span></span>
* <span data-ttu-id="0bba9-1905">Ein Problem mit `keyvault secret backup` wurde behoben, aufgrund dessen einige Benutzer bei Verwendung von `--id` einen `unexpected_keyword`-Fehler erhielten.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1905">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="0bba9-1906">Überwachen</span><span class="sxs-lookup"><span data-stu-id="0bba9-1906">Monitor</span></span>
* <span data-ttu-id="0bba9-1907">`monitor metrics alert [create|update]` wurde so geändert, dass der Dimensionswert `*` zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1907">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="0bba9-1908">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0bba9-1908">Network</span></span>
* <span data-ttu-id="0bba9-1909">`dns zone export` wurde geändert, um sicherzustellen, dass es sich bei exportierten CNAMEs um FQDNs handelt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1909">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="0bba9-1910">Parameter `--gateway-name` wurde zu `nic ip-config address-pool [add|remove]` hinzugefügt, um Back-End-Adresspools von Anwendungsgateways zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1910">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="0bba9-1911">Argumente `--traffic-analytics` und `--workspace` wurden zu `network watcher flow-log configure` hinzugefügt, um Datenverkehrsanalysen über einen Log Analytics-Arbeitsbereich zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1911">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="0bba9-1912">`--idle-timeout` und `--floating-ip` wurden zu `lb inbound-nat-pool [create|update]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1912">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="0bba9-1913">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="0bba9-1913">Policy Insights</span></span>
* <span data-ttu-id="0bba9-1914">`policy remediation`-Befehle wurden hinzugefügt, um Korrekturfunktionen der Ressourcenrichtlinie zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1914">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="0bba9-1915">RDBMS</span><span class="sxs-lookup"><span data-stu-id="0bba9-1915">RDBMS</span></span>
* <span data-ttu-id="0bba9-1916">Hilfemeldung und Befehlsparameter wurden verbessert.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1916">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="0bba9-1917">Redis</span><span class="sxs-lookup"><span data-stu-id="0bba9-1917">Redis</span></span>
* <span data-ttu-id="0bba9-1918">Befehle zum Verwalten von „firewall-rules“ (erstellen, aktualisieren, löschen, anzeigen, auflisten) wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1918">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="0bba9-1919">Befehle zum Verwalten von „server-link“ (erstellen, aktualisieren, löschen, anzeigen, auflisten) wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1919">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="0bba9-1920">Befehle zum Verwalten von „patch-schedule“ (erstellen, aktualisieren, löschen, anzeigen, auflisten) wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1920">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="0bba9-1921">Unterstützung für Verfügbarkeitszonen und TLS-Mindestversion wurden zu „redis create“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1921">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="0bba9-1922">[BREAKING CHANGE] Befehle `redis update-settings` und `redis list-all` wurden entfernt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1922">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="0bba9-1923">[BREAKING CHANGE] Parameter für `redis create`: „Mandanteneinstellungen“ werden im Format „Schlüssel[=Wert] nicht akzeptiert.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1923">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="0bba9-1924">[VERALTET] Warnmeldung zur Markierung des Befehls `redis import-method` als veraltet hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1924">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="0bba9-1925">Role</span><span class="sxs-lookup"><span data-stu-id="0bba9-1925">Role</span></span>
* <span data-ttu-id="0bba9-1926">[BREAKING CHANGE] Befehl `az identity` wurde aus den `vm`-Befehlen hierher verschoben.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1926">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="0bba9-1927">SQL-VM</span><span class="sxs-lookup"><span data-stu-id="0bba9-1927">SQL VM</span></span>
* <span data-ttu-id="0bba9-1928">[VERALTET] Argument `--boostrap-acc-pwd` aufgrund eines Tippfehlers als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-1928">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="0bba9-1929">VM</span><span class="sxs-lookup"><span data-stu-id="0bba9-1929">VM</span></span>
* <span data-ttu-id="0bba9-1930">`vm list-skus` wurde so geändert, dass `--all` anstelle von `--all true` verwendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1930">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="0bba9-1931">`vmss run-command [invoke | list | show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1931">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="0bba9-1932">Ein Fehler wurde behoben, aufgrund dessen bei der Ausführung von `vmss encryption enable` bisher ein Fehler auftrat.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1932">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="0bba9-1933">[BREAKING CHANGE] Die Befehle vom Typ `az identity` wurden zu `role`-Befehlen verschoben.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1933">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="0bba9-1934">31. Januar 2019</span><span class="sxs-lookup"><span data-stu-id="0bba9-1934">January 31, 2019</span></span>

<span data-ttu-id="0bba9-1935">Version 2.0.57</span><span class="sxs-lookup"><span data-stu-id="0bba9-1935">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="0bba9-1936">Core</span><span class="sxs-lookup"><span data-stu-id="0bba9-1936">Core</span></span>

* <span data-ttu-id="0bba9-1937">Hotfix für [Problem 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="0bba9-1937">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="0bba9-1938">28. Januar 2019</span><span class="sxs-lookup"><span data-stu-id="0bba9-1938">January 28, 2019</span></span>

<span data-ttu-id="0bba9-1939">Version 2.0.56</span><span class="sxs-lookup"><span data-stu-id="0bba9-1939">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="0bba9-1940">ACR</span><span class="sxs-lookup"><span data-stu-id="0bba9-1940">ACR</span></span>
* <span data-ttu-id="0bba9-1941">Unterstützung für VNet/IP-Regeln wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1941">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="0bba9-1942">ACS</span><span class="sxs-lookup"><span data-stu-id="0bba9-1942">ACS</span></span>
* <span data-ttu-id="0bba9-1943">Virtuelle Knoten (Vorschau) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1943">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="0bba9-1944">Verwaltete OpenShift-Befehle wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1944">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="0bba9-1945">Unterstützung für den Dienstprinzipal-Updatevorgang mit `aks update-credentials -reset-service-principal` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1945">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="0bba9-1946">AMS</span><span class="sxs-lookup"><span data-stu-id="0bba9-1946">AMS</span></span>
* <span data-ttu-id="0bba9-1947">[BREAKING CHANGE]`ams asset get-streaming-locators` in `ams asset list-streaming-locators` umbenannt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1947">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="0bba9-1948">[BREAKING CHANGE]`ams streaming-locator get-content-keys` in `ams streaming-locator list-content-keys` umbenannt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1948">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="0bba9-1949">AppService</span><span class="sxs-lookup"><span data-stu-id="0bba9-1949">Appservice</span></span>
* <span data-ttu-id="0bba9-1950">Unterstützung für App-Erkenntnisse in `functionapp create` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1950">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="0bba9-1951">Unterstützung für die Erstellung von App Service-Plänen (einschließlich Elastic Premium) wurde zu Funktions-Apps hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1951">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="0bba9-1952">Probleme bei einer App-Einstellung mit Elastic Premium-Plänen wurden behoben.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1952">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="0bba9-1953">Container</span><span class="sxs-lookup"><span data-stu-id="0bba9-1953">Container</span></span>
* <span data-ttu-id="0bba9-1954">Befehl `container start` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1954">Added `container start` command</span></span>
* <span data-ttu-id="0bba9-1955">Eine Änderung wurde vorgenommen, um bei der Containererstellung die Verwendung von Dezimalwerten für die CPU zuzulassen.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1955">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="0bba9-1956">EventGrid</span><span class="sxs-lookup"><span data-stu-id="0bba9-1956">EventGrid</span></span>
* <span data-ttu-id="0bba9-1957">Parameter `--deadletter-endpoint` zu `event-subscription [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1957">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="0bba9-1958">„storagequeue“ und „hybridconnection“ wurden als neue Werte für „event-subscription [create|update] --endpoint-type“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1958">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="0bba9-1959">Parameter `--max-delivery-attempts` und `--event-ttl` wurden zu `event-subscription create` hinzugefügt, um die Wiederholungsrichtlinie für Ereignisse anzugeben.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1959">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="0bba9-1960">Eine Warnmeldung wurde zu `event-subscription [create|update]` hinzugefügt, wenn Webhook als Ziel für ein Ereignisabonnement verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1960">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="0bba9-1961">Parameter „source-resource-id“ wurde für alle Befehle im Zusammenhang mit Ereignisabonnements hinzugefügt, und alle anderen Parameter im Zusammenhang mit Quellressourcen wurden als veraltet markiert.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1961">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="0bba9-1962">HDInsight</span><span class="sxs-lookup"><span data-stu-id="0bba9-1962">HDInsight</span></span>
* <span data-ttu-id="0bba9-1963">[BREAKING CHANGE] Die Parameter `--virtual-network` und `--subnet-name` wurden aus `hdinsight [application] create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1963">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="0bba9-1964">[BREAKING CHANGE]`hdinsight create --storage-account` wurde so geändert, dass der Name oder die ID eines Speicherkontos anstellen von Blobendpunkten akzeptiert wird.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1964">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="0bba9-1965">Parameter `--vnet-name` und `--subnet-name` zu `hdinsight create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1965">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="0bba9-1966">Unterstützung für das Enterprise-Sicherheitspaket und Datenträgerverschlüsselung wurde zu `hdinsight create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1966">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="0bba9-1967">Befehl `hdinsight rotate-disk-encryption-key` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1967">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="0bba9-1968">Befehl `hdinsight update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-1968">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="0bba9-1969">IoT</span><span class="sxs-lookup"><span data-stu-id="0bba9-1969">IoT</span></span>
* <span data-ttu-id="0bba9-1970">Codierungsformat wurde zu Befehl „routing-endpoint“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1970">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="0bba9-1971">Kusto</span><span class="sxs-lookup"><span data-stu-id="0bba9-1971">Kusto</span></span>
* <span data-ttu-id="0bba9-1972">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="0bba9-1972">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="0bba9-1973">Überwachen</span><span class="sxs-lookup"><span data-stu-id="0bba9-1973">Monitor</span></span>
* <span data-ttu-id="0bba9-1974">ID-Vergleich wurde so geändert, dass Groß-/Kleinschreibung nicht mehr beachtet wird.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1974">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="0bba9-1975">Profil</span><span class="sxs-lookup"><span data-stu-id="0bba9-1975">Profile</span></span>
* <span data-ttu-id="0bba9-1976">Konto auf Mandantenebene für verwaltete Dienstidentität für `login` wird aktiviert.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1976">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="0bba9-1977">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0bba9-1977">Network</span></span>
* <span data-ttu-id="0bba9-1978">Ein Problem mit `express-route update` wurde behoben, aufgrund dessen das Argument `--bandwidth` ignoriert wurde.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1978">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="0bba9-1979">Ein Problem mit `ddos-protection update` wurde behoben, aufgrund dessen das festgelegte Verständnis zu einer Stapelüberwachung führte.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1979">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="0bba9-1980">Resource</span><span class="sxs-lookup"><span data-stu-id="0bba9-1980">Resource</span></span>
* <span data-ttu-id="0bba9-1981">Unterstützung für die URI-Parameterdatei wurde zu `group deployment create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1981">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="0bba9-1982">Unterstützung für verwaltete Identitäten wurde zu `policy assignment [create|list|show]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1982">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="0bba9-1983">Virtueller SQL-Computer</span><span class="sxs-lookup"><span data-stu-id="0bba9-1983">SQL Virtual Machine</span></span>
* <span data-ttu-id="0bba9-1984">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="0bba9-1984">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="0bba9-1985">Storage</span><span class="sxs-lookup"><span data-stu-id="0bba9-1985">Storage</span></span>
* <span data-ttu-id="0bba9-1986">Eine Lösung wurde so geändert, dass nur Eigenschaften aktualisiert werden, die im selben Objekt geändert werden.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1986">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="0bba9-1987">Nr. 8021 wurde korrigiert, Binärdaten werden bei der Rückgabe in Base64 codiert.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1987">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="0bba9-1988">VM</span><span class="sxs-lookup"><span data-stu-id="0bba9-1988">VM</span></span>
* <span data-ttu-id="0bba9-1989">`vm encryption enable` wurde geändert, um den Schlüsseltresor für die Datenträgerverschlüsselung zu überprüfen und sicherzustellen, dass der Schlüsseltresor für die Schlüsselverschlüsselung vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1989">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="0bba9-1990">Flag `--force` wurde zu `vm encryption enable` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1990">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="0bba9-1991">15. Januar 2019</span><span class="sxs-lookup"><span data-stu-id="0bba9-1991">January 15, 2019</span></span>

<span data-ttu-id="0bba9-1992">Version 2.0.55</span><span class="sxs-lookup"><span data-stu-id="0bba9-1992">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="0bba9-1993">ACR</span><span class="sxs-lookup"><span data-stu-id="0bba9-1993">ACR</span></span>
* <span data-ttu-id="0bba9-1994">Wurde geändert, um den Push eines nicht vorhandenen Helm-Diagramms zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1994">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="0bba9-1995">Wurde geändert, um Laufzeitvorgänge ohne ARM-Anforderungen zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1995">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="0bba9-1996">[VERALTET] Parameter `--resource-group` in folgenden Befehlen als veraltet markiert:</span><span class="sxs-lookup"><span data-stu-id="0bba9-1996">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="0bba9-1997">ACS</span><span class="sxs-lookup"><span data-stu-id="0bba9-1997">ACS</span></span>
* <span data-ttu-id="0bba9-1998">Unterstützung für neue ACI-Regionen wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-1998">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="0bba9-1999">AppService</span><span class="sxs-lookup"><span data-stu-id="0bba9-1999">Appservice</span></span>
* <span data-ttu-id="0bba9-2000">Ein Problem beim Hochladen von Zertifikaten für in einer ASE gehostete Apps wurde behoben, aufgrund dessen die AS-RG und die App-RG nicht übereinstimmten.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2000">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="0bba9-2001">`webapp up` wurde geändert, sodass SKU P1V1 als Standard für Linux verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2001">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="0bba9-2002">`[webapp|functionapp] deployment source config-zip` wurde korrigiert, sodass beim Fehlschlagen einer Bereitstellung die richtige Fehlermeldung angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2002">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="0bba9-2003">Befehl `webapp ssh` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2003">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="0bba9-2004">Botservice</span><span class="sxs-lookup"><span data-stu-id="0bba9-2004">Botservice</span></span>
* <span data-ttu-id="0bba9-2005">Aktualisierungen des Bereitstellungsstatus wurden zu `bot create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2005">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="0bba9-2006">Konfigurieren</span><span class="sxs-lookup"><span data-stu-id="0bba9-2006">Configure</span></span>
* <span data-ttu-id="0bba9-2007">`none` wurde als konfigurierbares Ausgabeformat hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2007">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="0bba9-2008">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="0bba9-2008">CosmosDB</span></span>
* <span data-ttu-id="0bba9-2009">Unterstützung für das Erstellen einer Datenbank mit gemeinsam genutztem Durchsatz wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2009">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="0bba9-2010">HDInsight</span><span class="sxs-lookup"><span data-stu-id="0bba9-2010">HDInsight</span></span>
* <span data-ttu-id="0bba9-2011">Befehle zum Verwalten von Anwendungen wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2011">Added commands for managing applications</span></span>
* <span data-ttu-id="0bba9-2012">Befehle zum Verwalten von Skriptaktionen wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2012">Added commands for managing script actions</span></span>
* <span data-ttu-id="0bba9-2013">Befehle zum Verwalten von der Operations Management Suite (OMS) wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2013">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="0bba9-2014">Unterstützung zum Auflisten der regionalen Nutzung wurde zu `hdinsight list-usage` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2014">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="0bba9-2015">[BREAKING CHANGE] Standardclustertyp wurde aus `hdinsight create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2015">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="0bba9-2016">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0bba9-2016">Network</span></span>
* <span data-ttu-id="0bba9-2017">Argumente `--custom-headers` und `--status-code-ranges` zu `traffic-manager profile [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2017">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="0bba9-2018">Neue Routingtypen wurden hinzugefügt: Subnetz und MultiValue</span><span class="sxs-lookup"><span data-stu-id="0bba9-2018">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="0bba9-2019">Argumente `--custom-headers` und `--subnets` zu `traffic-manager endpoint [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2019">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="0bba9-2020">Eine Problem wurde behoben, aufgrund dessen die Angabe von `--vnets ""` für `ddos-protection update` einen Fehler verursacht hat.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2020">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="0bba9-2021">Role</span><span class="sxs-lookup"><span data-stu-id="0bba9-2021">Role</span></span>
* <span data-ttu-id="0bba9-2022">[VERALTET] Argument `--password` als veraltet markiert für `create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2022">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="0bba9-2023">Verwenden Sie stattdessen sichere, von der CLI generierte Kennwörter.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2023">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="0bba9-2024">Sicherheit</span><span class="sxs-lookup"><span data-stu-id="0bba9-2024">Security</span></span>
* <span data-ttu-id="0bba9-2025">Erstrelease</span><span class="sxs-lookup"><span data-stu-id="0bba9-2025">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="0bba9-2026">Storage</span><span class="sxs-lookup"><span data-stu-id="0bba9-2026">Storage</span></span>
* <span data-ttu-id="0bba9-2027">[BREAKING CHANGE] Die Standardanzahl von Ergebnissen wurde für `storage [blob|file|container|share] list` in 5.000 geändert.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2027">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="0bba9-2028">Verwenden Sie `--num-results *` für das ursprüngliche Verhalten, alle Ergebnisse zurückzugeben.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2028">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="0bba9-2029">Parameter `--marker` zu `storage [blob|file|container|share] list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2029">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="0bba9-2030">Ein Protokollmarker für die nächste Seite wurde zur STDERR für `storage [blob|file|container|share] list` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2030">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="0bba9-2031">Der Befehl `storage blob service-properties update` mit Unterstützung für statische Websites wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2031">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="0bba9-2032">VM</span><span class="sxs-lookup"><span data-stu-id="0bba9-2032">VM</span></span>
* <span data-ttu-id="0bba9-2033">`vm [disk|unmanaged-disk]` und `vmss disk` wurden geändert, sodass sie konsistentere Parameter enthalten.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2033">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="0bba9-2034">Unterstützung für mandantenübergreifende Imageverweise wurden zu `[vm|vmss] create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2034">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="0bba9-2035">Fehler bei Standardkonfiguration in `vm diagnostics get-default-config --windows-os` wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2035">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="0bba9-2036">Argument `--provision-after-extensions` wurde zu `vmss extension set` hinzugefügt, um zu definieren, welche Erweiterungen vor dem Festlegen der Erweiterung bereitgestellt werden müssen.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2036">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="0bba9-2037">Argument `--replica-count` wurde zu `sig image-version update` hinzugefügt, um die Standardanzahl für die Replikation festzulegen.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2037">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="0bba9-2038">Fehler bei `image create --source` wurde behoben, aufgrund dessen, der Quellbetriebssystem-Datenträger für einen virtuellen Computer mit dem gleichen Namen gehalten wurde, selbst wenn die vollständige Ressourcen-ID angegeben war.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2038">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="0bba9-2039">20. Dezember 2018</span><span class="sxs-lookup"><span data-stu-id="0bba9-2039">December 20, 2018</span></span>

<span data-ttu-id="0bba9-2040">Version 2.0.54</span><span class="sxs-lookup"><span data-stu-id="0bba9-2040">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="0bba9-2041">AppService</span><span class="sxs-lookup"><span data-stu-id="0bba9-2041">Appservice</span></span>
* <span data-ttu-id="0bba9-2042">Problem behoben, bei dem `webapp up` nicht erneut bereitgestellt werden konnte</span><span class="sxs-lookup"><span data-stu-id="0bba9-2042">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="0bba9-2043">Unterstützung für das Auflisten und Wiederherstellen von Web-App-Momentaufnahmen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2043">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="0bba9-2044">Unterstützung für das Flag `--runtime` zu Windows-Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2044">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="0bba9-2045">IoTCentral</span><span class="sxs-lookup"><span data-stu-id="0bba9-2045">IoTCentral</span></span>
* <span data-ttu-id="0bba9-2046">Fehler bei API-Aufruf für update-Befehl behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-2046">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="0bba9-2047">Role</span><span class="sxs-lookup"><span data-stu-id="0bba9-2047">Role</span></span>
* <span data-ttu-id="0bba9-2048">[BREAKING CHANGE]`ad [app|sp] list` geändert, damit standardmäßig nur die ersten 100 Objekte aufgelistet werden</span><span class="sxs-lookup"><span data-stu-id="0bba9-2048">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="0bba9-2049">SQL</span><span class="sxs-lookup"><span data-stu-id="0bba9-2049">SQL</span></span>
* <span data-ttu-id="0bba9-2050">Unterstützung für die benutzerdefinierte Sortierung auf verwalteten Instanzen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2050">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="0bba9-2051">VM</span><span class="sxs-lookup"><span data-stu-id="0bba9-2051">VM</span></span>
* <span data-ttu-id="0bba9-2052">Parameter `---os-type` zu `disk create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2052">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="0bba9-2053">18. Dezember 2018</span><span class="sxs-lookup"><span data-stu-id="0bba9-2053">December 18, 2018</span></span>

<span data-ttu-id="0bba9-2054">Version 2.0.53</span><span class="sxs-lookup"><span data-stu-id="0bba9-2054">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="0bba9-2055">ACR</span><span class="sxs-lookup"><span data-stu-id="0bba9-2055">ACR</span></span>
* <span data-ttu-id="0bba9-2056">Unterstützung für Imageimport aus externen Containerregistrierungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2056">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="0bba9-2057">Tabellenlayout für Aufgabenliste komprimiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-2057">Condensed the table layout for task list</span></span>
* <span data-ttu-id="0bba9-2058">Unterstützung für Azure DevOps-URLs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2058">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="0bba9-2059">ACS</span><span class="sxs-lookup"><span data-stu-id="0bba9-2059">ACS</span></span>
* <span data-ttu-id="0bba9-2060">Virtuelle Knoten (Vorschau) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2060">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="0bba9-2061">„(PREVIEW)“ aus AAD-Argumenten für `aks create` entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2061">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="0bba9-2062">[VERALTET]`az acs`-Befehle als veraltet markiert.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2062">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="0bba9-2063">ACS wird am 31. Januar 2020 eingestellt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2063">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="0bba9-2064">Unterstützung für Netzwerkrichtlinie bei der Erstellung neuer AKS-Cluster hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2064">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="0bba9-2065">Anforderung des Arguments `--nodepool-name` bei nur einem Knotenpool für `aks scale` entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2065">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="0bba9-2066">AppService</span><span class="sxs-lookup"><span data-stu-id="0bba9-2066">Appservice</span></span>
* <span data-ttu-id="0bba9-2067">Problem behoben, bei dem für `webapp config container` der Parameter `--slot` nicht berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="0bba9-2067">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="0bba9-2068">Botservice</span><span class="sxs-lookup"><span data-stu-id="0bba9-2068">Botservice</span></span>
* <span data-ttu-id="0bba9-2069">Unterstützung für Analyse von `.bot`-Dateien beim Aufrufen von `bot show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2069">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="0bba9-2070">Fehler bei der AppInsights-Bereitstellung behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-2070">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="0bba9-2071">Leerzeichenfehler bei Dateipfaden behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-2071">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="0bba9-2072">Kudu-Netzwerkaufrufe reduziert</span><span class="sxs-lookup"><span data-stu-id="0bba9-2072">Reduced Kudu network calls</span></span>
* <span data-ttu-id="0bba9-2073">Allgemeine Verbesserungen bei Befehlen der Benutzeroberfläche durchgeführt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2073">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="0bba9-2074">Nutzung</span><span class="sxs-lookup"><span data-stu-id="0bba9-2074">Consumption</span></span>
* <span data-ttu-id="0bba9-2075">Fehler für Budget-API zum Anzeigen von Benachrichtigungen behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-2075">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="0bba9-2076">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="0bba9-2076">CosmosDB</span></span>
* <span data-ttu-id="0bba9-2077">Unterstützung für die Aktualisierung des Kontos von „Singlemaster“ auf „Multimaster“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2077">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="0bba9-2078">Karten</span><span class="sxs-lookup"><span data-stu-id="0bba9-2078">Maps</span></span>
* <span data-ttu-id="0bba9-2079">Unterstützung für SKU „S1“ für `maps account [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2079">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="0bba9-2080">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0bba9-2080">Network</span></span>
* <span data-ttu-id="0bba9-2081">Unterstützung für `--format` und `--log-version` für `watcher flow-log configure` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2081">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="0bba9-2082">Problem mit `dns zone update` behoben, bei dem die Verwendung von "" zum Löschen von Auflösungs- und Registrierungs-VNETs nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="0bba9-2082">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="0bba9-2083">Resource</span><span class="sxs-lookup"><span data-stu-id="0bba9-2083">Resource</span></span>
* <span data-ttu-id="0bba9-2084">Verarbeitung des Bereichsparameters für Verwaltungsgruppen in `policy assignment [create|list|delete|show|update]` behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-2084">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="0bba9-2085">Neuen Befehl `resource wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2085">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="0bba9-2086">Storage</span><span class="sxs-lookup"><span data-stu-id="0bba9-2086">Storage</span></span>
*  <span data-ttu-id="0bba9-2087">Möglichkeit zum Aktualisieren der Protokollschemaversion für Speicherdienste in `storage logging update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2087">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="0bba9-2088">VM</span><span class="sxs-lookup"><span data-stu-id="0bba9-2088">VM</span></span>
* <span data-ttu-id="0bba9-2089">Absturz in `vm identity remove` behoben, der aufgetreten ist, wenn der angegebenen VM keine verwalteten Dienstidentitäten zugewiesen waren</span><span class="sxs-lookup"><span data-stu-id="0bba9-2089">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="0bba9-2090">4\. Dezember 2018</span><span class="sxs-lookup"><span data-stu-id="0bba9-2090">December 4, 2018</span></span>

<span data-ttu-id="0bba9-2091">Version 2.0.52</span><span class="sxs-lookup"><span data-stu-id="0bba9-2091">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="0bba9-2092">Core</span><span class="sxs-lookup"><span data-stu-id="0bba9-2092">Core</span></span>
* <span data-ttu-id="0bba9-2093">Unterstützung für mandantenübergreifende Ressourcenbereitstellung für mehrinstanzenfähigen Dienstprinzipal hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2093">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="0bba9-2094">Behebung eines Fehlers, aufgrund dessen IDs, die von einem Befehl mit Ausgabe im TSV-Format weitergeleitet wurden, nicht ordnungsgemäß analysiert wurden</span><span class="sxs-lookup"><span data-stu-id="0bba9-2094">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="0bba9-2095">AppService</span><span class="sxs-lookup"><span data-stu-id="0bba9-2095">Appservice</span></span>
* <span data-ttu-id="0bba9-2096">[VORSCHAU] Befehl `webapp up` hinzugefügt, der Benutzer beim Erstellen und Bereitstellen von Inhalten in Apps unterstützt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2096">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="0bba9-2097">Behebung eines Fehlers in einer containerbasierten Windows-App, der aufgrund einer Back-End-Änderung auftrat</span><span class="sxs-lookup"><span data-stu-id="0bba9-2097">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="0bba9-2098">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0bba9-2098">Network</span></span>
* <span data-ttu-id="0bba9-2099">Argument `--exclusion` zu `application-gateway waf-config set` hinzugefügt, um WAF-Ausschlüsse zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="0bba9-2099">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="0bba9-2100">Role</span><span class="sxs-lookup"><span data-stu-id="0bba9-2100">Role</span></span>
* <span data-ttu-id="0bba9-2101">Unterstützung für benutzerdefinierte Bezeichner für Kennwortanmeldeinformation hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2101">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="0bba9-2102">VM</span><span class="sxs-lookup"><span data-stu-id="0bba9-2102">VM</span></span>
* <span data-ttu-id="0bba9-2103">[VERALTET] Parameter `vm extension [show|wait] --expand` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-2103">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="0bba9-2104">Parameter `--force` zu `vm restart` hinzugefügt, um nicht reagierende virtuelle Computer erneut bereitzustellen</span><span class="sxs-lookup"><span data-stu-id="0bba9-2104">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="0bba9-2105">`[vm|vmss] create --authentication-type` geändert, um „all“ zu akzeptieren und einen virtuellen Computer mit Kennwort- und SSH-Authentifizierung zu erstellen</span><span class="sxs-lookup"><span data-stu-id="0bba9-2105">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="0bba9-2106">Parameter `image create --os-disk-caching` hinzugefügt, um die Zwischenspeicherung von Betriebssystemdatenträgern für ein Image festzulegen</span><span class="sxs-lookup"><span data-stu-id="0bba9-2106">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="0bba9-2107">20. November 2018</span><span class="sxs-lookup"><span data-stu-id="0bba9-2107">November 20, 2018</span></span>

<span data-ttu-id="0bba9-2108">Version 2.0.51</span><span class="sxs-lookup"><span data-stu-id="0bba9-2108">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="0bba9-2109">Core</span><span class="sxs-lookup"><span data-stu-id="0bba9-2109">Core</span></span>
* <span data-ttu-id="0bba9-2110">MSI-Anmeldung geändert, sodass der Abonnementname nicht in der Identität wiederverwendet wird</span><span class="sxs-lookup"><span data-stu-id="0bba9-2110">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="0bba9-2111">ACR</span><span class="sxs-lookup"><span data-stu-id="0bba9-2111">ACR</span></span>
* <span data-ttu-id="0bba9-2112">Kontexttoken zum Aufgabenschritt hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2112">Added context token to task step</span></span>
* <span data-ttu-id="0bba9-2113">Unterstützung für das Festlegen von Geheimnissen in „acr run“ zum Spiegeln der ACR-Aufgabe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2113">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="0bba9-2114">Unterstützung für `--top` und `--orderby` für die Befehle `show-tags` und `show-manifests` verbessert</span><span class="sxs-lookup"><span data-stu-id="0bba9-2114">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="0bba9-2115">AppService</span><span class="sxs-lookup"><span data-stu-id="0bba9-2115">Appservice</span></span>
* <span data-ttu-id="0bba9-2116">Standardtimeout der ZIP-Bereitstellung für das Abrufen des Status auf fünf Minuten erhöht und Timeout-Eigenschaft zum Anpassen dieses Werts hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2116">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="0bba9-2117">Aktualisierung der standardmäßigen `node_version`.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2117">Updated the default `node_version`.</span></span> <span data-ttu-id="0bba9-2118">Während eines Austauschvorgangs mit zwei Phasen werden bei der Austauschaktion zum Zurücksetzen des Slots alle App-Einstellungen und Verbindungszeichenfolgen beibehalten.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2118">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="0bba9-2119">Clientseitige SKU-Überprüfung für die Erstellung eines Linux-App Service-Plans entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2119">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="0bba9-2120">Behebung eines Fehlers beim Abrufen des ZipDeploy-Status</span><span class="sxs-lookup"><span data-stu-id="0bba9-2120">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="0bba9-2121">IotCentral</span><span class="sxs-lookup"><span data-stu-id="0bba9-2121">IotCentral</span></span>
* <span data-ttu-id="0bba9-2122">Verfügbarkeitsprüfung für Unterdomänen beim Erstellen einer IoT Central-Anwendung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2122">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="0bba9-2123">KeyVault</span><span class="sxs-lookup"><span data-stu-id="0bba9-2123">KeyVault</span></span>
* <span data-ttu-id="0bba9-2124">Behebung eines Fehlers, aufgrund dessen Fehler mitunter ignoriert wurden</span><span class="sxs-lookup"><span data-stu-id="0bba9-2124">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="0bba9-2125">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0bba9-2125">Network</span></span>
* <span data-ttu-id="0bba9-2126">`root-cert`-Unterbefehle zum Behandeln von vertrauenswürdigen Stammzertifikaten zu `application-gateway` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2126">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="0bba9-2127">Optionen `--min-capacity` und `--custom-error-pages` zu `application-gateway [create|update]` hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="0bba9-2127">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="0bba9-2128">`--zones` zur Unterstützung von Verfügbarkeitszonen zu `application-gateway create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2128">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="0bba9-2129">Argumente `--file-upload-limit`, `--max-request-body-size` und `--request-body-check` zu `application-gateway waf-config set` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2129">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="0bba9-2130">Rdbms</span><span class="sxs-lookup"><span data-stu-id="0bba9-2130">Rdbms</span></span>
* <span data-ttu-id="0bba9-2131">MariaDB-VNET-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2131">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="0bba9-2132">RBAC</span><span class="sxs-lookup"><span data-stu-id="0bba9-2132">Rbac</span></span>
* <span data-ttu-id="0bba9-2133">Problem beim Aktualisieren unveränderlicher Anmeldeinformationen in `ad app update` behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-2133">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="0bba9-2134">Ausgabewarnungen zur Ankündigung bevorstehender Breaking Changes für `ad [app|sp] list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2134">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="0bba9-2135">Storage</span><span class="sxs-lookup"><span data-stu-id="0bba9-2135">Storage</span></span>
* <span data-ttu-id="0bba9-2136">Behandlung von Ausnahmefällen für Speicherkopierbefehle verbessert</span><span class="sxs-lookup"><span data-stu-id="0bba9-2136">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="0bba9-2137">Problem behoben, aufgrund dessen `storage blob copy start-batch` bei identischen Ziel- und Quellkonten keine Anmeldeinformationen verwendete</span><span class="sxs-lookup"><span data-stu-id="0bba9-2137">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="0bba9-2138">Fehler bei `storage [blob|file] url` behoben, aufgrund dessen `sas_token` nicht in die URL eingebunden wurde</span><span class="sxs-lookup"><span data-stu-id="0bba9-2138">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="0bba9-2139">Breaking Change-Warnung zu `[blob|container] list` hinzugefügt: In Kürze werden standardmäßig nur die ersten 5.000 Ergebnisse ausgegeben.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2139">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="0bba9-2140">VM</span><span class="sxs-lookup"><span data-stu-id="0bba9-2140">VM</span></span>
* <span data-ttu-id="0bba9-2141">Unterstützung für die separate Angabe einer Speicherkonto-SKU für verwaltete Betriebssystemdatenträger und Datenträger zu `[vm|vmss] create --storage-sku` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2141">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="0bba9-2142">Parameter für den Versionsnamen von `sig image-version` in `--image-version -e` geändert</span><span class="sxs-lookup"><span data-stu-id="0bba9-2142">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="0bba9-2143">`sig image-version`-Argument `--image-version-name` als veraltet markiert und durch `--image-version` ersetzt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2143">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="0bba9-2144">Unterstützung für die Verwendung des lokalen Betriebssystemdatenträgers für `[vm|vmss] create --ephemeral-os-disk` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2144">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="0bba9-2145">Unterstützung für `--no-wait` zu `snapshot create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2145">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="0bba9-2146">Befehl `snapshot wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2146">Added `snapshot wait` command</span></span>
* <span data-ttu-id="0bba9-2147">Unterstützung für die Verwendung von Instanznamen mit `[vm|vmss] extension set --extension-instance-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2147">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="0bba9-2148">6\. November 2018</span><span class="sxs-lookup"><span data-stu-id="0bba9-2148">November 6, 2018</span></span>

<span data-ttu-id="0bba9-2149">Version 2.0.50</span><span class="sxs-lookup"><span data-stu-id="0bba9-2149">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="0bba9-2150">Core</span><span class="sxs-lookup"><span data-stu-id="0bba9-2150">Core</span></span>
* <span data-ttu-id="0bba9-2151">Unterstützung für die Dienstprinzipalauthentifizierung (SN und Aussteller) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2151">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="0bba9-2152">ACR</span><span class="sxs-lookup"><span data-stu-id="0bba9-2152">ACR</span></span>
* <span data-ttu-id="0bba9-2153">Unterstützung für Commit- und Pull Request-Git-Ereignisse für Aufgabenquellentrigger hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2153">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="0bba9-2154">Auf Verwendung des Standard-Dockerfiles umgestellt, falls im Erstellungsbefehl kein Dockerfile angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="0bba9-2154">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="0bba9-2155">ACS</span><span class="sxs-lookup"><span data-stu-id="0bba9-2155">ACS</span></span>
* <span data-ttu-id="0bba9-2156">[BREAKING CHANGE]`enable_cloud_console_aks_browse` entfernt, um standardmäßig „az aks browse“ zu aktivieren</span><span class="sxs-lookup"><span data-stu-id="0bba9-2156">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="0bba9-2157">Advisor</span><span class="sxs-lookup"><span data-stu-id="0bba9-2157">Advisor</span></span>
* <span data-ttu-id="0bba9-2158">Allgemein verfügbares Release</span><span class="sxs-lookup"><span data-stu-id="0bba9-2158">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="0bba9-2159">AMS</span><span class="sxs-lookup"><span data-stu-id="0bba9-2159">AMS</span></span>
* <span data-ttu-id="0bba9-2160">Neue Befehlsgruppen hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="0bba9-2160">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="0bba9-2161">Neue Befehle hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="0bba9-2161">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="0bba9-2162">Unterstützung von Verschlüsselungsparametern für `ams streaming-policy create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2162">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="0bba9-2163">Für `ams transform output remove` kann jetzt der zu entfernende Ausgabeindex angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2163">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="0bba9-2164">Argumente `--correlation-data` und `--label` zur Befehlsgruppe `ams job` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2164">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="0bba9-2165">Argumente `--storage-account` und `--container` zur Befehlsgruppe `ams asset` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2165">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="0bba9-2166">Standardwerte für Ablaufzeit (aktueller Zeitpunkt + 23 Std.) und Berechtigungen (Lesen) im Befehl `ams asset get-sas-url` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2166">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="0bba9-2167">[BREAKING CHANGE] Befehl `ams streaming locator` durch `ams streaming-locator` ersetzt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2167">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="0bba9-2168">[BREAKING CHANGE] Argument `--content-keys` von `ams streaming locator` aktualisiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-2168">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="0bba9-2169">[BREAKING CHANGE]`--content-policy-name` im Befehl `ams streaming locator` in `--content-key-policy-name` umbenannt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2169">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="0bba9-2170">[BREAKING CHANGE] Befehl `ams streaming policy` durch `ams streaming-policy` ersetzt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2170">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="0bba9-2171">[BREAKING CHANGE] Das Argument `--preset-names` wurde in der Befehlsgruppe `--preset` durch `ams transform` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2171">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="0bba9-2172">Ab sofort kann nur noch eine einzelne Ausgabe/Voreinstellung festgelegt werden. (Wenn Sie weitere hinzufügen möchten, müssen Sie `ams transform output add` ausführen.)</span><span class="sxs-lookup"><span data-stu-id="0bba9-2172">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="0bba9-2173">Darüber hinaus können Sie eine benutzerdefinierte Voreinstellung für den Standard-Encoder (StandardEncoderPreset) festlegen, indem Sie den Pfad an Ihr benutzerdefiniertes JSON-Objekt übergeben.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2173">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="0bba9-2174">[BREAKING CHANGE]`--output-asset-names ` wurde im Befehl `ams job start` in `--output-assets` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2174">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="0bba9-2175">Ab sofort wird eine durch Leerzeichen getrennte Ressourcenliste im Format „assetName=Bezeichnung“ akzeptiert.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2175">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="0bba9-2176">Ressourcen ohne Bezeichnung können wie folgt gesendet werden: „assetName=“.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2176">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="0bba9-2177">AppService</span><span class="sxs-lookup"><span data-stu-id="0bba9-2177">AppService</span></span>
* <span data-ttu-id="0bba9-2178">Fehler in `az webapp config backup update` behoben, der dazu führte, dass kein Sicherungszeitplan festgelegt werden konnte, wenn noch keiner festgelegt war</span><span class="sxs-lookup"><span data-stu-id="0bba9-2178">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="0bba9-2179">Konfigurieren</span><span class="sxs-lookup"><span data-stu-id="0bba9-2179">Configure</span></span>
* <span data-ttu-id="0bba9-2180">YAML zu Ausgabeformatoptionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2180">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="0bba9-2181">Container</span><span class="sxs-lookup"><span data-stu-id="0bba9-2181">Container</span></span>
* <span data-ttu-id="0bba9-2182">Auf Anzeige der Identität umgestellt, wenn eine Containergruppe nach YAML exportiert wird</span><span class="sxs-lookup"><span data-stu-id="0bba9-2182">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="0bba9-2183">EventHub</span><span class="sxs-lookup"><span data-stu-id="0bba9-2183">EventHub</span></span>
* <span data-ttu-id="0bba9-2184">Flag `--enable-kafka` hinzugefügt, um Kafka in `eventhub namespace [create|update]` zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="0bba9-2184">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="0bba9-2185">Interactive</span><span class="sxs-lookup"><span data-stu-id="0bba9-2185">Interactive</span></span>
* <span data-ttu-id="0bba9-2186">Interactive installiert nun die Erweiterung `interactive`, um schnellere Updates und schnelleren Support zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="0bba9-2186">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="0bba9-2187">Überwachen</span><span class="sxs-lookup"><span data-stu-id="0bba9-2187">Monitor</span></span>
* <span data-ttu-id="0bba9-2188">Unterstützung für Metriknamen mit Schrägstrichen und Punkten zu `--condition` in `monitor metrics alert [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2188">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="0bba9-2189">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0bba9-2189">Network</span></span>
* <span data-ttu-id="0bba9-2190">Befehlsnamen vom Typ `network interface-endpoint` zugunsten von `network private-endpoint` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-2190">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="0bba9-2191">Problem behoben, das dazu führte, dass das Argument `--peer-circuit` in `express-route peering connection create` keine ID akzeptiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-2191">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="0bba9-2192">Problem behoben, das dazu führte, dass `--ip-tags` mit `public-ip create` nicht ordnungsgemäß funktioniert</span><span class="sxs-lookup"><span data-stu-id="0bba9-2192">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="0bba9-2193">Profil</span><span class="sxs-lookup"><span data-stu-id="0bba9-2193">Profile</span></span>
* <span data-ttu-id="0bba9-2194">`--use-cert-sn-issuer` zu `az login` hinzugefügt, um Dienstprinzipalanmeldungen mit automatischem Zertifikatrollover zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="0bba9-2194">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="0bba9-2195">RDBMS</span><span class="sxs-lookup"><span data-stu-id="0bba9-2195">RDBMS</span></span>
* <span data-ttu-id="0bba9-2196">MySQL-Replikatbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2196">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="0bba9-2197">Resource</span><span class="sxs-lookup"><span data-stu-id="0bba9-2197">Resource</span></span>
* <span data-ttu-id="0bba9-2198">Unterstützung für Verwaltungsgruppen und Abonnements zu Befehlen vom Typ `policy definition|set-definition` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2198">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="0bba9-2199">Role</span><span class="sxs-lookup"><span data-stu-id="0bba9-2199">Role</span></span>
* <span data-ttu-id="0bba9-2200">Unterstützung für die API-Berechtigungsverwaltung, den angemeldeten Benutzer und die Verwaltung von Anwendungskennwörtern und Zertifikatanmeldeinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2200">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="0bba9-2201">`ad sp create-for-rbac` geändert, um „displayName“ und Dienstprinzipalname besser unterscheiden zu können</span><span class="sxs-lookup"><span data-stu-id="0bba9-2201">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="0bba9-2202">Unterstützung der Gewährung von Berechtigungen für AAD-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2202">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="0bba9-2203">Storage</span><span class="sxs-lookup"><span data-stu-id="0bba9-2203">Storage</span></span>
* <span data-ttu-id="0bba9-2204">Möglichkeit hinzugefügt, allein mit SAS und Endpunkten (ohne Kontoname oder Schlüssel) eine Verbindung mit Speicherdiensten herzustellen, wie unter `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>` beschrieben</span><span class="sxs-lookup"><span data-stu-id="0bba9-2204">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="0bba9-2205">VM</span><span class="sxs-lookup"><span data-stu-id="0bba9-2205">VM</span></span>
* <span data-ttu-id="0bba9-2206">Argument `storage-sku` zu `image create` hinzugefügt, um das Festlegen des standardmäßigen Speicherkontotyps für das Image zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="0bba9-2206">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="0bba9-2207">Fehler für `vm resize` behoben, durch den die Option `--no-wait` einen Absturz des Befehls verursachte</span><span class="sxs-lookup"><span data-stu-id="0bba9-2207">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="0bba9-2208">Tabellenausgabeformat für `vm encryption show` geändert, um den Status anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="0bba9-2208">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="0bba9-2209">`vm secret format` geändert, um JSON/JSONC-Ausgabe erforderlich zu machen.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2209">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="0bba9-2210">Der Benutzer wird gewarnt, und es wird standardmäßig die JSON-Ausgabe verwendet, wenn ein unzulässiges Ausgabeformat ausgewählt wird.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2210">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="0bba9-2211">Argumentüberprüfung für `vm create --image` verbessert</span><span class="sxs-lookup"><span data-stu-id="0bba9-2211">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="0bba9-2212">23. Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="0bba9-2212">October 23, 2018</span></span>

<span data-ttu-id="0bba9-2213">Version 2.0.49</span><span class="sxs-lookup"><span data-stu-id="0bba9-2213">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="0bba9-2214">Core</span><span class="sxs-lookup"><span data-stu-id="0bba9-2214">Core</span></span>
* <span data-ttu-id="0bba9-2215">Problem mit `--ids` behoben, aufgrund dessen `--subscription` Vorrang vor dem Abonnement in `--ids` hatte</span><span class="sxs-lookup"><span data-stu-id="0bba9-2215">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="0bba9-2216">Ausdrückliche Warnungen hinzugefügt, wenn Parameter durch die Verwendung von `--ids` ignoriert würden</span><span class="sxs-lookup"><span data-stu-id="0bba9-2216">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="0bba9-2217">ACR</span><span class="sxs-lookup"><span data-stu-id="0bba9-2217">ACR</span></span>
* <span data-ttu-id="0bba9-2218">Problem mit der ACR Build-Codierung in Python2 behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-2218">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="0bba9-2219">CDN</span><span class="sxs-lookup"><span data-stu-id="0bba9-2219">CDN</span></span>
* <span data-ttu-id="0bba9-2220">[BREAKING CHANGE] Standardverhalten beim Zwischenspeichern der Abfragezeichenfolge von `cdn endpoint create` so geändert, dass der Standardwert nicht mehr „IgnoreQueryString“ ist.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2220">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="0bba9-2221">Er wird jetzt vom Dienst festgelegt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2221">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="0bba9-2222">Container</span><span class="sxs-lookup"><span data-stu-id="0bba9-2222">Container</span></span>
* <span data-ttu-id="0bba9-2223">`Private` als gültiger Typ für die Übergabe an „--ip-address“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2223">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="0bba9-2224">Geändert, sodass nur eine Subnetz-ID für das Einrichten eines virtuellen Netzwerks für die Containergruppe zulässig ist</span><span class="sxs-lookup"><span data-stu-id="0bba9-2224">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="0bba9-2225">Geändert, sodass das Verwenden eines VNET-Namens oder einer Ressourcen-ID zulässig ist, um die Verwendung von VNETs aus verschiedenen Ressourcengruppen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="0bba9-2225">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="0bba9-2226">`--assign-identity` hinzugefügt, um einer Containergruppe eine MSI-Identität hinzuzufügen</span><span class="sxs-lookup"><span data-stu-id="0bba9-2226">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="0bba9-2227">`--scope` hinzugefügt, um eine Rollenzuweisung für die vom System zugewiesene MSI-Identität zu erstellen</span><span class="sxs-lookup"><span data-stu-id="0bba9-2227">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="0bba9-2228">Warnung hinzugefügt, wenn eine Containergruppe mit einem Image ohne Prozess mit langer Ausführungszeit erstellt wird</span><span class="sxs-lookup"><span data-stu-id="0bba9-2228">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="0bba9-2229">Probleme mit der Tabellenausgabe für Befehle `list` und `show` behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-2229">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="0bba9-2230">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="0bba9-2230">CosmosDB</span></span>
* <span data-ttu-id="0bba9-2231">Unterstützung für `--enable-multiple-write-locations` zu `cosmosdb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2231">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="0bba9-2232">Interactive</span><span class="sxs-lookup"><span data-stu-id="0bba9-2232">Interactive</span></span>
* <span data-ttu-id="0bba9-2233">Geändert, um sicherzustellen, dass der Parameter für globales Abonnement in Parametern angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="0bba9-2233">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="0bba9-2234">IoT Central</span><span class="sxs-lookup"><span data-stu-id="0bba9-2234">IoT Central</span></span>
* <span data-ttu-id="0bba9-2235">Optionen für Vorlagen und Anzeigenamen für die Erstellung von IoT Central-Anwendungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2235">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="0bba9-2236">[BREAKING CHANGE] Unterstützung für F1-SKU entfernt; stattdessen ist die S1-SKU zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2236">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="0bba9-2237">Überwachen</span><span class="sxs-lookup"><span data-stu-id="0bba9-2237">Monitor</span></span>
* <span data-ttu-id="0bba9-2238">Änderungen an `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="0bba9-2238">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="0bba9-2239">Unterstützung für das Auflisten aller Ereignisse auf Abonnementebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2239">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="0bba9-2240">`--offset`-Parameter für das einfachere Erstellen von Zeitabfragen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2240">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="0bba9-2241">Validierung für `--start-time` und `--end-time` verbessert, um die Verwendung von mehr ISO8601-Formate und benutzerfreundlicheren datetime-Formaten zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="0bba9-2241">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="0bba9-2242">`--namespace` als Alias für veraltete Option `--resource-provider` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2242">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="0bba9-2243">`--filters` als veraltet markiert, da vom Dienst ausschließlich Werte mit stark typisierten Optionen unterstützt werden</span><span class="sxs-lookup"><span data-stu-id="0bba9-2243">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="0bba9-2244">Änderungen an `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="0bba9-2244">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="0bba9-2245">`--offset`-Parameter für das einfachere Erstellen von Zeitabfragen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2245">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="0bba9-2246">Validierung für `--start-time` und `--end-time` verbessert, um die Verwendung von mehr ISO8601-Formate und benutzerfreundlicheren datetime-Formaten zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="0bba9-2246">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="0bba9-2247">Validierung für `--event-hub`- und `--event-hub-rule`-Argumente an `monitor diagnostic-settings create` verbessert</span><span class="sxs-lookup"><span data-stu-id="0bba9-2247">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="0bba9-2248">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0bba9-2248">Network</span></span>
* <span data-ttu-id="0bba9-2249">`--app-gateway-address-pools`- und `--gateway-name`-Argumente zu `nic create` hinzugefügt, um das Hinzufügen von Back-End-Adresspools für Anwendungsgateways zu einer NIC zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="0bba9-2249">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="0bba9-2250">`--app-gateway-address-pools`- und `--gateway-name`-Argumente zu `nic ip-config create/update` hinzugefügt, um das Hinzufügen von Back-End-Adresspools für Anwendungsgateways zu einer NIC zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="0bba9-2250">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="0bba9-2251">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="0bba9-2251">ServiceBus</span></span>
* <span data-ttu-id="0bba9-2252">Schreibgeschütztes `migration_state`-Element zu „MigrationConfigProperties“ hinzugefügt, um den aktuellen Status der Migration von Service Bus Standard- zu Premium-Namespace anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="0bba9-2252">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="0bba9-2253">SQL</span><span class="sxs-lookup"><span data-stu-id="0bba9-2253">SQL</span></span>
* <span data-ttu-id="0bba9-2254">`sql failover-group create` und `sql failover-group update` korrigiert, damit die Verwendung einer Richtlinie für manuelles Failover möglich ist</span><span class="sxs-lookup"><span data-stu-id="0bba9-2254">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="0bba9-2255">Storage</span><span class="sxs-lookup"><span data-stu-id="0bba9-2255">Storage</span></span>
* <span data-ttu-id="0bba9-2256">Formatierung der `az storage cors list`-Ausgabe korrigiert, sodass alle Elemente den richtigen Dienstschlüssel anzeigen</span><span class="sxs-lookup"><span data-stu-id="0bba9-2256">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="0bba9-2257">`--bypass-immutability-policy`-Parameter für das Löschen von durch Unveränderlichkeitsrichtlinien blockierten Containern hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2257">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="0bba9-2258">VM</span><span class="sxs-lookup"><span data-stu-id="0bba9-2258">VM</span></span>
* <span data-ttu-id="0bba9-2259">Datenträger-Zwischenspeicherungsmodus `None` für Lv/Lv2-Computerserine in `[vm|vmss] create` erzwungen</span><span class="sxs-lookup"><span data-stu-id="0bba9-2259">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="0bba9-2260">Liste der unterstützten Größen für unterstützenden Netzwerkbeschleuniger für `vm create` aktualisiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-2260">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="0bba9-2261">Stark typisierte Argumente für UltraSSD-IOPS und MBit/s-Konfigurationen für `disk create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2261">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="0bba9-2262">16. Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="0bba9-2262">October 16, 2018</span></span>

<span data-ttu-id="0bba9-2263">Version 2.0.48</span><span class="sxs-lookup"><span data-stu-id="0bba9-2263">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="0bba9-2264">VM</span><span class="sxs-lookup"><span data-stu-id="0bba9-2264">VM</span></span>
* <span data-ttu-id="0bba9-2265">SDK-Problem behoben, das ein Fehlschlagen der Homebrew-Installation verursacht hat</span><span class="sxs-lookup"><span data-stu-id="0bba9-2265">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="0bba9-2266">9\. Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="0bba9-2266">October 9, 2018</span></span>

<span data-ttu-id="0bba9-2267">Version 2.0.47</span><span class="sxs-lookup"><span data-stu-id="0bba9-2267">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="0bba9-2268">Core</span><span class="sxs-lookup"><span data-stu-id="0bba9-2268">Core</span></span>
* <span data-ttu-id="0bba9-2269">Verbesserte Fehlerbehandlung für Fehler vom Typ „Ungültige Anforderung“</span><span class="sxs-lookup"><span data-stu-id="0bba9-2269">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="0bba9-2270">ACR</span><span class="sxs-lookup"><span data-stu-id="0bba9-2270">ACR</span></span>
* <span data-ttu-id="0bba9-2271">Unterstützung für ähnliches Tabellenformat wie Helm-Client hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2271">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="0bba9-2272">ACS</span><span class="sxs-lookup"><span data-stu-id="0bba9-2272">ACS</span></span>
* <span data-ttu-id="0bba9-2273">`aks [create|scale] --nodepool-name` zum Konfigurieren des Knotenpoolnamens hinzugefügt, auf 12 Zeichen gekürzt, Standard: nodepool1</span><span class="sxs-lookup"><span data-stu-id="0bba9-2273">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="0bba9-2274">Korrektur, bei der auf „scp“ zurückgegriffen wird, wenn Parimiko nicht funktioniert</span><span class="sxs-lookup"><span data-stu-id="0bba9-2274">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="0bba9-2275">`aks create` geändert, sodass `--aad-tenant-id` nicht mehr erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="0bba9-2275">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="0bba9-2276">Verbesserte Zusammenführung von Kubernetes-Anmeldeinformationen, wenn doppelte Einträge vorhanden sind</span><span class="sxs-lookup"><span data-stu-id="0bba9-2276">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="0bba9-2277">Container</span><span class="sxs-lookup"><span data-stu-id="0bba9-2277">Container</span></span>
* <span data-ttu-id="0bba9-2278">`functionapp create` geändert, sodass das Erstellen eines Linux-Nutzungsplans mit einer bestimmten Runtime unterstützt wird</span><span class="sxs-lookup"><span data-stu-id="0bba9-2278">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="0bba9-2279">[VORSCHAUVERSION] Unterstützung für das Hosten von Web-Apps in Windows-Containern hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2279">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="0bba9-2280">Event Hub</span><span class="sxs-lookup"><span data-stu-id="0bba9-2280">Event Hub</span></span>
* <span data-ttu-id="0bba9-2281">Befehl `eventhub update` korrigiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-2281">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="0bba9-2282">[BREAKING CHANGE]`list`-Befehle geändert, sodass Fehler von Typ „NotFound(404)“ für Ressourcen mit der typische Vorgehensweise behandelt werden, anstatt eine leere Liste anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="0bba9-2282">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="0bba9-2283">Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="0bba9-2283">Extensions</span></span>
* <span data-ttu-id="0bba9-2284">Problem beim Hinzufügen einer Erweiterung behoben, die bereits installiert ist</span><span class="sxs-lookup"><span data-stu-id="0bba9-2284">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="0bba9-2285">HDInsight</span><span class="sxs-lookup"><span data-stu-id="0bba9-2285">HDInsight</span></span>
* <span data-ttu-id="0bba9-2286">Erste Veröffentlichung</span><span class="sxs-lookup"><span data-stu-id="0bba9-2286">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="0bba9-2287">IoT</span><span class="sxs-lookup"><span data-stu-id="0bba9-2287">IoT</span></span>
* <span data-ttu-id="0bba9-2288">Befehl zur Erweiterungsinstallation zu Banner bei der ersten Ausführung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2288">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="0bba9-2289">KeyVault</span><span class="sxs-lookup"><span data-stu-id="0bba9-2289">KeyVault</span></span>
* <span data-ttu-id="0bba9-2290">Geändert, sodass Key Vault-Speicherbefehle auf das aktuelle API-Profil beschränkt sind</span><span class="sxs-lookup"><span data-stu-id="0bba9-2290">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="0bba9-2291">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0bba9-2291">Network</span></span>
* <span data-ttu-id="0bba9-2292">`network dns zone create` korrigiert: Befehl ist auch erfolgreich, wenn der Benutzer einen Standardspeicherort konfiguriert hat.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2292">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="0bba9-2293">Siehe Nr. 6052</span><span class="sxs-lookup"><span data-stu-id="0bba9-2293">See #6052</span></span>
* <span data-ttu-id="0bba9-2294">`--remote-vnet-id` für `network vnet peering create` eingestellt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2294">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="0bba9-2295">`--remote-vnet` zum `network vnet peering create`-Element hinzugefügt, das einen Namen oder eine ID akzeptiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-2295">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="0bba9-2296">Unterstützung für mehrere Subnetzpräfixe zu `network vnet create` in `--subnet-prefixes` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2296">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="0bba9-2297">Unterstützung für mehrere Subnetzpräfixe zu `network vnet subnet [create|update]` in `--address-prefixes` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2297">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="0bba9-2298">Problem mit `network application-gateway create` behoben, das die Erstellung von Gateways mit der SKU `WAF_v2` oder `Standard_v2` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="0bba9-2298">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="0bba9-2299">`--service-endpoint-policy`-Argument für Benutzerfreundlichkeit zu `network vnet subnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2299">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="0bba9-2300">Role</span><span class="sxs-lookup"><span data-stu-id="0bba9-2300">Role</span></span>
* <span data-ttu-id="0bba9-2301">Unterstützung für das Auflisten von Azure AD-App-Besitzern in `ad app owner` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2301">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="0bba9-2302">Unterstützung für das Auflisten von Azure AD-Dienstprinzipalbesitzern in `ad sp owner` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2302">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="0bba9-2303">Geändert, um sicherzustellen, dass die Erstellungs- und Aktualisierungsbefehle für die Rollendefinition Konfigurationen mit mehreren Berechtigungen akzeptieren</span><span class="sxs-lookup"><span data-stu-id="0bba9-2303">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="0bba9-2304">`ad sp create-for-rbac` geändert, um sicherzustellen, dass der Homepage-URI immer „https“ ist</span><span class="sxs-lookup"><span data-stu-id="0bba9-2304">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="0bba9-2305">Service Bus</span><span class="sxs-lookup"><span data-stu-id="0bba9-2305">Service Bus</span></span>
* <span data-ttu-id="0bba9-2306">[BREAKING CHANGE]`list`-Befehle geändert, sodass Fehler von Typ „NotFound(404)“ für Ressourcen mit der typische Vorgehensweise behandelt werden, anstatt eine leere Liste anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="0bba9-2306">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="0bba9-2307">VM</span><span class="sxs-lookup"><span data-stu-id="0bba9-2307">VM</span></span>
* <span data-ttu-id="0bba9-2308">Leeres `accessSas`-Feld in `disk grant-access` korrigiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-2308">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="0bba9-2309">`vmss create` geändert, sodass ein ausreichend großer Front-End-Portbereich zur Verarbeitung von Überbereitstellung reserviert ist</span><span class="sxs-lookup"><span data-stu-id="0bba9-2309">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="0bba9-2310">Aktualisierungsbefehle für `sig` korrigiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-2310">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="0bba9-2311">`--no-wait`-Unterstützung für die Verwaltung von Imageversionen in `sig` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2311">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="0bba9-2312">`vm list-ip-addresses` geändert, sodass die Verfügbarkeitszone von öffentlichen IP-Adressen angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="0bba9-2312">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="0bba9-2313">`[vm|vmss] disk attach` geändert, sodass die Standard-LUN eines Datenträgers standardmäßig auf die erste verfügbare Stelle festgelegt wird</span><span class="sxs-lookup"><span data-stu-id="0bba9-2313">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="0bba9-2314">21. September 2018</span><span class="sxs-lookup"><span data-stu-id="0bba9-2314">September 21, 2018</span></span>

<span data-ttu-id="0bba9-2315">Version 2.0.46</span><span class="sxs-lookup"><span data-stu-id="0bba9-2315">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="0bba9-2316">ACR</span><span class="sxs-lookup"><span data-stu-id="0bba9-2316">ACR</span></span>
* <span data-ttu-id="0bba9-2317">ACR-Aufgabenbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2317">Added ACR Task commands</span></span>
* <span data-ttu-id="0bba9-2318">Befehl für die Schnellausführung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2318">Added quick run command</span></span>
* <span data-ttu-id="0bba9-2319">`build-task`-Befehlsgruppe als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-2319">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="0bba9-2320">`helm`-Befehlsgruppe hinzugefügt, um die Verwaltung von Helm-Diagrammen mit ACR zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="0bba9-2320">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="0bba9-2321">Unterstützung für idempotentes Erstellen für die verwaltete Registrierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2321">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="0bba9-2322">Formatfreies Flag für die Anzeige von Buildprotokollen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2322">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="0bba9-2323">ACS</span><span class="sxs-lookup"><span data-stu-id="0bba9-2323">ACS</span></span>
* <span data-ttu-id="0bba9-2324">Befehl `install-connector` zum Festlegen des AKS-Master-FQDN geändert</span><span class="sxs-lookup"><span data-stu-id="0bba9-2324">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="0bba9-2325">Erstellen der Rollenzuweisung für „vnet-subnet-id“ (wenn kein Dienstprinzipal angegeben wurde) und „skip-role-assignment“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-2325">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="0bba9-2326">AppService</span><span class="sxs-lookup"><span data-stu-id="0bba9-2326">AppService</span></span>

* <span data-ttu-id="0bba9-2327">Unterstützung für WebJobs-Vorgangsverwaltung hinzugefügt (kontinuierlich/ausgelöst)</span><span class="sxs-lookup"><span data-stu-id="0bba9-2327">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="0bba9-2328">„az webapp config set“ unterstützt die Eigenschaft „--fts-state“; Unterstützung für „az functionapp config set/show“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2328">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="0bba9-2329">Unterstützung für Bring Your Own Storage für Web-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2329">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="0bba9-2330">Unterstützung für das Auflisten und Wiederherstellen gelöschter Web-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2330">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="0bba9-2331">Batch</span><span class="sxs-lookup"><span data-stu-id="0bba9-2331">Batch</span></span>
* <span data-ttu-id="0bba9-2332">Hinzufügen von Aufgaben über `--json-file` geändert, um die AddTaskCollectionParameter-Syntax zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="0bba9-2332">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="0bba9-2333">Dokumentation akzeptierter `--json-file`-Formate aktualisiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-2333">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="0bba9-2334">`--max-tasks-per-node-option` zu `batch pool create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2334">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="0bba9-2335">Verhalten von `batch account` geändert, um das aktuell angemeldete Konto anzuzeigen, wenn keine Optionen angegeben wurden</span><span class="sxs-lookup"><span data-stu-id="0bba9-2335">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="0bba9-2336">Batch KI</span><span class="sxs-lookup"><span data-stu-id="0bba9-2336">Batch AI</span></span> 
* <span data-ttu-id="0bba9-2337">Fehler bei der automatischen Speicherkontoerstellung im Befehl `batchai cluster create` behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-2337">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="0bba9-2338">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="0bba9-2338">Cognitive Services</span></span>
* <span data-ttu-id="0bba9-2339">Vervollständigung für die Argumente `--sku`, `--kind` und `--location` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2339">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="0bba9-2340">Befehl `cognitiveservices account list-usage` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2340">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="0bba9-2341">Befehl `cognitiveservices account list-kinds` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2341">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="0bba9-2342">Befehl `cognitiveservices account list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2342">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="0bba9-2343">`cognitiveservices list` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-2343">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="0bba9-2344">`--name` geändert (ist jetzt optional für `cognitiveservices account list-skus`)</span><span class="sxs-lookup"><span data-stu-id="0bba9-2344">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="0bba9-2345">Container</span><span class="sxs-lookup"><span data-stu-id="0bba9-2345">Container</span></span>
* <span data-ttu-id="0bba9-2346">Möglichkeit zum Neustarten und Beenden einer ausgeführten Containergruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2346">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="0bba9-2347">`--network-profile` zum Übergeben eines Netzwerkprofils hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2347">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="0bba9-2348">`--subnet` und `--vnet_name` hinzugefügt, um das Erstellen von Containergruppen in einem VNET zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="0bba9-2348">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="0bba9-2349">Tabellenausgabe geändert, sodass der Status der Containergruppe angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="0bba9-2349">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="0bba9-2350">Data Lake</span><span class="sxs-lookup"><span data-stu-id="0bba9-2350">Datalake</span></span>
* <span data-ttu-id="0bba9-2351">Befehle für VNET-Regeln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2351">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="0bba9-2352">Interaktive Shell</span><span class="sxs-lookup"><span data-stu-id="0bba9-2352">Interactive Shell</span></span>
* <span data-ttu-id="0bba9-2353">Fehler in Windows behoben, durch den Befehle nicht ordnungsgemäß ausgeführt wurden</span><span class="sxs-lookup"><span data-stu-id="0bba9-2353">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="0bba9-2354">Durch veraltete Objekte verursachtes Problem beim Laden von Befehlen im interaktiven Modus behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-2354">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="0bba9-2355">IoT</span><span class="sxs-lookup"><span data-stu-id="0bba9-2355">IoT</span></span>
* <span data-ttu-id="0bba9-2356">Routingunterstützung für IoT Hubs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2356">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="0bba9-2357">Key Vault</span><span class="sxs-lookup"><span data-stu-id="0bba9-2357">Key Vault</span></span>
* <span data-ttu-id="0bba9-2358">Key Vault-Schlüsselimport für RSA-Schlüssel korrigiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-2358">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="0bba9-2359">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0bba9-2359">Network</span></span>
* <span data-ttu-id="0bba9-2360">Befehle vom Typ `network public-ip prefix` hinzugefügt, um Präfixe von öffentlichen IP-Adressen zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="0bba9-2360">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="0bba9-2361">Befehle vom Typ `network service-endpoint` hinzugefügt, um Dienstendpunktrichtlinien-Features zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="0bba9-2361">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="0bba9-2362">Befehle vom Typ `network lb outbound-rule` hinzugefügt, um die Erstellung von Ausgangsregeln für Load Balancer Standard zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="0bba9-2362">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="0bba9-2363">`--public-ip-prefix` zu `network lb frontend-ip create/update` hinzugefügt, um Front-End-IP-Konfigurationen mit Präfixen von öffentlichen IP-Adressen zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="0bba9-2363">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="0bba9-2364">`--enable-tcp-reset` zu `network lb rule/inbound-nat-rule/inbound-nat-pool create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2364">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="0bba9-2365">`--disable-outbound-snat` zu `network lb rule create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2365">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="0bba9-2366">Verwendung von `network watcher flow-log show/configure` mit klassischen NSGs ermöglicht</span><span class="sxs-lookup"><span data-stu-id="0bba9-2366">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="0bba9-2367">Hinzufügen des `network watcher run-configuration-diagnostic`-Befehls</span><span class="sxs-lookup"><span data-stu-id="0bba9-2367">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="0bba9-2368">Befehl `network watcher test-connectivity` korrigiert und Eigenschaften `--method`, `--valid-status-codes` und `--headers` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2368">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="0bba9-2369">`network express-route create/update`: Flag `--allow-global-reach` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2369">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="0bba9-2370">`network vnet subnet create/update`: Unterstützung für `--delegation` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2370">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="0bba9-2371">Befehl `network vnet subnet list-available-delegations` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2371">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="0bba9-2372">`network traffic-manager profile create/update`: Unterstützung für `--interval`, `--timeout` und `--max-failures` für die Überwachungskonfiguration hinzugefügt; Optionen `--monitor-path`, `--monitor-port` und `--monitor-protocol` zugunsten von `--path`, `--port` und `--protocol` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-2372">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="0bba9-2373">`network lb frontend-ip create/update`: Logik für das Festlegen der Zuweisungsmethode für private IP-Adressen korrigiert. Bei Angabe einer privaten IP-Adresse ist die Zuweisung statisch. Wird keine private IP-Adresse (oder eine leere Zeichenfolge für die private IP-Adresse) angegeben, erfolgt eine dynamische Zuweisung.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2373">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="0bba9-2374">`dns record-set * create/update`: Unterstützung für `--target-resource` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2374">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="0bba9-2375">Befehle vom Typ `network interface-endpoint` hinzugefügt, um Schnittstellenendpunkt-Objekte abzufragen</span><span class="sxs-lookup"><span data-stu-id="0bba9-2375">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="0bba9-2376">`network profile show/list/delete` für die partielle Verwaltung von Netzwerkprofilen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2376">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="0bba9-2377">Befehle vom Typ `network express-route peering connection` für die Verwaltung von Peeringverbindungen zwischen ExpressRoute-Instanzen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2377">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="0bba9-2378">RDBMS</span><span class="sxs-lookup"><span data-stu-id="0bba9-2378">RDBMS</span></span>
* <span data-ttu-id="0bba9-2379">Unterstützung für den MariaDB-Dienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2379">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="0bba9-2380">Reservierung</span><span class="sxs-lookup"><span data-stu-id="0bba9-2380">Reservation</span></span>
* <span data-ttu-id="0bba9-2381">Cosmos DB im Enumerationstyp für reservierte Ressourcen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2381">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="0bba9-2382">Namenseigenschaft im Patchmodell hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2382">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="0bba9-2383">App-Verwaltung</span><span class="sxs-lookup"><span data-stu-id="0bba9-2383">Manage App</span></span>
* <span data-ttu-id="0bba9-2384">Fehler in `managedapp create --kind MarketPlace` korrigiert, der zum Absturz der Instanzerstellung einer verwalteten Marketplace-App führte</span><span class="sxs-lookup"><span data-stu-id="0bba9-2384">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="0bba9-2385">Befehle vom Typ `feature` geändert, um sie auf unterstützte Profile zu beschränken</span><span class="sxs-lookup"><span data-stu-id="0bba9-2385">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="0bba9-2386">Role</span><span class="sxs-lookup"><span data-stu-id="0bba9-2386">Role</span></span>
* <span data-ttu-id="0bba9-2387">Unterstützung für das Auflisten der Gruppenmitgliedschaften des Benutzers hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2387">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="0bba9-2388">SignalR</span><span class="sxs-lookup"><span data-stu-id="0bba9-2388">SignalR</span></span>
* <span data-ttu-id="0bba9-2389">Erste Version</span><span class="sxs-lookup"><span data-stu-id="0bba9-2389">First release</span></span>

### <a name="storage"></a><span data-ttu-id="0bba9-2390">Storage</span><span class="sxs-lookup"><span data-stu-id="0bba9-2390">Storage</span></span>
* <span data-ttu-id="0bba9-2391">Parameter `--auth-mode login` für die Verwendung der Anmeldeinformationen des Benutzers für die Blob- und Warteschlangenautorisierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2391">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="0bba9-2392">`storage container immutability-policy/legal-hold` für die Verwaltung von unveränderlichem Speicher hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2392">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="0bba9-2393">VM</span><span class="sxs-lookup"><span data-stu-id="0bba9-2393">VM</span></span>
* <span data-ttu-id="0bba9-2394">Problem behoben, das dazu führte, dass die Datei mit dem privaten Schlüssel durch `vm create --generate-ssh-keys` überschrieben wird, wenn die Datei mit dem privaten Schlüssel fehlt (Nr. 4725, 6780)</span><span class="sxs-lookup"><span data-stu-id="0bba9-2394">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="0bba9-2395">Unterstützung für den gemeinsamen Image-Katalog über `az sig` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2395">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="0bba9-2396">28. August 2018</span><span class="sxs-lookup"><span data-stu-id="0bba9-2396">August 28, 2018</span></span>

<span data-ttu-id="0bba9-2397">Version 2.0.45</span><span class="sxs-lookup"><span data-stu-id="0bba9-2397">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="0bba9-2398">Core</span><span class="sxs-lookup"><span data-stu-id="0bba9-2398">Core</span></span>

* <span data-ttu-id="0bba9-2399">Das Problem, aufgrund dessen eine leere Konfigurationsdatei geladen wurde, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2399">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="0bba9-2400">Unterstützung für Profil `2018-03-01-hybrid` für Azure Stack hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2400">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="0bba9-2401">ACR</span><span class="sxs-lookup"><span data-stu-id="0bba9-2401">ACR</span></span>

* <span data-ttu-id="0bba9-2402">Problemumgehung für Laufzeitvorgänge ohne ARM-Anforderungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2402">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="0bba9-2403">Änderung vorgenommen, um im Befehl `build` Versionskontrolldateien (etwa „.git“ und „.gitignore“) standardmäßig aus der TAR-Datei auszuschließen</span><span class="sxs-lookup"><span data-stu-id="0bba9-2403">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="0bba9-2404">ACS</span><span class="sxs-lookup"><span data-stu-id="0bba9-2404">ACS</span></span>

* <span data-ttu-id="0bba9-2405">`aks create` geändert, dass standardmäßig virtuelle Computer vom Typ `Standard_DS2_v2` erstellt werden</span><span class="sxs-lookup"><span data-stu-id="0bba9-2405">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="0bba9-2406">`aks get-credentials` geändert, um nun neue APIs zum Abrufen der Clusteranmeldeinformationen aufzurufen</span><span class="sxs-lookup"><span data-stu-id="0bba9-2406">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="0bba9-2407">AppService</span><span class="sxs-lookup"><span data-stu-id="0bba9-2407">AppService</span></span>

* <span data-ttu-id="0bba9-2408">Unterstützung für CORS in „functionapp“ und „webapp“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2408">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="0bba9-2409">ARM-Tagunterstützung in Erstellungsbefehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2409">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="0bba9-2410">`[webapp|functionapp] identity show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="0bba9-2410">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="0bba9-2411">Backup</span><span class="sxs-lookup"><span data-stu-id="0bba9-2411">Backup</span></span>

* <span data-ttu-id="0bba9-2412">`backup vault backup-properties show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="0bba9-2412">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="0bba9-2413">Botdienst</span><span class="sxs-lookup"><span data-stu-id="0bba9-2413">Bot Service</span></span>

* <span data-ttu-id="0bba9-2414">Anfängliches Release der Botdienst-CLI</span><span class="sxs-lookup"><span data-stu-id="0bba9-2414">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="0bba9-2415">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="0bba9-2415">Cognitive Services</span></span>

* <span data-ttu-id="0bba9-2416">Neuer Parameter `--api-properties,` hinzugefügt, der zum Erstellen einiger Dienste erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="0bba9-2416">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="0bba9-2417">IoT</span><span class="sxs-lookup"><span data-stu-id="0bba9-2417">IoT</span></span>

* <span data-ttu-id="0bba9-2418">Problem mit dem Zuweisen verknüpfter Hubs behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-2418">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="0bba9-2419">Überwachen</span><span class="sxs-lookup"><span data-stu-id="0bba9-2419">Monitor</span></span>

* <span data-ttu-id="0bba9-2420">`monitor metrics alert`-Befehle für Metrikwarnungen nahezu in Echtzeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2420">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="0bba9-2421">`monitor alert`-Befehle als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-2421">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="0bba9-2422">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0bba9-2422">Network</span></span>

* <span data-ttu-id="0bba9-2423">`network application-gateway ssl-policy predefined show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="0bba9-2423">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="0bba9-2424">Resource</span><span class="sxs-lookup"><span data-stu-id="0bba9-2424">Resource</span></span>

* <span data-ttu-id="0bba9-2425">`provider operation show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="0bba9-2425">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="0bba9-2426">Storage</span><span class="sxs-lookup"><span data-stu-id="0bba9-2426">Storage</span></span>

* <span data-ttu-id="0bba9-2427">`storage share policy show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="0bba9-2427">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="0bba9-2428">VM</span><span class="sxs-lookup"><span data-stu-id="0bba9-2428">VM</span></span>

* <span data-ttu-id="0bba9-2429">`vm/vmss identity show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="0bba9-2429">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="0bba9-2430">`--storage-caching` für `vm create` eingestellt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2430">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="0bba9-2431">14. August 2018</span><span class="sxs-lookup"><span data-stu-id="0bba9-2431">Auguest 14, 2018</span></span>

<span data-ttu-id="0bba9-2432">Version 2.0.44</span><span class="sxs-lookup"><span data-stu-id="0bba9-2432">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="0bba9-2433">Core</span><span class="sxs-lookup"><span data-stu-id="0bba9-2433">Core</span></span>

* <span data-ttu-id="0bba9-2434">Numerische Anzeige in `table`-Ausgabe korrigiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-2434">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="0bba9-2435">YAML-Ausgabeformat hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2435">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="0bba9-2436">Telemetrie</span><span class="sxs-lookup"><span data-stu-id="0bba9-2436">Telemetry</span></span>

* <span data-ttu-id="0bba9-2437">Verbesserte Berichterstellung für Telemetriedaten</span><span class="sxs-lookup"><span data-stu-id="0bba9-2437">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="0bba9-2438">ACR</span><span class="sxs-lookup"><span data-stu-id="0bba9-2438">ACR</span></span>

* <span data-ttu-id="0bba9-2439">Befehle vom Typ `content-trust policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2439">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="0bba9-2440">Problem behoben, aufgrund dessen `.dockerignore` nicht richtig verarbeitet wurde</span><span class="sxs-lookup"><span data-stu-id="0bba9-2440">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="0bba9-2441">ACS</span><span class="sxs-lookup"><span data-stu-id="0bba9-2441">ACS</span></span>

* <span data-ttu-id="0bba9-2442">`az acs/aks install-cli` für die Installation in `%USERPROFILE%\.azure-kubectl` unter Windows geändert</span><span class="sxs-lookup"><span data-stu-id="0bba9-2442">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="0bba9-2443">`az aks install-connector` geändert, um zu ermitteln, ob der Cluster über RBAC verfügt, und um den ACI-Connector entsprechend zu konfigurieren</span><span class="sxs-lookup"><span data-stu-id="0bba9-2443">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="0bba9-2444">Geändert in Rollenzuweisung zum Subnetz bei entsprechender Angabe</span><span class="sxs-lookup"><span data-stu-id="0bba9-2444">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="0bba9-2445">Neue Option zum Überspringen der Rollenzuweisung für Subnetz hinzugefügt, wenn dieses angegeben ist</span><span class="sxs-lookup"><span data-stu-id="0bba9-2445">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="0bba9-2446">Geändert, um Rollenzuweisung zum Subnetz zu überspringen, wenn bereits eine Zuweisung vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="0bba9-2446">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="0bba9-2447">AppService</span><span class="sxs-lookup"><span data-stu-id="0bba9-2447">AppService</span></span>

* <span data-ttu-id="0bba9-2448">Fehler behoben, der das Erstellen einer Funktions-App mithilfe von Speicherkonten in externen Ressourcengruppen verhinderte</span><span class="sxs-lookup"><span data-stu-id="0bba9-2448">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="0bba9-2449">Absturz bei ZIP-Bereitstellung behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-2449">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="0bba9-2450">Batch AI</span><span class="sxs-lookup"><span data-stu-id="0bba9-2450">BatchAI</span></span>

* <span data-ttu-id="0bba9-2451">Protokollierungsausgabe für die automatische Speicherkontoerstellung geändert, sodass nun „Ressourcen*gruppe*“ angegeben wird</span><span class="sxs-lookup"><span data-stu-id="0bba9-2451">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="0bba9-2452">Container</span><span class="sxs-lookup"><span data-stu-id="0bba9-2452">Container</span></span>

* <span data-ttu-id="0bba9-2453">`--secure-environment-variables` zum Übergeben sicherer Umgebungsvariablen an einen Container hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2453">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="0bba9-2454">IoT</span><span class="sxs-lookup"><span data-stu-id="0bba9-2454">IoT</span></span>

* <span data-ttu-id="0bba9-2455">[BREAKING CHANGE] Veraltete Befehle entfernt, die in die IoT-Erweiterung verschoben wurden</span><span class="sxs-lookup"><span data-stu-id="0bba9-2455">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="0bba9-2456">Elemente aktualisiert, um nicht die Domäne `azure-devices.net` anzunehmen</span><span class="sxs-lookup"><span data-stu-id="0bba9-2456">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="0bba9-2457">Iot Central</span><span class="sxs-lookup"><span data-stu-id="0bba9-2457">Iot Central</span></span>

* <span data-ttu-id="0bba9-2458">Erstes Release des IoT Central-Moduls</span><span class="sxs-lookup"><span data-stu-id="0bba9-2458">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="0bba9-2459">KeyVault</span><span class="sxs-lookup"><span data-stu-id="0bba9-2459">KeyVault</span></span>


* <span data-ttu-id="0bba9-2460">Befehle zum Verwalten von Speicherkonten und SAS-Definitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2460">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="0bba9-2461">Befehle für Netzwerkregeln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2461">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="0bba9-2462">Parameter `--id` zu Geheimnis-, Schlüssel- und Zertifikatvorgängen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2462">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="0bba9-2463">Unterstützung für Version mit mehreren APIs zur Schlüsseltresorverwaltung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2463">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="0bba9-2464">Unterstützung für Version mit mehreren APIs zur Schlüsseltresordatenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2464">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="0bba9-2465">Relay</span><span class="sxs-lookup"><span data-stu-id="0bba9-2465">Relay</span></span>

* <span data-ttu-id="0bba9-2466">Erste Veröffentlichung</span><span class="sxs-lookup"><span data-stu-id="0bba9-2466">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="0bba9-2467">Sql</span><span class="sxs-lookup"><span data-stu-id="0bba9-2467">Sql</span></span>

* <span data-ttu-id="0bba9-2468">Befehle vom Typ `sql failover-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2468">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="0bba9-2469">Storage</span><span class="sxs-lookup"><span data-stu-id="0bba9-2469">Storage</span></span>

* <span data-ttu-id="0bba9-2470">[BREAKING CHANGE]`storage account show-usage` geändert, um Parameter `--location` erforderlich zu machen. Auflistung nach Region</span><span class="sxs-lookup"><span data-stu-id="0bba9-2470">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="0bba9-2471">Parameter `--resource-group` geändert, sodass er für `storage account`-Befehle optional ist</span><span class="sxs-lookup"><span data-stu-id="0bba9-2471">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="0bba9-2472">Warnungen vom Typ „Fehler bei Vorbedingung“ für einzelne Fehler in Batch-Befehlen für eine aggregiert Nachricht entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2472">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="0bba9-2473">`[blob|file] delete-batch`-Befehle geändert, sodass kein Array mit Null-Werten mehr ausgegeben wird</span><span class="sxs-lookup"><span data-stu-id="0bba9-2473">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="0bba9-2474">`blob [download|upload|delete-batch]`-Befehle geändert, um SAS-Token aus Container-URL zu lesen</span><span class="sxs-lookup"><span data-stu-id="0bba9-2474">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="0bba9-2475">VM</span><span class="sxs-lookup"><span data-stu-id="0bba9-2475">VM</span></span>

* <span data-ttu-id="0bba9-2476">Allgemeine Filter zu `vm list-skus` für höhere Benutzerfreundlichkeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2476">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="0bba9-2477">31. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="0bba9-2477">July 31, 2018</span></span>

<span data-ttu-id="0bba9-2478">Version 2.0.43</span><span class="sxs-lookup"><span data-stu-id="0bba9-2478">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="0bba9-2479">ACR</span><span class="sxs-lookup"><span data-stu-id="0bba9-2479">ACR</span></span>

* <span data-ttu-id="0bba9-2480">Flag `--with-secure-properties` zum Befehl `acr build-task show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2480">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="0bba9-2481">Befehl `acr build-task update-build` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2481">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="0bba9-2482">ACS</span><span class="sxs-lookup"><span data-stu-id="0bba9-2482">ACS</span></span>

* <span data-ttu-id="0bba9-2483">Änderung, um 0 (Erfolg) zurückzugeben, wenn `az aks browse` durch Drücken von [STRG+C] beendet wird</span><span class="sxs-lookup"><span data-stu-id="0bba9-2483">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="0bba9-2484">Batch</span><span class="sxs-lookup"><span data-stu-id="0bba9-2484">Batch</span></span>

* <span data-ttu-id="0bba9-2485">Korrektur eines Fehlers bei der Anzeige des AAD-Tokens in Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="0bba9-2485">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="0bba9-2486">Container</span><span class="sxs-lookup"><span data-stu-id="0bba9-2486">Container</span></span>

* <span data-ttu-id="0bba9-2487">Voraussetzung von `--log-analytics-workspace-key` für Name oder ID im festgelegten Abonnement entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2487">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="0bba9-2488">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0bba9-2488">Network</span></span>

* <span data-ttu-id="0bba9-2489">DNS-Unterstützung zu „2017-03-09-profile“ für Azure Stack hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2489">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="0bba9-2490">Resource</span><span class="sxs-lookup"><span data-stu-id="0bba9-2490">Resource</span></span>

* <span data-ttu-id="0bba9-2491">`--rollback-on-error` zu `group deployment create` hinzugefügt, um bei einem Fehler eine als funktionierend bekannte Bereitstellung auszuführen</span><span class="sxs-lookup"><span data-stu-id="0bba9-2491">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="0bba9-2492">Problem behoben, aufgrund dessen `--parameters {}` mit `group deployment create` zu einem Fehler führte</span><span class="sxs-lookup"><span data-stu-id="0bba9-2492">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="0bba9-2493">Role</span><span class="sxs-lookup"><span data-stu-id="0bba9-2493">Role</span></span>

* <span data-ttu-id="0bba9-2494">Unterstützung für das Stack-Profil „2017-03-09-profile“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2494">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="0bba9-2495">Problem behoben, aufgrund dessen das generische Update von Parametern auf `app update` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="0bba9-2495">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="0bba9-2496">Suchen,</span><span class="sxs-lookup"><span data-stu-id="0bba9-2496">Search</span></span>

* <span data-ttu-id="0bba9-2497">Befehle für Azure Search-Dienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2497">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="0bba9-2498">Service Bus</span><span class="sxs-lookup"><span data-stu-id="0bba9-2498">Service Bus</span></span>

* <span data-ttu-id="0bba9-2499">Migrationsbefehlsgruppe hinzugefügt, um einen Namespace von Service Bus Standard zu Premium zu migrieren</span><span class="sxs-lookup"><span data-stu-id="0bba9-2499">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="0bba9-2500">Neue optionale Eigenschaften zu Service Bus-Warteschlange und -Abonnement hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2500">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="0bba9-2501">`--enable-batched-operations` und `--enable-dead-lettering-on-message-expiration` in `queue`</span><span class="sxs-lookup"><span data-stu-id="0bba9-2501">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="0bba9-2502">`--dead-letter-on-filter-exceptions` in `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="0bba9-2502">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="0bba9-2503">Storage</span><span class="sxs-lookup"><span data-stu-id="0bba9-2503">Storage</span></span>

* <span data-ttu-id="0bba9-2504">Unterstützung für den Download großer Dateien über eine einzelne Verbindung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2504">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="0bba9-2505">`show`-Befehle konvertiert, bei denen im Falle einer fehlenden Ressource kein Fehler mit dem Exitcode 3 ausgelöst wurde</span><span class="sxs-lookup"><span data-stu-id="0bba9-2505">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="0bba9-2506">VM</span><span class="sxs-lookup"><span data-stu-id="0bba9-2506">VM</span></span>

* <span data-ttu-id="0bba9-2507">Unterstützung zum Auflisten von Verfügbarkeitsgruppen nach Abonnement hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2507">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="0bba9-2508">Unterstützung für `StandardSSD_LRS` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2508">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="0bba9-2509">Unterstützung für Anwendungssicherheitsgruppe beim Erstellen einer VM-Skalierungsgruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2509">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="0bba9-2510">[BREAKING CHANGE]`[vm|vmss] create`, `[vm|vmss] identity assign` und `[vm|vmss] identity remove` wurden geändert, um vom Benutzer zugewiesene Identitäten im Wörterbuchformat auszugeben.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2510">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="0bba9-2511">18. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="0bba9-2511">July 18, 2018</span></span>

<span data-ttu-id="0bba9-2512">Version 2.0.42</span><span class="sxs-lookup"><span data-stu-id="0bba9-2512">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="0bba9-2513">Core</span><span class="sxs-lookup"><span data-stu-id="0bba9-2513">Core</span></span>

* <span data-ttu-id="0bba9-2514">Unterstützung für browserbasierte Anmeldung WSL-Bash-Fenster hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2514">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="0bba9-2515">`--force-string`-Flag für alle generischen Updatebefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2515">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="0bba9-2516">[BREAKING CHANGE] Befehle vom Typ „show“ so geändert, dass die Fehlermeldung protokolliert wird und der Vorgang bei einer fehlenden Ressource mit dem Exitcode 3 fehlschlägt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2516">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="0bba9-2517">ACR</span><span class="sxs-lookup"><span data-stu-id="0bba9-2517">ACR</span></span>

* <span data-ttu-id="0bba9-2518">[BREAKING CHANGE] „--no-push“ in Befehl „acr build“ in reines Flag geändert</span><span class="sxs-lookup"><span data-stu-id="0bba9-2518">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="0bba9-2519">Befehle `show` und `update` unter Gruppe `acr repository` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2519">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="0bba9-2520">`--detail`-Flag für `show-manifests` und `show-tags` hinzugefügt, um ausführlichere Informationen anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="0bba9-2520">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="0bba9-2521">Parameter `--image` zur Unterstützung des Abrufs von Builddetails oder Protokollen anhand eines Images hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2521">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="0bba9-2522">ACS</span><span class="sxs-lookup"><span data-stu-id="0bba9-2522">ACS</span></span>

* <span data-ttu-id="0bba9-2523">`az aks create` so geändert, dass mit Fehler beendet wird, wenn `--max-pods` kleiner als 5 ist</span><span class="sxs-lookup"><span data-stu-id="0bba9-2523">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="0bba9-2524">AppService</span><span class="sxs-lookup"><span data-stu-id="0bba9-2524">AppService</span></span>

* <span data-ttu-id="0bba9-2525">Unterstützung für PremiumV2-SKUs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2525">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="0bba9-2526">Batch</span><span class="sxs-lookup"><span data-stu-id="0bba9-2526">Batch</span></span>

* <span data-ttu-id="0bba9-2527">Korrektur eines Fehlers bei der Verwendung von Anmeldeinformationen im Cloud Shell-Modus</span><span class="sxs-lookup"><span data-stu-id="0bba9-2527">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="0bba9-2528">JSON-Eingabe so geändert, dass Groß-/Kleinschreibung nicht beachtet wird</span><span class="sxs-lookup"><span data-stu-id="0bba9-2528">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="0bba9-2529">Batch KI</span><span class="sxs-lookup"><span data-stu-id="0bba9-2529">Batch AI</span></span>

* <span data-ttu-id="0bba9-2530">Befehl `az batchai job exec` korrigiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-2530">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="0bba9-2531">Container</span><span class="sxs-lookup"><span data-stu-id="0bba9-2531">Container</span></span>

* <span data-ttu-id="0bba9-2532">Anforderung von Benutzername und Kennwort für Nicht-DockerHub-Registrierungen entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2532">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="0bba9-2533">Fehler beim Erstellen von Containergruppen aus YAML-Datei behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-2533">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="0bba9-2534">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0bba9-2534">Network</span></span>

* <span data-ttu-id="0bba9-2535">Unterstützung für `--no-wait` zu `network nic [create|update|delete]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2535">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="0bba9-2536">`network nic wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2536">Added `network nic wait`</span></span>
* <span data-ttu-id="0bba9-2537">`--ids`-Argument für `network vnet [subnet|peering] list` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-2537">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="0bba9-2538">`--include-default`-Flag hinzugefügt, um Standardsicherheitsregeln in die Ausgabe von `network nsg rule list` aufzunehmen</span><span class="sxs-lookup"><span data-stu-id="0bba9-2538">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="0bba9-2539">Resource</span><span class="sxs-lookup"><span data-stu-id="0bba9-2539">Resource</span></span>

* <span data-ttu-id="0bba9-2540">Unterstützung für `--no-wait` zu `group deployment delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2540">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="0bba9-2541">Unterstützung für `--no-wait` zu `deployment delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2541">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="0bba9-2542">Befehl `deployment wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2542">Added `deployment wait` command</span></span>
* <span data-ttu-id="0bba9-2543">Problem behoben, aufgrund dessen die `az deployment`-Befehle auf Abonnementebene fälschlicherweise für Profil „2017-03-09-profile“ angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="0bba9-2543">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="0bba9-2544">SQL</span><span class="sxs-lookup"><span data-stu-id="0bba9-2544">SQL</span></span>

* <span data-ttu-id="0bba9-2545">Fehler „Der angegebene Ressourcengruppenname ... entsprach nicht dem Namen in der URL“ beim Angeben des Namens des Pools für elastische Datenbanken für `sql db copy`-und `sql db replica create`-Befehle behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-2545">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="0bba9-2546">Konfigurieren des Standard-SQL Servers durch Ausführen von `az configure --defaults sql-server=<name>` zulässig</span><span class="sxs-lookup"><span data-stu-id="0bba9-2546">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="0bba9-2547">Tabellenformatierer für Befehle `sql server`, `sql server firewall-rule`, `sql list-usages` und `sql show-usage` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2547">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="0bba9-2548">Storage</span><span class="sxs-lookup"><span data-stu-id="0bba9-2548">Storage</span></span>

* <span data-ttu-id="0bba9-2549">`pageRanges`-Eigenschaft zu `storage blob show`-Ausgabe hinzugefügt, die für Seitenblobs ausgefüllt wird</span><span class="sxs-lookup"><span data-stu-id="0bba9-2549">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="0bba9-2550">VM</span><span class="sxs-lookup"><span data-stu-id="0bba9-2550">VM</span></span>

* <span data-ttu-id="0bba9-2551">[BREAKING CHANGE]`vmss create` so geändert, dass `Standard_DS1_v2` als standardmäßige Instanzgröße verwendet wird</span><span class="sxs-lookup"><span data-stu-id="0bba9-2551">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="0bba9-2552">Unterstützung für `--no-wait` zu `vm extension [set|delete]` und `vmss extension [set|delete]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2552">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="0bba9-2553">`vm extension wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2553">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="0bba9-2554">3\. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="0bba9-2554">July 3, 2018</span></span>

<span data-ttu-id="0bba9-2555">Version 2.0.41</span><span class="sxs-lookup"><span data-stu-id="0bba9-2555">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="0bba9-2556">AKS</span><span class="sxs-lookup"><span data-stu-id="0bba9-2556">AKS</span></span>

* <span data-ttu-id="0bba9-2557">Überwachung geändert, sodass Abonnement-ID verwendet wird</span><span class="sxs-lookup"><span data-stu-id="0bba9-2557">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="0bba9-2558">3\. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="0bba9-2558">July 3, 2018</span></span>

<span data-ttu-id="0bba9-2559">Version 2.0.40</span><span class="sxs-lookup"><span data-stu-id="0bba9-2559">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="0bba9-2560">Core</span><span class="sxs-lookup"><span data-stu-id="0bba9-2560">Core</span></span>

* <span data-ttu-id="0bba9-2561">Neuer Autorisierungscode-Flow für interaktive Anmeldung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2561">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="0bba9-2562">ACR</span><span class="sxs-lookup"><span data-stu-id="0bba9-2562">ACR</span></span>

* <span data-ttu-id="0bba9-2563">Abruf-Buildstatus hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2563">Added polling build status</span></span>
* <span data-ttu-id="0bba9-2564">Unterstützung für Enumerationswerte ohne Berücksichtigung von Groß-/Kleinschreibung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2564">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="0bba9-2565">Parameter `--top` und `--orderby` für `show-manifests` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2565">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="0bba9-2566">ACS</span><span class="sxs-lookup"><span data-stu-id="0bba9-2566">ACS</span></span>

* <span data-ttu-id="0bba9-2567">[BREAKING CHANGE] Standardmäßiges Aktivieren der rollenbasierten Zugriffssteuerung für Kubernetes</span><span class="sxs-lookup"><span data-stu-id="0bba9-2567">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="0bba9-2568">Argument `--disable-rbac` hinzugefügt und `--enable-rbac` als veraltet festgelegt, da es nun der Standard ist</span><span class="sxs-lookup"><span data-stu-id="0bba9-2568">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="0bba9-2569">Optionen für Befehl `aks browse` wurden aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2569">Updated options for `aks browse` command.</span></span> <span data-ttu-id="0bba9-2570">Unterstützung für `--listen-port` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2570">Added `--listen-port` support</span></span>
* <span data-ttu-id="0bba9-2571">Standardmäßiges Helm-Diagrammpaket für Befehl `aks install-connector` wurde aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2571">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="0bba9-2572">Verwenden von „virtual-kubelet-for-aks-latest.tgz“</span><span class="sxs-lookup"><span data-stu-id="0bba9-2572">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="0bba9-2573">Befehle `aks enable-addons` und `aks disable-addons` zum Aktualisieren eines vorhandenen Clusters hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2573">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="0bba9-2574">AppService</span><span class="sxs-lookup"><span data-stu-id="0bba9-2574">AppService</span></span>

* <span data-ttu-id="0bba9-2575">Unterstützung für das Deaktivieren der Identität über `webapp identity remove` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2575">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="0bba9-2576">`preview`-Tag für Identitätsfunktion entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2576">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="0bba9-2577">Backup</span><span class="sxs-lookup"><span data-stu-id="0bba9-2577">Backup</span></span>

* <span data-ttu-id="0bba9-2578">Moduldefinition aktualisiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-2578">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="0bba9-2579">Batch AI</span><span class="sxs-lookup"><span data-stu-id="0bba9-2579">BatchAI</span></span>

* <span data-ttu-id="0bba9-2580">Tabellenausgabe für Befehle `batchai cluster node list` und `batchai job node list` korrigiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-2580">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="0bba9-2581">Cloud</span><span class="sxs-lookup"><span data-stu-id="0bba9-2581">Cloud</span></span>

* <span data-ttu-id="0bba9-2582">Serversuffix `acr login` zu Cloudkonfiguration hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2582">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="0bba9-2583">Container</span><span class="sxs-lookup"><span data-stu-id="0bba9-2583">Container</span></span>

* <span data-ttu-id="0bba9-2584">`container create` zu Standard für Vorgang mit langer Ausführungsdauer geändert</span><span class="sxs-lookup"><span data-stu-id="0bba9-2584">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="0bba9-2585">Log Analytics-Parameter `--log-analytics-workspace` und `--log-analytics-workspace-key` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2585">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="0bba9-2586">Parameter `--protocol` zum Festlegen des zu verwendenden Netzwerkprotokolls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2586">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="0bba9-2587">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="0bba9-2587">Extension</span></span>

* <span data-ttu-id="0bba9-2588">`extension list-available` geändert, sodass nur mit der CLI-Version kompatible Erweiterungen angezeigt werden</span><span class="sxs-lookup"><span data-stu-id="0bba9-2588">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="0bba9-2589">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0bba9-2589">Network</span></span>

* <span data-ttu-id="0bba9-2590">Problem behoben, aufgrund dessen bei Datensatztypen die Groß-/Kleinschreibung beachtet werden musste ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="0bba9-2590">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="0bba9-2591">Rdbms</span><span class="sxs-lookup"><span data-stu-id="0bba9-2591">Rdbms</span></span>

* <span data-ttu-id="0bba9-2592">Befehle vom Typ `[postgres|myql] server vnet-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2592">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="0bba9-2593">Resource</span><span class="sxs-lookup"><span data-stu-id="0bba9-2593">Resource</span></span>

* <span data-ttu-id="0bba9-2594">Neue Vorgangsgruppe `deployment` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2594">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="0bba9-2595">VM</span><span class="sxs-lookup"><span data-stu-id="0bba9-2595">VM</span></span>

* <span data-ttu-id="0bba9-2596">Unterstützung für das Entfernen der vom System zugewiesenen Identität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2596">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="0bba9-2597">25. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="0bba9-2597">June 25, 2018</span></span>

<span data-ttu-id="0bba9-2598">Version 2.0.39</span><span class="sxs-lookup"><span data-stu-id="0bba9-2598">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="0bba9-2599">Befehlszeilenschnittstelle (CLI)</span><span class="sxs-lookup"><span data-stu-id="0bba9-2599">CLI</span></span>

* <span data-ttu-id="0bba9-2600">Dateieinschränkung in MSI-Installer aktualisiert, um Problem mit der Erweiterungsinstallation zu beheben</span><span class="sxs-lookup"><span data-stu-id="0bba9-2600">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="0bba9-2601">19. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="0bba9-2601">June 19, 2018</span></span>

<span data-ttu-id="0bba9-2602">Version 2.0.38</span><span class="sxs-lookup"><span data-stu-id="0bba9-2602">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="0bba9-2603">Core</span><span class="sxs-lookup"><span data-stu-id="0bba9-2603">Core</span></span>

* <span data-ttu-id="0bba9-2604">Globale Unterstützung für `--subscription` zu den meisten Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2604">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="0bba9-2605">ACR</span><span class="sxs-lookup"><span data-stu-id="0bba9-2605">ACR</span></span>

* <span data-ttu-id="0bba9-2606">`azure-storage-blob` als Abhängigkeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2606">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="0bba9-2607">CPU-Standardkonfiguration für `acr build-task create` geändert, sodass zwei Kerne verwendet werden</span><span class="sxs-lookup"><span data-stu-id="0bba9-2607">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="0bba9-2608">ACS</span><span class="sxs-lookup"><span data-stu-id="0bba9-2608">ACS</span></span>

* <span data-ttu-id="0bba9-2609">Optionen des Befehls `aks use-dev-spaces` wurden aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2609">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="0bba9-2610">Unterstützung für `--update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2610">Added `--update` support</span></span>
* <span data-ttu-id="0bba9-2611">`aks get-credentials --admin` geändert, sodass der Benutzerkontext in `$HOME/.kube/config` ersetzt wird</span><span class="sxs-lookup"><span data-stu-id="0bba9-2611">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="0bba9-2612">Schreibgeschützte `nodeResourceGroup`-Eigenschaft in verwalteten Clustern verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="0bba9-2612">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="0bba9-2613">Befehlsfehler `acs browse` korrigiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-2613">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="0bba9-2614">`--connector-name` für `aks install-connector`, `aks upgrade-connector` und `aks remove-connector` als optional festgelegt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2614">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="0bba9-2615">Neue Azure Container Instances-Regionen für `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2615">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="0bba9-2616">Normalisierter Speicherort im Helm-Versionsnamen und Knotenname zu `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2616">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="0bba9-2617">AppService</span><span class="sxs-lookup"><span data-stu-id="0bba9-2617">AppService</span></span>

* <span data-ttu-id="0bba9-2618">Unterstützung für neuere Versionen von „urllib“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2618">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="0bba9-2619">Unterstützung der Verwendung eines App Service-Plans aus externen Ressourcengruppen zu `functionapp create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2619">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="0bba9-2620">Batch</span><span class="sxs-lookup"><span data-stu-id="0bba9-2620">Batch</span></span>

* <span data-ttu-id="0bba9-2621">`azure-batch-extensions`-Abhängigkeit entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2621">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="0bba9-2622">Batch KI</span><span class="sxs-lookup"><span data-stu-id="0bba9-2622">Batch AI</span></span>

* <span data-ttu-id="0bba9-2623">Unterstützung für Arbeitsbereiche wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2623">Added support for workspaces.</span></span> <span data-ttu-id="0bba9-2624">Arbeitsbereiche ermöglichen das Zusammenfassen von Clustern, Dateiservern und Experimenten in Gruppen ohne Beschränkung der Anzahl von Ressourcen, die erstellt werden können.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2624">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="0bba9-2625">Unterstützung für Experimente wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2625">Added support for experiments.</span></span> <span data-ttu-id="0bba9-2626">Experimente ermöglichen das Zusammenfassen von Aufträgen in Sammlungen ohne Beschränkung der Anzahl von erstellten Aufträgen.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2626">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="0bba9-2627">Unterstützung für das Konfigurieren von `/dev/shm` für Aufträge hinzugefügt, die in einem Docker-Container ausgeführt werden</span><span class="sxs-lookup"><span data-stu-id="0bba9-2627">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="0bba9-2628">Die Befehle `batchai cluster node exec` und `batchai job node exec` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2628">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="0bba9-2629">Diese Befehle ermöglichen die Ausführung aller Befehle direkt auf Knoten und bieten Funktionen zur Portweiterleitung.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2629">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="0bba9-2630">Unterstützung für `--ids` zu `batchai`-Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2630">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="0bba9-2631">[BREAKING CHANGE] Alle Cluster und Dateiserver müssen unter Arbeitsbereichen erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2631">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="0bba9-2632">[BREAKING CHANGE] Aufträge müssen unter Experimenten erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2632">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="0bba9-2633">[BREAKING CHANGE]`--nfs-resource-group` wurde aus den Befehlen `cluster create` und `job create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2633">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="0bba9-2634">Geben Sie zum Bereitstellen eines NFS, das einem anderen Arbeitsbereich/einer anderen Ressourcengruppe angehört, die ARM-ID des Dateiservers über die Option `--nfs` an.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2634">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="0bba9-2635">[BREAKING CHANGE]`--cluster-resource-group` wurde aus dem Befehl `job create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2635">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="0bba9-2636">Geben Sie zum Übermitteln eines Auftrags, der einem anderen Arbeitsbereich/einer anderen Ressourcengruppe angehört, die ARM-ID des Clusters über die Option `--cluster` an.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2636">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="0bba9-2637">[BREAKING CHANGE] Attribut `location` wurde aus Aufträgen, Clustern und Dateiservern entfernt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2637">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="0bba9-2638">„Location“ ist jetzt ein Attribut eines Arbeitsbereichs.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2638">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="0bba9-2639">[BREAKING CHANGE]`--location` wurde aus den Befehlen `job create`, `cluster create` und `file-server create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2639">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="0bba9-2640">[BREAKING CHANGE] Namen von Kurzoptionen wurden geändert, um die Schnittstelle konsistenter zu machen:</span><span class="sxs-lookup"><span data-stu-id="0bba9-2640">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="0bba9-2641">[`--config`, `-c`] in [`--config-file`, `-f`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2641">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="0bba9-2642">[`--cluster`, `-r`] in [`--cluster`, `-c`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2642">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="0bba9-2643">[`--cluster`, `-n`] in [`--cluster`, `-c`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2643">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="0bba9-2644">[`--job`, `-n`] in [`--job`, `-j`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2644">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="0bba9-2645">Karten</span><span class="sxs-lookup"><span data-stu-id="0bba9-2645">Maps</span></span>

* <span data-ttu-id="0bba9-2646">[BREAKING CHANGE]`maps account create` wurde so geändert, dass Nutzungsbedingungen entweder durch interaktive Eingabeaufforderung oder `--accept-tos`-Flag akzeptiert werden müssen.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2646">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="0bba9-2647">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0bba9-2647">Network</span></span>

* <span data-ttu-id="0bba9-2648">Unterstützung für `https` zu `network lb probe create` hinzugefügt [Nr. 6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="0bba9-2648">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="0bba9-2649">Problem behoben, aufgrund dessen die Groß-/Kleinschreibung von `--endpoint-status` berücksichtigt wurde.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2649">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="0bba9-2650">#6502</span><span class="sxs-lookup"><span data-stu-id="0bba9-2650">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="0bba9-2651">Reservations</span><span class="sxs-lookup"><span data-stu-id="0bba9-2651">Reservations</span></span>

* <span data-ttu-id="0bba9-2652">[BREAKING CHANGE] Erforderlicher Parameter `ReservedResourceType` zu `reservations catalog show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2652">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="0bba9-2653">Parameter `Location` zu `reservations catalog show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2653">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="0bba9-2654">[BREAKING CHANGE]`kind` aus `ReservationProperties` entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2654">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="0bba9-2655">[BREAKING CHANGE]`capabilities` wurde in `Catalog` in `sku_properties` umbenannt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2655">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="0bba9-2656">[BREAKING CHANGE] Eigenschaften `size` und `tier` aus `Catalog` entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2656">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="0bba9-2657">Parameter `InstanceFlexibility` zu `reservations reservation update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2657">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="0bba9-2658">Role</span><span class="sxs-lookup"><span data-stu-id="0bba9-2658">Role</span></span>

* <span data-ttu-id="0bba9-2659">Fehlerbehandlung verbessert</span><span class="sxs-lookup"><span data-stu-id="0bba9-2659">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="0bba9-2660">SQL</span><span class="sxs-lookup"><span data-stu-id="0bba9-2660">SQL</span></span>

* <span data-ttu-id="0bba9-2661">Verwirrender Fehler behoben, der beim Ausführen von `az sql db list-editions` für einen Ort auftrat, der für Ihr Abonnement nicht verfügbar ist</span><span class="sxs-lookup"><span data-stu-id="0bba9-2661">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="0bba9-2662">Storage</span><span class="sxs-lookup"><span data-stu-id="0bba9-2662">Storage</span></span>

* <span data-ttu-id="0bba9-2663">Lesbarkeit der Tabellenausgabe für `storage blob download` verbessert</span><span class="sxs-lookup"><span data-stu-id="0bba9-2663">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="0bba9-2664">VM</span><span class="sxs-lookup"><span data-stu-id="0bba9-2664">VM</span></span>

* <span data-ttu-id="0bba9-2665">Verbesserte Einschränkung der VM-Größenüberprüfung für Unterstützung von beschleunigten Netzwerken in `vm create`</span><span class="sxs-lookup"><span data-stu-id="0bba9-2665">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="0bba9-2666">Warnung für `vmss create` hinzugefügt, dass die VM-Standardgröße von `Standard_D1_v2` auf `Standard_DS1_v2` umgestellt wird</span><span class="sxs-lookup"><span data-stu-id="0bba9-2666">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="0bba9-2667">`--force-update` zu `[vm|vmss] extension set` hinzugefügt, um die Erweiterung auch dann zu aktualisieren, wenn die Konfiguration nicht geändert wurde</span><span class="sxs-lookup"><span data-stu-id="0bba9-2667">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="0bba9-2668">13. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="0bba9-2668">June 13, 2018</span></span>

<span data-ttu-id="0bba9-2669">Version 2.0.37</span><span class="sxs-lookup"><span data-stu-id="0bba9-2669">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="0bba9-2670">Core</span><span class="sxs-lookup"><span data-stu-id="0bba9-2670">Core</span></span>

* <span data-ttu-id="0bba9-2671">Verbesserte interaktive Telemetrie</span><span class="sxs-lookup"><span data-stu-id="0bba9-2671">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="0bba9-2672">13. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="0bba9-2672">June 13, 2018</span></span>

<span data-ttu-id="0bba9-2673">Version 2.0.36</span><span class="sxs-lookup"><span data-stu-id="0bba9-2673">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="0bba9-2674">AKS</span><span class="sxs-lookup"><span data-stu-id="0bba9-2674">AKS</span></span>

* <span data-ttu-id="0bba9-2675">Zusätzliche erweiterte Netzwerkoptionen zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2675">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="0bba9-2676">Argumente zu `aks create` zum Aktivieren der Überwachung und HTTP-Routing hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2676">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="0bba9-2677">Argument `--no-ssh-key` zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2677">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="0bba9-2678">Argument `--enable-rbac` zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2678">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="0bba9-2679">[VORSCHAUVERSION] Unterstützung für Azure Active Directory-Authentifizierung zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2679">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="0bba9-2680">AppService</span><span class="sxs-lookup"><span data-stu-id="0bba9-2680">AppService</span></span>

* <span data-ttu-id="0bba9-2681">Problem mit inkompatiblen urllib-Versionen behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-2681">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="0bba9-2682">5\. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="0bba9-2682">June 5, 2018</span></span>

<span data-ttu-id="0bba9-2683">Version 2.0.35</span><span class="sxs-lookup"><span data-stu-id="0bba9-2683">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="0bba9-2684">Interactive</span><span class="sxs-lookup"><span data-stu-id="0bba9-2684">Interactive</span></span>

* <span data-ttu-id="0bba9-2685">Grenzwerte für die Abhängigkeiten des interaktiven Modus hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2685">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="0bba9-2686">5\. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="0bba9-2686">June 5, 2018</span></span>

<span data-ttu-id="0bba9-2687">Version 2.0.34</span><span class="sxs-lookup"><span data-stu-id="0bba9-2687">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="0bba9-2688">Core</span><span class="sxs-lookup"><span data-stu-id="0bba9-2688">Core</span></span>

* <span data-ttu-id="0bba9-2689">Unterstützung für mandantenübergreifende Ressourcenverweise hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2689">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="0bba9-2690">Verbesserte Zuverlässigkeit bei Telemetrieuploads</span><span class="sxs-lookup"><span data-stu-id="0bba9-2690">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="0bba9-2691">ACR</span><span class="sxs-lookup"><span data-stu-id="0bba9-2691">ACR</span></span>

* <span data-ttu-id="0bba9-2692">Unterstützung für VSTS als Remotequellort hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2692">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="0bba9-2693">Befehl `acr import` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2693">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="0bba9-2694">AKS</span><span class="sxs-lookup"><span data-stu-id="0bba9-2694">AKS</span></span>

* <span data-ttu-id="0bba9-2695">`aks get-credentials` wurde geändert, um die Kube-Konfigurationsdatei mit sichereren Dateisystemberechtigungen zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2695">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="0bba9-2696">Batch</span><span class="sxs-lookup"><span data-stu-id="0bba9-2696">Batch</span></span>

* <span data-ttu-id="0bba9-2697">Fehler bei der Formatierung der Poollistentabelle behoben [[Problem 4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="0bba9-2697">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="0bba9-2698">IoT</span><span class="sxs-lookup"><span data-stu-id="0bba9-2698">IOT</span></span>

* <span data-ttu-id="0bba9-2699">Unterstützung für das Erstellen von IoT Hub-Instanzen im Tarif „Basic“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2699">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="0bba9-2700">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0bba9-2700">Network</span></span>

* <span data-ttu-id="0bba9-2701">`network vnet peering` wurde verbessert.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2701">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="0bba9-2702">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="0bba9-2702">Policy Insights</span></span>

* <span data-ttu-id="0bba9-2703">Erstrelease</span><span class="sxs-lookup"><span data-stu-id="0bba9-2703">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="0bba9-2704">ARM</span><span class="sxs-lookup"><span data-stu-id="0bba9-2704">ARM</span></span>

* <span data-ttu-id="0bba9-2705">Befehle vom Typ `account management-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2705">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="0bba9-2706">SQL</span><span class="sxs-lookup"><span data-stu-id="0bba9-2706">SQL</span></span>

* <span data-ttu-id="0bba9-2707">Neue Befehle für verwaltete Instanzen hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="0bba9-2707">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="0bba9-2708">Neue Befehle für verwaltete Datenbanken hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="0bba9-2708">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="0bba9-2709">Storage</span><span class="sxs-lookup"><span data-stu-id="0bba9-2709">Storage</span></span>

* <span data-ttu-id="0bba9-2710">Zusätzliche MimeTypes für JSON und JavaScript hinzugefügt (abzuleiten aus Dateierweiterungen)</span><span class="sxs-lookup"><span data-stu-id="0bba9-2710">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="0bba9-2711">VM</span><span class="sxs-lookup"><span data-stu-id="0bba9-2711">VM</span></span>

* <span data-ttu-id="0bba9-2712">`vm list-skus` wurde geändert, um feste Spalten zu verwenden und eine Warnung hinzuzufügen, dass `Tier` und `Size` entfernt werden.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2712">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="0bba9-2713">Option `--accelerated-networking` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2713">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="0bba9-2714">`--tags` zu `identity create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2714">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="0bba9-2715">22. Mai 2018</span><span class="sxs-lookup"><span data-stu-id="0bba9-2715">May 22, 2018</span></span>

<span data-ttu-id="0bba9-2716">Version 2.0.33</span><span class="sxs-lookup"><span data-stu-id="0bba9-2716">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="0bba9-2717">Core</span><span class="sxs-lookup"><span data-stu-id="0bba9-2717">Core</span></span>

* <span data-ttu-id="0bba9-2718">Unterstützung für das Erweitern von `@` in Dateinamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2718">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="0bba9-2719">ACS</span><span class="sxs-lookup"><span data-stu-id="0bba9-2719">ACS</span></span>

* <span data-ttu-id="0bba9-2720">Neue Dev Spaces-Befehle `aks use-dev-spaces` und `aks remove-dev-spaces` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2720">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="0bba9-2721">Tippfehler in Hilfemeldung korrigiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-2721">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="0bba9-2722">AppService</span><span class="sxs-lookup"><span data-stu-id="0bba9-2722">AppService</span></span>

* <span data-ttu-id="0bba9-2723">Verbesserte generische Aktualisierungsbefehle</span><span class="sxs-lookup"><span data-stu-id="0bba9-2723">Improved generic update commands</span></span>
* <span data-ttu-id="0bba9-2724">Asynchrone Unterstützung für `webapp deployment source config-zip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2724">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="0bba9-2725">Container</span><span class="sxs-lookup"><span data-stu-id="0bba9-2725">Container</span></span>

* <span data-ttu-id="0bba9-2726">Unterstützung für das Exportieren einer Containergruppe im YAML-Format hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2726">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="0bba9-2727">Unterstützung für die Verwendung einer YAML-Datei zum Erstellen/Aktualisieren einer Containergruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2727">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="0bba9-2728">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="0bba9-2728">Extension</span></span>

* <span data-ttu-id="0bba9-2729">Verbesserte Entfernung von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="0bba9-2729">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="0bba9-2730">Interactive</span><span class="sxs-lookup"><span data-stu-id="0bba9-2730">Interactive</span></span>

* <span data-ttu-id="0bba9-2731">Protokollierung geändert, um Parser für Abschlüsse zu deaktivieren</span><span class="sxs-lookup"><span data-stu-id="0bba9-2731">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="0bba9-2732">Verbesserte Verarbeitung beschädigter Hilfscaches</span><span class="sxs-lookup"><span data-stu-id="0bba9-2732">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="0bba9-2733">KeyVault</span><span class="sxs-lookup"><span data-stu-id="0bba9-2733">KeyVault</span></span>

* <span data-ttu-id="0bba9-2734">keyvault-Befehle wurden korrigiert, damit sie in Cloud Shell oder auf virtuellen Computern mit Identität verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2734">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="0bba9-2735">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0bba9-2735">Network</span></span>

* <span data-ttu-id="0bba9-2736">Problem behoben, aufgrund dessen `network watcher show-topology` nicht mit einem VNET und/oder Subnetznamen verwendet werden konnte ([#6326](https://github.com/Azure/azure-cli/issues/6326))</span><span class="sxs-lookup"><span data-stu-id="0bba9-2736">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="0bba9-2737">Problem behoben, aufgrund dessen einige `network watcher`-Befehle fälschlicherweise angaben, dass Network Watcher nicht für bestimmte Regionen aktiviert ist ([#6264](https://github.com/Azure/azure-cli/issues/6264))</span><span class="sxs-lookup"><span data-stu-id="0bba9-2737">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="0bba9-2738">SQL</span><span class="sxs-lookup"><span data-stu-id="0bba9-2738">SQL</span></span>

* <span data-ttu-id="0bba9-2739">[BREAKING CHANGE] Von den Befehlen `db` und `dw` zurückgegebene Antwortobjekte geändert:</span><span class="sxs-lookup"><span data-stu-id="0bba9-2739">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="0bba9-2740">Eigenschaft `serviceLevelObjective` in `currentServiceObjectiveName` umbenannt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2740">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="0bba9-2741">Eigenschaften `currentServiceObjectiveId` und `requestedServiceObjectiveId` entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2741">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="0bba9-2742">Eigenschaft `maxSizeBytes` geändert (ist nun keine Zeichenfolge mehr, sondern ein Ganzzahlwert)</span><span class="sxs-lookup"><span data-stu-id="0bba9-2742">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="0bba9-2743">[BREAKING CHANGE] Die folgenden `db`- und `dw`-Eigenschaften wurden geändert und sind jetzt schreibgeschützt:</span><span class="sxs-lookup"><span data-stu-id="0bba9-2743">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="0bba9-2744">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2744">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="0bba9-2745">Verwenden Sie zum Aktualisieren den Parameter `--service-objective`, oder legen Sie die Eigenschaft `sku.name` fest.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2745">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="0bba9-2746">`edition`.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2746">`edition`.</span></span> <span data-ttu-id="0bba9-2747">Verwenden Sie zum Aktualisieren den Parameter `--edition`, oder legen Sie die Eigenschaft `sku.tier` fest.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2747">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="0bba9-2748">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2748">`elasticPoolName`.</span></span> <span data-ttu-id="0bba9-2749">Verwenden Sie zum Aktualisieren den Parameter `--elastic-pool`, oder legen Sie die Eigenschaft `elasticPoolId` fest.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2749">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="0bba9-2750">[BREAKING CHANGE] Die folgenden `elastic-pool`-Eigenschaften wurden geändert und sind jetzt schreibgeschützt:</span><span class="sxs-lookup"><span data-stu-id="0bba9-2750">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="0bba9-2751">`edition`.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2751">`edition`.</span></span> <span data-ttu-id="0bba9-2752">Verwenden Sie zum Aktualisieren den Parameter `--edition`.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2752">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="0bba9-2753">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2753">`dtu`.</span></span> <span data-ttu-id="0bba9-2754">Verwenden Sie zum Aktualisieren den Parameter `--capacity`.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2754">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="0bba9-2755">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2755">`databaseDtuMin`.</span></span> <span data-ttu-id="0bba9-2756">Verwenden Sie zum Aktualisieren den Parameter `--db-min-capacity`.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2756">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="0bba9-2757">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2757">`databaseDtuMax`.</span></span> <span data-ttu-id="0bba9-2758">Verwenden Sie zum Aktualisieren den Parameter `--db-max-capacity`.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2758">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="0bba9-2759">Die Parameter `--family` und `--capacity` wurden zu den `db`-, `dw`- und `elastic-pool`-Befehlen hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2759">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="0bba9-2760">Den `db`-, `dw`- und `elastic-pool`-Befehlen wurden Tabellenformatierer hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2760">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="0bba9-2761">Storage</span><span class="sxs-lookup"><span data-stu-id="0bba9-2761">Storage</span></span>

* <span data-ttu-id="0bba9-2762">Vervollständigung für das Argument `--account-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2762">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="0bba9-2763">Problem mit `storage entity query` behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-2763">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="0bba9-2764">VM</span><span class="sxs-lookup"><span data-stu-id="0bba9-2764">VM</span></span>

* <span data-ttu-id="0bba9-2765">[BREAKING CHANGE]`--write-accelerator` aus `vm create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2765">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="0bba9-2766">Die gleiche Unterstützung kann über `vm update` oder `vm disk attach` erzielt werden.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2766">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="0bba9-2767">Erweiterungsimageabgleich in `[vm|vmss] extension` korrigiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-2767">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="0bba9-2768">`--boot-diagnostics-storage` zu `vm create` zur Erfassung des Startprotokolls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2768">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="0bba9-2769">`--license-type` zu `[vm|vmss] update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2769">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="0bba9-2770">7\. Mai 2018</span><span class="sxs-lookup"><span data-stu-id="0bba9-2770">May 7, 2018</span></span>

<span data-ttu-id="0bba9-2771">Version 2.0.32</span><span class="sxs-lookup"><span data-stu-id="0bba9-2771">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="0bba9-2772">Core</span><span class="sxs-lookup"><span data-stu-id="0bba9-2772">Core</span></span>

* <span data-ttu-id="0bba9-2773">Ein Ausnahmefehler wurde behoben, der beim Abrufen von Geheimnissen aus einem Dienstprinzipalkonto mit Zertifikat auftrat.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2773">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="0bba9-2774">Eingeschränkte Unterstützung für positionelle Argumente hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2774">Added limited support for positional arguments</span></span>
* <span data-ttu-id="0bba9-2775">Problem behoben, aufgrund dessen `--query` nicht mit `--ids` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="0bba9-2775">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="0bba9-2776">#5591</span><span class="sxs-lookup"><span data-stu-id="0bba9-2776">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="0bba9-2777">Pipingszenarien von Befehlen bei Verwendung von `--ids` verbessert</span><span class="sxs-lookup"><span data-stu-id="0bba9-2777">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="0bba9-2778">Unterstützt `-o tsv` mit angegebener Abfrage bzw. `-o json` ohne angegeben Abfrage</span><span class="sxs-lookup"><span data-stu-id="0bba9-2778">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="0bba9-2779">Befehlsvorschläge bei Fehler hinzugefügt, wenn Befehle Tippfehler enthielten</span><span class="sxs-lookup"><span data-stu-id="0bba9-2779">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="0bba9-2780">Fehler bei der Eingabe von `az ''` behandelt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2780">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="0bba9-2781">Unterstützung für benutzerdefinierte Ressourcentypen für Befehlsmodule und -erweiterungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2781">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="0bba9-2782">ACR</span><span class="sxs-lookup"><span data-stu-id="0bba9-2782">ACR</span></span>

* <span data-ttu-id="0bba9-2783">ACR Build-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2783">Added ACR Build commands</span></span>
* <span data-ttu-id="0bba9-2784">Fehlermeldungen vom Typ „Ressource nicht gefunden.“ verbessert</span><span class="sxs-lookup"><span data-stu-id="0bba9-2784">Improved resource not found error messages</span></span>
* <span data-ttu-id="0bba9-2785">Höhere Leistung bei der Ressourcenerstellung und optimierte Fehlerbehandlung</span><span class="sxs-lookup"><span data-stu-id="0bba9-2785">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="0bba9-2786">ACR-Anmeldung bei nicht standardmäßigen Konsolen und WSL optimiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-2786">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="0bba9-2787">Fehlermeldungen zu Repositorybefehlen optimiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-2787">Improved repository commands error messages</span></span>
* <span data-ttu-id="0bba9-2788">Tabellenspalten und -reihenfolge aktualisiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-2788">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="0bba9-2789">ACS</span><span class="sxs-lookup"><span data-stu-id="0bba9-2789">ACS</span></span>

* <span data-ttu-id="0bba9-2790">Warnung hinzugefügt, dass `az aks` eine Vorschauversion des Diensts ist</span><span class="sxs-lookup"><span data-stu-id="0bba9-2790">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="0bba9-2791">Berechtigungsproblem in `aks install-connector` behoben, wenn `--aci-resource-group` nicht angegeben wird</span><span class="sxs-lookup"><span data-stu-id="0bba9-2791">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="0bba9-2792">AMS</span><span class="sxs-lookup"><span data-stu-id="0bba9-2792">AMS</span></span>

* <span data-ttu-id="0bba9-2793">Erste Version: Verwalten von Azure Media Services-Ressourcen</span><span class="sxs-lookup"><span data-stu-id="0bba9-2793">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="0bba9-2794">AppService</span><span class="sxs-lookup"><span data-stu-id="0bba9-2794">Appservice</span></span>

* <span data-ttu-id="0bba9-2795">Ein Problem in `webapp delete` wurde behoben, das bei Angabe von `--slot` auftrat.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2795">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="0bba9-2796">`--runtime-version` aus `webapp auth update` entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2796">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="0bba9-2797">Unterstützung für „min\_tls\_version“ und „https2.0“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2797">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="0bba9-2798">Unterstützung für mehrere Container hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2798">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="0bba9-2799">Batch KI</span><span class="sxs-lookup"><span data-stu-id="0bba9-2799">Batch AI</span></span>

* <span data-ttu-id="0bba9-2800">`batchai create cluster` wurde geändert, um die in der Konfigurationsdatei des Clusters konfigurierte VM-Priorität zu berücksichtigen.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2800">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="0bba9-2801">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="0bba9-2801">Cognitive Services</span></span>

* <span data-ttu-id="0bba9-2802">Tippfehler im Beispiel für `cognitiveservices account create` behoben [Nr. 5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="0bba9-2802">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="0bba9-2803">Nutzung</span><span class="sxs-lookup"><span data-stu-id="0bba9-2803">Consumption</span></span>

* <span data-ttu-id="0bba9-2804">Neue Befehle für Budget-API hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2804">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="0bba9-2805">Container</span><span class="sxs-lookup"><span data-stu-id="0bba9-2805">Container</span></span>

* <span data-ttu-id="0bba9-2806">`--registry-server` muss nicht mehr für `container create` angegeben werden, wenn ein Registrierungsserver im Imagenamen enthalten ist.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2806">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="0bba9-2807">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="0bba9-2807">Cosmos DB</span></span>

* <span data-ttu-id="0bba9-2808">VNET-Unterstützung für Azure CLI eingeführt: Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="0bba9-2808">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="0bba9-2809">DMS</span><span class="sxs-lookup"><span data-stu-id="0bba9-2809">DMS</span></span>

* <span data-ttu-id="0bba9-2810">Erste Version: Die Migration von SQL zu Azure SQL wird nun unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2810">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="0bba9-2811">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="0bba9-2811">Extension</span></span>

* <span data-ttu-id="0bba9-2812">Fehler behoben, aufgrund dessen Erweiterungsmetadaten nicht mehr angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="0bba9-2812">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="0bba9-2813">Interactive</span><span class="sxs-lookup"><span data-stu-id="0bba9-2813">Interactive</span></span>

* <span data-ttu-id="0bba9-2814">Interaktive Vervollständigung funktioniert nun auch mit positionellen Argumenten.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2814">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="0bba9-2815">Benutzerfreundlichere Ausgabe bei der Eingabe von '\'</span><span class="sxs-lookup"><span data-stu-id="0bba9-2815">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="0bba9-2816">Abschlüsse für Parameter ohne Hilfe korrigiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-2816">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="0bba9-2817">Beschreibungen für Befehlsgruppen korrigiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-2817">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="0bba9-2818">Labor</span><span class="sxs-lookup"><span data-stu-id="0bba9-2818">Lab</span></span>

* <span data-ttu-id="0bba9-2819">Regressionen aus Knack-Umwandlung korrigiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-2819">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="0bba9-2820">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0bba9-2820">Network</span></span>

* <span data-ttu-id="0bba9-2821">[BREAKING CHANGE] Parameter `--ids` entfernt für:</span><span class="sxs-lookup"><span data-stu-id="0bba9-2821">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="0bba9-2822">Profil</span><span class="sxs-lookup"><span data-stu-id="0bba9-2822">Profile</span></span>

* <span data-ttu-id="0bba9-2823">Quellerkennung für `disk create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-2823">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="0bba9-2824">[BREAKING CHANGE]`--msi-port` und `--identity-port` entfernt, da sie nicht mehr verwendet werden</span><span class="sxs-lookup"><span data-stu-id="0bba9-2824">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="0bba9-2825">Tippfehler in kurzer Zusammenfassung für `account get-access-token` korrigiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-2825">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="0bba9-2826">Redis</span><span class="sxs-lookup"><span data-stu-id="0bba9-2826">Redis</span></span>

* <span data-ttu-id="0bba9-2827">`redis patch-schedule patch-schedule show` wurde durch `redis patch-schedule show` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2827">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="0bba9-2828">`redis list-all` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-2828">Deprecated `redis list-all`.</span></span> <span data-ttu-id="0bba9-2829">Diese Funktion wurde in `redis list` integriert.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2829">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="0bba9-2830">`redis import-method` wurde durch `redis import` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2830">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="0bba9-2831">Unterstützung für `--ids` zu verschiedenen Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2831">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="0bba9-2832">Role</span><span class="sxs-lookup"><span data-stu-id="0bba9-2832">Role</span></span>

* <span data-ttu-id="0bba9-2833">[BREAKING CHANGE] Veralteter Befehl `ad sp reset-credentials` entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2833">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="0bba9-2834">Storage</span><span class="sxs-lookup"><span data-stu-id="0bba9-2834">Storage</span></span>

* <span data-ttu-id="0bba9-2835">Zulassen, dass das Ziel-SAS-Token für die Blobkopie auf die Quelle angewendet wird, wenn Quell-SAS und Kontoschlüssel nicht angegeben werden</span><span class="sxs-lookup"><span data-stu-id="0bba9-2835">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="0bba9-2836">Verfügbar gemacht: Socket-Timeout für Blobuploads und -downloads</span><span class="sxs-lookup"><span data-stu-id="0bba9-2836">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="0bba9-2837">Blobnamen, die mit Pfadtrennzeichen beginnen, als relative Pfade behandeln</span><span class="sxs-lookup"><span data-stu-id="0bba9-2837">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="0bba9-2838">Zulassen, dass `storage blob copy --source-sas` mit dem Abfragezeichen „?“ beginnt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2838">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="0bba9-2839">`storage entity query --marker` korrigiert, um Liste von Schlüsselwerten zu akzeptieren</span><span class="sxs-lookup"><span data-stu-id="0bba9-2839">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="0bba9-2840">VM</span><span class="sxs-lookup"><span data-stu-id="0bba9-2840">VM</span></span>

* <span data-ttu-id="0bba9-2841">Ungültige Erkennungslogik für nicht verwalteten Blob-URI korrigiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-2841">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="0bba9-2842">Unterstützung für Datenträgerverschlüsselung ohne vom Benutzer bereitgestellte Dienstprinzipale hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2842">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="0bba9-2843">[BREAKING CHANGE] Verwenden Sie nicht „ManagedIdentityExtension“ des virtuellen Computers für MSI-Unterstützung.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2843">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="0bba9-2844">Unterstützung für Entfernungsrichtlinie zu `vmss` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2844">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="0bba9-2845">[BREAKING CHANGE]`--ids` entfernt aus:</span><span class="sxs-lookup"><span data-stu-id="0bba9-2845">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="0bba9-2846">Unterstützung für Schreibbeschleunigung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2846">Added write accelerator support</span></span>
* <span data-ttu-id="0bba9-2847">`vmss perform-maintenance` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2847">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="0bba9-2848">`vm diagnostics set` korrigiert, um zuverlässig den Betriebssystemtyp des virtuellen Computers zu erkennen</span><span class="sxs-lookup"><span data-stu-id="0bba9-2848">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="0bba9-2849">`vm resize` geändert, um zu überprüfen, ob die angeforderte Größe von der derzeit festgelegten Größe abweicht, und nur bei einer Änderung eine Aktualisierung auszuführen</span><span class="sxs-lookup"><span data-stu-id="0bba9-2849">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="0bba9-2850">10. April 2018</span><span class="sxs-lookup"><span data-stu-id="0bba9-2850">April 10, 2018</span></span>

<span data-ttu-id="0bba9-2851">Version 2.0.31</span><span class="sxs-lookup"><span data-stu-id="0bba9-2851">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="0bba9-2852">ACR</span><span class="sxs-lookup"><span data-stu-id="0bba9-2852">ACR</span></span>

* <span data-ttu-id="0bba9-2853">Verbesserte Fehlerbehandlung für wincred-Fallback</span><span class="sxs-lookup"><span data-stu-id="0bba9-2853">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="0bba9-2854">ACS</span><span class="sxs-lookup"><span data-stu-id="0bba9-2854">ACS</span></span>

* <span data-ttu-id="0bba9-2855">Gültigkeit von per AKS erstellten SPNs in fünf Jahre geändert</span><span class="sxs-lookup"><span data-stu-id="0bba9-2855">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="0bba9-2856">AppService</span><span class="sxs-lookup"><span data-stu-id="0bba9-2856">Appservice</span></span>

* [BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="0bba9-2858">Nicht abgefangene Ausnahme für nicht vorhandene Web-App-Pläne behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-2858">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="0bba9-2859">Batch AI</span><span class="sxs-lookup"><span data-stu-id="0bba9-2859">BatchAI</span></span>

* <span data-ttu-id="0bba9-2860">Unterstützung für API 2018-03-01 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2860">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="0bba9-2861">Bereitstellung auf Auftragsebene</span><span class="sxs-lookup"><span data-stu-id="0bba9-2861">Job level mounting</span></span>
  - <span data-ttu-id="0bba9-2862">Umgebungsvariablen mit Geheimniswerten</span><span class="sxs-lookup"><span data-stu-id="0bba9-2862">Environment variables with secret values</span></span>
  - <span data-ttu-id="0bba9-2863">Einstellungen von Leistungsindikatoren</span><span class="sxs-lookup"><span data-stu-id="0bba9-2863">Performance counters settings</span></span>
  - <span data-ttu-id="0bba9-2864">Berichtstellung für auftragsspezifisches Pfadsegment</span><span class="sxs-lookup"><span data-stu-id="0bba9-2864">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="0bba9-2865">Unterstützung für Unterordner in Listendateien-API</span><span class="sxs-lookup"><span data-stu-id="0bba9-2865">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="0bba9-2866">Berichterstellung zur Nutzung und zu Grenzwerten</span><span class="sxs-lookup"><span data-stu-id="0bba9-2866">Usage and limits reporting</span></span>
  - <span data-ttu-id="0bba9-2867">Zulassen der Angabe des Cachetyps für NFS-Server</span><span class="sxs-lookup"><span data-stu-id="0bba9-2867">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="0bba9-2868">Unterstützung für benutzerdefinierte Images</span><span class="sxs-lookup"><span data-stu-id="0bba9-2868">Support for custom images</span></span>
  - <span data-ttu-id="0bba9-2869">Unterstützung für pyTorch-Toolkit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2869">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="0bba9-2870">Befehl `job wait` hinzugefügt, der das Warten auf die Auftragsfertigstellung ermöglicht und den Code für die Auftragsbeendigung meldet</span><span class="sxs-lookup"><span data-stu-id="0bba9-2870">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="0bba9-2871">Befehl `usage show` hinzugefügt, mit dem die aktuelle Nutzung von Batch KI-Ressourcen und die Grenzwerte für verschiedene Regionen aufgelistet werden</span><span class="sxs-lookup"><span data-stu-id="0bba9-2871">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="0bba9-2872">Nationale Clouds werden unterstützt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2872">National clouds are supported</span></span>
* <span data-ttu-id="0bba9-2873">Befehlszeilenargumente für Aufträge hinzugefügt, um das Bereitstellen von Dateisystemen auf Auftragsebene zusätzlich zu Konfigurationsdateien zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="0bba9-2873">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="0bba9-2874">Weitere Optionen zum Anpassen von Clustern hinzugefügt – VM-Priorität, Subnetz, anfängliche Knotenanzahl für Cluster mit automatischer Skalierung, Angeben eines benutzerdefinierten Images</span><span class="sxs-lookup"><span data-stu-id="0bba9-2874">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="0bba9-2875">Befehlszeilenoption zum Angeben des Cachetyps für NFS mit Verwaltung per Batch KI hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2875">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="0bba9-2876">Angeben der Bereitstellung von Dateisystemen in Konfigurationsdateien vereinfacht.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2876">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="0bba9-2877">Weglassen von Anmeldeinformationen für Azure-Dateifreigaben und Azure-Blobcontainer ist jetzt möglich. Die CLI füllt fehlende Anmeldeinformationen auf, indem der Speicherkontoschlüssel verwendet wird, der über Befehlszeilenparameter oder per Umgebungsvariable angegeben wird, oder der Schlüssel wird über Azure Storage abgefragt (sofern das Speicherkonto zum aktuellen Abonnement gehört).</span><span class="sxs-lookup"><span data-stu-id="0bba9-2877">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="0bba9-2878">Der Befehl zum Streamen von Auftragsdateien wird jetzt automatisch abgeschlossen, nachdem der Auftrag beendet ist (Erfolg, Fehler, Beendigung oder Löschung)</span><span class="sxs-lookup"><span data-stu-id="0bba9-2878">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="0bba9-2879">Verbesserte `table`-Ausgabe für `show`-Vorgänge</span><span class="sxs-lookup"><span data-stu-id="0bba9-2879">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="0bba9-2880">Option `--use-auto-storage` für die Clustererstellung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2880">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="0bba9-2881">Diese Option erleichtert die Verwaltung von Speicherkonten und die Bereitstellung von Azure-Dateifreigaben und Azure-Blobcontainern in Clustern.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2881">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="0bba9-2882">`--generate-ssh-keys` für `cluster create` und `file-server create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2882">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="0bba9-2883">Möglichkeit zum Angeben der Knotensetupaufgabe über die Befehlszeile</span><span class="sxs-lookup"><span data-stu-id="0bba9-2883">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="0bba9-2884">[BREAKING CHANGE] Befehl `job stream-file` und `job list-files` in die Gruppe `job file` verschoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-2884">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="0bba9-2885">[BREAKING CHANGE]`--admin-user-name` im Befehl `file-server create` in `--user-name` umbenannt, um Einheitlichkeit mit dem Befehl `cluster create` zu erzielen</span><span class="sxs-lookup"><span data-stu-id="0bba9-2885">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="0bba9-2886">Abrechnung</span><span class="sxs-lookup"><span data-stu-id="0bba9-2886">Billing</span></span>

* <span data-ttu-id="0bba9-2887">Registrierungskontobefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2887">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="0bba9-2888">Nutzung</span><span class="sxs-lookup"><span data-stu-id="0bba9-2888">Consumption</span></span>

* <span data-ttu-id="0bba9-2889">Befehle vom Typ `marketplace` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2889">Added `marketplace` commands</span></span>
* <span data-ttu-id="0bba9-2890">[BREAKING CHANGE]`reservations summaries` in `reservation summary` umbenannt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2890">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="0bba9-2891">[BREAKING CHANGE]`reservations details` in `reservation detail` umbenannt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2891">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="0bba9-2892">[BREAKING CHANGE] Kurzoptionen `--reservation-order-id` und `--reservation-id` für `reservation`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2892">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="0bba9-2893">[BREAKING CHANGE]`--grain`-Kurzoptionen für `reservation summary`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2893">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="0bba9-2894">[BREAKING CHANGE]`--include-meter-details`-Kurzoptionen für `pricesheet`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2894">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="0bba9-2895">Container</span><span class="sxs-lookup"><span data-stu-id="0bba9-2895">Container</span></span>

* <span data-ttu-id="0bba9-2896">Parameter für die Volumebereitstellung für das Git-Repository hinzugefügt: `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` und `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="0bba9-2896">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="0bba9-2897">[#5926](https://github.com/Azure/azure-cli/issues/5926) behoben: Fehler bei `az container exec`, wenn „--container-name“ angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="0bba9-2897">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="0bba9-2898">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="0bba9-2898">Extension</span></span>

* <span data-ttu-id="0bba9-2899">Meldung für Distributionsüberprüfung in Debugebene geändert</span><span class="sxs-lookup"><span data-stu-id="0bba9-2899">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="0bba9-2900">Interactive</span><span class="sxs-lookup"><span data-stu-id="0bba9-2900">Interactive</span></span>

* <span data-ttu-id="0bba9-2901">Geändert: Verhinderung des Abschlusses bei nicht erkannten Befehlen</span><span class="sxs-lookup"><span data-stu-id="0bba9-2901">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="0bba9-2902">Ereignishooks vor und nach der Erstellung der Teilstruktur von Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2902">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="0bba9-2903">Abschluss für `--ids`-Parameter hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2903">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="0bba9-2904">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0bba9-2904">Network</span></span>

* <span data-ttu-id="0bba9-2905">[#5936](https://github.com/Azure/azure-cli/issues/5936) behoben: `application-gateway create`-Tags konnten nicht festgelegt werden</span><span class="sxs-lookup"><span data-stu-id="0bba9-2905">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="0bba9-2906">Argument `--auth-certs` zum Anfügen von Authentifizierungszertifikaten für `application-gateway http-settings [create|update]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2906">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="0bba9-2907">#4910</span><span class="sxs-lookup"><span data-stu-id="0bba9-2907">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="0bba9-2908">`ddos-protection`-Befehle zum Erstellen von DDoS-Schutzplänen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2908">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="0bba9-2909">Unterstützung von `--ddos-protection-plan` für `vnet [create|update]` hinzugefügt, um das Zuordnen eines VNET zu einem DDoS-Schutzplan zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="0bba9-2909">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="0bba9-2910">Problem mit `--disable-bgp-route-propagation`-Flag in `network route-table [create|update]` behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-2910">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="0bba9-2911">Dummy-Argumente `--public-ip-address-type` und `--subnet-type` für `network lb [create|update]` entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2911">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="0bba9-2912">Unterstützung für TXT-Datensätze mit RFC 1035-Escapesequenzen für `network dns zone [import|export]` und `network dns record-set txt add-record` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2912">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="0bba9-2913">Profil</span><span class="sxs-lookup"><span data-stu-id="0bba9-2913">Profile</span></span>

* <span data-ttu-id="0bba9-2914">Unterstützung für klassische Azure-Konten in `account list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2914">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="0bba9-2915">[BREAKING CHANGE]`--msi` & `--msi-port`-Argumente entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2915">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="0bba9-2916">RDBMS</span><span class="sxs-lookup"><span data-stu-id="0bba9-2916">RDBMS</span></span>

* <span data-ttu-id="0bba9-2917">Befehl `georestore` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2917">Added `georestore` command</span></span>
* <span data-ttu-id="0bba9-2918">Speichergrößenbeschränkung aus Befehl `create` entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2918">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="0bba9-2919">Resource</span><span class="sxs-lookup"><span data-stu-id="0bba9-2919">Resource</span></span>

* <span data-ttu-id="0bba9-2920">Unterstützung für `--metadata` zu `policy definition create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2920">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="0bba9-2921">Unterstützung von `--metadata`, `--set`, `--add`, `--remove` für `policy definition update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2921">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="0bba9-2922">SQL</span><span class="sxs-lookup"><span data-stu-id="0bba9-2922">SQL</span></span>

* <span data-ttu-id="0bba9-2923">`sql elastic-pool op list` und `sql elastic-pool op cancel` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2923">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="0bba9-2924">Storage</span><span class="sxs-lookup"><span data-stu-id="0bba9-2924">Storage</span></span>

* <span data-ttu-id="0bba9-2925">Fehlermeldungen für falsch formatierte Verbindungszeichenfolgen verbessert</span><span class="sxs-lookup"><span data-stu-id="0bba9-2925">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="0bba9-2926">VM</span><span class="sxs-lookup"><span data-stu-id="0bba9-2926">VM</span></span>

* <span data-ttu-id="0bba9-2927">Unterstützung für die Konfiguration der Plattform-Fehlerdomänenanzahl für `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2927">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="0bba9-2928">`vmss create` geändert, damit standardmäßig „Standard LB“ für zonales, großes oder per einzelner Platzierungsgruppe deaktiviertes Scale Set festgelegt wird</span><span class="sxs-lookup"><span data-stu-id="0bba9-2928">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret`
* <span data-ttu-id="0bba9-2930">Unterstützung für SKU mit öffentlicher IP für `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2930">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="0bba9-2931">Argumente `--keyvault` und `--resource-group` für `vm secret format` hinzugefügt, um Szenarien zu unterstützen, bei denen der Befehl die Tresor-ID nicht auflösen kann.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2931">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="0bba9-2932">#5718</span><span class="sxs-lookup"><span data-stu-id="0bba9-2932">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="0bba9-2933">Bessere Fehler für `[vm|vmss create]`, wenn der Standort einer Ressourcengruppe keine Zonenunterstützung aufweist</span><span class="sxs-lookup"><span data-stu-id="0bba9-2933">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="0bba9-2934">27. März 2018</span><span class="sxs-lookup"><span data-stu-id="0bba9-2934">March 27, 2018</span></span>

<span data-ttu-id="0bba9-2935">Version 2.0.30</span><span class="sxs-lookup"><span data-stu-id="0bba9-2935">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="0bba9-2936">Core</span><span class="sxs-lookup"><span data-stu-id="0bba9-2936">Core</span></span>

* <span data-ttu-id="0bba9-2937">Anzeigen einer Meldung für Erweiterungen, die in der Hilfe als Vorschauversion gekennzeichnet sind</span><span class="sxs-lookup"><span data-stu-id="0bba9-2937">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="0bba9-2938">ACS</span><span class="sxs-lookup"><span data-stu-id="0bba9-2938">ACS</span></span>

* <span data-ttu-id="0bba9-2939">Behebung eines Fehlers bei der SSL-Zertifikatprüfung für `aks install-cli` in Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="0bba9-2939">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="0bba9-2940">AppService</span><span class="sxs-lookup"><span data-stu-id="0bba9-2940">Appservice</span></span>

* <span data-ttu-id="0bba9-2941">Unterstützung nur von HTTPS zu `webapp update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2941">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="0bba9-2942">Unterstützung für Slots zu `az webapp identity [assign|show]` und `az functionapp identity [assign|show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2942">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="0bba9-2943">Backup</span><span class="sxs-lookup"><span data-stu-id="0bba9-2943">Backup</span></span>

* <span data-ttu-id="0bba9-2944">Neuer Befehl `az backup protection isenabled-for-vm` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2944">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="0bba9-2945">Mit diesem Befehl kann überprüft werden, ob ein virtueller Computer von einem beliebigen Tresor im Abonnement gesichert wird.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2945">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="0bba9-2946">Azure-Objekt-IDs für Parameter `--resource-group` und `--vault-name` für die folgenden Befehle aktiviert:</span><span class="sxs-lookup"><span data-stu-id="0bba9-2946">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="0bba9-2947">`--name`-Parameter wurden geändert, um das Ausgabeformat von `backup ... show`-Befehlen zu akzeptieren.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2947">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="0bba9-2948">Container</span><span class="sxs-lookup"><span data-stu-id="0bba9-2948">Container</span></span>

* <span data-ttu-id="0bba9-2949">Befehl `container exec` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2949">Added `container exec` command.</span></span> <span data-ttu-id="0bba9-2950">Ausführung von Befehlen in einem Container für eine ausgeführte Containergruppe</span><span class="sxs-lookup"><span data-stu-id="0bba9-2950">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="0bba9-2951">Zulassen der Tabellenausgabe zum Erstellen und Aktualisieren einer Containergruppe</span><span class="sxs-lookup"><span data-stu-id="0bba9-2951">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="0bba9-2952">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="0bba9-2952">Extension</span></span>

* <span data-ttu-id="0bba9-2953">Meldung für `extension add` hinzugefügt, wenn sich die Erweiterung in der Vorschauphase befindet</span><span class="sxs-lookup"><span data-stu-id="0bba9-2953">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="0bba9-2954">`extension list-available` geändert, um vollständige Erweiterungsdaten mit `--show-details` anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="0bba9-2954">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="0bba9-2955">[BREAKING CHANGE]`extension list-available` geändert, um standardmäßig vereinfachte Erweiterungsdaten anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="0bba9-2955">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="0bba9-2956">Interactive</span><span class="sxs-lookup"><span data-stu-id="0bba9-2956">Interactive</span></span>

* <span data-ttu-id="0bba9-2957">Vervollständigungen wurden geändert und werden jetzt aktiviert, sobald das Laden der Befehlstabelle abgeschlossen ist.</span><span class="sxs-lookup"><span data-stu-id="0bba9-2957">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="0bba9-2958">Fehler bei der Verwendung des Parameters `--style` behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-2958">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="0bba9-2959">Interaktiver Lexer nach Befehlstabellensicherung instanziiert (sofern nicht vorhanden)</span><span class="sxs-lookup"><span data-stu-id="0bba9-2959">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="0bba9-2960">Verbesserte Unterstützung der Vervollständigung</span><span class="sxs-lookup"><span data-stu-id="0bba9-2960">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="0bba9-2961">Labor</span><span class="sxs-lookup"><span data-stu-id="0bba9-2961">Lab</span></span>

* <span data-ttu-id="0bba9-2962">Probleme mit Befehl `create environment` behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-2962">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="0bba9-2963">Überwachen</span><span class="sxs-lookup"><span data-stu-id="0bba9-2963">Monitor</span></span>

* <span data-ttu-id="0bba9-2964">Unterstützung für `--top`, `--orderby` und `--namespace` zu `metrics list` hinzugefügt [Nr. 5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="0bba9-2964">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="0bba9-2965">[#4529](https://github.com/Azure/azure-cli/issues/5785) behoben: `metrics list` akzeptiert eine durch Leerzeichen getrennte Liste von abzurufenden Metriken</span><span class="sxs-lookup"><span data-stu-id="0bba9-2965">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="0bba9-2966">Unterstützung für `--namespace` zu `metrics list-definitions` hinzugefügt [Nr. 5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="0bba9-2966">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="0bba9-2967">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0bba9-2967">Network</span></span>

* <span data-ttu-id="0bba9-2968">Unterstützung für private DNS-Zonen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2968">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="0bba9-2969">Profil</span><span class="sxs-lookup"><span data-stu-id="0bba9-2969">Profile</span></span>

* <span data-ttu-id="0bba9-2970">Warnung für `--identity-port` und `--msi-port` zu `login` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2970">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="0bba9-2971">RDBMS</span><span class="sxs-lookup"><span data-stu-id="0bba9-2971">RDBMS</span></span>

* <span data-ttu-id="0bba9-2972">GA-API-Version 2017-12-01 (Geschäftsmodell) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2972">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="0bba9-2973">Resource</span><span class="sxs-lookup"><span data-stu-id="0bba9-2973">Resource</span></span>

* [BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="0bba9-2975">Role</span><span class="sxs-lookup"><span data-stu-id="0bba9-2975">Role</span></span>

* <span data-ttu-id="0bba9-2976">Unterstützung für erforderliche Zugriffskonfigurationen und native Clients zu `az ad app create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2976">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="0bba9-2977">`rbac`-Befehle geändert, um maximal 1.000 IDs für Objektauflösung zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="0bba9-2977">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="0bba9-2978">Befehle zur Verwaltung von Anmeldeinformationen (`ad sp credential [reset|list|delete]`) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2978">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="0bba9-2979">[BREAKING CHANGE] „properties“ aus `az role assignment [list|show]`-Ausgabe entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2979">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="0bba9-2980">Unterstützung für `dataActions`- und `notDataActions`-Berechtigungen zu `role definition` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2980">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="0bba9-2981">Storage</span><span class="sxs-lookup"><span data-stu-id="0bba9-2981">Storage</span></span>

* <span data-ttu-id="0bba9-2982">Problem beim Hochladen von Dateien mit einer Größe von 195 GB bis 200 GB behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-2982">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="0bba9-2983">[#4049](https://github.com/Azure/azure-cli/issues/4049) behoben: Probleme bei Uploads von Anfügeblobs behoben, die ein Ignorieren der Bedingungsparameter verursacht haben</span><span class="sxs-lookup"><span data-stu-id="0bba9-2983">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="0bba9-2984">VM</span><span class="sxs-lookup"><span data-stu-id="0bba9-2984">VM</span></span>

* <span data-ttu-id="0bba9-2985">Warnung für anstehende BREAKING CHANGEen für Sätze mit mehr als 100 Instanzen zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2985">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="0bba9-2986">Unterstützung der Zonenresilienz zu `vm [snapshot|image]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2986">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="0bba9-2987">Datenträgerinstanzansicht geändert, um besseren Verschlüsselungsstatus zu melden</span><span class="sxs-lookup"><span data-stu-id="0bba9-2987">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="0bba9-2988">[BREAKING CHANGE]`vm extension delete` geändert, um keine Ausgabe mehr zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="0bba9-2988">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="0bba9-2989">13. März 2018</span><span class="sxs-lookup"><span data-stu-id="0bba9-2989">March 13, 2018</span></span>

<span data-ttu-id="0bba9-2990">Version 2.0.29</span><span class="sxs-lookup"><span data-stu-id="0bba9-2990">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="0bba9-2991">ACR</span><span class="sxs-lookup"><span data-stu-id="0bba9-2991">ACR</span></span>

* <span data-ttu-id="0bba9-2992">Unterstützung für den Parameter `--image` zu `repository delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2992">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="0bba9-2993">Parameter `--manifest` und `--tag` des Befehls `repository delete` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-2993">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="0bba9-2994">Befehl `repository untag` zum Entfernen eines Tags ohne das Löschen von Daten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2994">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="0bba9-2995">ACS</span><span class="sxs-lookup"><span data-stu-id="0bba9-2995">ACS</span></span>

* <span data-ttu-id="0bba9-2996">Befehl `aks upgrade-connector` zum Aktualisieren eines vorhandenen Connectors hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2996">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="0bba9-2997">`kubectl`-Konfigurationsdateien zur Verwendung von besser lesbarem YAML im Blockstil geändert</span><span class="sxs-lookup"><span data-stu-id="0bba9-2997">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="0bba9-2998">Advisor</span><span class="sxs-lookup"><span data-stu-id="0bba9-2998">Advisor</span></span>

* <span data-ttu-id="0bba9-2999">[BREAKING CHANGE]`advisor configuration get` in `advisor configuration list` umbenannt</span><span class="sxs-lookup"><span data-stu-id="0bba9-2999">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="0bba9-3000">[BREAKING CHANGE]`advisor configuration set` in `advisor configuration update` umbenannt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3000">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="0bba9-3001">[BREAKING CHANGE]`advisor recommendation generate` entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3001">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="0bba9-3002">Parameter `--refresh` zu `advisor recommendation list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3002">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="0bba9-3003">Befehl `advisor recommendation show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3003">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="0bba9-3004">AppService</span><span class="sxs-lookup"><span data-stu-id="0bba9-3004">Appservice</span></span>

* <span data-ttu-id="0bba9-3005">`[webapp|functionapp] assign-identity` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-3005">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="0bba9-3006">Befehle `webapp identity [assign|show]` und `functionapp identity [assign|show]` für verwaltete Identität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3006">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="0bba9-3007">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="0bba9-3007">Eventhubs</span></span>

* <span data-ttu-id="0bba9-3008">Erste Veröffentlichung</span><span class="sxs-lookup"><span data-stu-id="0bba9-3008">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="0bba9-3009">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="0bba9-3009">Extension</span></span>

* <span data-ttu-id="0bba9-3010">Überprüfung zum Warnen von Benutzern hinzugefügt, wenn sich die verwendete Distribution von der in der Paketquelldatei gespeicherten Distribution unterscheidet, da dies Fehlern führen kann</span><span class="sxs-lookup"><span data-stu-id="0bba9-3010">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="0bba9-3011">Interactive</span><span class="sxs-lookup"><span data-stu-id="0bba9-3011">Interactive</span></span>

* <span data-ttu-id="0bba9-3012">[#5625](https://github.com/Azure/azure-cli/issues/5625) behoben: Verlauf über verschiedene Sitzungen hinweg beibehalten</span><span class="sxs-lookup"><span data-stu-id="0bba9-3012">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="0bba9-3013">[#3016](https://github.com/Azure/azure-cli/issues/3016) behoben: Verlauf nicht aufgezeichnet, obwohl er innerhalb des Bereichs liegt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3013">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="0bba9-3014">[#5688](https://github.com/Azure/azure-cli/issues/5688) behoben: Abschlüsse wurden nicht angezeigt, wenn beim Laden der Befehlstabelle eine Ausnahme aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="0bba9-3014">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="0bba9-3015">Statusanzeige für lang ausgeführte Vorgänge korrigiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-3015">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="0bba9-3016">Überwachen</span><span class="sxs-lookup"><span data-stu-id="0bba9-3016">Monitor</span></span>

* <span data-ttu-id="0bba9-3017">`monitor autoscale-settings`-Befehle als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-3017">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="0bba9-3018">Befehle vom Typ `monitor autoscale` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3018">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="0bba9-3019">Befehle vom Typ `monitor autoscale profile` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3019">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="0bba9-3020">Befehle vom Typ `monitor autoscale rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3020">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="0bba9-3021">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0bba9-3021">Network</span></span>

* <span data-ttu-id="0bba9-3022">[BREAKING CHANGE] Parameter `--tags` aus `route-filter rule create` entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3022">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="0bba9-3023">Einige fehlerhafte Standardwerte für die folgenden Befehle entfernt:</span><span class="sxs-lookup"><span data-stu-id="0bba9-3023">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="0bba9-3024">`network watcher connection-monitor`-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3024">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="0bba9-3025">Parameter `--vnet` und `--subnet` zu `network watcher show-topology` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3025">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="0bba9-3026">Profil</span><span class="sxs-lookup"><span data-stu-id="0bba9-3026">Profile</span></span>

* <span data-ttu-id="0bba9-3027">Parameter `--msi` für `az login` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-3027">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="0bba9-3028">Parameter `--identity` für `az login` als Ersatz vor `--msi` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3028">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="0bba9-3029">RDBMS</span><span class="sxs-lookup"><span data-stu-id="0bba9-3029">RDBMS</span></span>

* <span data-ttu-id="0bba9-3030">[VORSCHAU] Geändert, sodass die API „2017-12-01-preview“ verwendet wird</span><span class="sxs-lookup"><span data-stu-id="0bba9-3030">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="0bba9-3031">Service Bus</span><span class="sxs-lookup"><span data-stu-id="0bba9-3031">Service Bus</span></span>

* <span data-ttu-id="0bba9-3032">Erste Veröffentlichung</span><span class="sxs-lookup"><span data-stu-id="0bba9-3032">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="0bba9-3033">Storage</span><span class="sxs-lookup"><span data-stu-id="0bba9-3033">Storage</span></span>

* <span data-ttu-id="0bba9-3034">[#4971](https://github.com/Azure/azure-cli/issues/4971) behoben: `storage blob copy` unterstützt jetzt andere Azure-Clouds.</span><span class="sxs-lookup"><span data-stu-id="0bba9-3034">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="0bba9-3035">[#5286](https://github.com/Azure/azure-cli/issues/5286) behoben: Batchbefehle `storage blob [delete-batch|download-batch|upload-batch]` lösen bei Vorbedingungsfehlern keinen Fehler mehr aus</span><span class="sxs-lookup"><span data-stu-id="0bba9-3035">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="0bba9-3036">VM</span><span class="sxs-lookup"><span data-stu-id="0bba9-3036">VM</span></span>

* <span data-ttu-id="0bba9-3037">`[vm|vmss] create` unterstützt jetzt das Anfügen nicht verwalteter Datenträger und das Konfigurieren der Zwischenspeicherung.</span><span class="sxs-lookup"><span data-stu-id="0bba9-3037">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="0bba9-3038">`[vm|vmss] assign-identity` und `[vm|vmss] remove-identity` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-3038">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="0bba9-3039">Befehle `vm identity [assign|remove|show]` und `vmss identity [assign|remove|show]` als Ersatz für veraltete Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3039">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="0bba9-3040">Standardpriorität in `vmss create` auf „Keine“ geändert</span><span class="sxs-lookup"><span data-stu-id="0bba9-3040">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="0bba9-3041">27. Februar 2018</span><span class="sxs-lookup"><span data-stu-id="0bba9-3041">February 27, 2018</span></span>

<span data-ttu-id="0bba9-3042">Version 2.0.28</span><span class="sxs-lookup"><span data-stu-id="0bba9-3042">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="0bba9-3043">Core</span><span class="sxs-lookup"><span data-stu-id="0bba9-3043">Core</span></span>

* <span data-ttu-id="0bba9-3044">[#5184](https://github.com/Azure/azure-cli/issues/5184) behoben: Problem beim Installieren von Homebrew</span><span class="sxs-lookup"><span data-stu-id="0bba9-3044">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="0bba9-3045">Unterstützung für Erweiterungstelemetrie mit benutzerdefinierten Schlüsseln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3045">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="0bba9-3046">HTTP-Protokollierung zu `--debug` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3046">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="0bba9-3047">ACS</span><span class="sxs-lookup"><span data-stu-id="0bba9-3047">ACS</span></span>

* <span data-ttu-id="0bba9-3048">Geändert, sodass für `aks install-connector` standardmäßig das Helm-Diagramm `virtual-kubelet-for-aks` verwendet wird</span><span class="sxs-lookup"><span data-stu-id="0bba9-3048">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="0bba9-3049">Problem behoben: Unzureichende Berechtigungen für Dienstprinzipale zum Erstellen einer ACI-Containergruppe</span><span class="sxs-lookup"><span data-stu-id="0bba9-3049">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="0bba9-3050">Parameter `--aci-container-group`, `--location` und `--image-tag` zu `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3050">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="0bba9-3051">Veraltungshinweis aus `aks get-versions` entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3051">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="0bba9-3052">AppService</span><span class="sxs-lookup"><span data-stu-id="0bba9-3052">Appservice</span></span>

* <span data-ttu-id="0bba9-3053">Updates für die neue SDK-Version (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="0bba9-3053">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="0bba9-3054">[5538](https://github.com/Azure/azure-cli/issues/5538) behoben: `Free` wurde als ungültige SKU gemeldet.</span><span class="sxs-lookup"><span data-stu-id="0bba9-3054">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="0bba9-3055">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="0bba9-3055">Cognitive Services</span></span>

* <span data-ttu-id="0bba9-3056">Hinweis beim Erstellen eines neuen Cognitive Services-Kontos aktualisiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-3056">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="0bba9-3057">Nutzung</span><span class="sxs-lookup"><span data-stu-id="0bba9-3057">Consumption</span></span>

* <span data-ttu-id="0bba9-3058">Neue Befehle für PriceSheet-API hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3058">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="0bba9-3059">Vorhandene Formate für Nutzungsdetails und Reservierungsdetails aktualisiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-3059">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="0bba9-3060">Container</span><span class="sxs-lookup"><span data-stu-id="0bba9-3060">Container</span></span>

* <span data-ttu-id="0bba9-3061">Argumente `--secrets` und `--secrets-mount-path` zu `container create` hinzugefügt, um Geheimnisse in ACI verwenden zu können</span><span class="sxs-lookup"><span data-stu-id="0bba9-3061">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="0bba9-3062">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0bba9-3062">Network</span></span>

* <span data-ttu-id="0bba9-3063">[#5559](https://github.com/Azure/azure-cli/issues/5559) behoben: Fehlender Client in `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="0bba9-3063">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="0bba9-3064">Resource</span><span class="sxs-lookup"><span data-stu-id="0bba9-3064">Resource</span></span>

* <span data-ttu-id="0bba9-3065">`group deployment export` geändert, um eine partielle Vorlage und ggf. Fehler anzuzeigen, wenn der Vorgang nicht erfolgreich war</span><span class="sxs-lookup"><span data-stu-id="0bba9-3065">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="0bba9-3066">Role</span><span class="sxs-lookup"><span data-stu-id="0bba9-3066">Role</span></span>

* <span data-ttu-id="0bba9-3067">`role assignment list-changelogs` hinzugefügt, um die Überprüfung von Dienstprinzipalrollen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="0bba9-3067">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="0bba9-3068">SQL</span><span class="sxs-lookup"><span data-stu-id="0bba9-3068">SQL</span></span>

* <span data-ttu-id="0bba9-3069">Zonenredundanzunterstützung für Datenbanken und Pools für elastische Datenbanken hinzugefügt (bei Erstellung und Aktualisierung)</span><span class="sxs-lookup"><span data-stu-id="0bba9-3069">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="0bba9-3070">Storage</span><span class="sxs-lookup"><span data-stu-id="0bba9-3070">Storage</span></span>

* <span data-ttu-id="0bba9-3071">Angabe von Zielpfad/Präfix für `storage blob [upload-batch|download-batch]` ermöglicht</span><span class="sxs-lookup"><span data-stu-id="0bba9-3071">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="0bba9-3072">VM</span><span class="sxs-lookup"><span data-stu-id="0bba9-3072">VM</span></span>

* <span data-ttu-id="0bba9-3073">Unterstützung für das Anfügen/Trennen von Datenträgern für eine einzelne VMSS-Instanz hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3073">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="0bba9-3074">13. Februar 2018</span><span class="sxs-lookup"><span data-stu-id="0bba9-3074">February 13, 2018</span></span>

<span data-ttu-id="0bba9-3075">Version 2.0.27</span><span class="sxs-lookup"><span data-stu-id="0bba9-3075">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="0bba9-3076">Core</span><span class="sxs-lookup"><span data-stu-id="0bba9-3076">Core</span></span>

* <span data-ttu-id="0bba9-3077">Authentifizierung für Abonnement-ID und Namen bei der MSI-Anmeldung in Authentifizierung mit Schlüssel geändert</span><span class="sxs-lookup"><span data-stu-id="0bba9-3077">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="0bba9-3078">ACS</span><span class="sxs-lookup"><span data-stu-id="0bba9-3078">ACS</span></span>

* <span data-ttu-id="0bba9-3079">[BREAKING CHANGE]`aks get-versions` aus Gründen der Genauigkeit in `aks get-upgrades` umbenannt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3079">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="0bba9-3080">`aks get-versions` zur Anzeige der verfügbaren Kubernetes-Versionen für `aks create` geändert</span><span class="sxs-lookup"><span data-stu-id="0bba9-3080">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="0bba9-3081">Standardwerte von `aks create` in Auswahl der Kubernetes-Version durch den Server geändert</span><span class="sxs-lookup"><span data-stu-id="0bba9-3081">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="0bba9-3082">Hilfemeldungen zu dem von AKS generierten Dienstprinzipal aktualisiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-3082">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="0bba9-3083">Standardknotengrößen für `aks create` von „Standard\_D1\_v2“ in „Standard\_DS1\_v2“ geändert</span><span class="sxs-lookup"><span data-stu-id="0bba9-3083">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="0bba9-3084">Zuverlässigkeit der Suche nach dem Dashboardpod für `az aks browse` verbessert</span><span class="sxs-lookup"><span data-stu-id="0bba9-3084">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="0bba9-3085">`aks get-credentials` korrigiert, um Unicode-Fehler beim Laden von Kubernetes-Konfigurationsdateien zu behandeln</span><span class="sxs-lookup"><span data-stu-id="0bba9-3085">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="0bba9-3086">Meldung zu `az aks install-cli` hinzugefügt, um das Abrufen von `kubectl` in `$PATH` zu erleichtern</span><span class="sxs-lookup"><span data-stu-id="0bba9-3086">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="0bba9-3087">AppService</span><span class="sxs-lookup"><span data-stu-id="0bba9-3087">Appservice</span></span>

* <span data-ttu-id="0bba9-3088">Problem behoben, das zu einem Fehler von `webapp [backup|restore]` aufgrund eines Nullverweises führte</span><span class="sxs-lookup"><span data-stu-id="0bba9-3088">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="0bba9-3089">Unterstützung für Standard-App Service-Pläne durch `az configure --defaults appserviceplan=my-asp` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3089">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="0bba9-3090">CDN</span><span class="sxs-lookup"><span data-stu-id="0bba9-3090">CDN</span></span>

* <span data-ttu-id="0bba9-3091">Befehle vom Typ `cdn custom-domain [enable-https|disable-https]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3091">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="0bba9-3092">Container</span><span class="sxs-lookup"><span data-stu-id="0bba9-3092">Container</span></span>

* <span data-ttu-id="0bba9-3093">Option `--follow` zu `az container logs` für Streamingprotokolle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3093">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="0bba9-3094">Befehl `container attach` hinzugefügt, der die lokale Standardausgabe und Fehlerdatenströme an einen Container in einer Containergruppe angefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3094">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="0bba9-3095">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="0bba9-3095">CosmosDB</span></span>

* <span data-ttu-id="0bba9-3096">Unterstützung für Einstellungsfunktionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3096">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="0bba9-3097">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="0bba9-3097">Extension</span></span>

* <span data-ttu-id="0bba9-3098">Unterstützung für den Parameter `--pip-proxy` zu Befehlen vom Typ `az extension [add|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3098">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="0bba9-3099">Unterstützung für das Argument `--pip-extra-index-urls` zu Befehlen vom Typ `az extension [add|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3099">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="0bba9-3100">Feedback</span><span class="sxs-lookup"><span data-stu-id="0bba9-3100">Feedback</span></span>

* <span data-ttu-id="0bba9-3101">Erweiterungsinformationen zu Telemetriedaten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3101">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="0bba9-3102">Interactive</span><span class="sxs-lookup"><span data-stu-id="0bba9-3102">Interactive</span></span>

* <span data-ttu-id="0bba9-3103">Problem behoben, aufgrund dessen der Benutzer bei Verwendung des interaktiven Modus in Cloud Shell zur Anmeldung aufgefordert wird</span><span class="sxs-lookup"><span data-stu-id="0bba9-3103">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="0bba9-3104">Regression mit fehlenden Parametervervollständigungen korrigiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-3104">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="0bba9-3105">IoT</span><span class="sxs-lookup"><span data-stu-id="0bba9-3105">IoT</span></span>

* <span data-ttu-id="0bba9-3106">Problem behoben, aufgrund dessen `iot dps access policy [create|update]` bei erfolgreicher Ausführung einen Fehler „nicht gefunden“ zurückgibt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3106">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="0bba9-3107">Problem behoben, aufgrund dessen `iot dps linked-hub [create|update]` bei erfolgreicher Ausführung einen Fehler „nicht gefunden“ zurückgibt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3107">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="0bba9-3108">Unterstützung für `--no-wait` zu `iot dps access policy [create|update]` und `iot dps linked-hub [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3108">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="0bba9-3109">`iot hub create` geändert, um die Angabe der Anzahl von Partitionen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="0bba9-3109">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="0bba9-3110">Überwachen</span><span class="sxs-lookup"><span data-stu-id="0bba9-3110">Monitor</span></span>

* <span data-ttu-id="0bba9-3111">Befehl `az monitor log-profiles create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-3111">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="0bba9-3112">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0bba9-3112">Network</span></span>

* <span data-ttu-id="0bba9-3113">Option `--tags` für folgende Befehle korrigiert:</span><span class="sxs-lookup"><span data-stu-id="0bba9-3113">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="0bba9-3114">Profil</span><span class="sxs-lookup"><span data-stu-id="0bba9-3114">Profile</span></span>

* <span data-ttu-id="0bba9-3115">`az login` im interaktiven Modus aktiviert</span><span class="sxs-lookup"><span data-stu-id="0bba9-3115">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="0bba9-3116">Resource</span><span class="sxs-lookup"><span data-stu-id="0bba9-3116">Resource</span></span>

* <span data-ttu-id="0bba9-3117">`feature show` wieder hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3117">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="0bba9-3118">Role</span><span class="sxs-lookup"><span data-stu-id="0bba9-3118">Role</span></span>

* <span data-ttu-id="0bba9-3119">Argument `--available-to-other-tenants` zu `ad app update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3119">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="0bba9-3120">SQL</span><span class="sxs-lookup"><span data-stu-id="0bba9-3120">SQL</span></span>

* <span data-ttu-id="0bba9-3121">Befehle vom Typ `sql server dns-alias` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3121">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="0bba9-3122">`sql db rename` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3122">Added `sql db rename`</span></span>
* <span data-ttu-id="0bba9-3123">Unterstützung für das Argument `--ids` für alle SQL-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3123">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="0bba9-3124">Storage</span><span class="sxs-lookup"><span data-stu-id="0bba9-3124">Storage</span></span>

* <span data-ttu-id="0bba9-3125">Befehle `storage blob service-properties delete-policy` und `storage blob undelete` hinzugefügt, um vorläufiges Löschen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="0bba9-3125">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="0bba9-3126">VM</span><span class="sxs-lookup"><span data-stu-id="0bba9-3126">VM</span></span>

* <span data-ttu-id="0bba9-3127">Absturz bei unvollständiger Initialisierung der VM-Verschlüsselung behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-3127">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="0bba9-3128">Prinzipal-ID-Ausgabe beim Aktivieren von MSI hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3128">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="0bba9-3129">`vm boot-diagnostics get-boot-log` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="0bba9-3129">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="0bba9-3130">31. Januar 2018</span><span class="sxs-lookup"><span data-stu-id="0bba9-3130">January 31, 2018</span></span>

<span data-ttu-id="0bba9-3131">Version 2.0.26</span><span class="sxs-lookup"><span data-stu-id="0bba9-3131">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="0bba9-3132">Core</span><span class="sxs-lookup"><span data-stu-id="0bba9-3132">Core</span></span>

* <span data-ttu-id="0bba9-3133">Unterstützung für das Abrufen von unformatierten Token im MSI-Kontext hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3133">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="0bba9-3134">Abrufindikator-Zeichenfolge nach Fertigstellung von LRO für die Windows-Datei „cmd.exe“ entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3134">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="0bba9-3135">Warnung hinzugefügt, die angezeigt wird, wenn ein konfigurierter Standardwert in einen Eintrag auf INFO-Ebene geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="0bba9-3135">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="0bba9-3136">`--verbose` zum Anzeigen verwenden.</span><span class="sxs-lookup"><span data-stu-id="0bba9-3136">Use `--verbose` to see</span></span>
* <span data-ttu-id="0bba9-3137">Statusanzeige für Wait-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3137">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="0bba9-3138">ACS</span><span class="sxs-lookup"><span data-stu-id="0bba9-3138">ACS</span></span>

* <span data-ttu-id="0bba9-3139">Argument `--disable-browser` erläutert</span><span class="sxs-lookup"><span data-stu-id="0bba9-3139">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="0bba9-3140">Vervollständigung mit der TAB-TASTE für Argumente vom Typ `--vm-size` verbessert</span><span class="sxs-lookup"><span data-stu-id="0bba9-3140">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="0bba9-3141">AppService</span><span class="sxs-lookup"><span data-stu-id="0bba9-3141">Appservice</span></span>

* <span data-ttu-id="0bba9-3142">`webapp log [tail|download]` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="0bba9-3142">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="0bba9-3143">Überprüfung `kind` für Web-Apps und Funktionen entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3143">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="0bba9-3144">CDN</span><span class="sxs-lookup"><span data-stu-id="0bba9-3144">CDN</span></span>

* <span data-ttu-id="0bba9-3145">Problem mit fehlendem Client für `cdn custom-domain create` behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-3145">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="0bba9-3146">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="0bba9-3146">CosmosDB</span></span>

* <span data-ttu-id="0bba9-3147">Parameterbeschreibung für Failoverrichtlinien korrigiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-3147">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="0bba9-3148">Interactive</span><span class="sxs-lookup"><span data-stu-id="0bba9-3148">Interactive</span></span>

* <span data-ttu-id="0bba9-3149">Problem behoben, aufgrund dessen Vervollständigungen von Befehlsoptionen nicht mehr angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="0bba9-3149">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="0bba9-3150">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0bba9-3150">Network</span></span>

* <span data-ttu-id="0bba9-3151">Schutz für `--cert-password` zu `application-gateway create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3151">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="0bba9-3152">Problem mit `application-gateway update` behoben, aufgrund dessen `--sku` fälschlicherweise einen Standardwert anwendete</span><span class="sxs-lookup"><span data-stu-id="0bba9-3152">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="0bba9-3153">Schutz für `--shared-key` und `--authorization-key` zu `vpn-connection create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3153">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="0bba9-3154">Problem mit fehlendem Client für `asg create` behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-3154">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="0bba9-3155">Parameter `--file-name / -f` für exportierte Namen zu `dns zone export` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3155">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="0bba9-3156">Folgende Probleme mit `dns zone export` behoben:</span><span class="sxs-lookup"><span data-stu-id="0bba9-3156">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="0bba9-3157">Problem behoben, aufgrund dessen lange TXT-Einträge nicht korrekt exportiert wurden</span><span class="sxs-lookup"><span data-stu-id="0bba9-3157">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="0bba9-3158">Problem behoben, aufgrund dessen TXT-Einträge in Anführungszeichen fälschlich ohne Anführungszeichen in Escapezeichen exportiert wurden</span><span class="sxs-lookup"><span data-stu-id="0bba9-3158">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="0bba9-3159">Problem behoben, aufgrund dessen bestimmte Datensätze zweimal mit `dns zone import` importiert wurden</span><span class="sxs-lookup"><span data-stu-id="0bba9-3159">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="0bba9-3160">Befehle `vnet-gateway root-cert` und `vnet-gateway revoked-cert` wiederhergestellt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3160">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="0bba9-3161">Profil</span><span class="sxs-lookup"><span data-stu-id="0bba9-3161">Profile</span></span>

* <span data-ttu-id="0bba9-3162">`get-access-token` zur Verwendung auf einer VM mit Identität korrigiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-3162">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="0bba9-3163">Resource</span><span class="sxs-lookup"><span data-stu-id="0bba9-3163">Resource</span></span>

* <span data-ttu-id="0bba9-3164">Fehler mit `deployment [create|validate]` korrigiert, aufgrund dessen fälschlich eine Warnung angezeigt wurde, wenn ein Vorlagenfeld „Typ“ Werte in Großbuchstaben enthielt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3164">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="0bba9-3165">Storage</span><span class="sxs-lookup"><span data-stu-id="0bba9-3165">Storage</span></span>

* <span data-ttu-id="0bba9-3166">Problem mit der Migration von Storage V1-Konten zu Storage V2 behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-3166">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="0bba9-3167">Statusberichterstellung für alle Upload-/Downloadbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3167">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="0bba9-3168">Fehler korrigiert, der die Verwendung der arg-Option „-n“ mit `storage account check-name` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="0bba9-3168">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="0bba9-3169">Spalte „Momentaufnahme“ zur Tabellenausgabe für `blob [list|show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3169">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="0bba9-3170">Fehler mit verschiedenen Parametern korrigiert, die als Int-Typen analysiert werden mussten</span><span class="sxs-lookup"><span data-stu-id="0bba9-3170">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="0bba9-3171">VM</span><span class="sxs-lookup"><span data-stu-id="0bba9-3171">VM</span></span>

* <span data-ttu-id="0bba9-3172">Befehl `vm image accept-terms` hinzugefügt, um die Erstellung von VMs aus Images mit zusätzlichen Gebühren zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="0bba9-3172">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="0bba9-3173">`[vm|vmss create]` korrigiert, um sicherzustellen, dass Befehle unter einem Proxy mit nicht signierten Zertifikaten ausgeführt werden können</span><span class="sxs-lookup"><span data-stu-id="0bba9-3173">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="0bba9-3174">[VORSCHAU] Unterstützung für „niedrige“ Priorität zu VMSS hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3174">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="0bba9-3175">Schutz für `--admin-password` zu `[vm|vmss] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3175">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="0bba9-3176">17. Januar 2018</span><span class="sxs-lookup"><span data-stu-id="0bba9-3176">January 17, 2018</span></span>

<span data-ttu-id="0bba9-3177">Version 2.0.25</span><span class="sxs-lookup"><span data-stu-id="0bba9-3177">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="0bba9-3178">ACR</span><span class="sxs-lookup"><span data-stu-id="0bba9-3178">ACR</span></span>

* <span data-ttu-id="0bba9-3179">Fallback auf ACR-Anmeldung bei Fehlern mit Windows-Anmeldeinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3179">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="0bba9-3180">Registrierungsprotokolle aktiviert</span><span class="sxs-lookup"><span data-stu-id="0bba9-3180">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="0bba9-3181">ACS</span><span class="sxs-lookup"><span data-stu-id="0bba9-3181">ACS</span></span>

* <span data-ttu-id="0bba9-3182">Befehl `get-credentials` korrigiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-3182">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="0bba9-3183">SPN-Rollenanforderung entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3183">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="0bba9-3184">AppService</span><span class="sxs-lookup"><span data-stu-id="0bba9-3184">Appservice</span></span>

* <span data-ttu-id="0bba9-3185">Fehler mit `config ssl upload` behoben, bei dem `hosting_environment_profile` NULL war</span><span class="sxs-lookup"><span data-stu-id="0bba9-3185">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="0bba9-3186">Unterstützung benutzerdefinierter URLs zu `browse` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3186">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="0bba9-3187">Slotunterstützung für `log tail` korrigiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-3187">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="0bba9-3188">Backup</span><span class="sxs-lookup"><span data-stu-id="0bba9-3188">Backup</span></span>

* <span data-ttu-id="0bba9-3189">Option `--container-name` von `backup item list` geändert (ist jetzt optional)</span><span class="sxs-lookup"><span data-stu-id="0bba9-3189">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="0bba9-3190">Speicherkontooptionen zu `backup restore restore-disks` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3190">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="0bba9-3191">Standortüberprüfung in `backup protection enable-for-vm` korrigiert (Groß-/Kleinschreibung wird jetzt nicht mehr beachtet)</span><span class="sxs-lookup"><span data-stu-id="0bba9-3191">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="0bba9-3192">Problem behoben, durch das bei Befehlen mit ungültigem Containernamen ein Fehler auftrat</span><span class="sxs-lookup"><span data-stu-id="0bba9-3192">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="0bba9-3193">`backup item list` geändert (Integritätsstatus jetzt standardmäßig enthalten)</span><span class="sxs-lookup"><span data-stu-id="0bba9-3193">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="0bba9-3194">Batch</span><span class="sxs-lookup"><span data-stu-id="0bba9-3194">Batch</span></span>

* <span data-ttu-id="0bba9-3195">`batch login` geändert, um Authentifizierungsdetails zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="0bba9-3195">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="0bba9-3196">Cloud</span><span class="sxs-lookup"><span data-stu-id="0bba9-3196">Cloud</span></span>

* <span data-ttu-id="0bba9-3197">Beim Festlegen von `--profile` für eine Cloud werden nun keine Endpunkte mehr benötigt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-3197">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="0bba9-3198">Nutzung</span><span class="sxs-lookup"><span data-stu-id="0bba9-3198">Consumption</span></span>

* <span data-ttu-id="0bba9-3199">Neue Befehle für Reservierungen hinzugefügt: `consumption reservations summaries` und `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="0bba9-3199">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="0bba9-3200">Event Grid</span><span class="sxs-lookup"><span data-stu-id="0bba9-3200">Event Grid</span></span>

* <span data-ttu-id="0bba9-3201">[BREAKING CHANGE] Die Befehle vom Typ `az eventgrid topic event-subscription` wurden in `eventgrid event-subscription` verschoben.</span><span class="sxs-lookup"><span data-stu-id="0bba9-3201">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="0bba9-3202">[BREAKING CHANGE] Die Befehle vom Typ `az eventgrid resource event-subscription` wurden in `eventgrid event-subscription` verschoben.</span><span class="sxs-lookup"><span data-stu-id="0bba9-3202">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="0bba9-3203">[BREAKING CHANGE] Der Befehl `eventgrid event-subscription show-endpoint-url` wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-3203">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="0bba9-3204">Verwenden Sie stattdessen `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="0bba9-3204">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="0bba9-3205">Befehl `eventgrid topic update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3205">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="0bba9-3206">Befehl `eventgrid event-subscription update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3206">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="0bba9-3207">Parameter `--ids` für Befehle vom Typ `eventgrid topic` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3207">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="0bba9-3208">Unterstützung der Vervollständigung mit der TAB-TASTE für Themennamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3208">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="0bba9-3209">Interactive</span><span class="sxs-lookup"><span data-stu-id="0bba9-3209">Interactive</span></span>

* <span data-ttu-id="0bba9-3210">Problem behoben, das dazu führte, dass der interaktive Modus nicht mit Python 2.x verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="0bba9-3210">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="0bba9-3211">Fehler beim Start behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-3211">Fixed errors on startup</span></span>
* <span data-ttu-id="0bba9-3212">Problem behoben, das dazu führte, dass einige Befehle nicht im interaktiven Modus ausgeführt werden konnten</span><span class="sxs-lookup"><span data-stu-id="0bba9-3212">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="0bba9-3213">IoT</span><span class="sxs-lookup"><span data-stu-id="0bba9-3213">IoT</span></span>

* <span data-ttu-id="0bba9-3214">Unterstützung für Gerätebereitstellungsdienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3214">Added support for device provisioning service</span></span>
* <span data-ttu-id="0bba9-3215">Benachrichtigungen zu veralteten Elementen in Befehlen und in der Befehlshilfe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3215">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="0bba9-3216">IoT-Überprüfung hinzugefügt, um Benutzer über die IoT-Erweiterung zu informieren</span><span class="sxs-lookup"><span data-stu-id="0bba9-3216">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="0bba9-3217">Überwachen</span><span class="sxs-lookup"><span data-stu-id="0bba9-3217">Monitor</span></span>

* <span data-ttu-id="0bba9-3218">Unterstützung mehrerer Diagnoseeinstellung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-3218">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="0bba9-3219">Der Parameter `--name` ist nun für `az monitor diagnostic-settings create` erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0bba9-3219">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="0bba9-3220">Befehl `monitor diagnostic-settings categories` zum Abrufen der Diagnoseeinstellungskategorie hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3220">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="0bba9-3221">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0bba9-3221">Network</span></span>

* <span data-ttu-id="0bba9-3222">Problem behoben, das beim Ändern des aktiven Standbymodus mit `vnet-gateway update` auftrat</span><span class="sxs-lookup"><span data-stu-id="0bba9-3222">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="0bba9-3223">Unterstützung für HTTP2 zu `application-gateway [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3223">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="0bba9-3224">Profil</span><span class="sxs-lookup"><span data-stu-id="0bba9-3224">Profile</span></span>

* <span data-ttu-id="0bba9-3225">Unterstützung für die Anmeldung mit durch Benutzer zugewiesenen Identitäten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3225">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="0bba9-3226">Role</span><span class="sxs-lookup"><span data-stu-id="0bba9-3226">Role</span></span>

* <span data-ttu-id="0bba9-3227">Argument `--assignee-object-id` zu `role assignment create` hinzugefügt, um Graph-Abfrage zu umgehen</span><span class="sxs-lookup"><span data-stu-id="0bba9-3227">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="0bba9-3228">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="0bba9-3228">Service Fabric</span></span>

* <span data-ttu-id="0bba9-3229">Ausführliche Fehler zur Überprüfungsantwort bei der Clustererstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3229">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="0bba9-3230">Problem mit fehlendem Client für verschiedene Befehle behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-3230">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="0bba9-3231">VM</span><span class="sxs-lookup"><span data-stu-id="0bba9-3231">VM</span></span>

* <span data-ttu-id="0bba9-3232">[VORSCHAUVERSION] Zonenübergreifende Unterstützung für `vmss`</span><span class="sxs-lookup"><span data-stu-id="0bba9-3232">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="0bba9-3233">[BREAKING CHANGE] Standard für Einzelzone (`vmss`) in Standardlastenausgleich geändert</span><span class="sxs-lookup"><span data-stu-id="0bba9-3233">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="0bba9-3234">[BREAKING CHANGE]`externalIdentities` in `userAssignedIdentities` geändert für EMSI</span><span class="sxs-lookup"><span data-stu-id="0bba9-3234">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="0bba9-3235">[VORSCHAUVERSION] Unterstützung für Austausch des Betriebssystemdatenträgers hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3235">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="0bba9-3236">Unterstützung der Verwendung von VM-Images aus anderen Abonnements hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3236">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="0bba9-3237">Argumente `--plan-name`, `--plan-product`, `--plan-promotion-code` und `--plan-publisher` zu `[vm|vmss] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3237">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="0bba9-3238">Fehlerbedingte Probleme mit `[vm|vmss] create` behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-3238">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="0bba9-3239">Übermäßige Ressourcenverwendung durch `vm image list --all` behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-3239">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="0bba9-3240">19. Dezember 2017</span><span class="sxs-lookup"><span data-stu-id="0bba9-3240">December 19, 2017</span></span>

<span data-ttu-id="0bba9-3241">Version 2.0.23</span><span class="sxs-lookup"><span data-stu-id="0bba9-3241">Version 2.0.23</span></span>

* <span data-ttu-id="0bba9-3242">Unterstützung für die Anmeldung mit durch Benutzer zugewiesenen Identitäten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3242">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="0bba9-3243">Container</span><span class="sxs-lookup"><span data-stu-id="0bba9-3243">Container</span></span>

* <span data-ttu-id="0bba9-3244">Falsche Reihenfolge der Parameter für Containerprotokolle behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-3244">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="0bba9-3245">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0bba9-3245">Network</span></span>

* <span data-ttu-id="0bba9-3246">Argument `--disable-bgp-route-propagation` zu `route-table [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3246">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="0bba9-3247">Argument `--ip-tags` zu `public-ip [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3247">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="0bba9-3248">Storage</span><span class="sxs-lookup"><span data-stu-id="0bba9-3248">Storage</span></span>

* <span data-ttu-id="0bba9-3249">Unterstützung für Storage V2 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3249">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="0bba9-3250">VM</span><span class="sxs-lookup"><span data-stu-id="0bba9-3250">VM</span></span>

* <span data-ttu-id="0bba9-3251">[VORSCHAUVERSION] Unterstützung für durch Benutzer zugewiesene Identitäten für virtuelle Computer und VMSSs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3251">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="0bba9-3252">5\. Dezember 2017</span><span class="sxs-lookup"><span data-stu-id="0bba9-3252">December 5, 2017</span></span>

<span data-ttu-id="0bba9-3253">Version 2.0.22</span><span class="sxs-lookup"><span data-stu-id="0bba9-3253">Version 2.0.22</span></span>

* <span data-ttu-id="0bba9-3254">`az component`-Befehle wurden entfernt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-3254">Removed `az component` commands.</span></span> <span data-ttu-id="0bba9-3255">Verwenden Sie stattdessen `az extension`.</span><span class="sxs-lookup"><span data-stu-id="0bba9-3255">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="0bba9-3256">Core</span><span class="sxs-lookup"><span data-stu-id="0bba9-3256">Core</span></span>
* <span data-ttu-id="0bba9-3257">Der `AZURE_US_GOV_CLOUD`-Autoritätsendpunkt von AAD wurde von „login.microsoftonline.com“ in „login.microsoftonline.us“ geändert.</span><span class="sxs-lookup"><span data-stu-id="0bba9-3257">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="0bba9-3258">Problem behoben, aufgrund dessen Telemetriedaten fortlaufend neu gesendet wurden</span><span class="sxs-lookup"><span data-stu-id="0bba9-3258">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="0bba9-3259">ACS</span><span class="sxs-lookup"><span data-stu-id="0bba9-3259">ACS</span></span>

* <span data-ttu-id="0bba9-3260">Die Befehle `aks install-connector` und `aks remove-connector` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-3260">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="0bba9-3261">Verbesserte Fehlerberichterstellung für `acs create`</span><span class="sxs-lookup"><span data-stu-id="0bba9-3261">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="0bba9-3262">Feste Verwendung von `aks get-credentials -f` ohne vollqualifizierten Pfad</span><span class="sxs-lookup"><span data-stu-id="0bba9-3262">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="0bba9-3263">Advisor</span><span class="sxs-lookup"><span data-stu-id="0bba9-3263">Advisor</span></span>

* <span data-ttu-id="0bba9-3264">Erste Veröffentlichung</span><span class="sxs-lookup"><span data-stu-id="0bba9-3264">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="0bba9-3265">AppService</span><span class="sxs-lookup"><span data-stu-id="0bba9-3265">Appservice</span></span>

* <span data-ttu-id="0bba9-3266">Erstellung feststehender Zertifikatnamen mit `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="0bba9-3266">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="0bba9-3267">`webapp [list|show]` und `functionapp [list|show]` wurden verbessert, um die richtigen Apps anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="0bba9-3267">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="0bba9-3268">Standardwert für `WEBSITE_NODE_DEFAULT_VERSION` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3268">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="0bba9-3269">Nutzung</span><span class="sxs-lookup"><span data-stu-id="0bba9-3269">Consumption</span></span>

* <span data-ttu-id="0bba9-3270">Unterstützung für API-Version 2017-11-30 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3270">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="0bba9-3271">Container</span><span class="sxs-lookup"><span data-stu-id="0bba9-3271">Container</span></span>

* <span data-ttu-id="0bba9-3272">Feste Regression für Standardports</span><span class="sxs-lookup"><span data-stu-id="0bba9-3272">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="0bba9-3273">Überwachen</span><span class="sxs-lookup"><span data-stu-id="0bba9-3273">Monitor</span></span>

* <span data-ttu-id="0bba9-3274">Unterstützung mehrerer Dimensionen zu Metrikbefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3274">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="0bba9-3275">Resource</span><span class="sxs-lookup"><span data-stu-id="0bba9-3275">Resource</span></span>

* <span data-ttu-id="0bba9-3276">Argument `--include-response-body` zu `resource show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3276">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="0bba9-3277">Role</span><span class="sxs-lookup"><span data-stu-id="0bba9-3277">Role</span></span>

* <span data-ttu-id="0bba9-3278">Anzeige von Standardzuweisungen für „klassische“ Administratoren zu `role assignment list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3278">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="0bba9-3279">Unterstützung für das Hinzufügen (anstelle der Überschreibung) von Anmeldeinformationen zu `ad sp reset-credentials` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3279">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="0bba9-3280">Verbesserte Fehlerberichterstellung für `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="0bba9-3280">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="0bba9-3281">SQL</span><span class="sxs-lookup"><span data-stu-id="0bba9-3281">SQL</span></span>

* <span data-ttu-id="0bba9-3282">Die Befehle `sql db list-usages` und `sql db show-usage` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-3282">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="0bba9-3283">Die Befehle `sql server conn-policy show` und `sql server conn-policy update` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-3283">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="0bba9-3284">VM</span><span class="sxs-lookup"><span data-stu-id="0bba9-3284">VM</span></span>

* <span data-ttu-id="0bba9-3285">Zoneninformationen zu `az vm list-skus` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3285">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="0bba9-3286">14. November 2017</span><span class="sxs-lookup"><span data-stu-id="0bba9-3286">November 14, 2017</span></span>

<span data-ttu-id="0bba9-3287">Version 2.0.21</span><span class="sxs-lookup"><span data-stu-id="0bba9-3287">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="0bba9-3288">ACR</span><span class="sxs-lookup"><span data-stu-id="0bba9-3288">ACR</span></span>

* <span data-ttu-id="0bba9-3289">Unterstützung für das Erstellen von Webhooks in Replikationsregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3289">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="0bba9-3290">ACS</span><span class="sxs-lookup"><span data-stu-id="0bba9-3290">ACS</span></span>

* <span data-ttu-id="0bba9-3291">Formulierung in AKS von „Agent“ in „Knoten“ geändert</span><span class="sxs-lookup"><span data-stu-id="0bba9-3291">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="0bba9-3292">Option `--orchestrator-release` für `acs create` als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="0bba9-3292">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="0bba9-3293">VM-Standardgröße für AKS in `Standard_D1_v2` geändert</span><span class="sxs-lookup"><span data-stu-id="0bba9-3293">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="0bba9-3294">`az aks browse` für Windows korrigiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-3294">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="0bba9-3295">`az aks get-credentials` für Windows korrigiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-3295">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="0bba9-3296">AppService</span><span class="sxs-lookup"><span data-stu-id="0bba9-3296">Appservice</span></span>

* <span data-ttu-id="0bba9-3297">Bereitstellungsquelle `config-zip` für Web-Apps und Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3297">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="0bba9-3298">Option `--docker-container-logging` zu `az webapp log config` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3298">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="0bba9-3299">Option `storage` aus dem Parameter `--web-server-logging` von `az webapp log config` entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3299">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="0bba9-3300">Fehlermeldungen für `deployment user set` verbessert</span><span class="sxs-lookup"><span data-stu-id="0bba9-3300">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="0bba9-3301">Unterstützung für das Erstellen von Linux-Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3301">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="0bba9-3302">`list-locations` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="0bba9-3302">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="0bba9-3303">Batch</span><span class="sxs-lookup"><span data-stu-id="0bba9-3303">Batch</span></span>

* <span data-ttu-id="0bba9-3304">Fehler im Poolerstellungsbefehl korrigiert, der bei Verwendung einer Ressourcen-ID mit dem Flag `--image` aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="0bba9-3304">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="0bba9-3305">BatchAI</span><span class="sxs-lookup"><span data-stu-id="0bba9-3305">Batchai</span></span>

* <span data-ttu-id="0bba9-3306">Kurzoption (`-s`) für `--vm-size` zur Angabe der VM-Größe im Befehl `file-server create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3306">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="0bba9-3307">Argumente für Speicherkontoname und -schlüssel zum Parameter `cluster create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3307">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="0bba9-3308">Dokumentation für `job list-files` und `job stream-file` korrigiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-3308">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="0bba9-3309">Kurzoption (`-r`) für `--cluster-name` zur Angabe des Clusternamens im Befehl `job create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3309">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="0bba9-3310">Cloud</span><span class="sxs-lookup"><span data-stu-id="0bba9-3310">Cloud</span></span>

* <span data-ttu-id="0bba9-3311">`cloud [register|update]` geändert, um die Registrierung von Clouds ohne erforderliche Endpunkte zu verhindern</span><span class="sxs-lookup"><span data-stu-id="0bba9-3311">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="0bba9-3312">Container</span><span class="sxs-lookup"><span data-stu-id="0bba9-3312">Container</span></span>

* <span data-ttu-id="0bba9-3313">Unterstützung für das Öffnen mehrerer Ports hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3313">Added support to open multiple ports</span></span>
* <span data-ttu-id="0bba9-3314">Neustartrichtlinie für Containergruppen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3314">Added container group restart policy</span></span>
* <span data-ttu-id="0bba9-3315">Unterstützung zum Einbinden einer Azure-Dateifreigabe als Volume hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3315">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="0bba9-3316">Hilfedokumente aktualisiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-3316">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="0bba9-3317">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="0bba9-3317">Data Lake Analytics</span></span>

* <span data-ttu-id="0bba9-3318">`[job|account] list` geändert, um präzisere Informationen zu erhalten</span><span class="sxs-lookup"><span data-stu-id="0bba9-3318">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="0bba9-3319">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="0bba9-3319">Data Lake Store</span></span>

* <span data-ttu-id="0bba9-3320">`account list` geändert, um präzisere Informationen zu erhalten</span><span class="sxs-lookup"><span data-stu-id="0bba9-3320">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="0bba9-3321">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="0bba9-3321">Extension</span></span>

* <span data-ttu-id="0bba9-3322">`extension list-available` hinzugefügt, um das Auflisten offizieller Microsoft-Erweiterungen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="0bba9-3322">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="0bba9-3323">`--name` zu `extension [add|update]` hinzugefügt, um das Installieren von Erweiterungen nach Name zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="0bba9-3323">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="0bba9-3324">IoT</span><span class="sxs-lookup"><span data-stu-id="0bba9-3324">IoT</span></span>

* <span data-ttu-id="0bba9-3325">Unterstützung für Zertifizierungsstellen (CAs) und Zertifikatketten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3325">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="0bba9-3326">Überwachen</span><span class="sxs-lookup"><span data-stu-id="0bba9-3326">Monitor</span></span>

* <span data-ttu-id="0bba9-3327">Befehle vom Typ `activity-log alert` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3327">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="0bba9-3328">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0bba9-3328">Network</span></span>

* <span data-ttu-id="0bba9-3329">Unterstützung für CAA-DNS-Einträge hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3329">Added support for CAA DNS records</span></span>
* <span data-ttu-id="0bba9-3330">Problem behoben, durch das Endpunkte nicht mit `traffic-manager profile update` aktualisiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="0bba9-3330">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="0bba9-3331">Problem behoben, durch das `vnet update --dns-servers` je nach VNet-Erstellungsmethode nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="0bba9-3331">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="0bba9-3332">Problem behoben, durch das relative DNS-Namen durch `dns zone import` nicht korrekt importiert wurden</span><span class="sxs-lookup"><span data-stu-id="0bba9-3332">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="0bba9-3333">Reservations</span><span class="sxs-lookup"><span data-stu-id="0bba9-3333">Reservations</span></span>

* <span data-ttu-id="0bba9-3334">Erste Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="0bba9-3334">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="0bba9-3335">Resource</span><span class="sxs-lookup"><span data-stu-id="0bba9-3335">Resource</span></span>

* <span data-ttu-id="0bba9-3336">Unterstützung für Ressourcen-IDs zum Parameter `--resource` und Sperren auf Ressourcenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3336">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="0bba9-3337">SQL</span><span class="sxs-lookup"><span data-stu-id="0bba9-3337">SQL</span></span>

* <span data-ttu-id="0bba9-3338">Parameter `--ignore-missing-vnet-service-endpoint` zu `sql server vnet-rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3338">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="0bba9-3339">Storage</span><span class="sxs-lookup"><span data-stu-id="0bba9-3339">Storage</span></span>

* <span data-ttu-id="0bba9-3340">`storage account create` geändert, sodass die SKU `Standard_RAGRS` als Standard verwendet wird</span><span class="sxs-lookup"><span data-stu-id="0bba9-3340">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="0bba9-3341">Fehler im Zusammenhang mit Datei-/Blobnamen korrigiert, die ASCII-fremde Zeichen enthalten</span><span class="sxs-lookup"><span data-stu-id="0bba9-3341">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="0bba9-3342">Fehler korrigiert, der die Verwendung von `--source-uri` mit `storage [blob|file] copy start-batch` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="0bba9-3342">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="0bba9-3343">Befehle zum Globalisieren und Löschen mehrerer Objekte mit `storage [blob|file] delete-batch` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3343">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="0bba9-3344">Problem beim Aktivieren von Metriken mit `storage metrics update` behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-3344">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="0bba9-3345">Problem mit Dateien über 200 GB bei Verwendung von `storage blob upload-batch` behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-3345">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="0bba9-3346">Problem behoben, durch das `--bypass` und `--default-action` von `storage account [create|update]` ignoriert wurden</span><span class="sxs-lookup"><span data-stu-id="0bba9-3346">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="0bba9-3347">VM</span><span class="sxs-lookup"><span data-stu-id="0bba9-3347">VM</span></span>

* <span data-ttu-id="0bba9-3348">Fehler mit `vmss create` korrigiert, der die Verwendung der Größenebene `Basic` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="0bba9-3348">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="0bba9-3349">`--plan`-Argumente zu `[vm|vmss] create` für benutzerdefinierte Images mit Abrechnungsinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3349">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="0bba9-3350">Befehle hinzugefügt: `vm secret `[add|remove|list]</span><span class="sxs-lookup"><span data-stu-id="0bba9-3350">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="0bba9-3351">`vm format-secret` in `vm secret format` umbenannt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3351">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="0bba9-3352">Argument `--encrypt format` zu `vm encryption enable` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3352">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="0bba9-3353">24. Oktober 2017</span><span class="sxs-lookup"><span data-stu-id="0bba9-3353">October 24, 2017</span></span>

<span data-ttu-id="0bba9-3354">Version 2.0.20</span><span class="sxs-lookup"><span data-stu-id="0bba9-3354">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="0bba9-3355">Core</span><span class="sxs-lookup"><span data-stu-id="0bba9-3355">Core</span></span>

* <span data-ttu-id="0bba9-3356">Aktualisierung von `2017-03-09-profile` zur Verwendung von Version `2016-01-01` der `MGMT_STORAGE`-API</span><span class="sxs-lookup"><span data-stu-id="0bba9-3356">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="0bba9-3357">ACR</span><span class="sxs-lookup"><span data-stu-id="0bba9-3357">ACR</span></span>

* <span data-ttu-id="0bba9-3358">Die Ressourcenverwaltung wurde aktualisiert und verweist nun auf die API-Version `2017-10-01`.</span><span class="sxs-lookup"><span data-stu-id="0bba9-3358">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="0bba9-3359">SKU „Bring Your Own Storage“ wurde in „Klassisch“ geändert.</span><span class="sxs-lookup"><span data-stu-id="0bba9-3359">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="0bba9-3360">Die Registrierungs-SKUs wurden in „Basic“, „Standard“ und „Premium“ umbenannt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-3360">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="0bba9-3361">ACS</span><span class="sxs-lookup"><span data-stu-id="0bba9-3361">ACS</span></span>

* <span data-ttu-id="0bba9-3362">[VORSCHAUVERSION] Befehle vom Typ `az aks` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3362">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="0bba9-3363">Problem mit `get-credentials` in Kubernetes behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-3363">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="0bba9-3364">AppService</span><span class="sxs-lookup"><span data-stu-id="0bba9-3364">Appservice</span></span>

* <span data-ttu-id="0bba9-3365">Problem behoben, aufgrund dessen heruntergeladene `webapp`-Protokolle unter Umständen ungültig waren</span><span class="sxs-lookup"><span data-stu-id="0bba9-3365">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="0bba9-3366">Komponente</span><span class="sxs-lookup"><span data-stu-id="0bba9-3366">Component</span></span>

* <span data-ttu-id="0bba9-3367">Deutlichere Meldung zur Einstellung für alle Installer und für Bestätigungsaufforderung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3367">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="0bba9-3368">Überwachen</span><span class="sxs-lookup"><span data-stu-id="0bba9-3368">Monitor</span></span>

* <span data-ttu-id="0bba9-3369">Befehle vom Typ `action-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3369">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="0bba9-3370">Resource</span><span class="sxs-lookup"><span data-stu-id="0bba9-3370">Resource</span></span>

* <span data-ttu-id="0bba9-3371">Inkompatibilität mit der aktuellen Version der msrest-Abhängigkeit in `group export` behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-3371">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="0bba9-3372">Problem mit `policy assignment create` behoben, sodass der Befehl mit integrierten Richtliniendefinitionen und Richtliniensatzdefinitionen verwendet werden kann</span><span class="sxs-lookup"><span data-stu-id="0bba9-3372">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="0bba9-3373">VM</span><span class="sxs-lookup"><span data-stu-id="0bba9-3373">VM</span></span>

* <span data-ttu-id="0bba9-3374">Argument `--accelerated-networking` zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3374">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="0bba9-3375">9\. Oktober 2017</span><span class="sxs-lookup"><span data-stu-id="0bba9-3375">October 9, 2017</span></span>

<span data-ttu-id="0bba9-3376">Version 2.0.19</span><span class="sxs-lookup"><span data-stu-id="0bba9-3376">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="0bba9-3377">Core</span><span class="sxs-lookup"><span data-stu-id="0bba9-3377">Core</span></span>

* <span data-ttu-id="0bba9-3378">Verarbeitung von ADFS-Autoritäts-URLs wurde mit einem nachgestellten Schrägstrich zu Azure Stack hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-3378">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="0bba9-3379">AppService</span><span class="sxs-lookup"><span data-stu-id="0bba9-3379">Appservice</span></span>

* <span data-ttu-id="0bba9-3380">Mit dem neuen Befehl `webapp update` wurde ein allgemeines Update hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-3380">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="0bba9-3381">Batch</span><span class="sxs-lookup"><span data-stu-id="0bba9-3381">Batch</span></span>

* <span data-ttu-id="0bba9-3382">Aktualisierung auf Batch SDK 4.0.0</span><span class="sxs-lookup"><span data-stu-id="0bba9-3382">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="0bba9-3383">Die Option `--image` von „VirtualMachineConfiguration“ wurde aktualisiert, um zusätzlich zu „publish:offer:sku:version“ ARM-Imageverweise zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="0bba9-3383">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="0bba9-3384">Unterstützung für das neue CLI-Erweiterungsmodell für Batch-Erweiterungsbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3384">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="0bba9-3385">Batch-Unterstützung aus dem Komponentenmodell entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3385">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="0bba9-3386">BatchAI</span><span class="sxs-lookup"><span data-stu-id="0bba9-3386">Batchai</span></span>

* <span data-ttu-id="0bba9-3387">Erste Version des Batch KI-Moduls</span><span class="sxs-lookup"><span data-stu-id="0bba9-3387">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="0bba9-3388">KeyVault</span><span class="sxs-lookup"><span data-stu-id="0bba9-3388">Keyvault</span></span>

* <span data-ttu-id="0bba9-3389">Key Vault-Authentifizierungsproblem behoben, das bei Verwendung von ADFS in Azure Stack auftrat.</span><span class="sxs-lookup"><span data-stu-id="0bba9-3389">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="0bba9-3390">(#4448)</span><span class="sxs-lookup"><span data-stu-id="0bba9-3390">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="0bba9-3391">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0bba9-3391">Network</span></span>

* <span data-ttu-id="0bba9-3392">Das Argument `--server` von `application-gateway address-pool create` ist nun optional, sodass leere Adresspools zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="0bba9-3392">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="0bba9-3393">`traffic-manager` wurde aktualisiert, um aktuelle Features zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="0bba9-3393">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="0bba9-3394">Resource</span><span class="sxs-lookup"><span data-stu-id="0bba9-3394">Resource</span></span>

* <span data-ttu-id="0bba9-3395">Zusätzliche Unterstützung für `--resource-group/-g`-Optionen für Ressourcengruppennamen zu `group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3395">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="0bba9-3396">Befehle für `account lock` hinzugefügt, um die Verwendung mit Sperren auf Abonnementebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="0bba9-3396">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="0bba9-3397">Befehle für `group lock` hinzugefügt, um die Verwendung mit Sperren auf Gruppenebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="0bba9-3397">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="0bba9-3398">Befehle für `resource lock` hinzugefügt, um die Verwendung mit Sperren auf Ressourcenebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="0bba9-3398">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="0bba9-3399">Sql</span><span class="sxs-lookup"><span data-stu-id="0bba9-3399">Sql</span></span>

* <span data-ttu-id="0bba9-3400">Unterstützung für SQL Transparent Data Encryption (TDE) und TDE für Bring Your Own Key-Szenarien hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3400">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="0bba9-3401">Der Befehl `db list-deleted` und der Parameter `db restore --deleted-time` wurden hinzugefügt, um die Ermittlung und Wiederherstellung gelöschter Datenbanken zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="0bba9-3401">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="0bba9-3402">`db op list` und `db op cancel` wurden hinzugefügt, um das Auflisten und Abbrechen ausgeführter Vorgänge für eine Datenbank zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="0bba9-3402">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="0bba9-3403">Storage</span><span class="sxs-lookup"><span data-stu-id="0bba9-3403">Storage</span></span>

* <span data-ttu-id="0bba9-3404">Unterstützung für Momentaufnahme von Dateifreigaben hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3404">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="0bba9-3405">VM</span><span class="sxs-lookup"><span data-stu-id="0bba9-3405">Vm</span></span>

* <span data-ttu-id="0bba9-3406">Korrektur eines Fehlers in `vm show`, bei dem die Verwendung von `-d` in Verbindung mit fehlenden privaten IP-Adressen einen Absturz verursachte</span><span class="sxs-lookup"><span data-stu-id="0bba9-3406">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="0bba9-3407">[VORSCHAUVERSION] Unterstützung für paralleles Upgrade zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3407">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="0bba9-3408">Unterstützung für das Aktualisieren der Verschlüsselungseinstellungen mit `vm encryption enable` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3408">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="0bba9-3409">Parameter `--os-disk-size-gb` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3409">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="0bba9-3410">Parameter `--license-type` für Windows zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3410">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="0bba9-3411">22. September 2017</span><span class="sxs-lookup"><span data-stu-id="0bba9-3411">September 22, 2017</span></span>

<span data-ttu-id="0bba9-3412">Version 2.0.18</span><span class="sxs-lookup"><span data-stu-id="0bba9-3412">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="0bba9-3413">Resource</span><span class="sxs-lookup"><span data-stu-id="0bba9-3413">Resource</span></span>

* <span data-ttu-id="0bba9-3414">Unterstützung für das Anzeigen integrierter Richtliniendefinitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3414">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="0bba9-3415">Unterstützungsmodusparameter zum Erstellen von Richtliniendefinitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3415">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="0bba9-3416">Unterstützung für UI-Definitionen und -Vorlagen zu `managedapp definition create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3416">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="0bba9-3417">[BREAKING CHANGE] Der Ressourcentyp `managedapp` wurde von `appliances` in `applications` und von `applianceDefinitions` in `applicationDefinitions` geändert.</span><span class="sxs-lookup"><span data-stu-id="0bba9-3417">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="0bba9-3418">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0bba9-3418">Network</span></span>

* <span data-ttu-id="0bba9-3419">Unterstützung für Verfügbarkeitszone zu Unterbefehlen `network lb` und `network public-ip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3419">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="0bba9-3420">Unterstützung für IPv6-Microsoft-Peering zu `express-route` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3420">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="0bba9-3421">Befehle für Anwendungssicherheitsgruppe `asg` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3421">Added `asg` application security group commands</span></span>
* <span data-ttu-id="0bba9-3422">Argument `--application-security-groups` zu `nic [create|ip-config create|ip-config update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3422">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="0bba9-3423">Argumente `--source-asgs` und `--destination-asgs` zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3423">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="0bba9-3424">Argumente `--ddos-protection` und `--vm-protection` zu `vnet [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3424">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="0bba9-3425">Befehle vom Typ `network [vnet-gateway|vpn-client|show-url]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3425">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="0bba9-3426">Storage</span><span class="sxs-lookup"><span data-stu-id="0bba9-3426">Storage</span></span>

* <span data-ttu-id="0bba9-3427">Problem behoben, das nach der Aktualisierung des SDK unter Umständen einen Fehler der `storage account network-rule`-Befehle zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="0bba9-3427">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="0bba9-3428">Eventgrid</span><span class="sxs-lookup"><span data-stu-id="0bba9-3428">Eventgrid</span></span>

* <span data-ttu-id="0bba9-3429">Azure Event Grid Python SDK für die Verwendung der neueren API-Version „2017-09-15-preview“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-3429">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="0bba9-3430">SQL</span><span class="sxs-lookup"><span data-stu-id="0bba9-3430">SQL</span></span>

* <span data-ttu-id="0bba9-3431">`sql server list`-Argument `--resource-group` geändert, sodass es nun optional ist.</span><span class="sxs-lookup"><span data-stu-id="0bba9-3431">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="0bba9-3432">Wird es nicht angegeben, werden alle SQL Server-Instanzen im Abonnement zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0bba9-3432">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="0bba9-3433">Parameter `--no-wait` zu `db [create|copy|restore|update|replica create|create|update]` und `dw [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3433">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="0bba9-3434">KeyVault</span><span class="sxs-lookup"><span data-stu-id="0bba9-3434">Keyvault</span></span>

* <span data-ttu-id="0bba9-3435">Unterstützung für die Keyvault-Befehlsausführung hinter einem Proxy hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3435">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="0bba9-3436">VM</span><span class="sxs-lookup"><span data-stu-id="0bba9-3436">VM</span></span>

* <span data-ttu-id="0bba9-3437">Unterstützung für Verfügbarkeitszone zu `[vm|vmss|disk] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3437">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="0bba9-3438">Problem behoben, das bei Verwendung von `--app-gateway ID` mit `vmss create` einen Fehler zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="0bba9-3438">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="0bba9-3439">Argument `--asgs` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3439">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="0bba9-3440">Unterstützung für die Ausführung von Befehlen auf virtuellen Computern mit `vm run-command` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3440">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="0bba9-3441">[VORSCHAU] Unterstützung für VMSS-Datenträgerverschlüsselung mit `vmss encryption` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3441">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="0bba9-3442">Unterstützung für die Durchführung der Wartung auf virtuellen Computern mit `vm perform-maintenance` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3442">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="0bba9-3443">ACS</span><span class="sxs-lookup"><span data-stu-id="0bba9-3443">ACS</span></span>

* <span data-ttu-id="0bba9-3444">[VORSCHAU] Argument `--orchestrator-release` zu `acs create` für ACS-Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3444">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="0bba9-3445">AppService</span><span class="sxs-lookup"><span data-stu-id="0bba9-3445">Appservice</span></span>

* <span data-ttu-id="0bba9-3446">Neue Möglichkeit zum Aktualisieren und Anzeigen der Authentifizierungseinstellungen mit `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="0bba9-3446">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="0bba9-3447">Backup</span><span class="sxs-lookup"><span data-stu-id="0bba9-3447">Backup</span></span>

* <span data-ttu-id="0bba9-3448">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="0bba9-3448">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="0bba9-3449">11. September 2017</span><span class="sxs-lookup"><span data-stu-id="0bba9-3449">September 11, 2017</span></span>

<span data-ttu-id="0bba9-3450">Version 2.0.17</span><span class="sxs-lookup"><span data-stu-id="0bba9-3450">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="0bba9-3451">Core</span><span class="sxs-lookup"><span data-stu-id="0bba9-3451">Core</span></span>

* <span data-ttu-id="0bba9-3452">Festlegung einer eigenen Korrelations-ID in Telemetrie durch das Befehlsmodul aktiviert</span><span class="sxs-lookup"><span data-stu-id="0bba9-3452">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="0bba9-3453">Ein Problem mit der JSON-Sicherungsdatei wurde behoben, das beim Festlegen des Diagnosemodus für Telemetrie auftrat</span><span class="sxs-lookup"><span data-stu-id="0bba9-3453">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="0bba9-3454">ACS</span><span class="sxs-lookup"><span data-stu-id="0bba9-3454">Acs</span></span>

* <span data-ttu-id="0bba9-3455">Befehl `acs list-locations` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3455">Added `acs list-locations` command</span></span>
* <span data-ttu-id="0bba9-3456">`ssh-key-file` wird mit dem erwarteten Standardwert versehen.</span><span class="sxs-lookup"><span data-stu-id="0bba9-3456">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="0bba9-3457">AppService</span><span class="sxs-lookup"><span data-stu-id="0bba9-3457">Appservice</span></span>

* <span data-ttu-id="0bba9-3458">Neue Möglichkeit zum Erstellen einer Web-App in einer anderen Ressourcengruppe als der des aktiven Diensttarifs</span><span class="sxs-lookup"><span data-stu-id="0bba9-3458">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="0bba9-3459">CDN</span><span class="sxs-lookup"><span data-stu-id="0bba9-3459">CDN</span></span>

* <span data-ttu-id="0bba9-3460">Der Fehler bei `cdn custom-domain create`, dass „CustomDomain“ nicht wiederholbar ist, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="0bba9-3460">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="0bba9-3461">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="0bba9-3461">Extension</span></span>

* <span data-ttu-id="0bba9-3462">Erstrelease</span><span class="sxs-lookup"><span data-stu-id="0bba9-3462">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="0bba9-3463">KeyVault</span><span class="sxs-lookup"><span data-stu-id="0bba9-3463">Keyvault</span></span>

* <span data-ttu-id="0bba9-3464">Problem behoben, aufgrund dessen bei den Berechtigungen für `keyvault set-policy` die Groß-/Kleinschreibung beachtet werden musste</span><span class="sxs-lookup"><span data-stu-id="0bba9-3464">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="0bba9-3465">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0bba9-3465">Network</span></span>

* <span data-ttu-id="0bba9-3466">`vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3466">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="0bba9-3467">Das Argument `--private-access-services` wurde für `vnet subnet create/update` in `--service-endpoints` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-3467">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="0bba9-3468">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3468">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="0bba9-3469">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3469">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="0bba9-3470">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3470">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="0bba9-3471">Resource</span><span class="sxs-lookup"><span data-stu-id="0bba9-3471">Resource</span></span>

* <span data-ttu-id="0bba9-3472">Übergabe von Parameterdefinitionen für Ressourcenrichtlinien in `policy definition create` und `policy definition update` zulassen</span><span class="sxs-lookup"><span data-stu-id="0bba9-3472">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="0bba9-3473">Übergabe von Parameterwerten für `policy assignment create` zulassen</span><span class="sxs-lookup"><span data-stu-id="0bba9-3473">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="0bba9-3474">Übergabe von JSON-Code oder einer Datei für alle Parameter zulassen</span><span class="sxs-lookup"><span data-stu-id="0bba9-3474">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="0bba9-3475">Inkrementierte API-Version</span><span class="sxs-lookup"><span data-stu-id="0bba9-3475">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="0bba9-3476">SQL</span><span class="sxs-lookup"><span data-stu-id="0bba9-3476">SQL</span></span>

* <span data-ttu-id="0bba9-3477">Befehle vom Typ `sql server vnet-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3477">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="0bba9-3478">VM</span><span class="sxs-lookup"><span data-stu-id="0bba9-3478">VM</span></span>

* <span data-ttu-id="0bba9-3479">Behoben: Zugriff nur zuweisen, wenn `--scope` angegeben wird</span><span class="sxs-lookup"><span data-stu-id="0bba9-3479">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="0bba9-3480">Behoben: Gleiche Erweiterungsbenennung wie Portal verwenden</span><span class="sxs-lookup"><span data-stu-id="0bba9-3480">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="0bba9-3481">`subscription` aus der Ausgabe von `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3481">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="0bba9-3482">Behoben: Speicher-SKU vom Typ `[vm|vmss] create` wird nicht auf Datenträger mit einem Image angewendet.</span><span class="sxs-lookup"><span data-stu-id="0bba9-3482">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="0bba9-3483">Behoben: `vm format-secret --secrets` akzeptierte keine durch neue Zeilen getrennte IDs.</span><span class="sxs-lookup"><span data-stu-id="0bba9-3483">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="0bba9-3484">31. August 2017</span><span class="sxs-lookup"><span data-stu-id="0bba9-3484">August 31, 2017</span></span>

<span data-ttu-id="0bba9-3485">Version 2.0.16</span><span class="sxs-lookup"><span data-stu-id="0bba9-3485">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="0bba9-3486">KeyVault</span><span class="sxs-lookup"><span data-stu-id="0bba9-3486">Keyvault</span></span>

* <span data-ttu-id="0bba9-3487">Fehler behoben, der beim Versuch auftrat, die Geheimniscodierung mit `secret download` automatisch aufzulösen</span><span class="sxs-lookup"><span data-stu-id="0bba9-3487">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="0bba9-3488">Sf</span><span class="sxs-lookup"><span data-stu-id="0bba9-3488">Sf</span></span>

* <span data-ttu-id="0bba9-3489">Alle Befehle wurden durch die Service Fabric-Befehlszeilenschnittstelle (sfctl) ersetzt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-3489">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="0bba9-3490">Storage</span><span class="sxs-lookup"><span data-stu-id="0bba9-3490">Storage</span></span>

* <span data-ttu-id="0bba9-3491">Problem behoben, aufgrund dessen Speicherkonten nicht in Regionen erstellt werden konnten, die die NetworkACLs-Funktion nicht unterstützen</span><span class="sxs-lookup"><span data-stu-id="0bba9-3491">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="0bba9-3492">Festlegen des Inhaltstyps und der Inhaltscodierung während Blob- und Dateiuploads, wenn weder Inhaltstyp noch Inhaltscodierung angegeben sind</span><span class="sxs-lookup"><span data-stu-id="0bba9-3492">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="0bba9-3493">28. August 2017</span><span class="sxs-lookup"><span data-stu-id="0bba9-3493">August 28, 2017</span></span>

<span data-ttu-id="0bba9-3494">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="0bba9-3494">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="0bba9-3495">Befehlszeilenschnittstelle (CLI)</span><span class="sxs-lookup"><span data-stu-id="0bba9-3495">CLI</span></span>

* <span data-ttu-id="0bba9-3496">Rechtlichen Hinweis zu `--version` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3496">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="0bba9-3497">ACS</span><span class="sxs-lookup"><span data-stu-id="0bba9-3497">ACS</span></span>

* <span data-ttu-id="0bba9-3498">Vorschauregionen korrigiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-3498">Corrected preview regions</span></span>
* <span data-ttu-id="0bba9-3499">Standardmäßiges DNS-Namenspräfix (`dns_name_prefix`) ordnungsgemäß formatiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-3499">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="0bba9-3500">ACS-Befehlsausgabe optimiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-3500">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="0bba9-3501">AppService</span><span class="sxs-lookup"><span data-stu-id="0bba9-3501">Appservice</span></span>

* <span data-ttu-id="0bba9-3502">[BREAKING CHANGE] Inkonsistenzen in der Ausgabe von `az webapp config appsettings [delete|set]` behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-3502">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="0bba9-3503">Neuen Alias (`-i`) für `az webapp config container set --docker-custom-image-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3503">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="0bba9-3504">`az webapp log show` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="0bba9-3504">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="0bba9-3505">Neue Argumente aus `az webapp delete` verfügbar gemacht, um App Service-Plan, Metriken oder DNS-Registrierung beizubehalten</span><span class="sxs-lookup"><span data-stu-id="0bba9-3505">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="0bba9-3506">Behoben: Korrekte Erkennung der Sloteinstellungen</span><span class="sxs-lookup"><span data-stu-id="0bba9-3506">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="0bba9-3507">IoT</span><span class="sxs-lookup"><span data-stu-id="0bba9-3507">IoT</span></span>

* <span data-ttu-id="0bba9-3508">#3934 behoben: Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="0bba9-3508">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="0bba9-3509">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0bba9-3509">Network</span></span>

* <span data-ttu-id="0bba9-3510">[BREAKING CHANGE]`vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3510">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="0bba9-3511">[BREAKING CHANGE] Option `--private-access-services` für `--service-endpoints` in `vnet subnet [create|update]` umbenannt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3511">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="0bba9-3512">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3512">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="0bba9-3513">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3513">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="0bba9-3514">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3514">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="0bba9-3515">Profil</span><span class="sxs-lookup"><span data-stu-id="0bba9-3515">Profile</span></span>

* <span data-ttu-id="0bba9-3516">`--msi` und `--msi-port` für die Anmeldung mit der Identität eines virtuellen Computers verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="0bba9-3516">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="0bba9-3517">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="0bba9-3517">Service Fabric</span></span>

* <span data-ttu-id="0bba9-3518">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="0bba9-3518">Preview release</span></span>
* <span data-ttu-id="0bba9-3519">Registrierungsbenutzer-/-kennwortregeln für Befehl vereinfacht</span><span class="sxs-lookup"><span data-stu-id="0bba9-3519">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="0bba9-3520">Kennwortanforderung für Benutzer trotz Parameterübergabe behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-3520">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="0bba9-3521">Unterstützung für leere Registrierungsanmeldeinformationen (`registry_cred`) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3521">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="0bba9-3522">Storage</span><span class="sxs-lookup"><span data-stu-id="0bba9-3522">Storage</span></span>

* <span data-ttu-id="0bba9-3523">Festlegen des Blobtarifs ermöglicht</span><span class="sxs-lookup"><span data-stu-id="0bba9-3523">Enabled setting blob tier</span></span>
* <span data-ttu-id="0bba9-3524">Argumente `--bypass` und `--default-action` zur Unterstützung von Diensttunneling zu `storage account [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3524">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="0bba9-3525">Befehle zum Hinzufügen von VNet-Regeln und IP-basierten Regeln zu `storage account network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3525">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="0bba9-3526">Dienstverschlüsselung durch vom Kunden verwalteten Schlüssel ermöglicht</span><span class="sxs-lookup"><span data-stu-id="0bba9-3526">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="0bba9-3527">[BREAKING CHANGE] Option `--encryption` für Befehl `az storage account create and az storage account update` in `--encryption-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3527">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="0bba9-3528">Behoben (4220): `az storage account update encryption` – Syntaxkonflikt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3528">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="0bba9-3529">VM</span><span class="sxs-lookup"><span data-stu-id="0bba9-3529">VM</span></span>

* <span data-ttu-id="0bba9-3530">Problem behoben, aufgrund dessen bei Verwendung von `--instance-id *` zusätzliche, fehlerhafte Informationen für `vmss get-instance-view` angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="0bba9-3530">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="0bba9-3531">Unterstützung für `--lb-sku` zu `vmss create` hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="0bba9-3531">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="0bba9-3532">Menschliche Namen aus der Administratornamen-Blacklist für `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3532">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="0bba9-3533">Problem behoben, aufgrund dessen `[vm|vmss] create` einen Fehler ausgelöst hat, wenn aus einem Image keine Tarifinformationen extrahiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="0bba9-3533">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="0bba9-3534">Absturzproblem beim Erstellen einer VMMS-Skalierungsgruppe mit einem internen Lastenausgleich behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-3534">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="0bba9-3535">Problem behoben, aufgrund dessen das Argument `--no-wait` nicht mit `vm availability-set create` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="0bba9-3535">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="0bba9-3536">15. August 2017</span><span class="sxs-lookup"><span data-stu-id="0bba9-3536">August 15, 2017</span></span>

<span data-ttu-id="0bba9-3537">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="0bba9-3537">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="0bba9-3538">ACS</span><span class="sxs-lookup"><span data-stu-id="0bba9-3538">ACS</span></span>

* <span data-ttu-id="0bba9-3539">sshMaster0-Portnummer für Kubernetes korrigiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-3539">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="0bba9-3540">AppService</span><span class="sxs-lookup"><span data-stu-id="0bba9-3540">Appservice</span></span>

* <span data-ttu-id="0bba9-3541">Ausnahme beim Erstellen einer neuen Git-basierten Linux-Web-App behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-3541">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="0bba9-3542">Event Grid</span><span class="sxs-lookup"><span data-stu-id="0bba9-3542">Event Grid</span></span>

* <span data-ttu-id="0bba9-3543">SDK-Abhängigkeiten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3543">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="0bba9-3544">11. August 2017</span><span class="sxs-lookup"><span data-stu-id="0bba9-3544">August 11, 2017</span></span>

<span data-ttu-id="0bba9-3545">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="0bba9-3545">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="0bba9-3546">ACS</span><span class="sxs-lookup"><span data-stu-id="0bba9-3546">ACS</span></span>

* <span data-ttu-id="0bba9-3547">Weitere Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3547">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="0bba9-3548">Batch</span><span class="sxs-lookup"><span data-stu-id="0bba9-3548">Batch</span></span>

* <span data-ttu-id="0bba9-3549">Auf Batch SDK 3.1.0 und Batch Management SDK 4.1.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-3549">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="0bba9-3550">Neuen Befehl zum Anzeigen der Aufgabenanzahl eines Auftrags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3550">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="0bba9-3551">Fehler in der SAS-URL-Verarbeitung der Ressourcendatei behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-3551">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="0bba9-3552">Batch-Kontoendpunkt unterstützt nun optionales Präfix „https://“</span><span class="sxs-lookup"><span data-stu-id="0bba9-3552">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="0bba9-3553">Unterstützung für das Hinzufügen von Listen mit mehr als 100 Aufgaben zu einem Auftrag</span><span class="sxs-lookup"><span data-stu-id="0bba9-3553">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="0bba9-3554">Debugprotokollierung für das Laden des Erweiterungsbefehlsmoduls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3554">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="0bba9-3555">Komponente</span><span class="sxs-lookup"><span data-stu-id="0bba9-3555">Component</span></span>

* <span data-ttu-id="0bba9-3556">Warnung für veraltete Befehle vom Typ „az component“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3556">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="0bba9-3557">Container</span><span class="sxs-lookup"><span data-stu-id="0bba9-3557">Container</span></span>

* <span data-ttu-id="0bba9-3558">`create`: Problem behoben, aufgrund dessen das Gleichheitszeichen innerhalb einer Umgebungsvariablen nicht zulässig war</span><span class="sxs-lookup"><span data-stu-id="0bba9-3558">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="0bba9-3559">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="0bba9-3559">Data Lake Store</span></span>

* <span data-ttu-id="0bba9-3560">Fortschrittsüberwachung ermöglicht</span><span class="sxs-lookup"><span data-stu-id="0bba9-3560">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="0bba9-3561">Event Grid</span><span class="sxs-lookup"><span data-stu-id="0bba9-3561">Event Grid</span></span>

* <span data-ttu-id="0bba9-3562">Erste Veröffentlichung</span><span class="sxs-lookup"><span data-stu-id="0bba9-3562">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="0bba9-3563">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0bba9-3563">Network</span></span>

* <span data-ttu-id="0bba9-3564">`lb`: Problem behoben, aufgrund dessen bestimmte Namen untergeordneter Ressourcen bei Auslassung nicht richtig aufgelöst wurden</span><span class="sxs-lookup"><span data-stu-id="0bba9-3564">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="0bba9-3565">`application-gateway {subresource} delete`: Problem behoben, aufgrund dessen `--no-wait` nicht berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="0bba9-3565">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="0bba9-3566">`application-gateway http-settings update`: Problem behoben, aufgrund dessen `--connection-draining-timeout` nicht deaktiviert werden konnte</span><span class="sxs-lookup"><span data-stu-id="0bba9-3566">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="0bba9-3567">Fehler behoben: Unerwartetes Schlüsselwortargument `sa_data_size_kilobyes` bei `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="0bba9-3567">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="0bba9-3568">Profil</span><span class="sxs-lookup"><span data-stu-id="0bba9-3568">Profile</span></span>

* <span data-ttu-id="0bba9-3569">`account list`: `--refresh` hinzugefügt, um die neuesten Abonnements vom Server zu synchronisieren</span><span class="sxs-lookup"><span data-stu-id="0bba9-3569">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="0bba9-3570">Storage</span><span class="sxs-lookup"><span data-stu-id="0bba9-3570">Storage</span></span>

* <span data-ttu-id="0bba9-3571">Aktualisieren des Speicherkontos mit vom System zugewiesener Identität ermöglicht</span><span class="sxs-lookup"><span data-stu-id="0bba9-3571">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="0bba9-3572">VM</span><span class="sxs-lookup"><span data-stu-id="0bba9-3572">VM</span></span>

* <span data-ttu-id="0bba9-3573">`availability-set`: Fehlerdomänenanzahl bei Konvertierung verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="0bba9-3573">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="0bba9-3574">Befehl `list-skus` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="0bba9-3574">Exposed `list-skus` command</span></span>
* <span data-ttu-id="0bba9-3575">Unterstützung der Identitätszuweisung ohne Erstellung von Rollenzuweisungen</span><span class="sxs-lookup"><span data-stu-id="0bba9-3575">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="0bba9-3576">Anwenden von Speicher-SKU beim Anfügen von Datenträgern</span><span class="sxs-lookup"><span data-stu-id="0bba9-3576">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="0bba9-3577">Standardmäßiger Betriebssystemdatenträger-Name und Speicher-SKU bei Verwendung verwalteter Datenträger entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3577">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="0bba9-3578">28. Juli 2017</span><span class="sxs-lookup"><span data-stu-id="0bba9-3578">July 28, 2017</span></span>

<span data-ttu-id="0bba9-3579">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="0bba9-3579">Version 2.0.12</span></span>

* <span data-ttu-id="0bba9-3580">Containerbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3580">Added container commands</span></span>
* <span data-ttu-id="0bba9-3581">Abrechnungs- und Nutzungsmodule hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3581">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="0bba9-3582">Core</span><span class="sxs-lookup"><span data-stu-id="0bba9-3582">Core</span></span>

* <span data-ttu-id="0bba9-3583">Ausgabe von SDK-Authentifizierungsinformationen für Dienstprinzipale mit Zertifikaten</span><span class="sxs-lookup"><span data-stu-id="0bba9-3583">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="0bba9-3584">Ausnahmen beim Bereitstellungsfortschritt behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-3584">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="0bba9-3585">Verwendung des ARM-Endpunkts aus der aktuellen Cloud für die Erstellung des Abonnementclients</span><span class="sxs-lookup"><span data-stu-id="0bba9-3585">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="0bba9-3586">Gleichzeitige Verarbeitung der Datei „clouds.config“ verbessert (3636)</span><span class="sxs-lookup"><span data-stu-id="0bba9-3586">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="0bba9-3587">Aktualisierung der Clientanforderungs-ID für jede Befehlsausführung</span><span class="sxs-lookup"><span data-stu-id="0bba9-3587">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="0bba9-3588">Erstellung von Abonnementclients mit richtigem SDK-Profil (3635)</span><span class="sxs-lookup"><span data-stu-id="0bba9-3588">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="0bba9-3589">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="0bba9-3589">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="0bba9-3590">Unterstützung für Auswahl von Tabellenausgabefeldern über jmespath Abfrage hinzugefügt (3581)</span><span class="sxs-lookup"><span data-stu-id="0bba9-3590">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="0bba9-3591">Stummschaltung von Analyseargumenten und Anfügeverlauf mit Gesten verbessert (3434)</span><span class="sxs-lookup"><span data-stu-id="0bba9-3591">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="0bba9-3592">Erstellung von Abonnementclients mit richtigem SDK-Profil</span><span class="sxs-lookup"><span data-stu-id="0bba9-3592">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="0bba9-3593">Verschiebung aller vorhandenen Erfassungsdateien in den neuesten Ordner</span><span class="sxs-lookup"><span data-stu-id="0bba9-3593">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="0bba9-3594">Idempotenz für VM-/VMSS-Erstellung behoben (3586)</span><span class="sxs-lookup"><span data-stu-id="0bba9-3594">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="0bba9-3595">Bei Befehlspfaden wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="0bba9-3595">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="0bba9-3596">Bei bestimmten booleschen Parametern wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="0bba9-3596">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="0bba9-3597">Unterstützung der Anmeldung bei lokalem AD FS-Server wie Azure Stack</span><span class="sxs-lookup"><span data-stu-id="0bba9-3597">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="0bba9-3598">Gleichzeitige Schreibvorgänge in „clouds.config“ behoben (3255)</span><span class="sxs-lookup"><span data-stu-id="0bba9-3598">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="0bba9-3599">ACR</span><span class="sxs-lookup"><span data-stu-id="0bba9-3599">ACR</span></span>

* <span data-ttu-id="0bba9-3600">Befehl `show-usage` für verwaltete Registrierungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3600">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="0bba9-3601">Unterstützung der SKU-Aktualisierung für verwaltete Registrierungen</span><span class="sxs-lookup"><span data-stu-id="0bba9-3601">Support SKU update for managed registries</span></span>
* <span data-ttu-id="0bba9-3602">Verwaltete Registrierungen mit verwalteter SKU hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3602">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="0bba9-3603">Webhooks für verwaltete Registrierungen mit ACR-Webhook-Befehlsmodul hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3603">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="0bba9-3604">AAD-Authentifizierung mit ACR-Anmeldebefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3604">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="0bba9-3605">Löschbefehl für Docker-Repositorys, Manifeste und Tags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3605">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="0bba9-3606">ACS</span><span class="sxs-lookup"><span data-stu-id="0bba9-3606">ACS</span></span>

* <span data-ttu-id="0bba9-3607">Unterstützung der API-Version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="0bba9-3607">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="0bba9-3608">AppService</span><span class="sxs-lookup"><span data-stu-id="0bba9-3608">Appservice</span></span>

* <span data-ttu-id="0bba9-3609">Fehler behoben, aufgrund dessen die Auflistung der Linux-Web-App keine Werte zurückgegeben hat</span><span class="sxs-lookup"><span data-stu-id="0bba9-3609">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="0bba9-3610">Unterstützung für das Abrufen von Anmeldeinformationen aus dem ACR</span><span class="sxs-lookup"><span data-stu-id="0bba9-3610">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="0bba9-3611">Entfernung aller Befehle unter `appservice web`</span><span class="sxs-lookup"><span data-stu-id="0bba9-3611">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="0bba9-3612">Maskierung von Docker-Registrierungskennwörtern aus der Befehlsausgabe (3656)</span><span class="sxs-lookup"><span data-stu-id="0bba9-3612">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="0bba9-3613">Gewährleistung der fehlerfreien Verwendung des Standardbrowsers unter macOS (3623)</span><span class="sxs-lookup"><span data-stu-id="0bba9-3613">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="0bba9-3614">Verbesserung des Nutzens von `webapp log tail` und `webapp log download` (3624)</span><span class="sxs-lookup"><span data-stu-id="0bba9-3614">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="0bba9-3615">Befehl `traffic-routing` zum Konfigurieren des statischen Routings verfügbar gemacht (3566)</span><span class="sxs-lookup"><span data-stu-id="0bba9-3615">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="0bba9-3616">Zuverlässigkeit beim Konfigurieren der Quellcodeverwaltung verbessert (3245)</span><span class="sxs-lookup"><span data-stu-id="0bba9-3616">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="0bba9-3617">Nicht unterstütztes Argument `--node-version` aus `webapp config update` für Windows-Web-Apps entfernt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-3617">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="0bba9-3618">Verwenden Sie stattdessen `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="0bba9-3618">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="0bba9-3619">Batch</span><span class="sxs-lookup"><span data-stu-id="0bba9-3619">Batch</span></span>

* <span data-ttu-id="0bba9-3620">Auf Batch SDK 3.0.0 mit Unterstützung virtueller Computer mit niedriger Priorität in Pools aktualisiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-3620">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="0bba9-3621">`pool create`-Option `--target-dedicated` in `--target-dedicated-nodes` umbenannt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3621">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="0bba9-3622">`pool create`-Optionen `--target-low-priority-nodes` und `--application-licenses` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3622">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="0bba9-3623">CDN</span><span class="sxs-lookup"><span data-stu-id="0bba9-3623">CDN</span></span>

* <span data-ttu-id="0bba9-3624">Besser verständliche Fehlermeldung für `cdn endpoint list`, wenn das von `--profile-name` angegebene Profil nicht vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="0bba9-3624">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="0bba9-3625">Cloud</span><span class="sxs-lookup"><span data-stu-id="0bba9-3625">Cloud</span></span>

* <span data-ttu-id="0bba9-3626">API-Version des Cloudmetadaten-Endpunkts in das Format JJJJ-MM-TT umgewandelt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3626">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="0bba9-3627">Katalogendpunkt nicht erforderlich</span><span class="sxs-lookup"><span data-stu-id="0bba9-3627">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="0bba9-3628">Unterstützung für die Cloudregistrierung nur mit ARM-Endpunkt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3628">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="0bba9-3629">Option für `cloud set` bereitgestellt, um beim Auswählen der aktuellen Cloud das Profil auswählen zu können</span><span class="sxs-lookup"><span data-stu-id="0bba9-3629">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="0bba9-3630">`endpoint_vm_image_alias_doc` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="0bba9-3630">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="0bba9-3631">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="0bba9-3631">CosmosDB</span></span>

* <span data-ttu-id="0bba9-3632">Möglichkeit zum Erstellen einer Auflistung mit benutzerdefiniertem Partitionsschlüssel behoben</span><span class="sxs-lookup"><span data-stu-id="0bba9-3632">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="0bba9-3633">Unterstützung für Auflistungs-Standardgültigkeitsdauer hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3633">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="0bba9-3634">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="0bba9-3634">Data Lake Analytics</span></span>

* <span data-ttu-id="0bba9-3635">Zusätzliche Befehle für Compute-Richtlinienverwaltung unter der Überschrift `dla account compute-policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3635">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="0bba9-3636">`dla job pipeline show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3636">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="0bba9-3637">`dla job recurrence list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3637">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="0bba9-3638">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="0bba9-3638">Data Lake Store</span></span>

* <span data-ttu-id="0bba9-3639">Unterstützung für vom Benutzer verwaltete Schlüsseltresor-Schlüsselrotation in `dls account update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3639">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="0bba9-3640">Zugrunde liegende SDK-Version des Data Lake Store-Dateisystems aktualisiert, um ein Leistungsproblem zu behandeln</span><span class="sxs-lookup"><span data-stu-id="0bba9-3640">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="0bba9-3641">Befehl `dls enable-key-vault` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-3641">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="0bba9-3642">Dieser Befehl versucht, eine vom Benutzer angegebene Key Vault-Instanz zur Verschlüsselung der Daten in einem Data Lake Store-Konto zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="0bba9-3642">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="0bba9-3643">Interactive</span><span class="sxs-lookup"><span data-stu-id="0bba9-3643">Interactive</span></span>

* <span data-ttu-id="0bba9-3644">Startzeit durch Verwendung zwischengespeicherter Befehle verbessert</span><span class="sxs-lookup"><span data-stu-id="0bba9-3644">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="0bba9-3645">Testabdeckung verbessert</span><span class="sxs-lookup"><span data-stu-id="0bba9-3645">Increased test coverage</span></span>
* <span data-ttu-id="0bba9-3646">?-Geste erweitert, sodass sie auch in den nächsten Befehl eingefügt wird</span><span class="sxs-lookup"><span data-stu-id="0bba9-3646">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="0bba9-3647">Interaktive Fehler mit dem Profil „2017-03-09-profile-preview“ behoben (3587)</span><span class="sxs-lookup"><span data-stu-id="0bba9-3647">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="0bba9-3648">`--version` als Parameter für den interaktiven Modus zugelassen (3645)</span><span class="sxs-lookup"><span data-stu-id="0bba9-3648">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="0bba9-3649">Beseitigung von Fehlern im interaktiven Modus beim Abschluss von Überprüfungen (3570)</span><span class="sxs-lookup"><span data-stu-id="0bba9-3649">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="0bba9-3650">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="0bba9-3650">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="0bba9-3651">Flag `--progress` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3651">Added `--progress` flag</span></span>
* <span data-ttu-id="0bba9-3652">`--debug` und `--verbose` aus Abschlüssen entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3652">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="0bba9-3653">`interactive` aus Abschlüssen entfernt (3324)</span><span class="sxs-lookup"><span data-stu-id="0bba9-3653">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="0bba9-3654">IoT</span><span class="sxs-lookup"><span data-stu-id="0bba9-3654">IoT</span></span>

* <span data-ttu-id="0bba9-3655">Behoben: Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="0bba9-3655">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="0bba9-3656">(3934)</span><span class="sxs-lookup"><span data-stu-id="0bba9-3656">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="0bba9-3657">Schlüsseltresor</span><span class="sxs-lookup"><span data-stu-id="0bba9-3657">Key vault</span></span>

* <span data-ttu-id="0bba9-3658">Befehle für Schlüsseltresor-Wiederherstellungsfeatures hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="0bba9-3658">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="0bba9-3659">`keyvault`-Unterbefehle: `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="0bba9-3659">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="0bba9-3660">`keyvault secret`-Unterbefehle: `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="0bba9-3660">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="0bba9-3661">`keyvault certificate`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="0bba9-3661">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="0bba9-3662">`keyvault key`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="0bba9-3662">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="0bba9-3663">Dienstprinzipal-Schlüsseltresorintegration hinzugefügt (3133)</span><span class="sxs-lookup"><span data-stu-id="0bba9-3663">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="0bba9-3664">Schlüsseltresor-Datenebene auf 0.3.2. aktualisiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-3664">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="0bba9-3665">(3307)</span><span class="sxs-lookup"><span data-stu-id="0bba9-3665">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="0bba9-3666">Labor</span><span class="sxs-lookup"><span data-stu-id="0bba9-3666">Lab</span></span>

* <span data-ttu-id="0bba9-3667">Unterstützung für Übernahme eines beliebigen virtuellen Computers im Labor über `az lab vm claim` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3667">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="0bba9-3668">Tabellenausgabeformatierer für `az lab vm list` und `az lab vm show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3668">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="0bba9-3669">Überwachen</span><span class="sxs-lookup"><span data-stu-id="0bba9-3669">Monitor</span></span>

* <span data-ttu-id="0bba9-3670">Korrektur für Vorlagendatei mit Befehl `monitor autoscale-settings get-parameters-template` (3349)</span><span class="sxs-lookup"><span data-stu-id="0bba9-3670">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="0bba9-3671">`monitor alert-rule-incidents list` in `monitor alert list-incidents` umbenannt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3671">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="0bba9-3672">`monitor alert-rule-incidents show` in `monitor alert show-incident` umbenannt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3672">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="0bba9-3673">`monitor metric-defintions list` in `monitor metrics list-definitions` umbenannt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3673">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="0bba9-3674">`monitor alert-rules` in `monitor alert` umbenannt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3674">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="0bba9-3675">`monitor alert create` geändert:</span><span class="sxs-lookup"><span data-stu-id="0bba9-3675">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="0bba9-3676">Unterbefehle vom Typ `condition` und `action` akzeptieren keinen JSON-Code mehr.</span><span class="sxs-lookup"><span data-stu-id="0bba9-3676">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="0bba9-3677">Hinzufügung zahlreicher Parameter zur Vereinfachung der Regelerstellung</span><span class="sxs-lookup"><span data-stu-id="0bba9-3677">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="0bba9-3678">`location` nicht mehr erforderlich</span><span class="sxs-lookup"><span data-stu-id="0bba9-3678">`location` no longer required</span></span>
  * <span data-ttu-id="0bba9-3679">Hinzufügung von Namen- und ID-Unterstützung für Ziel</span><span class="sxs-lookup"><span data-stu-id="0bba9-3679">Add name and ID support for target</span></span>
  * <span data-ttu-id="0bba9-3680">Entfernung von `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="0bba9-3680">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="0bba9-3681">Umbenennung von `is-enabled` in `enabled` (nicht mehr erforderlich)</span><span class="sxs-lookup"><span data-stu-id="0bba9-3681">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="0bba9-3682">`description` wird nun abhängig von der angegebenen Bedingung auf einen Standardwert festgelegt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-3682">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="0bba9-3683">Hinzufügung von Beispielen zur Verdeutlichung des neuen Formats</span><span class="sxs-lookup"><span data-stu-id="0bba9-3683">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="0bba9-3684">Unterstützung von Namen oder IDs für Befehle vom Typ `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="0bba9-3684">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="0bba9-3685">Komfortargumente und Beispiele zu `monitor alert rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3685">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="0bba9-3686">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0bba9-3686">Network</span></span>

* <span data-ttu-id="0bba9-3687">Befehl `list-private-access-services` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3687">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="0bba9-3688">Argument `--private-access-services` zu `vnet subnet create` und `vnet subnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3688">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="0bba9-3689">Problem behoben, das einen Fehler für `application-gateway redirect-config create` zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="0bba9-3689">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="0bba9-3690">Problem behoben, aufgrund dessen `application-gateway redirect-config update` nicht mit `--no-wait` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="0bba9-3690">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="0bba9-3691">Fehler behoben, der bei der Verwendung des Arguments `--servers` mit `application-gateway address-pool create` und `application-gateway address-pool update` aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="0bba9-3691">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="0bba9-3692">Befehle vom Typ `application-gateway redirect-config` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3692">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="0bba9-3693">Befehle zu `application-gateway ssl-policy` hinzugefügt: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="0bba9-3693">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="0bba9-3694">Argumente zu `application-gateway ssl-policy set` hinzugefügt: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="0bba9-3694">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="0bba9-3695">Argumente zu `application-gateway http-settings create` und `application-gateway http-settings update` hinzugefügt: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="0bba9-3695">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="0bba9-3696">Argumente zu `application-gateway url-path-map create` und `application-gateway url-path-map update` hinzugefügt: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="0bba9-3696">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="0bba9-3697">Argument `--redirect-config` zu `application-gateway url-path-map rule create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3697">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="0bba9-3698">Unterstützung für `--no-wait` zu `application-gateway url-path-map rule delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3698">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="0bba9-3699">Argumente zu `application-gateway probe create` und `application-gateway probe update` hinzugefügt: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="0bba9-3699">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="0bba9-3700">Argument `--redirect-config` zu `application-gateway rule create` und `application-gateway rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3700">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="0bba9-3701">Unterstützung für `--accelerated-networking` zu `nic create` und `nic update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3701">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="0bba9-3702">Argument `--internal-dns-name-suffix` von `nic create` entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3702">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="0bba9-3703">Unterstützung für `--dns-servers` zu `nic update` und `nic create` hinzugefügt: Hinzufügung von Unterstützung für --dns-servers</span><span class="sxs-lookup"><span data-stu-id="0bba9-3703">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="0bba9-3704">Fehler korrigiert, aufgrund dessen `--local-address-prefixes` von `local-gateway create` ignoriert wurde</span><span class="sxs-lookup"><span data-stu-id="0bba9-3704">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="0bba9-3705">Unterstützung für `--dns-servers` zu `vnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3705">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="0bba9-3706">Fehler beim Erstellen eines Peerings ohne Routenfilterung mit `express-route peering create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-3706">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="0bba9-3707">Fehler korrigiert, aufgrund dessen die Argumente `--provider` und `--bandwidth` nicht mit `express-route update` verwendet werden konnten</span><span class="sxs-lookup"><span data-stu-id="0bba9-3707">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="0bba9-3708">Fehler mit Standardlogik von `network watcher show-topology` korrigiert</span><span class="sxs-lookup"><span data-stu-id="0bba9-3708">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="0bba9-3709">Ausgabeformatierung für `network list-usages` verbessert</span><span class="sxs-lookup"><span data-stu-id="0bba9-3709">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="0bba9-3710">Verwendung der standardmäßigen Front-End-IP-Adresse für `application-gateway http-listener create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="0bba9-3710">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="0bba9-3711">Verwendung des Standardadresspools, der HTTP-Standardeinstellungen und des HTTP-Standardlisteners für `application-gateway rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="0bba9-3711">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="0bba9-3712">Verwendung der standardmäßigen Front-End-IP-Adresse und des standardmäßigen Back-End-Pools für `lb rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="0bba9-3712">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="0bba9-3713">Verwendung der standardmäßigen Front-End-IP-Adresse für `lb inbound-nat-rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="0bba9-3713">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="0bba9-3714">Profil</span><span class="sxs-lookup"><span data-stu-id="0bba9-3714">Profile</span></span>

* <span data-ttu-id="0bba9-3715">Unterstützung der Anmeldung innerhalb eines virtuellen Computers mit einer verwalteten Identität</span><span class="sxs-lookup"><span data-stu-id="0bba9-3715">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="0bba9-3716">Unterstützung der Ausgabe für `account show` im SDK-Authentifizierungsdateiformat</span><span class="sxs-lookup"><span data-stu-id="0bba9-3716">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="0bba9-3717">Anzeige von Warnungen für veraltete Befehle bei Verwendung von „--expanded-view“</span><span class="sxs-lookup"><span data-stu-id="0bba9-3717">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="0bba9-3718">Befehl `get-access-token` für die Bereitstellung eines unformatierten AAD-Tokens hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3718">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="0bba9-3719">Unterstützung der Anmeldung mit einem Benutzerkonto ohne zugeordnete Abonnements</span><span class="sxs-lookup"><span data-stu-id="0bba9-3719">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="0bba9-3720">RDBMS</span><span class="sxs-lookup"><span data-stu-id="0bba9-3720">RDBMS</span></span>

* <span data-ttu-id="0bba9-3721">Unterstützung der abonnementübergreifenden Auflistung von Servern (3417)</span><span class="sxs-lookup"><span data-stu-id="0bba9-3721">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="0bba9-3722">Behoben: `%s` wird aufgrund von fehlendem `% server_type` nicht verarbeitet (3393)</span><span class="sxs-lookup"><span data-stu-id="0bba9-3722">Fixed `%s` not processed because of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="0bba9-3723">Dokumentquellenzuordnung behoben und CI-Aufgabe zur Überprüfung hinzugefügt (3361)</span><span class="sxs-lookup"><span data-stu-id="0bba9-3723">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="0bba9-3724">MySQL- und PostgreSQL-Hilfe korrigiert (3369)</span><span class="sxs-lookup"><span data-stu-id="0bba9-3724">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="0bba9-3725">Resource</span><span class="sxs-lookup"><span data-stu-id="0bba9-3725">Resource</span></span>

* <span data-ttu-id="0bba9-3726">Eingabeaufforderungen bei fehlenden Parametern für `group deployment create` verbessert</span><span class="sxs-lookup"><span data-stu-id="0bba9-3726">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="0bba9-3727">Analyse der Syntax `--parameters KEY=VALUE` verbessert</span><span class="sxs-lookup"><span data-stu-id="0bba9-3727">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="0bba9-3728">Probleme behoben, durch die Parameterdateien von `group deployment create` bei Verwendung der Syntax `@<file>` nicht mehr erkannt wurden</span><span class="sxs-lookup"><span data-stu-id="0bba9-3728">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="0bba9-3729">Unterstützung des Arguments `--ids` für Befehle vom Typ `resource` und `managedapp`</span><span class="sxs-lookup"><span data-stu-id="0bba9-3729">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="0bba9-3730">Einige Analyse- und Fehlermeldungen korrigiert (3584)</span><span class="sxs-lookup"><span data-stu-id="0bba9-3730">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="0bba9-3731">Analyse vom Typ `--resource-type` für den Befehl `lock` korrigiert, sodass `<resource-namespace>` und `<resource-type>` akzeptiert werden</span><span class="sxs-lookup"><span data-stu-id="0bba9-3731">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="0bba9-3732">Parameterüberprüfung für Vorlagenlinkvorlagen hinzugefügt (3629)</span><span class="sxs-lookup"><span data-stu-id="0bba9-3732">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="0bba9-3733">Unterstützung für die Angabe von Bereitstellungsparametern mit der Syntax `KEY=VALUE` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3733">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="0bba9-3734">Role</span><span class="sxs-lookup"><span data-stu-id="0bba9-3734">Role</span></span>

* <span data-ttu-id="0bba9-3735">Unterstützung der Ausgabe im SDK-Authentifizierungsdateiformat für `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="0bba9-3735">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="0bba9-3736">Rollenzuweisungen und dazugehörige AAD-Anwendung beim Löschen eines Dienstprinzipals bereinigt (3610)</span><span class="sxs-lookup"><span data-stu-id="0bba9-3736">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="0bba9-3737">Einbeziehung des Zeitformats in Beschreibungen vom Typ `--start-date` und `--end-date` für `app create`-Argumente</span><span class="sxs-lookup"><span data-stu-id="0bba9-3737">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="0bba9-3738">Anzeige von Warnungen für veraltete Befehle bei Verwendung von `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="0bba9-3738">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="0bba9-3739">Schlüsseltresorintegration zu den Befehlen `create-for-rbac` und `reset-credentials` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3739">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="0bba9-3740">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="0bba9-3740">Service Fabric</span></span>
* <span data-ttu-id="0bba9-3741">Problem behoben, aufgrund dessen große Dateien in Anwendungen beim Hochladen gekürzt wurden (3666)</span><span class="sxs-lookup"><span data-stu-id="0bba9-3741">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="0bba9-3742">Tests für Service Fabric-Befehle hinzugefügt (3424)</span><span class="sxs-lookup"><span data-stu-id="0bba9-3742">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="0bba9-3743">Zahlreiche Service Fabric-Befehle korrigiert (3234)</span><span class="sxs-lookup"><span data-stu-id="0bba9-3743">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="0bba9-3744">SQL</span><span class="sxs-lookup"><span data-stu-id="0bba9-3744">SQL</span></span>

* <span data-ttu-id="0bba9-3745">Fehlerhafte1 Parameter `--identity` für `sql server create` entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3745">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="0bba9-3746">Kennwortwerte aus der Befehlsausgabe von `sql server create` und `sql server update` entfernt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3746">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="0bba9-3747">Befehle `sql db list-editions` und `sql elastic-pool list-editions` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3747">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="0bba9-3748">Storage</span><span class="sxs-lookup"><span data-stu-id="0bba9-3748">Storage</span></span>

* <span data-ttu-id="0bba9-3749">Option `--marker` für die Befehle `storage blob list`, `storage container list` und `storage share list` entfernt (3745)</span><span class="sxs-lookup"><span data-stu-id="0bba9-3749">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="0bba9-3750">Erstellung eines reinen HTTPS-Speicherkontos ermöglicht</span><span class="sxs-lookup"><span data-stu-id="0bba9-3750">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="0bba9-3751">Speichermetriken, Protokollierung und CORS-Befehle aktualisiert (3495)</span><span class="sxs-lookup"><span data-stu-id="0bba9-3751">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="0bba9-3752">Ausnahmemeldung von „cors add“ umformuliert (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="0bba9-3752">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="0bba9-3753">Generator im Probelaufmodus des Downloadbatchbefehls in eine Liste konvertiert (3592)</span><span class="sxs-lookup"><span data-stu-id="0bba9-3753">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="0bba9-3754">Problem bei Probelauf des Blobdownloadbatchs behoben (3640) (3592)</span><span class="sxs-lookup"><span data-stu-id="0bba9-3754">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="0bba9-3755">VM</span><span class="sxs-lookup"><span data-stu-id="0bba9-3755">VM</span></span>

* <span data-ttu-id="0bba9-3756">Unterstützung der NSG-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="0bba9-3756">Support configuring nsg</span></span>
* <span data-ttu-id="0bba9-3757">Fehler behoben, aufgrund dessen der DNS-Server nicht ordnungsgemäß konfiguriert wurde</span><span class="sxs-lookup"><span data-stu-id="0bba9-3757">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="0bba9-3758">Unterstützung verwalteter Dienstidentitäten</span><span class="sxs-lookup"><span data-stu-id="0bba9-3758">Support managed service identities</span></span>
* <span data-ttu-id="0bba9-3759">Problem behoben, aufgrund dessen `cmss create` mit einem vorhandenen Lastenausgleich `--backend-pool-name` benötigte</span><span class="sxs-lookup"><span data-stu-id="0bba9-3759">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="0bba9-3760">Festlegung, dass die LUN von mit `vm image create` erstellten Datenträgern mit 0 beginnt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3760">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="0bba9-3761">10. Mai 2017</span><span class="sxs-lookup"><span data-stu-id="0bba9-3761">May 10, 2017</span></span>

<span data-ttu-id="0bba9-3762">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="0bba9-3762">Version 2.0.6</span></span>

* <span data-ttu-id="0bba9-3763">Umbenennen von „documentdb“ in „cosmosdb“</span><span class="sxs-lookup"><span data-stu-id="0bba9-3763">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="0bba9-3764">Hinzufügen von rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="0bba9-3764">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="0bba9-3765">Einbeziehen der Data Lake Analytics- und Data Lake Store-Module</span><span class="sxs-lookup"><span data-stu-id="0bba9-3765">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="0bba9-3766">Einbeziehen des Cognitive Services-Moduls</span><span class="sxs-lookup"><span data-stu-id="0bba9-3766">Include Cognitive Services module</span></span>
* <span data-ttu-id="0bba9-3767">Einbeziehen des Service Fabric-Moduls</span><span class="sxs-lookup"><span data-stu-id="0bba9-3767">Include Service Fabric module</span></span>
* <span data-ttu-id="0bba9-3768">Einbeziehen des interaktiven Moduls (Umbenennen von „az-shell“)</span><span class="sxs-lookup"><span data-stu-id="0bba9-3768">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="0bba9-3769">Hinzufügen von Unterstützung für CDN-Befehle</span><span class="sxs-lookup"><span data-stu-id="0bba9-3769">Add support for CDN commands</span></span>
* <span data-ttu-id="0bba9-3770">Entfernen des Containermoduls</span><span class="sxs-lookup"><span data-stu-id="0bba9-3770">Remove Container module</span></span>
* <span data-ttu-id="0bba9-3771">Hinzufügen von „az -v“ als Verknüpfung für „az --version“ ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="0bba9-3771">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="0bba9-3772">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="0bba9-3772">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="0bba9-3773">Core</span><span class="sxs-lookup"><span data-stu-id="0bba9-3773">Core</span></span>

* <span data-ttu-id="0bba9-3774">Core: Erfassen von Ausnahmen, die durch einen nicht registrierten Anbieter verursacht werden, und automatische Registrierung</span><span class="sxs-lookup"><span data-stu-id="0bba9-3774">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="0bba9-3775">Leistung: Dauerhaftes Speichern des ADAL-Tokencaches im Arbeitsspeicher bis zum Prozessende ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="0bba9-3775">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="0bba9-3776">Korrigieren der vom hexadezimalen Fingerabdruck -o tsv zurückgegebenen Bytes ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="0bba9-3776">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="0bba9-3777">Verbessern des Downloads des Schlüsseltresorzertifikats und der AAD-SP-Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="0bba9-3777">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="0bba9-3778">Hinzufügen des Python-Speicherorts zu „az –version“ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="0bba9-3778">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="0bba9-3779">Anmeldung: Unterstützung der Anmeldung, wenn keine Abonnements vorhanden sind ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="0bba9-3779">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="0bba9-3780">Core: Beheben eines Fehlers bei zweimaliger Verwendung eines Dienstprinzipals bei der Anmeldung ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="0bba9-3780">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="0bba9-3781">Core: Ermöglichen der Konfiguration des Dateipfads von „accessTokens.json“ über eine Umgebungsvariable ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="0bba9-3781">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="0bba9-3782">Core: Zulassen der Anwendung konfigurierter Standardwerte auf optionale Argumente ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="0bba9-3782">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="0bba9-3783">Core: Verbesserte Leistung</span><span class="sxs-lookup"><span data-stu-id="0bba9-3783">core: Improved performance</span></span>
* <span data-ttu-id="0bba9-3784">Core: Zertifikate von benutzerdefinierter Zertifizierungsstelle – Unterstützung für das Festlegen der REQUESTS_CA_BUNDLE-Umgebungsvariablen</span><span class="sxs-lookup"><span data-stu-id="0bba9-3784">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="0bba9-3785">Core: Cloudkonfiguration – Verwenden des Endpunkts „resource manager“, wenn Endpunkt „management“ nicht festgelegt ist</span><span class="sxs-lookup"><span data-stu-id="0bba9-3785">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="0bba9-3786">ACS</span><span class="sxs-lookup"><span data-stu-id="0bba9-3786">ACS</span></span>

* <span data-ttu-id="0bba9-3787">Korrigieren der Master- und Agentanzahl als ganze Zahl statt Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0bba9-3787">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="0bba9-3788">Verfügbarmachen von „az acs create --no-wait“ und „az acs wait“ für die asynchrone Erstellung</span><span class="sxs-lookup"><span data-stu-id="0bba9-3788">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="0bba9-3789">Verfügbarmachen von „az acs create --validate“ für Probelaufüberprüfungen</span><span class="sxs-lookup"><span data-stu-id="0bba9-3789">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="0bba9-3790">Entfernen von Windows-Profil vor PUT-Aufruf für Skalierungsbefehl ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="0bba9-3790">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="0bba9-3791">AppService</span><span class="sxs-lookup"><span data-stu-id="0bba9-3791">AppService</span></span>

* <span data-ttu-id="0bba9-3792">functionapp: Hinzufügen der vollständigen functionapp-Unterstützung, einschließlich Erstellen, Anzeigen, Auflisten, Löschen, Hostname, SSL usw.</span><span class="sxs-lookup"><span data-stu-id="0bba9-3792">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="0bba9-3793">Hinzufügen von Team Services (vsts) als Continuous Delivery-Option zu „appservice web source-control config“</span><span class="sxs-lookup"><span data-stu-id="0bba9-3793">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="0bba9-3794">Erstellen von „az webapp“ als Ersatz für „az appservice web“ (für Abwärtskompatibilität bleibt „az appservice web“ für 2 weitere Releases erhalten)</span><span class="sxs-lookup"><span data-stu-id="0bba9-3794">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="0bba9-3795">Verfügbarmachen von Argumenten zum Konfigurieren von Bereitstellung und Laufzeitstapeln beim Erstellen von Web-Apps</span><span class="sxs-lookup"><span data-stu-id="0bba9-3795">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="0bba9-3796">Verfügbarmachen von „webapp list-runtimes“</span><span class="sxs-lookup"><span data-stu-id="0bba9-3796">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="0bba9-3797">Unterstützen der Konfiguration von Verbindungszeichenfolgen ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="0bba9-3797">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="0bba9-3798">Unterstützen des Slottauschs mit Vorschau</span><span class="sxs-lookup"><span data-stu-id="0bba9-3798">support slot swap with preview</span></span>
* <span data-ttu-id="0bba9-3799">Beheben von Fehlern in appservice-Befehlen ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="0bba9-3799">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="0bba9-3800">Verwenden der Ressourcengruppe des App Service-Plans für Zertifizierungsvorgänge ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="0bba9-3800">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="0bba9-3801">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="0bba9-3801">CosmosDB</span></span>

* <span data-ttu-id="0bba9-3802">Umbenennen des documentdb-Moduls in cosmosdb</span><span class="sxs-lookup"><span data-stu-id="0bba9-3802">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="0bba9-3803">Zusätzliche Unterstützung für documentdb-APIs auf Datenebene: Datenbank- und Sammlungsverwaltung</span><span class="sxs-lookup"><span data-stu-id="0bba9-3803">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="0bba9-3804">Zusätzliche Unterstützung für das Aktivieren des automatischen Failovers für Datenbankkonten</span><span class="sxs-lookup"><span data-stu-id="0bba9-3804">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="0bba9-3805">Zusätzliche Unterstützung für die neue ConsistentPrefix-Konsistenzrichtlinie</span><span class="sxs-lookup"><span data-stu-id="0bba9-3805">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="0bba9-3806">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="0bba9-3806">Data Lake Analytics</span></span>

* <span data-ttu-id="0bba9-3807">Beheben eines Fehlers, bei dem das Filtern von Auftragslisten nach Ergebnis und Status einen Fehler auslöst</span><span class="sxs-lookup"><span data-stu-id="0bba9-3807">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="0bba9-3808">Hinzufügen von Unterstützung für den neuen Katalogelementtyp „Paket“</span><span class="sxs-lookup"><span data-stu-id="0bba9-3808">Add support for new catalog item type: package.</span></span> <span data-ttu-id="0bba9-3809">Zugriff über: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="0bba9-3809">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="0bba9-3810">Ermöglichen der Auflistung folgender Katalogelemente innerhalb einer Datenbank (keine Schemaspezifikation erforderlich):</span><span class="sxs-lookup"><span data-stu-id="0bba9-3810">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="0bba9-3811">Tabelle</span><span class="sxs-lookup"><span data-stu-id="0bba9-3811">Table</span></span>
  * <span data-ttu-id="0bba9-3812">Tabellenwertfunktion</span><span class="sxs-lookup"><span data-stu-id="0bba9-3812">Table valued function</span></span>
  * <span data-ttu-id="0bba9-3813">Sicht</span><span class="sxs-lookup"><span data-stu-id="0bba9-3813">View</span></span>
  * <span data-ttu-id="0bba9-3814">Tabellenstatistiken.</span><span class="sxs-lookup"><span data-stu-id="0bba9-3814">Table Statistics.</span></span> <span data-ttu-id="0bba9-3815">Können auch mit einem Schema, jedoch ohne Angabe eines Tabellennamens aufgelistet werden.</span><span class="sxs-lookup"><span data-stu-id="0bba9-3815">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="0bba9-3816">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="0bba9-3816">Data Lake Store</span></span>

* <span data-ttu-id="0bba9-3817">Aktualisieren der Version des zugrunde liegenden Dateisystem-SDK, wodurch eine bessere Unterstützung für die Verarbeitung von Drosselungsszenarien auf Serverseite gewährt wird</span><span class="sxs-lookup"><span data-stu-id="0bba9-3817">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="0bba9-3818">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="0bba9-3818">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="0bba9-3819">Fehlende Hilfe für Zugriffsanzeige</span><span class="sxs-lookup"><span data-stu-id="0bba9-3819">missed help for access show.</span></span> <span data-ttu-id="0bba9-3820">hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="0bba9-3820">adding it.</span></span> <span data-ttu-id="0bba9-3821">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="0bba9-3821">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="0bba9-3822">Suchen</span><span class="sxs-lookup"><span data-stu-id="0bba9-3822">Find</span></span>

* <span data-ttu-id="0bba9-3823">Verbessern von Suchergebnissen und Ermöglichen der Versionsverwaltung des Suchindex</span><span class="sxs-lookup"><span data-stu-id="0bba9-3823">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="0bba9-3824">KeyVault</span><span class="sxs-lookup"><span data-stu-id="0bba9-3824">KeyVault</span></span>

* <span data-ttu-id="0bba9-3825">BC:`az keyvault certificate download` Ändern von „-e“ von Zeichenfolge oder Binärdatentyp in PEM oder DER zur besseren Darstellung der Optionen</span><span class="sxs-lookup"><span data-stu-id="0bba9-3825">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="0bba9-3826">BC: Entfernen von „--expires“ und „--not-before“ aus `keyvault certificate create`, da diese Parameter nicht vom Dienst unterstützt werden</span><span class="sxs-lookup"><span data-stu-id="0bba9-3826">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="0bba9-3827">Hinzufügen des Parameters „--validity“ zu `keyvault certificate create`, um gezielt den Wert in „--policy“ zu überschreiben</span><span class="sxs-lookup"><span data-stu-id="0bba9-3827">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="0bba9-3828">Beheben des Problems in `keyvault certificate get-default-policy`, bei dem „expires“ und „not_before“ verfügbar gemacht wurden, „validity_in_months“ hingegen nicht</span><span class="sxs-lookup"><span data-stu-id="0bba9-3828">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="0bba9-3829">Keyvault-Korrektur für den Import von PEM und PFX ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="0bba9-3829">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="0bba9-3830">Labor</span><span class="sxs-lookup"><span data-stu-id="0bba9-3830">Lab</span></span>

* <span data-ttu-id="0bba9-3831">Hinzufügen der Befehle „create“, „show“, „delete“ und „list“ für die Laborumgebung</span><span class="sxs-lookup"><span data-stu-id="0bba9-3831">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="0bba9-3832">Hinzufügen der Befehle „show“ und „list“ zur Anzeige von ARM-Vorlagen im Labor</span><span class="sxs-lookup"><span data-stu-id="0bba9-3832">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="0bba9-3833">Hinzufügen des Kennzeichens „--environment“ in `az lab vm list`, um virtuelle Computer nach Umgebung im Labor zu filtern</span><span class="sxs-lookup"><span data-stu-id="0bba9-3833">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="0bba9-3834">Hinzufügen des benutzerfreundlichen Befehls `az lab formula export-artifacts` zum Exportieren des Artefaktgerüsts innerhalb der Formel eines Labors</span><span class="sxs-lookup"><span data-stu-id="0bba9-3834">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="0bba9-3835">Hinzufügen von Befehlen zum Verwalten von Geheimnissen in einem Labor</span><span class="sxs-lookup"><span data-stu-id="0bba9-3835">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="0bba9-3836">Überwachen</span><span class="sxs-lookup"><span data-stu-id="0bba9-3836">Monitor</span></span>

* <span data-ttu-id="0bba9-3837">Fehlerbehebung: Modellieren von `--actions` von `az alert-rules create` zum Verarbeiten von JSON-Zeichenfolgen ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="0bba9-3837">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="0bba9-3838">Programmfehlerbehebung: Beim Erstellen von Diagnoseeinstellungen werden Protokolle/Metriken aus Anzeigebefehlen nicht akzeptiert ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="0bba9-3838">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="0bba9-3839">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0bba9-3839">Network</span></span>

* <span data-ttu-id="0bba9-3840">Hinzufügen des `network watcher test-connectivity`-Befehls</span><span class="sxs-lookup"><span data-stu-id="0bba9-3840">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="0bba9-3841">Hinzufügen von Unterstützung für den `--filters`-Parameter für `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="0bba9-3841">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="0bba9-3842">Hinzufügen von Unterstützung für den Application Gateway-Verbindungsausgleich</span><span class="sxs-lookup"><span data-stu-id="0bba9-3842">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="0bba9-3843">Hinzufügen von Unterstützung für die Konfiguration von Application Gateway-WAF-Regelsätzen</span><span class="sxs-lookup"><span data-stu-id="0bba9-3843">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="0bba9-3844">Hinzufügen von Unterstützung für ExpressRoute-Routenfilter und -Regeln</span><span class="sxs-lookup"><span data-stu-id="0bba9-3844">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="0bba9-3845">Hinzufügen von Unterstützung für geografisches TrafficManager-Routing</span><span class="sxs-lookup"><span data-stu-id="0bba9-3845">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="0bba9-3846">Hinzufügen von Unterstützung für richtlinienbasierte Datenverkehrsselektoren für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="0bba9-3846">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="0bba9-3847">Hinzufügen von Unterstützung für IPSec-Richtlinien für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="0bba9-3847">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="0bba9-3848">Korrektur eines Fehlers bei `vpn-connection create` bei Verwendung der Parameter `--no-wait` oder `--validate`</span><span class="sxs-lookup"><span data-stu-id="0bba9-3848">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="0bba9-3849">Hinzufügen von Unterstützung für Aktiv/Aktiv-VNET-Gateways</span><span class="sxs-lookup"><span data-stu-id="0bba9-3849">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="0bba9-3850">Entfernen von NULL-Werten aus der Ausgabe von `network vpn-connection list/show`-Befehlen</span><span class="sxs-lookup"><span data-stu-id="0bba9-3850">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="0bba9-3851">BC: Korrektur eines Fehlers in der Ausgabe von `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="0bba9-3851">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="0bba9-3852">Korrektur eines Fehlers, bei dem das Argument „--key-length“ von „vpn-connection create“ nicht ordnungsgemäß analysiert wurde</span><span class="sxs-lookup"><span data-stu-id="0bba9-3852">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="0bba9-3853">Korrektur eines Fehlers in `dns zone import`, bei dem Datensätze nicht ordnungsgemäß importiert wurden</span><span class="sxs-lookup"><span data-stu-id="0bba9-3853">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="0bba9-3854">Korrektur eines Fehlers, bei dem `traffic-manager endpoint update` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="0bba9-3854">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="0bba9-3855">Hinzufügen von Network Watcher-Vorschaubefehlen</span><span class="sxs-lookup"><span data-stu-id="0bba9-3855">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="0bba9-3856">Profil</span><span class="sxs-lookup"><span data-stu-id="0bba9-3856">Profile</span></span>

* <span data-ttu-id="0bba9-3857">Unterstützung der Anmeldung, wenn keine Abonnements gefunden werden ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="0bba9-3857">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="0bba9-3858">Unterstützung für kurze Parameternamen in „az account set --subscription“ ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="0bba9-3858">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="0bba9-3859">Redis</span><span class="sxs-lookup"><span data-stu-id="0bba9-3859">Redis</span></span>

* <span data-ttu-id="0bba9-3860">Hinzufügen des Updatebefehls, durch den auch die Möglichkeit zum Skalieren für Redis Cache hinzugefügt wird</span><span class="sxs-lookup"><span data-stu-id="0bba9-3860">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="0bba9-3861">Verwerfen des Befehls „update-settings“</span><span class="sxs-lookup"><span data-stu-id="0bba9-3861">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="0bba9-3862">Resource</span><span class="sxs-lookup"><span data-stu-id="0bba9-3862">Resource</span></span>

* <span data-ttu-id="0bba9-3863">Hinzufügen der Befehle „managedapp“ und „managedapp definition“ ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="0bba9-3863">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="0bba9-3864">Unterstützung für die „provider operation“-Befehle ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="0bba9-3864">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="0bba9-3865">Unterstützung für die Erstellung generischer Ressourcen ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="0bba9-3865">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="0bba9-3866">Korrigieren der Ressourcenanalyse und der API-Versionssuche</span><span class="sxs-lookup"><span data-stu-id="0bba9-3866">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="0bba9-3867">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="0bba9-3867">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="0bba9-3868">Hinzufügen von Dokumenten für „az lock update“</span><span class="sxs-lookup"><span data-stu-id="0bba9-3868">Add docs for az lock update.</span></span> <span data-ttu-id="0bba9-3869">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="0bba9-3869">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="0bba9-3870">Beenden mit Fehler bei dem Versuch, Ressourcen für eine nicht vorhandene Gruppe aufzulisten</span><span class="sxs-lookup"><span data-stu-id="0bba9-3870">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="0bba9-3871">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="0bba9-3871">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="0bba9-3872">[Compute] Beheben von Problemen mit dem Update von VMSS- und VM-Verfügbarkeitsgruppen</span><span class="sxs-lookup"><span data-stu-id="0bba9-3872">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="0bba9-3873">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="0bba9-3873">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="0bba9-3874">Korrigieren des Erstellungs- und Löschvorgangs für Sperren, wenn „parent-resource-path“ auf „None“ festgelegt ist ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="0bba9-3874">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="0bba9-3875">Role</span><span class="sxs-lookup"><span data-stu-id="0bba9-3875">Role</span></span>

* <span data-ttu-id="0bba9-3876">create-for-rbac: Sicherstellen, dass das SP-Enddatum nicht das Ablaufdatum des Zertifikats überschreitet ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="0bba9-3876">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="0bba9-3877">RBAC: Hinzufügen vollständiger Unterstützung für „ad group“ ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="0bba9-3877">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="0bba9-3878">Rolle: Beheben von Probleme beim Rollendefinitionsupdate ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="0bba9-3878">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="0bba9-3879">create-for-rbac: Sicherstellen, dass das angegebene Benutzerkennwort übernommen wird</span><span class="sxs-lookup"><span data-stu-id="0bba9-3879">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="0bba9-3880">SQL</span><span class="sxs-lookup"><span data-stu-id="0bba9-3880">SQL</span></span>

* <span data-ttu-id="0bba9-3881">Hinzufügen der Befehle „az sql server list-usages“ und „az sql db list-usages“</span><span class="sxs-lookup"><span data-stu-id="0bba9-3881">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="0bba9-3882">SQL: Möglichkeit zur direkten Verbindung mit Ressourcenanbieter ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="0bba9-3882">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="0bba9-3883">Storage</span><span class="sxs-lookup"><span data-stu-id="0bba9-3883">Storage</span></span>

* <span data-ttu-id="0bba9-3884">Festlegen des Ressourcengruppenstandorts als Standardstandort für `storage account create`</span><span class="sxs-lookup"><span data-stu-id="0bba9-3884">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="0bba9-3885">Hinzufügen von Unterstützung für das inkrementelle Kopieren von Blobs</span><span class="sxs-lookup"><span data-stu-id="0bba9-3885">Add support for incremental blob copy</span></span>
* <span data-ttu-id="0bba9-3886">Hinzufügen von Unterstützung für den Upload umfangreicher Blockblobs</span><span class="sxs-lookup"><span data-stu-id="0bba9-3886">Add support for large block blob upload</span></span>
* <span data-ttu-id="0bba9-3887">Ändern der Blockgröße auf 100 MB, wenn die hochzuladende Datei größer als 200 GB ist</span><span class="sxs-lookup"><span data-stu-id="0bba9-3887">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="0bba9-3888">VM</span><span class="sxs-lookup"><span data-stu-id="0bba9-3888">VM</span></span>

* <span data-ttu-id="0bba9-3889">avail-set: Festlegen der UD- und FD-Domänenanzahl als optional</span><span class="sxs-lookup"><span data-stu-id="0bba9-3889">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="0bba9-3890">Hinweis: VM-Befehle in unabhängigen Clouds: Vermeiden Sie Features im Zusammenhang mit verwalteten Datenträgern, einschließlich der folgenden:</span><span class="sxs-lookup"><span data-stu-id="0bba9-3890">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="0bba9-3891">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="0bba9-3891">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="0bba9-3892">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="0bba9-3892">az vm/vmss disk</span></span>
  3. <span data-ttu-id="0bba9-3893">Verwenden Sie in „az vm/vmss create“ den Befehl „—use-unmanaged-disk“, um verwaltete Datenträger zu vermeiden. Andere Befehle sollten funktionieren.</span><span class="sxs-lookup"><span data-stu-id="0bba9-3893">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="0bba9-3894">vm/vmss: Verbessern des Warnungstexts beim Generieren von SSH-Schlüsselpaaren</span><span class="sxs-lookup"><span data-stu-id="0bba9-3894">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="0bba9-3895">vm/vmss: Unterstützen der Erstellung über ein Marketplace-Image, für das Planinformationen erforderlich sind ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="0bba9-3895">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="0bba9-3896">3\. April 2017</span><span class="sxs-lookup"><span data-stu-id="0bba9-3896">April 3, 2017</span></span>

<span data-ttu-id="0bba9-3897">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="0bba9-3897">Version 2.0.2</span></span>

<span data-ttu-id="0bba9-3898">In dieser Version wurden die Komponenten ACR, Batch, KeyVault und SQL eingeführt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-3898">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="0bba9-3899">Core</span><span class="sxs-lookup"><span data-stu-id="0bba9-3899">Core</span></span>

* <span data-ttu-id="0bba9-3900">Hinzufügen der Module „acr“, „lab“, „monitor“ und „find“ zur Standardliste</span><span class="sxs-lookup"><span data-stu-id="0bba9-3900">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="0bba9-3901">Anmeldung: Überspringen des fehlerhaften Mandanten ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="0bba9-3901">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="0bba9-3902">Anmeldung: Festlegen des Standardabonnements auf ein Abonnement mit dem Status „Enabled“ ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="0bba9-3902">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="0bba9-3903">Hinzufügen von wait-Befehlen und Unterstützung von „--no-wait“ für mehr Befehle ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="0bba9-3903">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="0bba9-3904">Core: Unterstützen der Anmeldung per Dienstprinzipal mit einem Zertifikat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="0bba9-3904">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="0bba9-3905">Hinzufügen der Meldung zu fehlenden Vorlagenparametern</span><span class="sxs-lookup"><span data-stu-id="0bba9-3905">Add prompting for missing template parameters.</span></span> <span data-ttu-id="0bba9-3906">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="0bba9-3906">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="0bba9-3907">Unterstützen des Festlegens von Standardwerten für häufig verwendete Argumente, z.B. Standardressourcengruppe, Standardweb und Standard-VM</span><span class="sxs-lookup"><span data-stu-id="0bba9-3907">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="0bba9-3908">Unterstützen der Anmeldung an einem bestimmten Mandanten</span><span class="sxs-lookup"><span data-stu-id="0bba9-3908">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="0bba9-3909">ACS</span><span class="sxs-lookup"><span data-stu-id="0bba9-3909">ACS</span></span>

* <span data-ttu-id="0bba9-3910">[ACS] Hinzufügen von Unterstützung für die Konfiguration eines ACS-Standardclusters ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="0bba9-3910">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="0bba9-3911">Hinzufügen von Unterstützung der Aufforderung zur Kennworteingabe für SSH-Schlüssel</span><span class="sxs-lookup"><span data-stu-id="0bba9-3911">Add support for ssh key password prompting.</span></span> <span data-ttu-id="0bba9-3912">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="0bba9-3912">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="0bba9-3913">Hinzufügen von Unterstützung für Windows-Cluster</span><span class="sxs-lookup"><span data-stu-id="0bba9-3913">Add support for windows clusters.</span></span> <span data-ttu-id="0bba9-3914">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="0bba9-3914">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="0bba9-3915">Wechseln von der Rolle „Besitzer“ zur Rolle „Mitwirkender“</span><span class="sxs-lookup"><span data-stu-id="0bba9-3915">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="0bba9-3916">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="0bba9-3916">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="0bba9-3917">AppService</span><span class="sxs-lookup"><span data-stu-id="0bba9-3917">AppService</span></span>

* <span data-ttu-id="0bba9-3918">appservice: Unterstützung für das Abrufen der externen IP-Adresse für DNS A-Einträge ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="0bba9-3918">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="0bba9-3919">appservice: Unterstützung der Bindung von Platzhalterzertifikaten ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="0bba9-3919">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="0bba9-3920">appservice: Unterstützung von Veröffentlichungsprofilen für Listen ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="0bba9-3920">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="0bba9-3921">AppService: Auslösen der Synchronisierung der Quellcodeverwaltung nach der Konfiguration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="0bba9-3921">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="0bba9-3922">DataLake</span><span class="sxs-lookup"><span data-stu-id="0bba9-3922">DataLake</span></span>

* <span data-ttu-id="0bba9-3923">Erste Version des Data Lake Analytics-Moduls</span><span class="sxs-lookup"><span data-stu-id="0bba9-3923">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="0bba9-3924">Erste Version des Data Lake Store-Moduls</span><span class="sxs-lookup"><span data-stu-id="0bba9-3924">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="0bba9-3925">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="0bba9-3925">DocuemntDB</span></span>

* <span data-ttu-id="0bba9-3926">DocumentDB: Hinzufügen von Unterstützung für das Auflisten von Verbindungszeichenfolgen ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="0bba9-3926">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="0bba9-3927">VM</span><span class="sxs-lookup"><span data-stu-id="0bba9-3927">VM</span></span>

* <span data-ttu-id="0bba9-3928">[Compute] Hinzufügen von AppGateway-Unterstützung für Erstellung von VM-Skalierungsgruppen ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="0bba9-3928">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="0bba9-3929">[VM/VMSS] Verbesserte Unterstützung für die Datenträgerzwischenspeicherung ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="0bba9-3929">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="0bba9-3930">VM/VMSS: Einbinden der vom Portal verwendeten Logik zur Überprüfung von Anmeldeinformationen ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="0bba9-3930">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="0bba9-3931">Hinzufügen von wait-Befehlen und Unterstützung für „--no-wait“ ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="0bba9-3931">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="0bba9-3932">VM-Skalierungsgruppe: Unterstützung von „\*“ zum Auflisten der übergreifenden Instanzansicht für VMs ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="0bba9-3932">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="0bba9-3933">Hinzufügen – Geheimnisse für virtuellen Computer und VM-Skalierungsgruppe ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="0bba9-3933">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="0bba9-3934">Zulassen der VM-Erstellung mit spezialisierter VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="0bba9-3934">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="0bba9-3935">27. Februar 2017</span><span class="sxs-lookup"><span data-stu-id="0bba9-3935">February 27, 2017</span></span>

<span data-ttu-id="0bba9-3936">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="0bba9-3936">Version 2.0.0</span></span>

<span data-ttu-id="0bba9-3937">Diese Version der Azure CLI 2.0 ist die erste „allgemein verfügbare“ Version. Die allgemeine Verfügbarkeit gilt für die folgenden Befehlsmodule:</span><span class="sxs-lookup"><span data-stu-id="0bba9-3937">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="0bba9-3938">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="0bba9-3938">Container Service (acs)</span></span>
- <span data-ttu-id="0bba9-3939">Compute (einschließlich Resource Manager, VM, VM-Skalierungsgruppen, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="0bba9-3939">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="0bba9-3940">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="0bba9-3940">Networking</span></span>
- <span data-ttu-id="0bba9-3941">Storage</span><span class="sxs-lookup"><span data-stu-id="0bba9-3941">Storage</span></span>

<span data-ttu-id="0bba9-3942">Diese Befehlsmodule können in der Produktion verwendet werden und verfügen über Unterstützung durch eine Standard-SLA von Microsoft. Sie können Anfragen zu Problemen direkt beim Microsoft-Support oder in der [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/) öffnen. Sie haben die Möglichkeit, Fragen in [StackOverflow mit dem Tag „azure-cli“](http://stackoverflow.com/questions/tagged/azure-cli) zu stellen oder sich unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) an das Produktteam zu wenden. Außerdem können Sie über die Befehlszeile mit dem Befehl `az feedback` Feedback senden.</span><span class="sxs-lookup"><span data-stu-id="0bba9-3942">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="0bba9-3943">Die Befehle in diesen Modulen sind stabil, und es ist nicht zu erwarten, dass sich die Syntax in den anstehenden Veröffentlichungen dieser Version der Azure CLI ändern.</span><span class="sxs-lookup"><span data-stu-id="0bba9-3943">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="0bba9-3944">Verwenden Sie zum Überprüfen der Version der CLI den Befehl `az --version`. In der Ausgabe werden die Version der CLI selbst (für diese Veröffentlichung 2.0.0), die einzelnen Befehlsmodule und die von Ihnen genutzten Versionen von Python und GCC aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-3944">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="0bba9-3945">Einige Befehlsmodule verfügen über das Postfix „b*n*“ oder „rc*n*“. Diese Befehlsmodule befinden sich noch in der Vorschauphase und werden später die allgemeine Verfügbarkeit erlangen.</span><span class="sxs-lookup"><span data-stu-id="0bba9-3945">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="0bba9-3946">Außerdem werden jeden Abend Vorschaubuilds der CLI bereitgestellt. Informationen hierzu finden Sie in der [Anleitung zum Abrufen der abendlichen Builds](https://github.com/Azure/azure-cli#nightly-builds) und im Abschnitt zum [Setup für Entwickler und Beitragen von Code](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="0bba9-3946">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="0bba9-3947">Sie können für die abendlichen Vorschaubuilds wie folgt Probleme melden:</span><span class="sxs-lookup"><span data-stu-id="0bba9-3947">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="0bba9-3948">Über die [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="0bba9-3948">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="0bba9-3949">Per Kontaktaufnahme mit dem Produktteam unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="0bba9-3949">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="0bba9-3950">Senden von Feedback über die Befehlszeile mit dem Befehl `az feedback`</span><span class="sxs-lookup"><span data-stu-id="0bba9-3950">Provide feedback from the command line with the `az feedback` command</span></span>

# <a name="beta-release-notes"></a>[<span data-ttu-id="0bba9-3951">Versionshinweise zur Betaversion</span><span class="sxs-lookup"><span data-stu-id="0bba9-3951">Beta release notes</span></span>](#tab/azure-cli-beta)

<span data-ttu-id="0bba9-3952">Die Azure CLI-Betaversion ist eine Migration der Authentifizierungsmethode der AAD-Plattform (v1.0) zu [Microsoft Identity Platform (v2.0)](/azure/active-directory/develop/v2-overview).</span><span class="sxs-lookup"><span data-stu-id="0bba9-3952">The Azure CLI beta release is a migration from the authentican method of AAD platform (v1.0) to [Microsoft Identity platform (v2.0)](/azure/active-directory/develop/v2-overview).</span></span>

## <a name="june-23-2020"></a><span data-ttu-id="0bba9-3953">23. Juni 2020</span><span class="sxs-lookup"><span data-stu-id="0bba9-3953">June 23, 2020</span></span>

### <a name="things-to-know-about-the-new-azure-cli-beta-release"></a><span data-ttu-id="0bba9-3954">Wissenswertes über die neue Azure CLI-Betaversion</span><span class="sxs-lookup"><span data-stu-id="0bba9-3954">Things to know about the new Azure CLI beta release</span></span>

-   <span data-ttu-id="0bba9-3955">Die Betaversion der Azure CLI unterstützt alle CLI-Befehle, die in der aktuellen veröffentlichten Version verfügbar sind.</span><span class="sxs-lookup"><span data-stu-id="0bba9-3955">The beta version of the Azure CLI supports all CLI commands that you will find in the current released version.</span></span>
-   <span data-ttu-id="0bba9-3956">Nach der Installation der Betaversion ist eine erneute Anmeldung erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0bba9-3956">Relogin is required after install the beta version.</span></span>
-   <span data-ttu-id="0bba9-3957">Die Betaversion unterstützt nur die Windows-Plattform.</span><span class="sxs-lookup"><span data-stu-id="0bba9-3957">The beta release only supports the Windows platform.</span></span>
-   <span data-ttu-id="0bba9-3958">Azure Stack wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-3958">The Azure Stack is not supported.</span></span>
-   <span data-ttu-id="0bba9-3959">Parameter `--use-cert-sn-issuer` wird nicht unterstützt, wenn für die Authentifizierung ein Dienstprinzipalschlüssel verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="0bba9-3959">`--use-cert-sn-issuer` parameter is not supported when using service principal key to authenticate.</span></span>
-   <span data-ttu-id="0bba9-3960">Das Überspringen der SSL-Überprüfung über die Umgebung `ADAL_PYTHON_SSL_NO_VERIFY` wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0bba9-3960">Skip SSL verification via environment `ADAL_PYTHON_SSL_NO_VERIFY` is not supported.</span></span>

<span data-ttu-id="0bba9-3961">Sollten Probleme in der Betaversion auftreten, können Sie auf [GitHub](https://github.com/Azure/azure-cli/issues/new/choose) gerne Kommentare für das Azure CLI-Entwicklungsteam hinterlassen.</span><span class="sxs-lookup"><span data-stu-id="0bba9-3961">If you find any issues in the beta release, the Azure CLI engineering team welcomes your comments on [GitHub](https://github.com/Azure/azure-cli/issues/new/choose).</span></span>

---

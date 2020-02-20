---
title: Versionshinweise für die Azure CLI
description: Enthält Informationen zu den aktuellen Updates der Azure CLI.
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 02/18/2020
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 6c07b93752df2dab6ca0b210675a48b5c7b85c1c
ms.sourcegitcommit: 91c1e5423bd054a948620999b559bc3a9828a688
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/19/2020
ms.locfileid: "77453476"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="aa5bc-103">Versionshinweise für die Azure CLI</span><span class="sxs-lookup"><span data-stu-id="aa5bc-103">Azure CLI release notes</span></span>

## <a name="february-18-2020"></a><span data-ttu-id="aa5bc-104">18. Februar 2020</span><span class="sxs-lookup"><span data-stu-id="aa5bc-104">February 18, 2020</span></span>

<span data-ttu-id="aa5bc-105">Version 2.1.0</span><span class="sxs-lookup"><span data-stu-id="aa5bc-105">Version 2.1.0</span></span>

### <a name="acr"></a><span data-ttu-id="aa5bc-106">ACR</span><span class="sxs-lookup"><span data-stu-id="aa5bc-106">ACR</span></span>

* <span data-ttu-id="aa5bc-107">Neues Argument `--expose-token` für `az acr login` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-107">Add a new argument `--expose-token` for `az acr login`</span></span>
* <span data-ttu-id="aa5bc-108">Falsche Ausgabe für `az acr task identity show -n Name -r Registry -o table` korrigiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-108">Fix the incorrect output of `az acr task identity show -n Name -r Registry -o table`</span></span>
* <span data-ttu-id="aa5bc-109">az acr login: Auslösen von „CLIError“, wenn vom Docker-Befehl Fehler zurückgegeben werden</span><span class="sxs-lookup"><span data-stu-id="aa5bc-109">az acr login: Throw a CLIError if there are errors returned by docker command</span></span>

### <a name="acs"></a><span data-ttu-id="aa5bc-110">ACS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-110">ACS</span></span>

* <span data-ttu-id="aa5bc-111">aks create/update: Validierung für `--vnet-subnet-id` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-111">aks create/update: add `--vnet-subnet-id` validation</span></span>

### <a name="aladdin"></a><span data-ttu-id="aa5bc-112">Aladdin</span><span class="sxs-lookup"><span data-stu-id="aa5bc-112">Aladdin</span></span>

* <span data-ttu-id="aa5bc-113">Analysieren der generierten Beispiele in „_help.py“ der Befehle</span><span class="sxs-lookup"><span data-stu-id="aa5bc-113">Parse generated examples into commands' _help.py</span></span>

### <a name="ams"></a><span data-ttu-id="aa5bc-114">AMS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-114">AMS</span></span>

* <span data-ttu-id="aa5bc-115">az ams ist jetzt allgemein verfügbar.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-115">az ams is GA now</span></span>

### <a name="appconfig"></a><span data-ttu-id="aa5bc-116">AppConfig</span><span class="sxs-lookup"><span data-stu-id="aa5bc-116">AppConfig</span></span>

* <span data-ttu-id="aa5bc-117">Hilfenachricht überarbeitet, um nicht unterstützte Schlüssel-/Bezeichnungsfilter auszuschließen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-117">Revise help message to exclude unsupported key/label filter</span></span>
* <span data-ttu-id="aa5bc-118">Vorschautag für die meisten Befehle entfernt (mit Ausnahme der Flags für verwaltete Identitäten und Features)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-118">Remove preview tag for most commands excluding managed identity and feature flags</span></span>
* <span data-ttu-id="aa5bc-119">Kundenseitig verwalteter Schlüssel beim Aktualisieren der Speicher hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-119">Add customer managed key when updating stores</span></span>

### <a name="appservice"></a><span data-ttu-id="aa5bc-120">AppService</span><span class="sxs-lookup"><span data-stu-id="aa5bc-120">AppService</span></span>

* <span data-ttu-id="aa5bc-121">az webapp list-runtimes: Fehler bei „list-runtimes“ behoben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-121">az webapp list-runtimes: Fix the bug for list-runtimes</span></span>
* <span data-ttu-id="aa5bc-122">„az webapp|functionapp config ssl create“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-122">Add az webapp|functionapp config ssl create</span></span>
* <span data-ttu-id="aa5bc-123">Unterstützung für v3-Funktions-Apps und Node 12</span><span class="sxs-lookup"><span data-stu-id="aa5bc-123">Add support for v3 function apps and node 12</span></span>

### <a name="arm"></a><span data-ttu-id="aa5bc-124">ARM</span><span class="sxs-lookup"><span data-stu-id="aa5bc-124">ARM</span></span>

* <span data-ttu-id="aa5bc-125">az policy assignment create: Fehlermeldung korrigiert, die angezeigt wird, wenn der Parameter `--policy` ungültig ist</span><span class="sxs-lookup"><span data-stu-id="aa5bc-125">az policy assignment create: Fix the error message when the `--policy` parameter is invalid</span></span>
* <span data-ttu-id="aa5bc-126">az group deployment create: Fehler „stat: path too long for Windows" korrigiert, der angezeigt wird, wenn eine zu große Datei vom Typ „parameters.json“ verwendet wird</span><span class="sxs-lookup"><span data-stu-id="aa5bc-126">az group deployment create: Fix "stat: path too long for Windows" error when using large parameters.json file</span></span>

### <a name="backup"></a><span data-ttu-id="aa5bc-127">Backup</span><span class="sxs-lookup"><span data-stu-id="aa5bc-127">Backup</span></span>

* <span data-ttu-id="aa5bc-128">Korrektur des Wiederherstellungsflows auf Elementebene am ursprünglichen Speicherort</span><span class="sxs-lookup"><span data-stu-id="aa5bc-128">Fix for item level recovery flow in OLR</span></span>
* <span data-ttu-id="aa5bc-129">Unterstützung von „Als Dateien wiederherstellen“ für SQL- und SAP-Datenbanken hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-129">Add restore as files support for SQL and SAP Databases</span></span>

### <a name="compute"></a><span data-ttu-id="aa5bc-130">Compute</span><span class="sxs-lookup"><span data-stu-id="aa5bc-130">Compute</span></span>

* <span data-ttu-id="aa5bc-131">vm/vmss/availability-set update: „--ppg“ hinzugefügt, um die Aktualisierung von „ProximityPlacementGroup“ zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-131">vm/vmss/availability-set update: add --ppg to allowing updating ProximityPlacementGroup</span></span>
* <span data-ttu-id="aa5bc-132">vmss create: „--data-disk-iops“ und „--data-disk-mbps“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-132">vmss create: add --data-disk-iops and --data-disk-mbps</span></span>
* <span data-ttu-id="aa5bc-133">az vm host: Vorschautag für `vm host` und `vm host group` entfernt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-133">az vm host: remove preview tag for `vm host` and `vm host group`</span></span>
* <span data-ttu-id="aa5bc-134">[BREAKING CHANGE] Behebung Nr. 10728: `az vm create`: Automatisches Erstellen des Subnetzes, wenn das VNET angegeben wird und das Subnetz nicht vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="aa5bc-134">[BREAKING CHANGE] Fix #10728: `az vm create`: create subnet automatically if vnet is specified and subnet not exists</span></span>
* <span data-ttu-id="aa5bc-135">Erhöhen der Stabilität von „vm image list“</span><span class="sxs-lookup"><span data-stu-id="aa5bc-135">Increase robustness of vm image list</span></span>

### <a name="eventhub"></a><span data-ttu-id="aa5bc-136">Eventhub</span><span class="sxs-lookup"><span data-stu-id="aa5bc-136">Eventhub</span></span>

* <span data-ttu-id="aa5bc-137">Azure Stack-Unterstützung für Profil „2019-03-01-hybrid“</span><span class="sxs-lookup"><span data-stu-id="aa5bc-137">Azure Stack support for 2019-03-01-hybrid profile</span></span>

### <a name="keyvault"></a><span data-ttu-id="aa5bc-138">KeyVault</span><span class="sxs-lookup"><span data-stu-id="aa5bc-138">KeyVault</span></span>

* <span data-ttu-id="aa5bc-139">az keyvault key create: neuer Wert `import` für Parameter `--ops` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-139">az keyvault key create: add a new value `import` for parameter `--ops`</span></span>
* <span data-ttu-id="aa5bc-140">az keyvault key list-versions: Unterstützung des Parameters `--id` für die Angabe von Schlüsseln</span><span class="sxs-lookup"><span data-stu-id="aa5bc-140">az keyvault key list-versions: support parameter `--id` for specifying keys</span></span>
* <span data-ttu-id="aa5bc-141">Unterstützung für Verbindungen mit privaten Endpunkten</span><span class="sxs-lookup"><span data-stu-id="aa5bc-141">Support private endpoint connections</span></span>

### <a name="network"></a><span data-ttu-id="aa5bc-142">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="aa5bc-142">Network</span></span>

* <span data-ttu-id="aa5bc-143">Geändert in „azure-mgmt-network 9.0.0“</span><span class="sxs-lookup"><span data-stu-id="aa5bc-143">Bump to azure-mgmt-network 9.0.0</span></span>
* <span data-ttu-id="aa5bc-144">az network private-link-service update/create: Unterstützung von „--enable-proxy-protocol“</span><span class="sxs-lookup"><span data-stu-id="aa5bc-144">az network private-link-service update/create: support --enable-proxy-protocol</span></span>
* <span data-ttu-id="aa5bc-145">Feature für Version 2 von Verbindungsmonitor hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-145">Add connection Monitor V2 feature</span></span>

### <a name="packaging"></a><span data-ttu-id="aa5bc-146">Verpackung</span><span class="sxs-lookup"><span data-stu-id="aa5bc-146">Packaging</span></span>

* <span data-ttu-id="aa5bc-147">[BREAKING CHANGE] Unterstützung für Python 2.7 eingestellt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-147">[BREAKING CHANGE] Drop support for Python 2.7</span></span>

### <a name="profile"></a><span data-ttu-id="aa5bc-148">Profil</span><span class="sxs-lookup"><span data-stu-id="aa5bc-148">Profile</span></span>

* <span data-ttu-id="aa5bc-149">Vorschau: Neue Attribute `homeTenantId` und `managedByTenants` zu Abonnementkonten hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-149">Preview: Add new attributes `homeTenantId` and `managedByTenants` to subscription accounts.</span></span> <span data-ttu-id="aa5bc-150">Führen Sie `az login` erneut aus, damit die Änderungen wirksam werden.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-150">Please re-run `az login` for the changes to take effect</span></span>
* <span data-ttu-id="aa5bc-151">az login: Eine Warnung wird angezeigt, wenn ein Abonnement von mehren Mandanten aufgeführt wird und der erste als Standard festgelegt wird.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-151">az login: Show a warning when a subscription is listed from more than one tenants and default to the first one.</span></span> <span data-ttu-id="aa5bc-152">Fügen Sie `--tenant` in `az login` ein, um beim Zugreifen auf dieses Abonnement einen bestimmten Mandanten auszuwählen.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-152">To select a specific tenant when accessing this subscription, please include `--tenant` in `az login`</span></span>

### <a name="role"></a><span data-ttu-id="aa5bc-153">Role</span><span class="sxs-lookup"><span data-stu-id="aa5bc-153">Role</span></span>

* <span data-ttu-id="aa5bc-154">az role assignment create: Problem behoben, das beim Zuweisen einer Rolle zu einem Dienstprinzipal nach Anzeigename einen Fehler vom Typ „HTTP 400“ verursachte</span><span class="sxs-lookup"><span data-stu-id="aa5bc-154">az role assignment create: Fix the error that assigning a role to a service principal by display name yields a HTTP 400</span></span>

### <a name="sql"></a><span data-ttu-id="aa5bc-155">SQL</span><span class="sxs-lookup"><span data-stu-id="aa5bc-155">SQL</span></span>

* <span data-ttu-id="aa5bc-156">Cmdlet `az sql mi update` der verwalteten SQL-Instanz mit zwei neuen Parametern aktualisiert: tier und family</span><span class="sxs-lookup"><span data-stu-id="aa5bc-156">Update SQL Managed Instance cmdlet `az sql mi update` with two new parameters: tier and family</span></span>

### <a name="storage"></a><span data-ttu-id="aa5bc-157">Storage</span><span class="sxs-lookup"><span data-stu-id="aa5bc-157">Storage</span></span>

* <span data-ttu-id="aa5bc-158">[BREAKING CHANGE] `az storage account create`: Art des Standardspeicherkontos in StorageV2 geändert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-158">[BREAKING CHANGE] `az storage account create`: Change default storage account kind to StorageV2</span></span>

## <a name="february-04-2020"></a><span data-ttu-id="aa5bc-159">04. Februar 2020</span><span class="sxs-lookup"><span data-stu-id="aa5bc-159">February 04, 2020</span></span>

<span data-ttu-id="aa5bc-160">Version 2.0.81</span><span class="sxs-lookup"><span data-stu-id="aa5bc-160">Version 2.0.81</span></span>

### <a name="acs"></a><span data-ttu-id="aa5bc-161">ACS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-161">ACS</span></span>

* <span data-ttu-id="aa5bc-162">Unterstützung für das Festlegen zugeordneter Ausgangsports und Leerlauftimeouts für Load Balancer Standard hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-162">Add support to set outbound allocated ports and idle timeouts on standard load balancer</span></span>
* <span data-ttu-id="aa5bc-163">Aktualisierung auf API-Version 2019-11-01</span><span class="sxs-lookup"><span data-stu-id="aa5bc-163">Update to API Version 2019-11-01</span></span>

### <a name="acr"></a><span data-ttu-id="aa5bc-164">ACR</span><span class="sxs-lookup"><span data-stu-id="aa5bc-164">ACR</span></span>

* <span data-ttu-id="aa5bc-165">[BREAKING CHANGE] `az acr delete` löst eine Eingabeaufforderung aus.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-165">[BREAKING CHANGE] `az acr delete` will prompt</span></span>
* <span data-ttu-id="aa5bc-166">[BREAKING CHANGE] „az acr task delete“ löst eine Eingabeaufforderung aus.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-166">[BREAKING CHANGE] 'az acr task delete' will prompt</span></span>
* <span data-ttu-id="aa5bc-167">Neue Befehlsgruppe „az acr taskrun show/list/delete“ für die Aufgabenausführungsverwaltung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-167">Add a new command group 'az acr taskrun show/list/delete' for taskrun management</span></span>

### <a name="aks"></a><span data-ttu-id="aa5bc-168">AKS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-168">AKS</span></span>

* <span data-ttu-id="aa5bc-169">Jeder Cluster erhält einen separaten Dienstprinzipal zur Verbesserung der Isolation.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-169">Each cluster gets a separate service principal to improve isolation</span></span>

### <a name="appconfig"></a><span data-ttu-id="aa5bc-170">AppConfig</span><span class="sxs-lookup"><span data-stu-id="aa5bc-170">AppConfig</span></span>

* <span data-ttu-id="aa5bc-171">Unterstützung für den Import/Export von KeyVault-Verweisen in/aus AppService</span><span class="sxs-lookup"><span data-stu-id="aa5bc-171">Support import/export of keyvault references from/to appservice</span></span>
* <span data-ttu-id="aa5bc-172">Unterstützung für den Import/Export aller Bezeichnungen in appconfig und aus appconfig</span><span class="sxs-lookup"><span data-stu-id="aa5bc-172">Support import/export of all labels from appconfig to appconfig</span></span>
* <span data-ttu-id="aa5bc-173">Überprüfen der Schlüssel- und Featurenamen vor dem Festlegen und Importieren</span><span class="sxs-lookup"><span data-stu-id="aa5bc-173">Validate key and feature names before setting and importing</span></span>
* <span data-ttu-id="aa5bc-174">Verfügbarmachen der SKU-Änderung für den Konfigurationsspeicher</span><span class="sxs-lookup"><span data-stu-id="aa5bc-174">Expose sku modification for configuration store.</span></span>
* <span data-ttu-id="aa5bc-175">Befehlsgruppe für die verwaltete Identität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-175">Add command group for managed identity.</span></span>

### <a name="appservice"></a><span data-ttu-id="aa5bc-176">AppService</span><span class="sxs-lookup"><span data-stu-id="aa5bc-176">AppService</span></span>

* <span data-ttu-id="aa5bc-177">Azure Stack: Oberflächenbefehle im Profil „2019-03-01-hybrid“</span><span class="sxs-lookup"><span data-stu-id="aa5bc-177">Azure Stack: surface commands under the profile of 2019-03-01-hybrid</span></span>
* <span data-ttu-id="aa5bc-178">functionapp: Funktion zum Erstellen von Java-Funktions-Apps in Linux hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-178">functionapp: Add ability to create Java function apps in Linux</span></span>

### <a name="arm"></a><span data-ttu-id="aa5bc-179">ARM</span><span class="sxs-lookup"><span data-stu-id="aa5bc-179">ARM</span></span>

* <span data-ttu-id="aa5bc-180">Behebung von Problem Nr. 10246: `az resource tag` stürzt ab, wenn der übergebene Parameter `--ids` der Ressourcengruppen-ID entspricht.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-180">Fix issue #10246: `az resource tag` crashes when the parameter `--ids` passed in is resource group ID</span></span>
* <span data-ttu-id="aa5bc-181">Behebung von Problem Nr. 11658: Der Befehl `az group export` unterstützt die Parameter `--query` und `--output` nicht.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-181">Fix issue #11658: `az group export` command does not support `--query` and `--output` parameters</span></span>
* <span data-ttu-id="aa5bc-182">Behebung von Problem Nr. 10279: Der Exitcode von `az group deployment validate` ist 0, wenn bei der Überprüfung ein Fehler auftritt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-182">Fix issue #10279: The exit code of `az group deployment validate` is 0 when the verification fails</span></span>
* <span data-ttu-id="aa5bc-183">Behebung von Problem Nr. 9916: Fehlermeldung des Konflikts zwischen Tag und anderen Filterbedingungen für Befehl `az resource list` verbessert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-183">Fix issue #9916: Improve the error message of the conflict between tag and other filter conditions for `az resource list` command</span></span>
* <span data-ttu-id="aa5bc-184">Neuer Parameter `--managed-by` hinzugefügt, um das Hinzufügen der Informationen vom Typ „managedBy“ für Befehl `az group create` zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-184">Add new parameter `--managed-by` to support adding managedBy information for command `az group create`</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="aa5bc-185">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="aa5bc-185">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="aa5bc-186">Untergruppe `monitor` hinzugefügt, um Log Analytics-Überwachung im Azure Red Hat OpenShift-Cluster zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-186">Add `monitor` subgroup to manage Log Analytics monitoring in Azure Red Hat OpensShift cluster</span></span>

### <a name="botservice"></a><span data-ttu-id="aa5bc-187">BotService</span><span class="sxs-lookup"><span data-stu-id="aa5bc-187">BotService</span></span>

* <span data-ttu-id="aa5bc-188">Behebung von Problem Nr. 11697: `az bot create` ist nicht idempotent.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-188">Fix issue #11697: `az bot create` is not idempotent</span></span>
* <span data-ttu-id="aa5bc-189">Tests zur Namenskorrektur geändert, sodass sie nur im Livemodus ausgeführt werden</span><span class="sxs-lookup"><span data-stu-id="aa5bc-189">Change name-correcting tests to run in Live-mode only</span></span>

### <a name="cdn"></a><span data-ttu-id="aa5bc-190">CDN</span><span class="sxs-lookup"><span data-stu-id="aa5bc-190">CDN</span></span>

* <span data-ttu-id="aa5bc-191">Unterstützung für das rulesEngine-Feature hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-191">Add support for rulesEngine feature</span></span>
* <span data-ttu-id="aa5bc-192">Neue Befehlsgruppe „cdn endpoint rule“ zum Verwalten von Regeln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-192">Add new commands group 'cdn endpoint rule' to manage rules</span></span>
* <span data-ttu-id="aa5bc-193">azure-mgmt-cdn-Version auf 4.0.0 aktualisiert, um API-Version 2019-04-15 zu verwenden</span><span class="sxs-lookup"><span data-stu-id="aa5bc-193">Update azure-mgmt-cdn version to 4.0.0 to use api version 2019-04-15</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="aa5bc-194">Bereitstellungs-Manager</span><span class="sxs-lookup"><span data-stu-id="aa5bc-194">Deployment Manager</span></span>

* <span data-ttu-id="aa5bc-195">Auflistungsvorgang für alle Ressourcen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-195">Add list operation for all resources.</span></span>
* <span data-ttu-id="aa5bc-196">Schrittressource für neuen Schritttyp optimiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-196">Enhance step resource for new step type.</span></span>
* <span data-ttu-id="aa5bc-197">Paket „azure-mgmt-deploymentmanager“ zur Verwendung von Version 0.2.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-197">Update azure-mgmt-deploymentmanager package to use version 0.2.0.</span></span>

### <a name="iot"></a><span data-ttu-id="aa5bc-198">IoT</span><span class="sxs-lookup"><span data-stu-id="aa5bc-198">IoT</span></span>

* <span data-ttu-id="aa5bc-199">Befehle vom Typ „IoT hub Job“ als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="aa5bc-199">Deprecate 'IoT hub Job' commands.</span></span>

### <a name="iot-central"></a><span data-ttu-id="aa5bc-200">IoT Central</span><span class="sxs-lookup"><span data-stu-id="aa5bc-200">IoT Central</span></span>

* <span data-ttu-id="aa5bc-201">Unterstützung der App-Erstellung/-Aktualisierung mit neuem SKU-Namen ST0, ST1, ST2</span><span class="sxs-lookup"><span data-stu-id="aa5bc-201">Support app creation/update with the new sku name ST0, ST1, ST2.</span></span>

### <a name="key-vault"></a><span data-ttu-id="aa5bc-202">Key Vault</span><span class="sxs-lookup"><span data-stu-id="aa5bc-202">Key Vault</span></span>

* <span data-ttu-id="aa5bc-203">Neuer Befehl `az keyvault key download` zum Herunterladen von Schlüsseln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-203">Add a new command `az keyvault key download` for downloading keys.</span></span>

### <a name="misc"></a><span data-ttu-id="aa5bc-204">Sonstiges</span><span class="sxs-lookup"><span data-stu-id="aa5bc-204">Misc</span></span>

* <span data-ttu-id="aa5bc-205">Behebung Nr. 6371: Unterstützung für die Vervollständigung von Dateinamen und Umgebungsvariablen in Bash</span><span class="sxs-lookup"><span data-stu-id="aa5bc-205">Fix #6371: Support filename and environment variable completion in Bash</span></span>

### <a name="network"></a><span data-ttu-id="aa5bc-206">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="aa5bc-206">Network</span></span>

* <span data-ttu-id="aa5bc-207">Behebung Nr. 2092: az network dns record-set add/remove: Warnung hinzugefügt, wenn Datensatzgruppe nicht gefunden wurde.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-207">Fix #2092: az network dns record-set add/remove: add warning when record-set is not found.</span></span> <span data-ttu-id="aa5bc-208">In Zukunft wird ein zusätzliches Argument unterstützt, um diese automatische Erstellung zu bestätigen.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-208">In the future, an extra argument will be supported to confirm this auto creation.</span></span>

### <a name="policy"></a><span data-ttu-id="aa5bc-209">Richtlinie</span><span class="sxs-lookup"><span data-stu-id="aa5bc-209">Policy</span></span>

* <span data-ttu-id="aa5bc-210">Neuer Befehl `az policy metadata` hinzugefügt, um umfangreiche Richtlinienmetadatenressourcen abzurufen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-210">Add new command `az policy metadata` to retrieve rich policy metadata resources</span></span>
* <span data-ttu-id="aa5bc-211">`az policy remediation create`: Geben Sie mit dem Parameter `--resource-discovery-mode` an, ob die Konformität vor der Wartung neu bewertet werden soll.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-211">`az policy remediation create`: Specify whether compliance should be re-evaluated prior to remediation with the `--resource-discovery-mode` parameter</span></span>

### <a name="profile"></a><span data-ttu-id="aa5bc-212">Profil</span><span class="sxs-lookup"><span data-stu-id="aa5bc-212">Profile</span></span>

* <span data-ttu-id="aa5bc-213">`az account get-access-token`: Parameter `--tenant` hinzugefügt, um das Token für den Mandanten direkt abzurufen. Es muss kein Abonnement angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-213">`az account get-access-token`: Add `--tenant` parameter to acquire token for the tenant directly, needless to specify a subscription</span></span>

### <a name="rbac"></a><span data-ttu-id="aa5bc-214">RBAC</span><span class="sxs-lookup"><span data-stu-id="aa5bc-214">RBAC</span></span>

* <span data-ttu-id="aa5bc-215">[BREAKING CHANGE] Behebung Nr. 11883: `az role assignment create`: Bei leerem Bereich wird ein Fehler ausgegeben.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-215">[BREAKING CHANGE] Fix #11883: `az role assignment create`: empty scope will prompt error</span></span>

### <a name="security"></a><span data-ttu-id="aa5bc-216">Sicherheit</span><span class="sxs-lookup"><span data-stu-id="aa5bc-216">Security</span></span>

* <span data-ttu-id="aa5bc-217">Neue Befehle `az atp show` und `az atp update` hinzugefügt, um erweiterte Einstellungen für den Bedrohungsschutz für Speicherkonten anzuzeigen und zu verwalten</span><span class="sxs-lookup"><span data-stu-id="aa5bc-217">Add new commands `az atp show` and `az atp update` to view and manage advanced threat protection settings for storage accounts.</span></span>

### <a name="sql"></a><span data-ttu-id="aa5bc-218">SQL</span><span class="sxs-lookup"><span data-stu-id="aa5bc-218">SQL</span></span>

* <span data-ttu-id="aa5bc-219">`sql dw create`: Parameter `--zone-redundant` und `--read-replica-count` als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-219">`sql dw create`: deprecate `--zone-redundant` and `--read-replica-count` parameters.</span></span> <span data-ttu-id="aa5bc-220">Diese Parameter gelten nicht für Datawarehouse.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-220">These parameters do not apply to DataWarehouse.</span></span>
* <span data-ttu-id="aa5bc-221">[BREAKING CHANGE] `az sql db create`: „WideWorldImportersStd“ und „WideWorldImportersFull“ als dokumentierte zulässige Werte für „az sql db create --sample-name“ entfernt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-221">[BREAKING CHANGE] `az sql db create`: Remove "WideWorldImportersStd" and "WideWorldImportersFull" as documented allowed values for "az sql db create --sample-name".</span></span> <span data-ttu-id="aa5bc-222">Diese Beispieldatenbanken führen immer zu einem Fehler bei der Erstellung.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-222">These sample databases would always cause creation to fail.</span></span>
* <span data-ttu-id="aa5bc-223">Neue Befehle `sql db classification show/list/update/delete` und `sql db classification recommendation list/enable/disable` zur Verwaltung von Vertraulichkeitsklassifizierungen für SQL-Datenbanken hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-223">Add New commands `sql db classification show/list/update/delete` and `sql db classification recommendation list/enable/disable` to manage sensitivity classifications for SQL databases.</span></span>
* <span data-ttu-id="aa5bc-224">`az sql db audit-policy`: Behebung für leere Überwachungsaktionen und -gruppen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-224">`az sql db audit-policy`: Fix for empty audit actions and groups</span></span>

### <a name="storage"></a><span data-ttu-id="aa5bc-225">Storage</span><span class="sxs-lookup"><span data-stu-id="aa5bc-225">Storage</span></span>

* <span data-ttu-id="aa5bc-226">Neue Befehlsgruppe `az storage share-rm` hinzugefügt, um den Ressourcenanbieter „Microsoft.Storage“ für Verwaltungsvorgänge der Azure-Dateifreigabe zu verwenden</span><span class="sxs-lookup"><span data-stu-id="aa5bc-226">Add a new command group `az storage share-rm` to use the Microsoft.Storage resource provider for Azure file share management operations.</span></span>
* <span data-ttu-id="aa5bc-227">Behebung für Problem Nr. 11415: Berechtigungsfehler für `az storage blob update`</span><span class="sxs-lookup"><span data-stu-id="aa5bc-227">Fix issue #11415: permission error for `az storage blob update`</span></span>
* <span data-ttu-id="aa5bc-228">Integration von Azcopy 10.3.3 und Unterstützung von Win32</span><span class="sxs-lookup"><span data-stu-id="aa5bc-228">Integrate Azcopy 10.3.3 and support Win32.</span></span>
* <span data-ttu-id="aa5bc-229">`az storage copy`: Parameter `--include-path`, `--include-pattern`, `--exclude-path` und`--exclude-pattern` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-229">`az storage copy`: Add `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="aa5bc-230">`az storage remove`: Parameter `--inlcude` und `--exclude` in Parameter `--include-path`, `--include-pattern`, `--exclude-path` und`--exclude-pattern` geändert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-230">`az storage remove`: Change `--inlcude` and `--exclude` parameters to `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="aa5bc-231">`az storage sync`: Parameter `--include-pattern`, `--exclude-path` und`--exclude-pattern` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-231">`az storage sync`: Add `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>

### <a name="servicefabric"></a><span data-ttu-id="aa5bc-232">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="aa5bc-232">ServiceFabric</span></span>

* <span data-ttu-id="aa5bc-233">Neue Befehle zum Verwalten von Anwendung und Diensten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-233">Add new commands to manage appliaction and services.</span></span>

## <a name="january-13-2020"></a><span data-ttu-id="aa5bc-234">13. Januar 2020</span><span class="sxs-lookup"><span data-stu-id="aa5bc-234">January 13, 2020</span></span>

<span data-ttu-id="aa5bc-235">Version 2.0.80</span><span class="sxs-lookup"><span data-stu-id="aa5bc-235">Version 2.0.80</span></span>

### <a name="compute"></a><span data-ttu-id="aa5bc-236">Compute</span><span class="sxs-lookup"><span data-stu-id="aa5bc-236">Compute</span></span>

* <span data-ttu-id="aa5bc-237">Datenträgeraktualisierung: „--disk-encryption-set“ und „--encryption-type“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-237">disk update: Add --disk-encryption-set and --encryption-type</span></span>
* <span data-ttu-id="aa5bc-238">Momentaufnahmeerstellung/-aktualisierung: „--disk-encryption-set“ und „--encryption-type“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-238">snapshot create/update: Add --disk-encryption-set and --encryption-type</span></span>

### <a name="storage"></a><span data-ttu-id="aa5bc-239">Storage</span><span class="sxs-lookup"><span data-stu-id="aa5bc-239">Storage</span></span>

* <span data-ttu-id="aa5bc-240">„azure-mgmt-storage“ auf Version 7.1.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-240">Upgrade azure-mgmt-storage version to 7.1.0</span></span>
* <span data-ttu-id="aa5bc-241">`az storage account create`: `--encryption-key-type-for-table` und `--encryption-key-type-for-queue` zur Unterstützung des Tabellen- und Warteschlangenverschlüsselungsdiensts hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-241">`az storage account create`: Add `--encryption-key-type-for-table` and `--encryption-key-type-for-queue` to support Table and Queue Encryption Service</span></span>

## <a name="january-07-2020"></a><span data-ttu-id="aa5bc-242">7\. Januar 2020</span><span class="sxs-lookup"><span data-stu-id="aa5bc-242">January 07, 2020</span></span>

<span data-ttu-id="aa5bc-243">Version 2.0.79</span><span class="sxs-lookup"><span data-stu-id="aa5bc-243">Version 2.0.79</span></span>

### <a name="acr"></a><span data-ttu-id="aa5bc-244">ACR</span><span class="sxs-lookup"><span data-stu-id="aa5bc-244">ACR</span></span>

* <span data-ttu-id="aa5bc-245">[BREAKING CHANGE] Parameter „--os“ für „acr build“, „acr task create/update“, „acr run“ und „acr pack“ wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-245">[BREAKING CHANGE] Remove '--os' parameter for 'acr build', 'acr task create/update', 'acr run', and 'acr pack'.</span></span> <span data-ttu-id="aa5bc-246">Verwenden Sie stattdessen „--platform“.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-246">Use '--platform' instead.</span></span>

### <a name="appconfig"></a><span data-ttu-id="aa5bc-247">AppConfig</span><span class="sxs-lookup"><span data-stu-id="aa5bc-247">AppConfig</span></span>

* <span data-ttu-id="aa5bc-248">Unterstützung für das Importieren/Exportieren von Featureflags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-248">Add support for importing/exporting feature flags</span></span>
* <span data-ttu-id="aa5bc-249">Neuer Befehl „az appconfig kv set-keyvault“ für das Erstellen einer KeyVault-Referenz hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-249">Add new command 'az appconfig kv set-keyvault' for creating keyvault reference</span></span>
* <span data-ttu-id="aa5bc-250">Unterstützung verschiedener Benennungskonventionen beim Exportieren von Featureflags in eine Datei</span><span class="sxs-lookup"><span data-stu-id="aa5bc-250">Support various naming conventions when exporting feature flags to file</span></span>

### <a name="appservice"></a><span data-ttu-id="aa5bc-251">AppService</span><span class="sxs-lookup"><span data-stu-id="aa5bc-251">AppService</span></span>

* <span data-ttu-id="aa5bc-252">Behebung von Problem Nr. 7154: Aktualisierung der Dokumentation für Befehl „<>“, sodass Backticks anstelle von einfachen Anführungszeichen verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-252">Fix issue #7154: Updating documentation for command <> to use back ticks instead of single quotes</span></span>
* <span data-ttu-id="aa5bc-253">Behebung von Problem Nr. 11287: „webapp up“: Für die mit „up“ erstellte App muss standardmäßig SSL aktiviert sein.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-253">Fix issue #11287: webapp up: By default make the app created using up 'should be 'SSL enabled'</span></span>
* <span data-ttu-id="aa5bc-254">Behebung von Problem Nr. 11592: Flag „az webapp up“ für statische HTML-Websites hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-254">Fix issue #11592: Add az webapp up flag for html static sites</span></span>

### <a name="arm"></a><span data-ttu-id="aa5bc-255">ARM</span><span class="sxs-lookup"><span data-stu-id="aa5bc-255">ARM</span></span>

* <span data-ttu-id="aa5bc-256">Behebung `az resource tag`: Recovery Services-Tresor-Tags können nicht aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-256">Fix `az resource tag`: Recovery Services Vault tags cannot be updated</span></span>

### <a name="backup"></a><span data-ttu-id="aa5bc-257">Backup</span><span class="sxs-lookup"><span data-stu-id="aa5bc-257">Backup</span></span>

* <span data-ttu-id="aa5bc-258">Neuer Befehl „backup protection undelete“ hinzugefügt, um die Funktion zum vorläufigen Löschen für IaasVM-Workloads zu aktivieren</span><span class="sxs-lookup"><span data-stu-id="aa5bc-258">Added new command 'backup protection undelete' to enable soft-delete feature for IaasVM workload</span></span>
* <span data-ttu-id="aa5bc-259">Neuer Parameter „--soft-delete-feature-state“ hinzugefügt, um den Befehl „backup-properties“ festzulegen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-259">Added new parameter '--soft-delete-feature-state' to set backup-properties command</span></span>
* <span data-ttu-id="aa5bc-260">Unterstützung für den Ausschluss von Datenträgern für IaasVM-Workload hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-260">Added disk exclusion support for IaasVM workload</span></span>

### <a name="compute"></a><span data-ttu-id="aa5bc-261">Compute</span><span class="sxs-lookup"><span data-stu-id="aa5bc-261">Compute</span></span>

* <span data-ttu-id="aa5bc-262">Fehler `vm create` in Azure Stack-Profil behoben.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-262">Fix `vm create` failure in Azure Stack profile.</span></span>
* <span data-ttu-id="aa5bc-263">vm monitor metrics tail/list-definitions: Unterstützung einer Abfragemetrik und von Listendefinitionen für eine VM.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-263">vm monitor metrics tail/list-definitions: support query metric and list definitions for a vm.</span></span>
* <span data-ttu-id="aa5bc-264">Neue Aktion des Befehls zum erneuten Anwenden für „az vm“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-264">Add new reapply command action for az vm</span></span>

### <a name="hdinsight"></a><span data-ttu-id="aa5bc-265">HDInsight</span><span class="sxs-lookup"><span data-stu-id="aa5bc-265">HDInsight</span></span>

* <span data-ttu-id="aa5bc-266">Unterstützung für das Erstellen eines Kafka-Clusters mit Kafka-REST-Proxy</span><span class="sxs-lookup"><span data-stu-id="aa5bc-266">Support for creating a Kafka cluster with Kafka Rest Proxy</span></span>
* <span data-ttu-id="aa5bc-267">„azure-mgmt-hdinsight“ auf 1.3.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-267">Upgrade azure-mgmt-hdinsight to 1.3.0</span></span>

### <a name="misc"></a><span data-ttu-id="aa5bc-268">Verschiedenes:</span><span class="sxs-lookup"><span data-stu-id="aa5bc-268">Misc.</span></span>

* <span data-ttu-id="aa5bc-269">Vorschaubefehl `az version show` hinzugefügt, um die Versionen der Azure CLI-Module und Erweiterungen standardmäßig im JSON-Format oder im mit „--output“ konfigurierten Format anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-269">Add preview command `az version show` to show the versions of Azure CLI modules and extensions in JSON format by default or format configured by --output</span></span>

### <a name="event-hubs"></a><span data-ttu-id="aa5bc-270">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="aa5bc-270">Event Hubs</span></span>

* <span data-ttu-id="aa5bc-271">[BREAKING CHANGE] Statusoption „ReceiveDisabled“ aus „az eventhubs eventhub update“ und „az eventhubs eventhub create“ entfernt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-271">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az eventhubs eventhub update' and 'az eventhubs eventhub create'.</span></span> <span data-ttu-id="aa5bc-272">Diese Option ist für Event Hub-Entitäten nicht gültig.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-272">This option is not valid for Event Hub entities.</span></span>

### <a name="service-bus"></a><span data-ttu-id="aa5bc-273">Service Bus</span><span class="sxs-lookup"><span data-stu-id="aa5bc-273">Service Bus</span></span>

* <span data-ttu-id="aa5bc-274">[BREAKING CHANGE] Statusoption „ReceiveDisabled“ aus Befehlen „az servicebus topic create“, „az servicebus topic update“, „az servicebus queue create“ und „az servicebus queue update“ entfernt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-274">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az servicebus topic create', 'az servicebus topic update', 'az servicebus queue create', and 'az servicebus queue update'.</span></span> <span data-ttu-id="aa5bc-275">Diese Option ist für Service Bus-Themen und -Warteschlangen nicht gültig.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-275">This option is not valid for Service Bus topics and queues.</span></span>

### <a name="rbac"></a><span data-ttu-id="aa5bc-276">RBAC</span><span class="sxs-lookup"><span data-stu-id="aa5bc-276">RBAC</span></span>

* <span data-ttu-id="aa5bc-277">Behebung Nr. 11712: `az ad app/sp show` gibt nicht den Exitcode 3 zurück, wenn die Anwendung oder der Dienstprinzipal nicht vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-277">Fix #11712: `az ad app/sp show` does not return exit code 3 when the application or service principal does not exist</span></span>

### <a name="storage"></a><span data-ttu-id="aa5bc-278">Storage</span><span class="sxs-lookup"><span data-stu-id="aa5bc-278">Storage</span></span>

* <span data-ttu-id="aa5bc-279">`az storage account create`: Vorschaukennzeichnung für Parameter „--enable-hierarchical-namespace“ entfernt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-279">`az storage account create`: Remove preview flag for --enable-hierarchical-namespace parameter</span></span>
* <span data-ttu-id="aa5bc-280">azure-mgmt-storage-Version auf 7.0.0 aktualisiert, um API-Version 2019-06-01 zu verwenden</span><span class="sxs-lookup"><span data-stu-id="aa5bc-280">Update azure-mgmt-storage version to 7.0.0 to use api version 2019-06-01</span></span>
* <span data-ttu-id="aa5bc-281">Neue Parameter `--enable-delete-retention` und `--delete-retention-days` hinzugefügt, um die Verwaltung der Aufbewahrungsrichtlinie für Löschen für „blob-service-properties“ von Speicherkonten zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-281">Add new parameters `--enable-delete-retention` and `--delete-retention-days` to support managing delete retention policy for storage account blob-service-properties.</span></span>

## <a name="december-17-2019"></a><span data-ttu-id="aa5bc-282">17. Dezember 2019</span><span class="sxs-lookup"><span data-stu-id="aa5bc-282">December 17, 2019</span></span>

<span data-ttu-id="aa5bc-283">2.0.78</span><span class="sxs-lookup"><span data-stu-id="aa5bc-283">2.0.78</span></span>

### <a name="acr"></a><span data-ttu-id="aa5bc-284">ACR</span><span class="sxs-lookup"><span data-stu-id="aa5bc-284">ACR</span></span>

* <span data-ttu-id="aa5bc-285">Unterstützung für lokalen Kontext in „acr task run“</span><span class="sxs-lookup"><span data-stu-id="aa5bc-285">Added support Local context in acr task run</span></span>

### <a name="acs"></a><span data-ttu-id="aa5bc-286">ACS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-286">ACS</span></span>

* <span data-ttu-id="aa5bc-287">[BREAKING CHANGE] az openshift create: `--workspace-resource-id` in `--workspace-id` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-287">[BREAKING CHANGE]az openshift create: rename `--workspace-resource-id` to `--workspace-id`.</span></span>

### <a name="ams"></a><span data-ttu-id="aa5bc-288">AMS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-288">AMS</span></span>

* <span data-ttu-id="aa5bc-289">Befehle zum Anzeigen aktualisiert, sodass 3 zurückgegeben wird, wenn die Ressource nicht gefunden wurde</span><span class="sxs-lookup"><span data-stu-id="aa5bc-289">Updated show commands to return 3 when resource not found</span></span>

### <a name="appconfig"></a><span data-ttu-id="aa5bc-290">AppConfig</span><span class="sxs-lookup"><span data-stu-id="aa5bc-290">AppConfig</span></span>

* <span data-ttu-id="aa5bc-291">Fehler beim Anhängen der API-Version an die Anforderungs-URL korrigiert.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-291">Fixed bug when appending api-version to request url.</span></span> <span data-ttu-id="aa5bc-292">Die vorhandene Lösung funktioniert nicht mit Paginierung.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-292">The existing solution doesn't work with pagination.</span></span>
* <span data-ttu-id="aa5bc-293">Unterstützung für die Anzeige von weiteren Sprachen neben Englisch hinzugefügt, da der Back-End-Dienst Unicode für die Globalisierung unterstützt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-293">Added support for showing languages besides English as our backend service support unicode for globalization.</span></span>

### <a name="appservice"></a><span data-ttu-id="aa5bc-294">AppService</span><span class="sxs-lookup"><span data-stu-id="aa5bc-294">AppService</span></span>

* <span data-ttu-id="aa5bc-295">Problem Nr. 11217 behoben: Web-App: „az webapp config ssl upload“ muss Slot-Parameter unterstützen.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-295">Fixed issue #11217: webapp: az webapp config ssl upload should support slot parameter</span></span>
* <span data-ttu-id="aa5bc-296">Problem Nr. 10965 behoben: Error: Der Name darf nicht leer sein.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-296">Fixed issue #10965: Error: Name cannot be empty.</span></span> <span data-ttu-id="aa5bc-297">Entfernen anhand von „ip_address“ und „subnet“ zulassen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-297">Allow remove by ip_address and subnet</span></span>
* <span data-ttu-id="aa5bc-298">Unterstützung des Imports von Zertifikaten aus Key Vault hinzugefügt `az webapp config ssl import`</span><span class="sxs-lookup"><span data-stu-id="aa5bc-298">Added support for importing certificates from Key Vault `az webapp config ssl import`</span></span>

### <a name="arm"></a><span data-ttu-id="aa5bc-299">ARM</span><span class="sxs-lookup"><span data-stu-id="aa5bc-299">ARM</span></span>

* <span data-ttu-id="aa5bc-300">Paket „azure-mgmt-resource“ auf die Verwendung von 6.0.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-300">Updated azure-mgmt-resource package to use 6.0.0</span></span>
* <span data-ttu-id="aa5bc-301">Mandantenübergreifende Unterstützung für Befehl `az group deployment create` durch Hinzufügen des neuen Parameters `--aux-subs`</span><span class="sxs-lookup"><span data-stu-id="aa5bc-301">Cross Tenant Support for `az group deployment create` command by adding new parameter `--aux-subs`</span></span>
* <span data-ttu-id="aa5bc-302">Neuer Parameter `--metadata` hinzugefügt, um das Hinzufügen von Metadateninformationen für Richtliniensatzdefinitionen zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-302">Added new parameter `--metadata` to support adding metadata information for policy set definitions.</span></span>

### <a name="backup"></a><span data-ttu-id="aa5bc-303">Backup</span><span class="sxs-lookup"><span data-stu-id="aa5bc-303">Backup</span></span>

* <span data-ttu-id="aa5bc-304">Unterstützung der Sicherung für SQL- und SAP Hana-Workloads hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-304">Added Backup support for SQL and SAP Hana workload.</span></span>

### <a name="botservice"></a><span data-ttu-id="aa5bc-305">BotService</span><span class="sxs-lookup"><span data-stu-id="aa5bc-305">BotService</span></span>

* <span data-ttu-id="aa5bc-306">[Breaking Change] Flag „--version“ aus Vorschaubefehl „az bot create“ entfernt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-306">[Breaking change] Remove '--version' flag from preview command 'az bot create'.</span></span> <span data-ttu-id="aa5bc-307">Nur v4-SDK-Bots werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-307">Only v4 SDK bots are supported.</span></span>
* <span data-ttu-id="aa5bc-308">Überprüfung der Namensverfügbarkeit für „az bot create“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-308">Added name availability check for 'az bot create'.</span></span>
* <span data-ttu-id="aa5bc-309">Unterstützung für das Aktualisieren der Symbol-URL für einen Bot über „az bot update“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-309">Added support for updating the icon URL for a bot via 'az bot update'.</span></span>
* <span data-ttu-id="aa5bc-310">Unterstützung für das Aktualisieren eines Direct Line-Kanals über „az bot directline update“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-310">Added support for updating a Direct Line channel via 'az bot directline update'.</span></span>
* <span data-ttu-id="aa5bc-311">Unterstützung für Flag „--enable-enhanced-auth“ zu „az bot directline create“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-311">Added '--enable-enhanced-auth' flag support to 'az bot directline create'.</span></span>
* <span data-ttu-id="aa5bc-312">Die folgenden Befehlsgruppen sind allgemein verfügbar und befinden sich nicht in der Vorschau: „az bot authsetting“.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-312">The following command groups are GA and not in preview: 'az bot authsetting'.</span></span>
* <span data-ttu-id="aa5bc-313">Die folgenden Befehle in „az bot“ sind allgemein verfügbar und befinden sich nicht in der Vorschau: „create“, „prepare-deploy“, „show“, „delete“, „update“.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-313">The following commands in 'az bot' are GA and not in preview: 'create', 'prepare-deploy', 'show', 'delete', 'update'.</span></span>
* <span data-ttu-id="aa5bc-314">„az bot prepare-deploy“ korrigiert, indem der Wert voon „--proj-file-path“ in Kleinschreibung geändert wurde (z. B. „Test.csproj“ in „test.csproj“).</span><span class="sxs-lookup"><span data-stu-id="aa5bc-314">Fixed 'az bot prepare-deploy' changing '--proj-file-path' value to lower case (e.g. "Test.csproj" to "test.csproj").</span></span>

### <a name="compute"></a><span data-ttu-id="aa5bc-315">Compute</span><span class="sxs-lookup"><span data-stu-id="aa5bc-315">Compute</span></span>

* <span data-ttu-id="aa5bc-316">vmss create/update: „--scale-in-policy“ hinzugefügt, womit entschieden wird, welche virtuellen Computer beim horizontalen Herunterskalieren einer VM-Skalierungsgruppe zum Entfernen ausgewählt werden.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-316">vmss create/update: Added --scale-in-policy, which decides which virtual machines are chosen for removal when a VMSS is scaled-in.</span></span>
* <span data-ttu-id="aa5bc-317">vm/vmss update: „--priority“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-317">vm/vmss update: Added --priority.</span></span>
* <span data-ttu-id="aa5bc-318">vm/vmss update: „--max-price“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-318">vm/vmss update: Added --max-price.</span></span>
* <span data-ttu-id="aa5bc-319">Befehlsgruppe „disk-encryption-set“ hinzugefügt (create, show, update, delete, list).</span><span class="sxs-lookup"><span data-stu-id="aa5bc-319">Added disk-encryption-set command group (create, show, update, delete, list).</span></span>
* <span data-ttu-id="aa5bc-320">disk create: „--encryption-type“ und „--disk-encryption-set“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-320">disk create: Added --encryption-type and --disk-encryption-set.</span></span>
* <span data-ttu-id="aa5bc-321">vm/vmss create: „--os-disk-encryption-set“ und „--data-disk-encryption-sets“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-321">vm/vmss create: Added --os-disk-encryption-set and --data-disk-encryption-sets.</span></span>

### <a name="core"></a><span data-ttu-id="aa5bc-322">Core</span><span class="sxs-lookup"><span data-stu-id="aa5bc-322">Core</span></span>

* <span data-ttu-id="aa5bc-323">Unterstützung für Python 3.4 entfernt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-323">Removed support for Python 3.4</span></span>
* <span data-ttu-id="aa5bc-324">Plug-In für HaTS-Umfrage in mehreren Befehlen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-324">Plug in HaTS survey in multiple commands</span></span>

### <a name="dls"></a><span data-ttu-id="aa5bc-325">DLS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-325">DLS</span></span>

* <span data-ttu-id="aa5bc-326">ADLS-SDK-Version aktualisiert (0.0.48).</span><span class="sxs-lookup"><span data-stu-id="aa5bc-326">Updated ADLS sdk version (0.0.48).</span></span>

### <a name="install"></a><span data-ttu-id="aa5bc-327">Installieren</span><span class="sxs-lookup"><span data-stu-id="aa5bc-327">Install</span></span>

* <span data-ttu-id="aa5bc-328">Installationsskript unterstützt Python 3.8</span><span class="sxs-lookup"><span data-stu-id="aa5bc-328">Install script support python 3.8</span></span>

### <a name="iot"></a><span data-ttu-id="aa5bc-329">IoT</span><span class="sxs-lookup"><span data-stu-id="aa5bc-329">IOT</span></span>

* <span data-ttu-id="aa5bc-330">[BREAKING CHANGE] Parameter „--failover-region“ aus „manual-failover“ entfernt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-330">[BREAKING CHANGE] Removed --failover-region parameter from manual-failover.</span></span> <span data-ttu-id="aa5bc-331">Das Failover erfolgt jetzt in eine zugewiesene, geografisch gekoppelte sekundäre Region.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-331">Now it will failover to assigned geo-paired secondary region.</span></span>

### <a name="key-vault"></a><span data-ttu-id="aa5bc-332">Key Vault</span><span class="sxs-lookup"><span data-stu-id="aa5bc-332">Key Vault</span></span>

* <span data-ttu-id="aa5bc-333">Nr. 8095 behoben: `az keyvault storage remove`: Hilfemeldung verbessert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-333">Fixed #8095: `az keyvault storage remove`: improve the help message</span></span>
* <span data-ttu-id="aa5bc-334">Nr. 8921 behoben: `az keyvault key/secret/certificate list/list-deleted/list-versions`: Validierungsfehler in Parameter `--maxresults` behoben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-334">Fixed #8921: `az keyvault key/secret/certificate list/list-deleted/list-versions`: fix the validation bug on parameter `--maxresults`</span></span>
* <span data-ttu-id="aa5bc-335">Nr. 10512 behoben: `az keyvault set-policy`: Fehlermeldung verbessert, wenn weder `--object-id`, `--spn` noch `--upn` angegeben ist</span><span class="sxs-lookup"><span data-stu-id="aa5bc-335">Fixed #10512: `az keyvault set-policy`: improve the error message when none of `--object-id`, `--spn` or `--upn` is specified</span></span>
* <span data-ttu-id="aa5bc-336">Nr. 10846 behoben: `az keyvault secret show-deleted`: Wenn `--id` angegeben ist, ist `--name/-n` nicht erforderlich.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-336">Fixed #10846: `az keyvault secret show-deleted`: when `--id` is specified, `--name/-n` is not required</span></span>
* <span data-ttu-id="aa5bc-337">Nr. 11084 behoben: `az keyvault secret download`: Hilfemeldung von Parameter `--encoding` verbessert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-337">Fixed #11084: `az keyvault secret download`: improve the help message of parameter `--encoding`</span></span>

### <a name="network"></a><span data-ttu-id="aa5bc-338">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="aa5bc-338">Network</span></span>

* <span data-ttu-id="aa5bc-339">az network application-gateway probe: Unterstützung für Option „--port“ hinzugefügt, um einen Port zum Prüfen von Back-End-Servern beim Erstellen und Aktualisieren anzugeben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-339">az network application-gateway probe: Added support --port option to specify a port for probing backend servers when create and update</span></span>
* <span data-ttu-id="aa5bc-340">az network application-gateway url-path-map create/update: Fehlerbehebung für `--waf-policy`</span><span class="sxs-lookup"><span data-stu-id="aa5bc-340">az network application-gateway url-path-map create/update: bug fix for `--waf-policy`</span></span>
* <span data-ttu-id="aa5bc-341">az network application-gateway: Unterstützung für `--rewrite-rule-set` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-341">az network application-gateway: Added support `--rewrite-rule-set`</span></span>
* <span data-ttu-id="aa5bc-342">az network list-service-aliases: Unterstützung für Listendienstaliase hinzugefügt, die für Dienstendpunktrichtlinien verwendet werden können</span><span class="sxs-lookup"><span data-stu-id="aa5bc-342">az network list-service-aliases: Added support list service aliases which can be used for Service Endpoint Policies</span></span>
* <span data-ttu-id="aa5bc-343">az network dns zone import: Unterstützung für „.@“ in Datensatzname hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-343">az network dns zone import: Added support .@ in record name</span></span>

### <a name="packaging"></a><span data-ttu-id="aa5bc-344">Verpackung</span><span class="sxs-lookup"><span data-stu-id="aa5bc-344">Packaging</span></span>

* <span data-ttu-id="aa5bc-345">Back-Edge-Builds für PIP-Installation hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-345">Added back edge builds for pip install</span></span>
* <span data-ttu-id="aa5bc-346">Ubuntu-Eoan-Paket hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-346">Added Ubuntu eoan package</span></span>

### <a name="policy"></a><span data-ttu-id="aa5bc-347">Richtlinie</span><span class="sxs-lookup"><span data-stu-id="aa5bc-347">Policy</span></span>

* <span data-ttu-id="aa5bc-348">Unterstützung für Version 2019-09-01 der Richtlinien-API hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-348">Added support for Policy API version 2019-09-01.</span></span>
* <span data-ttu-id="aa5bc-349">az policy set-definition: Unterstützung der Gruppierung innerhalb von Richtliniensatzdefinitionen mit `--definition-groups`-Parameter hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-349">az policy set-definition: Added support grouping within policy set definitions with `--definition-groups` parameter</span></span>

### <a name="redis"></a><span data-ttu-id="aa5bc-350">Redis</span><span class="sxs-lookup"><span data-stu-id="aa5bc-350">Redis</span></span>

* <span data-ttu-id="aa5bc-351">Vorschauparameter `--replicas-per-master` zu Befehl `az redis create`hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-351">Added preview param `--replicas-per-master` to `az redis create` command</span></span>
* <span data-ttu-id="aa5bc-352">„azure-mgmt-redis“ von 6.0.0 auf 7.0.0rc1 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-352">Updated azure-mgmt-redis from 6.0.0 to 7.0.0rc1</span></span>

### <a name="servicefabric"></a><span data-ttu-id="aa5bc-353">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="aa5bc-353">ServiceFabric</span></span>

* <span data-ttu-id="aa5bc-354">Hinzufügen von Logik in Knotentyp korrigiert, einschließlich Nr. 10963: Beim Hinzufügen eines neuen Knotentyps mit Dauerhaftigkeitsstufe „Gold“ wird immer ein CLI-Fehler ausgegeben.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-354">Fixed in node-type add logic including #10963: Adding new node type with durability level Gold will always throw CLI error</span></span>
* <span data-ttu-id="aa5bc-355">ServiceFabricNodeVmExt-Version in Erstellungsvorlage auf 1.1 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-355">Updated ServiceFabricNodeVmExt version to 1.1 in creation template</span></span>

### <a name="sql"></a><span data-ttu-id="aa5bc-356">SQL</span><span class="sxs-lookup"><span data-stu-id="aa5bc-356">SQL</span></span>

* <span data-ttu-id="aa5bc-357">Parameter „--read-scale“ und „--read-replicas“ zu Befehlen „sql db create“ und „sql db update“ hinzugefügt, um Leseskalierungsverwaltung zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-357">Added "--read-scale" and "--read-replicas" parameters to sql db create and update commands, to support read scale management.</span></span>

### <a name="storage"></a><span data-ttu-id="aa5bc-358">Storage</span><span class="sxs-lookup"><span data-stu-id="aa5bc-358">Storage</span></span>

* <span data-ttu-id="aa5bc-359">Allgemein verfügbares Release – Eigenschaft „Large File Shares“ für Befehle „storage account create“ und „storage account update“</span><span class="sxs-lookup"><span data-stu-id="aa5bc-359">GA Release Large File Shares property for storage account create and update command</span></span>
* <span data-ttu-id="aa5bc-360">Allgemein verfügbares Release – Unterstützung von SAS-Token für die Benutzerdelegierung</span><span class="sxs-lookup"><span data-stu-id="aa5bc-360">GA Release User Delegation SAS token Support</span></span>
* <span data-ttu-id="aa5bc-361">Neue Befehle `az storage account blob-service-properties show` und `az storage account blob-service-properties update --enable-change-feed` hinzugefügt, um Blob-Diensteigenschaften für das Speicherkonto zu verwalten.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-361">Added new commands `az storage account blob-service-properties show` and `az storage account blob-service-properties update --enable-change-feed` to manage blob service properties for storage account.</span></span>
* <span data-ttu-id="aa5bc-362">[BEVORSTEHENDER BREAKING CHANGE] `az storage copy`: Das Zeichen `*` wird nicht mehr als Platzhalter in der URL, es werden jedoch die neuen Parameter „--include-pattern“ und „--exclude-pattern“ mit Unterstützung des Platzhalters `*` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-362">[COMING BREAKING CHANGE] `az storage copy`: `*` character is no longer supported as a wildcard in URL, but new parameters --include-pattern and --exclude-pattern will be added with `*` wildcard support.</span></span>
* <span data-ttu-id="aa5bc-363">Problem Nr. 11043 behoben: Unterstützung für das Entfernen des gesamten Containers/der gesamten Freigabe in `az storage remove` Befehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-363">Fixed issue #11043: Added support to remove whole container/share in `az storage remove` command</span></span>

## <a name="november-26-2019"></a><span data-ttu-id="aa5bc-364">26. November 2019</span><span class="sxs-lookup"><span data-stu-id="aa5bc-364">November 26, 2019</span></span>

<span data-ttu-id="aa5bc-365">Version 2.0.77</span><span class="sxs-lookup"><span data-stu-id="aa5bc-365">Version 2.0.77</span></span>

### <a name="acr"></a><span data-ttu-id="aa5bc-366">ACR</span><span class="sxs-lookup"><span data-stu-id="aa5bc-366">ACR</span></span>

* <span data-ttu-id="aa5bc-367">Parameter `--branch` in „acr task create/update“ als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-367">Deprecated parameter `--branch` from acr task create/update</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="aa5bc-368">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="aa5bc-368">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="aa5bc-369">`--workspace-resource-id`-Flag hinzugefügt, um die Erstellung eines Azure Red Hat OpenShift-Clusters mit Überwachung zuzulassen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-369">Added `--workspace-resource-id` flag to allow creation of Azure Red Hat Openshift cluster with monitoring</span></span>
* <span data-ttu-id="aa5bc-370">`monitor_profile`-Flag hinzugefügt, um einen Azure Red Hat OpenShift-Clusters mit Überwachung zu erstellen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-370">Added `monitor_profile` to create Azure Red Hat OpenShift cluster with monitoring</span></span>

### <a name="aks"></a><span data-ttu-id="aa5bc-371">AKS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-371">AKS</span></span>

* <span data-ttu-id="aa5bc-372">Unterstützung des Rotationsvorgangs für Clusterzertifikate mithilfe von für Cluster Zertifikat Rotation mit „az aks rotate-certs“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-372">Added support cluster certificate rotation operation using "az aks rotate-certs".</span></span>

### <a name="appconfig"></a><span data-ttu-id="aa5bc-373">AppConfig</span><span class="sxs-lookup"><span data-stu-id="aa5bc-373">AppConfig</span></span>

* <span data-ttu-id="aa5bc-374">Unterstützung für die Verwendung von „:“ für `as az appconfig kv import`-Trennzeichen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-374">Added support for using ":" for `as az appconfig kv import` separator</span></span>
* <span data-ttu-id="aa5bc-375">Problem beim Auflisten von Schlüsselwerten mit mehreren Bezeichnungen, einschließlich NULL-Bezeichnung, behoben.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-375">Fixed issue for listing key values with multiple labels including null label.</span></span> 
* <span data-ttu-id="aa5bc-376">Verwaltungsebenen-SDK, „azure-mgmt-appconfiguration“, auf Version 0.3.0 aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-376">Updated management plane sdk, azure-mgmt-appconfiguration, to version 0.3.0.</span></span> 

### <a name="appservice"></a><span data-ttu-id="aa5bc-377">AppService</span><span class="sxs-lookup"><span data-stu-id="aa5bc-377">AppService</span></span>

* <span data-ttu-id="aa5bc-378">Problem Nr. 11100 behoben AttributeError für „az webapp up“ beim Erstellen eines Dienstplans</span><span class="sxs-lookup"><span data-stu-id="aa5bc-378">Fixed issue #11100: AttributeError for az webapp up when create service plan</span></span>
* <span data-ttu-id="aa5bc-379">az webapp up: Erzwingen der Erstellung oder Bereitstellung auf einer Website für unterstützte Sprachen, es werden keine Standardeinstellungen verwendet.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-379">az webapp up: Forcing the creation or deployment to a site for supported languages, no defaults used.</span></span>
* <span data-ttu-id="aa5bc-380">Unterstützung für App Service-Umgebung hinzugefügt: az appservice ase show | list | list-addresses | list-plans | create | update | delete</span><span class="sxs-lookup"><span data-stu-id="aa5bc-380">Added support for App Service Environment: az appservice ase show | list | list-addresses | list-plans | create | update | delete</span></span>

### <a name="backup"></a><span data-ttu-id="aa5bc-381">Backup</span><span class="sxs-lookup"><span data-stu-id="aa5bc-381">Backup</span></span>

* <span data-ttu-id="aa5bc-382">Problem in Az-Sicherungsrichtlinie „list-associated-items“ behoben.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-382">Fixed issue in az backup policy list-associated-items.</span></span> <span data-ttu-id="aa5bc-383">Optionaler Parameter „BackupManagementType“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-383">Added optional BackupManagementType parameter.</span></span>

### <a name="compute"></a><span data-ttu-id="aa5bc-384">Compute</span><span class="sxs-lookup"><span data-stu-id="aa5bc-384">Compute</span></span>

* <span data-ttu-id="aa5bc-385">API-Version von Compute, Datenträger, Momentaufnahmen auf 2019-07-01 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-385">Upgraded API version of compute, disks, snapshots to 2019-07-01</span></span>
* <span data-ttu-id="aa5bc-386">vmss create: Verbesserung für – Orchestrierungsmodus</span><span class="sxs-lookup"><span data-stu-id="aa5bc-386">vmss create: Improvement for --orchestration-mode</span></span>
* <span data-ttu-id="aa5bc-387">sig image-definition create: „--os-state“ hinzugefügt, um die Angabe zu ermöglichen, ob die unter diesem Image erstellten virtuellen Computer „generalisiert“ oder „spezialisiert“ sind</span><span class="sxs-lookup"><span data-stu-id="aa5bc-387">sig image-definition create: Added --os-state to allow specifying whether the virtual machines created under this image are 'Generalized' or 'Specialized'</span></span>
* <span data-ttu-id="aa5bc-388">sig image-definition create: „--hyper-v-generation“ hinzugefügt, um die Angabe der Hypervisorgeneration zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-388">sig image-definition create: Added --hyper-v-generation to allow specifying the hypervisor generation</span></span>
* <span data-ttu-id="aa5bc-389">sig image-version create: Unterstützung für „--os-snapshot“ und „--data-snapshots“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-389">sig image-version create: Added support --os-snapshot and --data-snapshots</span></span>
* <span data-ttu-id="aa5bc-390">image create: „--data-disk-caching“ hinzugefügt, um die Angabe der Zwischenspeicherungseinstellung von Datenträger zu ermöflichen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-390">image create: Added --data-disk-caching to allow specifying caching setting of data disks</span></span>
* <span data-ttu-id="aa5bc-391">Upgrade des Python-Compute-SDK auf 10.0.0</span><span class="sxs-lookup"><span data-stu-id="aa5bc-391">Upgraded Python Compute SDK to 10.0.0</span></span>
* <span data-ttu-id="aa5bc-392">vm/vmss create: „Spot“ zu Aufzählungseigenschaft „Priority“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-392">vm/vmss create: Added 'Spot' to 'Priority' enum property</span></span>
* <span data-ttu-id="aa5bc-393">[Breaking Change] Parameter „--max-billing“ für sowohl VM als auch VMSS in „--max-price“ umbenannt, um die Konsistenz mit Swagger- und PowerShell-Cmdlets sicherzustellen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-393">[Breaking change] Renamed '--max-billing' parameter to '--max-price', for both VM and VMSS, to be consistent with Swagger and Powershell cmdlets</span></span>
* <span data-ttu-id="aa5bc-394">vm monitor log show: Unterstützung für das Abfragen von Protokollen über verknüpften Protokollanalyse-Arbeitsbereich hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-394">vm monitor log show: Added support for querying log over linked log analytics workspace.</span></span>

### <a name="iot"></a><span data-ttu-id="aa5bc-395">IoT</span><span class="sxs-lookup"><span data-stu-id="aa5bc-395">IOT</span></span>

* <span data-ttu-id="aa5bc-396">Behebung Nr. 2531: Argumente für Benutzerfreundlichkeit für Hub-Update hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-396">Fix #2531: Added convenience arguments for hub update.</span></span>
* <span data-ttu-id="aa5bc-397">Behebung Nr. 8323: Fehlende Parameter zum Erstellen eines benutzerdefinierten Speicherendpunkts hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-397">Fix #8323: Added missing parameters to create storage custom endpoint.</span></span>
* <span data-ttu-id="aa5bc-398">Regressionsfehler behoben: Die Änderungen wurden rückgängig gemacht, sodass der standardmäßige Speicherendpunkt überschrieben wurde.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-398">Fix regression bug: Reverted the changes which overrides the default storage endpoint.</span></span>

### <a name="key-vault"></a><span data-ttu-id="aa5bc-399">Key Vault</span><span class="sxs-lookup"><span data-stu-id="aa5bc-399">Key Vault</span></span>

* <span data-ttu-id="aa5bc-400">Nr. 11121 behoben: Bei der Verwendung von `az keyvault certificate list` erfordert die Übergabe von `--include-pending` jetzt nicht mehr den Wert `true` oder `false`.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-400">Fixed #11121: When using `az keyvault certificate list`, passing `--include-pending` now doesn't require a value of `true` or `false`</span></span>

### <a name="netappfiles"></a><span data-ttu-id="aa5bc-401">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="aa5bc-401">NetAppFiles</span></span>

* <span data-ttu-id="aa5bc-402">Upgrade von „azure-mgmt-netapp“ auf Version 0.7.0, die einige zusätzliche Volumeeigenschaften enthält, die bevorstehenden Replikationsvorgängen zugeordnet sind</span><span class="sxs-lookup"><span data-stu-id="aa5bc-402">Upgraded azure-mgmt-netapp to 0.7.0 which includes some additional volume properties associated with upcoming replication operations</span></span>

### <a name="network"></a><span data-ttu-id="aa5bc-403">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="aa5bc-403">Network</span></span>

* <span data-ttu-id="aa5bc-404">application-gateway waf-config: veraltet</span><span class="sxs-lookup"><span data-stu-id="aa5bc-404">application-gateway waf-config: deprecated</span></span>
* <span data-ttu-id="aa5bc-405">application-gateway waf-policy: Untergruppe „managed-rules“ zur Verwaltung von verwalteten Regelsätzen und Ausschlussregeln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-405">application-gateway waf-policy: Added subgroup managed-rules to manage managed rule sets and exclusion rules</span></span>
* <span data-ttu-id="aa5bc-406">application-gateway waf-policy: Untergruppe „policy-setting“ zur Verwaltung der globalen Konfiguration von „waf-policy“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-406">application-gateway waf-policy: Added subgroup policy-setting to manage global configuration of a waf-policy</span></span>
* <span data-ttu-id="aa5bc-407">[BREAKING CHANGE] application-gateway waf-policy: Untergruppenregel in „custom-rule“ umbenannt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-407">[BREAKING CHANGE] application-gateway waf-policy: Renamed subgroup rule to custom-rule</span></span>
* <span data-ttu-id="aa5bc-408">application-gateway http-listener: „--firewall-policy“ beim Erstellen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-408">application-gateway http-listener: Added --firewall-policy when create</span></span>
* <span data-ttu-id="aa5bc-409">application-gateway url-path-map rule: „--firewall-policy“ beim Erstellen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-409">application-gateway url-path-map rule: Added --firewall-policy when create</span></span>

### <a name="packaging"></a><span data-ttu-id="aa5bc-410">Verpackung</span><span class="sxs-lookup"><span data-stu-id="aa5bc-410">Packaging</span></span>

* <span data-ttu-id="aa5bc-411">Az-Wrapper in Python neu geschrieben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-411">Rewrote the az wrapper in Python</span></span>
* <span data-ttu-id="aa5bc-412">Unterstützung für Python 3.8 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-412">Added support for Python 3.8</span></span>
* <span data-ttu-id="aa5bc-413">Für RPM-Paket in Python 3 geändert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-413">Changed to Python 3 for RPM package</span></span>

### <a name="profile"></a><span data-ttu-id="aa5bc-414">Profil</span><span class="sxs-lookup"><span data-stu-id="aa5bc-414">Profile</span></span>

* <span data-ttu-id="aa5bc-415">Fehler beim Ausführen von `az login -u {} -p {}` mit Microsoft-Konto entfernt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-415">Polished error when running `az login -u {} -p {}` with Microsoft account</span></span>
* <span data-ttu-id="aa5bc-416">`SSLError` beim Ausführen von `az login` hinter einem Proxy mit einem selbstsignierten Stammzertifikat entfernt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-416">Polished `SSLError` when running `az login` behind a proxy with self-signed root certificate</span></span>
* <span data-ttu-id="aa5bc-417">Nr. 10578 behoben: `az login` hängt, wenn mehrere Instanzen gleichzeitig unter Windows oder WSL gestartet werden.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-417">Fixed #10578: `az login` hangs when more than one instances are launched at the same time on Windows or WSL</span></span>
* <span data-ttu-id="aa5bc-418">Nr. 11059 behoben: `az login --allow-no-subscriptions` schlägt fehl, wenn Abonnements im Mandanten vorhanden sind.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-418">Fixed #11059: `az login --allow-no-subscriptions` fails if there are subscriptions in the tenant</span></span>
* <span data-ttu-id="aa5bc-419">Nr. 11238 behoben: Nach dem Umbenennen eines Abonnements führt die Anmeldung mit MSI dazu, dass das gleiche Abonnement zweimal angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-419">Fixed #11238: After renaming a subscription, logging in with MSI will result in the same subscription appearing twice</span></span>

### <a name="rbac"></a><span data-ttu-id="aa5bc-420">RBAC</span><span class="sxs-lookup"><span data-stu-id="aa5bc-420">RBAC</span></span>

* <span data-ttu-id="aa5bc-421">Nr. 10996 behoben: Fehler für `--force-change-password-next-login` in `az ad user update` entfernt, wenn `--password` nicht angegeben ist</span><span class="sxs-lookup"><span data-stu-id="aa5bc-421">Fixed #10996: Polish error for `--force-change-password-next-login` in `az ad user update` when `--password` is not specified</span></span>

### <a name="redis"></a><span data-ttu-id="aa5bc-422">Redis</span><span class="sxs-lookup"><span data-stu-id="aa5bc-422">Redis</span></span>

* <span data-ttu-id="aa5bc-423">Nr. 2902 behoben: Festlegen von Speicherkonfigurationen beim Aktualisieren des Basic-SKU-Cache vermeiden</span><span class="sxs-lookup"><span data-stu-id="aa5bc-423">Fixed #2902: Avoid setting memory configs while updating Basic SKU cache</span></span>

### <a name="reservations"></a><span data-ttu-id="aa5bc-424">Reservations</span><span class="sxs-lookup"><span data-stu-id="aa5bc-424">Reservations</span></span>

* <span data-ttu-id="aa5bc-425">SDK-Version auf 0.6.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-425">Upgraded SDK Version to 0.6.0</span></span>
* <span data-ttu-id="aa5bc-426">Abrechnungsplandetails nach dem Aufrufen von „Get-Gatalogs“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-426">Added billingplan details info after calling Get-Gatalogs</span></span>
* <span data-ttu-id="aa5bc-427">Neuer Befehl `az reservations reservation-order calculate` zum Berechnen des Preises für eine Reservierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-427">Added new command `az reservations reservation-order calculate` to calculate the price for a reservation</span></span>
* <span data-ttu-id="aa5bc-428">Neuer Befehl `az reservations reservation-order purchase` zum Erwerb einer neuen Reservierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-428">Added new command `az reservations reservation-order purchase` to purchase a new reservation</span></span>

### <a name="rest"></a><span data-ttu-id="aa5bc-429">REST</span><span class="sxs-lookup"><span data-stu-id="aa5bc-429">Rest</span></span>
* <span data-ttu-id="aa5bc-430">`az rest` in allgemeine Verfügbarkeit geändert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-430">Changed `az rest` to GA</span></span>

### <a name="sql"></a><span data-ttu-id="aa5bc-431">SQL</span><span class="sxs-lookup"><span data-stu-id="aa5bc-431">SQL</span></span>

* <span data-ttu-id="aa5bc-432">„azure-mgmt-sql“ auf Version 0.15.0 aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-432">Updated azure-mgmt-sql to version 0.15.0.</span></span>

### <a name="storage"></a><span data-ttu-id="aa5bc-433">Storage</span><span class="sxs-lookup"><span data-stu-id="aa5bc-433">Storage</span></span>

* <span data-ttu-id="aa5bc-434">storage account create: „--enable-hierarchical-namespace“ hinzugefügt, um Dateisystemsemantik in Blobdienst zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-434">storage account create: Added --enable-hierarchical-namespace to support filesystem semantics in blob service.</span></span>
* <span data-ttu-id="aa5bc-435">Ausnahme ohne Zusammenhang aus Fehlermeldung entfernt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-435">Removed unrelated exception from error message</span></span>
* <span data-ttu-id="aa5bc-436">Probleme mit falscher Fehlermeldung „Sie verfügen nicht über die erforderlichen Berechtigungen zum Ausführen dieses Vorgangs“ behoben.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-436">Fixed issues with incorrect error message "You do not have the required permissions needed to perform this operation."</span></span> <span data-ttu-id="aa5bc-437">bei Blockierung durch Netzwerkregeln oder bei „AuthenticationFailed“.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-437">when blocked by network rules or AuthenticationFailed.</span></span>

## <a name="november-4-2019"></a><span data-ttu-id="aa5bc-438">4\. November 2019</span><span class="sxs-lookup"><span data-stu-id="aa5bc-438">November 4, 2019</span></span>

<span data-ttu-id="aa5bc-439">Version 2.0.76</span><span class="sxs-lookup"><span data-stu-id="aa5bc-439">Version 2.0.76</span></span>

### <a name="acr"></a><span data-ttu-id="aa5bc-440">ACR</span><span class="sxs-lookup"><span data-stu-id="aa5bc-440">ACR</span></span>

* <span data-ttu-id="aa5bc-441">Vorschauparameter `--pack-image-tag` wurde dem Befehl `az acr pack build` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-441">Added a preview parameter `--pack-image-tag` to command `az acr pack build`.</span></span>
* <span data-ttu-id="aa5bc-442">Unterstützung der Aktivierung der Überwachung beim Erstellen einer Registrierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-442">Added support for enabling auditing on creating a registry</span></span>
* <span data-ttu-id="aa5bc-443">Unterstützung von RBAC mit Repositoryumfang hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-443">Added support for Repository-scoped RBAC</span></span>

### <a name="aks"></a><span data-ttu-id="aa5bc-444">AKS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-444">AKS</span></span>

* <span data-ttu-id="aa5bc-445">`--enable-cluster-autoscaler`, `--min-count` und `--max-count` wurden dem Befehl `az aks create` hinzugefügt, sodass die automatische Clusterskalierung für den Knotenpool aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-445">Added `--enable-cluster-autoscaler`, `--min-count` and `--max-count` to the `az aks create` command, which enables cluster autoscaler for the node pool.</span></span>
* <span data-ttu-id="aa5bc-446">Die obigen Flags sowie `--update-cluster-autoscaler` und `--disable-cluster-autoscaler` wurden dem Befehl `az aks update` hinzugefügt, sodass Updates der automatischen Clusterskalierung zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-446">Added the above flags as well as `--update-cluster-autoscaler` and `--disable-cluster-autoscaler` to the `az aks update` command, allowing updates to cluster autoscaler.</span></span>

### <a name="appconfig"></a><span data-ttu-id="aa5bc-447">AppConfig</span><span class="sxs-lookup"><span data-stu-id="aa5bc-447">AppConfig</span></span>

* <span data-ttu-id="aa5bc-448">Befehlsgruppe der AppConfig-Funktion zum Verwalten von in einer App Configuration-Instanz gespeicherten Featureflags wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-448">Added appconfig feature command group to manage feature flags stored in an App Configuration.</span></span>
* <span data-ttu-id="aa5bc-449">Geringfügiger Programmfehler für Befehl „appconfig kv export to file“ wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-449">Fixed minor bug for appconfig kv export to file command.</span></span> <span data-ttu-id="aa5bc-450">Das Lesen der Zieldateiinhalte wird während des Exports angehalten.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-450">Stop reading dest file contents during export.</span></span>

### <a name="appservice"></a><span data-ttu-id="aa5bc-451">AppService</span><span class="sxs-lookup"><span data-stu-id="aa5bc-451">AppService</span></span>

* <span data-ttu-id="aa5bc-452">`az appservice plan create`: Unterstützung für das Festlegen von „persitescalung“ beim Erstellen eines App-Serviceplans wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-452">`az appservice plan create`: Added support to set 'persitescaling' on appservice plan create.</span></span>
* <span data-ttu-id="aa5bc-453">Ein Problem wurde behoben, aufgrund dessen der Vorgang „webapp config ssl bind“ vorhandene Tags aus der Ressource entfernt hat.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-453">Fixed an issue where webapp config ssl bind operation was removing existing tags from the resource</span></span>
* <span data-ttu-id="aa5bc-454">Flag `--build-remote` wurde für `az functionapp deployment source config-zip` hinzugefügt, um die Remotebuildaktion während der Funktions-App-Bereitstellung zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-454">Added `--build-remote` flag for `az functionapp deployment source config-zip` to support remote build action during function app deployment.</span></span>
* <span data-ttu-id="aa5bc-455">Die Standardknotenversion in Funktions-Apps wurde für Windows in ~ 10 geändert.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-455">Changed default node version on function apps to ~10 for Windows</span></span>
* <span data-ttu-id="aa5bc-456">`--runtime-version`-Eigenschaft zu `az functionapp create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-456">Added `--runtime-version` property to `az functionapp create`</span></span>

### <a name="arm"></a><span data-ttu-id="aa5bc-457">ARM</span><span class="sxs-lookup"><span data-stu-id="aa5bc-457">ARM</span></span>

* <span data-ttu-id="aa5bc-458">`az deployment/group deployment validate`: Parameter `--handle-extended-json-format` wurde hinzugefügt, um bei der Bereitstellung mehrere Zeilen und Kommentare in der JSON-Vorlage zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-458">`az deployment/group deployment validate`: Added `--handle-extended-json-format` parameter to support multiline and comments in json template when deployment.</span></span>
* <span data-ttu-id="aa5bc-459">„azure-mgmt-resource“ auf „2019-07-01“ festgelegt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-459">Bumped azure-mgmt-resource to 2019-07-01</span></span>

### <a name="backup"></a><span data-ttu-id="aa5bc-460">Backup</span><span class="sxs-lookup"><span data-stu-id="aa5bc-460">Backup</span></span>

* <span data-ttu-id="aa5bc-461">Unterstützung für AzureFiles-Sicherung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-461">Added AzureFiles backup support</span></span>

### <a name="compute"></a><span data-ttu-id="aa5bc-462">Compute</span><span class="sxs-lookup"><span data-stu-id="aa5bc-462">Compute</span></span>

* <span data-ttu-id="aa5bc-463">`az vm create`: Beim gleichzeitigen Festlegen von beschleunigtem Netzwerkbetrieb und einer vorhandenen NIC wurde eine Warnung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-463">`az vm create`: Added warning when specifying accelerated networking and an existing NIC together.</span></span>
* <span data-ttu-id="aa5bc-464">`az vm create`: `--vmss` hinzugefügt, um eine vorhandene VM-Skalierungsgruppe anzugeben, welcher der virtuelle Computer zugewiesen werden soll.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-464">`az vm create`: Added `--vmss` to specify an existing virtual machine scale set that the virtual machine should be assigned to.</span></span>
* <span data-ttu-id="aa5bc-465">`az vm/vmss create`: Eine lokale Kopie der Imagealiasdatei wurde hinzugefügt, sodass in einer eingeschränkten Netzwerkumgebung darauf zugegriffen werden kann.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-465">`az vm/vmss create`: Added a local copy of image alias file so that it can be accessed in a restricted network environment.</span></span>
* <span data-ttu-id="aa5bc-466">`az vmss create`: `--orchestration-mode` hinzugefügt, um anzugeben, wie virtuelle Computer von der Skalierungsgruppe verwaltet werden.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-466">`az vmss create`: Added `--orchestration-mode` to specify how virtual machines are managed by the scale set.</span></span>
* <span data-ttu-id="aa5bc-467">`az vm/vmss update`: `--ultra-ssd-enabled` hinzugefügt, um das Aktualisieren der SSD-Einstellung zuzulassen.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-467">`az vm/vmss update`: Added `--ultra-ssd-enabled` to allow updating ultra SSD setting.</span></span>
* <span data-ttu-id="aa5bc-468">[BREAKING CHANGE] `az vm extension set`: Ein Fehler wurde behoben, aufgrund dessen Benutzer mit `--ids` keine Erweiterung auf einem virtuellen Computer festlegen konnten.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-468">[BREAKING CHANGE] `az vm extension set`: Fixed bug where users could not set an extension on a VM with `--ids`.</span></span>
* <span data-ttu-id="aa5bc-469">Neue Befehle wurden zu `az vm image terms accept/cancel/show` hinzugefügt , um Azure Marketplace-Imagebedingungen zu verwalten.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-469">Added new commands `az vm image terms accept/cancel/show` to manage Azure Marketplace image terms.</span></span>
* <span data-ttu-id="aa5bc-470">VMAccessForLinux auf Version 1.5 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-470">Updated VMAccessForLinux to version 1.5</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="aa5bc-471">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="aa5bc-471">CosmosDB</span></span>

* <span data-ttu-id="aa5bc-472">[BREAKING CHANGE] `az sql container create`: `--partition-key-path` in erforderlichen Parameter geändert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-472">[BREAKING CHANGE] `az sql container create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="aa5bc-473">[BREAKING CHANGE] `az gremlin graph create`: `--partition-key-path` in erforderlichen Parameter geändert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-473">[BREAKING CHANGE] `az gremlin graph create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="aa5bc-474">`az sql container create`: `--unique-key-policy` und `--conflict-resolution-policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-474">`az sql container create`: Added `--unique-key-policy` and `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="aa5bc-475">`az sql container create/update`: Aktualisierung des `--idx`-Standardschemas</span><span class="sxs-lookup"><span data-stu-id="aa5bc-475">`az sql container create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="aa5bc-476">`gremlin graph create`: `--conflict-resolution-policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-476">`gremlin graph create`: Added `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="aa5bc-477">`gremlin graph create/update`: Aktualisierung des `--idx`-Standardschemas</span><span class="sxs-lookup"><span data-stu-id="aa5bc-477">`gremlin graph create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="aa5bc-478">Tippfehler in Hilfemeldung korrigiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-478">Fixed typo in help message</span></span>
* <span data-ttu-id="aa5bc-479">Datenbank: Ablaufinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-479">database: Added deprecation infomation</span></span>
* <span data-ttu-id="aa5bc-480">Auflistung: Ablaufinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-480">collection: Added deprecation infomation</span></span>

### <a name="iot"></a><span data-ttu-id="aa5bc-481">IoT</span><span class="sxs-lookup"><span data-stu-id="aa5bc-481">IoT</span></span>

* <span data-ttu-id="aa5bc-482">Neuer Routingquelltyp hinzugefügt: DigitalTwinChangeEvents</span><span class="sxs-lookup"><span data-stu-id="aa5bc-482">Added new routing source type: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="aa5bc-483">Fehlende Features in `az iot hub create` behoben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-483">Fixed missing features in `az iot hub create`</span></span>

### <a name="key-vault"></a><span data-ttu-id="aa5bc-484">Key Vault</span><span class="sxs-lookup"><span data-stu-id="aa5bc-484">Key Vault</span></span>

* <span data-ttu-id="aa5bc-485">Ein unerwarteter Fehler wurde behoben, bei dem keine Zertifikatdatei vorhanden war.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-485">Fixed an unexpected error when certificate file does not exist</span></span>
* <span data-ttu-id="aa5bc-486">Funktionsunfähigkeit von `az keyvault recover/purge` behoben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-486">Fixed `az keyvault recover/purge` not working</span></span>

### <a name="netappfiles"></a><span data-ttu-id="aa5bc-487">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="aa5bc-487">NetAppFiles</span></span>

* <span data-ttu-id="aa5bc-488">„azure-mgmt-netapp“ wurde auf 0.6.0 aktualisiert, um API-Version 2019-07-01 zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-488">Upgraded azure-mgmt-netapp to 0.6.0 to use API version 2019-07-01.</span></span> <span data-ttu-id="aa5bc-489">Diese neue API-Version umfasst:</span><span class="sxs-lookup"><span data-stu-id="aa5bc-489">This new API version includes:</span></span>

    - <span data-ttu-id="aa5bc-490">Volumeerstellung `--protocol-types` akzeptiert jetzt „NFSv4.1“ anstelle von „NFSv4“.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-490">Volume creation `--protocol-types` accepts now "NFSv4.1" not "NFSv4"</span></span>
    - <span data-ttu-id="aa5bc-491">Die Richtlinie der Volumeexportrichtlinie heißt jetzt „nfsv41“ anstelle von „nfsv4“.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-491">Volume export policy property now named 'nfsv41' not 'nfsv4'</span></span>
    - <span data-ttu-id="aa5bc-492">Volume `--creation-token` wurde in `--file-path` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-492">Volume `--creation-token` renamed to `--file-path`</span></span>
    - <span data-ttu-id="aa5bc-493">Das Erstellungsdatum einer Momentaufnahme heißt jetzt einfach „erstellt“.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-493">Snapshot creation date now named just 'created'</span></span>

### <a name="network"></a><span data-ttu-id="aa5bc-494">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="aa5bc-494">Network</span></span>

* <span data-ttu-id="aa5bc-495">`az network private-dns link vnet create/update`: Unterstützung für mandantenübergreifende Verknüpfung virtueller Netzwerke.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-495">`az network private-dns link vnet create/update`: Support cross-tenant virtual network linking.</span></span>
* <span data-ttu-id="aa5bc-496">[BREAKING CHANGE] `az network vnet subnet list`: `--resource-group` und `--vnet-name` wurden geändert und sind jetzt erforderlich.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-496">[BREAKING CHANGE] `az network vnet subnet list`: Changed `--resource-group` and `--vnet-name` to be required now.</span></span>
* <span data-ttu-id="aa5bc-497">`az network public-ip prefix create`: Unterstützung der Angabe der IP-Adressversion (IPv4, IPv6) bei der Erstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-497">`az network public-ip prefix create`: Added support to specify IP address version (IPv4, IPv6) when creation</span></span>
* <span data-ttu-id="aa5bc-498">„azure-mgmt-network“ auf 7.0.0 und „api-version“ auf 2019-09-01 festgelegt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-498">Bumped azure-mgmt-network to 7.0.0 and api-version to 2019-09-01</span></span>
* <span data-ttu-id="aa5bc-499">`az network vrouter`: Unterstützung für neuen virtuellen Dienstrouter und virtuelles Routerpeering hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-499">`az network vrouter`: Added support for new service virtual router and virtual router peering</span></span>
* <span data-ttu-id="aa5bc-500">`az network express-route gateway connection`: Unterstützung für `--internet-security` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-500">`az network express-route gateway connection`: Added support for `--internet-security`</span></span>

### <a name="profile"></a><span data-ttu-id="aa5bc-501">Profil</span><span class="sxs-lookup"><span data-stu-id="aa5bc-501">Profile</span></span>

* <span data-ttu-id="aa5bc-502">Funktionsunfähigkeit von `az account get-access-token --resource-type ms-graph` behoben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-502">Fixed `az account get-access-token --resource-type ms-graph` not working</span></span>
* <span data-ttu-id="aa5bc-503">Warnung aus `az login` entfernt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-503">Removed warning from `az login`</span></span>

### <a name="rbac"></a><span data-ttu-id="aa5bc-504">RBAC</span><span class="sxs-lookup"><span data-stu-id="aa5bc-504">RBAC</span></span>

* <span data-ttu-id="aa5bc-505">Funktionsunfähigkeit von `az ad app update --id {} --display-name {}` behoben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-505">Fixed `az ad app update --id {} --display-name {}` doesn't work</span></span>

### <a name="servicefabric"></a><span data-ttu-id="aa5bc-506">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="aa5bc-506">ServiceFabric</span></span>

* <span data-ttu-id="aa5bc-507">`az sf cluster create`: Ein Problem wurde behoben, indem die Compute-VMSS von „template.json“ für Service Fabric unter Linux und Windows von Standarddatenträgern auf verwaltete Datenträger umgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-507">`az sf cluster create`: Fixed an issue by modifying service fabric linux and windows template.json compute vmss from standard to managed disks</span></span>

### <a name="sql"></a><span data-ttu-id="aa5bc-508">SQL</span><span class="sxs-lookup"><span data-stu-id="aa5bc-508">SQL</span></span>

* <span data-ttu-id="aa5bc-509">Die Parameter `--compute-model`, `--auto-pause-delay` und `--min-capacity` wurden hinzugefügt, um CRUD-Vorgänge für das neue SQL-Datenbank-Angebot zu unterstützen: Serverloses Computemodell.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-509">Added `--compute-model`, `--auto-pause-delay`, and `--min-capacity` parameters to support CRUD operations for new SQL Database offering: Serverless compute model.</span></span>

### <a name="storage"></a><span data-ttu-id="aa5bc-510">Storage</span><span class="sxs-lookup"><span data-stu-id="aa5bc-510">Storage</span></span>

* <span data-ttu-id="aa5bc-511">`az storage account create/update`: Parameter „--enable-files-adds“ und Azure Active Directory-Eigenschaftenargumentgruppe hinzugefügt, um Active Directory Domain-Dienstauthentifizierung für Azure Files zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-511">`az storage account create/update`: Added --enable-files-adds parameter and Azure Active Directory Properties Argument group to support Azure Files Active Directory Domain Service Authentication</span></span>
* <span data-ttu-id="aa5bc-512">`az storage account keys list/renew` wurde erweitert, um die Auflistung oder erneute Generierung von Kerberos-Schlüsseln des Speicherkontos zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-512">Expanded `az storage account keys list/renew` to support listing or regenerating Kerberos keys of storage account.</span></span>

## <a name="october-15-2019"></a><span data-ttu-id="aa5bc-513">15. Oktober 2019</span><span class="sxs-lookup"><span data-stu-id="aa5bc-513">October 15, 2019</span></span>

<span data-ttu-id="aa5bc-514">Version 2.0.75</span><span class="sxs-lookup"><span data-stu-id="aa5bc-514">Version 2.0.75</span></span>

### <a name="aks"></a><span data-ttu-id="aa5bc-515">AKS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-515">AKS</span></span>

* <span data-ttu-id="aa5bc-516">Standardwert `--load-balancer-sku` in `standard` geändert, sofern von der Kubernetes-Version unterstützt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-516">Changed `--load-balancer-sku` default value to `standard` if supported by the kubernetes version</span></span>
* <span data-ttu-id="aa5bc-517">Standardwert `--vm-set-type` in `virtualmachinescalesets` geändert, sofern von der Kubernetes-Version unterstützt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-517">Changed `--vm-set-type` default value to `virtualmachinescalesets` if supported by the kubernetes version</span></span>

### <a name="ams"></a><span data-ttu-id="aa5bc-518">AMS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-518">AMS</span></span>

* <span data-ttu-id="aa5bc-519">[BREAKING CHANGE] Name von `job start` in `job create` geändert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-519">[BREAKING CHANGE] Changed the name of `job start` to `job create`</span></span>
* <span data-ttu-id="aa5bc-520">[BREAKING CHANGE] Parameter `--ask` von `content-key-policy create` geändert, sodass eine hexadezimale Zeichenfolge mit 32 Zeichen anstelle von UTF8 verwendet wird</span><span class="sxs-lookup"><span data-stu-id="aa5bc-520">[BREAKING CHANGE] Changed the `--ask` parameter of `content-key-policy create` to use a 32-character hex string instead of UTF8</span></span>

### <a name="appservice"></a><span data-ttu-id="aa5bc-521">AppService</span><span class="sxs-lookup"><span data-stu-id="aa5bc-521">AppService</span></span>

* <span data-ttu-id="aa5bc-522">Befehle vom Typ `webapp config access-restriction show|set|add|remove` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-522">Added commands `webapp config access-restriction show|set|add|remove`</span></span>
* <span data-ttu-id="aa5bc-523">Bessere Fehlerbehandlung zu `webapp up` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-523">Added better error handling to `webapp up`</span></span>
* <span data-ttu-id="aa5bc-524">Unterstützung für SKU `Isolated` zu `appservice plan update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-524">Added support for `Isolated` SKU to `appservice plan update`</span></span>

### <a name="arm"></a><span data-ttu-id="aa5bc-525">ARM</span><span class="sxs-lookup"><span data-stu-id="aa5bc-525">ARM</span></span>

* <span data-ttu-id="aa5bc-526">Parameter `--handle-extended-json-format` zu `deployment create` hinzugefügt, um mehrere Zeilen und Kommentare in der JSON-Vorlage zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-526">Added `--handle-extended-json-format` parameter `deployment create` to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="aa5bc-527">Compute</span><span class="sxs-lookup"><span data-stu-id="aa5bc-527">Compute</span></span>

* <span data-ttu-id="aa5bc-528">Parameter `--enable-agent` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-528">Added `--enable-agent` parameter to `vm create`</span></span>
* <span data-ttu-id="aa5bc-529">`vm create` geändert, um bei der Verwendung von Zonen die SKU „Standard“ für die öffentliche IP-Adresse zu verwenden</span><span class="sxs-lookup"><span data-stu-id="aa5bc-529">Changed `vm create` to use standard public IP SKU automatically when using zones</span></span>
* <span data-ttu-id="aa5bc-530">`vm create` geändert, um automatisch einen gültigen Computernamen für eine VM zu erstellen, falls keiner angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="aa5bc-530">Changed `vm create` to automatically create a valid computer name for a VM if none is provided</span></span>
* <span data-ttu-id="aa5bc-531">Parameter `--computer-name-prefix` zu `vmss create` hinzugefügt, um das benutzerdefinierte Computernamenspräfix virtueller Computer in VMSS zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-531">Added `--computer-name-prefix` parameter to `vmss create` to support custom computer name prefix of virtual machines in the VMSS</span></span>
* <span data-ttu-id="aa5bc-532">Parameter `--workspace` zu `vm create` hinzugefügt, um automatisch einen Log Analytics-Arbeitsbereich zu aktivieren</span><span class="sxs-lookup"><span data-stu-id="aa5bc-532">Add `--workspace` parameter to `vm create` to enable log analytics workspace automatically</span></span>
* <span data-ttu-id="aa5bc-533">API-Version für Kataloge auf 2019-07-01 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-533">Updated galleries API version to 2019-07-01</span></span>

### <a name="core"></a><span data-ttu-id="aa5bc-534">Core</span><span class="sxs-lookup"><span data-stu-id="aa5bc-534">Core</span></span>

* <span data-ttu-id="aa5bc-535">Syntaxprüfung für Parameter `--set` im generischen Updatebefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-535">Added syntax check for `--set` parameter in generic update command</span></span>

### <a name="iot"></a><span data-ttu-id="aa5bc-536">IoT</span><span class="sxs-lookup"><span data-stu-id="aa5bc-536">IoT</span></span>

* <span data-ttu-id="aa5bc-537">Problem behoben, bei dem für `iot hub show` der Fehler „Ressource nicht gefunden.“ zurückgegeben wurde</span><span class="sxs-lookup"><span data-stu-id="aa5bc-537">Fixed an issue where `iot hub show` would incorrectly error with "resource not found"</span></span>

### <a name="monitor"></a><span data-ttu-id="aa5bc-538">Überwachen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-538">Monitor</span></span>

* <span data-ttu-id="aa5bc-539">Unterstützung für CRUD zu `monitor log-analytics workspace` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-539">Added support for CRUD to `monitor log-analytics workspace`</span></span>

### <a name="network"></a><span data-ttu-id="aa5bc-540">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="aa5bc-540">Network</span></span>

* <span data-ttu-id="aa5bc-541">Unterstützung für mandantenübergreifende virtuelle Verbindung zu `network private-dns link vnet [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-541">Added support for cross-tenant virtual linking to `network private-dns link vnet [create|update]`</span></span>
* <span data-ttu-id="aa5bc-542">[BREAKING CHANGE]`network vnet subnet list` geändert, um Parameter `--resource-group` und `--vnet-name` vorauszusetzen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-542">[BREAKING CHANGE] Changed `network vnet subnet list` to require `--resource-group` and `--vnet-name` parameters</span></span>

### <a name="sql"></a><span data-ttu-id="aa5bc-543">SQL</span><span class="sxs-lookup"><span data-stu-id="aa5bc-543">SQL</span></span>

* <span data-ttu-id="aa5bc-544">Befehle zu `sql mi ad-admin` hinzugefügt, die das Festlegen eines AAD-Administrators für verwaltete Instanzen unterstützen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-544">Added commands to `sql mi ad-admin` that support setting an AAD administrator on managed instances</span></span>

### <a name="storage"></a><span data-ttu-id="aa5bc-545">Storage</span><span class="sxs-lookup"><span data-stu-id="aa5bc-545">Storage</span></span>

* <span data-ttu-id="aa5bc-546">Parameter `--preserve-s2s-access-tier` zu `storage copy` hinzugefügt, um die Zugriffsebene beim Kopieren von Dienst zu Dienst beizubehalten</span><span class="sxs-lookup"><span data-stu-id="aa5bc-546">Added `--preserve-s2s-access-tier` parameter `storage copy` to preserve access tier during service to service copy</span></span>
* <span data-ttu-id="aa5bc-547">Parameter `--enable-large-file-share` zu `storage account [create|update]` hinzugefügt, um große Dateifreigaben für ein Speicherkonto zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-547">Added `--enable-large-file-share` parameter to `storage account [create|update]` to support large file shares for storage account</span></span>

## <a name="september-24-2019"></a><span data-ttu-id="aa5bc-548">24. September 2019</span><span class="sxs-lookup"><span data-stu-id="aa5bc-548">September 24, 2019</span></span>

<span data-ttu-id="aa5bc-549">Version 2.0.74</span><span class="sxs-lookup"><span data-stu-id="aa5bc-549">Version 2.0.74</span></span>

### <a name="acr"></a><span data-ttu-id="aa5bc-550">ACR</span><span class="sxs-lookup"><span data-stu-id="aa5bc-550">ACR</span></span>

* <span data-ttu-id="aa5bc-551">Erforderlicher Parameter `--type` zu `acr config retention update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-551">Added a required `--type` parameter to `acr config retention update`</span></span>
* <span data-ttu-id="aa5bc-552">[BREAKING CHANGE] Umbenannter Parameter `--name -n` in `--registry -r ` für Befehlsgruppe `acr config` geändert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-552">[BREAKING CHNAGE] Renamed parameter `--name -n` changed to `--registry -r ` for `acr config` command group</span></span>

### <a name="aks"></a><span data-ttu-id="aa5bc-553">AKS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-553">AKS</span></span>

* <span data-ttu-id="aa5bc-554">Parameter `--load-balancer-sku` zum Befehl `aks create` hinzugefügt, um die Erstellung von AKS-Clustern mit SLB zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-554">Added `--load-balancer-sku` parameter to `aks create` command, which allows for creating AKS cluster with SLB</span></span>
* <span data-ttu-id="aa5bc-555">Parameter `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` und `--load-balancer-outbound-ip-prefixes` zu den Befehlen `aks [create|update]` hinzugefügt,um die Aktualisierung des Lastenausgleichsprofils eines AKS-Clusters mit SLB zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-555">Added `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` and `--load-balancer-outbound-ip-prefixes` parameters to `aks [create|update]` commands, which allow for updating load balancer profile of an AKS cluster with SLB</span></span>
* <span data-ttu-id="aa5bc-556">Parameter `--vm-set-type` zum Befehl `aks create` hinzugefügt, um die Angabe von VM-Typen eines AKS-Clusters (vmas oder vmss) zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-556">Added `--vm-set-type` parameter to `aks create` command, which allows to specify vm types of an AKS Cluster (vmas or vmss)</span></span>

### <a name="arm"></a><span data-ttu-id="aa5bc-557">ARM</span><span class="sxs-lookup"><span data-stu-id="aa5bc-557">ARM</span></span>

* <span data-ttu-id="aa5bc-558">Parameter `--handle-extended-json-format` zum Befehl `group deployment create` hinzugefügt, um mehrere Zeilen und Kommentare in der JSON-Vorlage zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-558">Added `--handle-extended-json-format` parameter to `group deployment create` command to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="aa5bc-559">Compute</span><span class="sxs-lookup"><span data-stu-id="aa5bc-559">Compute</span></span>

* <span data-ttu-id="aa5bc-560">Parameter `--terminate-notification-time` zu den Befehlen `vmss [create|update]` hinzugefügt, um die Konfigurierbarkeit der Beendigung geplanter Ereignisse zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-560">Added `--terminate-notification-time` parameter to `vmss [create|update]` commands to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="aa5bc-561">Parameter `--enable-terminate-notification` zu den Befehlen `vmss update` hinzugefügt, um die Konfigurierbarkeit der Beendigung geplanter Ereignisse zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-561">Added `--enable-terminate-notification` parameter to `vmss update` command to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="aa5bc-562">Parameter `--priority,` `--eviction-policy,` `--max-billing` zu `[vm|vmss] create`-Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-562">Added `--priority,` `--eviction-policy,` `--max-billing` parameters to `[vm|vmss] create` commands</span></span>
* <span data-ttu-id="aa5bc-563">`disk create` geändert, um die Angabe der genauen Größe des Datenträgeruploads zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-563">Changed `disk create` to allow specifying the exact size of the disk upload</span></span>
* <span data-ttu-id="aa5bc-564">Unterstützung für inkrementelle Momentaufnahmen für verwaltete Datenträger zu `snapshot create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-564">Added support for incremental snapshots for managed disks to `snapshot create`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="aa5bc-565">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="aa5bc-565">Cosmos DB</span></span>

* <span data-ttu-id="aa5bc-566">Parameter `--type <key-type>` zum Befehl `cosmosdb keys list` hinzugefügt, um Schlüssel, schreibgeschützte Schlüssel oder Verbindungszeichenfolgen anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-566">Added `--type <key-type>` parameter to `cosmosdb keys list` command to show key, read only keys or connection strings</span></span>
* <span data-ttu-id="aa5bc-567">Befehl `cosmosdb keys regenerate` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-567">Added `cosmosdb keys regenerate` command</span></span>
* <span data-ttu-id="aa5bc-568">[VERALTET] Befehle `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` und `cosmosdb list-read-only-keys` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-568">[DEPRECATED] Deprecated `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` and `cosmosdb list-read-only-keys` commands</span></span>

### <a name="eventgrid"></a><span data-ttu-id="aa5bc-569">EventGrid</span><span class="sxs-lookup"><span data-stu-id="aa5bc-569">EventGrid</span></span>

* <span data-ttu-id="aa5bc-570">Endpunkthilfetext korrigiert, um auf den richtigen Parameter zu verweisen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-570">Fixed the endpoint help text to refer to the right parameter</span></span>

### <a name="key-vault"></a><span data-ttu-id="aa5bc-571">Key Vault</span><span class="sxs-lookup"><span data-stu-id="aa5bc-571">Key Vault</span></span>

* <span data-ttu-id="aa5bc-572">Problem behoben, aufgrund dessen die Anmeldung mit einem Mandanten (`login -t`) unter Umständen zu einem Fehler von `keyvault create` führte</span><span class="sxs-lookup"><span data-stu-id="aa5bc-572">Fixed issue where logging in with a tenant (`login -t`) could cause `keyvault create` to fail</span></span>

### <a name="monitor"></a><span data-ttu-id="aa5bc-573">Überwachen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-573">Monitor</span></span>

* <span data-ttu-id="aa5bc-574">Problem behoben, aufgrund dessen das Zeichen `:` in `--condition` für `monitor metrics alert create` nicht zulässig war</span><span class="sxs-lookup"><span data-stu-id="aa5bc-574">Fixed issue where `:` character was not allowed in `--condition` argument to `monitor metrics alert create`</span></span>

### <a name="policy"></a><span data-ttu-id="aa5bc-575">Richtlinie</span><span class="sxs-lookup"><span data-stu-id="aa5bc-575">Policy</span></span>

* <span data-ttu-id="aa5bc-576">Unterstützung für Policy-API-Version 2019-06-01 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-576">Added support for Policy API version 2019-06-01</span></span>
* <span data-ttu-id="aa5bc-577">Parameter `--enforcement-mode` zum Befehl `policy assignment create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-577">Added `--enforcement-mode` parameter to `policy assignment create` command</span></span>

### <a name="storage"></a><span data-ttu-id="aa5bc-578">Storage</span><span class="sxs-lookup"><span data-stu-id="aa5bc-578">Storage</span></span>

* <span data-ttu-id="aa5bc-579">Parameter `--blob-type` zum Befehl `az storage copy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-579">Added `--blob-type` parameter to `az storage copy` command</span></span>

## <a name="september-10-2019"></a><span data-ttu-id="aa5bc-580">10. September 2019</span><span class="sxs-lookup"><span data-stu-id="aa5bc-580">September 10, 2019</span></span>

### <a name="acr"></a><span data-ttu-id="aa5bc-581">ACR</span><span class="sxs-lookup"><span data-stu-id="aa5bc-581">ACR</span></span>

* <span data-ttu-id="aa5bc-582">Befehlsgruppe `acr config retention` zum Konfigurieren der Aufbewahrungsrichtlinie hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-582">Added command group `acr config retention` to configure retention policy</span></span>

### <a name="aks"></a><span data-ttu-id="aa5bc-583">AKS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-583">AKS</span></span>

* <span data-ttu-id="aa5bc-584">Unterstützung für die ACR-Integration mit den folgenden Befehlen hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="aa5bc-584">Added support for ACR integration with the following commands:</span></span>
  * <span data-ttu-id="aa5bc-585">Parameter `--attach-acr` zu `aks [create|update]` hinzugefügt, um einen ACR an einen AKS-Cluster anzufügen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-585">Added `--attach-acr` parameter to `aks [create|update]` to attach an ACR to an AKS cluster</span></span>
  * <span data-ttu-id="aa5bc-586">Parameter `--detach-acr` zu `aks update` hinzugefügt, um den ACR von einem AKS-Cluster zu trennen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-586">Added `--detach-acr` parameter to `aks update` to detach the ACR from an AKS cluster</span></span>

### <a name="arm"></a><span data-ttu-id="aa5bc-587">ARM</span><span class="sxs-lookup"><span data-stu-id="aa5bc-587">ARM</span></span>

* <span data-ttu-id="aa5bc-588">Zur Verwendung der API-Version 2019-05-10 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-588">Updated to use API version 2019-05-10</span></span>

### <a name="batch"></a><span data-ttu-id="aa5bc-589">Batch</span><span class="sxs-lookup"><span data-stu-id="aa5bc-589">Batch</span></span>

* <span data-ttu-id="aa5bc-590">Neue JSON-Konfigurationseinstellungen für `batch pool create` zu `--json-file` hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="aa5bc-590">Added new JSON configuration settings to `--json-file` for `batch pool create`:</span></span>
  * <span data-ttu-id="aa5bc-591">`MountConfigurations` für Dateisystemeinbindungen hinzugefügt (Details siehe https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body )</span><span class="sxs-lookup"><span data-stu-id="aa5bc-591">Added `MountConfigurations` for file system mounts (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
  * <span data-ttu-id="aa5bc-592">Optionale Eigenschaft `publicIPs` in `NetworkConfiguration` für öffentliche IP-Adressen für Pools hinzugefügt (Details siehe https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body )</span><span class="sxs-lookup"><span data-stu-id="aa5bc-592">Added optional property `publicIPs` on `NetworkConfiguration` for public IPs on pools (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
* <span data-ttu-id="aa5bc-593">Unterstützung für Kataloge mit freigegebenen Images zu `--image` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-593">Added support for shared image galleries to `--image`</span></span>
* <span data-ttu-id="aa5bc-594">[BREAKING CHANGE] Standardwert von `--start-task-wait-for-success` für `batch pool create` in `true` geändert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-594">[BREAKING CHANGE] Changed default value of `--start-task-wait-for-success` on `batch pool create` to be `true`</span></span>
* <span data-ttu-id="aa5bc-595">[BREAKING CHANGE] Standardwert von `Scope` für `AutoUserSpecification` geändert, damit immer „Pool“ verwendet wird (vormals `Task` für Windows-Knoten bzw. `Pool` für Linux-Knoten)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-595">[BREAKING CHANGE] Changed default value for `Scope` on `AutoUserSpecification` to always be Pool (was `Task` on Windows nodes, `Pool` on Linux nodes)</span></span>
  * <span data-ttu-id="aa5bc-596">Dieses Argument kann nur über eine JSON-Konfiguration mit `--json-file` festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-596">This argument can only be set from a JSON configuration with `--json-file`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="aa5bc-597">HDInsight</span><span class="sxs-lookup"><span data-stu-id="aa5bc-597">HDInsight</span></span>

* <span data-ttu-id="aa5bc-598">Allgemein verfügbares Release</span><span class="sxs-lookup"><span data-stu-id="aa5bc-598">GA release</span></span>
* <span data-ttu-id="aa5bc-599">[BREAKING CHANGE] Parameter `--workernode-count/-c` von `az hdinsight resize` in erforderlich geändert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-599">[BREAKING CHANGE] Changed parameter `--workernode-count/-c` of `az hdinsight resize` to be required.</span></span>

### <a name="key-vault"></a><span data-ttu-id="aa5bc-600">Key Vault</span><span class="sxs-lookup"><span data-stu-id="aa5bc-600">Key Vault</span></span>

* <span data-ttu-id="aa5bc-601">Problem behoben, aufgrund dessen Subnetze nicht aus Netzwerkregeln gelöscht werden konnten</span><span class="sxs-lookup"><span data-stu-id="aa5bc-601">Fixed issue where subnets couldn't be deleted from network rules</span></span>
* <span data-ttu-id="aa5bc-602">Problem behoben, aufgrund dessen doppelte Subnetze und IP-Adressen zu Netzwerkregeln hinzugefügt werden konnten</span><span class="sxs-lookup"><span data-stu-id="aa5bc-602">Fixed issue where duplicated subnets and IP addresses could be added to network rules</span></span>

### <a name="network"></a><span data-ttu-id="aa5bc-603">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="aa5bc-603">Network</span></span>

* <span data-ttu-id="aa5bc-604">Parameter `--interval` zu `network watcher flow-log` hinzugefügt, um den Wert für das Intervall der Datenverkehrsanalyse festzulegen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-604">Added `--interval` parameter to `network watcher flow-log` to set traffic analysis interval value</span></span>
* <span data-ttu-id="aa5bc-605">`network application-gateway identity` zum Verwalten der Gatewayidentität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-605">Added `network application-gateway identity` to manage gateway identity</span></span>
* <span data-ttu-id="aa5bc-606">Unterstützung zum Festlegen der Key Vault-ID zu `network application-gateway ssl-cert` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-606">Added support for setting Key Vault ID to `network application-gateway ssl-cert`</span></span>
* <span data-ttu-id="aa5bc-607">`network express-route peering peer-connection [show|list]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-607">Added `network express-route peering peer-connection [show|list]`</span></span>

### <a name="policy"></a><span data-ttu-id="aa5bc-608">Richtlinie</span><span class="sxs-lookup"><span data-stu-id="aa5bc-608">Policy</span></span>

* <span data-ttu-id="aa5bc-609">Zur Verwendung der API-Version 2019-01-01 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-609">Updated to use API version 2019-01-01</span></span>

## <a name="august-27-2019"></a><span data-ttu-id="aa5bc-610">27. August 2019</span><span class="sxs-lookup"><span data-stu-id="aa5bc-610">August 27, 2019</span></span>

<span data-ttu-id="aa5bc-611">Version 2.0.72</span><span class="sxs-lookup"><span data-stu-id="aa5bc-611">Version 2.0.72</span></span>

### <a name="acr"></a><span data-ttu-id="aa5bc-612">ACR</span><span class="sxs-lookup"><span data-stu-id="aa5bc-612">ACR</span></span>

* <span data-ttu-id="aa5bc-613">[BREAKING CHANGE] Unterstützung für SKU `classic` entfernt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-613">[BREAKING CHANGE] Removed support for the `classic` SKU</span></span>

### <a name="api-management"></a><span data-ttu-id="aa5bc-614">API Management</span><span class="sxs-lookup"><span data-stu-id="aa5bc-614">API Management</span></span>

* <span data-ttu-id="aa5bc-615">[VORSCHAU] Befehlsgruppe `apim` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-615">[PREVIEW] Added `apim` command group</span></span>

### <a name="appservice"></a><span data-ttu-id="aa5bc-616">AppService</span><span class="sxs-lookup"><span data-stu-id="aa5bc-616">AppService</span></span>

* <span data-ttu-id="aa5bc-617">Problem mit dem Befehl `webapp webjob continuous start` bei Angabe eines Slots behoben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-617">Fixed issue with `webapp webjob continuous start` command when specifying a slot</span></span>
* <span data-ttu-id="aa5bc-618">`webapp up` geändert, um den Ordner `env` zu erkennen und aus der für die Bereitstellung verwendeten Datei zu entfernen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-618">Changed `webapp up` to detect `env` folder and remove it from the file used for deployment</span></span>

### <a name="keyvault"></a><span data-ttu-id="aa5bc-619">KeyVault</span><span class="sxs-lookup"><span data-stu-id="aa5bc-619">Keyvault</span></span>

* <span data-ttu-id="aa5bc-620">Fehler in `keyvault secret set` behoben, aufgrund dessen das Argument `--expires` ignoriert wurde</span><span class="sxs-lookup"><span data-stu-id="aa5bc-620">Fixed a bug in `keyvault secret set` that igored the `--expires` argument</span></span>

### <a name="network"></a><span data-ttu-id="aa5bc-621">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="aa5bc-621">Network</span></span>

* <span data-ttu-id="aa5bc-622">Unterstützung für IPv6-Adressen zu Argumenten vom Typ `--private-ip-address-version` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-622">Added support for IPv6 addresses to `--private-ip-address-version` arguments</span></span>
* <span data-ttu-id="aa5bc-623">Neue Befehle vom Typ `network private-endpoint [create|update|list-types]` für die Verwaltung privater Endpunkte hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-623">Added new commands `network private-endpoint [create|update|list-types]` for private endpoint management</span></span>
* <span data-ttu-id="aa5bc-624">Befehlsgruppe `network private-link-service` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-624">Added command group `network private-link-service`</span></span>
* <span data-ttu-id="aa5bc-625">Argumente `--private-endpoint-network-policies` und `--private-link-service-network-policies` zu `network vnet subnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-625">Added `--private-endpoint-network-policies` and `--private-link-service-network-policies` arguments to `network vnet subnet update`</span></span>

### <a name="rbac"></a><span data-ttu-id="aa5bc-626">RBAC</span><span class="sxs-lookup"><span data-stu-id="aa5bc-626">RBAC</span></span>

* <span data-ttu-id="aa5bc-627">Problem mit `ad app update --homepage` behoben, aufgrund dessen die Startseite nicht aktualisiert wurde</span><span class="sxs-lookup"><span data-stu-id="aa5bc-627">Fixed issue with `ad app update --homepage` where homepage would not be updated</span></span>

### <a name="servicefabric"></a><span data-ttu-id="aa5bc-628">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="aa5bc-628">ServiceFabric</span></span>

* <span data-ttu-id="aa5bc-629">Unterstützung für Key Vault-Namen mit Groß- und Kleinschreibung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-629">Added support for mixed-case Key Vault names</span></span>
* <span data-ttu-id="aa5bc-630">Problem bei der Verwendung von Zertifikaten in Key Vault behoben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-630">Fixed issue when using certificates in Key Vault</span></span>
* <span data-ttu-id="aa5bc-631">Problem bei der Verwendung von PFX-Zertifikatdateien behoben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-631">Fixed issue with using PFX certificate files</span></span>
* <span data-ttu-id="aa5bc-632">Problem mit `sf cluster certificate add` behoben, wenn keine Key Vault-Ressourcengruppe angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="aa5bc-632">Fixed issue with `sf cluster certificate add` when Key Vault resource group wasn't specified</span></span>
* <span data-ttu-id="aa5bc-633">Problem behoben, aufgrund dessen `sf cluster set` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="aa5bc-633">Fixed issue with `sf cluster set` not working</span></span>

### <a name="signalr"></a><span data-ttu-id="aa5bc-634">SignalR</span><span class="sxs-lookup"><span data-stu-id="aa5bc-634">SignalR</span></span>

* <span data-ttu-id="aa5bc-635">Neue Befehle hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="aa5bc-635">Added new commands:</span></span>
  * <span data-ttu-id="aa5bc-636">`signalr cors`: Verwalten von CORS für SignalR</span><span class="sxs-lookup"><span data-stu-id="aa5bc-636">`signalr cors`: Manage SignalR CORS</span></span>
  * <span data-ttu-id="aa5bc-637">`signalr restart`: Starten eines SignalR-Diensts</span><span class="sxs-lookup"><span data-stu-id="aa5bc-637">`signalr restart`: Restart a SignalR service</span></span>
  * <span data-ttu-id="aa5bc-638">`signalr update`: Aktualisieren eines SignalR-Diensts</span><span class="sxs-lookup"><span data-stu-id="aa5bc-638">`signalr update`: Update a SignalR service</span></span>
* <span data-ttu-id="aa5bc-639">Argument `--service-mode` zu `signalr create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-639">Added `--service-mode` argument to `signalr create`</span></span>

### <a name="storage"></a><span data-ttu-id="aa5bc-640">Storage</span><span class="sxs-lookup"><span data-stu-id="aa5bc-640">Storage</span></span>

* <span data-ttu-id="aa5bc-641">Befehl `storage account revoke-delegation-keys` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-641">Added `storage account revoke-delegation-keys` command</span></span>

## <a name="august-13-2019"></a><span data-ttu-id="aa5bc-642">13. August 2019</span><span class="sxs-lookup"><span data-stu-id="aa5bc-642">August 13, 2019</span></span>

<span data-ttu-id="aa5bc-643">Version 2.0.71</span><span class="sxs-lookup"><span data-stu-id="aa5bc-643">Version 2.0.71</span></span>

### <a name="appservice"></a><span data-ttu-id="aa5bc-644">AppService</span><span class="sxs-lookup"><span data-stu-id="aa5bc-644">AppService</span></span>

* <span data-ttu-id="aa5bc-645">Problem behoben, aufgrund dessen bei Befehlen vom Typ `webapp webjob continuous` für Slots Fehler auftraten</span><span class="sxs-lookup"><span data-stu-id="aa5bc-645">Fixed issue where `webapp webjob continuous` commands were failing for slots</span></span>

### <a name="botservice"></a><span data-ttu-id="aa5bc-646">BotService</span><span class="sxs-lookup"><span data-stu-id="aa5bc-646">BotService</span></span>

* <span data-ttu-id="aa5bc-647">[BREAKING CHANGE] Unterstützung für die Erstellung von Bots der Version 3 entfernt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-647">[BREAKING CHANGE] Removed support for creating v3 SDK bots</span></span>

### <a name="cognitiveservices"></a><span data-ttu-id="aa5bc-648">CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="aa5bc-648">CognitiveServices</span></span>

* <span data-ttu-id="aa5bc-649">Befehle vom Typ `cognitiveservices account network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-649">Added `cognitiveservices account network-rule` commands</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="aa5bc-650">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="aa5bc-650">Cosmos DB</span></span>

* <span data-ttu-id="aa5bc-651">Beim Aktualisieren mehrerer Schreibstandorte wurde eine Warnung entfernt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-651">Removed warning when updating multiple write locations</span></span>
* <span data-ttu-id="aa5bc-652">CRUD-Befehle für CosmosDB SQL-, MongoDB-, Cassandra-, Gremlin- und Tabellenressourcen sowie den Ressourcendurchsatz hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-652">Added CRUD commands for CosmosDB SQL, MongoDB, Cassandra, Gremlin and Table resources and resource's throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="aa5bc-653">HDInsight</span><span class="sxs-lookup"><span data-stu-id="aa5bc-653">HDInsight</span></span>

<span data-ttu-id="aa5bc-654">Dieses Release enthält zahlreiche wichtige Änderungen.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-654">This release contains a large number of breaking changes.</span></span>

* <span data-ttu-id="aa5bc-655">[BREAKING CHANGE] Parameter für `hdinsight create` umbenannt:</span><span class="sxs-lookup"><span data-stu-id="aa5bc-655">[BREAKING CHANGE] Renamed parameters for `hdinsight create`:</span></span>
  * <span data-ttu-id="aa5bc-656">`--storage-default-container` in `--storage-container` umbenannt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-656">Renamed `--storage-default-container` to `--storage-container`</span></span>
  * <span data-ttu-id="aa5bc-657">`--storage-default-filesystem` in `--storage-filesystem` umbenannt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-657">Renamed `--storage-default-filesystem` to `--storage-filesystem`</span></span>
* <span data-ttu-id="aa5bc-658">[BREAKING CHANGE] Das Argument `--name` von `application create` wurde so geändert, dass es den Anwendungsnamen anstelle des Clusternamens darstellt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-658">[BREAKING CHANGE] Changed the `--name` argument of `application create` to represent the application name instead of the cluster name</span></span>
* <span data-ttu-id="aa5bc-659">Argument `--cluster-name` zu `application create` hinzugefügt, um die alte Funktion `--name` zu ersetzen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-659">Added `--cluster-name` argument to `application create` to replace old `--name` functionality</span></span>
* <span data-ttu-id="aa5bc-660">[BREAKING CHANGE] Parameter für `application create` umbenannt:</span><span class="sxs-lookup"><span data-stu-id="aa5bc-660">[BREAKING CHANGE] Renamed parameters for `application create`:</span></span>
  * <span data-ttu-id="aa5bc-661">`--application-type` in `--type` umbenannt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-661">Renamed `--application-type` to `--type`</span></span>
  * <span data-ttu-id="aa5bc-662">`--marketplace-identifier` in `--marketplace-id` umbenannt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-662">Renamed `--marketplace-identifier` to `--marketplace-id`</span></span>
  * <span data-ttu-id="aa5bc-663">`--https-endpoint-access-mode` in `--access-mode` umbenannt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-663">Renamed `--https-endpoint-access-mode` to `--access-mode`</span></span>
  * <span data-ttu-id="aa5bc-664">`--https-endpoint-destination-port` in `--destination-port` umbenannt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-664">Renamed  `--https-endpoint-destination-port` to `--destination-port`</span></span>
* <span data-ttu-id="aa5bc-665">[BREAKING CHANGE] Parameter für `application create` entfernt:</span><span class="sxs-lookup"><span data-stu-id="aa5bc-665">[BREAKING CHANGE] Removed parameters for `application create`:</span></span>
  * `--https-endpoint-location`
  * `--https-endpoint-public-port`
  * `--ssh-endpoint-destination-port`
  * `--ssh-endpoint-location`
  * `--ssh-endpoint-public-port`
* <span data-ttu-id="aa5bc-666">[WICHTIGE ÄNDERUNG] `--target-instance-count` für `hdinsight resize` in `--workernode-count` umbenannt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-666">[BREAKING CHNAGE] Renamed `--target-instance-count` to `--workernode-count` for `hdinsight resize`</span></span>
* <span data-ttu-id="aa5bc-667">[BREAKING CHANGE] Alle Befehle in der Gruppe `hdinsight script-action` wurden so geändert, dass sie den Parameter `--name` als Namen der Skriptaktion verwenden.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-667">[BREAKING CHANGE] Changed all commands in the `hdinsight script-action` group to use the `--name` parameter as the name of the script action.</span></span>
* <span data-ttu-id="aa5bc-668">Argument `--cluster-name` zu allen Befehlen vom Typ `hdinsight script-action` hinzugefügt, um die alte Funktion `--name` zu ersetzen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-668">Added `--cluster-name` argument to all `hdinsight script-action` commands to replace old `--name` functionality</span></span>
* <span data-ttu-id="aa5bc-669">[BREAKING CHANGE]`--script-execution-id` für alle Befehle vom Typ `hdinsight script-action` in `--execution-id` umbenannt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-669">[BREAKING CHANGE] Renamed `--script-execution-id` to `--execution-id` for all `hdinsight script-action` commands</span></span>
* <span data-ttu-id="aa5bc-670">[BREAKING CHANGE]`hdinsight script-action show` in `hdinsight script-action show-execution-details` umbenannt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-670">[BREAKING CHANGE] Renamed `hdinsight script-action show` to `hdinsight script-action show-execution-details`</span></span>
* <span data-ttu-id="aa5bc-671">[WICHTIGE ÄNDERUNG] Parameter in `hdinsight script-action execute --roles` geändert, sodass sie durch Leerzeichen anstelle von Kommas getrennt sind</span><span class="sxs-lookup"><span data-stu-id="aa5bc-671">[BREAKING CHNAGE] Changed parameters to `hdinsight script-action execute --roles` to be space-separated instead of comma-separated</span></span>
* <span data-ttu-id="aa5bc-672">[BREAKING CHANGE] Parameter `--persisted` für `hdinsight script-action list` entfernt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-672">[BREAKING CHANGE] Removed the `--persisted` parameter of `hdinsight script-action list`</span></span>
* <span data-ttu-id="aa5bc-673">Der Parameter `hdinsight create --cluster-configurations` wurde so geändert, dass er einen Pfad zu einer lokalen JSON-Datei oder JSON-Zeichenfolge akzeptiert.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-673">Changed the `hdinsight create --cluster-configurations` parameter to accept a path to a local JSON file or a JSON string</span></span>
* <span data-ttu-id="aa5bc-674">Befehl `hdinsight script-action list-execution-history` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-674">Added command `hdinsight script-action list-execution-history`</span></span>
* <span data-ttu-id="aa5bc-675">`hdinsight monitor enable --workspace` geändert, um die ID oder den Namen eines Log Analytics-Arbeitsbereichs zu akzeptieren</span><span class="sxs-lookup"><span data-stu-id="aa5bc-675">Changed `hdinsight monitor enable --workspace` to accept a Log Analytics workspace ID or workspace name</span></span>
* <span data-ttu-id="aa5bc-676">Argument `hdinsight monitor enable --primary-key` hinzugefügt. Dieses Argument wird benötigt, wenn eine Arbeitsbereichs-ID als Parameter angegeben wird.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-676">Added the `hdinsight monitor enable --primary-key` argument, which is needed if a workspace ID is provided as the parameter</span></span>
* <span data-ttu-id="aa5bc-677">Weitere Beispiele und aktualisierte Beschreibungen für Hilfemeldungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-677">Added more examples and updated descriptions for help messages</span></span>

### <a name="interactive"></a><span data-ttu-id="aa5bc-678">Interactive</span><span class="sxs-lookup"><span data-stu-id="aa5bc-678">Interactive</span></span>

* <span data-ttu-id="aa5bc-679">Ladefehler behoben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-679">Fixed a loading error</span></span>

### <a name="kubernetes"></a><span data-ttu-id="aa5bc-680">Kubernetes</span><span class="sxs-lookup"><span data-stu-id="aa5bc-680">Kubernetes</span></span>

* <span data-ttu-id="aa5bc-681">Änderung, um `https` zu verwenden, wenn der Dashboardcontainerport `https` verwendet</span><span class="sxs-lookup"><span data-stu-id="aa5bc-681">Changed to use `https` if dashboard container port is using `https`</span></span>

### <a name="network"></a><span data-ttu-id="aa5bc-682">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="aa5bc-682">Network</span></span>

* <span data-ttu-id="aa5bc-683">Argument `--yes` hinzugefügt zu `network dns record-set cname delete`</span><span class="sxs-lookup"><span data-stu-id="aa5bc-683">Added `--yes` argument `network dns record-set cname delete`</span></span>

### <a name="profile"></a><span data-ttu-id="aa5bc-684">Profil</span><span class="sxs-lookup"><span data-stu-id="aa5bc-684">Profile</span></span>

* <span data-ttu-id="aa5bc-685">Argument `--resource-type` zu `account get-access-token` zum Abrufen von Ressourcenzugriffstoken hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-685">Added `--resource-type` argument to `account get-access-token` to get resource access tokens</span></span>

### <a name="servicefabric"></a><span data-ttu-id="aa5bc-686">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="aa5bc-686">ServiceFabric</span></span>

* <span data-ttu-id="aa5bc-687">Alle unterstützten Betriebssystemversionen für „sf cluster create“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-687">Added all supported os version for sf cluster create</span></span>
* <span data-ttu-id="aa5bc-688">Fehler beim Überprüfen des primären Zertifikats behoben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-688">Fixed primary certificate validation bug</span></span>

### <a name="storage"></a><span data-ttu-id="aa5bc-689">Storage</span><span class="sxs-lookup"><span data-stu-id="aa5bc-689">Storage</span></span>

* <span data-ttu-id="aa5bc-690">Befehl `storage copy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-690">Added command `storage copy`</span></span>

## <a name="july-30-2019"></a><span data-ttu-id="aa5bc-691">30. Juli 2019</span><span class="sxs-lookup"><span data-stu-id="aa5bc-691">July 30, 2019</span></span>

<span data-ttu-id="aa5bc-692">Version 2.0.70</span><span class="sxs-lookup"><span data-stu-id="aa5bc-692">Version 2.0.70</span></span>

### <a name="acr"></a><span data-ttu-id="aa5bc-693">ACR</span><span class="sxs-lookup"><span data-stu-id="aa5bc-693">ACR</span></span>

* <span data-ttu-id="aa5bc-694">Problem #9952 behoben (Regression im Befehl `acr pack build`)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-694">Fixed issue #9952 (a regression in the `acr pack build` command)</span></span>
* <span data-ttu-id="aa5bc-695">Standardname des Generatorimages in `acr pack build` entfernt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-695">Removed the default builder image name in `acr pack build`</span></span>

### <a name="appservice"></a><span data-ttu-id="aa5bc-696">AppService</span><span class="sxs-lookup"><span data-stu-id="aa5bc-696">Appservice</span></span>

* <span data-ttu-id="aa5bc-697">`webapp config ssl` geändert, um eine Meldung anzuzeigen, wenn eine Ressource nicht gefunden wurde</span><span class="sxs-lookup"><span data-stu-id="aa5bc-697">Changed `webapp config ssl` to show a message if a resource is not found</span></span>
* <span data-ttu-id="aa5bc-698">Problem behoben, aufgrund dessen `functionapp create` den Speicherkontotypen `Standard_RAGRS` nicht akzeptiert hat</span><span class="sxs-lookup"><span data-stu-id="aa5bc-698">Fixed issue where `functionapp create` does not accept `Standard_RAGRS` storage account type</span></span>
* <span data-ttu-id="aa5bc-699">Problem behoben, aufgrund dessen für `webapp up` ein Fehler auftrat, wenn für die Ausführung ältere Python-Versionen verwendet wurden</span><span class="sxs-lookup"><span data-stu-id="aa5bc-699">Fixed an issue where `webapp up` would fail if run using older versions of python</span></span>

### <a name="network"></a><span data-ttu-id="aa5bc-700">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="aa5bc-700">Network</span></span>

* <span data-ttu-id="aa5bc-701">Ungültiger Parameter `--ids` aus `network nic ip-config add` entfernt (Fehlerbehebungen #9861)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-701">Removed invalid parameter `--ids` from `network nic ip-config add` (fixes #9861)</span></span>
* <span data-ttu-id="aa5bc-702">Fehlerbehebungen #9604.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-702">Fixes #9604.</span></span> <span data-ttu-id="aa5bc-703">Parameter `--root-certs` zu `network application-gateway http-settings [create|update]` hinzugefügt, um vom Benutzer zugewiesene vertrauenswürdige Stammzertifikate zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-703">Added `--root-certs` parameter to `network application-gateway http-settings [create|update]` to support user associate trusted root certificates.</span></span>
* <span data-ttu-id="aa5bc-704">Argument `--subscription` für `network dns record-set ns create` korrigiert (#9965)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-704">Fixed arguent `--subscription` for `network dns record-set ns create` (#9965)</span></span>

### <a name="rbac"></a><span data-ttu-id="aa5bc-705">RBAC</span><span class="sxs-lookup"><span data-stu-id="aa5bc-705">RBAC</span></span>

* <span data-ttu-id="aa5bc-706">Befehl `user update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-706">Added `user update` command</span></span>
* <span data-ttu-id="aa5bc-707">[VERALTET]`--upn-or-object-id` in benutzerbezogenen Befehlen als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-707">[DEPRECATED] Deprecated `--upn-or-object-id` from user-related commands</span></span>
    * <span data-ttu-id="aa5bc-708">Verwenden Sie das Ersatzargument `--id`.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-708">Use replacement argument `--id`</span></span>
* <span data-ttu-id="aa5bc-709">Argument `--id` zu benutzerbezogenen Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-709">Added `--id` argument to user-related commands</span></span>

### <a name="sql"></a><span data-ttu-id="aa5bc-710">SQL</span><span class="sxs-lookup"><span data-stu-id="aa5bc-710">SQL</span></span>

* <span data-ttu-id="aa5bc-711">Verwaltungsbefehle für Schlüssel verwalteter Instanzen und TDE-Schutzvorrichtung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-711">Added management commands for managed instance keys and TDE protector</span></span>

### <a name="storage"></a><span data-ttu-id="aa5bc-712">Storage</span><span class="sxs-lookup"><span data-stu-id="aa5bc-712">Storage</span></span>

* <span data-ttu-id="aa5bc-713">Befehl `storage remove` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-713">Added `storage remove` command</span></span>
* <span data-ttu-id="aa5bc-714">Problem mit `storage blob update` behoben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-714">Fixed an issue with `storage blob update`</span></span>

### <a name="vm"></a><span data-ttu-id="aa5bc-715">VM</span><span class="sxs-lookup"><span data-stu-id="aa5bc-715">VM</span></span>

* <span data-ttu-id="aa5bc-716">`list-skus` wurde geändert, um eine neuere API-Version für die Ausgabe von Zonendetails zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-716">Changed `list-skus` to use newer api-version to output zone details</span></span>
* <span data-ttu-id="aa5bc-717">Standardwert `--single-placement-group` für `vmss create` in `false` geändert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-717">Changed default of `--single-placement-group` to `false` for `vmss create`</span></span>
* <span data-ttu-id="aa5bc-718">Möglichkeit zum Auswählen von ZRS-Speicher-SKUs für `[snapshot|disk] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-718">Added ability to select ZRS storage SKUs for `[snapshot|disk] create`</span></span>
* <span data-ttu-id="aa5bc-719">Neue Befehlsgruppe `vm host` zur Unterstützung dedizierter Hosts hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-719">Added new command group `vm host` to support dedicated hosts</span></span>
* <span data-ttu-id="aa5bc-720">Parameter `--host` und `--host-group` für `vm create` hinzugefügt, um den dedizierten VM-Host festzulegen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-720">Added parameters `--host` and `--host-group` on `vm create` to set VM dedicated host</span></span>

## <a name="july-16-2019"></a><span data-ttu-id="aa5bc-721">16. Juli 2019</span><span class="sxs-lookup"><span data-stu-id="aa5bc-721">July 16, 2019</span></span>

<span data-ttu-id="aa5bc-722">Version 2.0.69</span><span class="sxs-lookup"><span data-stu-id="aa5bc-722">Version 2.0.69</span></span>

### <a name="appservice"></a><span data-ttu-id="aa5bc-723">AppService</span><span class="sxs-lookup"><span data-stu-id="aa5bc-723">Appservice</span></span>

* <span data-ttu-id="aa5bc-724">`webapp identity`-Befehle geändert, um eine korrekte Fehlermeldung zurückzugeben, wenn „ResourceGroupName“ oder der App-Name ungültig sind</span><span class="sxs-lookup"><span data-stu-id="aa5bc-724">Changed `webapp identity` commands to return a proper error message if ResourceGroupName or App name are invalid</span></span>
* <span data-ttu-id="aa5bc-725">`webapp list` korrigiert, sodass der korrekte Wert für „numberOfSites“ zurückgegeben wird, wenn „ResourceGroup“ nicht angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="aa5bc-725">Fixed `webapp list` to return the correct value for numberOfSites if no ResourceGroup was provided</span></span>
* <span data-ttu-id="aa5bc-726">Nebeneffekte von `appservice plan create` und `webapp create` behoben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-726">Fixed side-effects of `appservice plan create` and `webapp create`</span></span>

### <a name="core"></a><span data-ttu-id="aa5bc-727">Core</span><span class="sxs-lookup"><span data-stu-id="aa5bc-727">Core</span></span>

* <span data-ttu-id="aa5bc-728">Problem behoben, aufgrund dessen `--subscription` angezeigt wurde, obwohl nicht anwendbar</span><span class="sxs-lookup"><span data-stu-id="aa5bc-728">Fixed issue where `--subscription` would appear despite being not applicable</span></span>

### <a name="batch"></a><span data-ttu-id="aa5bc-729">Batch</span><span class="sxs-lookup"><span data-stu-id="aa5bc-729">Batch</span></span>

* <span data-ttu-id="aa5bc-730">[BREAKING CHANGE]`batch pool node-agent-skus list` durch `batch pool supported-images list` ersetzt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-730">[BREAKING CHANGE] Replaced `batch pool node-agent-skus list` with `batch pool supported-images list`</span></span>
* <span data-ttu-id="aa5bc-731">Unterstützung für Sicherheitsregeln hinzugefügt, die den Netzwerkzugriff auf einen Pool basierend auf dem Quellport des Datenverkehrs blockieren, wenn die Option `--json-file` von `batch pool create network` verwendet wird</span><span class="sxs-lookup"><span data-stu-id="aa5bc-731">Added support for security rules blocking network access to a pool based on the source port of the traffic when using the `--json-file` option of `batch pool create network`</span></span>
* <span data-ttu-id="aa5bc-732">Unterstützung für die Ausführung der Aufgabe im Arbeitsverzeichnis des Containers oder der Batch-Aufgabe hinzugefügt, wenn die Option `--json-file` von `batch task create` verwendet wird</span><span class="sxs-lookup"><span data-stu-id="aa5bc-732">Added support for executing the task in the container working directory or in the Batch task working directory when using the `--json-file` option of `batch task create`</span></span>
* <span data-ttu-id="aa5bc-733">Fehler in Option `--application-package-references` von `batch pool create` behoben, aufgrund dessen nur Standardeinstellungen möglich waren</span><span class="sxs-lookup"><span data-stu-id="aa5bc-733">Fixed error in `--application-package-references` option of `batch pool create` where it would only work with defaults</span></span>

### <a name="eventhubs"></a><span data-ttu-id="aa5bc-734">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="aa5bc-734">Eventhubs</span></span>

* <span data-ttu-id="aa5bc-735">Validierung für Parameter `--rights` von `authorizationrule`-Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-735">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="rdbms"></a><span data-ttu-id="aa5bc-736">RDBMS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-736">RDBMS</span></span>

* <span data-ttu-id="aa5bc-737">Optionaler Parameter zum Angeben der Replikat-SKU für den Befehl zum Erstellen von Replikaten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-737">Added optional parameter to specify replica SKU for create replica command</span></span>
* <span data-ttu-id="aa5bc-738">Problem mit CI-Testfehler bei der Erstellung von MySQL-Replikaten behoben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-738">Fixed the issue with CI test failure with creating MySQL replica</span></span>

### <a name="relay"></a><span data-ttu-id="aa5bc-739">Relay</span><span class="sxs-lookup"><span data-stu-id="aa5bc-739">Relay</span></span>

* <span data-ttu-id="aa5bc-740">Problem mit Hybridverbindung behoben, wenn die Client-Autorisierung deaktiviert ist [#8775](https://github.com/azure/azure-cli/issues/8775)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-740">Fixed issue with hybrid connection when client authroization disabled [#8775](https://github.com/azure/azure-cli/issues/8775)</span></span>
* <span data-ttu-id="aa5bc-741">Parameter `--requires-transport-security` zu `relay wcfrelay create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-741">Added parameter `--requires-transport-security` to `relay wcfrelay create`</span></span>

### <a name="servicebus"></a><span data-ttu-id="aa5bc-742">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="aa5bc-742">Servicebus</span></span>

* <span data-ttu-id="aa5bc-743">Validierung für Parameter `--rights` von `authorizationrule`-Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-743">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="storage"></a><span data-ttu-id="aa5bc-744">Storage</span><span class="sxs-lookup"><span data-stu-id="aa5bc-744">Storage</span></span>

* <span data-ttu-id="aa5bc-745">AADDS für Files für Speicherkontoaktualisierung aktiviert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-745">Enable Files AADDS for storage account update</span></span>
* <span data-ttu-id="aa5bc-746">Problem `storage blob service-properties update --set` behoben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-746">Fixed issue `storage blob service-properties update --set`</span></span>

## <a name="july-2-2019"></a><span data-ttu-id="aa5bc-747">2\. Juli 2019</span><span class="sxs-lookup"><span data-stu-id="aa5bc-747">July 2, 2019</span></span>

<span data-ttu-id="aa5bc-748">Version 2.0.68</span><span class="sxs-lookup"><span data-stu-id="aa5bc-748">Version 2.0.68</span></span>

### <a name="core"></a><span data-ttu-id="aa5bc-749">Core</span><span class="sxs-lookup"><span data-stu-id="aa5bc-749">Core</span></span>

* <span data-ttu-id="aa5bc-750">Befehlsmodule sind jetzt in einer einzelnen verteilbaren Python-Komponente zusammengefasst.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-750">Command modules are now consolidated into a single Python distributable.</span></span> <span data-ttu-id="aa5bc-751">Die direkte Verwendung zahlreicher Pakete vom Typ `azure-cli-` in PyPI ist daher veraltet.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-751">This deprecates direct use of many `azure-cli-` packages on PyPI.</span></span>
  <span data-ttu-id="aa5bc-752">Dadurch sollte sich die Installationsgröße reduzieren. Darüber hinaus sollte es nur Benutzer betreffen, die eine direkte Installation über `pip` ausgeführt haben.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-752">This should reduce install size and only affect users who have directly installed via `pip`.</span></span>

### <a name="acr"></a><span data-ttu-id="aa5bc-753">ACR</span><span class="sxs-lookup"><span data-stu-id="aa5bc-753">ACR</span></span>

* <span data-ttu-id="aa5bc-754">Unterstützung für Trigger mit Timer zu Aufgabe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-754">Added support for Timer Triggers to Task</span></span>

### <a name="appservice"></a><span data-ttu-id="aa5bc-755">AppService</span><span class="sxs-lookup"><span data-stu-id="aa5bc-755">Appservice</span></span>

* <span data-ttu-id="aa5bc-756">`functionapp create` wurde so geändert, das Application Insights standardmäßig aktiviert wird.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-756">Changed `functionapp create` to enable application insights by default</span></span>
* <span data-ttu-id="aa5bc-757">[BREAKING CHANGE] Veralteter Befehl `functionapp devops-build` entfernt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-757">[BREAKING CHANGE] Removed deprecated `functionapp devops-build` command.</span></span>
  *  <span data-ttu-id="aa5bc-758">Verwenden Sie stattdessen den neuen Befehl `az functionapp devops-pipeline`.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-758">Use the new command `az functionapp devops-pipeline` instead</span></span>
* <span data-ttu-id="aa5bc-759">Unterstützung des Funktions-App-Plans für Linux-Verbrauch zu `functionapp deployment config-zip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-759">Added Linux Consumption function app plan support to `functionapp deployment config-zip`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="aa5bc-760">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="aa5bc-760">Cosmos DB</span></span>

* <span data-ttu-id="aa5bc-761">Unterstützung für das Deaktivieren von TTL hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-761">Added support for disabling TTL</span></span>

### <a name="dls"></a><span data-ttu-id="aa5bc-762">DLS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-762">DLS</span></span>

* <span data-ttu-id="aa5bc-763">Aktualisierte ADLS-Version (0.0.45)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-763">Updated ADLS version (0.0.45)</span></span>

### <a name="feedback"></a><span data-ttu-id="aa5bc-764">Feedback</span><span class="sxs-lookup"><span data-stu-id="aa5bc-764">Feedback</span></span>

* <span data-ttu-id="aa5bc-765">Wird ein fehlgeschlagener Erweiterungsbefehl gemeldet, versucht `az feedback` nun, über den Index die Projekt-/Repository-URL der Erweiterung im Browser zu öffnen.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-765">When reporting a failed extension command, `az feedback` now attempts to open the browser to the project/repo url of the extension from the index</span></span>

### <a name="hdinsight"></a><span data-ttu-id="aa5bc-766">HDInsight</span><span class="sxs-lookup"><span data-stu-id="aa5bc-766">HDInsight</span></span>

* <span data-ttu-id="aa5bc-767">[BREAKING CHANGE] Der Befehlsgruppenname `oms` wurde in `monitor` geändert.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-767">[BREAKING CHANGE] Changed `oms` command group name to `monitor`</span></span>
* <span data-ttu-id="aa5bc-768">[BREAKING CHANGE]`--http-password/-p` als erforderlicher Parameter festgelegt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-768">[BREAKING CHANGE] Made `--http-password/-p` a required parameter</span></span> 
* <span data-ttu-id="aa5bc-769">Vervollständigungen für `--cluster-admin-account` und `cluster-users-group-dns` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-769">Added completers for `--cluster-admin-account` and `cluster-users-group-dns` parameters completer</span></span> 
* <span data-ttu-id="aa5bc-770">Parameter `cluster-users-group-dns` so geändert, dass er erforderlich ist, wenn `—esp` vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="aa5bc-770">Changed `cluster-users-group-dns` parameter to be required when `—esp` is present</span></span>
* <span data-ttu-id="aa5bc-771">Timeout für alle vorhandenen automatischen Argumentvervollständigungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-771">Added a timeout for all existing argument auto-completers</span></span>
* <span data-ttu-id="aa5bc-772">Timeout für das Transformieren des Ressourcennamens in eine Ressourcen-ID hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-772">Added a timeout for transforming resource name to resource id</span></span>
* <span data-ttu-id="aa5bc-773">Die automatischen Vervollständigungen wurden so geändert, dass Ressourcen aus einer beliebigen Ressourcengruppe ausgewählt werden.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-773">Changed Auto-completers to select resources from any resource group.</span></span> <span data-ttu-id="aa5bc-774">Dabei kann es sich um eine andere Ressourcengruppe als die mit `-g` angegebene Gruppe handeln.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-774">It can be a different resource group than the one specified with `-g`</span></span>
* <span data-ttu-id="aa5bc-775">Unterstützung für die Parameter `--sub-domain-suffix` und `--disable_gateway_auth` im Befehl `hdinsight application create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-775">Added support for `--sub-domain-suffix` and `--disable_gateway_auth` parameters in the `hdinsight application create` command</span></span>

### <a name="managed-services"></a><span data-ttu-id="aa5bc-776">Verwaltete Dienste</span><span class="sxs-lookup"><span data-stu-id="aa5bc-776">Managed Services</span></span>

* <span data-ttu-id="aa5bc-777">Befehlsmodul für verwaltete Dienste als Vorschau eingeführt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-777">Introducing managed service command module in preview</span></span>

### <a name="profile"></a><span data-ttu-id="aa5bc-778">Profil</span><span class="sxs-lookup"><span data-stu-id="aa5bc-778">Profile</span></span>
* <span data-ttu-id="aa5bc-779">Argument `--subscription` für Abmeldebefehl unterdrückt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-779">Suppress `--subscription` argument for logout command</span></span>

### <a name="rbac"></a><span data-ttu-id="aa5bc-780">RBAC</span><span class="sxs-lookup"><span data-stu-id="aa5bc-780">RBAC</span></span>

* <span data-ttu-id="aa5bc-781">[BREAKING CHANGE] Argument `--password` für `create-for-rbac` entfernt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-781">[BREAKING CHANGE] Removed `--password` argument for `create-for-rbac`</span></span>
* <span data-ttu-id="aa5bc-782">Parameter `--assignee-principal-type` zum Befehl `create` hinzugefügt, um zeitweilige Fehler zu vermeiden, die durch die Replikationswartezeit des AAD-Graph-Servers verursacht werden</span><span class="sxs-lookup"><span data-stu-id="aa5bc-782">Added `--assignee-principal-type` parameter to `create` command to avoid intermittent failures caused by AAD graph server replication latency</span></span>
* <span data-ttu-id="aa5bc-783">Absturz in `ad signed-in-user` beim Auflisten von in Besitz befindlichen Objekten behoben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-783">Fixed a crash in `ad signed-in-user` when listing owned objects</span></span>
* <span data-ttu-id="aa5bc-784">Problem behoben, aufgrund dessen `ad sp` nicht die richtige Anwendung über einen Dienstprinzipal fand</span><span class="sxs-lookup"><span data-stu-id="aa5bc-784">Fixed issue where `ad sp` would not find the right application from a service principal</span></span>

### <a name="rdbms"></a><span data-ttu-id="aa5bc-785">RDBMS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-785">RDBMS</span></span>

* <span data-ttu-id="aa5bc-786">Unterstützung für die Replikation für MariaDB hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-786">Added support for replication for MariaDB</span></span>

### <a name="sql"></a><span data-ttu-id="aa5bc-787">SQL</span><span class="sxs-lookup"><span data-stu-id="aa5bc-787">SQL</span></span>

* <span data-ttu-id="aa5bc-788">Zulässige Werte für `sql db create --sample-name` dokumentiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-788">Documented allowed values for `sql db create --sample-name`</span></span>

### <a name="storage"></a><span data-ttu-id="aa5bc-789">Storage</span><span class="sxs-lookup"><span data-stu-id="aa5bc-789">Storage</span></span>

* <span data-ttu-id="aa5bc-790">Unterstützung von SAS-Token für die Benutzerdelegierung mit `--as-user` zu `storage blob generate-sas` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-790">Added user delegation SAS token support with `--as-user` to `storage blob generate-sas`</span></span> 
* <span data-ttu-id="aa5bc-791">Unterstützung von SAS-Token für die Benutzerdelegierung mit `--as-user` zu `storage container generate-sas` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-791">Added user delegation SAS token support with `--as-user` to `storage container generate-sas`</span></span> 

### <a name="vm"></a><span data-ttu-id="aa5bc-792">VM</span><span class="sxs-lookup"><span data-stu-id="aa5bc-792">VM</span></span>

* <span data-ttu-id="aa5bc-793">Fehler behoben, aufgrund dessen `vmss create` bei der Ausführung mit `--no-wait` eine Fehlermeldung zurückgab</span><span class="sxs-lookup"><span data-stu-id="aa5bc-793">Fixed bug where `vmss create` returns an error message when run with `--no-wait`</span></span>
* <span data-ttu-id="aa5bc-794">Die clientseitige Validierung für `vmss create --single-placement-group` wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-794">Removed client-side validation for `vmss create --single-placement-group`.</span></span> <span data-ttu-id="aa5bc-795">Es tritt kein Fehler auf, wenn `--single-placement-group` auf `true` und für `--instance-count` ein größerer Wert als 100 festgelegt wird oder wenn Verfügbarkeitszonen angegeben werden. Diese Validierung wird jedoch dem Computedienst überlassen.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-795">Does not fail if `--single-placement-group` is set to `true` and`--instance-count` is greater than 100 or availability zones are specified, but leaves this validation to the compute service</span></span>
* <span data-ttu-id="aa5bc-796">Problem behoben, aufgrund dessen bei der Verwendung von `--latest` für `[vm|vmss] extension image list` ein Fehler auftrat</span><span class="sxs-lookup"><span data-stu-id="aa5bc-796">Fixed bug where `[vm|vmss] extension image list` fails when used with `--latest`</span></span>


## <a name="june-18-2019"></a><span data-ttu-id="aa5bc-797">18. Juni 2019</span><span class="sxs-lookup"><span data-stu-id="aa5bc-797">June 18, 2019</span></span>

<span data-ttu-id="aa5bc-798">Version 2.0.67</span><span class="sxs-lookup"><span data-stu-id="aa5bc-798">Version 2.0.67</span></span>

### <a name="core"></a><span data-ttu-id="aa5bc-799">Core</span><span class="sxs-lookup"><span data-stu-id="aa5bc-799">Core</span></span>

<span data-ttu-id="aa5bc-800">In diesem Release wird das neue [Preview]-Tag eingeführt, um Kunden gegenüber deutlich zu machen, dass sich eine Befehlsgruppe, ein Befehl oder ein Argument in der Vorschauphase befindet.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-800">This release introduces a new [Preview] tag to more clearly communicate to customers when a command group, command or argument is in preview status.</span></span> <span data-ttu-id="aa5bc-801">Diese Information war zuvor im Hilfetext oder implizit durch die Versionsnummer des Befehlsmoduls angegeben.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-801">This was previously called out in help text or communicated implicitly by the command module version number.</span></span>
<span data-ttu-id="aa5bc-802">Die Befehlszeilenschnittstelle wird künftig Versionsnummern für einzelne Pakete entfernen.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-802">The CLI will be removing version numbers for individual packages in the future.</span></span> <span data-ttu-id="aa5bc-803">Wenn sich ein Befehl in der Vorschauphase befindet, gilt dies auch für alle seine Argumente.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-803">If a command is in preview, all of its arguments are as well.</span></span> <span data-ttu-id="aa5bc-804">Wenn eine Befehlsgruppe als Vorschau gekennzeichnet ist, befinden sich auch alle Befehle und Argumente in der Vorschauphase.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-804">If a command group is labeled as being in preview, then all commands and arguments are considered to be in preview as well.</span></span>

<span data-ttu-id="aa5bc-805">Infolge dieser Änderung befinden sich in diesem Release verschiedene Befehlsgruppen anscheinend „plötzlich“ in der Vorschauphase.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-805">As a result of this change, several command groups may seem to "suddenly" appear to be in a preview status with this release.</span></span> <span data-ttu-id="aa5bc-806">Tatsächlich ist es jedoch so, dass sich die meisten Pakete in der Vorschauphase befanden, in diesem Release jedoch als allgemein verfügbar gelten.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-806">What actually happened is that most packages were in a preview status, but are being deemed GA with this release</span></span>

### <a name="acr"></a><span data-ttu-id="aa5bc-807">ACR</span><span class="sxs-lookup"><span data-stu-id="aa5bc-807">ACR</span></span>
* <span data-ttu-id="aa5bc-808">Befehl „acr check-health“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-808">Added 'acr check-health' command</span></span>
* <span data-ttu-id="aa5bc-809">Verbesserte Fehlerbehandlung für AAD-Token und für das Abrufen externer Befehle</span><span class="sxs-lookup"><span data-stu-id="aa5bc-809">Improved error handling for AAD tokens and for retrieving external commands</span></span>

### <a name="acs"></a><span data-ttu-id="aa5bc-810">ACS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-810">ACS</span></span>
* <span data-ttu-id="aa5bc-811">Veraltete ACS-Befehle werden jetzt in der Hilfeansicht ausgeblendet.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-811">Deprecated ACS commands are now hidden from help view</span></span>

### <a name="ams"></a><span data-ttu-id="aa5bc-812">AMS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-812">AMS</span></span>
* <span data-ttu-id="aa5bc-813">[BREAKING CHANGE] Änderung, damit ISO 8601-Zeitzeichenfolgen für „archive-window-length“ und „key-frame-interval-duration“ zurückgegeben werden</span><span class="sxs-lookup"><span data-stu-id="aa5bc-813">[BREAKING CHANGE] Changed to return ISO 8601 time strings for archive-window-length and key-frame-interval-duration</span></span>

### <a name="appservice"></a><span data-ttu-id="aa5bc-814">AppService</span><span class="sxs-lookup"><span data-stu-id="aa5bc-814">AppService</span></span>
* <span data-ttu-id="aa5bc-815">Standortbasiertes Routing für `webapp deleted list` und `webapp deleted restore` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-815">Added location based routing for `webapp deleted list` and `webapp deleted restore`</span></span>
* <span data-ttu-id="aa5bc-816">Problem behoben, aufgrund dessen in Azure Cloud Shell nicht auf die von einer Web-App protokollierte Ziel-URL („Sie können die App starten unter...“) geklickt werden konnte</span><span class="sxs-lookup"><span data-stu-id="aa5bc-816">Fixed issue where webapp up logged target URL ("You can launch the app at...") was not clickable in Azure Cloud Shell</span></span>
* <span data-ttu-id="aa5bc-817">Problem behoben, aufgrund dessen beim Erstellen von Apps bei einigen SKUs ein AlwaysOn-Fehler auftrat</span><span class="sxs-lookup"><span data-stu-id="aa5bc-817">Fixed an issue where creating apps with the some SKUs was failing with an AlwaysOn error</span></span>
* <span data-ttu-id="aa5bc-818">Vorabüberprüfung zu `[appservice|webapp] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-818">Added pre-validation to `[appservice|webapp] create`</span></span>
* <span data-ttu-id="aa5bc-819">`[webapp|functionapp] traffic-routing` korrigiert, damit der richtige actionHostName-Wert verwendet wird</span><span class="sxs-lookup"><span data-stu-id="aa5bc-819">Fixed `[webapp|functionapp] traffic-routing` to use the correct actionHostName</span></span>
* <span data-ttu-id="aa5bc-820">Slotunterstützung zu `functionapp`-Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-820">Added slot support to `functionapp` commands</span></span>

### <a name="batch"></a><span data-ttu-id="aa5bc-821">Batch</span><span class="sxs-lookup"><span data-stu-id="aa5bc-821">Batch</span></span>
* <span data-ttu-id="aa5bc-822">AAD-Authentifizierungsregression korrigiert, die von übermäßiger Berichterstellung für Authentifizierung mit gemeinsam verwendetem Schlüssel verursacht wurde</span><span class="sxs-lookup"><span data-stu-id="aa5bc-822">Fixed AAD auth regression caused by over-aggressive error reporting for Shared Key Auth</span></span>

### <a name="batchai"></a><span data-ttu-id="aa5bc-823">Batch AI</span><span class="sxs-lookup"><span data-stu-id="aa5bc-823">BatchAI</span></span>
* <span data-ttu-id="aa5bc-824">BatchAI-Befehle sind jetzt veraltet und ausgeblendet.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-824">BatchAI commands are now deprecated and hidden</span></span>

### <a name="botservice"></a><span data-ttu-id="aa5bc-825">BotService</span><span class="sxs-lookup"><span data-stu-id="aa5bc-825">BotService</span></span>
* <span data-ttu-id="aa5bc-826">Für Befehle, die Version 3 des SDK unterstützen, wurden die Warnmeldungen „Support eingestellt“/„Wartungsmodus“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-826">Added "discontinued support"/"maintenance mode" warning messages for commands that support the v3 SDK</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="aa5bc-827">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="aa5bc-827">CosmosDB</span></span>
* <span data-ttu-id="aa5bc-828">[VERALTET] Der Befehl `cosmosdb list-keys` wurde als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-828">[DEPRECATED] Deprecated the `cosmosdb list-keys` command</span></span>
* <span data-ttu-id="aa5bc-829">Befehl `cosmosdb keys list` hinzugefügt, er ersetzt `cosmosdb list-keys`.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-829">Added the `cosmosdb keys list` command - replaces `cosmosdb list-keys`</span></span>
* <span data-ttu-id="aa5bc-830">`cosmsodb create/update`: Neues Format für „--location“ hinzugefügt, um das Festlegen der Eigenschaft „isZoneRedundant“ zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-830">`cosmsodb create/update`: Added new format for --location to allow setting "isZoneRedundant" property.</span></span> <span data-ttu-id="aa5bc-831">Das alte Format wurde als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-831">Deprecated old format</span></span>

### <a name="eventgrid"></a><span data-ttu-id="aa5bc-832">EventGrid</span><span class="sxs-lookup"><span data-stu-id="aa5bc-832">EventGrid</span></span>
* <span data-ttu-id="aa5bc-833">`eventgrid domain`-Befehle für CRUD-Vorgänge für Domänen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-833">Added `eventgrid domain` commands for domain CRUD operations</span></span>
* <span data-ttu-id="aa5bc-834">`eventgrid domain topic`-Befehle für CRUD-Vorgänge für Domänenthemen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-834">Added `eventgrid domain topic` commands for domain topics CRUD operations</span></span>
* <span data-ttu-id="aa5bc-835">Argument `--odata-query` zu `eventgrid [topic|event-subscription] list` zum Filtern der Ergebnisse mithilfe von OData-Syntax hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-835">Added `--odata-query` argument to `eventgrid [topic|event-subscription] list` for filtering results using OData syntax</span></span>
* <span data-ttu-id="aa5bc-836">`event-subscription create/update`: „servicebusqueue“ als neue Werte für den Parameter `--endpoint-type` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-836">`event-subscription create/update`: Added servicebusqueue as new values for the `--endpoint-type` parameter</span></span>
* <span data-ttu-id="aa5bc-837">[BREAKING CHANGE] Unterstützung für `--included-event-types All` mit `eventgrid event-subscription [create|update]` entfernt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-837">[BREAKING CHANGE] Removed support for `--included-event-types All` with `eventgrid event-subscription [create|update]`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="aa5bc-838">HDInsight</span><span class="sxs-lookup"><span data-stu-id="aa5bc-838">HDInsight</span></span>
* <span data-ttu-id="aa5bc-839">Unterstützung für den Parameter `--ssh-public-key` im Befehl vom Typ `hdinsight create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-839">Added support for `--ssh-public-key` parameter in `hdinsight create` command</span></span>

### <a name="iot"></a><span data-ttu-id="aa5bc-840">IoT</span><span class="sxs-lookup"><span data-stu-id="aa5bc-840">IoT</span></span>
* <span data-ttu-id="aa5bc-841">Unterstützung für das erneute Generieren von Autorisierungsrichtlinienschlüsseln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-841">Added support to regenerate authorization policy keys</span></span>
* <span data-ttu-id="aa5bc-842">SDK und Unterstützung für den Bereitstellungsdienst des DigitalTwin-Repositorys hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-842">Added SDK and support for DigitalTwin Repository Provisioning Service</span></span>

### <a name="network"></a><span data-ttu-id="aa5bc-843">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="aa5bc-843">Network</span></span>
* <span data-ttu-id="aa5bc-844">Zonenunterstützung für NAT Gateway hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-844">Added Zone support for Nat Gateway</span></span>
* <span data-ttu-id="aa5bc-845">Befehl `network list-service-tags` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-845">Added command `network list-service-tags`</span></span>
* <span data-ttu-id="aa5bc-846">Problem mit `dns zone import` behoben, aufgrund dessen Benutzer keine A-Platzhaltereinträge importieren konnten</span><span class="sxs-lookup"><span data-stu-id="aa5bc-846">Fixed issue with `dns zone import` where users could not import wildcard A records</span></span>
* <span data-ttu-id="aa5bc-847">Problem mit `watcher flow-log configure` behoben, aufgrund dessen die Flowprotokollierung in bestimmten Regionen nicht aktiviert werden konnte</span><span class="sxs-lookup"><span data-stu-id="aa5bc-847">Fixed issue with `watcher flow-log configure` where flow logging could not be enabled in certain regions</span></span>

### <a name="resource"></a><span data-ttu-id="aa5bc-848">Resource</span><span class="sxs-lookup"><span data-stu-id="aa5bc-848">Resource</span></span>
* <span data-ttu-id="aa5bc-849">Befehl `az rest` zum Ausführen von REST-Aufrufen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-849">Added `az rest` command for making REST calls</span></span>
* <span data-ttu-id="aa5bc-850">Fehler behoben, der bei Verwendung von `policy assignment list` mit `--scope` auf Ressourcengruppen- oder Abonnementebene auftrat</span><span class="sxs-lookup"><span data-stu-id="aa5bc-850">Fixed error when using `policy assignment list` with a resource group or subscription level `--scope`</span></span>

### <a name="servicebus"></a><span data-ttu-id="aa5bc-851">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="aa5bc-851">ServiceBus</span></span>
* <span data-ttu-id="aa5bc-852">Problem mit `servicebus topic create --max-size` behoben [Nr. 9319](https://github.com/azure/azure-cli/issues/9319)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-852">Fixed issue with `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span></span>

### <a name="sql"></a><span data-ttu-id="aa5bc-853">SQL</span><span class="sxs-lookup"><span data-stu-id="aa5bc-853">SQL</span></span>
* <span data-ttu-id="aa5bc-854">`--location` wurde geändert und ist nun für `sql [server|mi] create` optional. Ohne Angabe wird der Ressourcengruppenstandort verwendet.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-854">Changed `--location` to be optional for `sql [server|mi] create` - uses resource group location if not specified</span></span>
* <span data-ttu-id="aa5bc-855">Der Fehler, dass das Objekt „NoneType“ nicht wiederholbar ist, wurde für `sql db list-editions --available` behoben.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-855">Fixed "'NoneType' object is not iterable" error for `sql db list-editions --available`</span></span>

### <a name="sqlvm"></a><span data-ttu-id="aa5bc-856">SQLVm</span><span class="sxs-lookup"><span data-stu-id="aa5bc-856">SQLVm</span></span>
* <span data-ttu-id="aa5bc-857">[WICHTIGE ÄNDERUNG] `sql vm create` wurde geändert und erfordert nun den Parameter `--license-type`.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-857">[BREAKING CHNAGE] Changed `sql vm create` to require `--license-type` parameter</span></span>
* <span data-ttu-id="aa5bc-858">Änderung, um beim Erstellen oder Aktualisieren einer SQL-VM das Festlegen der SQL-Image-SKU zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-858">Changed to allow setting SQL image SKU when creating or updating a sql vm</span></span>

### <a name="storage"></a><span data-ttu-id="aa5bc-859">Storage</span><span class="sxs-lookup"><span data-stu-id="aa5bc-859">Storage</span></span>
* <span data-ttu-id="aa5bc-860">Problem mit fehlendem Kontoschlüssel für `storage container generate-sas` behoben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-860">Fixed issue with missing account key for `storage container generate-sas`</span></span>
* <span data-ttu-id="aa5bc-861">Problem mit `storage blob sync` unter Linux behoben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-861">Fixed issue with `storage blob sync` on Linux</span></span>

### <a name="vm"></a><span data-ttu-id="aa5bc-862">VM</span><span class="sxs-lookup"><span data-stu-id="aa5bc-862">VM</span></span>
* <span data-ttu-id="aa5bc-863">[VORSCHAU] Befehle vom Typ `vm image template` zum Erstellen von VM-Images hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-863">[PREVIEW] Added `vm image template` commands to build VM images</span></span>

## <a name="june-4-2019"></a><span data-ttu-id="aa5bc-864">4\. Juni 2019</span><span class="sxs-lookup"><span data-stu-id="aa5bc-864">June 4, 2019</span></span>

<span data-ttu-id="aa5bc-865">Version 2.0.66</span><span class="sxs-lookup"><span data-stu-id="aa5bc-865">Version 2.0.66</span></span>

### <a name="core"></a><span data-ttu-id="aa5bc-866">Core</span><span class="sxs-lookup"><span data-stu-id="aa5bc-866">Core</span></span>
* <span data-ttu-id="aa5bc-867">Fehler behoben, aufgrund dessen bei Befehlen ein Fehler auftrat, wenn `--output yaml` mit `--query` verwendet wurde</span><span class="sxs-lookup"><span data-stu-id="aa5bc-867">Fixed bug where commands fail if `--output yaml` is used with `--query`</span></span>

### <a name="acr"></a><span data-ttu-id="aa5bc-868">ACR</span><span class="sxs-lookup"><span data-stu-id="aa5bc-868">ACR</span></span>
* <span data-ttu-id="aa5bc-869">Befehlsgruppe „acr pack“ zum Erstellen von Aufgaben zur Schnellerstellung mit Buildpacks hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-869">Added 'acr pack' command group for creating quick build Tasks using Buildpacks.</span></span>

### <a name="acs"></a><span data-ttu-id="aa5bc-870">ACS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-870">ACS</span></span>
* <span data-ttu-id="aa5bc-871">Zulassen der Aktivierung/Deaktivierung des AKS-Add-Ons für das Kube-Dashboard</span><span class="sxs-lookup"><span data-stu-id="aa5bc-871">Allow enabling/disabling AKS kube-dashboard addon</span></span>
* <span data-ttu-id="aa5bc-872">Ausgeben einer benutzerfreundlichen Nachricht, wenn das Abonnement nicht in der Whitelist zur Verwendung von Azure Red Hat OpenShift enthalten ist</span><span class="sxs-lookup"><span data-stu-id="aa5bc-872">Print a friendly message when the subscription is not whitelisted to use Azure Red Hat OpenShift</span></span>

### <a name="batch"></a><span data-ttu-id="aa5bc-873">Batch</span><span class="sxs-lookup"><span data-stu-id="aa5bc-873">Batch</span></span>
* <span data-ttu-id="aa5bc-874">Bessere Fehlerbehandlung, wenn der Benutzer nicht bei einem Konto angemeldet ist \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span><span class="sxs-lookup"><span data-stu-id="aa5bc-874">Improved error handling when not logged in to an account \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span></span>

### <a name="iot"></a><span data-ttu-id="aa5bc-875">IoT</span><span class="sxs-lookup"><span data-stu-id="aa5bc-875">IoT</span></span>
* <span data-ttu-id="aa5bc-876">Unterstützung für manuelles Failover hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-876">Added support for manual failover</span></span>

### <a name="network"></a><span data-ttu-id="aa5bc-877">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="aa5bc-877">Network</span></span>
* <span data-ttu-id="aa5bc-878">Befehle vom Typ `network application-gateway waf-policy` hinzugefügt, um benutzerdefinierte WAF-Regeln zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-878">Added `network application-gateway waf-policy` commands to support custom WAF rules.</span></span>
* <span data-ttu-id="aa5bc-879">Argumente `--waf-policy` und `--max-capacity` zu `network application-gateway [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-879">Added `--waf-policy` and `--max-capacity` arguments to `network application-gateway [create|update]`</span></span> 

### <a name="resource"></a><span data-ttu-id="aa5bc-880">Resource</span><span class="sxs-lookup"><span data-stu-id="aa5bc-880">Resource</span></span>
* <span data-ttu-id="aa5bc-881">Verbesserte Fehlermeldungen aus `deployment create`, wenn TTY nicht verfügbar ist</span><span class="sxs-lookup"><span data-stu-id="aa5bc-881">Improved error message from `deployment create` when there is no TTY available</span></span>

### <a name="role"></a><span data-ttu-id="aa5bc-882">Role</span><span class="sxs-lookup"><span data-stu-id="aa5bc-882">Role</span></span>
* <span data-ttu-id="aa5bc-883">Hilfetext aktualisiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-883">Updated help text.</span></span>

### <a name="compute"></a><span data-ttu-id="aa5bc-884">Compute</span><span class="sxs-lookup"><span data-stu-id="aa5bc-884">Compute</span></span>
* <span data-ttu-id="aa5bc-885">Unterstützung zu `vm create` für virtuelle Computer aus einem verwalteten Image mit Datenträger-LUNs hinzugefügt, die nicht bei 0 beginnen oder die Nummern überspringen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-885">Added support to `vm create` for VMs from a managed image with data-disk luns that do not start from 0 or that skip numbers</span></span>

## <a name="may-21-2019"></a><span data-ttu-id="aa5bc-886">21. Mai 2019</span><span class="sxs-lookup"><span data-stu-id="aa5bc-886">May 21, 2019</span></span>

<span data-ttu-id="aa5bc-887">Version 2.0.65</span><span class="sxs-lookup"><span data-stu-id="aa5bc-887">Version 2.0.65</span></span>

### <a name="core"></a><span data-ttu-id="aa5bc-888">Core</span><span class="sxs-lookup"><span data-stu-id="aa5bc-888">Core</span></span>
* <span data-ttu-id="aa5bc-889">Besseres Feedback für Authentifizierungsfehler hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-889">Added better feedback for authentication errors</span></span>
* <span data-ttu-id="aa5bc-890">Problem behoben, aufgrund dessen die CLI Erweiterungen lädt, die nicht mit der Core-Version kompatibel waren</span><span class="sxs-lookup"><span data-stu-id="aa5bc-890">Fixed issue where the CLI would load extensions that were not compatible with its core version</span></span>
* <span data-ttu-id="aa5bc-891">Problem beim Starten behoben, wenn `clouds.config` beschädigt ist</span><span class="sxs-lookup"><span data-stu-id="aa5bc-891">Fixed issue with launching when `clouds.config` is corrupted</span></span>

### <a name="acr"></a><span data-ttu-id="aa5bc-892">ACR</span><span class="sxs-lookup"><span data-stu-id="aa5bc-892">ACR</span></span>
* <span data-ttu-id="aa5bc-893">Unterstützung für verwaltete Identitäten zu Aufgaben hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-893">Added support for Managed Identities to Tasks</span></span>

### <a name="acs"></a><span data-ttu-id="aa5bc-894">ACS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-894">ACS</span></span>
* <span data-ttu-id="aa5bc-895">`openshift create`-Befehl bei der Verwendung mit dem AAD-Kundenclient korrigiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-895">Fixed `openshift create` command when used with customer AAD client</span></span>

### <a name="appservice"></a><span data-ttu-id="aa5bc-896">AppService</span><span class="sxs-lookup"><span data-stu-id="aa5bc-896">AppService</span></span>
* <span data-ttu-id="aa5bc-897">[VERALTET] Befehl `functionapp devops-build` als veraltet gekennzeichnet – wird in der nächsten Version entfernt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-897">[DEPRECATED] Deprecated `functionapp devops-build` command - will be removed in next release</span></span>
* <span data-ttu-id="aa5bc-898">`functionapp devops-pipeline` geändert, um das Buildprotokoll von Azure DevOps im ausführlichen Modus abzurufen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-898">Changed `functionapp devops-pipeline` to fetch build log from Azure DevOps in verbose mode</span></span>
* <span data-ttu-id="aa5bc-899">[BREAKING CHANGE] Flag `--use_local_settings` aus dem Befehl `functionapp devops-pipeline` entfernt – kein Vorgang wurde ausgeführt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-899">[BREAKING CHANGE] Removed `--use_local_settings` flag from `functionapp devops-pipeline` command - was a no-op</span></span>
* <span data-ttu-id="aa5bc-900">`webapp up` geändert, sodass die JSON-Ausgabe zurückgegeben wird, wenn `--logs` nicht verwendet wird</span><span class="sxs-lookup"><span data-stu-id="aa5bc-900">Changed `webapp up` to return JSON output if `--logs` is not used</span></span>
* <span data-ttu-id="aa5bc-901">Unterstützung hinzugefügt zum Schreiben von Standardressourcen in die lokale Konfiguration für `webapp up`</span><span class="sxs-lookup"><span data-stu-id="aa5bc-901">Added support for writing default resources to local config for `webapp up`</span></span>
* <span data-ttu-id="aa5bc-902">Unterstützung zu `webapp up` hinzugefügt für die erneute Bereitstellung einer App ohne Verwendung des `--location`-Arguments</span><span class="sxs-lookup"><span data-stu-id="aa5bc-902">Added support to `webapp up` for redeploying an app without using the `--location` argument</span></span>
* <span data-ttu-id="aa5bc-903">Problem behoben, bei dem für die ASP-Erstellung der Linux-SKU „Free“ der SKU-Wert „Free“ nicht funktioniert hat</span><span class="sxs-lookup"><span data-stu-id="aa5bc-903">Fixed an issue where for Linux Free SKU ASP creation use Free as SKU value was not working</span></span>

### <a name="botservice"></a><span data-ttu-id="aa5bc-904">BotService</span><span class="sxs-lookup"><span data-stu-id="aa5bc-904">BotService</span></span>
* <span data-ttu-id="aa5bc-905">Geändert, sodass Groß-/Kleinschreibung für `--lang`-Parameter für Befehle zulässig ist</span><span class="sxs-lookup"><span data-stu-id="aa5bc-905">Changed to allow all casing for `--lang` parameters for commands</span></span>
* <span data-ttu-id="aa5bc-906">Beschreibung für das Befehlsmodul aktualisiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-906">Updated description for command module</span></span>

### <a name="consumption"></a><span data-ttu-id="aa5bc-907">Nutzung</span><span class="sxs-lookup"><span data-stu-id="aa5bc-907">Consumption</span></span>
* <span data-ttu-id="aa5bc-908">Fehlende erforderliche Parameter bei der Ausführung von `consumption usage list --billing-period-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-908">Added missing required parameter when running `consumption usage list --billing-period-name`</span></span>

### <a name="iot"></a><span data-ttu-id="aa5bc-909">IoT</span><span class="sxs-lookup"><span data-stu-id="aa5bc-909">IoT</span></span>
* <span data-ttu-id="aa5bc-910">Unterstützung für das Auflisten aller Schlüssel hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-910">Added support to list all keys</span></span>

### <a name="network"></a><span data-ttu-id="aa5bc-911">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="aa5bc-911">Network</span></span>
* [BREAKING CHANGE]: Removed `network interface-endpoints` command group - use `network private-endpoints` 
* <span data-ttu-id="aa5bc-913">`--nat-gateway`-Argument zu `network vnet subnet [create|update]` für das Anfügen an ein NAT-Gateway hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-913">Added `--nat-gateway` argument to `network vnet subnet [create|update]` for attaching to a NAT gateway</span></span>
* <span data-ttu-id="aa5bc-914">Problem mit `dns zone import` behoben, aufgrund dessen Eintragsnamen keinem Datensatztyp entsprochen haben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-914">Fixed issue with `dns zone import` where record names could not match a record type</span></span>

### <a name="rdbms"></a><span data-ttu-id="aa5bc-915">RDBMS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-915">RDBMS</span></span>
* <span data-ttu-id="aa5bc-916">Postgres- und MySLQ-Unterstützung für die Georeplikation hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-916">Added postgres and mysql support for geo replication</span></span>

### <a name="rbac"></a><span data-ttu-id="aa5bc-917">RBAC</span><span class="sxs-lookup"><span data-stu-id="aa5bc-917">RBAC</span></span>
* <span data-ttu-id="aa5bc-918">Unterstützung für den Verwaltungsgruppenumfang zu `role assignment` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-918">Added support for management group scope to `role assignment`</span></span>

### <a name="storage"></a><span data-ttu-id="aa5bc-919">Storage</span><span class="sxs-lookup"><span data-stu-id="aa5bc-919">Storage</span></span>
* <span data-ttu-id="aa5bc-920">`storage blob sync`: Synchronisierungsbefehl für Speicherblob hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-920">`storage blob sync`: add sync command for storage blob</span></span>

### <a name="compute"></a><span data-ttu-id="aa5bc-921">Compute</span><span class="sxs-lookup"><span data-stu-id="aa5bc-921">Compute</span></span>
* <span data-ttu-id="aa5bc-922">`--computer-name` zu `vm create` zum Festlegen des Computernamens eines virtuellen Computers hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-922">Added `--computer-name` to `vm create` for setting a VM's computer name</span></span>
* <span data-ttu-id="aa5bc-923">`--ssh-key-value` umbenannt in `--ssh-key-values` für `[vm|vmss] create`: Jetzt können mehrere öffentliche SSH-Schlüsselwerte oder -pfade akzeptiert werden.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-923">Renamed `--ssh-key-value` renamed to `--ssh-key-values` for `[vm|vmss] create` - can now accept multiple ssh public key values or paths</span></span>
  * <span data-ttu-id="aa5bc-924">__Hinweis__: Dies ist **kein** Breaking Change: `--ssh-key-value` wird korrekt analysiert, da nur eine Übereinstimmung mit `--ssh-key-values` besteht.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-924">__Note__: This is **not** a breaking change - `--ssh-key-value` will be parsed correctly as it matches only `--ssh-key-values`</span></span>
* <span data-ttu-id="aa5bc-925">`--type`-Argument von `ppg create` in optionales Argument geändert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-925">Changed the `--type` argument of `ppg create` to be optional</span></span>

## <a name="may-6-2019"></a><span data-ttu-id="aa5bc-926">6\. Mai 2019</span><span class="sxs-lookup"><span data-stu-id="aa5bc-926">May 6, 2019</span></span>

<span data-ttu-id="aa5bc-927">Version 2.0.64</span><span class="sxs-lookup"><span data-stu-id="aa5bc-927">Version 2.0.64</span></span>

### <a name="acs"></a><span data-ttu-id="aa5bc-928">ACS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-928">ACS</span></span>
* <span data-ttu-id="aa5bc-929">[BREAKING CHANGE] Flag `--fqdn` aus den `openshift`-Befehlen entfernt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-929">[BREAKING CHANGE] Removed `--fqdn` flag on `openshift` commands</span></span>
* <span data-ttu-id="aa5bc-930">Geändert, sodass die allgemein verfügbare Azure Red Hat Openshift-API-Version verwendet wird</span><span class="sxs-lookup"><span data-stu-id="aa5bc-930">Changed to use Azure Red Hat Openshift GA API Version</span></span>
* <span data-ttu-id="aa5bc-931">Flag `customer-admin-group-id` wurde zu `openshift create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-931">Added `customer-admin-group-id` flag to `openshift create`</span></span>
* <span data-ttu-id="aa5bc-932">[ALLGEMEIN VERFÜGBAR] `(PREVIEW)` aus der `aks create`-Option `--network-policy` entfernt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-932">[GA] Removed `(PREVIEW)` from `aks create` option `--network-policy`</span></span>

### <a name="appservice"></a><span data-ttu-id="aa5bc-933">AppService</span><span class="sxs-lookup"><span data-stu-id="aa5bc-933">Appservice</span></span>
* <span data-ttu-id="aa5bc-934">[VERALTET] Befehl `functionapp devops-build` als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="aa5bc-934">[DEPRECATED] Deprecated `functionapp devops-build` command</span></span>
  * <span data-ttu-id="aa5bc-935">Umbenannt in `functionapp devops-pipeline`</span><span class="sxs-lookup"><span data-stu-id="aa5bc-935">Renamed to `functionapp devops-pipeline`</span></span>
* <span data-ttu-id="aa5bc-936">Fehler beim Abrufen des richtigen Benutzernamens für Cloud Shell behoben, der einen Fehler von `webapp up` verursachte</span><span class="sxs-lookup"><span data-stu-id="aa5bc-936">Fixed getting the correct username for cloudshell which was causing `webapp up` to fail</span></span>
* <span data-ttu-id="aa5bc-937">Dokumentation von `appservice plan --sku` mit den unterstützten App Service-Plänen aktualisiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-937">Updated `appservice plan --sku` documentation updated to reflect the supported appserviceplans</span></span>
* <span data-ttu-id="aa5bc-938">Optionale Argumente für Ressourcengruppe und Plan zu `webapp up` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-938">Added optional arguments for resource group and plan to `webapp up`</span></span>
* <span data-ttu-id="aa5bc-939">Unterstützung zur Berücksichtigung der Umgebungsvariablen `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` zu `webapp ssh` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-939">Added support to `webapp ssh` to respect `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>
* <span data-ttu-id="aa5bc-940">Unterstützung für `appserviceplan create` für die kostenlose Linux-SKU hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-940">Added `appserviceplan create` support for Linux Free SKU</span></span>
* <span data-ttu-id="aa5bc-941">`webapp up` geändert, um nach dem Festlegen der App-Einstellung `SCM_DO_BUILD_DURING_DEPLOYMENT=true` zum Verarbeiten des Kudu-Kaltstarts für 30 Sekunden in den Energiesparmodus zu wechseln</span><span class="sxs-lookup"><span data-stu-id="aa5bc-941">Changed `webapp up` to have a 30s sleep after setting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` appsetting to handle kudu cold start</span></span>
* <span data-ttu-id="aa5bc-942">Unterstützung für die `powershell`-Runtime zu `functionapp create` unter Windows hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-942">Added support for `powershell` runtime to `functionapp create` on Windows</span></span>
* <span data-ttu-id="aa5bc-943">Befehl `create-remote-connection` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-943">Added `create-remote-connection` command</span></span>

### <a name="batch"></a><span data-ttu-id="aa5bc-944">Batch</span><span class="sxs-lookup"><span data-stu-id="aa5bc-944">Batch</span></span>
* <span data-ttu-id="aa5bc-945">Fehler im Validierungssteuerelement für `--application-package-references`-Optionen korrigiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-945">Fixed bug in validator for `--application-package-references` options</span></span>

### <a name="botservice"></a><span data-ttu-id="aa5bc-946">Botservice</span><span class="sxs-lookup"><span data-stu-id="aa5bc-946">Botservice</span></span>
* <span data-ttu-id="aa5bc-947">[BREAKING CHANGE]`bot create -v v4 -k webapp` geändert, sodass standardmäßig eine leerer Web-App-Bot erstellt wird (d. h. kein Bot wird in App Service bereitgestellt)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-947">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to create an empty Web App Bot by default (i.e. no bot is deployed to the App Service)</span></span>
* <span data-ttu-id="aa5bc-948">`--echo`-Flag zu `bot create` hinzugefügt, sodass das alte Verhalten mit `-v v4` verwendet wird</span><span class="sxs-lookup"><span data-stu-id="aa5bc-948">Added `--echo` flag to `bot create` to use the old behavior with `-v v4`</span></span>
* <span data-ttu-id="aa5bc-949">[BREAKING CHANGE] Standardwert von `--version` in `v4` geändert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-949">[BREAKING CHANGE] Changed the default value of  `--version` to `v4`</span></span>
  * <span data-ttu-id="aa5bc-950">__HINWEIS:__ `bot prepare-publish` verwendet weiterhin den alten Standard.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-950">__NOTE:__ `bot prepare-publish` still uses the its old default</span></span>
* <span data-ttu-id="aa5bc-951">[BREAKING CHANGE]`--lang` geändert, sodass der Standard nicht mehr `Csharp` ist.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-951">[BREAKING CHANGE] Changed `--lang` to no longer default to `Csharp`.</span></span> <span data-ttu-id="aa5bc-952">Wenn der Befehl `--lang` erfordert und dies nicht angegeben ist, wird der Befehl nun mit Fehler beendet.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-952">If the command requires `--lang` and it is not provided, the command will now error out</span></span>
* <span data-ttu-id="aa5bc-953">[BREAKING CHANGE]`--appid`- und `--password`-Argumente für `bot create` in erforderlich geändert, sie können jetzt über `ad app create` erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-953">[BREAKING CHANGE] Changed the `--appid` and `--password` args for `bot create` to be required and can now be created via `ad app create`</span></span>
* <span data-ttu-id="aa5bc-954">`--appid`- und `--password`-Validierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-954">Added `--appid` and `--password` validation</span></span>
* <span data-ttu-id="aa5bc-955">[BREAKING CHANGE]`bot create -v v4` geändert, sodass kein Speicherkonto bzw. keine Application Insights-Instanz erstellt oder verwendet wird</span><span class="sxs-lookup"><span data-stu-id="aa5bc-955">[BREAKING CHANGE] Changed `bot create -v v4` to not create or use a Storage Account or Application Insights</span></span>
* <span data-ttu-id="aa5bc-956">[BREAKING CHANGE]`bot create -v v3` geändert, sodass eine Region erforderlich ist, in der Application Insights verfügbar ist</span><span class="sxs-lookup"><span data-stu-id="aa5bc-956">[BREAKING CHANGE] Changed `bot create -v v3` to require a region where Application Insights is available</span></span>
* <span data-ttu-id="aa5bc-957">[BREAKING CHANGE]`bot update` geändert, sodass es sich jetzt nur auf spezifische Eigenschaften eines Bots auswirkt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-957">[BREAKING CHANGE] Changed `bot update` to now affect only specific properties of a bot</span></span>
* <span data-ttu-id="aa5bc-958">[BREAKING CHANGE]`--lang`-Flags geändert, sodass `Javascript` anstelle von `Node` akzeptiert wird</span><span class="sxs-lookup"><span data-stu-id="aa5bc-958">[BREAKING CHANGE] Changed `--lang` flags to accept `Javascript` instead of `Node`</span></span>
* <span data-ttu-id="aa5bc-959">[BREAKING CHANGE]`Node` als zulässiger `--lang`-Wert entfernt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-959">[BREAKING CHANGE] Removed `Node` as an allowed `--lang` value</span></span>
* <span data-ttu-id="aa5bc-960">[BREAKING CHANGE]`bot create -v v4 -k webapp` geändert, sodass `SCM_DO_BUILD_DURING_DEPLOYMENT` nicht mehr auf TRUE festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-960">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to no longer set `SCM_DO_BUILD_DURING_DEPLOYMENT` to true.</span></span> <span data-ttu-id="aa5bc-961">Alle Bereitstellungen über Kudu fungieren ihrem Standardverhalten entsprechend.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-961">All deployments through Kudu will act according to their default behavior</span></span>
* <span data-ttu-id="aa5bc-962">`bot download` für Bots ohne `.bot`-Dateien geändert, sodass die sprachspezifische Konfigurationsdatei mit Werten aus den Anwendungseinstellungen für den Bot erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-962">Changed `bot download` for bots without `.bot` files to create the language-specific configuration file with values from the Application Settings for the bot</span></span>
* <span data-ttu-id="aa5bc-963">Unterstützung für `Typescript` zu `bot prepare-deploy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-963">Added `Typescript` support to `bot prepare-deploy`</span></span>
* <span data-ttu-id="aa5bc-964">Warnmeldung zu `bot prepare-deploy` für `Javascript`- und `Typescript`-Bots hinzugefügt, wenn `package.json` in `--code-dir` nicht enthalten ist</span><span class="sxs-lookup"><span data-stu-id="aa5bc-964">Added warning message to `bot prepare-deploy` for `Javascript` and `Typescript` bots for when `--code-dir` does not contain `package.json`</span></span>
* <span data-ttu-id="aa5bc-965">`bot prepare-deploy` geändert, sodass bei Erfolg `true` zurückgegeben wird</span><span class="sxs-lookup"><span data-stu-id="aa5bc-965">Changed `bot prepare-deploy` to return `true` if successful</span></span>
* <span data-ttu-id="aa5bc-966">Ausführliche Protokollierung zu `bot prepare-deploy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-966">Added verbose logging to `bot prepare-deploy`</span></span>
* <span data-ttu-id="aa5bc-967">Mehr verfügbare Application Insights-Regionen zu `az bot create -v v3` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-967">Added more available Application Insights regions to `az bot create -v v3`</span></span>

### <a name="configure"></a><span data-ttu-id="aa5bc-968">Konfigurieren</span><span class="sxs-lookup"><span data-stu-id="aa5bc-968">Configure</span></span>
* <span data-ttu-id="aa5bc-969">Unterstützung für die ordnerbasierte Argument-Standardwertkonfigurationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-969">Added support for folder based argument default value configurations</span></span>

### <a name="eventhubs"></a><span data-ttu-id="aa5bc-970">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="aa5bc-970">Eventhubs</span></span>
* <span data-ttu-id="aa5bc-971">Befehle vom Typ `namespace network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-971">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="aa5bc-972">`--default-action`-Argument für Netzwerkregeln zu `namespace [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-972">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="aa5bc-973">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="aa5bc-973">Network</span></span>
* <span data-ttu-id="aa5bc-974">[BREAKING CHANGE]`--cache`-Argument mit `--defer` für `vnet [create|update]` ersetzt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-974">[BREAKING CHANGE] Replaced `--cache` arugment with `--defer` for `vnet [create|update]`</span></span> 

### <a name="policy-insights"></a><span data-ttu-id="aa5bc-975">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="aa5bc-975">Policy Insights</span></span>
* <span data-ttu-id="aa5bc-976">Unterstützung für `--expand PolicyEvaluationDetails` hinzugefügt, sodass Richtlinienauswertungsdetails von der Ressource abgefragt werden</span><span class="sxs-lookup"><span data-stu-id="aa5bc-976">Added support for `--expand PolicyEvaluationDetails` to query policy evaluation details on the resource</span></span>

### <a name="role"></a><span data-ttu-id="aa5bc-977">Role</span><span class="sxs-lookup"><span data-stu-id="aa5bc-977">Role</span></span>
* <span data-ttu-id="aa5bc-978">[VERALTET]: Ausblenden des „--password"-Arguments von `create-for-rbac` geändert; Unterstützung wird im Mai 2019 entfernt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-978">[DEPRECATED] Changed `create-for-rbac` hide '--password' argument - support will be removed in May 2019</span></span>

### <a name="service-bus"></a><span data-ttu-id="aa5bc-979">Service Bus</span><span class="sxs-lookup"><span data-stu-id="aa5bc-979">Service Bus</span></span>
* <span data-ttu-id="aa5bc-980">Befehle vom Typ `namespace network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-980">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="aa5bc-981">`--default-action`-Argument für Netzwerkregeln zu `namespace [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-981">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>
* <span data-ttu-id="aa5bc-982">`topic [create|update]` korrigiert, sodass `--max-size`-Unterstützung für 10-, 20-, 40- und 80-GB-Werte mit Premium-SKU zulässig ist</span><span class="sxs-lookup"><span data-stu-id="aa5bc-982">Fixed `topic [create|update]` to allow `--max-size` support for 10, 20, 40 and 80GB values with premium SKU</span></span>

### <a name="sql"></a><span data-ttu-id="aa5bc-983">SQL</span><span class="sxs-lookup"><span data-stu-id="aa5bc-983">SQL</span></span>
* <span data-ttu-id="aa5bc-984">Befehle vom Typ `sql virtual-cluster [list|show|delete]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-984">Added `sql virtual-cluster [list|show|delete]` commands</span></span>

### <a name="vm"></a><span data-ttu-id="aa5bc-985">VM</span><span class="sxs-lookup"><span data-stu-id="aa5bc-985">VM</span></span>
* <span data-ttu-id="aa5bc-986">`--protect-from-scale-in` und `--protect-from-scale-set-actions` zu `vmss update` hinzugefügt, sodass Aktualisierungen der Schutzrichtlinie von VMSS-VM-Instanzen aktiviert sind</span><span class="sxs-lookup"><span data-stu-id="aa5bc-986">Added `--protect-from-scale-in` and `--protect-from-scale-set-actions` to `vmss update` to enable updates to the protection policy of VMSS VM instances</span></span>
* <span data-ttu-id="aa5bc-987">`--instance-id` zu `vmss update` hinzugefügt, sodass allgemeine Aktualisierungen von VMSS-VM-Instanzen aktiviert sind</span><span class="sxs-lookup"><span data-stu-id="aa5bc-987">Added `--instance-id` to `vmss update` to enable generic update of VMSS VM instances</span></span>
* <span data-ttu-id="aa5bc-988">`--instance-id` zu `vmss wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-988">Added `--instance-id` to `vmss wait`</span></span>
* <span data-ttu-id="aa5bc-989">Neue `ppg`-Befehlsgruppe für die Verwaltung von Näherungsplatzierungsgruppen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-989">Added new `ppg` command group for managing Proximity Placement Groups</span></span>
* <span data-ttu-id="aa5bc-990">`--ppg` zu `[vm|vmss] create` und `vm availability-set create` für die Verwaltung von PPGs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-990">Added `--ppg` to `[vm|vmss] create` and `vm availability-set create` for managing PPGs</span></span>
* <span data-ttu-id="aa5bc-991">Parameter `--hyper-v-generation` zu `image create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-991">Added `--hyper-v-generation` parameter to `image create`</span></span>

## <a name="april-23-2019"></a><span data-ttu-id="aa5bc-992">23. April 2019</span><span class="sxs-lookup"><span data-stu-id="aa5bc-992">April 23, 2019</span></span>

<span data-ttu-id="aa5bc-993">Version 2.0.63</span><span class="sxs-lookup"><span data-stu-id="aa5bc-993">Version 2.0.63</span></span>

### <a name="acs"></a><span data-ttu-id="aa5bc-994">ACS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-994">ACS</span></span>
* <span data-ttu-id="aa5bc-995">`aks get-credentials` zur Anzeige einer Eingabeaufforderung zum Überschreiben doppelter Werte geändert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-995">Changed `aks get-credentials` to prompt to overwrite duplicated values</span></span>
* <span data-ttu-id="aa5bc-996">`(PREVIEW)` aus Dev Spaces-Befehlen „aks use-dev-spaces“ und „aks remove-dev-spaces“ entfernt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-996">Removed `(PREVIEW)` from Dev Spaces commands "aks use-dev-spaces" and "aks remove-dev-spaces"</span></span>

### <a name="ams"></a><span data-ttu-id="aa5bc-997">AMS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-997">AMS</span></span>
* <span data-ttu-id="aa5bc-998">Fehler bei der Objekt- und Kontofilteraktualisierung behoben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-998">Fixed bug with asset and account filters update</span></span>

### <a name="appservice"></a><span data-ttu-id="aa5bc-999">AppService</span><span class="sxs-lookup"><span data-stu-id="aa5bc-999">AppService</span></span>
* <span data-ttu-id="aa5bc-1000">Unterstützung für die App Service-Umgebung (App Service Environment, ASE) und Zeitlimit zu `webapp ssh` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1000">Added support for ASE and timeout to `webapp ssh`</span></span>
* <span data-ttu-id="aa5bc-1001">Unterstützung für die Einrichtung von CI/CD für eine Azure DevOps-Pipeline aus einem GitHub-Repository zu Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1001">Added support for establishing CI CD to an Azure DevOps pipeline from a Github repository to Function apps</span></span>
* <span data-ttu-id="aa5bc-1002">`--github-pat`-Argument zu `functionapp devops-build create` hinzugefügt, um persönliche GitHub-Zugriffstoken zu akzeptieren</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1002">Added `--github-pat` argument to `functionapp devops-build create` to accept Github personal access token</span></span>
* <span data-ttu-id="aa5bc-1003">`--github-repository`-Argument zu `functionapp devops-build create` hinzugefügt, um das GitHub-Repository mit dem Quellcode einer Funktions-App zu akzeptieren</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1003">Added `--github-repository` argument to `functionapp devops-build create` to accept Github repository that contains a functionapp source code</span></span>
* <span data-ttu-id="aa5bc-1004">Problem behoben, aufgrund dessen bei `az webapp up --logs` ein Fehler auftrat und die .NET Core-Standardversion auf 2.1 aktualisiert wurde</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1004">Fixed issue where `az webapp up --logs` was failing with a error and updating default .NETCORE version to 2.1</span></span>
* <span data-ttu-id="aa5bc-1005">Unnötige Funktions-App-Einstellungen beim Erstellen einer Funktions-App mit Verbrauchsplan entfernt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1005">Removed unnecessary functionapp settings when creating a function app with consumption plan</span></span>
* <span data-ttu-id="aa5bc-1006">`webapp up` geändert, sodass die ASP-Standardzeichenfolge jetzt eine Zahl am Ende anfügt, um einen neuen ASP basierend auf SKU-Optionen zu erstellen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1006">Changed `webapp up` so the default asp string now appends number at the end to create a new ASP based on SKU options</span></span>
* <span data-ttu-id="aa5bc-1007">`-b` als Option für `webapp up` hinzugefügt, um die App im Browser zu starten</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1007">Added `-b` as an option to `webapp up` to launch the app in the browser</span></span>
* <span data-ttu-id="aa5bc-1008">`webapp deployment source config zip` geändert, um die `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`-Umgebungsvariable zu behandeln</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1008">Changed `webapp deployment source config zip` to handle `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="aa5bc-1009">Bereitstellungs-Manager</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1009">Deployment Manager</span></span>
* <span data-ttu-id="aa5bc-1010">[VORSCHAUVERSIPN] Erstellen und Verwalten von Artefakten, die Rollouts unterstützen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1010">[PREVIEW] Create and manage artifacts that support rollouts</span></span>

### <a name="lab"></a><span data-ttu-id="aa5bc-1011">Labor</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1011">Lab</span></span>
* <span data-ttu-id="aa5bc-1012">Fehler behoben, der zu einer vorzeitigen Beendigung führen würde</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1012">Fixed bug which would cause an early exit</span></span>

### <a name="network"></a><span data-ttu-id="aa5bc-1013">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1013">Network</span></span>
* <span data-ttu-id="aa5bc-1014">Automatische Delegierung des Namenservers im übergeordneten Element während der Erstellung der untergeordneten Zone zu `dns zone create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1014">Added auto name server delegation to `dns zone create` in parent during child zone creation</span></span>

### <a name="resource"></a><span data-ttu-id="aa5bc-1015">Resource</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1015">Resource</span></span>
* <span data-ttu-id="aa5bc-1016">[VERALTET]: Argumente `--link-id`, `--target-id` und `--filter-string` von `resource link` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1016">[DEPRECATED] Deprecated `--link-id`, `--target-id` and `--filter-string` arguments of `resource link`</span></span>
  * <span data-ttu-id="aa5bc-1017">Verwenden Sie stattdessen die Argumente `--link`, `--target` und `--filter`.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1017">Use the arguments `--link`, `--target`, and `--filter` instead</span></span>
* <span data-ttu-id="aa5bc-1018">Problem behoben, aufgrund dessen `resource link [create|update]`-Befehle nicht verwendet werden konnten</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1018">Fixed issue where `resource link [create|update]` commands would not work</span></span>
* <span data-ttu-id="aa5bc-1019">Problem behoben, aufgrund dessen das Löschen anhand einer Ressourcen-ID bei einem Fehler zu einem Absturz führen konnte</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1019">Fixed an issue where deleting using a resource ID could crash on error</span></span>

### <a name="sql"></a><span data-ttu-id="aa5bc-1020">SQL</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1020">SQL</span></span>
* <span data-ttu-id="aa5bc-1021">Unterstützung für benutzerdefinierte Zeitzonen auf verwalteten Instanzen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1021">Added support for custom time zone on managed instances</span></span>
* <span data-ttu-id="aa5bc-1022">Geändert, um die Verwendung des Namens eines Pools für elastische Datenbanken mit `sql db update` zuzulassen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1022">Changed to allow elastic pool name to be used with `sql db update`</span></span>
* <span data-ttu-id="aa5bc-1023">Unterstützung für `--no-wait` zu `sql server [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1023">Added `--no-wait` support to `sql server [create|update]`</span></span>
* <span data-ttu-id="aa5bc-1024">Befehl `sql server wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1024">Added command `sql server wait`</span></span>

### <a name="storage"></a><span data-ttu-id="aa5bc-1025">Storage</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1025">Storage</span></span>
* <span data-ttu-id="aa5bc-1026">Problem mit doppelt codierten SAS-Token in `storage blob generate-sas` behoben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1026">Fixed issue with double-encoded SAS tokens in `storage blob generate-sas`</span></span>

### <a name="vm"></a><span data-ttu-id="aa5bc-1027">VM</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1027">VM</span></span>
* <span data-ttu-id="aa5bc-1028">`--skip-shutdown`-Flag zum Ausschalten von VMs ohne Herunterfahren zu `vm|vmss stop` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1028">Added `--skip-shutdown` flag to `vm|vmss stop` to power-off VMs without shutdown</span></span>
* <span data-ttu-id="aa5bc-1029">`--storage-account-type`-Argument zum Festlegen des Kontotyps des Veröffentlichungsprofils zu `sig image-version create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1029">Added `--storage-account-type` argument to `sig image-version create` to set the publishing profile's account type</span></span>
* <span data-ttu-id="aa5bc-1030">`--target-regions`-Argument zu `sig image-version create` hinzugefügt, um das Festlegen von regionsspezifischen Speicherkontotypen zuzulassen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1030">Added `--target-regions` argument to `sig image-version create` to allow setting region-specific storage account types</span></span>

## <a name="april-9-2019"></a><span data-ttu-id="aa5bc-1031">9\. April 2019</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1031">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="aa5bc-1032">Core</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1032">Core</span></span>
* <span data-ttu-id="aa5bc-1033">Problem behoben, aufgrund dessen einige Erweiterungen mit der Version `Unknown` angezeigt wurden und nicht aktualisiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1033">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="aa5bc-1034">ACR</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1034">ACR</span></span>
* <span data-ttu-id="aa5bc-1035">Unterstützung für die kontextlose Ausführung eines Images hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1035">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="aa5bc-1036">AMS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1036">AMS</span></span>
* [VERALTET]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
[DEPRECATED]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [BREAKING CHANGE]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="aa5bc-1039">Unterstützung für neue Verschlüsselungsparameter in `ams streaming-policy create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1039">Added new encryption parameters support in `ams streaming-policy create`</span></span>
* <span data-ttu-id="aa5bc-1040">Neuer Parameter `--filters` zu `ams streaming-locator create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1040">Added new paramter `--filters` to `ams streaming-locator create`</span></span>

### <a name="appservice"></a><span data-ttu-id="aa5bc-1041">AppService</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1041">AppService</span></span>
* <span data-ttu-id="aa5bc-1042">Unterstützung für `--logs` zu `webapp up` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1042">Added `--logs` support to `webapp up`</span></span>
* <span data-ttu-id="aa5bc-1043">Probleme bei der Generierung von `azure-pipelines.yml` beim Befehl `functionapp devops-build create` behoben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1043">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="aa5bc-1044">Fehlerbehandlung und Indikatoren für `unctionapp devops-build create` verbessert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1044">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="aa5bc-1045">[BREAKING CHANGE] Flag `--local-git` für den Befehl `devops-build` entfernt; lokale Git-Erkennung und -Verarbeitung sind zum Erstellen von Azure DevOps-Pipelines obligatorisch</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1045">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="aa5bc-1046">Unterstützung für das Erstellen von Linux-Functions-Plänen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1046">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="aa5bc-1047">Möglichkeit zum Wechseln eines Plans unter einer Funktions-App mit `functionapp update --plan` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1047">Added ability to switch a plan underneath a function app using `functionapp update --plan`</span></span>
* <span data-ttu-id="aa5bc-1048">Unterstützung für Einstellungen zum horizontalen Hochskalieren für den Azure Functions-Premium-Plan hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1048">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="aa5bc-1049">CDN</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1049">CDN</span></span>
* <span data-ttu-id="aa5bc-1050">Unterstützung hinzugefügt für `Microsoft_Standard` und `Standard_ChinaCdn`</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1050">Added support for `Microsoft_Standard` and `Standard_ChinaCdn`</span></span>

### <a name="feedback"></a><span data-ttu-id="aa5bc-1051">Feedback</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1051">Feedback</span></span>
* <span data-ttu-id="aa5bc-1052">`feedback` zur Anzeige von Metadaten zu den zuletzt ausgeführten Befehlen geändert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1052">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="aa5bc-1053">`feedback` geändert, um den Benutzer zur Unterstützung beim Issueerstellungsprozess aufzufordern (durch Öffnen eines Browsers und Verwenden einer Issuevorlage)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1053">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="aa5bc-1054">`feedback` geändert, um den Issuetext bei der Ausführung mit „--verbose“ auszugeben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1054">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="aa5bc-1055">Überwachen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1055">Monitor</span></span>
* <span data-ttu-id="aa5bc-1056">Problem behoben, aufgrund dessen „Count“ kein zulässiger Wert für `metrics alert [create|update]` war</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1056">Fixed issue where "count" was not a permitted value with `metrics alert [create|update]`</span></span> 

### <a name="network"></a><span data-ttu-id="aa5bc-1057">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1057">Network</span></span>
* <span data-ttu-id="aa5bc-1058">Problem behoben, aufgrund dessen das Tabellenformat mit `vnet-gateway list-bgp-peer-status` nicht angezeigt wurde</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1058">Fixed table format not displaying with `vnet-gateway list-bgp-peer-status`</span></span>
* <span data-ttu-id="aa5bc-1059">Befehle `list-request-headers` und `list-response-headers` zu `application-gateway rewrite-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1059">Added `list-request-headers` and `list-response-headers` commands to `application-gateway rewrite-rule`</span></span>
* <span data-ttu-id="aa5bc-1060">Befehl `list-server-variables` zu `application-gateway rewrite-rule condition` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1060">Added `list-server-variables` command to `application-gateway rewrite-rule condition`</span></span>
* <span data-ttu-id="aa5bc-1061">Problem behoben, aufgrund dessen durch das Aktualisieren des Linkstatus für einen ExpressRoute-Port eine Ausnahme vom Typ „unbekanntes Attribut“ ausgelöst wurde: `express-route port update`</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1061">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception `express-route port update`</span></span>

### <a name="privatedns"></a><span data-ttu-id="aa5bc-1062">PrivateDNS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1062">PrivateDNS</span></span>
* <span data-ttu-id="aa5bc-1063">`network private-dns` für private DNS-Zonen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1063">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="aa5bc-1064">Resource</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1064">Resource</span></span>
* <span data-ttu-id="aa5bc-1065">Problem mit `deployment create` und `group deployment create` behoben, aufgrund dessen eine Parameterdatei mit leerem Parametersatz nicht verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1065">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="aa5bc-1066">Role</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1066">Role</span></span>
* <span data-ttu-id="aa5bc-1067">`create-for-rbac` korrigiert, um `--years` korrekt zu verarbeiten</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1067">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="aa5bc-1068">[BREAKING CHANGE]`role assignment delete` geändert, um eine Eingabeaufforderung anzuzeigen, wenn alle Zuweisungen im Abonnement ohne Bedingungen gelöscht werden</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1068">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="aa5bc-1069">SQL</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1069">SQL</span></span>
* <span data-ttu-id="aa5bc-1070">`sql mi [create|update]` mit den Eigenschaften „proxyOverride“ und „publicDataEndpointEnabled“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1070">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="aa5bc-1071">Storage</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1071">Storage</span></span>
* <span data-ttu-id="aa5bc-1072">[BREAKING CHANGE] Ergebnis von `storage blob delete` entfernt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1072">[BREAKING CHANGE] Removed result of `storage blob delete`</span></span>
* <span data-ttu-id="aa5bc-1073">`--full-uri` zu `storage blob generate-sas` hinzugefügt, um den vollständigen URI für das Blob mit SAS zu erstellen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1073">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="aa5bc-1074">`--file-snapshot` zu `storage file copy start` hinzugefügt, um die Datei aus der Momentaufnahme zu kopieren</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1074">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="aa5bc-1075">`storage blob copy cancel` geändert, um anstelle der Ausnahme für „NoPendingCopyOperation“ nur den Fehler anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1075">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="aa5bc-1076">26. März 2019</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1076">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="aa5bc-1077">Core</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1077">Core</span></span>
* <span data-ttu-id="aa5bc-1078">Probleme mit der Inkompatibilität der Entwicklungserweiterung behoben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1078">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="aa5bc-1079">Die Fehlerbehandlung verweist Kunden jetzt auf die Problemseite.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1079">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="aa5bc-1080">Cloud</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1080">Cloud</span></span>
* <span data-ttu-id="aa5bc-1081">Fehler „Abonnement nicht gefunden“ in `cloud set` behoben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1081">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="aa5bc-1082">ACR</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1082">ACR</span></span>
* <span data-ttu-id="aa5bc-1083">Redundante Quellen im Imageimport korrigiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1083">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="aa5bc-1084">`--auth-mode` wurde den Befehlen `acr build`, `acr run`, `acr task create` und `acr task update` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1084">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="aa5bc-1085">Befehlsgruppe „acr task credential“ zum Verwalten von Anmeldeinformationen für eine Aufgabe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1085">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="aa5bc-1086">„--no-wait“ zum Befehl `acr build` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1086">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="aa5bc-1087">AppService</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1087">AppService</span></span>
* <span data-ttu-id="aa5bc-1088">Problem behoben, das dazu führte, dass die Ausführung aus einem leeren Verzeichnis oder ein Szenario mit unbekannten Code von `webapp up` nicht korrekt behandelt wurde</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1088">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="aa5bc-1089">Problem behoben, aufgrund dessen Slots für `[webapp|functionapp] config ssl bind` nicht verwendet werden konnten</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1089">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="aa5bc-1090">Bot Service</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1090">BOT Service</span></span>
* <span data-ttu-id="aa5bc-1091">`bot prepare-deploy` hinzugefügt, um die Bereitstellung von Bots über `webapp` vorzubereiten</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1091">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="aa5bc-1092">`bot create --kind registration` geändert, um das Kennwort anzuzeigen, falls kein Kennwort angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1092">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="aa5bc-1093">[BREAKING CHANGE]`--endpoint` wurde in `bot create --kind registration` geändert, sodass nun standardmäßig eine leere Zeichenfolge verwendet wird, anstatt eine Angabe zu erfordern.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1093">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="aa5bc-1094">`SCM_DO_BUILD_DURING_DEPLOYMENT` zu den Anwendungseinstellungen der ARM-Vorlage für Web-App-Bot (v4) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1094">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="aa5bc-1095">CDN</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1095">CDN</span></span>
* <span data-ttu-id="aa5bc-1096">Unterstützung für `--no-wait` zu `cdn endpoint [create|update|start|stop|delete|load|purge]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1096">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* <span data-ttu-id="aa5bc-1097">[BREAKING CHANGE] Das standardmäßige Zwischenspeicherverhalten für Abfragezeichenfolgen von `cdn endpoint create` wurde geändert.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1097">[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour.</span></span> <span data-ttu-id="aa5bc-1098">Es wird nicht mehr standardmäßig „IgnoreQueryString“ festgelegt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1098">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="aa5bc-1099">Er wird jetzt vom Dienst festgelegt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1099">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="aa5bc-1100">Cosmosdb</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1100">Cosmosdb</span></span>
* <span data-ttu-id="aa5bc-1101">Unterstützung für `--enable-multiple-write-locations` bei Kontoaktualisierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1101">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="aa5bc-1102">Untergruppe `network-rule` mit Befehlen `add`, `remove` und `list` zum Verwalten von VNET-Regeln eines Cosmos DB-Kontos hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1102">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="aa5bc-1103">Interactive</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1103">Interactive</span></span>
* <span data-ttu-id="aa5bc-1104">Inkompatibilität mit der über azdev installierten interaktiven Erweiterung korrigiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1104">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="aa5bc-1105">Überwachen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1105">Monitor</span></span>
* <span data-ttu-id="aa5bc-1106">Geändert, sodass der Dimensionswert `*` für `monitor metrics alert [create|update]` zulässig ist</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1106">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="aa5bc-1107">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1107">Network</span></span>
* <span data-ttu-id="aa5bc-1108">Befehlsgruppe `rewrite-rule` zu `application-gateway` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1108">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="aa5bc-1109">Profil</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1109">Profile</span></span>
* <span data-ttu-id="aa5bc-1110">Kontounterstützung auf Mandantenebene für verwaltete Dienstidentität zu `login` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1110">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="aa5bc-1111">Postgres</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1111">Postgres</span></span> 
* <span data-ttu-id="aa5bc-1112">postgresql-Befehle vom Typ `replica` und Befehl `restart server` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1112">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="aa5bc-1113">Änderungen vorgenommen, um den Standardspeicherort aus der Ressourcengruppe abzurufen, wenn er für die Erstellung von Servern nicht angegeben wurde, und um eine Überprüfung für die Aufbewahrungstage hinzuzufügen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1113">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="aa5bc-1114">Resource</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1114">Resource</span></span>
* <span data-ttu-id="aa5bc-1115">Verbesserte Tabellenausgabe für `deployment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1115">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="aa5bc-1116">Problem mit `deployment [create|validate]` behoben, aufgrund dessen der Typ „secureObject“ nicht erkannt wurde</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1116">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="aa5bc-1117">Graph</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1117">Graph</span></span>
* <span data-ttu-id="aa5bc-1118">Unterstützung für `--end-date` zu `ad [app|sp] credential reset` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1118">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="aa5bc-1119">Unterstützung für das Hinzufügen von Berechtigungen mit `ad app permission add` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1119">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="aa5bc-1120">Fehler mit `ad app permission list` behoben, wenn keine Berechtigungen vorlagen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1120">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="aa5bc-1121">Änderung an `ad sp delete` vorgenommen, um das Entfernen einer Rollenzuweisung zu überspringen, wenn das aktuelle Konto kein Abonnement enthält</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1121">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="aa5bc-1122">`ad app create` geändert, sodass ohne Angabe für `--identifier-uris` standardmäßig eine leere Liste verwendet wird</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1122">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="aa5bc-1123">storage</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1123">storage</span></span>
* <span data-ttu-id="aa5bc-1124">`--snapshot` zu `storage file download-batch` für den Download von einer Freigabemomentaufnahme hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1124">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="aa5bc-1125">Statusanzeige für `storage blob [download-batch|upload-batch]` geändert, damit sie weniger ausführlich dargestellt wird und das aktuelle Blob angibt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1125">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="aa5bc-1126">Problem mit `storage account update` behoben, das beim Aktualisieren von Verschlüsselungsparametern auftrat</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1126">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="aa5bc-1127">Problem behoben, bei dem für `storage blob show` ein Fehler auftrat, wenn oauth (`--auth-mode=login`) verwendet wurde</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1127">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="aa5bc-1128">VM</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1128">VM</span></span>
* <span data-ttu-id="aa5bc-1129">Befehl `image update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1129">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="aa5bc-1130">12. März 2019</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1130">March 12, 2019</span></span>

<span data-ttu-id="aa5bc-1131">Version 2.0.60</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1131">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="aa5bc-1132">Core</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1132">Core</span></span>

* <span data-ttu-id="aa5bc-1133">Falsche Fehlermeldung in `cloud set` zu nicht gefundenem Abonnement korrigiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1133">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="aa5bc-1134">ACR</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1134">ACR</span></span>

* <span data-ttu-id="aa5bc-1135">Redundante Quellen im Imageimport korrigiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1135">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="aa5bc-1136">ACS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1136">ACS</span></span>

* <span data-ttu-id="aa5bc-1137">Änderung vorgenommen, um den Parameter `--listen-address` für `aks browse` zu ignorieren, wenn er nicht von kubectl unterstützt wird</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1137">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="aa5bc-1138">AppService</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1138">AppService</span></span>

* <span data-ttu-id="aa5bc-1139">`[webapp|functionapp] deployment list-publishing-credentials` hinzugefügt, um die Kudu-Veröffentlichungs-URL und die entsprechenden Anmeldeinformationen abzurufen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1139">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="aa5bc-1140">Fehlerhafte Ausgabeanweisung für `webapp auth update` entfernt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1140">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="aa5bc-1141">`functionapp` korrigiert, um das korrekte Image für die Runtime in App Service-Plänen unter Linux festzulegen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1141">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="aa5bc-1142">Vorschau-Tag für `webapp up` entfernt und Verbesserungen am Befehl implementiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1142">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="aa5bc-1143">Botservice</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1143">Botservice</span></span>

* <span data-ttu-id="aa5bc-1144">`SCM_DO_BUILD_DURING_DEPLOYMENT` zu den Anwendungseinstellungen der ARM-Vorlage für Web-App-Bot (v4) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1144">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="aa5bc-1145">`Microsoft-BotFramework-AppId` und `Microsoft-BotFramework-AppPassword` zu den Anwendungseinstellungen der ARM-Vorlage für Web-App-Bot (v4) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1145">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="aa5bc-1146">Einfache Anführungszeichen aus der Befehlsausgabe von `bot publish` am Ende von `bot create` entfernt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1146">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="aa5bc-1147">`bot publish` wurde geändert und ist jetzt asynchron.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1147">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="aa5bc-1148">Container</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1148">Container</span></span>

* <span data-ttu-id="aa5bc-1149">Argument `--no-wait` zu `container [start|restart]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1149">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="aa5bc-1150">EventHub</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1150">EventHub</span></span>

* <span data-ttu-id="aa5bc-1151">Flag `--skip-empty-archives` zu `eventhub create|update` hinzugefügt, um leere Archive in der Aufzeichnung zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1151">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="aa5bc-1152">Suchen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1152">Find</span></span>

* <span data-ttu-id="aa5bc-1153">Umfangreiches Funktionsupdate</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1153">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="aa5bc-1154">HDInsight</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1154">HDInsight</span></span>

* <span data-ttu-id="aa5bc-1155">Parameter `--storage-account-managed-identity` zu `hdinsight create` hinzugefügt, um MSI in ADLS Gen2 zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1155">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="aa5bc-1156">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1156">Network</span></span>

* <span data-ttu-id="aa5bc-1157">Problem mit `vpn-connection update` behoben, aufgrund dessen die Aktualisierung einer VPN-Verbindung zwischen Gateways in verschiedenen Abonnements fehlschlug</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1157">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="aa5bc-1158">Rdbms</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1158">Rdbms</span></span>

* <span data-ttu-id="aa5bc-1159">Kleinere Korrekturen, um den Standardspeicherort aus der Ressourcengruppe abzurufen, wenn er für die Erstellung von Servern nicht angegeben wurde, und um eine Überprüfung für die Aufbewahrungstage hinzuzufügen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1159">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="aa5bc-1160">Role</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1160">Role</span></span>

* <span data-ttu-id="aa5bc-1161">`role definition update` wurde korrigiert und nutzt nun die ID, um die Definition korrekt aufzulösen.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1161">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="aa5bc-1162">`ad app credential reset` geändert, um die Annahme zu entfernen, dass der Dienstprinzipal der App stets vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1162">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="aa5bc-1163">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1163">Service Fabric</span></span>

* <span data-ttu-id="aa5bc-1164">Das Problem, dass `sf cluster list` nicht wiederholbar war, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1164">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="aa5bc-1165">26. Februar 2019</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1165">February 26, 2019</span></span>

<span data-ttu-id="aa5bc-1166">Version 2.0.59</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1166">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="aa5bc-1167">Core</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1167">Core</span></span>

* <span data-ttu-id="aa5bc-1168">Problem behoben, aufgrund dessen die Verwendung von `--subscription NAME` in einigen Instanzen eine Ausnahme ausgelöst hat</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1168">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="aa5bc-1169">ACR</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1169">ACR</span></span>

* <span data-ttu-id="aa5bc-1170">Parameter `--target` für die Befehle `acr build`, `acr task create` und `acr task update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1170">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="aa5bc-1171">Verbesserte Fehlerbehandlung für Runtimebefehle, wenn keine Anmeldung bei Azure besteht</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1171">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="aa5bc-1172">ACS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1172">ACS</span></span>

* <span data-ttu-id="aa5bc-1173">Option `--listen-address` zu `aks port-forward` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1173">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="aa5bc-1174">AppService</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1174">AppService</span></span>

* <span data-ttu-id="aa5bc-1175">Befehl `functionapp devops-build` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1175">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="aa5bc-1176">Batch</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1176">Batch</span></span>
* <span data-ttu-id="aa5bc-1177">[BREAKING CHANGE] Befehl `batch pool upgrade os` entfernt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1177">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="aa5bc-1178">[BREAKING CHANGE]`Pacakges`-Eigenschaft aus `Application`-Antworten entfernt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1178">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="aa5bc-1179">Befehl `batch application package list` zum Auflisten von Paketen einer Anwendung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1179">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="aa5bc-1180">[BREAKING CHANGE]`--application-id` in allen `batch application`-Befehlen in `--application-name` geändert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1180">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="aa5bc-1181">Argument `--json-file` für Befehle zum Anfordern der unformatierten API-Antwort hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1181">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="aa5bc-1182">Validierung aktualisiert, sodass das `https://`-Element automatisch in alle Endpunkte aufgenommen wird, wenn es fehlt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1182">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="aa5bc-1183">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1183">CosmosDB</span></span>

* <span data-ttu-id="aa5bc-1184">Untergruppe `network-rule` mit Befehlen `add`, `remove` und `list` zum Verwalten von VNET-Regeln eines Cosmos DB-Kontos hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1184">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="aa5bc-1185">Kusto</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1185">Kusto</span></span>

* <span data-ttu-id="aa5bc-1186">[BREAKING CHANGE] Typen `hot_cache_period` und `soft_delete_period` für Datenbank in Format der Zeitspanne nach ISO8601 geändert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1186">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="aa5bc-1187">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1187">Network</span></span>

* <span data-ttu-id="aa5bc-1188">Argument `--express-route-gateway-bypass` zu `vpn-connection [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1188">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="aa5bc-1189">Befehlsgruppen aus `express-route`-Erweiterungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1189">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="aa5bc-1190">Befehlsgruppen `express-route gateway` und `express-route port` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1190">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="aa5bc-1191">Argument `--legacy-mode` zu `express-route peering [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1191">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="aa5bc-1192">Argumente `--allow-classic-operations` und `--express-route-port` zu `express-route [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1192">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="aa5bc-1193">Argument `--gateway-default-site` zu `vnet-gateway [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1193">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="aa5bc-1194">Befehle vom Typ `ipsec-policy` zu `vnet-gateway` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1194">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="aa5bc-1195">Resource</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1195">Resource</span></span>

* <span data-ttu-id="aa5bc-1196">Problem mit `deployment create` behoben, aufgrund dessen beim Feld „Typ“ die Groß-/Kleinschreibung beachtet wurde</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1196">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="aa5bc-1197">Unterstützung für URI-basierte Parameterdatei zu `policy assignment create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1197">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="aa5bc-1198">Unterstützung für URI-basierte Parameter und Definitionen zu `policy set-definition update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1198">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="aa5bc-1199">Verarbeitung von Parametern und Regeln für `policy definition update` korrigiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1199">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="aa5bc-1200">Problem mit `resource show/update/delete/tag/invoke-action` behoben, aufgrund dessen bei abonnementübergreifenden IDs die Abonnement-ID nicht ordnungsgemäß berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1200">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="aa5bc-1201">Role</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1201">Role</span></span>

* <span data-ttu-id="aa5bc-1202">Unterstützung für App-Rollen zu `ad app [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1202">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="aa5bc-1203">VM</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1203">VM</span></span>

* <span data-ttu-id="aa5bc-1204">Problem mit `vm create where ` behoben, aufgrund dessen der beschleunigte Netzwerkbetrieb für Ubuntu 18.0 nicht standardmäßig aktiviert war</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1204">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="aa5bc-1205">12. Februar 2019</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1205">February 12, 2019</span></span>

<span data-ttu-id="aa5bc-1206">Version 2.0.58</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1206">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="aa5bc-1207">Core</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1207">Core</span></span>

* <span data-ttu-id="aa5bc-1208">`az --version` zeigt jetzt eine Benachrichtigung an, wenn Sie Pakete haben, für die ein Update verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1208">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="aa5bc-1209">Die Regression, dass `--ids` nicht mehr mit JSON-Ausgaben verwendet werden konnte, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1209">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="aa5bc-1210">ACR</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1210">ACR</span></span>
* <span data-ttu-id="aa5bc-1211">[BREAKING CHANGE] Die Befehlsgruppe `acr build-task` wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1211">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="aa5bc-1212">[BREAKING CHANGE] Die Optionen `--tag` und `--manifest` wurden aus `acr repository delete` entfernt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1212">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="aa5bc-1213">ACS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1213">ACS</span></span>
* <span data-ttu-id="aa5bc-1214">Unterstützung für Namen ohne Berücksichtigung von Groß-/Kleinschreibung wurde zu `aks [enable-addons|disable-addons]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1214">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="aa5bc-1215">Unterstützung für Azure Active Directory-Aktualisierungsvorgang mithilfe von `aks update-credentials --reset-aad` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1215">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="aa5bc-1216">Die Information, dass `--output` für `aks get-credentials` ignoriert wird, wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1216">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="aa5bc-1217">AMS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1217">AMS</span></span>
* <span data-ttu-id="aa5bc-1218">Befehle vom Typ `ams streaming-endpoint [start | stop | create | update] wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1218">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="aa5bc-1219">Befehle vom Typ `ams live-event [create | start | stop | reset] wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1219">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="aa5bc-1220">AppService</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1220">Appservice</span></span>
* <span data-ttu-id="aa5bc-1221">Die Möglichkeit zum Erstellen und Konfigurieren von Funktionen mithilfe von ACR-Containern wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1221">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="aa5bc-1222">Unterstützung für das Aktualisieren von Web-App-Konfigurationen über JSON wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1222">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="aa5bc-1223">Die Hilfe für `appservice-plan-update` wurde verbessert.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1223">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="aa5bc-1224">Unterstützung für App-Erkenntnisse beim Erstellen von Funktions-Apps wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1224">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="aa5bc-1225">Probleme mit der Web-App SSH wurden behoben.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1225">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="aa5bc-1226">Botservice</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1226">Botservice</span></span>
* <span data-ttu-id="aa5bc-1227">Die Benutzeroberfläche für `bot publish` wurde verbessert.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1227">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="aa5bc-1228">Eine Warnung für Zeitlimit bei der Ausführung von `npm install` während `az bot publish` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1228">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="aa5bc-1229">Ungültiges char-Element wurde `.` aus `--name` in `az bot create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1229">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="aa5bc-1230">Eine Änderung wurde vorgenommen, um die zufällige Zuordnung von Ressourcennamen beim Erstellen von Azure Storage-Instanzen, App Service-Plänen, Funktions-/Web-Apps und Application Insights-Instanzen zu verhindern.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1230">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="aa5bc-1231">[VERALTET] Argument `--proj-name` zugunsten von `--proj-file-path` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1231">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="aa5bc-1232">`az bot publish` wurde geändert, um abgerufene IIS-Bereitstellungsdateien vom Typ „Node.js“ zu entfernen, wenn sie nicht bereits vorhanden waren.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1232">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="aa5bc-1233">Das `--keep-node-modules` Argument wurde zu `az bot publish` hinzugefügt, damit der Ordner `node_modules` in App Service nicht gelöscht wird.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1233">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="aa5bc-1234">Das Schlüssel-Wert-Paar `"publishCommand"` wurde der Ausgabe von `az bot create` beim Erstellen einer Funktions-App oder eines Web-App-Bots hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1234">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="aa5bc-1235">Der Wert von `"publishCommand"` ist ein `az bot publish`-Befehl, der bereits die erforderlichen Parameter zum Veröffentlichen des neu erstellten Bots enthält.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1235">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="aa5bc-1236">`"WEBSITE_NODE_DEFAULT_VERSION"` in der ARM-Vorlage wurde so aktualisiert, dass v4-SDK-Bots 10.14.1 anstelle von 8.9.4 verwenden.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1236">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="aa5bc-1237">Key Vault</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1237">Key Vault</span></span>
* <span data-ttu-id="aa5bc-1238">Ein Problem mit `keyvault secret backup` wurde behoben, aufgrund dessen einige Benutzer bei Verwendung von `--id` einen `unexpected_keyword`-Fehler erhielten.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1238">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="aa5bc-1239">Überwachen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1239">Monitor</span></span>
* <span data-ttu-id="aa5bc-1240">`monitor metrics alert [create|update]` wurde so geändert, dass der Dimensionswert `*` zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1240">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="aa5bc-1241">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1241">Network</span></span>
* <span data-ttu-id="aa5bc-1242">`dns zone export` wurde geändert, um sicherzustellen, dass es sich bei exportierten CNAMEs um FQDNs handelt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1242">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="aa5bc-1243">Parameter `--gateway-name` wurde zu `nic ip-config address-pool [add|remove]` hinzugefügt, um Back-End-Adresspools von Anwendungsgateways zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1243">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="aa5bc-1244">Argumente `--traffic-analytics` und `--workspace` wurden zu `network watcher flow-log configure` hinzugefügt, um Datenverkehrsanalysen über einen Log Analytics-Arbeitsbereich zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1244">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="aa5bc-1245">`--idle-timeout` und `--floating-ip` wurden zu `lb inbound-nat-pool [create|update]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1245">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="aa5bc-1246">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1246">Policy Insights</span></span>
* <span data-ttu-id="aa5bc-1247">`policy remediation`-Befehle wurden hinzugefügt, um Korrekturfunktionen der Ressourcenrichtlinie zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1247">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="aa5bc-1248">RDBMS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1248">RDBMS</span></span>
* <span data-ttu-id="aa5bc-1249">Hilfemeldung und Befehlsparameter wurden verbessert.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1249">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="aa5bc-1250">Redis</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1250">Redis</span></span>
* <span data-ttu-id="aa5bc-1251">Befehle zum Verwalten von „firewall-rules“ (erstellen, aktualisieren, löschen, anzeigen, auflisten) wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1251">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="aa5bc-1252">Befehle zum Verwalten von „server-link“ (erstellen, aktualisieren, löschen, anzeigen, auflisten) wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1252">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="aa5bc-1253">Befehle zum Verwalten von „patch-schedule“ (erstellen, aktualisieren, löschen, anzeigen, auflisten) wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1253">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="aa5bc-1254">Unterstützung für Verfügbarkeitszonen und TLS-Mindestversion wurden zu „redis create“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1254">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="aa5bc-1255">[BREAKING CHANGE] Befehle `redis update-settings` und `redis list-all` wurden entfernt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1255">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="aa5bc-1256">[BREAKING CHANGE] Parameter für `redis create`: „Mandanteneinstellungen“ werden im Format „Schlüssel[=Wert] nicht akzeptiert.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1256">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="aa5bc-1257">[VERALTET] Warnmeldung zur Markierung des Befehls `redis import-method` als veraltet hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1257">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="aa5bc-1258">Role</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1258">Role</span></span>
* <span data-ttu-id="aa5bc-1259">[BREAKING CHANGE] Befehl `az identity` wurde aus den `vm`-Befehlen hierher verschoben.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1259">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="aa5bc-1260">SQL-VM</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1260">SQL VM</span></span>
* <span data-ttu-id="aa5bc-1261">[VERALTET] Argument `--boostrap-acc-pwd` aufgrund eines Tippfehlers als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1261">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="aa5bc-1262">VM</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1262">VM</span></span>
* <span data-ttu-id="aa5bc-1263">`vm list-skus` wurde so geändert, dass `--all` anstelle von `--all true` verwendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1263">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="aa5bc-1264">`vmss run-command [invoke | list | show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1264">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="aa5bc-1265">Ein Fehler wurde behoben, aufgrund dessen bei der Ausführung von `vmss encryption enable` bisher ein Fehler auftrat.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1265">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="aa5bc-1266">[BREAKING CHANGE] Die Befehle vom Typ `az identity` wurden zu `role`-Befehlen verschoben.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1266">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="aa5bc-1267">31. Januar 2019</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1267">January 31, 2019</span></span>

<span data-ttu-id="aa5bc-1268">Version 2.0.57</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1268">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="aa5bc-1269">Core</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1269">Core</span></span>

* <span data-ttu-id="aa5bc-1270">Hotfix für [Problem 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1270">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="aa5bc-1271">28. Januar 2019</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1271">January 28, 2019</span></span>

<span data-ttu-id="aa5bc-1272">Version 2.0.56</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1272">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="aa5bc-1273">ACR</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1273">ACR</span></span>
* <span data-ttu-id="aa5bc-1274">Unterstützung für VNet/IP-Regeln wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1274">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="aa5bc-1275">ACS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1275">ACS</span></span>
* <span data-ttu-id="aa5bc-1276">Virtuelle Knoten (Vorschau) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1276">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="aa5bc-1277">Verwaltete OpenShift-Befehle wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1277">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="aa5bc-1278">Unterstützung für den Dienstprinzipal-Updatevorgang mit `aks update-credentials -reset-service-principal` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1278">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="aa5bc-1279">AMS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1279">AMS</span></span>
* <span data-ttu-id="aa5bc-1280">[BREAKING CHANGE]`ams asset get-streaming-locators` in `ams asset list-streaming-locators` umbenannt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1280">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="aa5bc-1281">[BREAKING CHANGE]`ams streaming-locator get-content-keys` in `ams streaming-locator list-content-keys` umbenannt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1281">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="aa5bc-1282">AppService</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1282">Appservice</span></span>
* <span data-ttu-id="aa5bc-1283">Unterstützung für App-Erkenntnisse in `functionapp create` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1283">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="aa5bc-1284">Unterstützung für die Erstellung von App Service-Plänen (einschließlich Elastic Premium) wurde zu Funktions-Apps hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1284">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="aa5bc-1285">Probleme bei einer App-Einstellung mit Elastic Premium-Plänen wurden behoben.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1285">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="aa5bc-1286">Container</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1286">Container</span></span>
* <span data-ttu-id="aa5bc-1287">Befehl `container start` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1287">Added `container start` command</span></span>
* <span data-ttu-id="aa5bc-1288">Eine Änderung wurde vorgenommen, um bei der Containererstellung die Verwendung von Dezimalwerten für die CPU zuzulassen.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1288">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="aa5bc-1289">EventGrid</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1289">EventGrid</span></span>
* <span data-ttu-id="aa5bc-1290">Parameter `--deadletter-endpoint` zu `event-subscription [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1290">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="aa5bc-1291">„storagequeue“ und „hybridconnection“ wurden als neue Werte für „event-subscription [create|update] --endpoint-type“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1291">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="aa5bc-1292">Parameter `--max-delivery-attempts` und `--event-ttl` wurden zu `event-subscription create` hinzugefügt, um die Wiederholungsrichtlinie für Ereignisse anzugeben.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1292">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="aa5bc-1293">Eine Warnmeldung wurde zu `event-subscription [create|update]` hinzugefügt, wenn Webhook als Ziel für ein Ereignisabonnement verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1293">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="aa5bc-1294">Parameter „source-resource-id“ wurde für alle Befehle im Zusammenhang mit Ereignisabonnements hinzugefügt, und alle anderen Parameter im Zusammenhang mit Quellressourcen wurden als veraltet markiert.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1294">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="aa5bc-1295">HDInsight</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1295">HDInsight</span></span>
* <span data-ttu-id="aa5bc-1296">[BREAKING CHANGE] Die Parameter `--virtual-network` und `--subnet-name` wurden aus `hdinsight [application] create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1296">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="aa5bc-1297">[BREAKING CHANGE]`hdinsight create --storage-account` wurde so geändert, dass der Name oder die ID eines Speicherkontos anstellen von Blobendpunkten akzeptiert wird.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1297">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="aa5bc-1298">Parameter `--vnet-name` und `--subnet-name` zu `hdinsight create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1298">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="aa5bc-1299">Unterstützung für das Enterprise-Sicherheitspaket und Datenträgerverschlüsselung wurde zu `hdinsight create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1299">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="aa5bc-1300">Befehl `hdinsight rotate-disk-encryption-key` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1300">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="aa5bc-1301">Befehl `hdinsight update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1301">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="aa5bc-1302">IoT</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1302">IoT</span></span>
* <span data-ttu-id="aa5bc-1303">Codierungsformat wurde zu Befehl „routing-endpoint“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1303">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="aa5bc-1304">Kusto</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1304">Kusto</span></span>
* <span data-ttu-id="aa5bc-1305">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1305">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="aa5bc-1306">Überwachen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1306">Monitor</span></span>
* <span data-ttu-id="aa5bc-1307">ID-Vergleich wurde so geändert, dass Groß-/Kleinschreibung nicht mehr beachtet wird.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1307">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="aa5bc-1308">Profil</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1308">Profile</span></span>
* <span data-ttu-id="aa5bc-1309">Konto auf Mandantenebene für verwaltete Dienstidentität für `login` wird aktiviert.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1309">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="aa5bc-1310">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1310">Network</span></span>
* <span data-ttu-id="aa5bc-1311">Ein Problem mit `express-route update` wurde behoben, aufgrund dessen das Argument `--bandwidth` ignoriert wurde.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1311">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="aa5bc-1312">Ein Problem mit `ddos-protection update` wurde behoben, aufgrund dessen das festgelegte Verständnis zu einer Stapelüberwachung führte.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1312">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="aa5bc-1313">Resource</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1313">Resource</span></span>
* <span data-ttu-id="aa5bc-1314">Unterstützung für die URI-Parameterdatei wurde zu `group deployment create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1314">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="aa5bc-1315">Unterstützung für verwaltete Identitäten wurde zu `policy assignment [create|list|show]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1315">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="aa5bc-1316">Virtueller SQL-Computer</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1316">SQL Virtual Machine</span></span>
* <span data-ttu-id="aa5bc-1317">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1317">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="aa5bc-1318">Storage</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1318">Storage</span></span>
* <span data-ttu-id="aa5bc-1319">Eine Lösung wurde so geändert, dass nur Eigenschaften aktualisiert werden, die im selben Objekt geändert werden.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1319">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="aa5bc-1320">Nr. 8021 wurde korrigiert, Binärdaten werden bei der Rückgabe in Base64 codiert.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1320">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="aa5bc-1321">VM</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1321">VM</span></span>
* <span data-ttu-id="aa5bc-1322">`vm encryption enable` wurde geändert, um den Schlüsseltresor für die Datenträgerverschlüsselung zu überprüfen und sicherzustellen, dass der Schlüsseltresor für die Schlüsselverschlüsselung vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1322">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="aa5bc-1323">Flag `--force` wurde zu `vm encryption enable` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1323">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="aa5bc-1324">15. Januar 2019</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1324">January 15, 2019</span></span>

<span data-ttu-id="aa5bc-1325">Version 2.0.55</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1325">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="aa5bc-1326">ACR</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1326">ACR</span></span>
* <span data-ttu-id="aa5bc-1327">Wurde geändert, um den Push eines nicht vorhandenen Helm-Diagramms zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1327">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="aa5bc-1328">Wurde geändert, um Laufzeitvorgänge ohne ARM-Anforderungen zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1328">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="aa5bc-1329">[VERALTET] Parameter `--resource-group` in folgenden Befehlen als veraltet markiert:</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1329">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="aa5bc-1330">ACS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1330">ACS</span></span>
* <span data-ttu-id="aa5bc-1331">Unterstützung für neue ACI-Regionen wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1331">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="aa5bc-1332">AppService</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1332">Appservice</span></span>
* <span data-ttu-id="aa5bc-1333">Ein Problem beim Hochladen von Zertifikaten für in einer ASE gehostete Apps wurde behoben, aufgrund dessen die AS-RG und die App-RG nicht übereinstimmten.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1333">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="aa5bc-1334">`webapp up` wurde geändert, sodass SKU P1V1 als Standard für Linux verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1334">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="aa5bc-1335">`[webapp|functionapp] deployment source config-zip` wurde korrigiert, sodass beim Fehlschlagen einer Bereitstellung die richtige Fehlermeldung angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1335">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="aa5bc-1336">Befehl `webapp ssh` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1336">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="aa5bc-1337">Botservice</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1337">Botservice</span></span>
* <span data-ttu-id="aa5bc-1338">Aktualisierungen des Bereitstellungsstatus wurden zu `bot create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1338">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="aa5bc-1339">Konfigurieren</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1339">Configure</span></span>
* <span data-ttu-id="aa5bc-1340">`none` wurde als konfigurierbares Ausgabeformat hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1340">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="aa5bc-1341">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1341">CosmosDB</span></span>
* <span data-ttu-id="aa5bc-1342">Unterstützung für das Erstellen einer Datenbank mit gemeinsam genutztem Durchsatz wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1342">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="aa5bc-1343">HDInsight</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1343">HDInsight</span></span>
* <span data-ttu-id="aa5bc-1344">Befehle zum Verwalten von Anwendungen wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1344">Added commands for managing applications</span></span>
* <span data-ttu-id="aa5bc-1345">Befehle zum Verwalten von Skriptaktionen wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1345">Added commands for managing script actions</span></span>
* <span data-ttu-id="aa5bc-1346">Befehle zum Verwalten von der Operations Management Suite (OMS) wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1346">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="aa5bc-1347">Unterstützung zum Auflisten der regionalen Nutzung wurde zu `hdinsight list-usage` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1347">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="aa5bc-1348">[BREAKING CHANGE] Standardclustertyp wurde aus `hdinsight create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1348">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="aa5bc-1349">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1349">Network</span></span>
* <span data-ttu-id="aa5bc-1350">Argumente `--custom-headers` und `--status-code-ranges` zu `traffic-manager profile [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1350">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="aa5bc-1351">Neue Routingtypen wurden hinzugefügt: Subnetz und MultiValue</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1351">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="aa5bc-1352">Argumente `--custom-headers` und `--subnets` zu `traffic-manager endpoint [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1352">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="aa5bc-1353">Eine Problem wurde behoben, aufgrund dessen die Angabe von `--vnets ""` für `ddos-protection update` einen Fehler verursacht hat.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1353">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="aa5bc-1354">Role</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1354">Role</span></span>
* <span data-ttu-id="aa5bc-1355">[VERALTET] Argument `--password` als veraltet markiert für `create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1355">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="aa5bc-1356">Verwenden Sie stattdessen sichere, von der CLI generierte Kennwörter.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1356">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="aa5bc-1357">Sicherheit</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1357">Security</span></span>
* <span data-ttu-id="aa5bc-1358">Erstrelease</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1358">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="aa5bc-1359">Storage</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1359">Storage</span></span>
* <span data-ttu-id="aa5bc-1360">[BREAKING CHANGE] Die Standardanzahl von Ergebnissen wurde für `storage [blob|file|container|share] list` in 5.000 geändert.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1360">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="aa5bc-1361">Verwenden Sie `--num-results *` für das ursprüngliche Verhalten, alle Ergebnisse zurückzugeben.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1361">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="aa5bc-1362">Parameter `--marker` zu `storage [blob|file|container|share] list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1362">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="aa5bc-1363">Ein Protokollmarker für die nächste Seite wurde zur STDERR für `storage [blob|file|container|share] list` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1363">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="aa5bc-1364">Der Befehl `storage blob service-properties update` mit Unterstützung für statische Websites wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1364">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="aa5bc-1365">VM</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1365">VM</span></span>
* <span data-ttu-id="aa5bc-1366">`vm [disk|unmanaged-disk]` und `vmss disk` wurden geändert, sodass sie konsistentere Parameter enthalten.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1366">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="aa5bc-1367">Unterstützung für mandantenübergreifende Imageverweise wurden zu `[vm|vmss] create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1367">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="aa5bc-1368">Fehler bei Standardkonfiguration in `vm diagnostics get-default-config --windows-os` wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1368">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="aa5bc-1369">Argument `--provision-after-extensions` wurde zu `vmss extension set` hinzugefügt, um zu definieren, welche Erweiterungen vor dem Festlegen der Erweiterung bereitgestellt werden müssen.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1369">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="aa5bc-1370">Argument `--replica-count` wurde zu `sig image-version update` hinzugefügt, um die Standardanzahl für die Replikation festzulegen.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1370">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="aa5bc-1371">Fehler bei `image create --source` wurde behoben, aufgrund dessen, der Quellbetriebssystem-Datenträger für einen virtuellen Computer mit dem gleichen Namen gehalten wurde, selbst wenn die vollständige Ressourcen-ID angegeben war.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1371">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="aa5bc-1372">20. Dezember 2018</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1372">December 20, 2018</span></span>

<span data-ttu-id="aa5bc-1373">Version 2.0.54</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1373">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="aa5bc-1374">AppService</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1374">Appservice</span></span>
* <span data-ttu-id="aa5bc-1375">Problem behoben, bei dem `webapp up` nicht erneut bereitgestellt werden konnte</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1375">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="aa5bc-1376">Unterstützung für das Auflisten und Wiederherstellen von Web-App-Momentaufnahmen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1376">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="aa5bc-1377">Unterstützung für das Flag `--runtime` zu Windows-Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1377">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="aa5bc-1378">IoTCentral</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1378">IoTCentral</span></span>
* <span data-ttu-id="aa5bc-1379">Fehler bei API-Aufruf für update-Befehl behoben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1379">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="aa5bc-1380">Role</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1380">Role</span></span>
* <span data-ttu-id="aa5bc-1381">[BREAKING CHANGE]`ad [app|sp] list` geändert, damit standardmäßig nur die ersten 100 Objekte aufgelistet werden</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1381">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="aa5bc-1382">SQL</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1382">SQL</span></span>
* <span data-ttu-id="aa5bc-1383">Unterstützung für die benutzerdefinierte Sortierung auf verwalteten Instanzen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1383">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="aa5bc-1384">VM</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1384">VM</span></span>
* <span data-ttu-id="aa5bc-1385">Parameter `---os-type` zu `disk create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1385">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="aa5bc-1386">18. Dezember 2018</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1386">December 18, 2018</span></span>

<span data-ttu-id="aa5bc-1387">Version 2.0.53</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1387">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="aa5bc-1388">ACR</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1388">ACR</span></span>
* <span data-ttu-id="aa5bc-1389">Unterstützung für Imageimport aus externen Containerregistrierungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1389">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="aa5bc-1390">Tabellenlayout für Aufgabenliste komprimiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1390">Condensed the table layout for task list</span></span>
* <span data-ttu-id="aa5bc-1391">Unterstützung für Azure DevOps-URLs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1391">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="aa5bc-1392">ACS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1392">ACS</span></span>
* <span data-ttu-id="aa5bc-1393">Virtuelle Knoten (Vorschau) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1393">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="aa5bc-1394">„(PREVIEW)“ aus AAD-Argumenten für `aks create` entfernt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1394">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="aa5bc-1395">[VERALTET]`az acs`-Befehle als veraltet markiert.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1395">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="aa5bc-1396">ACS wird am 31. Januar 2020 eingestellt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1396">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="aa5bc-1397">Unterstützung für Netzwerkrichtlinie bei der Erstellung neuer AKS-Cluster hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1397">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="aa5bc-1398">Anforderung des Arguments `--nodepool-name` bei nur einem Knotenpool für `aks scale` entfernt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1398">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="aa5bc-1399">AppService</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1399">Appservice</span></span>
* <span data-ttu-id="aa5bc-1400">Problem behoben, bei dem für `webapp config container` der Parameter `--slot` nicht berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1400">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="aa5bc-1401">Botservice</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1401">Botservice</span></span>
* <span data-ttu-id="aa5bc-1402">Unterstützung für Analyse von `.bot`-Dateien beim Aufrufen von `bot show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1402">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="aa5bc-1403">Fehler bei der AppInsights-Bereitstellung behoben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1403">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="aa5bc-1404">Leerzeichenfehler bei Dateipfaden behoben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1404">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="aa5bc-1405">Kudu-Netzwerkaufrufe reduziert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1405">Reduced Kudu network calls</span></span>
* <span data-ttu-id="aa5bc-1406">Allgemeine Verbesserungen bei Befehlen der Benutzeroberfläche durchgeführt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1406">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="aa5bc-1407">Nutzung</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1407">Consumption</span></span>
* <span data-ttu-id="aa5bc-1408">Fehler für Budget-API zum Anzeigen von Benachrichtigungen behoben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1408">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="aa5bc-1409">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1409">CosmosDB</span></span>
* <span data-ttu-id="aa5bc-1410">Unterstützung für die Aktualisierung des Kontos von „Singlemaster“ auf „Multimaster“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1410">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="aa5bc-1411">Karten</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1411">Maps</span></span>
* <span data-ttu-id="aa5bc-1412">Unterstützung für SKU „S1“ für `maps account [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1412">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="aa5bc-1413">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1413">Network</span></span>
* <span data-ttu-id="aa5bc-1414">Unterstützung für `--format` und `--log-version` für `watcher flow-log configure` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1414">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="aa5bc-1415">Problem mit `dns zone update` behoben, bei dem die Verwendung von "" zum Löschen von Auflösungs- und Registrierungs-VNETs nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1415">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="aa5bc-1416">Resource</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1416">Resource</span></span>
* <span data-ttu-id="aa5bc-1417">Verarbeitung des Bereichsparameters für Verwaltungsgruppen in `policy assignment [create|list|delete|show|update]` behoben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1417">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="aa5bc-1418">Neuen Befehl `resource wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1418">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="aa5bc-1419">Storage</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1419">Storage</span></span>
*  <span data-ttu-id="aa5bc-1420">Möglichkeit zum Aktualisieren der Protokollschemaversion für Speicherdienste in `storage logging update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1420">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="aa5bc-1421">VM</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1421">VM</span></span>
* <span data-ttu-id="aa5bc-1422">Absturz in `vm identity remove` behoben, der aufgetreten ist, wenn der angegebenen VM keine verwalteten Dienstidentitäten zugewiesen waren</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1422">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="aa5bc-1423">4\. Dezember 2018</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1423">December 4, 2018</span></span>

<span data-ttu-id="aa5bc-1424">Version 2.0.52</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1424">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="aa5bc-1425">Core</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1425">Core</span></span>
* <span data-ttu-id="aa5bc-1426">Unterstützung für mandantenübergreifende Ressourcenbereitstellung für mehrinstanzenfähigen Dienstprinzipal hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1426">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="aa5bc-1427">Behebung eines Fehlers, aufgrund dessen IDs, die von einem Befehl mit Ausgabe im TSV-Format weitergeleitet wurden, nicht ordnungsgemäß analysiert wurden</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1427">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="aa5bc-1428">AppService</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1428">Appservice</span></span>
* <span data-ttu-id="aa5bc-1429">[VORSCHAU] Befehl `webapp up` hinzugefügt, der Benutzer beim Erstellen und Bereitstellen von Inhalten in Apps unterstützt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1429">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="aa5bc-1430">Behebung eines Fehlers in einer containerbasierten Windows-App, der aufgrund einer Back-End-Änderung auftrat</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1430">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="aa5bc-1431">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1431">Network</span></span>
* <span data-ttu-id="aa5bc-1432">Argument `--exclusion` zu `application-gateway waf-config set` hinzugefügt, um WAF-Ausschlüsse zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1432">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="aa5bc-1433">Role</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1433">Role</span></span>
* <span data-ttu-id="aa5bc-1434">Unterstützung für benutzerdefinierte Bezeichner für Kennwortanmeldeinformation hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1434">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="aa5bc-1435">VM</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1435">VM</span></span>
* <span data-ttu-id="aa5bc-1436">[VERALTET] Parameter `vm extension [show|wait] --expand` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1436">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="aa5bc-1437">Parameter `--force` zu `vm restart` hinzugefügt, um nicht reagierende virtuelle Computer erneut bereitzustellen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1437">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="aa5bc-1438">`[vm|vmss] create --authentication-type` geändert, um „all“ zu akzeptieren und einen virtuellen Computer mit Kennwort- und SSH-Authentifizierung zu erstellen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1438">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="aa5bc-1439">Parameter `image create --os-disk-caching` hinzugefügt, um die Zwischenspeicherung von Betriebssystemdatenträgern für ein Image festzulegen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1439">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="aa5bc-1440">20. November 2018</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1440">November 20, 2018</span></span>

<span data-ttu-id="aa5bc-1441">Version 2.0.51</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1441">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="aa5bc-1442">Core</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1442">Core</span></span>
* <span data-ttu-id="aa5bc-1443">MSI-Anmeldung geändert, sodass der Abonnementname nicht in der Identität wiederverwendet wird</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1443">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="aa5bc-1444">ACR</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1444">ACR</span></span>
* <span data-ttu-id="aa5bc-1445">Kontexttoken zum Aufgabenschritt hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1445">Added context token to task step</span></span>
* <span data-ttu-id="aa5bc-1446">Unterstützung für das Festlegen von Geheimnissen in „acr run“ zum Spiegeln der ACR-Aufgabe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1446">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="aa5bc-1447">Unterstützung für `--top` und `--orderby` für die Befehle `show-tags` und `show-manifests` verbessert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1447">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="aa5bc-1448">AppService</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1448">Appservice</span></span>
* <span data-ttu-id="aa5bc-1449">Standardtimeout der ZIP-Bereitstellung für das Abrufen des Status auf fünf Minuten erhöht und Timeout-Eigenschaft zum Anpassen dieses Werts hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1449">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="aa5bc-1450">Aktualisierung der standardmäßigen `node_version`.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1450">Updated the default `node_version`.</span></span> <span data-ttu-id="aa5bc-1451">Während eines Austauschvorgangs mit zwei Phasen werden bei der Austauschaktion zum Zurücksetzen des Slots alle App-Einstellungen und Verbindungszeichenfolgen beibehalten.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1451">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="aa5bc-1452">Clientseitige SKU-Überprüfung für die Erstellung eines Linux-App Service-Plans entfernt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1452">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="aa5bc-1453">Behebung eines Fehlers beim Abrufen des ZipDeploy-Status</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1453">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="aa5bc-1454">IotCentral</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1454">IotCentral</span></span>
* <span data-ttu-id="aa5bc-1455">Verfügbarkeitsprüfung für Unterdomänen beim Erstellen einer IoT Central-Anwendung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1455">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="aa5bc-1456">KeyVault</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1456">KeyVault</span></span>
* <span data-ttu-id="aa5bc-1457">Behebung eines Fehlers, aufgrund dessen Fehler mitunter ignoriert wurden</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1457">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="aa5bc-1458">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1458">Network</span></span>
* <span data-ttu-id="aa5bc-1459">`root-cert`-Unterbefehle zum Behandeln von vertrauenswürdigen Stammzertifikaten zu `application-gateway` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1459">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="aa5bc-1460">Optionen `--min-capacity` und `--custom-error-pages` zu `application-gateway [create|update]` hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1460">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="aa5bc-1461">`--zones` zur Unterstützung von Verfügbarkeitszonen zu `application-gateway create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1461">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="aa5bc-1462">Argumente `--file-upload-limit`, `--max-request-body-size` und `--request-body-check` zu `application-gateway waf-config set` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1462">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="aa5bc-1463">Rdbms</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1463">Rdbms</span></span>
* <span data-ttu-id="aa5bc-1464">MariaDB-VNET-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1464">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="aa5bc-1465">RBAC</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1465">Rbac</span></span>
* <span data-ttu-id="aa5bc-1466">Problem beim Aktualisieren unveränderlicher Anmeldeinformationen in `ad app update` behoben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1466">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="aa5bc-1467">Ausgabewarnungen zur Ankündigung bevorstehender Breaking Changes für `ad [app|sp] list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1467">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="aa5bc-1468">Storage</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1468">Storage</span></span>
* <span data-ttu-id="aa5bc-1469">Behandlung von Ausnahmefällen für Speicherkopierbefehle verbessert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1469">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="aa5bc-1470">Problem behoben, aufgrund dessen `storage blob copy start-batch` bei identischen Ziel- und Quellkonten keine Anmeldeinformationen verwendete</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1470">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="aa5bc-1471">Fehler bei `storage [blob|file] url` behoben, aufgrund dessen `sas_token` nicht in die URL eingebunden wurde</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1471">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="aa5bc-1472">Breaking Change-Warnung zu `[blob|container] list` hinzugefügt: In Kürze werden standardmäßig nur die ersten 5.000 Ergebnisse ausgegeben.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1472">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="aa5bc-1473">VM</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1473">VM</span></span>
* <span data-ttu-id="aa5bc-1474">Unterstützung für die separate Angabe einer Speicherkonto-SKU für verwaltete Betriebssystemdatenträger und Datenträger zu `[vm|vmss] create --storage-sku` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1474">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="aa5bc-1475">Parameter für den Versionsnamen von `sig image-version` in `--image-version -e` geändert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1475">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="aa5bc-1476">`sig image-version`-Argument `--image-version-name` als veraltet markiert und durch `--image-version` ersetzt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1476">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="aa5bc-1477">Unterstützung für die Verwendung des lokalen Betriebssystemdatenträgers für `[vm|vmss] create --ephemeral-os-disk` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1477">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="aa5bc-1478">Unterstützung für `--no-wait` zu `snapshot create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1478">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="aa5bc-1479">Befehl `snapshot wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1479">Added `snapshot wait` command</span></span>
* <span data-ttu-id="aa5bc-1480">Unterstützung für die Verwendung von Instanznamen mit `[vm|vmss] extension set --extension-instance-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1480">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="aa5bc-1481">6\. November 2018</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1481">November 6, 2018</span></span>

<span data-ttu-id="aa5bc-1482">Version 2.0.50</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1482">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="aa5bc-1483">Core</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1483">Core</span></span>
* <span data-ttu-id="aa5bc-1484">Unterstützung für die Dienstprinzipalauthentifizierung (SN und Aussteller) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1484">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="aa5bc-1485">ACR</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1485">ACR</span></span>
* <span data-ttu-id="aa5bc-1486">Unterstützung für Commit- und Pull Request-Git-Ereignisse für Aufgabenquellentrigger hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1486">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="aa5bc-1487">Auf Verwendung des Standard-Dockerfiles umgestellt, falls im Erstellungsbefehl kein Dockerfile angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1487">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="aa5bc-1488">ACS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1488">ACS</span></span>
* <span data-ttu-id="aa5bc-1489">[BREAKING CHANGE]`enable_cloud_console_aks_browse` entfernt, um standardmäßig „az aks browse“ zu aktivieren</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1489">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="aa5bc-1490">Advisor</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1490">Advisor</span></span>
* <span data-ttu-id="aa5bc-1491">Allgemein verfügbares Release</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1491">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="aa5bc-1492">AMS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1492">AMS</span></span>
* <span data-ttu-id="aa5bc-1493">Neue Befehlsgruppen hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1493">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="aa5bc-1494">Neue Befehle hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1494">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="aa5bc-1495">Unterstützung von Verschlüsselungsparametern für `ams streaming-policy create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1495">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="aa5bc-1496">Für `ams transform output remove` kann jetzt der zu entfernende Ausgabeindex angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1496">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="aa5bc-1497">Argumente `--correlation-data` und `--label` zur Befehlsgruppe `ams job` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1497">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="aa5bc-1498">Argumente `--storage-account` und `--container` zur Befehlsgruppe `ams asset` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1498">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="aa5bc-1499">Standardwerte für Ablaufzeit (aktueller Zeitpunkt + 23 Std.) und Berechtigungen (Lesen) im Befehl `ams asset get-sas-url` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1499">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="aa5bc-1500">[BREAKING CHANGE] Befehl `ams streaming locator` durch `ams streaming-locator` ersetzt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1500">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="aa5bc-1501">[BREAKING CHANGE] Argument `--content-keys` von `ams streaming locator` aktualisiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1501">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="aa5bc-1502">[BREAKING CHANGE]`--content-policy-name` im Befehl `ams streaming locator` in `--content-key-policy-name` umbenannt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1502">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="aa5bc-1503">[BREAKING CHANGE] Befehl `ams streaming policy` durch `ams streaming-policy` ersetzt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1503">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="aa5bc-1504">[BREAKING CHANGE] Das Argument `--preset-names` wurde in der Befehlsgruppe `--preset` durch `ams transform` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1504">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="aa5bc-1505">Ab sofort kann nur noch eine einzelne Ausgabe/Voreinstellung festgelegt werden. (Wenn Sie weitere hinzufügen möchten, müssen Sie `ams transform output add` ausführen.)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1505">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="aa5bc-1506">Darüber hinaus können Sie eine benutzerdefinierte Voreinstellung für den Standard-Encoder (StandardEncoderPreset) festlegen, indem Sie den Pfad an Ihr benutzerdefiniertes JSON-Objekt übergeben.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1506">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="aa5bc-1507">[BREAKING CHANGE]`--output-asset-names ` wurde im Befehl `ams job start` in `--output-assets` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1507">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="aa5bc-1508">Ab sofort wird eine durch Leerzeichen getrennte Ressourcenliste im Format „assetName=Bezeichnung“ akzeptiert.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1508">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="aa5bc-1509">Ressourcen ohne Bezeichnung können wie folgt gesendet werden: „assetName=“.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1509">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="aa5bc-1510">AppService</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1510">AppService</span></span>
* <span data-ttu-id="aa5bc-1511">Fehler in `az webapp config backup update` behoben, der dazu führte, dass kein Sicherungszeitplan festgelegt werden konnte, wenn noch keiner festgelegt war</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1511">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="aa5bc-1512">Konfigurieren</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1512">Configure</span></span>
* <span data-ttu-id="aa5bc-1513">YAML zu Ausgabeformatoptionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1513">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="aa5bc-1514">Container</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1514">Container</span></span>
* <span data-ttu-id="aa5bc-1515">Auf Anzeige der Identität umgestellt, wenn eine Containergruppe nach YAML exportiert wird</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1515">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="aa5bc-1516">EventHub</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1516">EventHub</span></span>
* <span data-ttu-id="aa5bc-1517">Flag `--enable-kafka` hinzugefügt, um Kafka in `eventhub namespace [create|update]` zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1517">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="aa5bc-1518">Interactive</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1518">Interactive</span></span>
* <span data-ttu-id="aa5bc-1519">Interactive installiert nun die Erweiterung `interactive`, um schnellere Updates und schnelleren Support zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1519">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="aa5bc-1520">Überwachen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1520">Monitor</span></span>
* <span data-ttu-id="aa5bc-1521">Unterstützung für Metriknamen mit Schrägstrichen und Punkten zu `--condition` in `monitor metrics alert [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1521">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="aa5bc-1522">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1522">Network</span></span>
* <span data-ttu-id="aa5bc-1523">Befehlsnamen vom Typ `network interface-endpoint` zugunsten von `network private-endpoint` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1523">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="aa5bc-1524">Problem behoben, das dazu führte, dass das Argument `--peer-circuit` in `express-route peering connection create` keine ID akzeptiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1524">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="aa5bc-1525">Problem behoben, das dazu führte, dass `--ip-tags` mit `public-ip create` nicht ordnungsgemäß funktioniert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1525">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="aa5bc-1526">Profil</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1526">Profile</span></span>
* <span data-ttu-id="aa5bc-1527">`--use-cert-sn-issuer` zu `az login` hinzugefügt, um Dienstprinzipalanmeldungen mit automatischem Zertifikatrollover zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1527">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="aa5bc-1528">RDBMS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1528">RDBMS</span></span>
* <span data-ttu-id="aa5bc-1529">MySQL-Replikatbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1529">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="aa5bc-1530">Resource</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1530">Resource</span></span>
* <span data-ttu-id="aa5bc-1531">Unterstützung für Verwaltungsgruppen und Abonnements zu Befehlen vom Typ `policy definition|set-definition` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1531">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="aa5bc-1532">Role</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1532">Role</span></span>
* <span data-ttu-id="aa5bc-1533">Unterstützung für die API-Berechtigungsverwaltung, den angemeldeten Benutzer und die Verwaltung von Anwendungskennwörtern und Zertifikatanmeldeinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1533">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="aa5bc-1534">`ad sp create-for-rbac` geändert, um „displayName“ und Dienstprinzipalname besser unterscheiden zu können</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1534">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="aa5bc-1535">Unterstützung der Gewährung von Berechtigungen für AAD-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1535">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="aa5bc-1536">Storage</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1536">Storage</span></span>
* <span data-ttu-id="aa5bc-1537">Möglichkeit hinzugefügt, allein mit SAS und Endpunkten (ohne Kontoname oder Schlüssel) eine Verbindung mit Speicherdiensten herzustellen, wie unter `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>` beschrieben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1537">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="aa5bc-1538">VM</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1538">VM</span></span>
* <span data-ttu-id="aa5bc-1539">Argument `storage-sku` zu `image create` hinzugefügt, um das Festlegen des standardmäßigen Speicherkontotyps für das Image zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1539">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="aa5bc-1540">Fehler für `vm resize` behoben, durch den die Option `--no-wait` einen Absturz des Befehls verursachte</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1540">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="aa5bc-1541">Tabellenausgabeformat für `vm encryption show` geändert, um den Status anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1541">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="aa5bc-1542">`vm secret format` geändert, um JSON/JSONC-Ausgabe erforderlich zu machen.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1542">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="aa5bc-1543">Der Benutzer wird gewarnt, und es wird standardmäßig die JSON-Ausgabe verwendet, wenn ein unzulässiges Ausgabeformat ausgewählt wird.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1543">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="aa5bc-1544">Argumentüberprüfung für `vm create --image` verbessert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1544">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="aa5bc-1545">23. Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1545">October 23, 2018</span></span>

<span data-ttu-id="aa5bc-1546">Version 2.0.49</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1546">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="aa5bc-1547">Core</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1547">Core</span></span>
* <span data-ttu-id="aa5bc-1548">Problem mit `--ids` behoben, aufgrund dessen `--subscription` Vorrang vor dem Abonnement in `--ids` hatte</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1548">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="aa5bc-1549">Ausdrückliche Warnungen hinzugefügt, wenn Parameter durch die Verwendung von `--ids` ignoriert würden</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1549">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="aa5bc-1550">ACR</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1550">ACR</span></span>
* <span data-ttu-id="aa5bc-1551">Problem mit der ACR Build-Codierung in Python2 behoben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1551">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="aa5bc-1552">CDN</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1552">CDN</span></span>
* <span data-ttu-id="aa5bc-1553">[BREAKING CHANGE] Standardverhalten beim Zwischenspeichern der Abfragezeichenfolge von `cdn endpoint create` so geändert, dass der Standardwert nicht mehr „IgnoreQueryString“ ist.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1553">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="aa5bc-1554">Er wird jetzt vom Dienst festgelegt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1554">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="aa5bc-1555">Container</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1555">Container</span></span>
* <span data-ttu-id="aa5bc-1556">`Private` als gültiger Typ für die Übergabe an „--ip-address“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1556">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="aa5bc-1557">Geändert, sodass nur eine Subnetz-ID für das Einrichten eines virtuellen Netzwerks für die Containergruppe zulässig ist</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1557">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="aa5bc-1558">Geändert, sodass das Verwenden eines VNET-Namens oder einer Ressourcen-ID zulässig ist, um die Verwendung von VNETs aus verschiedenen Ressourcengruppen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1558">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="aa5bc-1559">`--assign-identity` hinzugefügt, um einer Containergruppe eine MSI-Identität hinzuzufügen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1559">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="aa5bc-1560">`--scope` hinzugefügt, um eine Rollenzuweisung für die vom System zugewiesene MSI-Identität zu erstellen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1560">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="aa5bc-1561">Warnung hinzugefügt, wenn eine Containergruppe mit einem Image ohne Prozess mit langer Ausführungszeit erstellt wird</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1561">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="aa5bc-1562">Probleme mit der Tabellenausgabe für Befehle `list` und `show` behoben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1562">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="aa5bc-1563">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1563">CosmosDB</span></span>
* <span data-ttu-id="aa5bc-1564">Unterstützung für `--enable-multiple-write-locations` zu `cosmosdb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1564">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="aa5bc-1565">Interactive</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1565">Interactive</span></span>
* <span data-ttu-id="aa5bc-1566">Geändert, um sicherzustellen, dass der Parameter für globales Abonnement in Parametern angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1566">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="aa5bc-1567">IoT Central</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1567">IoT Central</span></span>
* <span data-ttu-id="aa5bc-1568">Optionen für Vorlagen und Anzeigenamen für die Erstellung von IoT Central-Anwendungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1568">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="aa5bc-1569">[BREAKING CHANGE] Unterstützung für F1-SKU entfernt; stattdessen ist die S1-SKU zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1569">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="aa5bc-1570">Überwachen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1570">Monitor</span></span>
* <span data-ttu-id="aa5bc-1571">Änderungen an `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1571">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="aa5bc-1572">Unterstützung für das Auflisten aller Ereignisse auf Abonnementebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1572">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="aa5bc-1573">`--offset`-Parameter für das einfachere Erstellen von Zeitabfragen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1573">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="aa5bc-1574">Validierung für `--start-time` und `--end-time` verbessert, um die Verwendung von mehr ISO8601-Formate und benutzerfreundlicheren datetime-Formaten zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1574">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="aa5bc-1575">`--namespace` als Alias für veraltete Option `--resource-provider` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1575">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="aa5bc-1576">`--filters` als veraltet markiert, da vom Dienst ausschließlich Werte mit stark typisierten Optionen unterstützt werden</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1576">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="aa5bc-1577">Änderungen an `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1577">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="aa5bc-1578">`--offset`-Parameter für das einfachere Erstellen von Zeitabfragen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1578">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="aa5bc-1579">Validierung für `--start-time` und `--end-time` verbessert, um die Verwendung von mehr ISO8601-Formate und benutzerfreundlicheren datetime-Formaten zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1579">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="aa5bc-1580">Validierung für `--event-hub`- und `--event-hub-rule`-Argumente an `monitor diagnostic-settings create` verbessert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1580">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="aa5bc-1581">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1581">Network</span></span>
* <span data-ttu-id="aa5bc-1582">`--app-gateway-address-pools`- und `--gateway-name`-Argumente zu `nic create` hinzugefügt, um das Hinzufügen von Back-End-Adresspools für Anwendungsgateways zu einer NIC zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1582">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="aa5bc-1583">`--app-gateway-address-pools`- und `--gateway-name`-Argumente zu `nic ip-config create/update` hinzugefügt, um das Hinzufügen von Back-End-Adresspools für Anwendungsgateways zu einer NIC zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1583">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="aa5bc-1584">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1584">ServiceBus</span></span>
* <span data-ttu-id="aa5bc-1585">Schreibgeschütztes `migration_state`-Element zu „MigrationConfigProperties“ hinzugefügt, um den aktuellen Status der Migration von Service Bus Standard- zu Premium-Namespace anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1585">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="aa5bc-1586">SQL</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1586">SQL</span></span>
* <span data-ttu-id="aa5bc-1587">`sql failover-group create` und `sql failover-group update` korrigiert, damit die Verwendung einer Richtlinie für manuelles Failover möglich ist</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1587">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="aa5bc-1588">Storage</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1588">Storage</span></span>
* <span data-ttu-id="aa5bc-1589">Formatierung der `az storage cors list`-Ausgabe korrigiert, sodass alle Elemente den richtigen Dienstschlüssel anzeigen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1589">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="aa5bc-1590">`--bypass-immutability-policy`-Parameter für das Löschen von durch Unveränderlichkeitsrichtlinien blockierten Containern hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1590">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="aa5bc-1591">VM</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1591">VM</span></span>
* <span data-ttu-id="aa5bc-1592">Datenträger-Zwischenspeicherungsmodus `None` für Lv/Lv2-Computerserine in `[vm|vmss] create` erzwungen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1592">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="aa5bc-1593">Liste der unterstützten Größen für unterstützenden Netzwerkbeschleuniger für `vm create` aktualisiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1593">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="aa5bc-1594">Stark typisierte Argumente für UltraSSD-IOPS und MBit/s-Konfigurationen für `disk create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1594">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="aa5bc-1595">16. Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1595">October 16, 2018</span></span>

<span data-ttu-id="aa5bc-1596">Version 2.0.48</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1596">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="aa5bc-1597">VM</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1597">VM</span></span>
* <span data-ttu-id="aa5bc-1598">SDK-Problem behoben, das ein Fehlschlagen der Homebrew-Installation verursacht hat</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1598">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="aa5bc-1599">9\. Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1599">October 9, 2018</span></span>

<span data-ttu-id="aa5bc-1600">Version 2.0.47</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1600">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="aa5bc-1601">Core</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1601">Core</span></span>
* <span data-ttu-id="aa5bc-1602">Verbesserte Fehlerbehandlung für Fehler vom Typ „Ungültige Anforderung“</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1602">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="aa5bc-1603">ACR</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1603">ACR</span></span>
* <span data-ttu-id="aa5bc-1604">Unterstützung für ähnliches Tabellenformat wie Helm-Client hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1604">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="aa5bc-1605">ACS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1605">ACS</span></span>
* <span data-ttu-id="aa5bc-1606">`aks [create|scale] --nodepool-name` zum Konfigurieren des Knotenpoolnamens hinzugefügt, auf 12 Zeichen gekürzt, Standard: nodepool1</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1606">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="aa5bc-1607">Korrektur, bei der auf „scp“ zurückgegriffen wird, wenn Parimiko nicht funktioniert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1607">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="aa5bc-1608">`aks create` geändert, sodass `--aad-tenant-id` nicht mehr erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1608">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="aa5bc-1609">Verbesserte Zusammenführung von Kubernetes-Anmeldeinformationen, wenn doppelte Einträge vorhanden sind</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1609">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="aa5bc-1610">Container</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1610">Container</span></span>
* <span data-ttu-id="aa5bc-1611">`functionapp create` geändert, sodass das Erstellen eines Linux-Nutzungsplans mit einer bestimmten Runtime unterstützt wird</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1611">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="aa5bc-1612">[VORSCHAUVERSION] Unterstützung für das Hosten von Web-Apps in Windows-Containern hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1612">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="aa5bc-1613">Event Hub</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1613">Event Hub</span></span>
* <span data-ttu-id="aa5bc-1614">Befehl `eventhub update` korrigiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1614">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="aa5bc-1615">[BREAKING CHANGE]`list`-Befehle geändert, sodass Fehler von Typ „NotFound(404)“ für Ressourcen mit der typische Vorgehensweise behandelt werden, anstatt eine leere Liste anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1615">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="aa5bc-1616">Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1616">Extensions</span></span>
* <span data-ttu-id="aa5bc-1617">Problem beim Hinzufügen einer Erweiterung behoben, die bereits installiert ist</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1617">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="aa5bc-1618">HDInsight</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1618">HDInsight</span></span>
* <span data-ttu-id="aa5bc-1619">Erste Veröffentlichung</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1619">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="aa5bc-1620">IoT</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1620">IoT</span></span>
* <span data-ttu-id="aa5bc-1621">Befehl zur Erweiterungsinstallation zu Banner bei der ersten Ausführung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1621">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="aa5bc-1622">KeyVault</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1622">KeyVault</span></span>
* <span data-ttu-id="aa5bc-1623">Geändert, sodass Key Vault-Speicherbefehle auf das aktuelle API-Profil beschränkt sind</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1623">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="aa5bc-1624">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1624">Network</span></span>
* <span data-ttu-id="aa5bc-1625">`network dns zone create` korrigiert: Befehl ist auch erfolgreich, wenn der Benutzer einen Standardspeicherort konfiguriert hat.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1625">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="aa5bc-1626">Siehe Nr. 6052</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1626">See #6052</span></span>
* <span data-ttu-id="aa5bc-1627">`--remote-vnet-id` für `network vnet peering create` eingestellt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1627">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="aa5bc-1628">`--remote-vnet` zum `network vnet peering create`-Element hinzugefügt, das einen Namen oder eine ID akzeptiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1628">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="aa5bc-1629">Unterstützung für mehrere Subnetzpräfixe zu `network vnet create` in `--subnet-prefixes` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1629">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="aa5bc-1630">Unterstützung für mehrere Subnetzpräfixe zu `network vnet subnet [create|update]` in `--address-prefixes` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1630">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="aa5bc-1631">Problem mit `network application-gateway create` behoben, das die Erstellung von Gateways mit der SKU `WAF_v2` oder `Standard_v2` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1631">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="aa5bc-1632">`--service-endpoint-policy`-Argument für Benutzerfreundlichkeit zu `network vnet subnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1632">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="aa5bc-1633">Role</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1633">Role</span></span>
* <span data-ttu-id="aa5bc-1634">Unterstützung für das Auflisten von Azure AD-App-Besitzern in `ad app owner` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1634">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="aa5bc-1635">Unterstützung für das Auflisten von Azure AD-Dienstprinzipalbesitzern in `ad sp owner` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1635">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="aa5bc-1636">Geändert, um sicherzustellen, dass die Erstellungs- und Aktualisierungsbefehle für die Rollendefinition Konfigurationen mit mehreren Berechtigungen akzeptieren</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1636">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="aa5bc-1637">`ad sp create-for-rbac` geändert, um sicherzustellen, dass der Homepage-URI immer „https“ ist</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1637">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="aa5bc-1638">Service Bus</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1638">Service Bus</span></span>
* <span data-ttu-id="aa5bc-1639">[BREAKING CHANGE]`list`-Befehle geändert, sodass Fehler von Typ „NotFound(404)“ für Ressourcen mit der typische Vorgehensweise behandelt werden, anstatt eine leere Liste anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1639">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="aa5bc-1640">VM</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1640">VM</span></span>
* <span data-ttu-id="aa5bc-1641">Leeres `accessSas`-Feld in `disk grant-access` korrigiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1641">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="aa5bc-1642">`vmss create` geändert, sodass ein ausreichend großer Front-End-Portbereich zur Verarbeitung von Überbereitstellung reserviert ist</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1642">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="aa5bc-1643">Aktualisierungsbefehle für `sig` korrigiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1643">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="aa5bc-1644">`--no-wait`-Unterstützung für die Verwaltung von Imageversionen in `sig` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1644">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="aa5bc-1645">`vm list-ip-addresses` geändert, sodass die Verfügbarkeitszone von öffentlichen IP-Adressen angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1645">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="aa5bc-1646">`[vm|vmss] disk attach` geändert, sodass die Standard-LUN eines Datenträgers standardmäßig auf die erste verfügbare Stelle festgelegt wird</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1646">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="aa5bc-1647">21. September 2018</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1647">September 21, 2018</span></span>

<span data-ttu-id="aa5bc-1648">Version 2.0.46</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1648">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="aa5bc-1649">ACR</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1649">ACR</span></span>
* <span data-ttu-id="aa5bc-1650">ACR-Aufgabenbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1650">Added ACR Task commands</span></span>
* <span data-ttu-id="aa5bc-1651">Befehl für die Schnellausführung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1651">Added quick run command</span></span>
* <span data-ttu-id="aa5bc-1652">`build-task`-Befehlsgruppe als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1652">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="aa5bc-1653">`helm`-Befehlsgruppe hinzugefügt, um die Verwaltung von Helm-Diagrammen mit ACR zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1653">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="aa5bc-1654">Unterstützung für idempotentes Erstellen für die verwaltete Registrierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1654">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="aa5bc-1655">Formatfreies Flag für die Anzeige von Buildprotokollen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1655">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="aa5bc-1656">ACS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1656">ACS</span></span>
* <span data-ttu-id="aa5bc-1657">Befehl `install-connector` zum Festlegen des AKS-Master-FQDN geändert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1657">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="aa5bc-1658">Erstellen der Rollenzuweisung für „vnet-subnet-id“ (wenn kein Dienstprinzipal angegeben wurde) und „skip-role-assignment“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1658">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="aa5bc-1659">AppService</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1659">AppService</span></span>

* <span data-ttu-id="aa5bc-1660">Unterstützung für WebJobs-Vorgangsverwaltung hinzugefügt (kontinuierlich/ausgelöst)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1660">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="aa5bc-1661">„az webapp config set“ unterstützt die Eigenschaft „--fts-state“; Unterstützung für „az functionapp config set/show“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1661">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="aa5bc-1662">Unterstützung für Bring Your Own Storage für Web-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1662">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="aa5bc-1663">Unterstützung für das Auflisten und Wiederherstellen gelöschter Web-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1663">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="aa5bc-1664">Batch</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1664">Batch</span></span>
* <span data-ttu-id="aa5bc-1665">Hinzufügen von Aufgaben über `--json-file` geändert, um die AddTaskCollectionParameter-Syntax zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1665">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="aa5bc-1666">Dokumentation akzeptierter `--json-file`-Formate aktualisiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1666">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="aa5bc-1667">`--max-tasks-per-node-option` zu `batch pool create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1667">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="aa5bc-1668">Verhalten von `batch account` geändert, um das aktuell angemeldete Konto anzuzeigen, wenn keine Optionen angegeben wurden</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1668">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="aa5bc-1669">Batch KI</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1669">Batch AI</span></span> 
* <span data-ttu-id="aa5bc-1670">Fehler bei der automatischen Speicherkontoerstellung im Befehl `batchai cluster create` behoben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1670">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="aa5bc-1671">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1671">Cognitive Services</span></span>
* <span data-ttu-id="aa5bc-1672">Vervollständigung für die Argumente `--sku`, `--kind` und `--location` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1672">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="aa5bc-1673">Befehl `cognitiveservices account list-usage` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1673">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="aa5bc-1674">Befehl `cognitiveservices account list-kinds` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1674">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="aa5bc-1675">Befehl `cognitiveservices account list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1675">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="aa5bc-1676">`cognitiveservices list` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1676">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="aa5bc-1677">`--name` geändert (ist jetzt optional für `cognitiveservices account list-skus`)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1677">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="aa5bc-1678">Container</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1678">Container</span></span>
* <span data-ttu-id="aa5bc-1679">Möglichkeit zum Neustarten und Beenden einer ausgeführten Containergruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1679">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="aa5bc-1680">`--network-profile` zum Übergeben eines Netzwerkprofils hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1680">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="aa5bc-1681">`--subnet` und `--vnet_name` hinzugefügt, um das Erstellen von Containergruppen in einem VNET zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1681">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="aa5bc-1682">Tabellenausgabe geändert, sodass der Status der Containergruppe angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1682">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="aa5bc-1683">Data Lake</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1683">Datalake</span></span>
* <span data-ttu-id="aa5bc-1684">Befehle für VNET-Regeln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1684">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="aa5bc-1685">Interaktive Shell</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1685">Interactive Shell</span></span>
* <span data-ttu-id="aa5bc-1686">Fehler in Windows behoben, durch den Befehle nicht ordnungsgemäß ausgeführt wurden</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1686">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="aa5bc-1687">Durch veraltete Objekte verursachtes Problem beim Laden von Befehlen im interaktiven Modus behoben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1687">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="aa5bc-1688">IoT</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1688">IoT</span></span>
* <span data-ttu-id="aa5bc-1689">Routingunterstützung für IoT Hubs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1689">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="aa5bc-1690">Key Vault</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1690">Key Vault</span></span>
* <span data-ttu-id="aa5bc-1691">Key Vault-Schlüsselimport für RSA-Schlüssel korrigiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1691">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="aa5bc-1692">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1692">Network</span></span>
* <span data-ttu-id="aa5bc-1693">Befehle vom Typ `network public-ip prefix` hinzugefügt, um Präfixe von öffentlichen IP-Adressen zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1693">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="aa5bc-1694">Befehle vom Typ `network service-endpoint` hinzugefügt, um Dienstendpunktrichtlinien-Features zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1694">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="aa5bc-1695">Befehle vom Typ `network lb outbound-rule` hinzugefügt, um die Erstellung von Ausgangsregeln für Load Balancer Standard zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1695">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="aa5bc-1696">`--public-ip-prefix` zu `network lb frontend-ip create/update` hinzugefügt, um Front-End-IP-Konfigurationen mit Präfixen von öffentlichen IP-Adressen zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1696">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="aa5bc-1697">`--enable-tcp-reset` zu `network lb rule/inbound-nat-rule/inbound-nat-pool create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1697">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="aa5bc-1698">`--disable-outbound-snat` zu `network lb rule create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1698">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="aa5bc-1699">Verwendung von `network watcher flow-log show/configure` mit klassischen NSGs ermöglicht</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1699">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="aa5bc-1700">Hinzufügen des `network watcher run-configuration-diagnostic`-Befehls</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1700">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="aa5bc-1701">Befehl `network watcher test-connectivity` korrigiert und Eigenschaften `--method`, `--valid-status-codes` und `--headers` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1701">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="aa5bc-1702">`network express-route create/update`: Flag `--allow-global-reach` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1702">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="aa5bc-1703">`network vnet subnet create/update`: Unterstützung für `--delegation` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1703">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="aa5bc-1704">Befehl `network vnet subnet list-available-delegations` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1704">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="aa5bc-1705">`network traffic-manager profile create/update`: Unterstützung für `--interval`, `--timeout` und `--max-failures` für die Überwachungskonfiguration hinzugefügt; Optionen `--monitor-path`, `--monitor-port` und `--monitor-protocol` zugunsten von `--path`, `--port` und `--protocol` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1705">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="aa5bc-1706">`network lb frontend-ip create/update`: Logik für das Festlegen der Zuweisungsmethode für private IP-Adressen korrigiert. Bei Angabe einer privaten IP-Adresse ist die Zuweisung statisch. Wird keine private IP-Adresse (oder eine leere Zeichenfolge für die private IP-Adresse) angegeben, erfolgt eine dynamische Zuweisung.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1706">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="aa5bc-1707">`dns record-set * create/update`: Unterstützung für `--target-resource` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1707">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="aa5bc-1708">Befehle vom Typ `network interface-endpoint` hinzugefügt, um Schnittstellenendpunkt-Objekte abzufragen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1708">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="aa5bc-1709">`network profile show/list/delete` für die partielle Verwaltung von Netzwerkprofilen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1709">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="aa5bc-1710">Befehle vom Typ `network express-route peering connection` für die Verwaltung von Peeringverbindungen zwischen ExpressRoute-Instanzen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1710">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="aa5bc-1711">RDBMS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1711">RDBMS</span></span>
* <span data-ttu-id="aa5bc-1712">Unterstützung für den MariaDB-Dienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1712">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="aa5bc-1713">Reservierung</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1713">Reservation</span></span>
* <span data-ttu-id="aa5bc-1714">Cosmos DB im Enumerationstyp für reservierte Ressourcen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1714">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="aa5bc-1715">Namenseigenschaft im Patchmodell hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1715">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="aa5bc-1716">App-Verwaltung</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1716">Manage App</span></span>
* <span data-ttu-id="aa5bc-1717">Fehler in `managedapp create --kind MarketPlace` korrigiert, der zum Absturz der Instanzerstellung einer verwalteten Marketplace-App führte</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1717">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="aa5bc-1718">Befehle vom Typ `feature` geändert, um sie auf unterstützte Profile zu beschränken</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1718">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="aa5bc-1719">Role</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1719">Role</span></span>
* <span data-ttu-id="aa5bc-1720">Unterstützung für das Auflisten der Gruppenmitgliedschaften des Benutzers hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1720">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="aa5bc-1721">SignalR</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1721">SignalR</span></span>
* <span data-ttu-id="aa5bc-1722">Erste Version</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1722">First release</span></span>

### <a name="storage"></a><span data-ttu-id="aa5bc-1723">Storage</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1723">Storage</span></span>
* <span data-ttu-id="aa5bc-1724">Parameter `--auth-mode login` für die Verwendung der Anmeldeinformationen des Benutzers für die Blob- und Warteschlangenautorisierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1724">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="aa5bc-1725">`storage container immutability-policy/legal-hold` für die Verwaltung von unveränderlichem Speicher hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1725">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="aa5bc-1726">VM</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1726">VM</span></span>
* <span data-ttu-id="aa5bc-1727">Problem behoben, das dazu führte, dass die Datei mit dem privaten Schlüssel durch `vm create --generate-ssh-keys` überschrieben wird, wenn die Datei mit dem privaten Schlüssel fehlt (Nr. 4725, 6780)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1727">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="aa5bc-1728">Unterstützung für den gemeinsamen Image-Katalog über `az sig` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1728">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="aa5bc-1729">28. August 2018</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1729">August 28, 2018</span></span>

<span data-ttu-id="aa5bc-1730">Version 2.0.45</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1730">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="aa5bc-1731">Core</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1731">Core</span></span>

* <span data-ttu-id="aa5bc-1732">Das Problem, aufgrund dessen eine leere Konfigurationsdatei geladen wurde, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1732">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="aa5bc-1733">Unterstützung für Profil `2018-03-01-hybrid` für Azure Stack hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1733">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="aa5bc-1734">ACR</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1734">ACR</span></span>

* <span data-ttu-id="aa5bc-1735">Problemumgehung für Laufzeitvorgänge ohne ARM-Anforderungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1735">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="aa5bc-1736">Änderung vorgenommen, um im Befehl `build` Versionskontrolldateien (etwa „.git“ und „.gitignore“) standardmäßig aus der TAR-Datei auszuschließen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1736">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="aa5bc-1737">ACS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1737">ACS</span></span>

* <span data-ttu-id="aa5bc-1738">`aks create` geändert, dass standardmäßig virtuelle Computer vom Typ `Standard_DS2_v2` erstellt werden</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1738">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="aa5bc-1739">`aks get-credentials` geändert, um nun neue APIs zum Abrufen der Clusteranmeldeinformationen aufzurufen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1739">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="aa5bc-1740">AppService</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1740">AppService</span></span>

* <span data-ttu-id="aa5bc-1741">Unterstützung für CORS in „functionapp“ und „webapp“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1741">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="aa5bc-1742">ARM-Tagunterstützung in Erstellungsbefehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1742">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="aa5bc-1743">`[webapp|functionapp] identity show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1743">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="aa5bc-1744">Backup</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1744">Backup</span></span>

* <span data-ttu-id="aa5bc-1745">`backup vault backup-properties show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1745">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="aa5bc-1746">Botdienst</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1746">Bot Service</span></span>

* <span data-ttu-id="aa5bc-1747">Anfängliches Release der Botdienst-CLI</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1747">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="aa5bc-1748">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1748">Cognitive Services</span></span>

* <span data-ttu-id="aa5bc-1749">Neuer Parameter `--api-properties,` hinzugefügt, der zum Erstellen einiger Dienste erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1749">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="aa5bc-1750">IoT</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1750">IoT</span></span>

* <span data-ttu-id="aa5bc-1751">Problem mit dem Zuweisen verknüpfter Hubs behoben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1751">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="aa5bc-1752">Überwachen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1752">Monitor</span></span>

* <span data-ttu-id="aa5bc-1753">`monitor metrics alert`-Befehle für Metrikwarnungen nahezu in Echtzeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1753">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="aa5bc-1754">`monitor alert`-Befehle als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1754">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="aa5bc-1755">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1755">Network</span></span>

* <span data-ttu-id="aa5bc-1756">`network application-gateway ssl-policy predefined show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1756">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="aa5bc-1757">Resource</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1757">Resource</span></span>

* <span data-ttu-id="aa5bc-1758">`provider operation show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1758">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="aa5bc-1759">Storage</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1759">Storage</span></span>

* <span data-ttu-id="aa5bc-1760">`storage share policy show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1760">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="aa5bc-1761">VM</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1761">VM</span></span>

* <span data-ttu-id="aa5bc-1762">`vm/vmss identity show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1762">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="aa5bc-1763">`--storage-caching` für `vm create` eingestellt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1763">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="aa5bc-1764">14. August 2018</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1764">Auguest 14, 2018</span></span>

<span data-ttu-id="aa5bc-1765">Version 2.0.44</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1765">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="aa5bc-1766">Core</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1766">Core</span></span>

* <span data-ttu-id="aa5bc-1767">Numerische Anzeige in `table`-Ausgabe korrigiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1767">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="aa5bc-1768">YAML-Ausgabeformat hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1768">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="aa5bc-1769">Telemetrie</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1769">Telemetry</span></span>

* <span data-ttu-id="aa5bc-1770">Verbesserte Berichterstellung für Telemetriedaten</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1770">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="aa5bc-1771">ACR</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1771">ACR</span></span>

* <span data-ttu-id="aa5bc-1772">Befehle vom Typ `content-trust policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1772">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="aa5bc-1773">Problem behoben, aufgrund dessen `.dockerignore` nicht richtig verarbeitet wurde</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1773">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="aa5bc-1774">ACS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1774">ACS</span></span>

* <span data-ttu-id="aa5bc-1775">`az acs/aks install-cli` für die Installation in `%USERPROFILE%\.azure-kubectl` unter Windows geändert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1775">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="aa5bc-1776">`az aks install-connector` geändert, um zu ermitteln, ob der Cluster über RBAC verfügt, und um den ACI-Connector entsprechend zu konfigurieren</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1776">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="aa5bc-1777">Geändert in Rollenzuweisung zum Subnetz bei entsprechender Angabe</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1777">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="aa5bc-1778">Neue Option zum Überspringen der Rollenzuweisung für Subnetz hinzugefügt, wenn dieses angegeben ist</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1778">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="aa5bc-1779">Geändert, um Rollenzuweisung zum Subnetz zu überspringen, wenn bereits eine Zuweisung vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1779">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="aa5bc-1780">AppService</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1780">AppService</span></span>

* <span data-ttu-id="aa5bc-1781">Fehler behoben, der das Erstellen einer Funktions-App mithilfe von Speicherkonten in externen Ressourcengruppen verhinderte</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1781">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="aa5bc-1782">Absturz bei ZIP-Bereitstellung behoben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1782">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="aa5bc-1783">Batch AI</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1783">BatchAI</span></span>

* <span data-ttu-id="aa5bc-1784">Protokollierungsausgabe für die automatische Speicherkontoerstellung geändert, sodass nun „Ressourcen*gruppe*“ angegeben wird</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1784">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="aa5bc-1785">Container</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1785">Container</span></span>

* <span data-ttu-id="aa5bc-1786">`--secure-environment-variables` zum Übergeben sicherer Umgebungsvariablen an einen Container hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1786">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="aa5bc-1787">IoT</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1787">IoT</span></span>

* <span data-ttu-id="aa5bc-1788">[BREAKING CHANGE] Veraltete Befehle entfernt, die in die IoT-Erweiterung verschoben wurden</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1788">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="aa5bc-1789">Elemente aktualisiert, um nicht die Domäne `azure-devices.net` anzunehmen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1789">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="aa5bc-1790">Iot Central</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1790">Iot Central</span></span>

* <span data-ttu-id="aa5bc-1791">Erstes Release des IoT Central-Moduls</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1791">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="aa5bc-1792">KeyVault</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1792">KeyVault</span></span>


* <span data-ttu-id="aa5bc-1793">Befehle zum Verwalten von Speicherkonten und SAS-Definitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1793">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="aa5bc-1794">Befehle für Netzwerkregeln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1794">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="aa5bc-1795">Parameter `--id` zu Geheimnis-, Schlüssel- und Zertifikatvorgängen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1795">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="aa5bc-1796">Unterstützung für Version mit mehreren APIs zur Schlüsseltresorverwaltung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1796">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="aa5bc-1797">Unterstützung für Version mit mehreren APIs zur Schlüsseltresordatenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1797">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="aa5bc-1798">Relay</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1798">Relay</span></span>

* <span data-ttu-id="aa5bc-1799">Erste Veröffentlichung</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1799">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="aa5bc-1800">Sql</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1800">Sql</span></span>

* <span data-ttu-id="aa5bc-1801">Befehle vom Typ `sql failover-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1801">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="aa5bc-1802">Storage</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1802">Storage</span></span>

* <span data-ttu-id="aa5bc-1803">[BREAKING CHANGE]`storage account show-usage` geändert, um Parameter `--location` erforderlich zu machen. Auflistung nach Region</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1803">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="aa5bc-1804">Parameter `--resource-group` geändert, sodass er für `storage account`-Befehle optional ist</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1804">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="aa5bc-1805">Warnungen vom Typ „Fehler bei Vorbedingung“ für einzelne Fehler in Batch-Befehlen für eine aggregiert Nachricht entfernt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1805">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="aa5bc-1806">`[blob|file] delete-batch`-Befehle geändert, sodass kein Array mit Null-Werten mehr ausgegeben wird</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1806">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="aa5bc-1807">`blob [download|upload|delete-batch]`-Befehle geändert, um SAS-Token aus Container-URL zu lesen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1807">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="aa5bc-1808">VM</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1808">VM</span></span>

* <span data-ttu-id="aa5bc-1809">Allgemeine Filter zu `vm list-skus` für höhere Benutzerfreundlichkeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1809">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="aa5bc-1810">31. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1810">July 31, 2018</span></span>

<span data-ttu-id="aa5bc-1811">Version 2.0.43</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1811">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="aa5bc-1812">ACR</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1812">ACR</span></span>

* <span data-ttu-id="aa5bc-1813">Flag `--with-secure-properties` zum Befehl `acr build-task show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1813">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="aa5bc-1814">Befehl `acr build-task update-build` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1814">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="aa5bc-1815">ACS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1815">ACS</span></span>

* <span data-ttu-id="aa5bc-1816">Änderung, um 0 (Erfolg) zurückzugeben, wenn `az aks browse` durch Drücken von [STRG+C] beendet wird</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1816">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="aa5bc-1817">Batch</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1817">Batch</span></span>

* <span data-ttu-id="aa5bc-1818">Korrektur eines Fehlers bei der Anzeige des AAD-Tokens in Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1818">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="aa5bc-1819">Container</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1819">Container</span></span>

* <span data-ttu-id="aa5bc-1820">Voraussetzung von `--log-analytics-workspace-key` für Name oder ID im festgelegten Abonnement entfernt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1820">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="aa5bc-1821">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1821">Network</span></span>

* <span data-ttu-id="aa5bc-1822">DNS-Unterstützung zu „2017-03-09-profile“ für Azure Stack hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1822">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="aa5bc-1823">Resource</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1823">Resource</span></span>

* <span data-ttu-id="aa5bc-1824">`--rollback-on-error` zu `group deployment create` hinzugefügt, um bei einem Fehler eine als funktionierend bekannte Bereitstellung auszuführen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1824">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="aa5bc-1825">Problem behoben, aufgrund dessen `--parameters {}` mit `group deployment create` zu einem Fehler führte</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1825">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="aa5bc-1826">Role</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1826">Role</span></span>

* <span data-ttu-id="aa5bc-1827">Unterstützung für das Stack-Profil „2017-03-09-profile“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1827">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="aa5bc-1828">Problem behoben, aufgrund dessen das generische Update von Parametern auf `app update` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1828">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="aa5bc-1829">Suchen,</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1829">Search</span></span>

* <span data-ttu-id="aa5bc-1830">Befehle für Azure Search-Dienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1830">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="aa5bc-1831">Service Bus</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1831">Service Bus</span></span>

* <span data-ttu-id="aa5bc-1832">Migrationsbefehlsgruppe hinzugefügt, um einen Namespace von Service Bus Standard zu Premium zu migrieren</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1832">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="aa5bc-1833">Neue optionale Eigenschaften zu Service Bus-Warteschlange und -Abonnement hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1833">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="aa5bc-1834">`--enable-batched-operations` und `--enable-dead-lettering-on-message-expiration` in `queue`</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1834">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="aa5bc-1835">`--dead-letter-on-filter-exceptions` in `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1835">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="aa5bc-1836">Storage</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1836">Storage</span></span>

* <span data-ttu-id="aa5bc-1837">Unterstützung für den Download großer Dateien über eine einzelne Verbindung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1837">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="aa5bc-1838">`show`-Befehle konvertiert, bei denen im Falle einer fehlenden Ressource kein Fehler mit dem Exitcode 3 ausgelöst wurde</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1838">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="aa5bc-1839">VM</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1839">VM</span></span>

* <span data-ttu-id="aa5bc-1840">Unterstützung zum Auflisten von Verfügbarkeitsgruppen nach Abonnement hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1840">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="aa5bc-1841">Unterstützung für `StandardSSD_LRS` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1841">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="aa5bc-1842">Unterstützung für Anwendungssicherheitsgruppe beim Erstellen einer VM-Skalierungsgruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1842">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="aa5bc-1843">[BREAKING CHANGE]`[vm|vmss] create`, `[vm|vmss] identity assign` und `[vm|vmss] identity remove` wurden geändert, um vom Benutzer zugewiesene Identitäten im Wörterbuchformat auszugeben.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1843">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="aa5bc-1844">18. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1844">July 18, 2018</span></span>

<span data-ttu-id="aa5bc-1845">Version 2.0.42</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1845">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="aa5bc-1846">Core</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1846">Core</span></span>

* <span data-ttu-id="aa5bc-1847">Unterstützung für browserbasierte Anmeldung WSL-Bash-Fenster hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1847">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="aa5bc-1848">`--force-string`-Flag für alle generischen Updatebefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1848">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="aa5bc-1849">[BREAKING CHANGE] Befehle vom Typ „show“ so geändert, dass die Fehlermeldung protokolliert wird und der Vorgang bei einer fehlenden Ressource mit dem Exitcode 3 fehlschlägt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1849">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="aa5bc-1850">ACR</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1850">ACR</span></span>

* <span data-ttu-id="aa5bc-1851">[BREAKING CHANGE] „--no-push“ in Befehl „acr build“ in reines Flag geändert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1851">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="aa5bc-1852">Befehle `show` und `update` unter Gruppe `acr repository` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1852">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="aa5bc-1853">`--detail`-Flag für `show-manifests` und `show-tags` hinzugefügt, um ausführlichere Informationen anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1853">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="aa5bc-1854">Parameter `--image` zur Unterstützung des Abrufs von Builddetails oder Protokollen anhand eines Images hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1854">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="aa5bc-1855">ACS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1855">ACS</span></span>

* <span data-ttu-id="aa5bc-1856">`az aks create` so geändert, dass mit Fehler beendet wird, wenn `--max-pods` kleiner als 5 ist</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1856">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="aa5bc-1857">AppService</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1857">AppService</span></span>

* <span data-ttu-id="aa5bc-1858">Unterstützung für PremiumV2-SKUs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1858">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="aa5bc-1859">Batch</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1859">Batch</span></span>

* <span data-ttu-id="aa5bc-1860">Korrektur eines Fehlers bei der Verwendung von Anmeldeinformationen im Cloud Shell-Modus</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1860">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="aa5bc-1861">JSON-Eingabe so geändert, dass Groß-/Kleinschreibung nicht beachtet wird</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1861">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="aa5bc-1862">Batch KI</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1862">Batch AI</span></span>

* <span data-ttu-id="aa5bc-1863">Befehl `az batchai job exec` korrigiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1863">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="aa5bc-1864">Container</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1864">Container</span></span>

* <span data-ttu-id="aa5bc-1865">Anforderung von Benutzername und Kennwort für Nicht-DockerHub-Registrierungen entfernt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1865">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="aa5bc-1866">Fehler beim Erstellen von Containergruppen aus YAML-Datei behoben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1866">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="aa5bc-1867">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1867">Network</span></span>

* <span data-ttu-id="aa5bc-1868">Unterstützung für `--no-wait` zu `network nic [create|update|delete]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1868">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="aa5bc-1869">`network nic wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1869">Added `network nic wait`</span></span>
* <span data-ttu-id="aa5bc-1870">`--ids`-Argument für `network vnet [subnet|peering] list` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1870">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="aa5bc-1871">`--include-default`-Flag hinzugefügt, um Standardsicherheitsregeln in die Ausgabe von `network nsg rule list` aufzunehmen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1871">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="aa5bc-1872">Resource</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1872">Resource</span></span>

* <span data-ttu-id="aa5bc-1873">Unterstützung für `--no-wait` zu `group deployment delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1873">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="aa5bc-1874">Unterstützung für `--no-wait` zu `deployment delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1874">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="aa5bc-1875">Befehl `deployment wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1875">Added `deployment wait` command</span></span>
* <span data-ttu-id="aa5bc-1876">Problem behoben, aufgrund dessen die `az deployment`-Befehle auf Abonnementebene fälschlicherweise für Profil „2017-03-09-profile“ angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1876">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="aa5bc-1877">SQL</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1877">SQL</span></span>

* <span data-ttu-id="aa5bc-1878">Fehler „Der angegebene Ressourcengruppenname ... entsprach nicht dem Namen in der URL“ beim Angeben des Namens des Pools für elastische Datenbanken für `sql db copy`-und `sql db replica create`-Befehle behoben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1878">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="aa5bc-1879">Konfigurieren des Standard-SQL Servers durch Ausführen von `az configure --defaults sql-server=<name>` zulässig</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1879">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="aa5bc-1880">Tabellenformatierer für Befehle `sql server`, `sql server firewall-rule`, `sql list-usages` und `sql show-usage` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1880">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="aa5bc-1881">Storage</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1881">Storage</span></span>

* <span data-ttu-id="aa5bc-1882">`pageRanges`-Eigenschaft zu `storage blob show`-Ausgabe hinzugefügt, die für Seitenblobs ausgefüllt wird</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1882">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="aa5bc-1883">VM</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1883">VM</span></span>

* <span data-ttu-id="aa5bc-1884">[BREAKING CHANGE]`vmss create` so geändert, dass `Standard_DS1_v2` als standardmäßige Instanzgröße verwendet wird</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1884">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="aa5bc-1885">Unterstützung für `--no-wait` zu `vm extension [set|delete]` und `vmss extension [set|delete]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1885">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="aa5bc-1886">`vm extension wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1886">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="aa5bc-1887">3\. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1887">July 3, 2018</span></span>

<span data-ttu-id="aa5bc-1888">Version 2.0.41</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1888">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="aa5bc-1889">AKS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1889">AKS</span></span>

* <span data-ttu-id="aa5bc-1890">Überwachung geändert, sodass Abonnement-ID verwendet wird</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1890">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="aa5bc-1891">3\. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1891">July 3, 2018</span></span>

<span data-ttu-id="aa5bc-1892">Version 2.0.40</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1892">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="aa5bc-1893">Core</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1893">Core</span></span>

* <span data-ttu-id="aa5bc-1894">Neuer Autorisierungscode-Flow für interaktive Anmeldung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1894">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="aa5bc-1895">ACR</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1895">ACR</span></span>

* <span data-ttu-id="aa5bc-1896">Abruf-Buildstatus hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1896">Added polling build status</span></span>
* <span data-ttu-id="aa5bc-1897">Unterstützung für Enumerationswerte ohne Berücksichtigung von Groß-/Kleinschreibung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1897">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="aa5bc-1898">Parameter `--top` und `--orderby` für `show-manifests` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1898">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="aa5bc-1899">ACS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1899">ACS</span></span>

* <span data-ttu-id="aa5bc-1900">[BREAKING CHANGE] Standardmäßiges Aktivieren der rollenbasierten Zugriffssteuerung für Kubernetes</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1900">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="aa5bc-1901">Argument `--disable-rbac` hinzugefügt und `--enable-rbac` als veraltet festgelegt, da es nun der Standard ist</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1901">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="aa5bc-1902">Optionen für Befehl `aks browse` wurden aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1902">Updated options for `aks browse` command.</span></span> <span data-ttu-id="aa5bc-1903">Unterstützung für `--listen-port` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1903">Added `--listen-port` support</span></span>
* <span data-ttu-id="aa5bc-1904">Standardmäßiges Helm-Diagrammpaket für Befehl `aks install-connector` wurde aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1904">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="aa5bc-1905">Verwenden von „virtual-kubelet-for-aks-latest.tgz“</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1905">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="aa5bc-1906">Befehle `aks enable-addons` und `aks disable-addons` zum Aktualisieren eines vorhandenen Clusters hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1906">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="aa5bc-1907">AppService</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1907">AppService</span></span>

* <span data-ttu-id="aa5bc-1908">Unterstützung für das Deaktivieren der Identität über `webapp identity remove` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1908">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="aa5bc-1909">`preview`-Tag für Identitätsfunktion entfernt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1909">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="aa5bc-1910">Backup</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1910">Backup</span></span>

* <span data-ttu-id="aa5bc-1911">Moduldefinition aktualisiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1911">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="aa5bc-1912">Batch AI</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1912">BatchAI</span></span>

* <span data-ttu-id="aa5bc-1913">Tabellenausgabe für Befehle `batchai cluster node list` und `batchai job node list` korrigiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1913">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="aa5bc-1914">Cloud</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1914">Cloud</span></span>

* <span data-ttu-id="aa5bc-1915">Serversuffix `acr login` zu Cloudkonfiguration hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1915">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="aa5bc-1916">Container</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1916">Container</span></span>

* <span data-ttu-id="aa5bc-1917">`container create` zu Standard für Vorgang mit langer Ausführungsdauer geändert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1917">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="aa5bc-1918">Log Analytics-Parameter `--log-analytics-workspace` und `--log-analytics-workspace-key` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1918">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="aa5bc-1919">Parameter `--protocol` zum Festlegen des zu verwendenden Netzwerkprotokolls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1919">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="aa5bc-1920">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1920">Extension</span></span>

* <span data-ttu-id="aa5bc-1921">`extension list-available` geändert, sodass nur mit der CLI-Version kompatible Erweiterungen angezeigt werden</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1921">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="aa5bc-1922">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1922">Network</span></span>

* <span data-ttu-id="aa5bc-1923">Problem behoben, aufgrund dessen bei Datensatztypen die Groß-/Kleinschreibung beachtet werden musste ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1923">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="aa5bc-1924">Rdbms</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1924">Rdbms</span></span>

* <span data-ttu-id="aa5bc-1925">Befehle vom Typ `[postgres|myql] server vnet-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1925">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="aa5bc-1926">Resource</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1926">Resource</span></span>

* <span data-ttu-id="aa5bc-1927">Neue Vorgangsgruppe `deployment` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1927">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="aa5bc-1928">VM</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1928">VM</span></span>

* <span data-ttu-id="aa5bc-1929">Unterstützung für das Entfernen der vom System zugewiesenen Identität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1929">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="aa5bc-1930">25. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1930">June 25, 2018</span></span>

<span data-ttu-id="aa5bc-1931">Version 2.0.39</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1931">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="aa5bc-1932">Befehlszeilenschnittstelle (CLI)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1932">CLI</span></span>

* <span data-ttu-id="aa5bc-1933">Dateieinschränkung in MSI-Installer aktualisiert, um Problem mit der Erweiterungsinstallation zu beheben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1933">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="aa5bc-1934">19. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1934">June 19, 2018</span></span>

<span data-ttu-id="aa5bc-1935">Version 2.0.38</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1935">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="aa5bc-1936">Core</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1936">Core</span></span>

* <span data-ttu-id="aa5bc-1937">Globale Unterstützung für `--subscription` zu den meisten Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1937">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="aa5bc-1938">ACR</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1938">ACR</span></span>

* <span data-ttu-id="aa5bc-1939">`azure-storage-blob` als Abhängigkeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1939">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="aa5bc-1940">CPU-Standardkonfiguration für `acr build-task create` geändert, sodass zwei Kerne verwendet werden</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1940">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="aa5bc-1941">ACS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1941">ACS</span></span>

* <span data-ttu-id="aa5bc-1942">Optionen des Befehls `aks use-dev-spaces` wurden aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1942">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="aa5bc-1943">Unterstützung für `--update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1943">Added `--update` support</span></span>
* <span data-ttu-id="aa5bc-1944">`aks get-credentials --admin` geändert, sodass der Benutzerkontext in `$HOME/.kube/config` ersetzt wird</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1944">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="aa5bc-1945">Schreibgeschützte `nodeResourceGroup`-Eigenschaft in verwalteten Clustern verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1945">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="aa5bc-1946">Befehlsfehler `acs browse` korrigiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1946">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="aa5bc-1947">`--connector-name` für `aks install-connector`, `aks upgrade-connector` und `aks remove-connector` als optional festgelegt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1947">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="aa5bc-1948">Neue Azure Container Instances-Regionen für `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1948">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="aa5bc-1949">Normalisierter Speicherort im Helm-Versionsnamen und Knotenname zu `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1949">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="aa5bc-1950">AppService</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1950">AppService</span></span>

* <span data-ttu-id="aa5bc-1951">Unterstützung für neuere Versionen von „urllib“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1951">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="aa5bc-1952">Unterstützung der Verwendung eines App Service-Plans aus externen Ressourcengruppen zu `functionapp create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1952">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="aa5bc-1953">Batch</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1953">Batch</span></span>

* <span data-ttu-id="aa5bc-1954">`azure-batch-extensions`-Abhängigkeit entfernt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1954">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="aa5bc-1955">Batch KI</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1955">Batch AI</span></span>

* <span data-ttu-id="aa5bc-1956">Unterstützung für Arbeitsbereiche wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1956">Added support for workspaces.</span></span> <span data-ttu-id="aa5bc-1957">Arbeitsbereiche ermöglichen das Zusammenfassen von Clustern, Dateiservern und Experimenten in Gruppen ohne Beschränkung der Anzahl von Ressourcen, die erstellt werden können.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1957">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="aa5bc-1958">Unterstützung für Experimente wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1958">Added support for experiments.</span></span> <span data-ttu-id="aa5bc-1959">Experimente ermöglichen das Zusammenfassen von Aufträgen in Sammlungen ohne Beschränkung der Anzahl von erstellten Aufträgen.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1959">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="aa5bc-1960">Unterstützung für das Konfigurieren von `/dev/shm` für Aufträge hinzugefügt, die in einem Docker-Container ausgeführt werden</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1960">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="aa5bc-1961">Die Befehle `batchai cluster node exec` und `batchai job node exec` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1961">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="aa5bc-1962">Diese Befehle ermöglichen die Ausführung aller Befehle direkt auf Knoten und bieten Funktionen zur Portweiterleitung.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1962">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="aa5bc-1963">Unterstützung für `--ids` zu `batchai`-Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1963">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="aa5bc-1964">[BREAKING CHANGE] Alle Cluster und Dateiserver müssen unter Arbeitsbereichen erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1964">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="aa5bc-1965">[BREAKING CHANGE] Aufträge müssen unter Experimenten erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1965">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="aa5bc-1966">[BREAKING CHANGE]`--nfs-resource-group` wurde aus den Befehlen `cluster create` und `job create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1966">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="aa5bc-1967">Geben Sie zum Bereitstellen eines NFS, das einem anderen Arbeitsbereich/einer anderen Ressourcengruppe angehört, die ARM-ID des Dateiservers über die Option `--nfs` an.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1967">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="aa5bc-1968">[BREAKING CHANGE]`--cluster-resource-group` wurde aus dem Befehl `job create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1968">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="aa5bc-1969">Geben Sie zum Übermitteln eines Auftrags, der einem anderen Arbeitsbereich/einer anderen Ressourcengruppe angehört, die ARM-ID des Clusters über die Option `--cluster` an.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1969">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="aa5bc-1970">[BREAKING CHANGE] Attribut `location` wurde aus Aufträgen, Clustern und Dateiservern entfernt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1970">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="aa5bc-1971">„Location“ ist jetzt ein Attribut eines Arbeitsbereichs.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1971">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="aa5bc-1972">[BREAKING CHANGE]`--location` wurde aus den Befehlen `job create`, `cluster create` und `file-server create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1972">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="aa5bc-1973">[BREAKING CHANGE] Namen von Kurzoptionen wurden geändert, um die Schnittstelle konsistenter zu machen:</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1973">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="aa5bc-1974">[`--config`, `-c`] in [`--config-file`, `-f`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1974">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="aa5bc-1975">[`--cluster`, `-r`] in [`--cluster`, `-c`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1975">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="aa5bc-1976">[`--cluster`, `-n`] in [`--cluster`, `-c`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1976">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="aa5bc-1977">[`--job`, `-n`] in [`--job`, `-j`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1977">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="aa5bc-1978">Karten</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1978">Maps</span></span>

* <span data-ttu-id="aa5bc-1979">[BREAKING CHANGE]`maps account create` wurde so geändert, dass Nutzungsbedingungen entweder durch interaktive Eingabeaufforderung oder `--accept-tos`-Flag akzeptiert werden müssen.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1979">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="aa5bc-1980">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1980">Network</span></span>

* <span data-ttu-id="aa5bc-1981">Unterstützung für `https` zu `network lb probe create` hinzugefügt [Nr. 6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1981">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="aa5bc-1982">Problem behoben, aufgrund dessen die Groß-/Kleinschreibung von `--endpoint-status` berücksichtigt wurde.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1982">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="aa5bc-1983">#6502</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1983">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="aa5bc-1984">Reservations</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1984">Reservations</span></span>

* <span data-ttu-id="aa5bc-1985">[BREAKING CHANGE] Erforderlicher Parameter `ReservedResourceType` zu `reservations catalog show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1985">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="aa5bc-1986">Parameter `Location` zu `reservations catalog show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1986">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="aa5bc-1987">[BREAKING CHANGE]`kind` aus `ReservationProperties` entfernt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1987">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="aa5bc-1988">[BREAKING CHANGE]`capabilities` wurde in `Catalog` in `sku_properties` umbenannt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1988">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="aa5bc-1989">[BREAKING CHANGE] Eigenschaften `size` und `tier` aus `Catalog` entfernt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1989">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="aa5bc-1990">Parameter `InstanceFlexibility` zu `reservations reservation update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1990">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="aa5bc-1991">Role</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1991">Role</span></span>

* <span data-ttu-id="aa5bc-1992">Fehlerbehandlung verbessert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1992">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="aa5bc-1993">SQL</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1993">SQL</span></span>

* <span data-ttu-id="aa5bc-1994">Verwirrender Fehler behoben, der beim Ausführen von `az sql db list-editions` für einen Ort auftrat, der für Ihr Abonnement nicht verfügbar ist</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1994">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="aa5bc-1995">Storage</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1995">Storage</span></span>

* <span data-ttu-id="aa5bc-1996">Lesbarkeit der Tabellenausgabe für `storage blob download` verbessert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1996">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="aa5bc-1997">VM</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1997">VM</span></span>

* <span data-ttu-id="aa5bc-1998">Verbesserte Einschränkung der VM-Größenüberprüfung für Unterstützung von beschleunigten Netzwerken in `vm create`</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1998">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="aa5bc-1999">Warnung für `vmss create` hinzugefügt, dass die VM-Standardgröße von `Standard_D1_v2` auf `Standard_DS1_v2` umgestellt wird</span><span class="sxs-lookup"><span data-stu-id="aa5bc-1999">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="aa5bc-2000">`--force-update` zu `[vm|vmss] extension set` hinzugefügt, um die Erweiterung auch dann zu aktualisieren, wenn die Konfiguration nicht geändert wurde</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2000">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="aa5bc-2001">13. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2001">June 13, 2018</span></span>

<span data-ttu-id="aa5bc-2002">Version 2.0.37</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2002">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="aa5bc-2003">Core</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2003">Core</span></span>

* <span data-ttu-id="aa5bc-2004">Verbesserte interaktive Telemetrie</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2004">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="aa5bc-2005">13. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2005">June 13, 2018</span></span>

<span data-ttu-id="aa5bc-2006">Version 2.0.36</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2006">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="aa5bc-2007">AKS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2007">AKS</span></span>

* <span data-ttu-id="aa5bc-2008">Zusätzliche erweiterte Netzwerkoptionen zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2008">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="aa5bc-2009">Argumente zu `aks create` zum Aktivieren der Überwachung und HTTP-Routing hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2009">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="aa5bc-2010">Argument `--no-ssh-key` zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2010">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="aa5bc-2011">Argument `--enable-rbac` zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2011">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="aa5bc-2012">[VORSCHAUVERSION] Unterstützung für Azure Active Directory-Authentifizierung zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2012">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="aa5bc-2013">AppService</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2013">AppService</span></span>

* <span data-ttu-id="aa5bc-2014">Problem mit inkompatiblen urllib-Versionen behoben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2014">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="aa5bc-2015">5\. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2015">June 5, 2018</span></span>

<span data-ttu-id="aa5bc-2016">Version 2.0.35</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2016">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="aa5bc-2017">Interactive</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2017">Interactive</span></span>

* <span data-ttu-id="aa5bc-2018">Grenzwerte für die Abhängigkeiten des interaktiven Modus hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2018">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="aa5bc-2019">5\. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2019">June 5, 2018</span></span>

<span data-ttu-id="aa5bc-2020">Version 2.0.34</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2020">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="aa5bc-2021">Core</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2021">Core</span></span>

* <span data-ttu-id="aa5bc-2022">Unterstützung für mandantenübergreifende Ressourcenverweise hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2022">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="aa5bc-2023">Verbesserte Zuverlässigkeit bei Telemetrieuploads</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2023">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="aa5bc-2024">ACR</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2024">ACR</span></span>

* <span data-ttu-id="aa5bc-2025">Unterstützung für VSTS als Remotequellort hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2025">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="aa5bc-2026">Befehl `acr import` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2026">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="aa5bc-2027">AKS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2027">AKS</span></span>

* <span data-ttu-id="aa5bc-2028">`aks get-credentials` wurde geändert, um die Kube-Konfigurationsdatei mit sichereren Dateisystemberechtigungen zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2028">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="aa5bc-2029">Batch</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2029">Batch</span></span>

* <span data-ttu-id="aa5bc-2030">Fehler bei der Formatierung der Poollistentabelle behoben [[Problem 4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2030">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="aa5bc-2031">IoT</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2031">IOT</span></span>

* <span data-ttu-id="aa5bc-2032">Unterstützung für das Erstellen von IoT Hub-Instanzen im Tarif „Basic“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2032">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="aa5bc-2033">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2033">Network</span></span>

* <span data-ttu-id="aa5bc-2034">`network vnet peering` wurde verbessert.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2034">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="aa5bc-2035">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2035">Policy Insights</span></span>

* <span data-ttu-id="aa5bc-2036">Erstrelease</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2036">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="aa5bc-2037">ARM</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2037">ARM</span></span>

* <span data-ttu-id="aa5bc-2038">Befehle vom Typ `account management-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2038">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="aa5bc-2039">SQL</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2039">SQL</span></span>

* <span data-ttu-id="aa5bc-2040">Neue Befehle für verwaltete Instanzen hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2040">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="aa5bc-2041">Neue Befehle für verwaltete Datenbanken hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2041">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="aa5bc-2042">Storage</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2042">Storage</span></span>

* <span data-ttu-id="aa5bc-2043">Zusätzliche MimeTypes für JSON und JavaScript hinzugefügt (abzuleiten aus Dateierweiterungen)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2043">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="aa5bc-2044">VM</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2044">VM</span></span>

* <span data-ttu-id="aa5bc-2045">`vm list-skus` wurde geändert, um feste Spalten zu verwenden und eine Warnung hinzuzufügen, dass `Tier` und `Size` entfernt werden.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2045">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="aa5bc-2046">Option `--accelerated-networking` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2046">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="aa5bc-2047">`--tags` zu `identity create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2047">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="aa5bc-2048">22. Mai 2018</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2048">May 22, 2018</span></span>

<span data-ttu-id="aa5bc-2049">Version 2.0.33</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2049">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="aa5bc-2050">Core</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2050">Core</span></span>

* <span data-ttu-id="aa5bc-2051">Unterstützung für das Erweitern von `@` in Dateinamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2051">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="aa5bc-2052">ACS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2052">ACS</span></span>

* <span data-ttu-id="aa5bc-2053">Neue Dev Spaces-Befehle `aks use-dev-spaces` und `aks remove-dev-spaces` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2053">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="aa5bc-2054">Tippfehler in Hilfemeldung korrigiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2054">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="aa5bc-2055">AppService</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2055">AppService</span></span>

* <span data-ttu-id="aa5bc-2056">Verbesserte generische Aktualisierungsbefehle</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2056">Improved generic update commands</span></span>
* <span data-ttu-id="aa5bc-2057">Asynchrone Unterstützung für `webapp deployment source config-zip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2057">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="aa5bc-2058">Container</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2058">Container</span></span>

* <span data-ttu-id="aa5bc-2059">Unterstützung für das Exportieren einer Containergruppe im YAML-Format hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2059">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="aa5bc-2060">Unterstützung für die Verwendung einer YAML-Datei zum Erstellen/Aktualisieren einer Containergruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2060">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="aa5bc-2061">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2061">Extension</span></span>

* <span data-ttu-id="aa5bc-2062">Verbesserte Entfernung von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2062">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="aa5bc-2063">Interactive</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2063">Interactive</span></span>

* <span data-ttu-id="aa5bc-2064">Protokollierung geändert, um Parser für Abschlüsse zu deaktivieren</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2064">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="aa5bc-2065">Verbesserte Verarbeitung beschädigter Hilfscaches</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2065">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="aa5bc-2066">KeyVault</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2066">KeyVault</span></span>

* <span data-ttu-id="aa5bc-2067">keyvault-Befehle wurden korrigiert, damit sie in Cloud Shell oder auf virtuellen Computern mit Identität verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2067">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="aa5bc-2068">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2068">Network</span></span>

* <span data-ttu-id="aa5bc-2069">Problem behoben, aufgrund dessen `network watcher show-topology` nicht mit einem VNET und/oder Subnetznamen verwendet werden konnte ([#6326](https://github.com/Azure/azure-cli/issues/6326))</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2069">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="aa5bc-2070">Problem behoben, aufgrund dessen einige `network watcher`-Befehle fälschlicherweise angaben, dass Network Watcher nicht für bestimmte Regionen aktiviert ist ([#6264](https://github.com/Azure/azure-cli/issues/6264))</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2070">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="aa5bc-2071">SQL</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2071">SQL</span></span>

* <span data-ttu-id="aa5bc-2072">[BREAKING CHANGE] Von den Befehlen `db` und `dw` zurückgegebene Antwortobjekte geändert:</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2072">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="aa5bc-2073">Eigenschaft `serviceLevelObjective` in `currentServiceObjectiveName` umbenannt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2073">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="aa5bc-2074">Eigenschaften `currentServiceObjectiveId` und `requestedServiceObjectiveId` entfernt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2074">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="aa5bc-2075">Eigenschaft `maxSizeBytes` geändert (ist nun keine Zeichenfolge mehr, sondern ein Ganzzahlwert)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2075">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="aa5bc-2076">[BREAKING CHANGE] Die folgenden `db`- und `dw`-Eigenschaften wurden geändert und sind jetzt schreibgeschützt:</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2076">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="aa5bc-2077">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2077">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="aa5bc-2078">Verwenden Sie zum Aktualisieren den Parameter `--service-objective`, oder legen Sie die Eigenschaft `sku.name` fest.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2078">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="aa5bc-2079">`edition`.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2079">`edition`.</span></span> <span data-ttu-id="aa5bc-2080">Verwenden Sie zum Aktualisieren den Parameter `--edition`, oder legen Sie die Eigenschaft `sku.tier` fest.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2080">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="aa5bc-2081">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2081">`elasticPoolName`.</span></span> <span data-ttu-id="aa5bc-2082">Verwenden Sie zum Aktualisieren den Parameter `--elastic-pool`, oder legen Sie die Eigenschaft `elasticPoolId` fest.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2082">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="aa5bc-2083">[BREAKING CHANGE] Die folgenden `elastic-pool`-Eigenschaften wurden geändert und sind jetzt schreibgeschützt:</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2083">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="aa5bc-2084">`edition`.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2084">`edition`.</span></span> <span data-ttu-id="aa5bc-2085">Verwenden Sie zum Aktualisieren den Parameter `--edition`.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2085">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="aa5bc-2086">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2086">`dtu`.</span></span> <span data-ttu-id="aa5bc-2087">Verwenden Sie zum Aktualisieren den Parameter `--capacity`.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2087">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="aa5bc-2088">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2088">`databaseDtuMin`.</span></span> <span data-ttu-id="aa5bc-2089">Verwenden Sie zum Aktualisieren den Parameter `--db-min-capacity`.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2089">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="aa5bc-2090">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2090">`databaseDtuMax`.</span></span> <span data-ttu-id="aa5bc-2091">Verwenden Sie zum Aktualisieren den Parameter `--db-max-capacity`.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2091">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="aa5bc-2092">Die Parameter `--family` und `--capacity` wurden zu den `db`-, `dw`- und `elastic-pool`-Befehlen hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2092">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="aa5bc-2093">Den `db`-, `dw`- und `elastic-pool`-Befehlen wurden Tabellenformatierer hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2093">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="aa5bc-2094">Storage</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2094">Storage</span></span>

* <span data-ttu-id="aa5bc-2095">Vervollständigung für das Argument `--account-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2095">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="aa5bc-2096">Problem mit `storage entity query` behoben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2096">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="aa5bc-2097">VM</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2097">VM</span></span>

* <span data-ttu-id="aa5bc-2098">[BREAKING CHANGE]`--write-accelerator` aus `vm create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2098">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="aa5bc-2099">Die gleiche Unterstützung kann über `vm update` oder `vm disk attach` erzielt werden.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2099">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="aa5bc-2100">Erweiterungsimageabgleich in `[vm|vmss] extension` korrigiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2100">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="aa5bc-2101">`--boot-diagnostics-storage` zu `vm create` zur Erfassung des Startprotokolls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2101">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="aa5bc-2102">`--license-type` zu `[vm|vmss] update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2102">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="aa5bc-2103">7\. Mai 2018</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2103">May 7, 2018</span></span>

<span data-ttu-id="aa5bc-2104">Version 2.0.32</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2104">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="aa5bc-2105">Core</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2105">Core</span></span>

* <span data-ttu-id="aa5bc-2106">Ein Ausnahmefehler wurde behoben, der beim Abrufen von Geheimnissen aus einem Dienstprinzipalkonto mit Zertifikat auftrat.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2106">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="aa5bc-2107">Eingeschränkte Unterstützung für positionelle Argumente hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2107">Added limited support for positional arguments</span></span>
* <span data-ttu-id="aa5bc-2108">Problem behoben, aufgrund dessen `--query` nicht mit `--ids` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2108">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="aa5bc-2109">#5591</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2109">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="aa5bc-2110">Pipingszenarien von Befehlen bei Verwendung von `--ids` verbessert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2110">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="aa5bc-2111">Unterstützt `-o tsv` mit angegebener Abfrage bzw. `-o json` ohne angegeben Abfrage</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2111">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="aa5bc-2112">Befehlsvorschläge bei Fehler hinzugefügt, wenn Befehle Tippfehler enthielten</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2112">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="aa5bc-2113">Fehler bei der Eingabe von `az ''` behandelt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2113">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="aa5bc-2114">Unterstützung für benutzerdefinierte Ressourcentypen für Befehlsmodule und -erweiterungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2114">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="aa5bc-2115">ACR</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2115">ACR</span></span>

* <span data-ttu-id="aa5bc-2116">ACR Build-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2116">Added ACR Build commands</span></span>
* <span data-ttu-id="aa5bc-2117">Fehlermeldungen vom Typ „Ressource nicht gefunden.“ verbessert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2117">Improved resource not found error messages</span></span>
* <span data-ttu-id="aa5bc-2118">Höhere Leistung bei der Ressourcenerstellung und optimierte Fehlerbehandlung</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2118">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="aa5bc-2119">ACR-Anmeldung bei nicht standardmäßigen Konsolen und WSL optimiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2119">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="aa5bc-2120">Fehlermeldungen zu Repositorybefehlen optimiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2120">Improved repository commands error messages</span></span>
* <span data-ttu-id="aa5bc-2121">Tabellenspalten und -reihenfolge aktualisiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2121">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="aa5bc-2122">ACS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2122">ACS</span></span>

* <span data-ttu-id="aa5bc-2123">Warnung hinzugefügt, dass `az aks` eine Vorschauversion des Diensts ist</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2123">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="aa5bc-2124">Berechtigungsproblem in `aks install-connector` behoben, wenn `--aci-resource-group` nicht angegeben wird</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2124">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="aa5bc-2125">AMS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2125">AMS</span></span>

* <span data-ttu-id="aa5bc-2126">Erste Version: Verwalten von Azure Media Services-Ressourcen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2126">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="aa5bc-2127">AppService</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2127">Appservice</span></span>

* <span data-ttu-id="aa5bc-2128">Ein Problem in `webapp delete` wurde behoben, das bei Angabe von `--slot` auftrat.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2128">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="aa5bc-2129">`--runtime-version` aus `webapp auth update` entfernt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2129">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="aa5bc-2130">Unterstützung für „min\_tls\_version“ und „https2.0“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2130">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="aa5bc-2131">Unterstützung für mehrere Container hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2131">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="aa5bc-2132">Batch KI</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2132">Batch AI</span></span>

* <span data-ttu-id="aa5bc-2133">`batchai create cluster` wurde geändert, um die in der Konfigurationsdatei des Clusters konfigurierte VM-Priorität zu berücksichtigen.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2133">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="aa5bc-2134">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2134">Cognitive Services</span></span>

* <span data-ttu-id="aa5bc-2135">Tippfehler im Beispiel für `cognitiveservices account create` behoben [Nr. 5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2135">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="aa5bc-2136">Nutzung</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2136">Consumption</span></span>

* <span data-ttu-id="aa5bc-2137">Neue Befehle für Budget-API hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2137">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="aa5bc-2138">Container</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2138">Container</span></span>

* <span data-ttu-id="aa5bc-2139">`--registry-server` muss nicht mehr für `container create` angegeben werden, wenn ein Registrierungsserver im Imagenamen enthalten ist.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2139">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="aa5bc-2140">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2140">Cosmos DB</span></span>

* <span data-ttu-id="aa5bc-2141">VNET-Unterstützung für Azure CLI eingeführt: Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2141">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="aa5bc-2142">DMS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2142">DMS</span></span>

* <span data-ttu-id="aa5bc-2143">Erste Version: Die Migration von SQL zu Azure SQL wird nun unterstützt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2143">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="aa5bc-2144">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2144">Extension</span></span>

* <span data-ttu-id="aa5bc-2145">Fehler behoben, aufgrund dessen Erweiterungsmetadaten nicht mehr angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2145">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="aa5bc-2146">Interactive</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2146">Interactive</span></span>

* <span data-ttu-id="aa5bc-2147">Interaktive Vervollständigung funktioniert nun auch mit positionellen Argumenten.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2147">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="aa5bc-2148">Benutzerfreundlichere Ausgabe bei der Eingabe von '\'</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2148">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="aa5bc-2149">Abschlüsse für Parameter ohne Hilfe korrigiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2149">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="aa5bc-2150">Beschreibungen für Befehlsgruppen korrigiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2150">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="aa5bc-2151">Labor</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2151">Lab</span></span>

* <span data-ttu-id="aa5bc-2152">Regressionen aus Knack-Umwandlung korrigiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2152">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="aa5bc-2153">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2153">Network</span></span>

* <span data-ttu-id="aa5bc-2154">[BREAKING CHANGE] Parameter `--ids` entfernt für:</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2154">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="aa5bc-2155">Profil</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2155">Profile</span></span>

* <span data-ttu-id="aa5bc-2156">Quellerkennung für `disk create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2156">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="aa5bc-2157">[BREAKING CHANGE]`--msi-port` und `--identity-port` entfernt, da sie nicht mehr verwendet werden</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2157">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="aa5bc-2158">Tippfehler in kurzer Zusammenfassung für `account get-access-token` korrigiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2158">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="aa5bc-2159">Redis</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2159">Redis</span></span>

* <span data-ttu-id="aa5bc-2160">`redis patch-schedule patch-schedule show` wurde durch `redis patch-schedule show` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2160">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="aa5bc-2161">`redis list-all` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2161">Deprecated `redis list-all`.</span></span> <span data-ttu-id="aa5bc-2162">Diese Funktion wurde in `redis list` integriert.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2162">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="aa5bc-2163">`redis import-method` wurde durch `redis import` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2163">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="aa5bc-2164">Unterstützung für `--ids` zu verschiedenen Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2164">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="aa5bc-2165">Role</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2165">Role</span></span>

* <span data-ttu-id="aa5bc-2166">[BREAKING CHANGE] Veralteter Befehl `ad sp reset-credentials` entfernt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2166">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="aa5bc-2167">Storage</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2167">Storage</span></span>

* <span data-ttu-id="aa5bc-2168">Zulassen, dass das Ziel-SAS-Token für die Blobkopie auf die Quelle angewendet wird, wenn Quell-SAS und Kontoschlüssel nicht angegeben werden</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2168">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="aa5bc-2169">Verfügbar gemacht: Socket-Timeout für Blobuploads und -downloads</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2169">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="aa5bc-2170">Blobnamen, die mit Pfadtrennzeichen beginnen, als relative Pfade behandeln</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2170">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="aa5bc-2171">Zulassen, dass `storage blob copy --source-sas` mit dem Abfragezeichen „?“ beginnt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2171">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="aa5bc-2172">`storage entity query --marker` korrigiert, um Liste von Schlüsselwerten zu akzeptieren</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2172">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="aa5bc-2173">VM</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2173">VM</span></span>

* <span data-ttu-id="aa5bc-2174">Ungültige Erkennungslogik für nicht verwalteten Blob-URI korrigiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2174">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="aa5bc-2175">Unterstützung für Datenträgerverschlüsselung ohne vom Benutzer bereitgestellte Dienstprinzipale hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2175">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="aa5bc-2176">[BREAKING CHANGE] Verwenden Sie nicht „ManagedIdentityExtension“ des virtuellen Computers für MSI-Unterstützung.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2176">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="aa5bc-2177">Unterstützung für Entfernungsrichtlinie zu `vmss` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2177">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="aa5bc-2178">[BREAKING CHANGE]`--ids` entfernt aus:</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2178">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="aa5bc-2179">Unterstützung für Schreibbeschleunigung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2179">Added write accelerator support</span></span>
* <span data-ttu-id="aa5bc-2180">`vmss perform-maintenance` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2180">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="aa5bc-2181">`vm diagnostics set` korrigiert, um zuverlässig den Betriebssystemtyp des virtuellen Computers zu erkennen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2181">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="aa5bc-2182">`vm resize` geändert, um zu überprüfen, ob die angeforderte Größe von der derzeit festgelegten Größe abweicht, und nur bei einer Änderung eine Aktualisierung auszuführen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2182">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="aa5bc-2183">10. April 2018</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2183">April 10, 2018</span></span>

<span data-ttu-id="aa5bc-2184">Version 2.0.31</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2184">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="aa5bc-2185">ACR</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2185">ACR</span></span>

* <span data-ttu-id="aa5bc-2186">Verbesserte Fehlerbehandlung für wincred-Fallback</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2186">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="aa5bc-2187">ACS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2187">ACS</span></span>

* <span data-ttu-id="aa5bc-2188">Gültigkeit von per AKS erstellten SPNs in fünf Jahre geändert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2188">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="aa5bc-2189">AppService</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2189">Appservice</span></span>

* [BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="aa5bc-2191">Nicht abgefangene Ausnahme für nicht vorhandene Web-App-Pläne behoben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2191">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="aa5bc-2192">Batch AI</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2192">BatchAI</span></span>

* <span data-ttu-id="aa5bc-2193">Unterstützung für API 2018-03-01 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2193">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="aa5bc-2194">Bereitstellung auf Auftragsebene</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2194">Job level mounting</span></span>
  - <span data-ttu-id="aa5bc-2195">Umgebungsvariablen mit Geheimniswerten</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2195">Environment variables with secret values</span></span>
  - <span data-ttu-id="aa5bc-2196">Einstellungen von Leistungsindikatoren</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2196">Performance counters settings</span></span>
  - <span data-ttu-id="aa5bc-2197">Berichtstellung für auftragsspezifisches Pfadsegment</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2197">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="aa5bc-2198">Unterstützung für Unterordner in Listendateien-API</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2198">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="aa5bc-2199">Berichterstellung zur Nutzung und zu Grenzwerten</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2199">Usage and limits reporting</span></span>
  - <span data-ttu-id="aa5bc-2200">Zulassen der Angabe des Cachetyps für NFS-Server</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2200">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="aa5bc-2201">Unterstützung für benutzerdefinierte Images</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2201">Support for custom images</span></span>
  - <span data-ttu-id="aa5bc-2202">Unterstützung für pyTorch-Toolkit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2202">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="aa5bc-2203">Befehl `job wait` hinzugefügt, der das Warten auf die Auftragsfertigstellung ermöglicht und den Code für die Auftragsbeendigung meldet</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2203">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="aa5bc-2204">Befehl `usage show` hinzugefügt, mit dem die aktuelle Nutzung von Batch KI-Ressourcen und die Grenzwerte für verschiedene Regionen aufgelistet werden</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2204">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="aa5bc-2205">Nationale Clouds werden unterstützt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2205">National clouds are supported</span></span>
* <span data-ttu-id="aa5bc-2206">Befehlszeilenargumente für Aufträge hinzugefügt, um das Bereitstellen von Dateisystemen auf Auftragsebene zusätzlich zu Konfigurationsdateien zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2206">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="aa5bc-2207">Weitere Optionen zum Anpassen von Clustern hinzugefügt – VM-Priorität, Subnetz, anfängliche Knotenanzahl für Cluster mit automatischer Skalierung, Angeben eines benutzerdefinierten Images</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2207">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="aa5bc-2208">Befehlszeilenoption zum Angeben des Cachetyps für NFS mit Verwaltung per Batch KI hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2208">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="aa5bc-2209">Angeben der Bereitstellung von Dateisystemen in Konfigurationsdateien vereinfacht.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2209">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="aa5bc-2210">Weglassen von Anmeldeinformationen für Azure-Dateifreigaben und Azure-Blobcontainer ist jetzt möglich. Die CLI füllt fehlende Anmeldeinformationen auf, indem der Speicherkontoschlüssel verwendet wird, der über Befehlszeilenparameter oder per Umgebungsvariable angegeben wird, oder der Schlüssel wird über Azure Storage abgefragt (sofern das Speicherkonto zum aktuellen Abonnement gehört).</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2210">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="aa5bc-2211">Der Befehl zum Streamen von Auftragsdateien wird jetzt automatisch abgeschlossen, nachdem der Auftrag beendet ist (Erfolg, Fehler, Beendigung oder Löschung)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2211">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="aa5bc-2212">Verbesserte `table`-Ausgabe für `show`-Vorgänge</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2212">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="aa5bc-2213">Option `--use-auto-storage` für die Clustererstellung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2213">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="aa5bc-2214">Diese Option erleichtert die Verwaltung von Speicherkonten und die Bereitstellung von Azure-Dateifreigaben und Azure-Blobcontainern in Clustern.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2214">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="aa5bc-2215">`--generate-ssh-keys` für `cluster create` und `file-server create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2215">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="aa5bc-2216">Möglichkeit zum Angeben der Knotensetupaufgabe über die Befehlszeile</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2216">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="aa5bc-2217">[BREAKING CHANGE] Befehl `job stream-file` und `job list-files` in die Gruppe `job file` verschoben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2217">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="aa5bc-2218">[BREAKING CHANGE]`--admin-user-name` im Befehl `file-server create` in `--user-name` umbenannt, um Einheitlichkeit mit dem Befehl `cluster create` zu erzielen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2218">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="aa5bc-2219">Abrechnung</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2219">Billing</span></span>

* <span data-ttu-id="aa5bc-2220">Registrierungskontobefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2220">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="aa5bc-2221">Nutzung</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2221">Consumption</span></span>

* <span data-ttu-id="aa5bc-2222">Befehle vom Typ `marketplace` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2222">Added `marketplace` commands</span></span>
* <span data-ttu-id="aa5bc-2223">[BREAKING CHANGE]`reservations summaries` in `reservation summary` umbenannt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2223">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="aa5bc-2224">[BREAKING CHANGE]`reservations details` in `reservation detail` umbenannt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2224">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="aa5bc-2225">[BREAKING CHANGE] Kurzoptionen `--reservation-order-id` und `--reservation-id` für `reservation`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2225">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="aa5bc-2226">[BREAKING CHANGE]`--grain`-Kurzoptionen für `reservation summary`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2226">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="aa5bc-2227">[BREAKING CHANGE]`--include-meter-details`-Kurzoptionen für `pricesheet`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2227">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="aa5bc-2228">Container</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2228">Container</span></span>

* <span data-ttu-id="aa5bc-2229">Parameter für die Volumebereitstellung für das Git-Repository hinzugefügt: `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` und `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2229">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="aa5bc-2230">[#5926](https://github.com/Azure/azure-cli/issues/5926) behoben: Fehler bei `az container exec`, wenn „--container-name“ angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2230">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="aa5bc-2231">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2231">Extension</span></span>

* <span data-ttu-id="aa5bc-2232">Meldung für Distributionsüberprüfung in Debugebene geändert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2232">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="aa5bc-2233">Interactive</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2233">Interactive</span></span>

* <span data-ttu-id="aa5bc-2234">Geändert: Verhinderung des Abschlusses bei nicht erkannten Befehlen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2234">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="aa5bc-2235">Ereignishooks vor und nach der Erstellung der Teilstruktur von Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2235">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="aa5bc-2236">Abschluss für `--ids`-Parameter hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2236">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="aa5bc-2237">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2237">Network</span></span>

* <span data-ttu-id="aa5bc-2238">[#5936](https://github.com/Azure/azure-cli/issues/5936) behoben: `application-gateway create`-Tags konnten nicht festgelegt werden</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2238">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="aa5bc-2239">Argument `--auth-certs` zum Anfügen von Authentifizierungszertifikaten für `application-gateway http-settings [create|update]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2239">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="aa5bc-2240">#4910</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2240">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="aa5bc-2241">`ddos-protection`-Befehle zum Erstellen von DDoS-Schutzplänen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2241">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="aa5bc-2242">Unterstützung von `--ddos-protection-plan` für `vnet [create|update]` hinzugefügt, um das Zuordnen eines VNET zu einem DDoS-Schutzplan zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2242">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="aa5bc-2243">Problem mit `--disable-bgp-route-propagation`-Flag in `network route-table [create|update]` behoben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2243">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="aa5bc-2244">Dummy-Argumente `--public-ip-address-type` und `--subnet-type` für `network lb [create|update]` entfernt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2244">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="aa5bc-2245">Unterstützung für TXT-Datensätze mit RFC 1035-Escapesequenzen für `network dns zone [import|export]` und `network dns record-set txt add-record` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2245">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="aa5bc-2246">Profil</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2246">Profile</span></span>

* <span data-ttu-id="aa5bc-2247">Unterstützung für klassische Azure-Konten in `account list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2247">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="aa5bc-2248">[BREAKING CHANGE]`--msi` & `--msi-port`-Argumente entfernt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2248">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="aa5bc-2249">RDBMS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2249">RDBMS</span></span>

* <span data-ttu-id="aa5bc-2250">Befehl `georestore` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2250">Added `georestore` command</span></span>
* <span data-ttu-id="aa5bc-2251">Speichergrößenbeschränkung aus Befehl `create` entfernt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2251">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="aa5bc-2252">Resource</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2252">Resource</span></span>

* <span data-ttu-id="aa5bc-2253">Unterstützung für `--metadata` zu `policy definition create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2253">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="aa5bc-2254">Unterstützung von `--metadata`, `--set`, `--add`, `--remove` für `policy definition update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2254">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="aa5bc-2255">SQL</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2255">SQL</span></span>

* <span data-ttu-id="aa5bc-2256">`sql elastic-pool op list` und `sql elastic-pool op cancel` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2256">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="aa5bc-2257">Storage</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2257">Storage</span></span>

* <span data-ttu-id="aa5bc-2258">Fehlermeldungen für falsch formatierte Verbindungszeichenfolgen verbessert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2258">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="aa5bc-2259">VM</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2259">VM</span></span>

* <span data-ttu-id="aa5bc-2260">Unterstützung für die Konfiguration der Plattform-Fehlerdomänenanzahl für `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2260">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="aa5bc-2261">`vmss create` geändert, damit standardmäßig „Standard LB“ für zonales, großes oder per einzelner Platzierungsgruppe deaktiviertes Scale Set festgelegt wird</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2261">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret`
* <span data-ttu-id="aa5bc-2263">Unterstützung für SKU mit öffentlicher IP für `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2263">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="aa5bc-2264">Argumente `--keyvault` und `--resource-group` für `vm secret format` hinzugefügt, um Szenarien zu unterstützen, bei denen der Befehl die Tresor-ID nicht auflösen kann.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2264">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="aa5bc-2265">#5718</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2265">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="aa5bc-2266">Bessere Fehler für `[vm|vmss create]`, wenn der Standort einer Ressourcengruppe keine Zonenunterstützung aufweist</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2266">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="aa5bc-2267">27. März 2018</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2267">March 27, 2018</span></span>

<span data-ttu-id="aa5bc-2268">Version 2.0.30</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2268">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="aa5bc-2269">Core</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2269">Core</span></span>

* <span data-ttu-id="aa5bc-2270">Anzeigen einer Meldung für Erweiterungen, die in der Hilfe als Vorschauversion gekennzeichnet sind</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2270">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="aa5bc-2271">ACS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2271">ACS</span></span>

* <span data-ttu-id="aa5bc-2272">Behebung eines Fehlers bei der SSL-Zertifikatprüfung für `aks install-cli` in Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2272">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="aa5bc-2273">AppService</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2273">Appservice</span></span>

* <span data-ttu-id="aa5bc-2274">Unterstützung nur von HTTPS zu `webapp update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2274">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="aa5bc-2275">Unterstützung für Slots zu `az webapp identity [assign|show]` und `az functionapp identity [assign|show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2275">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="aa5bc-2276">Backup</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2276">Backup</span></span>

* <span data-ttu-id="aa5bc-2277">Neuer Befehl `az backup protection isenabled-for-vm` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2277">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="aa5bc-2278">Mit diesem Befehl kann überprüft werden, ob ein virtueller Computer von einem beliebigen Tresor im Abonnement gesichert wird.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2278">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="aa5bc-2279">Azure-Objekt-IDs für Parameter `--resource-group` und `--vault-name` für die folgenden Befehle aktiviert:</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2279">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="aa5bc-2280">`--name`-Parameter wurden geändert, um das Ausgabeformat von `backup ... show`-Befehlen zu akzeptieren.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2280">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="aa5bc-2281">Container</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2281">Container</span></span>

* <span data-ttu-id="aa5bc-2282">Befehl `container exec` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2282">Added `container exec` command.</span></span> <span data-ttu-id="aa5bc-2283">Ausführung von Befehlen in einem Container für eine ausgeführte Containergruppe</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2283">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="aa5bc-2284">Zulassen der Tabellenausgabe zum Erstellen und Aktualisieren einer Containergruppe</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2284">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="aa5bc-2285">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2285">Extension</span></span>

* <span data-ttu-id="aa5bc-2286">Meldung für `extension add` hinzugefügt, wenn sich die Erweiterung in der Vorschauphase befindet</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2286">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="aa5bc-2287">`extension list-available` geändert, um vollständige Erweiterungsdaten mit `--show-details` anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2287">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="aa5bc-2288">[BREAKING CHANGE]`extension list-available` geändert, um standardmäßig vereinfachte Erweiterungsdaten anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2288">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="aa5bc-2289">Interactive</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2289">Interactive</span></span>

* <span data-ttu-id="aa5bc-2290">Vervollständigungen wurden geändert und werden jetzt aktiviert, sobald das Laden der Befehlstabelle abgeschlossen ist.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2290">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="aa5bc-2291">Fehler bei der Verwendung des Parameters `--style` behoben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2291">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="aa5bc-2292">Interaktiver Lexer nach Befehlstabellensicherung instanziiert (sofern nicht vorhanden)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2292">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="aa5bc-2293">Verbesserte Unterstützung der Vervollständigung</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2293">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="aa5bc-2294">Labor</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2294">Lab</span></span>

* <span data-ttu-id="aa5bc-2295">Probleme mit Befehl `create environment` behoben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2295">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="aa5bc-2296">Überwachen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2296">Monitor</span></span>

* <span data-ttu-id="aa5bc-2297">Unterstützung für `--top`, `--orderby` und `--namespace` zu `metrics list` hinzugefügt [Nr. 5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2297">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="aa5bc-2298">[#4529](https://github.com/Azure/azure-cli/issues/5785) behoben: `metrics list` akzeptiert eine durch Leerzeichen getrennte Liste von abzurufenden Metriken</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2298">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="aa5bc-2299">Unterstützung für `--namespace` zu `metrics list-definitions` hinzugefügt [Nr. 5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2299">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="aa5bc-2300">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2300">Network</span></span>

* <span data-ttu-id="aa5bc-2301">Unterstützung für private DNS-Zonen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2301">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="aa5bc-2302">Profil</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2302">Profile</span></span>

* <span data-ttu-id="aa5bc-2303">Warnung für `--identity-port` und `--msi-port` zu `login` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2303">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="aa5bc-2304">RDBMS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2304">RDBMS</span></span>

* <span data-ttu-id="aa5bc-2305">GA-API-Version 2017-12-01 (Geschäftsmodell) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2305">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="aa5bc-2306">Resource</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2306">Resource</span></span>

* [BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="aa5bc-2308">Role</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2308">Role</span></span>

* <span data-ttu-id="aa5bc-2309">Unterstützung für erforderliche Zugriffskonfigurationen und native Clients zu `az ad app create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2309">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="aa5bc-2310">`rbac`-Befehle geändert, um maximal 1.000 IDs für Objektauflösung zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2310">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="aa5bc-2311">Befehle zur Verwaltung von Anmeldeinformationen (`ad sp credential [reset|list|delete]`) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2311">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="aa5bc-2312">[BREAKING CHANGE] „properties“ aus `az role assignment [list|show]`-Ausgabe entfernt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2312">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="aa5bc-2313">Unterstützung für `dataActions`- und `notDataActions`-Berechtigungen zu `role definition` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2313">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="aa5bc-2314">Storage</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2314">Storage</span></span>

* <span data-ttu-id="aa5bc-2315">Problem beim Hochladen von Dateien mit einer Größe von 195 GB bis 200 GB behoben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2315">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="aa5bc-2316">[#4049](https://github.com/Azure/azure-cli/issues/4049) behoben: Probleme bei Uploads von Anfügeblobs behoben, die ein Ignorieren der Bedingungsparameter verursacht haben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2316">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="aa5bc-2317">VM</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2317">VM</span></span>

* <span data-ttu-id="aa5bc-2318">Warnung für anstehende BREAKING CHANGEen für Sätze mit mehr als 100 Instanzen zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2318">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="aa5bc-2319">Unterstützung der Zonenresilienz zu `vm [snapshot|image]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2319">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="aa5bc-2320">Datenträgerinstanzansicht geändert, um besseren Verschlüsselungsstatus zu melden</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2320">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="aa5bc-2321">[BREAKING CHANGE]`vm extension delete` geändert, um keine Ausgabe mehr zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2321">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="aa5bc-2322">13. März 2018</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2322">March 13, 2018</span></span>

<span data-ttu-id="aa5bc-2323">Version 2.0.29</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2323">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="aa5bc-2324">ACR</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2324">ACR</span></span>

* <span data-ttu-id="aa5bc-2325">Unterstützung für den Parameter `--image` zu `repository delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2325">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="aa5bc-2326">Parameter `--manifest` und `--tag` des Befehls `repository delete` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2326">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="aa5bc-2327">Befehl `repository untag` zum Entfernen eines Tags ohne das Löschen von Daten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2327">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="aa5bc-2328">ACS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2328">ACS</span></span>

* <span data-ttu-id="aa5bc-2329">Befehl `aks upgrade-connector` zum Aktualisieren eines vorhandenen Connectors hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2329">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="aa5bc-2330">`kubectl`-Konfigurationsdateien zur Verwendung von besser lesbarem YAML im Blockstil geändert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2330">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="aa5bc-2331">Advisor</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2331">Advisor</span></span>

* <span data-ttu-id="aa5bc-2332">[BREAKING CHANGE]`advisor configuration get` in `advisor configuration list` umbenannt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2332">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="aa5bc-2333">[BREAKING CHANGE]`advisor configuration set` in `advisor configuration update` umbenannt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2333">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="aa5bc-2334">[BREAKING CHANGE]`advisor recommendation generate` entfernt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2334">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="aa5bc-2335">Parameter `--refresh` zu `advisor recommendation list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2335">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="aa5bc-2336">Befehl `advisor recommendation show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2336">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="aa5bc-2337">AppService</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2337">Appservice</span></span>

* <span data-ttu-id="aa5bc-2338">`[webapp|functionapp] assign-identity` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2338">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="aa5bc-2339">Befehle `webapp identity [assign|show]` und `functionapp identity [assign|show]` für verwaltete Identität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2339">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="aa5bc-2340">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2340">Eventhubs</span></span>

* <span data-ttu-id="aa5bc-2341">Erste Veröffentlichung</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2341">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="aa5bc-2342">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2342">Extension</span></span>

* <span data-ttu-id="aa5bc-2343">Überprüfung zum Warnen von Benutzern hinzugefügt, wenn sich die verwendete Distribution von der in der Paketquelldatei gespeicherten Distribution unterscheidet, da dies Fehlern führen kann</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2343">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="aa5bc-2344">Interactive</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2344">Interactive</span></span>

* <span data-ttu-id="aa5bc-2345">[#5625](https://github.com/Azure/azure-cli/issues/5625) behoben: Verlauf über verschiedene Sitzungen hinweg beibehalten</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2345">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="aa5bc-2346">[#3016](https://github.com/Azure/azure-cli/issues/3016) behoben: Verlauf nicht aufgezeichnet, obwohl er innerhalb des Bereichs liegt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2346">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="aa5bc-2347">[#5688](https://github.com/Azure/azure-cli/issues/5688) behoben: Abschlüsse wurden nicht angezeigt, wenn beim Laden der Befehlstabelle eine Ausnahme aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2347">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="aa5bc-2348">Statusanzeige für lang ausgeführte Vorgänge korrigiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2348">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="aa5bc-2349">Überwachen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2349">Monitor</span></span>

* <span data-ttu-id="aa5bc-2350">`monitor autoscale-settings`-Befehle als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2350">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="aa5bc-2351">Befehle vom Typ `monitor autoscale` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2351">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="aa5bc-2352">Befehle vom Typ `monitor autoscale profile` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2352">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="aa5bc-2353">Befehle vom Typ `monitor autoscale rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2353">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="aa5bc-2354">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2354">Network</span></span>

* <span data-ttu-id="aa5bc-2355">[BREAKING CHANGE] Parameter `--tags` aus `route-filter rule create` entfernt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2355">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="aa5bc-2356">Einige fehlerhafte Standardwerte für die folgenden Befehle entfernt:</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2356">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="aa5bc-2357">`network watcher connection-monitor`-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2357">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="aa5bc-2358">Parameter `--vnet` und `--subnet` zu `network watcher show-topology` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2358">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="aa5bc-2359">Profil</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2359">Profile</span></span>

* <span data-ttu-id="aa5bc-2360">Parameter `--msi` für `az login` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2360">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="aa5bc-2361">Parameter `--identity` für `az login` als Ersatz vor `--msi` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2361">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="aa5bc-2362">RDBMS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2362">RDBMS</span></span>

* <span data-ttu-id="aa5bc-2363">[VORSCHAU] Geändert, sodass die API „2017-12-01-preview“ verwendet wird</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2363">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="aa5bc-2364">Service Bus</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2364">Service Bus</span></span>

* <span data-ttu-id="aa5bc-2365">Erste Veröffentlichung</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2365">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="aa5bc-2366">Storage</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2366">Storage</span></span>

* <span data-ttu-id="aa5bc-2367">[#4971](https://github.com/Azure/azure-cli/issues/4971) behoben: `storage blob copy` unterstützt jetzt andere Azure-Clouds.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2367">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="aa5bc-2368">[#5286](https://github.com/Azure/azure-cli/issues/5286) behoben: Batchbefehle `storage blob [delete-batch|download-batch|upload-batch]` lösen bei Vorbedingungsfehlern keinen Fehler mehr aus</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2368">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="aa5bc-2369">VM</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2369">VM</span></span>

* <span data-ttu-id="aa5bc-2370">`[vm|vmss] create` unterstützt jetzt das Anfügen nicht verwalteter Datenträger und das Konfigurieren der Zwischenspeicherung.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2370">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="aa5bc-2371">`[vm|vmss] assign-identity` und `[vm|vmss] remove-identity` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2371">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="aa5bc-2372">Befehle `vm identity [assign|remove|show]` und `vmss identity [assign|remove|show]` als Ersatz für veraltete Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2372">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="aa5bc-2373">Standardpriorität in `vmss create` auf „Keine“ geändert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2373">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="aa5bc-2374">27. Februar 2018</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2374">February 27, 2018</span></span>

<span data-ttu-id="aa5bc-2375">Version 2.0.28</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2375">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="aa5bc-2376">Core</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2376">Core</span></span>

* <span data-ttu-id="aa5bc-2377">[#5184](https://github.com/Azure/azure-cli/issues/5184) behoben: Problem beim Installieren von Homebrew</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2377">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="aa5bc-2378">Unterstützung für Erweiterungstelemetrie mit benutzerdefinierten Schlüsseln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2378">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="aa5bc-2379">HTTP-Protokollierung zu `--debug` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2379">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="aa5bc-2380">ACS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2380">ACS</span></span>

* <span data-ttu-id="aa5bc-2381">Geändert, sodass für `aks install-connector` standardmäßig das Helm-Diagramm `virtual-kubelet-for-aks` verwendet wird</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2381">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="aa5bc-2382">Problem behoben: Unzureichende Berechtigungen für Dienstprinzipale zum Erstellen einer ACI-Containergruppe</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2382">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="aa5bc-2383">Parameter `--aci-container-group`, `--location` und `--image-tag` zu `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2383">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="aa5bc-2384">Veraltungshinweis aus `aks get-versions` entfernt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2384">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="aa5bc-2385">AppService</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2385">Appservice</span></span>

* <span data-ttu-id="aa5bc-2386">Updates für die neue SDK-Version (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2386">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="aa5bc-2387">[5538](https://github.com/Azure/azure-cli/issues/5538) behoben: `Free` wurde als ungültige SKU gemeldet.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2387">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="aa5bc-2388">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2388">Cognitive Services</span></span>

* <span data-ttu-id="aa5bc-2389">Hinweis beim Erstellen eines neuen Cognitive Services-Kontos aktualisiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2389">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="aa5bc-2390">Nutzung</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2390">Consumption</span></span>

* <span data-ttu-id="aa5bc-2391">Neue Befehle für PriceSheet-API hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2391">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="aa5bc-2392">Vorhandene Formate für Nutzungsdetails und Reservierungsdetails aktualisiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2392">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="aa5bc-2393">Container</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2393">Container</span></span>

* <span data-ttu-id="aa5bc-2394">Argumente `--secrets` und `--secrets-mount-path` zu `container create` hinzugefügt, um Geheimnisse in ACI verwenden zu können</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2394">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="aa5bc-2395">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2395">Network</span></span>

* <span data-ttu-id="aa5bc-2396">[#5559](https://github.com/Azure/azure-cli/issues/5559) behoben: Fehlender Client in `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2396">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="aa5bc-2397">Resource</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2397">Resource</span></span>

* <span data-ttu-id="aa5bc-2398">`group deployment export` geändert, um eine partielle Vorlage und ggf. Fehler anzuzeigen, wenn der Vorgang nicht erfolgreich war</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2398">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="aa5bc-2399">Role</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2399">Role</span></span>

* <span data-ttu-id="aa5bc-2400">`role assignment list-changelogs` hinzugefügt, um die Überprüfung von Dienstprinzipalrollen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2400">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="aa5bc-2401">SQL</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2401">SQL</span></span>

* <span data-ttu-id="aa5bc-2402">Zonenredundanzunterstützung für Datenbanken und Pools für elastische Datenbanken hinzugefügt (bei Erstellung und Aktualisierung)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2402">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="aa5bc-2403">Storage</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2403">Storage</span></span>

* <span data-ttu-id="aa5bc-2404">Angabe von Zielpfad/Präfix für `storage blob [upload-batch|download-batch]` ermöglicht</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2404">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="aa5bc-2405">VM</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2405">VM</span></span>

* <span data-ttu-id="aa5bc-2406">Unterstützung für das Anfügen/Trennen von Datenträgern für eine einzelne VMSS-Instanz hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2406">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="aa5bc-2407">13. Februar 2018</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2407">February 13, 2018</span></span>

<span data-ttu-id="aa5bc-2408">Version 2.0.27</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2408">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="aa5bc-2409">Core</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2409">Core</span></span>

* <span data-ttu-id="aa5bc-2410">Authentifizierung für Abonnement-ID und Namen bei der MSI-Anmeldung in Authentifizierung mit Schlüssel geändert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2410">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="aa5bc-2411">ACS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2411">ACS</span></span>

* <span data-ttu-id="aa5bc-2412">[BREAKING CHANGE]`aks get-versions` aus Gründen der Genauigkeit in `aks get-upgrades` umbenannt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2412">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="aa5bc-2413">`aks get-versions` zur Anzeige der verfügbaren Kubernetes-Versionen für `aks create` geändert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2413">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="aa5bc-2414">Standardwerte von `aks create` in Auswahl der Kubernetes-Version durch den Server geändert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2414">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="aa5bc-2415">Hilfemeldungen zu dem von AKS generierten Dienstprinzipal aktualisiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2415">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="aa5bc-2416">Standardknotengrößen für `aks create` von „Standard\_D1\_v2“ in „Standard\_DS1\_v2“ geändert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2416">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="aa5bc-2417">Zuverlässigkeit der Suche nach dem Dashboardpod für `az aks browse` verbessert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2417">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="aa5bc-2418">`aks get-credentials` korrigiert, um Unicode-Fehler beim Laden von Kubernetes-Konfigurationsdateien zu behandeln</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2418">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="aa5bc-2419">Meldung zu `az aks install-cli` hinzugefügt, um das Abrufen von `kubectl` in `$PATH` zu erleichtern</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2419">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="aa5bc-2420">AppService</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2420">Appservice</span></span>

* <span data-ttu-id="aa5bc-2421">Problem behoben, das zu einem Fehler von `webapp [backup|restore]` aufgrund eines Nullverweises führte</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2421">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="aa5bc-2422">Unterstützung für Standard-App Service-Pläne durch `az configure --defaults appserviceplan=my-asp` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2422">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="aa5bc-2423">CDN</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2423">CDN</span></span>

* <span data-ttu-id="aa5bc-2424">Befehle vom Typ `cdn custom-domain [enable-https|disable-https]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2424">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="aa5bc-2425">Container</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2425">Container</span></span>

* <span data-ttu-id="aa5bc-2426">Option `--follow` zu `az container logs` für Streamingprotokolle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2426">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="aa5bc-2427">Befehl `container attach` hinzugefügt, der die lokale Standardausgabe und Fehlerdatenströme an einen Container in einer Containergruppe angefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2427">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="aa5bc-2428">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2428">CosmosDB</span></span>

* <span data-ttu-id="aa5bc-2429">Unterstützung für Einstellungsfunktionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2429">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="aa5bc-2430">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2430">Extension</span></span>

* <span data-ttu-id="aa5bc-2431">Unterstützung für den Parameter `--pip-proxy` zu Befehlen vom Typ `az extension [add|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2431">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="aa5bc-2432">Unterstützung für das Argument `--pip-extra-index-urls` zu Befehlen vom Typ `az extension [add|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2432">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="aa5bc-2433">Feedback</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2433">Feedback</span></span>

* <span data-ttu-id="aa5bc-2434">Erweiterungsinformationen zu Telemetriedaten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2434">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="aa5bc-2435">Interactive</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2435">Interactive</span></span>

* <span data-ttu-id="aa5bc-2436">Problem behoben, aufgrund dessen der Benutzer bei Verwendung des interaktiven Modus in Cloud Shell zur Anmeldung aufgefordert wird</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2436">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="aa5bc-2437">Regression mit fehlenden Parametervervollständigungen korrigiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2437">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="aa5bc-2438">IoT</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2438">IoT</span></span>

* <span data-ttu-id="aa5bc-2439">Problem behoben, aufgrund dessen `iot dps access policy [create|update]` bei erfolgreicher Ausführung einen Fehler „nicht gefunden“ zurückgibt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2439">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="aa5bc-2440">Problem behoben, aufgrund dessen `iot dps linked-hub [create|update]` bei erfolgreicher Ausführung einen Fehler „nicht gefunden“ zurückgibt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2440">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="aa5bc-2441">Unterstützung für `--no-wait` zu `iot dps access policy [create|update]` und `iot dps linked-hub [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2441">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="aa5bc-2442">`iot hub create` geändert, um die Angabe der Anzahl von Partitionen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2442">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="aa5bc-2443">Überwachen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2443">Monitor</span></span>

* <span data-ttu-id="aa5bc-2444">Befehl `az monitor log-profiles create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2444">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="aa5bc-2445">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2445">Network</span></span>

* <span data-ttu-id="aa5bc-2446">Option `--tags` für folgende Befehle korrigiert:</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2446">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="aa5bc-2447">Profil</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2447">Profile</span></span>

* <span data-ttu-id="aa5bc-2448">`az login` im interaktiven Modus aktiviert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2448">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="aa5bc-2449">Resource</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2449">Resource</span></span>

* <span data-ttu-id="aa5bc-2450">`feature show` wieder hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2450">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="aa5bc-2451">Role</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2451">Role</span></span>

* <span data-ttu-id="aa5bc-2452">Argument `--available-to-other-tenants` zu `ad app update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2452">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="aa5bc-2453">SQL</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2453">SQL</span></span>

* <span data-ttu-id="aa5bc-2454">Befehle vom Typ `sql server dns-alias` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2454">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="aa5bc-2455">`sql db rename` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2455">Added `sql db rename`</span></span>
* <span data-ttu-id="aa5bc-2456">Unterstützung für das Argument `--ids` für alle SQL-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2456">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="aa5bc-2457">Storage</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2457">Storage</span></span>

* <span data-ttu-id="aa5bc-2458">Befehle `storage blob service-properties delete-policy` und `storage blob undelete` hinzugefügt, um vorläufiges Löschen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2458">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="aa5bc-2459">VM</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2459">VM</span></span>

* <span data-ttu-id="aa5bc-2460">Absturz bei unvollständiger Initialisierung der VM-Verschlüsselung behoben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2460">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="aa5bc-2461">Prinzipal-ID-Ausgabe beim Aktivieren von MSI hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2461">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="aa5bc-2462">`vm boot-diagnostics get-boot-log` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2462">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="aa5bc-2463">31. Januar 2018</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2463">January 31, 2018</span></span>

<span data-ttu-id="aa5bc-2464">Version 2.0.26</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2464">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="aa5bc-2465">Core</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2465">Core</span></span>

* <span data-ttu-id="aa5bc-2466">Unterstützung für das Abrufen von unformatierten Token im MSI-Kontext hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2466">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="aa5bc-2467">Abrufindikator-Zeichenfolge nach Fertigstellung von LRO für die Windows-Datei „cmd.exe“ entfernt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2467">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="aa5bc-2468">Warnung hinzugefügt, die angezeigt wird, wenn ein konfigurierter Standardwert in einen Eintrag auf INFO-Ebene geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2468">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="aa5bc-2469">`--verbose` zum Anzeigen verwenden.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2469">Use `--verbose` to see</span></span>
* <span data-ttu-id="aa5bc-2470">Statusanzeige für Wait-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2470">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="aa5bc-2471">ACS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2471">ACS</span></span>

* <span data-ttu-id="aa5bc-2472">Argument `--disable-browser` erläutert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2472">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="aa5bc-2473">Vervollständigung mit der TAB-TASTE für Argumente vom Typ `--vm-size` verbessert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2473">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="aa5bc-2474">AppService</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2474">Appservice</span></span>

* <span data-ttu-id="aa5bc-2475">`webapp log [tail|download]` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2475">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="aa5bc-2476">Überprüfung `kind` für Web-Apps und Funktionen entfernt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2476">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="aa5bc-2477">CDN</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2477">CDN</span></span>

* <span data-ttu-id="aa5bc-2478">Problem mit fehlendem Client für `cdn custom-domain create` behoben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2478">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="aa5bc-2479">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2479">CosmosDB</span></span>

* <span data-ttu-id="aa5bc-2480">Parameterbeschreibung für Failoverrichtlinien korrigiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2480">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="aa5bc-2481">Interactive</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2481">Interactive</span></span>

* <span data-ttu-id="aa5bc-2482">Problem behoben, aufgrund dessen Vervollständigungen von Befehlsoptionen nicht mehr angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2482">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="aa5bc-2483">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2483">Network</span></span>

* <span data-ttu-id="aa5bc-2484">Schutz für `--cert-password` zu `application-gateway create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2484">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="aa5bc-2485">Problem mit `application-gateway update` behoben, aufgrund dessen `--sku` fälschlicherweise einen Standardwert anwendete</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2485">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="aa5bc-2486">Schutz für `--shared-key` und `--authorization-key` zu `vpn-connection create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2486">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="aa5bc-2487">Problem mit fehlendem Client für `asg create` behoben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2487">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="aa5bc-2488">Parameter `--file-name / -f` für exportierte Namen zu `dns zone export` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2488">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="aa5bc-2489">Folgende Probleme mit `dns zone export` behoben:</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2489">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="aa5bc-2490">Problem behoben, aufgrund dessen lange TXT-Einträge nicht korrekt exportiert wurden</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2490">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="aa5bc-2491">Problem behoben, aufgrund dessen TXT-Einträge in Anführungszeichen fälschlich ohne Anführungszeichen in Escapezeichen exportiert wurden</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2491">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="aa5bc-2492">Problem behoben, aufgrund dessen bestimmte Datensätze zweimal mit `dns zone import` importiert wurden</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2492">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="aa5bc-2493">Befehle `vnet-gateway root-cert` und `vnet-gateway revoked-cert` wiederhergestellt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2493">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="aa5bc-2494">Profil</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2494">Profile</span></span>

* <span data-ttu-id="aa5bc-2495">`get-access-token` zur Verwendung auf einer VM mit Identität korrigiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2495">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="aa5bc-2496">Resource</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2496">Resource</span></span>

* <span data-ttu-id="aa5bc-2497">Fehler mit `deployment [create|validate]` korrigiert, aufgrund dessen fälschlich eine Warnung angezeigt wurde, wenn ein Vorlagenfeld „Typ“ Werte in Großbuchstaben enthielt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2497">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="aa5bc-2498">Storage</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2498">Storage</span></span>

* <span data-ttu-id="aa5bc-2499">Problem mit der Migration von Storage V1-Konten zu Storage V2 behoben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2499">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="aa5bc-2500">Statusberichterstellung für alle Upload-/Downloadbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2500">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="aa5bc-2501">Fehler korrigiert, der die Verwendung der arg-Option „-n“ mit `storage account check-name` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2501">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="aa5bc-2502">Spalte „Momentaufnahme“ zur Tabellenausgabe für `blob [list|show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2502">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="aa5bc-2503">Fehler mit verschiedenen Parametern korrigiert, die als Int-Typen analysiert werden mussten</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2503">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="aa5bc-2504">VM</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2504">VM</span></span>

* <span data-ttu-id="aa5bc-2505">Befehl `vm image accept-terms` hinzugefügt, um die Erstellung von VMs aus Images mit zusätzlichen Gebühren zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2505">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="aa5bc-2506">`[vm|vmss create]` korrigiert, um sicherzustellen, dass Befehle unter einem Proxy mit nicht signierten Zertifikaten ausgeführt werden können</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2506">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="aa5bc-2507">[VORSCHAU] Unterstützung für „niedrige“ Priorität zu VMSS hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2507">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="aa5bc-2508">Schutz für `--admin-password` zu `[vm|vmss] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2508">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="aa5bc-2509">17. Januar 2018</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2509">January 17, 2018</span></span>

<span data-ttu-id="aa5bc-2510">Version 2.0.25</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2510">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="aa5bc-2511">ACR</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2511">ACR</span></span>

* <span data-ttu-id="aa5bc-2512">Fallback auf ACR-Anmeldung bei Fehlern mit Windows-Anmeldeinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2512">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="aa5bc-2513">Registrierungsprotokolle aktiviert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2513">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="aa5bc-2514">ACS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2514">ACS</span></span>

* <span data-ttu-id="aa5bc-2515">Befehl `get-credentials` korrigiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2515">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="aa5bc-2516">SPN-Rollenanforderung entfernt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2516">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="aa5bc-2517">AppService</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2517">Appservice</span></span>

* <span data-ttu-id="aa5bc-2518">Fehler mit `config ssl upload` behoben, bei dem `hosting_environment_profile` NULL war</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2518">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="aa5bc-2519">Unterstützung benutzerdefinierter URLs zu `browse` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2519">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="aa5bc-2520">Slotunterstützung für `log tail` korrigiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2520">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="aa5bc-2521">Backup</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2521">Backup</span></span>

* <span data-ttu-id="aa5bc-2522">Option `--container-name` von `backup item list` geändert (ist jetzt optional)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2522">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="aa5bc-2523">Speicherkontooptionen zu `backup restore restore-disks` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2523">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="aa5bc-2524">Standortüberprüfung in `backup protection enable-for-vm` korrigiert (Groß-/Kleinschreibung wird jetzt nicht mehr beachtet)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2524">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="aa5bc-2525">Problem behoben, durch das bei Befehlen mit ungültigem Containernamen ein Fehler auftrat</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2525">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="aa5bc-2526">`backup item list` geändert (Integritätsstatus jetzt standardmäßig enthalten)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2526">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="aa5bc-2527">Batch</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2527">Batch</span></span>

* <span data-ttu-id="aa5bc-2528">`batch login` geändert, um Authentifizierungsdetails zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2528">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="aa5bc-2529">Cloud</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2529">Cloud</span></span>

* <span data-ttu-id="aa5bc-2530">Beim Festlegen von `--profile` für eine Cloud werden nun keine Endpunkte mehr benötigt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2530">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="aa5bc-2531">Nutzung</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2531">Consumption</span></span>

* <span data-ttu-id="aa5bc-2532">Neue Befehle für Reservierungen hinzugefügt: `consumption reservations summaries` und `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2532">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="aa5bc-2533">Event Grid</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2533">Event Grid</span></span>

* <span data-ttu-id="aa5bc-2534">[BREAKING CHANGE] Die Befehle vom Typ `az eventgrid topic event-subscription` wurden in `eventgrid event-subscription` verschoben.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2534">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="aa5bc-2535">[BREAKING CHANGE] Die Befehle vom Typ `az eventgrid resource event-subscription` wurden in `eventgrid event-subscription` verschoben.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2535">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="aa5bc-2536">[BREAKING CHANGE] Der Befehl `eventgrid event-subscription show-endpoint-url` wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2536">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="aa5bc-2537">Verwenden Sie stattdessen `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2537">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="aa5bc-2538">Befehl `eventgrid topic update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2538">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="aa5bc-2539">Befehl `eventgrid event-subscription update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2539">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="aa5bc-2540">Parameter `--ids` für Befehle vom Typ `eventgrid topic` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2540">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="aa5bc-2541">Unterstützung der Vervollständigung mit der TAB-TASTE für Themennamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2541">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="aa5bc-2542">Interactive</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2542">Interactive</span></span>

* <span data-ttu-id="aa5bc-2543">Problem behoben, das dazu führte, dass der interaktive Modus nicht mit Python 2.x verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2543">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="aa5bc-2544">Fehler beim Start behoben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2544">Fixed errors on startup</span></span>
* <span data-ttu-id="aa5bc-2545">Problem behoben, das dazu führte, dass einige Befehle nicht im interaktiven Modus ausgeführt werden konnten</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2545">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="aa5bc-2546">IoT</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2546">IoT</span></span>

* <span data-ttu-id="aa5bc-2547">Unterstützung für Gerätebereitstellungsdienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2547">Added support for device provisioning service</span></span>
* <span data-ttu-id="aa5bc-2548">Benachrichtigungen zu veralteten Elementen in Befehlen und in der Befehlshilfe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2548">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="aa5bc-2549">IoT-Überprüfung hinzugefügt, um Benutzer über die IoT-Erweiterung zu informieren</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2549">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="aa5bc-2550">Überwachen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2550">Monitor</span></span>

* <span data-ttu-id="aa5bc-2551">Unterstützung mehrerer Diagnoseeinstellung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2551">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="aa5bc-2552">Der Parameter `--name` ist nun für `az monitor diagnostic-settings create` erforderlich.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2552">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="aa5bc-2553">Befehl `monitor diagnostic-settings categories` zum Abrufen der Diagnoseeinstellungskategorie hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2553">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="aa5bc-2554">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2554">Network</span></span>

* <span data-ttu-id="aa5bc-2555">Problem behoben, das beim Ändern des aktiven Standbymodus mit `vnet-gateway update` auftrat</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2555">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="aa5bc-2556">Unterstützung für HTTP2 zu `application-gateway [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2556">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="aa5bc-2557">Profil</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2557">Profile</span></span>

* <span data-ttu-id="aa5bc-2558">Unterstützung für die Anmeldung mit durch Benutzer zugewiesenen Identitäten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2558">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="aa5bc-2559">Role</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2559">Role</span></span>

* <span data-ttu-id="aa5bc-2560">Argument `--assignee-object-id` zu `role assignment create` hinzugefügt, um Graph-Abfrage zu umgehen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2560">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="aa5bc-2561">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2561">Service Fabric</span></span>

* <span data-ttu-id="aa5bc-2562">Ausführliche Fehler zur Überprüfungsantwort bei der Clustererstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2562">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="aa5bc-2563">Problem mit fehlendem Client für verschiedene Befehle behoben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2563">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="aa5bc-2564">VM</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2564">VM</span></span>

* <span data-ttu-id="aa5bc-2565">[VORSCHAUVERSION] Zonenübergreifende Unterstützung für `vmss`</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2565">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="aa5bc-2566">[BREAKING CHANGE] Standard für Einzelzone (`vmss`) in Standardlastenausgleich geändert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2566">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="aa5bc-2567">[BREAKING CHANGE]`externalIdentities` in `userAssignedIdentities` geändert für EMSI</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2567">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="aa5bc-2568">[VORSCHAUVERSION] Unterstützung für Austausch des Betriebssystemdatenträgers hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2568">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="aa5bc-2569">Unterstützung der Verwendung von VM-Images aus anderen Abonnements hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2569">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="aa5bc-2570">Argumente `--plan-name`, `--plan-product`, `--plan-promotion-code` und `--plan-publisher` zu `[vm|vmss] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2570">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="aa5bc-2571">Fehlerbedingte Probleme mit `[vm|vmss] create` behoben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2571">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="aa5bc-2572">Übermäßige Ressourcenverwendung durch `vm image list --all` behoben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2572">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="aa5bc-2573">19. Dezember 2017</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2573">December 19, 2017</span></span>

<span data-ttu-id="aa5bc-2574">Version 2.0.23</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2574">Version 2.0.23</span></span>

* <span data-ttu-id="aa5bc-2575">Unterstützung für die Anmeldung mit durch Benutzer zugewiesenen Identitäten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2575">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="aa5bc-2576">Container</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2576">Container</span></span>

* <span data-ttu-id="aa5bc-2577">Falsche Reihenfolge der Parameter für Containerprotokolle behoben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2577">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="aa5bc-2578">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2578">Network</span></span>

* <span data-ttu-id="aa5bc-2579">Argument `--disable-bgp-route-propagation` zu `route-table [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2579">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="aa5bc-2580">Argument `--ip-tags` zu `public-ip [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2580">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="aa5bc-2581">Storage</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2581">Storage</span></span>

* <span data-ttu-id="aa5bc-2582">Unterstützung für Storage V2 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2582">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="aa5bc-2583">VM</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2583">VM</span></span>

* <span data-ttu-id="aa5bc-2584">[VORSCHAUVERSION] Unterstützung für durch Benutzer zugewiesene Identitäten für virtuelle Computer und VMSSs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2584">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="aa5bc-2585">5\. Dezember 2017</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2585">December 5, 2017</span></span>

<span data-ttu-id="aa5bc-2586">Version 2.0.22</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2586">Version 2.0.22</span></span>

* <span data-ttu-id="aa5bc-2587">`az component`-Befehle wurden entfernt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2587">Removed `az component` commands.</span></span> <span data-ttu-id="aa5bc-2588">Verwenden Sie stattdessen `az extension`.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2588">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="aa5bc-2589">Core</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2589">Core</span></span>
* <span data-ttu-id="aa5bc-2590">Der `AZURE_US_GOV_CLOUD`-Autoritätsendpunkt von AAD wurde von „login.microsoftonline.com“ in „login.microsoftonline.us“ geändert.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2590">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="aa5bc-2591">Problem behoben, aufgrund dessen Telemetriedaten fortlaufend neu gesendet wurden</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2591">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="aa5bc-2592">ACS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2592">ACS</span></span>

* <span data-ttu-id="aa5bc-2593">Die Befehle `aks install-connector` und `aks remove-connector` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2593">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="aa5bc-2594">Verbesserte Fehlerberichterstellung für `acs create`</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2594">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="aa5bc-2595">Feste Verwendung von `aks get-credentials -f` ohne vollqualifizierten Pfad</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2595">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="aa5bc-2596">Advisor</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2596">Advisor</span></span>

* <span data-ttu-id="aa5bc-2597">Erste Veröffentlichung</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2597">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="aa5bc-2598">AppService</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2598">Appservice</span></span>

* <span data-ttu-id="aa5bc-2599">Erstellung feststehender Zertifikatnamen mit `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2599">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="aa5bc-2600">`webapp [list|show]` und `functionapp [list|show]` wurden verbessert, um die richtigen Apps anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2600">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="aa5bc-2601">Standardwert für `WEBSITE_NODE_DEFAULT_VERSION` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2601">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="aa5bc-2602">Nutzung</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2602">Consumption</span></span>

* <span data-ttu-id="aa5bc-2603">Unterstützung für API-Version 2017-11-30 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2603">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="aa5bc-2604">Container</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2604">Container</span></span>

* <span data-ttu-id="aa5bc-2605">Feste Regression für Standardports</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2605">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="aa5bc-2606">Überwachen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2606">Monitor</span></span>

* <span data-ttu-id="aa5bc-2607">Unterstützung mehrerer Dimensionen zu Metrikbefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2607">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="aa5bc-2608">Resource</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2608">Resource</span></span>

* <span data-ttu-id="aa5bc-2609">Argument `--include-response-body` zu `resource show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2609">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="aa5bc-2610">Role</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2610">Role</span></span>

* <span data-ttu-id="aa5bc-2611">Anzeige von Standardzuweisungen für „klassische“ Administratoren zu `role assignment list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2611">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="aa5bc-2612">Unterstützung für das Hinzufügen (anstelle der Überschreibung) von Anmeldeinformationen zu `ad sp reset-credentials` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2612">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="aa5bc-2613">Verbesserte Fehlerberichterstellung für `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2613">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="aa5bc-2614">SQL</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2614">SQL</span></span>

* <span data-ttu-id="aa5bc-2615">Die Befehle `sql db list-usages` und `sql db show-usage` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2615">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="aa5bc-2616">Die Befehle `sql server conn-policy show` und `sql server conn-policy update` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2616">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="aa5bc-2617">VM</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2617">VM</span></span>

* <span data-ttu-id="aa5bc-2618">Zoneninformationen zu `az vm list-skus` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2618">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="aa5bc-2619">14. November 2017</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2619">November 14, 2017</span></span>

<span data-ttu-id="aa5bc-2620">Version 2.0.21</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2620">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="aa5bc-2621">ACR</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2621">ACR</span></span>

* <span data-ttu-id="aa5bc-2622">Unterstützung für das Erstellen von Webhooks in Replikationsregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2622">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="aa5bc-2623">ACS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2623">ACS</span></span>

* <span data-ttu-id="aa5bc-2624">Formulierung in AKS von „Agent“ in „Knoten“ geändert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2624">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="aa5bc-2625">Option `--orchestrator-release` für `acs create` als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2625">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="aa5bc-2626">VM-Standardgröße für AKS in `Standard_D1_v2` geändert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2626">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="aa5bc-2627">`az aks browse` für Windows korrigiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2627">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="aa5bc-2628">`az aks get-credentials` für Windows korrigiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2628">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="aa5bc-2629">AppService</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2629">Appservice</span></span>

* <span data-ttu-id="aa5bc-2630">Bereitstellungsquelle `config-zip` für Web-Apps und Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2630">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="aa5bc-2631">Option `--docker-container-logging` zu `az webapp log config` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2631">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="aa5bc-2632">Option `storage` aus dem Parameter `--web-server-logging` von `az webapp log config` entfernt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2632">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="aa5bc-2633">Fehlermeldungen für `deployment user set` verbessert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2633">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="aa5bc-2634">Unterstützung für das Erstellen von Linux-Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2634">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="aa5bc-2635">`list-locations` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2635">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="aa5bc-2636">Batch</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2636">Batch</span></span>

* <span data-ttu-id="aa5bc-2637">Fehler im Poolerstellungsbefehl korrigiert, der bei Verwendung einer Ressourcen-ID mit dem Flag `--image` aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2637">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="aa5bc-2638">BatchAI</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2638">Batchai</span></span>

* <span data-ttu-id="aa5bc-2639">Kurzoption (`-s`) für `--vm-size` zur Angabe der VM-Größe im Befehl `file-server create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2639">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="aa5bc-2640">Argumente für Speicherkontoname und -schlüssel zum Parameter `cluster create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2640">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="aa5bc-2641">Dokumentation für `job list-files` und `job stream-file` korrigiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2641">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="aa5bc-2642">Kurzoption (`-r`) für `--cluster-name` zur Angabe des Clusternamens im Befehl `job create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2642">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="aa5bc-2643">Cloud</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2643">Cloud</span></span>

* <span data-ttu-id="aa5bc-2644">`cloud [register|update]` geändert, um die Registrierung von Clouds ohne erforderliche Endpunkte zu verhindern</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2644">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="aa5bc-2645">Container</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2645">Container</span></span>

* <span data-ttu-id="aa5bc-2646">Unterstützung für das Öffnen mehrerer Ports hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2646">Added support to open multiple ports</span></span>
* <span data-ttu-id="aa5bc-2647">Neustartrichtlinie für Containergruppen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2647">Added container group restart policy</span></span>
* <span data-ttu-id="aa5bc-2648">Unterstützung zum Einbinden einer Azure-Dateifreigabe als Volume hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2648">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="aa5bc-2649">Hilfedokumente aktualisiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2649">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="aa5bc-2650">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2650">Data Lake Analytics</span></span>

* <span data-ttu-id="aa5bc-2651">`[job|account] list` geändert, um präzisere Informationen zu erhalten</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2651">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="aa5bc-2652">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2652">Data Lake Store</span></span>

* <span data-ttu-id="aa5bc-2653">`account list` geändert, um präzisere Informationen zu erhalten</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2653">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="aa5bc-2654">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2654">Extension</span></span>

* <span data-ttu-id="aa5bc-2655">`extension list-available` hinzugefügt, um das Auflisten offizieller Microsoft-Erweiterungen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2655">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="aa5bc-2656">`--name` zu `extension [add|update]` hinzugefügt, um das Installieren von Erweiterungen nach Name zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2656">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="aa5bc-2657">IoT</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2657">IoT</span></span>

* <span data-ttu-id="aa5bc-2658">Unterstützung für Zertifizierungsstellen (CAs) und Zertifikatketten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2658">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="aa5bc-2659">Überwachen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2659">Monitor</span></span>

* <span data-ttu-id="aa5bc-2660">Befehle vom Typ `activity-log alert` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2660">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="aa5bc-2661">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2661">Network</span></span>

* <span data-ttu-id="aa5bc-2662">Unterstützung für CAA-DNS-Einträge hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2662">Added support for CAA DNS records</span></span>
* <span data-ttu-id="aa5bc-2663">Problem behoben, durch das Endpunkte nicht mit `traffic-manager profile update` aktualisiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2663">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="aa5bc-2664">Problem behoben, durch das `vnet update --dns-servers` je nach VNet-Erstellungsmethode nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2664">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="aa5bc-2665">Problem behoben, durch das relative DNS-Namen durch `dns zone import` nicht korrekt importiert wurden</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2665">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="aa5bc-2666">Reservations</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2666">Reservations</span></span>

* <span data-ttu-id="aa5bc-2667">Erste Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2667">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="aa5bc-2668">Resource</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2668">Resource</span></span>

* <span data-ttu-id="aa5bc-2669">Unterstützung für Ressourcen-IDs zum Parameter `--resource` und Sperren auf Ressourcenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2669">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="aa5bc-2670">SQL</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2670">SQL</span></span>

* <span data-ttu-id="aa5bc-2671">Parameter `--ignore-missing-vnet-service-endpoint` zu `sql server vnet-rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2671">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="aa5bc-2672">Storage</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2672">Storage</span></span>

* <span data-ttu-id="aa5bc-2673">`storage account create` geändert, sodass die SKU `Standard_RAGRS` als Standard verwendet wird</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2673">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="aa5bc-2674">Fehler im Zusammenhang mit Datei-/Blobnamen korrigiert, die ASCII-fremde Zeichen enthalten</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2674">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="aa5bc-2675">Fehler korrigiert, der die Verwendung von `--source-uri` mit `storage [blob|file] copy start-batch` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2675">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="aa5bc-2676">Befehle zum Globalisieren und Löschen mehrerer Objekte mit `storage [blob|file] delete-batch` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2676">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="aa5bc-2677">Problem beim Aktivieren von Metriken mit `storage metrics update` behoben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2677">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="aa5bc-2678">Problem mit Dateien über 200 GB bei Verwendung von `storage blob upload-batch` behoben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2678">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="aa5bc-2679">Problem behoben, durch das `--bypass` und `--default-action` von `storage account [create|update]` ignoriert wurden</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2679">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="aa5bc-2680">VM</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2680">VM</span></span>

* <span data-ttu-id="aa5bc-2681">Fehler mit `vmss create` korrigiert, der die Verwendung der Größenebene `Basic` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2681">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="aa5bc-2682">`--plan`-Argumente zu `[vm|vmss] create` für benutzerdefinierte Images mit Abrechnungsinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2682">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="aa5bc-2683">Befehle hinzugefügt: `vm secret `[add|remove|list]</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2683">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="aa5bc-2684">`vm format-secret` in `vm secret format` umbenannt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2684">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="aa5bc-2685">Argument `--encrypt format` zu `vm encryption enable` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2685">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="aa5bc-2686">24. Oktober 2017</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2686">October 24, 2017</span></span>

<span data-ttu-id="aa5bc-2687">Version 2.0.20</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2687">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="aa5bc-2688">Core</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2688">Core</span></span>

* <span data-ttu-id="aa5bc-2689">Aktualisierung von `2017-03-09-profile` zur Verwendung von Version `2016-01-01` der `MGMT_STORAGE`-API</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2689">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="aa5bc-2690">ACR</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2690">ACR</span></span>

* <span data-ttu-id="aa5bc-2691">Die Ressourcenverwaltung wurde aktualisiert und verweist nun auf die API-Version `2017-10-01`.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2691">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="aa5bc-2692">SKU „Bring Your Own Storage“ wurde in „Klassisch“ geändert.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2692">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="aa5bc-2693">Die Registrierungs-SKUs wurden in „Basic“, „Standard“ und „Premium“ umbenannt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2693">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="aa5bc-2694">ACS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2694">ACS</span></span>

* <span data-ttu-id="aa5bc-2695">[VORSCHAUVERSION] Befehle vom Typ `az aks` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2695">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="aa5bc-2696">Problem mit `get-credentials` in Kubernetes behoben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2696">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="aa5bc-2697">AppService</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2697">Appservice</span></span>

* <span data-ttu-id="aa5bc-2698">Problem behoben, aufgrund dessen heruntergeladene `webapp`-Protokolle unter Umständen ungültig waren</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2698">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="aa5bc-2699">Komponente</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2699">Component</span></span>

* <span data-ttu-id="aa5bc-2700">Deutlichere Meldung zur Einstellung für alle Installer und für Bestätigungsaufforderung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2700">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="aa5bc-2701">Überwachen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2701">Monitor</span></span>

* <span data-ttu-id="aa5bc-2702">Befehle vom Typ `action-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2702">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="aa5bc-2703">Resource</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2703">Resource</span></span>

* <span data-ttu-id="aa5bc-2704">Inkompatibilität mit der aktuellen Version der msrest-Abhängigkeit in `group export` behoben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2704">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="aa5bc-2705">Problem mit `policy assignment create` behoben, sodass der Befehl mit integrierten Richtliniendefinitionen und Richtliniensatzdefinitionen verwendet werden kann</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2705">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="aa5bc-2706">VM</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2706">VM</span></span>

* <span data-ttu-id="aa5bc-2707">Argument `--accelerated-networking` zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2707">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="aa5bc-2708">9\. Oktober 2017</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2708">October 9, 2017</span></span>

<span data-ttu-id="aa5bc-2709">Version 2.0.19</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2709">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="aa5bc-2710">Core</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2710">Core</span></span>

* <span data-ttu-id="aa5bc-2711">Verarbeitung von ADFS-Autoritäts-URLs wurde mit einem nachgestellten Schrägstrich zu Azure Stack hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2711">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="aa5bc-2712">AppService</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2712">Appservice</span></span>

* <span data-ttu-id="aa5bc-2713">Mit dem neuen Befehl `webapp update` wurde ein allgemeines Update hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2713">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="aa5bc-2714">Batch</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2714">Batch</span></span>

* <span data-ttu-id="aa5bc-2715">Aktualisierung auf Batch SDK 4.0.0</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2715">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="aa5bc-2716">Die Option `--image` von „VirtualMachineConfiguration“ wurde aktualisiert, um zusätzlich zu „publish:offer:sku:version“ ARM-Imageverweise zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2716">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="aa5bc-2717">Unterstützung für das neue CLI-Erweiterungsmodell für Batch-Erweiterungsbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2717">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="aa5bc-2718">Batch-Unterstützung aus dem Komponentenmodell entfernt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2718">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="aa5bc-2719">BatchAI</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2719">Batchai</span></span>

* <span data-ttu-id="aa5bc-2720">Erste Version des Batch KI-Moduls</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2720">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="aa5bc-2721">KeyVault</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2721">Keyvault</span></span>

* <span data-ttu-id="aa5bc-2722">Key Vault-Authentifizierungsproblem behoben, das bei Verwendung von ADFS in Azure Stack auftrat.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2722">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="aa5bc-2723">(#4448)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2723">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="aa5bc-2724">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2724">Network</span></span>

* <span data-ttu-id="aa5bc-2725">Das Argument `--server` von `application-gateway address-pool create` ist nun optional, sodass leere Adresspools zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2725">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="aa5bc-2726">`traffic-manager` wurde aktualisiert, um aktuelle Features zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2726">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="aa5bc-2727">Resource</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2727">Resource</span></span>

* <span data-ttu-id="aa5bc-2728">Zusätzliche Unterstützung für `--resource-group/-g`-Optionen für Ressourcengruppennamen zu `group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2728">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="aa5bc-2729">Befehle für `account lock` hinzugefügt, um die Verwendung mit Sperren auf Abonnementebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2729">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="aa5bc-2730">Befehle für `group lock` hinzugefügt, um die Verwendung mit Sperren auf Gruppenebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2730">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="aa5bc-2731">Befehle für `resource lock` hinzugefügt, um die Verwendung mit Sperren auf Ressourcenebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2731">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="aa5bc-2732">Sql</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2732">Sql</span></span>

* <span data-ttu-id="aa5bc-2733">Unterstützung für SQL Transparent Data Encryption (TDE) und TDE für Bring Your Own Key-Szenarien hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2733">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="aa5bc-2734">Der Befehl `db list-deleted` und der Parameter `db restore --deleted-time` wurden hinzugefügt, um die Ermittlung und Wiederherstellung gelöschter Datenbanken zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2734">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="aa5bc-2735">`db op list` und `db op cancel` wurden hinzugefügt, um das Auflisten und Abbrechen ausgeführter Vorgänge für eine Datenbank zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2735">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="aa5bc-2736">Storage</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2736">Storage</span></span>

* <span data-ttu-id="aa5bc-2737">Unterstützung für Momentaufnahme von Dateifreigaben hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2737">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="aa5bc-2738">VM</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2738">Vm</span></span>

* <span data-ttu-id="aa5bc-2739">Korrektur eines Fehlers in `vm show`, bei dem die Verwendung von `-d` in Verbindung mit fehlenden privaten IP-Adressen einen Absturz verursachte</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2739">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="aa5bc-2740">[VORSCHAUVERSION] Unterstützung für paralleles Upgrade zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2740">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="aa5bc-2741">Unterstützung für das Aktualisieren der Verschlüsselungseinstellungen mit `vm encryption enable` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2741">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="aa5bc-2742">Parameter `--os-disk-size-gb` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2742">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="aa5bc-2743">Parameter `--license-type` für Windows zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2743">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="aa5bc-2744">22. September 2017</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2744">September 22, 2017</span></span>

<span data-ttu-id="aa5bc-2745">Version 2.0.18</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2745">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="aa5bc-2746">Resource</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2746">Resource</span></span>

* <span data-ttu-id="aa5bc-2747">Unterstützung für das Anzeigen integrierter Richtliniendefinitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2747">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="aa5bc-2748">Unterstützungsmodusparameter zum Erstellen von Richtliniendefinitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2748">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="aa5bc-2749">Unterstützung für UI-Definitionen und -Vorlagen zu `managedapp definition create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2749">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="aa5bc-2750">[BREAKING CHANGE] Der Ressourcentyp `managedapp` wurde von `appliances` in `applications` und von `applianceDefinitions` in `applicationDefinitions` geändert.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2750">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="aa5bc-2751">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2751">Network</span></span>

* <span data-ttu-id="aa5bc-2752">Unterstützung für Verfügbarkeitszone zu Unterbefehlen `network lb` und `network public-ip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2752">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="aa5bc-2753">Unterstützung für IPv6-Microsoft-Peering zu `express-route` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2753">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="aa5bc-2754">Befehle für Anwendungssicherheitsgruppe `asg` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2754">Added `asg` application security group commands</span></span>
* <span data-ttu-id="aa5bc-2755">Argument `--application-security-groups` zu `nic [create|ip-config create|ip-config update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2755">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="aa5bc-2756">Argumente `--source-asgs` und `--destination-asgs` zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2756">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="aa5bc-2757">Argumente `--ddos-protection` und `--vm-protection` zu `vnet [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2757">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="aa5bc-2758">Befehle vom Typ `network [vnet-gateway|vpn-client|show-url]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2758">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="aa5bc-2759">Storage</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2759">Storage</span></span>

* <span data-ttu-id="aa5bc-2760">Problem behoben, das nach der Aktualisierung des SDK unter Umständen einen Fehler der `storage account network-rule`-Befehle zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2760">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="aa5bc-2761">Eventgrid</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2761">Eventgrid</span></span>

* <span data-ttu-id="aa5bc-2762">Azure Event Grid Python SDK für die Verwendung der neueren API-Version „2017-09-15-preview“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2762">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="aa5bc-2763">SQL</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2763">SQL</span></span>

* <span data-ttu-id="aa5bc-2764">`sql server list`-Argument `--resource-group` geändert, sodass es nun optional ist.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2764">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="aa5bc-2765">Wird es nicht angegeben, werden alle SQL Server-Instanzen im Abonnement zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2765">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="aa5bc-2766">Parameter `--no-wait` zu `db [create|copy|restore|update|replica create|create|update]` und `dw [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2766">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="aa5bc-2767">KeyVault</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2767">Keyvault</span></span>

* <span data-ttu-id="aa5bc-2768">Unterstützung für die Keyvault-Befehlsausführung hinter einem Proxy hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2768">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="aa5bc-2769">VM</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2769">VM</span></span>

* <span data-ttu-id="aa5bc-2770">Unterstützung für Verfügbarkeitszone zu `[vm|vmss|disk] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2770">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="aa5bc-2771">Problem behoben, das bei Verwendung von `--app-gateway ID` mit `vmss create` einen Fehler zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2771">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="aa5bc-2772">Argument `--asgs` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2772">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="aa5bc-2773">Unterstützung für die Ausführung von Befehlen auf virtuellen Computern mit `vm run-command` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2773">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="aa5bc-2774">[VORSCHAU] Unterstützung für VMSS-Datenträgerverschlüsselung mit `vmss encryption` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2774">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="aa5bc-2775">Unterstützung für die Durchführung der Wartung auf virtuellen Computern mit `vm perform-maintenance` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2775">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="aa5bc-2776">ACS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2776">ACS</span></span>

* <span data-ttu-id="aa5bc-2777">[VORSCHAU] Argument `--orchestrator-release` zu `acs create` für ACS-Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2777">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="aa5bc-2778">AppService</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2778">Appservice</span></span>

* <span data-ttu-id="aa5bc-2779">Neue Möglichkeit zum Aktualisieren und Anzeigen der Authentifizierungseinstellungen mit `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2779">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="aa5bc-2780">Backup</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2780">Backup</span></span>

* <span data-ttu-id="aa5bc-2781">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2781">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="aa5bc-2782">11. September 2017</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2782">September 11, 2017</span></span>

<span data-ttu-id="aa5bc-2783">Version 2.0.17</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2783">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="aa5bc-2784">Core</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2784">Core</span></span>

* <span data-ttu-id="aa5bc-2785">Festlegung einer eigenen Korrelations-ID in Telemetrie durch das Befehlsmodul aktiviert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2785">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="aa5bc-2786">Ein Problem mit der JSON-Sicherungsdatei wurde behoben, das beim Festlegen des Diagnosemodus für Telemetrie auftrat</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2786">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="aa5bc-2787">ACS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2787">Acs</span></span>

* <span data-ttu-id="aa5bc-2788">Befehl `acs list-locations` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2788">Added `acs list-locations` command</span></span>
* <span data-ttu-id="aa5bc-2789">`ssh-key-file` wird mit dem erwarteten Standardwert versehen.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2789">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="aa5bc-2790">AppService</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2790">Appservice</span></span>

* <span data-ttu-id="aa5bc-2791">Neue Möglichkeit zum Erstellen einer Web-App in einer anderen Ressourcengruppe als der des aktiven Diensttarifs</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2791">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="aa5bc-2792">CDN</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2792">CDN</span></span>

* <span data-ttu-id="aa5bc-2793">Der Fehler bei `cdn custom-domain create`, dass „CustomDomain“ nicht wiederholbar ist, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2793">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="aa5bc-2794">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2794">Extension</span></span>

* <span data-ttu-id="aa5bc-2795">Erstrelease</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2795">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="aa5bc-2796">KeyVault</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2796">Keyvault</span></span>

* <span data-ttu-id="aa5bc-2797">Problem behoben, aufgrund dessen bei den Berechtigungen für `keyvault set-policy` die Groß-/Kleinschreibung beachtet werden musste</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2797">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="aa5bc-2798">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2798">Network</span></span>

* <span data-ttu-id="aa5bc-2799">`vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2799">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="aa5bc-2800">Das Argument `--private-access-services` wurde für `vnet subnet create/update` in `--service-endpoints` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2800">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="aa5bc-2801">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2801">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="aa5bc-2802">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2802">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="aa5bc-2803">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2803">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="aa5bc-2804">Resource</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2804">Resource</span></span>

* <span data-ttu-id="aa5bc-2805">Übergabe von Parameterdefinitionen für Ressourcenrichtlinien in `policy definition create` und `policy definition update` zulassen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2805">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="aa5bc-2806">Übergabe von Parameterwerten für `policy assignment create` zulassen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2806">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="aa5bc-2807">Übergabe von JSON-Code oder einer Datei für alle Parameter zulassen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2807">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="aa5bc-2808">Inkrementierte API-Version</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2808">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="aa5bc-2809">SQL</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2809">SQL</span></span>

* <span data-ttu-id="aa5bc-2810">Befehle vom Typ `sql server vnet-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2810">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="aa5bc-2811">VM</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2811">VM</span></span>

* <span data-ttu-id="aa5bc-2812">Behoben: Zugriff nur zuweisen, wenn `--scope` angegeben wird</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2812">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="aa5bc-2813">Behoben: Gleiche Erweiterungsbenennung wie Portal verwenden</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2813">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="aa5bc-2814">`subscription` aus der Ausgabe von `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2814">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="aa5bc-2815">Behoben: Speicher-SKU vom Typ `[vm|vmss] create` wird nicht auf Datenträger mit einem Image angewendet.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2815">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="aa5bc-2816">Behoben: `vm format-secret --secrets` akzeptierte keine durch neue Zeilen getrennte IDs.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2816">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="aa5bc-2817">31. August 2017</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2817">August 31, 2017</span></span>

<span data-ttu-id="aa5bc-2818">Version 2.0.16</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2818">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="aa5bc-2819">KeyVault</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2819">Keyvault</span></span>

* <span data-ttu-id="aa5bc-2820">Fehler behoben, der beim Versuch auftrat, die Geheimniscodierung mit `secret download` automatisch aufzulösen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2820">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="aa5bc-2821">Sf</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2821">Sf</span></span>

* <span data-ttu-id="aa5bc-2822">Alle Befehle wurden durch die Service Fabric-Befehlszeilenschnittstelle (sfctl) ersetzt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2822">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="aa5bc-2823">Storage</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2823">Storage</span></span>

* <span data-ttu-id="aa5bc-2824">Problem behoben, aufgrund dessen Speicherkonten nicht in Regionen erstellt werden konnten, die die NetworkACLs-Funktion nicht unterstützen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2824">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="aa5bc-2825">Festlegen des Inhaltstyps und der Inhaltscodierung während Blob- und Dateiuploads, wenn weder Inhaltstyp noch Inhaltscodierung angegeben sind</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2825">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="aa5bc-2826">28. August 2017</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2826">August 28, 2017</span></span>

<span data-ttu-id="aa5bc-2827">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2827">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="aa5bc-2828">Befehlszeilenschnittstelle (CLI)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2828">CLI</span></span>

* <span data-ttu-id="aa5bc-2829">Rechtlichen Hinweis zu `--version` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2829">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="aa5bc-2830">ACS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2830">ACS</span></span>

* <span data-ttu-id="aa5bc-2831">Vorschauregionen korrigiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2831">Corrected preview regions</span></span>
* <span data-ttu-id="aa5bc-2832">Standardmäßiges DNS-Namenspräfix (`dns_name_prefix`) ordnungsgemäß formatiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2832">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="aa5bc-2833">ACS-Befehlsausgabe optimiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2833">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="aa5bc-2834">AppService</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2834">Appservice</span></span>

* <span data-ttu-id="aa5bc-2835">[BREAKING CHANGE] Inkonsistenzen in der Ausgabe von `az webapp config appsettings [delete|set]` behoben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2835">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="aa5bc-2836">Neuen Alias (`-i`) für `az webapp config container set --docker-custom-image-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2836">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="aa5bc-2837">`az webapp log show` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2837">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="aa5bc-2838">Neue Argumente aus `az webapp delete` verfügbar gemacht, um App Service-Plan, Metriken oder DNS-Registrierung beizubehalten</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2838">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="aa5bc-2839">Behoben: Korrekte Erkennung der Sloteinstellungen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2839">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="aa5bc-2840">IoT</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2840">IoT</span></span>

* <span data-ttu-id="aa5bc-2841">#3934 behoben: Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2841">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="aa5bc-2842">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2842">Network</span></span>

* <span data-ttu-id="aa5bc-2843">[BREAKING CHANGE]`vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2843">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="aa5bc-2844">[BREAKING CHANGE] Option `--private-access-services` für `--service-endpoints` in `vnet subnet [create|update]` umbenannt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2844">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="aa5bc-2845">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2845">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="aa5bc-2846">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2846">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="aa5bc-2847">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2847">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="aa5bc-2848">Profil</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2848">Profile</span></span>

* <span data-ttu-id="aa5bc-2849">`--msi` und `--msi-port` für die Anmeldung mit der Identität eines virtuellen Computers verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2849">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="aa5bc-2850">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2850">Service Fabric</span></span>

* <span data-ttu-id="aa5bc-2851">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2851">Preview release</span></span>
* <span data-ttu-id="aa5bc-2852">Registrierungsbenutzer-/-kennwortregeln für Befehl vereinfacht</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2852">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="aa5bc-2853">Kennwortanforderung für Benutzer trotz Parameterübergabe behoben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2853">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="aa5bc-2854">Unterstützung für leere Registrierungsanmeldeinformationen (`registry_cred`) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2854">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="aa5bc-2855">Storage</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2855">Storage</span></span>

* <span data-ttu-id="aa5bc-2856">Festlegen des Blobtarifs ermöglicht</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2856">Enabled setting blob tier</span></span>
* <span data-ttu-id="aa5bc-2857">Argumente `--bypass` und `--default-action` zur Unterstützung von Diensttunneling zu `storage account [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2857">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="aa5bc-2858">Befehle zum Hinzufügen von VNet-Regeln und IP-basierten Regeln zu `storage account network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2858">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="aa5bc-2859">Dienstverschlüsselung durch vom Kunden verwalteten Schlüssel ermöglicht</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2859">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="aa5bc-2860">[BREAKING CHANGE] Option `--encryption` für Befehl `az storage account create and az storage account update` in `--encryption-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2860">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="aa5bc-2861">Behoben (4220): `az storage account update encryption` – Syntaxkonflikt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2861">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="aa5bc-2862">VM</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2862">VM</span></span>

* <span data-ttu-id="aa5bc-2863">Problem behoben, aufgrund dessen bei Verwendung von `--instance-id *` zusätzliche, fehlerhafte Informationen für `vmss get-instance-view` angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2863">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="aa5bc-2864">Unterstützung für `--lb-sku` zu `vmss create` hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2864">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="aa5bc-2865">Menschliche Namen aus der Administratornamen-Blacklist für `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2865">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="aa5bc-2866">Problem behoben, aufgrund dessen `[vm|vmss] create` einen Fehler ausgelöst hat, wenn aus einem Image keine Tarifinformationen extrahiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2866">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="aa5bc-2867">Absturzproblem beim Erstellen einer VMMS-Skalierungsgruppe mit einem internen Lastenausgleich behoben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2867">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="aa5bc-2868">Problem behoben, aufgrund dessen das Argument `--no-wait` nicht mit `vm availability-set create` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2868">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="aa5bc-2869">15. August 2017</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2869">August 15, 2017</span></span>

<span data-ttu-id="aa5bc-2870">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2870">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="aa5bc-2871">ACS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2871">ACS</span></span>

* <span data-ttu-id="aa5bc-2872">sshMaster0-Portnummer für Kubernetes korrigiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2872">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="aa5bc-2873">AppService</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2873">Appservice</span></span>

* <span data-ttu-id="aa5bc-2874">Ausnahme beim Erstellen einer neuen Git-basierten Linux-Web-App behoben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2874">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="aa5bc-2875">Event Grid</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2875">Event Grid</span></span>

* <span data-ttu-id="aa5bc-2876">SDK-Abhängigkeiten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2876">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="aa5bc-2877">11. August 2017</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2877">August 11, 2017</span></span>

<span data-ttu-id="aa5bc-2878">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2878">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="aa5bc-2879">ACS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2879">ACS</span></span>

* <span data-ttu-id="aa5bc-2880">Weitere Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2880">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="aa5bc-2881">Batch</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2881">Batch</span></span>

* <span data-ttu-id="aa5bc-2882">Auf Batch SDK 3.1.0 und Batch Management SDK 4.1.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2882">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="aa5bc-2883">Neuen Befehl zum Anzeigen der Aufgabenanzahl eines Auftrags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2883">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="aa5bc-2884">Fehler in der SAS-URL-Verarbeitung der Ressourcendatei behoben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2884">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="aa5bc-2885">Batch-Kontoendpunkt unterstützt nun optionales Präfix „https://“</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2885">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="aa5bc-2886">Unterstützung für das Hinzufügen von Listen mit mehr als 100 Aufgaben zu einem Auftrag</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2886">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="aa5bc-2887">Debugprotokollierung für das Laden des Erweiterungsbefehlsmoduls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2887">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="aa5bc-2888">Komponente</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2888">Component</span></span>

* <span data-ttu-id="aa5bc-2889">Warnung für veraltete Befehle vom Typ „az component“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2889">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="aa5bc-2890">Container</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2890">Container</span></span>

* <span data-ttu-id="aa5bc-2891">`create`: Problem behoben, aufgrund dessen das Gleichheitszeichen innerhalb einer Umgebungsvariablen nicht zulässig war</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2891">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="aa5bc-2892">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2892">Data Lake Store</span></span>

* <span data-ttu-id="aa5bc-2893">Fortschrittsüberwachung ermöglicht</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2893">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="aa5bc-2894">Event Grid</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2894">Event Grid</span></span>

* <span data-ttu-id="aa5bc-2895">Erste Veröffentlichung</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2895">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="aa5bc-2896">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2896">Network</span></span>

* <span data-ttu-id="aa5bc-2897">`lb`: Problem behoben, aufgrund dessen bestimmte Namen untergeordneter Ressourcen bei Auslassung nicht richtig aufgelöst wurden</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2897">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="aa5bc-2898">`application-gateway {subresource} delete`: Problem behoben, aufgrund dessen `--no-wait` nicht berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2898">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="aa5bc-2899">`application-gateway http-settings update`: Problem behoben, aufgrund dessen `--connection-draining-timeout` nicht deaktiviert werden konnte</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2899">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="aa5bc-2900">Fehler behoben: Unerwartetes Schlüsselwortargument `sa_data_size_kilobyes` bei `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2900">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="aa5bc-2901">Profil</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2901">Profile</span></span>

* <span data-ttu-id="aa5bc-2902">`account list`: `--refresh` hinzugefügt, um die neuesten Abonnements vom Server zu synchronisieren</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2902">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="aa5bc-2903">Storage</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2903">Storage</span></span>

* <span data-ttu-id="aa5bc-2904">Aktualisieren des Speicherkontos mit vom System zugewiesener Identität ermöglicht</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2904">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="aa5bc-2905">VM</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2905">VM</span></span>

* <span data-ttu-id="aa5bc-2906">`availability-set`: Fehlerdomänenanzahl bei Konvertierung verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2906">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="aa5bc-2907">Befehl `list-skus` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2907">Exposed `list-skus` command</span></span>
* <span data-ttu-id="aa5bc-2908">Unterstützung der Identitätszuweisung ohne Erstellung von Rollenzuweisungen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2908">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="aa5bc-2909">Anwenden von Speicher-SKU beim Anfügen von Datenträgern</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2909">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="aa5bc-2910">Standardmäßiger Betriebssystemdatenträger-Name und Speicher-SKU bei Verwendung verwalteter Datenträger entfernt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2910">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="aa5bc-2911">28. Juli 2017</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2911">July 28, 2017</span></span>

<span data-ttu-id="aa5bc-2912">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2912">Version 2.0.12</span></span>

* <span data-ttu-id="aa5bc-2913">Containerbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2913">Added container commands</span></span>
* <span data-ttu-id="aa5bc-2914">Abrechnungs- und Nutzungsmodule hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2914">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="aa5bc-2915">Core</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2915">Core</span></span>

* <span data-ttu-id="aa5bc-2916">Ausgabe von SDK-Authentifizierungsinformationen für Dienstprinzipale mit Zertifikaten</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2916">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="aa5bc-2917">Ausnahmen beim Bereitstellungsfortschritt behoben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2917">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="aa5bc-2918">Verwendung des ARM-Endpunkts aus der aktuellen Cloud für die Erstellung des Abonnementclients</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2918">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="aa5bc-2919">Gleichzeitige Verarbeitung der Datei „clouds.config“ verbessert (3636)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2919">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="aa5bc-2920">Aktualisierung der Clientanforderungs-ID für jede Befehlsausführung</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2920">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="aa5bc-2921">Erstellung von Abonnementclients mit richtigem SDK-Profil (3635)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2921">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="aa5bc-2922">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2922">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="aa5bc-2923">Unterstützung für Auswahl von Tabellenausgabefeldern über jmespath Abfrage hinzugefügt (3581)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2923">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="aa5bc-2924">Stummschaltung von Analyseargumenten und Anfügeverlauf mit Gesten verbessert (3434)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2924">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="aa5bc-2925">Erstellung von Abonnementclients mit richtigem SDK-Profil</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2925">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="aa5bc-2926">Verschiebung aller vorhandenen Erfassungsdateien in den neuesten Ordner</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2926">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="aa5bc-2927">Idempotenz für VM-/VMSS-Erstellung behoben (3586)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2927">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="aa5bc-2928">Bei Befehlspfaden wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2928">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="aa5bc-2929">Bei bestimmten booleschen Parametern wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2929">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="aa5bc-2930">Unterstützung der Anmeldung bei lokalem AD FS-Server wie Azure Stack</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2930">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="aa5bc-2931">Gleichzeitige Schreibvorgänge in „clouds.config“ behoben (3255)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2931">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="aa5bc-2932">ACR</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2932">ACR</span></span>

* <span data-ttu-id="aa5bc-2933">Befehl `show-usage` für verwaltete Registrierungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2933">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="aa5bc-2934">Unterstützung der SKU-Aktualisierung für verwaltete Registrierungen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2934">Support SKU update for managed registries</span></span>
* <span data-ttu-id="aa5bc-2935">Verwaltete Registrierungen mit verwalteter SKU hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2935">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="aa5bc-2936">Webhooks für verwaltete Registrierungen mit ACR-Webhook-Befehlsmodul hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2936">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="aa5bc-2937">AAD-Authentifizierung mit ACR-Anmeldebefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2937">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="aa5bc-2938">Löschbefehl für Docker-Repositorys, Manifeste und Tags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2938">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="aa5bc-2939">ACS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2939">ACS</span></span>

* <span data-ttu-id="aa5bc-2940">Unterstützung der API-Version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2940">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="aa5bc-2941">AppService</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2941">Appservice</span></span>

* <span data-ttu-id="aa5bc-2942">Fehler behoben, aufgrund dessen die Auflistung der Linux-Web-App keine Werte zurückgegeben hat</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2942">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="aa5bc-2943">Unterstützung für das Abrufen von Anmeldeinformationen aus dem ACR</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2943">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="aa5bc-2944">Entfernung aller Befehle unter `appservice web`</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2944">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="aa5bc-2945">Maskierung von Docker-Registrierungskennwörtern aus der Befehlsausgabe (3656)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2945">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="aa5bc-2946">Gewährleistung der fehlerfreien Verwendung des Standardbrowsers unter macOS (3623)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2946">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="aa5bc-2947">Verbesserung des Nutzens von `webapp log tail` und `webapp log download` (3624)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2947">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="aa5bc-2948">Befehl `traffic-routing` zum Konfigurieren des statischen Routings verfügbar gemacht (3566)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2948">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="aa5bc-2949">Zuverlässigkeit beim Konfigurieren der Quellcodeverwaltung verbessert (3245)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2949">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="aa5bc-2950">Nicht unterstütztes Argument `--node-version` aus `webapp config update` für Windows-Web-Apps entfernt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2950">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="aa5bc-2951">Verwenden Sie stattdessen `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2951">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="aa5bc-2952">Batch</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2952">Batch</span></span>

* <span data-ttu-id="aa5bc-2953">Auf Batch SDK 3.0.0 mit Unterstützung virtueller Computer mit niedriger Priorität in Pools aktualisiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2953">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="aa5bc-2954">`pool create`-Option `--target-dedicated` in `--target-dedicated-nodes` umbenannt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2954">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="aa5bc-2955">`pool create`-Optionen `--target-low-priority-nodes` und `--application-licenses` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2955">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="aa5bc-2956">CDN</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2956">CDN</span></span>

* <span data-ttu-id="aa5bc-2957">Besser verständliche Fehlermeldung für `cdn endpoint list`, wenn das von `--profile-name` angegebene Profil nicht vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2957">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="aa5bc-2958">Cloud</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2958">Cloud</span></span>

* <span data-ttu-id="aa5bc-2959">API-Version des Cloudmetadaten-Endpunkts in das Format JJJJ-MM-TT umgewandelt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2959">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="aa5bc-2960">Katalogendpunkt nicht erforderlich</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2960">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="aa5bc-2961">Unterstützung für die Cloudregistrierung nur mit ARM-Endpunkt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2961">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="aa5bc-2962">Option für `cloud set` bereitgestellt, um beim Auswählen der aktuellen Cloud das Profil auswählen zu können</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2962">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="aa5bc-2963">`endpoint_vm_image_alias_doc` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2963">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="aa5bc-2964">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2964">CosmosDB</span></span>

* <span data-ttu-id="aa5bc-2965">Möglichkeit zum Erstellen einer Auflistung mit benutzerdefiniertem Partitionsschlüssel behoben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2965">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="aa5bc-2966">Unterstützung für Auflistungs-Standardgültigkeitsdauer hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2966">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="aa5bc-2967">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2967">Data Lake Analytics</span></span>

* <span data-ttu-id="aa5bc-2968">Zusätzliche Befehle für Compute-Richtlinienverwaltung unter der Überschrift `dla account compute-policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2968">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="aa5bc-2969">`dla job pipeline show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2969">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="aa5bc-2970">`dla job recurrence list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2970">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="aa5bc-2971">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2971">Data Lake Store</span></span>

* <span data-ttu-id="aa5bc-2972">Unterstützung für vom Benutzer verwaltete Schlüsseltresor-Schlüsselrotation in `dls account update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2972">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="aa5bc-2973">Zugrunde liegende SDK-Version des Data Lake Store-Dateisystems aktualisiert, um ein Leistungsproblem zu behandeln</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2973">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="aa5bc-2974">Befehl `dls enable-key-vault` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2974">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="aa5bc-2975">Dieser Befehl versucht, eine vom Benutzer angegebene Key Vault-Instanz zur Verschlüsselung der Daten in einem Data Lake Store-Konto zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2975">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="aa5bc-2976">Interactive</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2976">Interactive</span></span>

* <span data-ttu-id="aa5bc-2977">Startzeit durch Verwendung zwischengespeicherter Befehle verbessert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2977">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="aa5bc-2978">Testabdeckung verbessert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2978">Increased test coverage</span></span>
* <span data-ttu-id="aa5bc-2979">?-Geste erweitert, sodass sie auch in den nächsten Befehl eingefügt wird</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2979">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="aa5bc-2980">Interaktive Fehler mit dem Profil „2017-03-09-profile-preview“ behoben (3587)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2980">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="aa5bc-2981">`--version` als Parameter für den interaktiven Modus zugelassen (3645)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2981">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="aa5bc-2982">Beseitigung von Fehlern im interaktiven Modus beim Abschluss von Überprüfungen (3570)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2982">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="aa5bc-2983">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2983">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="aa5bc-2984">Flag `--progress` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2984">Added `--progress` flag</span></span>
* <span data-ttu-id="aa5bc-2985">`--debug` und `--verbose` aus Abschlüssen entfernt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2985">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="aa5bc-2986">`interactive` aus Abschlüssen entfernt (3324)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2986">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="aa5bc-2987">IoT</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2987">IoT</span></span>

* <span data-ttu-id="aa5bc-2988">Behoben: Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2988">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="aa5bc-2989">(3934)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2989">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="aa5bc-2990">Schlüsseltresor</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2990">Key vault</span></span>

* <span data-ttu-id="aa5bc-2991">Befehle für Schlüsseltresor-Wiederherstellungsfeatures hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2991">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="aa5bc-2992">`keyvault`-Unterbefehle: `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2992">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="aa5bc-2993">`keyvault secret`-Unterbefehle: `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2993">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="aa5bc-2994">`keyvault certificate`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2994">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="aa5bc-2995">`keyvault key`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2995">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="aa5bc-2996">Dienstprinzipal-Schlüsseltresorintegration hinzugefügt (3133)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2996">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="aa5bc-2997">Schlüsseltresor-Datenebene auf 0.3.2. aktualisiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2997">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="aa5bc-2998">(3307)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2998">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="aa5bc-2999">Labor</span><span class="sxs-lookup"><span data-stu-id="aa5bc-2999">Lab</span></span>

* <span data-ttu-id="aa5bc-3000">Unterstützung für Übernahme eines beliebigen virtuellen Computers im Labor über `az lab vm claim` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3000">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="aa5bc-3001">Tabellenausgabeformatierer für `az lab vm list` und `az lab vm show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3001">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="aa5bc-3002">Überwachen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3002">Monitor</span></span>

* <span data-ttu-id="aa5bc-3003">Korrektur für Vorlagendatei mit Befehl `monitor autoscale-settings get-parameters-template` (3349)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3003">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="aa5bc-3004">`monitor alert-rule-incidents list` in `monitor alert list-incidents` umbenannt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3004">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="aa5bc-3005">`monitor alert-rule-incidents show` in `monitor alert show-incident` umbenannt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3005">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="aa5bc-3006">`monitor metric-defintions list` in `monitor metrics list-definitions` umbenannt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3006">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="aa5bc-3007">`monitor alert-rules` in `monitor alert` umbenannt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3007">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="aa5bc-3008">`monitor alert create` geändert:</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3008">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="aa5bc-3009">Unterbefehle vom Typ `condition` und `action` akzeptieren keinen JSON-Code mehr.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3009">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="aa5bc-3010">Hinzufügung zahlreicher Parameter zur Vereinfachung der Regelerstellung</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3010">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="aa5bc-3011">`location` nicht mehr erforderlich</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3011">`location` no longer required</span></span>
  * <span data-ttu-id="aa5bc-3012">Hinzufügung von Namen- und ID-Unterstützung für Ziel</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3012">Add name and ID support for target</span></span>
  * <span data-ttu-id="aa5bc-3013">Entfernung von `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3013">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="aa5bc-3014">Umbenennung von `is-enabled` in `enabled` (nicht mehr erforderlich)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3014">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="aa5bc-3015">`description` wird nun abhängig von der angegebenen Bedingung auf einen Standardwert festgelegt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3015">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="aa5bc-3016">Hinzufügung von Beispielen zur Verdeutlichung des neuen Formats</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3016">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="aa5bc-3017">Unterstützung von Namen oder IDs für Befehle vom Typ `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3017">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="aa5bc-3018">Komfortargumente und Beispiele zu `monitor alert rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3018">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="aa5bc-3019">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3019">Network</span></span>

* <span data-ttu-id="aa5bc-3020">Befehl `list-private-access-services` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3020">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="aa5bc-3021">Argument `--private-access-services` zu `vnet subnet create` und `vnet subnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3021">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="aa5bc-3022">Problem behoben, das einen Fehler für `application-gateway redirect-config create` zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3022">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="aa5bc-3023">Problem behoben, aufgrund dessen `application-gateway redirect-config update` nicht mit `--no-wait` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3023">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="aa5bc-3024">Fehler behoben, der bei der Verwendung des Arguments `--servers` mit `application-gateway address-pool create` und `application-gateway address-pool update` aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3024">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="aa5bc-3025">Befehle vom Typ `application-gateway redirect-config` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3025">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="aa5bc-3026">Befehle zu `application-gateway ssl-policy` hinzugefügt: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3026">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="aa5bc-3027">Argumente zu `application-gateway ssl-policy set` hinzugefügt: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3027">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="aa5bc-3028">Argumente zu `application-gateway http-settings create` und `application-gateway http-settings update` hinzugefügt: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3028">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="aa5bc-3029">Argumente zu `application-gateway url-path-map create` und `application-gateway url-path-map update` hinzugefügt: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3029">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="aa5bc-3030">Argument `--redirect-config` zu `application-gateway url-path-map rule create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3030">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="aa5bc-3031">Unterstützung für `--no-wait` zu `application-gateway url-path-map rule delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3031">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="aa5bc-3032">Argumente zu `application-gateway probe create` und `application-gateway probe update` hinzugefügt: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3032">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="aa5bc-3033">Argument `--redirect-config` zu `application-gateway rule create` und `application-gateway rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3033">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="aa5bc-3034">Unterstützung für `--accelerated-networking` zu `nic create` und `nic update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3034">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="aa5bc-3035">Argument `--internal-dns-name-suffix` von `nic create` entfernt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3035">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="aa5bc-3036">Unterstützung für `--dns-servers` zu `nic update` und `nic create` hinzugefügt: Hinzufügung von Unterstützung für --dns-servers</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3036">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="aa5bc-3037">Fehler korrigiert, aufgrund dessen `--local-address-prefixes` von `local-gateway create` ignoriert wurde</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3037">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="aa5bc-3038">Unterstützung für `--dns-servers` zu `vnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3038">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="aa5bc-3039">Fehler beim Erstellen eines Peerings ohne Routenfilterung mit `express-route peering create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3039">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="aa5bc-3040">Fehler korrigiert, aufgrund dessen die Argumente `--provider` und `--bandwidth` nicht mit `express-route update` verwendet werden konnten</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3040">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="aa5bc-3041">Fehler mit Standardlogik von `network watcher show-topology` korrigiert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3041">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="aa5bc-3042">Ausgabeformatierung für `network list-usages` verbessert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3042">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="aa5bc-3043">Verwendung der standardmäßigen Front-End-IP-Adresse für `application-gateway http-listener create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3043">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="aa5bc-3044">Verwendung des Standardadresspools, der HTTP-Standardeinstellungen und des HTTP-Standardlisteners für `application-gateway rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3044">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="aa5bc-3045">Verwendung der standardmäßigen Front-End-IP-Adresse und des standardmäßigen Back-End-Pools für `lb rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3045">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="aa5bc-3046">Verwendung der standardmäßigen Front-End-IP-Adresse für `lb inbound-nat-rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3046">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="aa5bc-3047">Profil</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3047">Profile</span></span>

* <span data-ttu-id="aa5bc-3048">Unterstützung der Anmeldung innerhalb eines virtuellen Computers mit einer verwalteten Identität</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3048">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="aa5bc-3049">Unterstützung der Ausgabe für `account show` im SDK-Authentifizierungsdateiformat</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3049">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="aa5bc-3050">Anzeige von Warnungen für veraltete Befehle bei Verwendung von „--expanded-view“</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3050">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="aa5bc-3051">Befehl `get-access-token` für die Bereitstellung eines unformatierten AAD-Tokens hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3051">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="aa5bc-3052">Unterstützung der Anmeldung mit einem Benutzerkonto ohne zugeordnete Abonnements</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3052">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="aa5bc-3053">RDBMS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3053">RDBMS</span></span>

* <span data-ttu-id="aa5bc-3054">Unterstützung der abonnementübergreifenden Auflistung von Servern (3417)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3054">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="aa5bc-3055">Behoben: `%s` wird aufgrund von fehlendem `% server_type` nicht verarbeitet (3393)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3055">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="aa5bc-3056">Dokumentquellenzuordnung behoben und CI-Aufgabe zur Überprüfung hinzugefügt (3361)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3056">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="aa5bc-3057">MySQL- und PostgreSQL-Hilfe korrigiert (3369)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3057">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="aa5bc-3058">Resource</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3058">Resource</span></span>

* <span data-ttu-id="aa5bc-3059">Eingabeaufforderungen bei fehlenden Parametern für `group deployment create` verbessert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3059">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="aa5bc-3060">Analyse der Syntax `--parameters KEY=VALUE` verbessert</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3060">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="aa5bc-3061">Probleme behoben, durch die Parameterdateien von `group deployment create` bei Verwendung der Syntax `@<file>` nicht mehr erkannt wurden</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3061">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="aa5bc-3062">Unterstützung des Arguments `--ids` für Befehle vom Typ `resource` und `managedapp`</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3062">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="aa5bc-3063">Einige Analyse- und Fehlermeldungen korrigiert (3584)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3063">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="aa5bc-3064">Analyse vom Typ `--resource-type` für den Befehl `lock` korrigiert, sodass `<resource-namespace>` und `<resource-type>` akzeptiert werden</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3064">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="aa5bc-3065">Parameterüberprüfung für Vorlagenlinkvorlagen hinzugefügt (3629)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3065">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="aa5bc-3066">Unterstützung für die Angabe von Bereitstellungsparametern mit der Syntax `KEY=VALUE` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3066">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="aa5bc-3067">Role</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3067">Role</span></span>

* <span data-ttu-id="aa5bc-3068">Unterstützung der Ausgabe im SDK-Authentifizierungsdateiformat für `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3068">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="aa5bc-3069">Rollenzuweisungen und dazugehörige AAD-Anwendung beim Löschen eines Dienstprinzipals bereinigt (3610)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3069">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="aa5bc-3070">Einbeziehung des Zeitformats in Beschreibungen vom Typ `--start-date` und `--end-date` für `app create`-Argumente</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3070">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="aa5bc-3071">Anzeige von Warnungen für veraltete Befehle bei Verwendung von `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3071">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="aa5bc-3072">Schlüsseltresorintegration zu den Befehlen `create-for-rbac` und `reset-credentials` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3072">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="aa5bc-3073">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3073">Service Fabric</span></span>
* <span data-ttu-id="aa5bc-3074">Problem behoben, aufgrund dessen große Dateien in Anwendungen beim Hochladen gekürzt wurden (3666)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3074">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="aa5bc-3075">Tests für Service Fabric-Befehle hinzugefügt (3424)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3075">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="aa5bc-3076">Zahlreiche Service Fabric-Befehle korrigiert (3234)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3076">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="aa5bc-3077">SQL</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3077">SQL</span></span>

* <span data-ttu-id="aa5bc-3078">Fehlerhafte1 Parameter `--identity` für `sql server create` entfernt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3078">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="aa5bc-3079">Kennwortwerte aus der Befehlsausgabe von `sql server create` und `sql server update` entfernt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3079">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="aa5bc-3080">Befehle `sql db list-editions` und `sql elastic-pool list-editions` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3080">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="aa5bc-3081">Storage</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3081">Storage</span></span>

* <span data-ttu-id="aa5bc-3082">Option `--marker` für die Befehle `storage blob list`, `storage container list` und `storage share list` entfernt (3745)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3082">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="aa5bc-3083">Erstellung eines reinen HTTPS-Speicherkontos ermöglicht</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3083">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="aa5bc-3084">Speichermetriken, Protokollierung und CORS-Befehle aktualisiert (3495)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3084">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="aa5bc-3085">Ausnahmemeldung von „cors add“ umformuliert (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3085">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="aa5bc-3086">Generator im Probelaufmodus des Downloadbatchbefehls in eine Liste konvertiert (3592)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3086">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="aa5bc-3087">Problem bei Probelauf des Blobdownloadbatchs behoben (3640) (3592)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3087">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="aa5bc-3088">VM</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3088">VM</span></span>

* <span data-ttu-id="aa5bc-3089">Unterstützung der NSG-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3089">Support configuring nsg</span></span>
* <span data-ttu-id="aa5bc-3090">Fehler behoben, aufgrund dessen der DNS-Server nicht ordnungsgemäß konfiguriert wurde</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3090">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="aa5bc-3091">Unterstützung verwalteter Dienstidentitäten</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3091">Support managed service identities</span></span>
* <span data-ttu-id="aa5bc-3092">Problem behoben, aufgrund dessen `cmss create` mit einem vorhandenen Lastenausgleich `--backend-pool-name` benötigte</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3092">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="aa5bc-3093">Festlegung, dass die LUN von mit `vm image create` erstellten Datenträgern mit 0 beginnt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3093">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="aa5bc-3094">10. Mai 2017</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3094">May 10, 2017</span></span>

<span data-ttu-id="aa5bc-3095">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3095">Version 2.0.6</span></span>

* <span data-ttu-id="aa5bc-3096">Umbenennen von „documentdb“ in „cosmosdb“</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3096">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="aa5bc-3097">Hinzufügen von rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3097">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="aa5bc-3098">Einbeziehen der Data Lake Analytics- und Data Lake Store-Module</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3098">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="aa5bc-3099">Einbeziehen des Cognitive Services-Moduls</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3099">Include Cognitive Services module</span></span>
* <span data-ttu-id="aa5bc-3100">Einbeziehen des Service Fabric-Moduls</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3100">Include Service Fabric module</span></span>
* <span data-ttu-id="aa5bc-3101">Einbeziehen des interaktiven Moduls (Umbenennen von „az-shell“)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3101">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="aa5bc-3102">Hinzufügen von Unterstützung für CDN-Befehle</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3102">Add support for CDN commands</span></span>
* <span data-ttu-id="aa5bc-3103">Entfernen des Containermoduls</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3103">Remove Container module</span></span>
* <span data-ttu-id="aa5bc-3104">Hinzufügen von „az -v“ als Verknüpfung für „az --version“ ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3104">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="aa5bc-3105">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3105">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="aa5bc-3106">Core</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3106">Core</span></span>

* <span data-ttu-id="aa5bc-3107">Core: Erfassen von Ausnahmen, die durch einen nicht registrierten Anbieter verursacht werden, und automatische Registrierung</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3107">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="aa5bc-3108">Leistung: Dauerhaftes Speichern des ADAL-Tokencaches im Arbeitsspeicher bis zum Prozessende ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3108">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="aa5bc-3109">Korrigieren der vom hexadezimalen Fingerabdruck -o tsv zurückgegebenen Bytes ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3109">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="aa5bc-3110">Verbessern des Downloads des Schlüsseltresorzertifikats und der AAD-SP-Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3110">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="aa5bc-3111">Hinzufügen des Python-Speicherorts zu „az –version“ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3111">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="aa5bc-3112">Anmeldung: Unterstützung der Anmeldung, wenn keine Abonnements vorhanden sind ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3112">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="aa5bc-3113">Core: Beheben eines Fehlers bei zweimaliger Verwendung eines Dienstprinzipals bei der Anmeldung ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3113">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="aa5bc-3114">Core: Ermöglichen der Konfiguration des Dateipfads von „accessTokens.json“ über eine Umgebungsvariable ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3114">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="aa5bc-3115">Core: Zulassen der Anwendung konfigurierter Standardwerte auf optionale Argumente ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3115">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="aa5bc-3116">Core: Verbesserte Leistung</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3116">core: Improved performance</span></span>
* <span data-ttu-id="aa5bc-3117">Core: Zertifikate von benutzerdefinierter Zertifizierungsstelle – Unterstützung für das Festlegen der REQUESTS_CA_BUNDLE-Umgebungsvariablen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3117">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="aa5bc-3118">Core: Cloudkonfiguration – Verwenden des Endpunkts „resource manager“, wenn Endpunkt „management“ nicht festgelegt ist</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3118">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="aa5bc-3119">ACS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3119">ACS</span></span>

* <span data-ttu-id="aa5bc-3120">Korrigieren der Master- und Agentanzahl als ganze Zahl statt Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3120">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="aa5bc-3121">Verfügbarmachen von „az acs create --no-wait“ und „az acs wait“ für die asynchrone Erstellung</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3121">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="aa5bc-3122">Verfügbarmachen von „az acs create --validate“ für Probelaufüberprüfungen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3122">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="aa5bc-3123">Entfernen von Windows-Profil vor PUT-Aufruf für Skalierungsbefehl ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3123">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="aa5bc-3124">AppService</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3124">AppService</span></span>

* <span data-ttu-id="aa5bc-3125">functionapp: Hinzufügen der vollständigen functionapp-Unterstützung, einschließlich Erstellen, Anzeigen, Auflisten, Löschen, Hostname, SSL usw.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3125">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="aa5bc-3126">Hinzufügen von Team Services (vsts) als Continuous Delivery-Option zu „appservice web source-control config“</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3126">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="aa5bc-3127">Erstellen von „az webapp“ als Ersatz für „az appservice web“ (für Abwärtskompatibilität bleibt „az appservice web“ für 2 weitere Releases erhalten)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3127">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="aa5bc-3128">Verfügbarmachen von Argumenten zum Konfigurieren von Bereitstellung und Laufzeitstapeln beim Erstellen von Web-Apps</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3128">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="aa5bc-3129">Verfügbarmachen von „webapp list-runtimes“</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3129">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="aa5bc-3130">Unterstützen der Konfiguration von Verbindungszeichenfolgen ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3130">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="aa5bc-3131">Unterstützen des Slottauschs mit Vorschau</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3131">support slot swap with preview</span></span>
* <span data-ttu-id="aa5bc-3132">Beheben von Fehlern in appservice-Befehlen ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3132">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="aa5bc-3133">Verwenden der Ressourcengruppe des App Service-Plans für Zertifizierungsvorgänge ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3133">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="aa5bc-3134">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3134">CosmosDB</span></span>

* <span data-ttu-id="aa5bc-3135">Umbenennen des documentdb-Moduls in cosmosdb</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3135">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="aa5bc-3136">Zusätzliche Unterstützung für documentdb-APIs auf Datenebene: Datenbank- und Sammlungsverwaltung</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3136">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="aa5bc-3137">Zusätzliche Unterstützung für das Aktivieren des automatischen Failovers für Datenbankkonten</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3137">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="aa5bc-3138">Zusätzliche Unterstützung für die neue ConsistentPrefix-Konsistenzrichtlinie</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3138">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="aa5bc-3139">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3139">Data Lake Analytics</span></span>

* <span data-ttu-id="aa5bc-3140">Beheben eines Fehlers, bei dem das Filtern von Auftragslisten nach Ergebnis und Status einen Fehler auslöst</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3140">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="aa5bc-3141">Hinzufügen von Unterstützung für den neuen Katalogelementtyp „Paket“</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3141">Add support for new catalog item type: package.</span></span> <span data-ttu-id="aa5bc-3142">Zugriff über: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3142">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="aa5bc-3143">Ermöglichen der Auflistung folgender Katalogelemente innerhalb einer Datenbank (keine Schemaspezifikation erforderlich):</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3143">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="aa5bc-3144">Tabelle</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3144">Table</span></span>
  * <span data-ttu-id="aa5bc-3145">Tabellenwertfunktion</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3145">Table valued function</span></span>
  * <span data-ttu-id="aa5bc-3146">Sicht</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3146">View</span></span>
  * <span data-ttu-id="aa5bc-3147">Tabellenstatistiken.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3147">Table Statistics.</span></span> <span data-ttu-id="aa5bc-3148">Können auch mit einem Schema, jedoch ohne Angabe eines Tabellennamens aufgelistet werden.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3148">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="aa5bc-3149">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3149">Data Lake Store</span></span>

* <span data-ttu-id="aa5bc-3150">Aktualisieren der Version des zugrunde liegenden Dateisystem-SDK, wodurch eine bessere Unterstützung für die Verarbeitung von Drosselungsszenarien auf Serverseite gewährt wird</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3150">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="aa5bc-3151">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3151">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="aa5bc-3152">Fehlende Hilfe für Zugriffsanzeige</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3152">missed help for access show.</span></span> <span data-ttu-id="aa5bc-3153">hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3153">adding it.</span></span> <span data-ttu-id="aa5bc-3154">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3154">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="aa5bc-3155">Suchen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3155">Find</span></span>

* <span data-ttu-id="aa5bc-3156">Verbessern von Suchergebnissen und Ermöglichen der Versionsverwaltung des Suchindex</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3156">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="aa5bc-3157">KeyVault</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3157">KeyVault</span></span>

* <span data-ttu-id="aa5bc-3158">BC:`az keyvault certificate download` Ändern von „-e“ von Zeichenfolge oder Binärdatentyp in PEM oder DER zur besseren Darstellung der Optionen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3158">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="aa5bc-3159">BC: Entfernen von „--expires“ und „--not-before“ aus `keyvault certificate create`, da diese Parameter nicht vom Dienst unterstützt werden</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3159">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="aa5bc-3160">Hinzufügen des Parameters „--validity“ zu `keyvault certificate create`, um gezielt den Wert in „--policy“ zu überschreiben</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3160">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="aa5bc-3161">Beheben des Problems in `keyvault certificate get-default-policy`, bei dem „expires“ und „not_before“ verfügbar gemacht wurden, „validity_in_months“ hingegen nicht</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3161">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="aa5bc-3162">Keyvault-Korrektur für den Import von PEM und PFX ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3162">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="aa5bc-3163">Labor</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3163">Lab</span></span>

* <span data-ttu-id="aa5bc-3164">Hinzufügen der Befehle „create“, „show“, „delete“ und „list“ für die Laborumgebung</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3164">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="aa5bc-3165">Hinzufügen der Befehle „show“ und „list“ zur Anzeige von ARM-Vorlagen im Labor</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3165">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="aa5bc-3166">Hinzufügen des Kennzeichens „--environment“ in `az lab vm list`, um virtuelle Computer nach Umgebung im Labor zu filtern</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3166">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="aa5bc-3167">Hinzufügen des benutzerfreundlichen Befehls `az lab formula export-artifacts` zum Exportieren des Artefaktgerüsts innerhalb der Formel eines Labors</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3167">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="aa5bc-3168">Hinzufügen von Befehlen zum Verwalten von Geheimnissen in einem Labor</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3168">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="aa5bc-3169">Überwachen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3169">Monitor</span></span>

* <span data-ttu-id="aa5bc-3170">Fehlerbehebung: Modellieren von `--actions` von `az alert-rules create` zum Verarbeiten von JSON-Zeichenfolgen ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3170">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="aa5bc-3171">Programmfehlerbehebung: Beim Erstellen von Diagnoseeinstellungen werden Protokolle/Metriken aus Anzeigebefehlen nicht akzeptiert ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3171">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="aa5bc-3172">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3172">Network</span></span>

* <span data-ttu-id="aa5bc-3173">Hinzufügen des `network watcher test-connectivity`-Befehls</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3173">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="aa5bc-3174">Hinzufügen von Unterstützung für den `--filters`-Parameter für `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3174">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="aa5bc-3175">Hinzufügen von Unterstützung für den Application Gateway-Verbindungsausgleich</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3175">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="aa5bc-3176">Hinzufügen von Unterstützung für die Konfiguration von Application Gateway-WAF-Regelsätzen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3176">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="aa5bc-3177">Hinzufügen von Unterstützung für ExpressRoute-Routenfilter und -Regeln</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3177">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="aa5bc-3178">Hinzufügen von Unterstützung für geografisches TrafficManager-Routing</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3178">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="aa5bc-3179">Hinzufügen von Unterstützung für richtlinienbasierte Datenverkehrsselektoren für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3179">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="aa5bc-3180">Hinzufügen von Unterstützung für IPSec-Richtlinien für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3180">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="aa5bc-3181">Korrektur eines Fehlers bei `vpn-connection create` bei Verwendung der Parameter `--no-wait` oder `--validate`</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3181">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="aa5bc-3182">Hinzufügen von Unterstützung für Aktiv/Aktiv-VNET-Gateways</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3182">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="aa5bc-3183">Entfernen von NULL-Werten aus der Ausgabe von `network vpn-connection list/show`-Befehlen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3183">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="aa5bc-3184">BC: Korrektur eines Fehlers in der Ausgabe von `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3184">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="aa5bc-3185">Korrektur eines Fehlers, bei dem das Argument „--key-length“ von „vpn-connection create“ nicht ordnungsgemäß analysiert wurde</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3185">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="aa5bc-3186">Korrektur eines Fehlers in `dns zone import`, bei dem Datensätze nicht ordnungsgemäß importiert wurden</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3186">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="aa5bc-3187">Korrektur eines Fehlers, bei dem `traffic-manager endpoint update` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3187">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="aa5bc-3188">Hinzufügen von Network Watcher-Vorschaubefehlen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3188">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="aa5bc-3189">Profil</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3189">Profile</span></span>

* <span data-ttu-id="aa5bc-3190">Unterstützung der Anmeldung, wenn keine Abonnements gefunden werden ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3190">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="aa5bc-3191">Unterstützung für kurze Parameternamen in „az account set --subscription“ ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3191">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="aa5bc-3192">Redis</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3192">Redis</span></span>

* <span data-ttu-id="aa5bc-3193">Hinzufügen des Updatebefehls, durch den auch die Möglichkeit zum Skalieren für Redis Cache hinzugefügt wird</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3193">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="aa5bc-3194">Verwerfen des Befehls „update-settings“</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3194">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="aa5bc-3195">Resource</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3195">Resource</span></span>

* <span data-ttu-id="aa5bc-3196">Hinzufügen der Befehle „managedapp“ und „managedapp definition“ ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3196">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="aa5bc-3197">Unterstützung für die „provider operation“-Befehle ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3197">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="aa5bc-3198">Unterstützung für die Erstellung generischer Ressourcen ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3198">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="aa5bc-3199">Korrigieren der Ressourcenanalyse und der API-Versionssuche</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3199">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="aa5bc-3200">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3200">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="aa5bc-3201">Hinzufügen von Dokumenten für „az lock update“</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3201">Add docs for az lock update.</span></span> <span data-ttu-id="aa5bc-3202">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3202">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="aa5bc-3203">Beenden mit Fehler bei dem Versuch, Ressourcen für eine nicht vorhandene Gruppe aufzulisten</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3203">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="aa5bc-3204">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3204">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="aa5bc-3205">[Compute] Beheben von Problemen mit dem Update von VMSS- und VM-Verfügbarkeitsgruppen</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3205">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="aa5bc-3206">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3206">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="aa5bc-3207">Korrigieren des Erstellungs- und Löschvorgangs für Sperren, wenn „parent-resource-path“ auf „None“ festgelegt ist ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3207">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="aa5bc-3208">Role</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3208">Role</span></span>

* <span data-ttu-id="aa5bc-3209">create-for-rbac: Sicherstellen, dass das SP-Enddatum nicht das Ablaufdatum des Zertifikats überschreitet ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3209">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="aa5bc-3210">RBAC: Hinzufügen vollständiger Unterstützung für „ad group“ ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3210">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="aa5bc-3211">Rolle: Beheben von Probleme beim Rollendefinitionsupdate ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3211">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="aa5bc-3212">create-for-rbac: Sicherstellen, dass das angegebene Benutzerkennwort übernommen wird</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3212">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="aa5bc-3213">SQL</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3213">SQL</span></span>

* <span data-ttu-id="aa5bc-3214">Hinzufügen der Befehle „az sql server list-usages“ und „az sql db list-usages“</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3214">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="aa5bc-3215">SQL: Möglichkeit zur direkten Verbindung mit Ressourcenanbieter ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3215">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="aa5bc-3216">Storage</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3216">Storage</span></span>

* <span data-ttu-id="aa5bc-3217">Festlegen des Ressourcengruppenstandorts als Standardstandort für `storage account create`</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3217">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="aa5bc-3218">Hinzufügen von Unterstützung für das inkrementelle Kopieren von Blobs</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3218">Add support for incremental blob copy</span></span>
* <span data-ttu-id="aa5bc-3219">Hinzufügen von Unterstützung für den Upload umfangreicher Blockblobs</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3219">Add support for large block blob upload</span></span>
* <span data-ttu-id="aa5bc-3220">Ändern der Blockgröße auf 100 MB, wenn die hochzuladende Datei größer als 200 GB ist</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3220">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="aa5bc-3221">VM</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3221">VM</span></span>

* <span data-ttu-id="aa5bc-3222">avail-set: Festlegen der UD- und FD-Domänenanzahl als optional</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3222">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="aa5bc-3223">Hinweis: VM-Befehle in unabhängigen Clouds: Vermeiden Sie Features im Zusammenhang mit verwalteten Datenträgern, einschließlich der folgenden:</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3223">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="aa5bc-3224">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3224">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="aa5bc-3225">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3225">az vm/vmss disk</span></span>
  3. <span data-ttu-id="aa5bc-3226">Verwenden Sie in „az vm/vmss create“ den Befehl „—use-unmanaged-disk“, um verwaltete Datenträger zu vermeiden. Andere Befehle sollten funktionieren.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3226">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="aa5bc-3227">vm/vmss: Verbessern des Warnungstexts beim Generieren von SSH-Schlüsselpaaren</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3227">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="aa5bc-3228">vm/vmss: Unterstützen der Erstellung über ein Marketplace-Image, für das Planinformationen erforderlich sind ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3228">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="aa5bc-3229">3\. April 2017</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3229">April 3, 2017</span></span>

<span data-ttu-id="aa5bc-3230">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3230">Version 2.0.2</span></span>

<span data-ttu-id="aa5bc-3231">In dieser Version wurden die Komponenten ACR, Batch, KeyVault und SQL eingeführt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3231">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="aa5bc-3232">Core</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3232">Core</span></span>

* <span data-ttu-id="aa5bc-3233">Hinzufügen der Module „acr“, „lab“, „monitor“ und „find“ zur Standardliste</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3233">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="aa5bc-3234">Anmeldung: Überspringen des fehlerhaften Mandanten ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3234">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="aa5bc-3235">Anmeldung: Festlegen des Standardabonnements auf ein Abonnement mit dem Status „Enabled“ ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3235">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="aa5bc-3236">Hinzufügen von wait-Befehlen und Unterstützung von „--no-wait“ für mehr Befehle ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3236">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="aa5bc-3237">Core: Unterstützen der Anmeldung per Dienstprinzipal mit einem Zertifikat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3237">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="aa5bc-3238">Hinzufügen der Meldung zu fehlenden Vorlagenparametern</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3238">Add prompting for missing template parameters.</span></span> <span data-ttu-id="aa5bc-3239">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3239">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="aa5bc-3240">Unterstützen des Festlegens von Standardwerten für häufig verwendete Argumente, z.B. Standardressourcengruppe, Standardweb und Standard-VM</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3240">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="aa5bc-3241">Unterstützen der Anmeldung an einem bestimmten Mandanten</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3241">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="aa5bc-3242">ACS</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3242">ACS</span></span>

* <span data-ttu-id="aa5bc-3243">[ACS] Hinzufügen von Unterstützung für die Konfiguration eines ACS-Standardclusters ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3243">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="aa5bc-3244">Hinzufügen von Unterstützung der Aufforderung zur Kennworteingabe für SSH-Schlüssel</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3244">Add support for ssh key password prompting.</span></span> <span data-ttu-id="aa5bc-3245">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3245">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="aa5bc-3246">Hinzufügen von Unterstützung für Windows-Cluster</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3246">Add support for windows clusters.</span></span> <span data-ttu-id="aa5bc-3247">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3247">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="aa5bc-3248">Wechseln von der Rolle „Besitzer“ zur Rolle „Mitwirkender“</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3248">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="aa5bc-3249">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3249">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="aa5bc-3250">AppService</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3250">AppService</span></span>

* <span data-ttu-id="aa5bc-3251">appservice: Unterstützung für das Abrufen der externen IP-Adresse für DNS A-Einträge ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3251">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="aa5bc-3252">appservice: Unterstützung der Bindung von Platzhalterzertifikaten ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3252">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="aa5bc-3253">appservice: Unterstützung von Veröffentlichungsprofilen für Listen ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3253">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="aa5bc-3254">AppService: Auslösen der Synchronisierung der Quellcodeverwaltung nach der Konfiguration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3254">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="aa5bc-3255">DataLake</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3255">DataLake</span></span>

* <span data-ttu-id="aa5bc-3256">Erste Version des Data Lake Analytics-Moduls</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3256">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="aa5bc-3257">Erste Version des Data Lake Store-Moduls</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3257">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="aa5bc-3258">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3258">DocuemntDB</span></span>

* <span data-ttu-id="aa5bc-3259">DocumentDB: Hinzufügen von Unterstützung für das Auflisten von Verbindungszeichenfolgen ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3259">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="aa5bc-3260">VM</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3260">VM</span></span>

* <span data-ttu-id="aa5bc-3261">[Compute] Hinzufügen von AppGateway-Unterstützung für Erstellung von VM-Skalierungsgruppen ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3261">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="aa5bc-3262">[VM/VMSS] Verbesserte Unterstützung für die Datenträgerzwischenspeicherung ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3262">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="aa5bc-3263">VM/VMSS: Einbinden der vom Portal verwendeten Logik zur Überprüfung von Anmeldeinformationen ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3263">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="aa5bc-3264">Hinzufügen von wait-Befehlen und Unterstützung für „--no-wait“ ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3264">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="aa5bc-3265">VM-Skalierungsgruppe: Unterstützung von „\*“ zum Auflisten der übergreifenden Instanzansicht für VMs ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3265">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="aa5bc-3266">Hinzufügen – Geheimnisse für virtuellen Computer und VM-Skalierungsgruppe ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3266">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="aa5bc-3267">Zulassen der VM-Erstellung mit spezialisierter VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3267">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="aa5bc-3268">27. Februar 2017</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3268">February 27, 2017</span></span>

<span data-ttu-id="aa5bc-3269">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3269">Version 2.0.0</span></span>

<span data-ttu-id="aa5bc-3270">Diese Version der Azure CLI 2.0 ist die erste „allgemein verfügbare“ Version. Die allgemeine Verfügbarkeit gilt für die folgenden Befehlsmodule:</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3270">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="aa5bc-3271">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3271">Container Service (acs)</span></span>
- <span data-ttu-id="aa5bc-3272">Compute (einschließlich Resource Manager, VM, VM-Skalierungsgruppen, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3272">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="aa5bc-3273">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3273">Networking</span></span>
- <span data-ttu-id="aa5bc-3274">Storage</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3274">Storage</span></span>

<span data-ttu-id="aa5bc-3275">Diese Befehlsmodule können in der Produktion verwendet werden und verfügen über Unterstützung durch eine Standard-SLA von Microsoft. Sie können Anfragen zu Problemen direkt beim Microsoft-Support oder in der [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/) öffnen. Sie haben die Möglichkeit, Fragen in [StackOverflow mit dem Tag „azure-cli“](http://stackoverflow.com/questions/tagged/azure-cli) zu stellen oder sich unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) an das Produktteam zu wenden. Außerdem können Sie über die Befehlszeile mit dem Befehl `az feedback` Feedback senden.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3275">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="aa5bc-3276">Die Befehle in diesen Modulen sind stabil, und es ist nicht zu erwarten, dass sich die Syntax in den anstehenden Veröffentlichungen dieser Version der Azure CLI ändern.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3276">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="aa5bc-3277">Verwenden Sie zum Überprüfen der Version der CLI den Befehl `az --version`. In der Ausgabe werden die Version der CLI selbst (für diese Veröffentlichung 2.0.0), die einzelnen Befehlsmodule und die von Ihnen genutzten Versionen von Python und GCC aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3277">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="aa5bc-3278">Einige Befehlsmodule verfügen über das Postfix „b*n*“ oder „rc*n*“. Diese Befehlsmodule befinden sich noch in der Vorschauphase und werden später die allgemeine Verfügbarkeit erlangen.</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3278">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="aa5bc-3279">Außerdem werden jeden Abend Vorschaubuilds der CLI bereitgestellt. Informationen hierzu finden Sie in der [Anleitung zum Abrufen der abendlichen Builds](https://github.com/Azure/azure-cli#nightly-builds) und im Abschnitt zum [Setup für Entwickler und Beitragen von Code](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3279">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="aa5bc-3280">Sie können für die abendlichen Vorschaubuilds wie folgt Probleme melden:</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3280">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="aa5bc-3281">Über die [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3281">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="aa5bc-3282">Per Kontaktaufnahme mit dem Produktteam unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3282">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="aa5bc-3283">Senden von Feedback über die Befehlszeile mit dem Befehl `az feedback`</span><span class="sxs-lookup"><span data-stu-id="aa5bc-3283">Provide feedback from the command line with the `az feedback` command</span></span>


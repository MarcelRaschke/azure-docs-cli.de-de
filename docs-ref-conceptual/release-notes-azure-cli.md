---
title: Versionshinweise für die Azure CLI
description: Enthält Informationen zu den aktuellen Updates der Azure CLI.
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 02/04/2020
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: eafd18344ac4c1c0124ff53864a45510070b6fe7
ms.sourcegitcommit: d0b2763cc856eef44a6ecb78f6b8c64291625750
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/04/2020
ms.locfileid: "77013283"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="b33c5-103">Versionshinweise für die Azure CLI</span><span class="sxs-lookup"><span data-stu-id="b33c5-103">Azure CLI release notes</span></span>

## <a name="february-04-2020"></a><span data-ttu-id="b33c5-104">04. Februar 2020</span><span class="sxs-lookup"><span data-stu-id="b33c5-104">February 04, 2020</span></span>

<span data-ttu-id="b33c5-105">Version 2.0.81</span><span class="sxs-lookup"><span data-stu-id="b33c5-105">Version 2.0.81</span></span>

### <a name="acs"></a><span data-ttu-id="b33c5-106">ACS</span><span class="sxs-lookup"><span data-stu-id="b33c5-106">ACS</span></span>

* <span data-ttu-id="b33c5-107">Unterstützung für das Festlegen zugeordneter Ausgangsports und Leerlauftimeouts für Load Balancer Standard hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-107">Add support to set outbound allocated ports and idle timeouts on standard load balancer</span></span>
* <span data-ttu-id="b33c5-108">Aktualisierung auf API-Version 2019-11-01</span><span class="sxs-lookup"><span data-stu-id="b33c5-108">Update to API Version 2019-11-01</span></span>

### <a name="acr"></a><span data-ttu-id="b33c5-109">ACR</span><span class="sxs-lookup"><span data-stu-id="b33c5-109">ACR</span></span>

* <span data-ttu-id="b33c5-110">[BREAKING CHANGE] `az acr delete` löst eine Eingabeaufforderung aus.</span><span class="sxs-lookup"><span data-stu-id="b33c5-110">[BREAKING CHANGE] `az acr delete` will prompt</span></span>
* <span data-ttu-id="b33c5-111">[BREAKING CHANGE] „az acr task delete“ löst eine Eingabeaufforderung aus.</span><span class="sxs-lookup"><span data-stu-id="b33c5-111">[BREAKING CHANGE] 'az acr task delete' will prompt</span></span>
* <span data-ttu-id="b33c5-112">Neue Befehlsgruppe „az acr taskrun show/list/delete“ für die Aufgabenausführungsverwaltung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-112">Add a new command group 'az acr taskrun show/list/delete' for taskrun management</span></span>

### <a name="aks"></a><span data-ttu-id="b33c5-113">AKS</span><span class="sxs-lookup"><span data-stu-id="b33c5-113">AKS</span></span>

* <span data-ttu-id="b33c5-114">Jeder Cluster erhält einen separaten Dienstprinzipal zur Verbesserung der Isolation.</span><span class="sxs-lookup"><span data-stu-id="b33c5-114">Each cluster gets a separate service principal to improve isolation</span></span>

### <a name="appconfig"></a><span data-ttu-id="b33c5-115">AppConfig</span><span class="sxs-lookup"><span data-stu-id="b33c5-115">AppConfig</span></span>

* <span data-ttu-id="b33c5-116">Unterstützung für den Import/Export von KeyVault-Verweisen in/aus AppService</span><span class="sxs-lookup"><span data-stu-id="b33c5-116">Support import/export of keyvault references from/to appservice</span></span>
* <span data-ttu-id="b33c5-117">Unterstützung für den Import/Export aller Bezeichnungen in appconfig und aus appconfig</span><span class="sxs-lookup"><span data-stu-id="b33c5-117">Support import/export of all labels from appconfig to appconfig</span></span>
* <span data-ttu-id="b33c5-118">Überprüfen der Schlüssel- und Featurenamen vor dem Festlegen und Importieren</span><span class="sxs-lookup"><span data-stu-id="b33c5-118">Validate key and feature names before setting and importing</span></span>
* <span data-ttu-id="b33c5-119">Verfügbarmachen der SKU-Änderung für den Konfigurationsspeicher</span><span class="sxs-lookup"><span data-stu-id="b33c5-119">Expose sku modification for configuration store.</span></span>
* <span data-ttu-id="b33c5-120">Befehlsgruppe für die verwaltete Identität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-120">Add command group for managed identity.</span></span>

### <a name="appservice"></a><span data-ttu-id="b33c5-121">AppService</span><span class="sxs-lookup"><span data-stu-id="b33c5-121">AppService</span></span>

* <span data-ttu-id="b33c5-122">Azure Stack: Oberflächenbefehle im Profil „2019-03-01-hybrid“</span><span class="sxs-lookup"><span data-stu-id="b33c5-122">Azure Stack: surface commands under the profile of 2019-03-01-hybrid</span></span>
* <span data-ttu-id="b33c5-123">functionapp: Funktion zum Erstellen von Java-Funktions-Apps in Linux hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-123">functionapp: Add ability to create Java function apps in Linux</span></span>

### <a name="arm"></a><span data-ttu-id="b33c5-124">ARM</span><span class="sxs-lookup"><span data-stu-id="b33c5-124">ARM</span></span>

* <span data-ttu-id="b33c5-125">Behebung von Problem Nr. 10246: `az resource tag` stürzt ab, wenn der übergebene Parameter `--ids` der Ressourcengruppen-ID entspricht.</span><span class="sxs-lookup"><span data-stu-id="b33c5-125">Fix issue #10246: `az resource tag` crashes when the parameter `--ids` passed in is resource group ID</span></span>
* <span data-ttu-id="b33c5-126">Behebung von Problem Nr. 11658: Der Befehl `az group export` unterstützt die Parameter `--query` und `--output` nicht.</span><span class="sxs-lookup"><span data-stu-id="b33c5-126">Fix issue #11658: `az group export` command does not support `--query` and `--output` parameters</span></span>
* <span data-ttu-id="b33c5-127">Behebung von Problem Nr. 10279: Der Exitcode von `az group deployment validate` ist 0, wenn bei der Überprüfung ein Fehler auftritt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-127">Fix issue #10279: The exit code of `az group deployment validate` is 0 when the verification fails</span></span>
* <span data-ttu-id="b33c5-128">Behebung von Problem Nr. 9916: Fehlermeldung des Konflikts zwischen Tag und anderen Filterbedingungen für Befehl `az resource list` verbessert</span><span class="sxs-lookup"><span data-stu-id="b33c5-128">Fix issue #9916: Improve the error message of the conflict between tag and other filter conditions for `az resource list` command</span></span>
* <span data-ttu-id="b33c5-129">Neuer Parameter `--managed-by` hinzugefügt, um das Hinzufügen der Informationen vom Typ „managedBy“ für Befehl `az group create` zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="b33c5-129">Add new parameter `--managed-by` to support adding managedBy information for command `az group create`</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="b33c5-130">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="b33c5-130">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="b33c5-131">Untergruppe `monitor` hinzugefügt, um Log Analytics-Überwachung im Azure Red Hat OpenShift-Cluster zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="b33c5-131">Add `monitor` subgroup to manage Log Analytics monitoring in Azure Red Hat OpensShift cluster</span></span>

### <a name="botservice"></a><span data-ttu-id="b33c5-132">BotService</span><span class="sxs-lookup"><span data-stu-id="b33c5-132">BotService</span></span>

* <span data-ttu-id="b33c5-133">Behebung von Problem Nr. 11697: `az bot create` ist nicht idempotent.</span><span class="sxs-lookup"><span data-stu-id="b33c5-133">Fix issue #11697: `az bot create` is not idempotent</span></span>
* <span data-ttu-id="b33c5-134">Tests zur Namenskorrektur geändert, sodass sie nur im Livemodus ausgeführt werden</span><span class="sxs-lookup"><span data-stu-id="b33c5-134">Change name-correcting tests to run in Live-mode only</span></span>

### <a name="cdn"></a><span data-ttu-id="b33c5-135">CDN</span><span class="sxs-lookup"><span data-stu-id="b33c5-135">CDN</span></span>

* <span data-ttu-id="b33c5-136">Unterstützung für das rulesEngine-Feature hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-136">Add support for rulesEngine feature</span></span>
* <span data-ttu-id="b33c5-137">Neue Befehlsgruppe „cdn endpoint rule“ zum Verwalten von Regeln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-137">Add new commands group 'cdn endpoint rule' to manage rules</span></span>
* <span data-ttu-id="b33c5-138">azure-mgmt-cdn-Version auf 4.0.0 aktualisiert, um API-Version 2019-04-15 zu verwenden</span><span class="sxs-lookup"><span data-stu-id="b33c5-138">Update azure-mgmt-cdn version to 4.0.0 to use api version 2019-04-15</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="b33c5-139">Bereitstellungs-Manager</span><span class="sxs-lookup"><span data-stu-id="b33c5-139">Deployment Manager</span></span>

* <span data-ttu-id="b33c5-140">Auflistungsvorgang für alle Ressourcen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-140">Add list operation for all resources.</span></span>
* <span data-ttu-id="b33c5-141">Schrittressource für neuen Schritttyp optimiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-141">Enhance step resource for new step type.</span></span>
* <span data-ttu-id="b33c5-142">Paket „azure-mgmt-deploymentmanager“ zur Verwendung von Version 0.2.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-142">Update azure-mgmt-deploymentmanager package to use version 0.2.0.</span></span>

### <a name="iot"></a><span data-ttu-id="b33c5-143">IoT</span><span class="sxs-lookup"><span data-stu-id="b33c5-143">IoT</span></span>

* <span data-ttu-id="b33c5-144">Befehle vom Typ „IoT hub Job“ als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="b33c5-144">Deprecate 'IoT hub Job' commands.</span></span>

### <a name="iot-central"></a><span data-ttu-id="b33c5-145">IoT Central</span><span class="sxs-lookup"><span data-stu-id="b33c5-145">IoT Central</span></span>

* <span data-ttu-id="b33c5-146">Unterstützung der App-Erstellung/-Aktualisierung mit neuem SKU-Namen ST0, ST1, ST2</span><span class="sxs-lookup"><span data-stu-id="b33c5-146">Support app creation/update with the new sku name ST0, ST1, ST2.</span></span>

### <a name="key-vault"></a><span data-ttu-id="b33c5-147">Key Vault</span><span class="sxs-lookup"><span data-stu-id="b33c5-147">Key Vault</span></span>

* <span data-ttu-id="b33c5-148">Neuer Befehl `az keyvault key download` zum Herunterladen von Schlüsseln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-148">Add a new command `az keyvault key download` for downloading keys.</span></span>

### <a name="misc"></a><span data-ttu-id="b33c5-149">Sonstiges</span><span class="sxs-lookup"><span data-stu-id="b33c5-149">Misc</span></span>

* <span data-ttu-id="b33c5-150">Behebung Nr. 6371: Unterstützung für die Vervollständigung von Dateinamen und Umgebungsvariablen in Bash</span><span class="sxs-lookup"><span data-stu-id="b33c5-150">Fix #6371: Support filename and environment variable completion in Bash</span></span>

### <a name="network"></a><span data-ttu-id="b33c5-151">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="b33c5-151">Network</span></span>

* <span data-ttu-id="b33c5-152">Behebung Nr. 2092: az network dns record-set add/remove: Warnung hinzugefügt, wenn Datensatzgruppe nicht gefunden wurde.</span><span class="sxs-lookup"><span data-stu-id="b33c5-152">Fix #2092: az network dns record-set add/remove: add warning when record-set is not found.</span></span> <span data-ttu-id="b33c5-153">In Zukunft wird ein zusätzliches Argument unterstützt, um diese automatische Erstellung zu bestätigen.</span><span class="sxs-lookup"><span data-stu-id="b33c5-153">In the future, an extra argument will be supported to confirm this auto creation.</span></span>

### <a name="policy"></a><span data-ttu-id="b33c5-154">Richtlinie</span><span class="sxs-lookup"><span data-stu-id="b33c5-154">Policy</span></span>

* <span data-ttu-id="b33c5-155">Neuer Befehl `az policy metadata` hinzugefügt, um umfangreiche Richtlinienmetadatenressourcen abzurufen</span><span class="sxs-lookup"><span data-stu-id="b33c5-155">Add new command `az policy metadata` to retrieve rich policy metadata resources</span></span>
* <span data-ttu-id="b33c5-156">`az policy remediation create`: Geben Sie mit dem Parameter `--resource-discovery-mode` an, ob die Konformität vor der Wartung neu bewertet werden soll.</span><span class="sxs-lookup"><span data-stu-id="b33c5-156">`az policy remediation create`: Specify whether compliance should be re-evaluated prior to remediation with the `--resource-discovery-mode` parameter</span></span>

### <a name="profile"></a><span data-ttu-id="b33c5-157">Profil</span><span class="sxs-lookup"><span data-stu-id="b33c5-157">Profile</span></span>

* <span data-ttu-id="b33c5-158">`az account get-access-token`: Parameter `--tenant` hinzugefügt, um das Token für den Mandanten direkt abzurufen. Es muss kein Abonnement angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="b33c5-158">`az account get-access-token`: Add `--tenant` parameter to acquire token for the tenant directly, needless to specify a subscription</span></span>

### <a name="rbac"></a><span data-ttu-id="b33c5-159">RBAC</span><span class="sxs-lookup"><span data-stu-id="b33c5-159">RBAC</span></span>

* <span data-ttu-id="b33c5-160">[BREAKING CHANGE] Behebung Nr. 11883: `az role assignment create`: Bei leerem Bereich wird ein Fehler ausgegeben.</span><span class="sxs-lookup"><span data-stu-id="b33c5-160">[BREAKING CHANGE] Fix #11883: `az role assignment create`: empty scope will prompt error</span></span>

### <a name="security"></a><span data-ttu-id="b33c5-161">Sicherheit</span><span class="sxs-lookup"><span data-stu-id="b33c5-161">Security</span></span>

* <span data-ttu-id="b33c5-162">Neue Befehle `az atp show` und `az atp update` hinzugefügt, um erweiterte Einstellungen für den Bedrohungsschutz für Speicherkonten anzuzeigen und zu verwalten</span><span class="sxs-lookup"><span data-stu-id="b33c5-162">Add new commands `az atp show` and `az atp update` to view and manage advanced threat protection settings for storage accounts.</span></span>

### <a name="sql"></a><span data-ttu-id="b33c5-163">SQL</span><span class="sxs-lookup"><span data-stu-id="b33c5-163">SQL</span></span>

* <span data-ttu-id="b33c5-164">`sql dw create`: Parameter `--zone-redundant` und `--read-replica-count` als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="b33c5-164">`sql dw create`: deprecate `--zone-redundant` and `--read-replica-count` parameters.</span></span> <span data-ttu-id="b33c5-165">Diese Parameter gelten nicht für Datawarehouse.</span><span class="sxs-lookup"><span data-stu-id="b33c5-165">These parameters do not apply to DataWarehouse.</span></span>
* <span data-ttu-id="b33c5-166">[BREAKING CHANGE] `az sql db create`: „WideWorldImportersStd“ und „WideWorldImportersFull“ als dokumentierte zulässige Werte für „az sql db create --sample-name“ entfernt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-166">[BREAKING CHANGE] `az sql db create`: Remove "WideWorldImportersStd" and "WideWorldImportersFull" as documented allowed values for "az sql db create --sample-name".</span></span> <span data-ttu-id="b33c5-167">Diese Beispieldatenbanken führen immer zu einem Fehler bei der Erstellung.</span><span class="sxs-lookup"><span data-stu-id="b33c5-167">These sample databases would always cause creation to fail.</span></span>
* <span data-ttu-id="b33c5-168">Neue Befehle `sql db classification show/list/update/delete` und `sql db classification recommendation list/enable/disable` zur Verwaltung von Vertraulichkeitsklassifizierungen für SQL-Datenbanken hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-168">Add New commands `sql db classification show/list/update/delete` and `sql db classification recommendation list/enable/disable` to manage sensitivity classifications for SQL databases.</span></span>
* <span data-ttu-id="b33c5-169">`az sql db audit-policy`: Behebung für leere Überwachungsaktionen und -gruppen</span><span class="sxs-lookup"><span data-stu-id="b33c5-169">`az sql db audit-policy`: Fix for empty audit actions and groups</span></span>

### <a name="storage"></a><span data-ttu-id="b33c5-170">Storage</span><span class="sxs-lookup"><span data-stu-id="b33c5-170">Storage</span></span>

* <span data-ttu-id="b33c5-171">Neue Befehlsgruppe `az storage share-rm` hinzugefügt, um den Ressourcenanbieter „Microsoft.Storage“ für Verwaltungsvorgänge der Azure-Dateifreigabe zu verwenden</span><span class="sxs-lookup"><span data-stu-id="b33c5-171">Add a new command group `az storage share-rm` to use the Microsoft.Storage resource provider for Azure file share management operations.</span></span>
* <span data-ttu-id="b33c5-172">Behebung für Problem Nr. 11415: Berechtigungsfehler für `az storage blob update`</span><span class="sxs-lookup"><span data-stu-id="b33c5-172">Fix issue #11415: permission error for `az storage blob update`</span></span>
* <span data-ttu-id="b33c5-173">Integration von Azcopy 10.3.3 und Unterstützung von Win32</span><span class="sxs-lookup"><span data-stu-id="b33c5-173">Integrate Azcopy 10.3.3 and support Win32.</span></span>
* <span data-ttu-id="b33c5-174">`az storage copy`: Parameter `--include-path`, `--include-pattern`, `--exclude-path` und`--exclude-pattern` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-174">`az storage copy`: Add `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="b33c5-175">`az storage remove`: Parameter `--inlcude` und `--exclude` in Parameter `--include-path`, `--include-pattern`, `--exclude-path` und`--exclude-pattern` geändert</span><span class="sxs-lookup"><span data-stu-id="b33c5-175">`az storage remove`: Change `--inlcude` and `--exclude` parameters to `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="b33c5-176">`az storage sync`: Parameter `--include-pattern`, `--exclude-path` und`--exclude-pattern` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-176">`az storage sync`: Add `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>

### <a name="servicefabric"></a><span data-ttu-id="b33c5-177">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="b33c5-177">ServiceFabric</span></span>

* <span data-ttu-id="b33c5-178">Neue Befehle zum Verwalten von Anwendung und Diensten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-178">Add new commands to manage appliaction and services.</span></span>

## <a name="january-13-2020"></a><span data-ttu-id="b33c5-179">13. Januar 2020</span><span class="sxs-lookup"><span data-stu-id="b33c5-179">January 13, 2020</span></span>

<span data-ttu-id="b33c5-180">Version 2.0.80</span><span class="sxs-lookup"><span data-stu-id="b33c5-180">Version 2.0.80</span></span>

### <a name="compute"></a><span data-ttu-id="b33c5-181">Compute</span><span class="sxs-lookup"><span data-stu-id="b33c5-181">Compute</span></span>

* <span data-ttu-id="b33c5-182">Datenträgeraktualisierung: „--disk-encryption-set“ und „--encryption-type“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-182">disk update: Add --disk-encryption-set and --encryption-type</span></span>
* <span data-ttu-id="b33c5-183">Momentaufnahmeerstellung/-aktualisierung: „--disk-encryption-set“ und „--encryption-type“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-183">snapshot create/update: Add --disk-encryption-set and --encryption-type</span></span>

### <a name="storage"></a><span data-ttu-id="b33c5-184">Storage</span><span class="sxs-lookup"><span data-stu-id="b33c5-184">Storage</span></span>

* <span data-ttu-id="b33c5-185">„azure-mgmt-storage“ auf Version 7.1.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-185">Upgrade azure-mgmt-storage version to 7.1.0</span></span>
* <span data-ttu-id="b33c5-186">`az storage account create`: `--encryption-key-type-for-table` und `--encryption-key-type-for-queue` zur Unterstützung des Tabellen- und Warteschlangenverschlüsselungsdiensts hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-186">`az storage account create`: Add `--encryption-key-type-for-table` and `--encryption-key-type-for-queue` to support Table and Queue Encryption Service</span></span>

## <a name="january-07-2020"></a><span data-ttu-id="b33c5-187">7\. Januar 2020</span><span class="sxs-lookup"><span data-stu-id="b33c5-187">January 07, 2020</span></span>

<span data-ttu-id="b33c5-188">Version 2.0.79</span><span class="sxs-lookup"><span data-stu-id="b33c5-188">Version 2.0.79</span></span>

### <a name="acr"></a><span data-ttu-id="b33c5-189">ACR</span><span class="sxs-lookup"><span data-stu-id="b33c5-189">ACR</span></span>

* <span data-ttu-id="b33c5-190">[BREAKING CHANGE] Parameter „--os“ für „acr build“, „acr task create/update“, „acr run“ und „acr pack“ wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-190">[BREAKING CHANGE] Remove '--os' parameter for 'acr build', 'acr task create/update', 'acr run', and 'acr pack'.</span></span> <span data-ttu-id="b33c5-191">Verwenden Sie stattdessen „--platform“.</span><span class="sxs-lookup"><span data-stu-id="b33c5-191">Use '--platform' instead.</span></span>

### <a name="appconfig"></a><span data-ttu-id="b33c5-192">AppConfig</span><span class="sxs-lookup"><span data-stu-id="b33c5-192">AppConfig</span></span>

* <span data-ttu-id="b33c5-193">Unterstützung für das Importieren/Exportieren von Featureflags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-193">Add support for importing/exporting feature flags</span></span>
* <span data-ttu-id="b33c5-194">Neuer Befehl „az appconfig kv set-keyvault“ für das Erstellen einer KeyVault-Referenz hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-194">Add new command 'az appconfig kv set-keyvault' for creating keyvault reference</span></span>
* <span data-ttu-id="b33c5-195">Unterstützung verschiedener Benennungskonventionen beim Exportieren von Featureflags in eine Datei</span><span class="sxs-lookup"><span data-stu-id="b33c5-195">Support various naming conventions when exporting feature flags to file</span></span>

### <a name="appservice"></a><span data-ttu-id="b33c5-196">AppService</span><span class="sxs-lookup"><span data-stu-id="b33c5-196">AppService</span></span>

* <span data-ttu-id="b33c5-197">Behebung von Problem Nr. 7154: Aktualisierung der Dokumentation für Befehl „<>“, sodass Backticks anstelle von einfachen Anführungszeichen verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="b33c5-197">Fix issue #7154: Updating documentation for command <> to use back ticks instead of single quotes</span></span>
* <span data-ttu-id="b33c5-198">Behebung von Problem Nr. 11287: „webapp up“: Für die mit „up“ erstellte App muss standardmäßig SSL aktiviert sein.</span><span class="sxs-lookup"><span data-stu-id="b33c5-198">Fix issue #11287: webapp up: By default make the app created using up 'should be 'SSL enabled'</span></span>
* <span data-ttu-id="b33c5-199">Behebung von Problem Nr. 11592: Flag „az webapp up“ für statische HTML-Websites hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-199">Fix issue #11592: Add az webapp up flag for html static sites</span></span>

### <a name="arm"></a><span data-ttu-id="b33c5-200">ARM</span><span class="sxs-lookup"><span data-stu-id="b33c5-200">ARM</span></span>

* <span data-ttu-id="b33c5-201">Behebung `az resource tag`: Recovery Services-Tresor-Tags können nicht aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="b33c5-201">Fix `az resource tag`: Recovery Services Vault tags cannot be updated</span></span>

### <a name="backup"></a><span data-ttu-id="b33c5-202">Backup</span><span class="sxs-lookup"><span data-stu-id="b33c5-202">Backup</span></span>

* <span data-ttu-id="b33c5-203">Neuer Befehl „backup protection undelete“ hinzugefügt, um die Funktion zum vorläufigen Löschen für IaasVM-Workloads zu aktivieren</span><span class="sxs-lookup"><span data-stu-id="b33c5-203">Added new command 'backup protection undelete' to enable soft-delete feature for IaasVM workload</span></span>
* <span data-ttu-id="b33c5-204">Neuer Parameter „--soft-delete-feature-state“ hinzugefügt, um den Befehl „backup-properties“ festzulegen</span><span class="sxs-lookup"><span data-stu-id="b33c5-204">Added new parameter '--soft-delete-feature-state' to set backup-properties command</span></span>
* <span data-ttu-id="b33c5-205">Unterstützung für den Ausschluss von Datenträgern für IaasVM-Workload hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-205">Added disk exclusion support for IaasVM workload</span></span>

### <a name="compute"></a><span data-ttu-id="b33c5-206">Compute</span><span class="sxs-lookup"><span data-stu-id="b33c5-206">Compute</span></span>

* <span data-ttu-id="b33c5-207">Fehler `vm create` in Azure Stack-Profil behoben.</span><span class="sxs-lookup"><span data-stu-id="b33c5-207">Fix `vm create` failure in Azure Stack profile.</span></span>
* <span data-ttu-id="b33c5-208">vm monitor metrics tail/list-definitions: Unterstützung einer Abfragemetrik und von Listendefinitionen für eine VM.</span><span class="sxs-lookup"><span data-stu-id="b33c5-208">vm monitor metrics tail/list-definitions: support query metric and list definitions for a vm.</span></span>
* <span data-ttu-id="b33c5-209">Neue Aktion des Befehls zum erneuten Anwenden für „az vm“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-209">Add new reapply command action for az vm</span></span>

### <a name="hdinsight"></a><span data-ttu-id="b33c5-210">HDInsight</span><span class="sxs-lookup"><span data-stu-id="b33c5-210">HDInsight</span></span>

* <span data-ttu-id="b33c5-211">Unterstützung für das Erstellen eines Kafka-Clusters mit Kafka-REST-Proxy</span><span class="sxs-lookup"><span data-stu-id="b33c5-211">Support for creating a Kafka cluster with Kafka Rest Proxy</span></span>
* <span data-ttu-id="b33c5-212">„azure-mgmt-hdinsight“ auf 1.3.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-212">Upgrade azure-mgmt-hdinsight to 1.3.0</span></span>

### <a name="misc"></a><span data-ttu-id="b33c5-213">Verschiedenes:</span><span class="sxs-lookup"><span data-stu-id="b33c5-213">Misc.</span></span>

* <span data-ttu-id="b33c5-214">Vorschaubefehl `az version show` hinzugefügt, um die Versionen der Azure CLI-Module und Erweiterungen standardmäßig im JSON-Format oder im mit „--output“ konfigurierten Format anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="b33c5-214">Add preview command `az version show` to show the versions of Azure CLI modules and extensions in JSON format by default or format configured by --output</span></span>

### <a name="event-hubs"></a><span data-ttu-id="b33c5-215">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="b33c5-215">Event Hubs</span></span>

* <span data-ttu-id="b33c5-216">[BREAKING CHANGE] Statusoption „ReceiveDisabled“ aus „az eventhubs eventhub update“ und „az eventhubs eventhub create“ entfernt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-216">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az eventhubs eventhub update' and 'az eventhubs eventhub create'.</span></span> <span data-ttu-id="b33c5-217">Diese Option ist für Event Hub-Entitäten nicht gültig.</span><span class="sxs-lookup"><span data-stu-id="b33c5-217">This option is not valid for Event Hub entities.</span></span>

### <a name="service-bus"></a><span data-ttu-id="b33c5-218">Service Bus</span><span class="sxs-lookup"><span data-stu-id="b33c5-218">Service Bus</span></span>

* <span data-ttu-id="b33c5-219">[BREAKING CHANGE] Statusoption „ReceiveDisabled“ aus Befehlen „az servicebus topic create“, „az servicebus topic update“, „az servicebus queue create“ und „az servicebus queue update“ entfernt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-219">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az servicebus topic create', 'az servicebus topic update', 'az servicebus queue create', and 'az servicebus queue update'.</span></span> <span data-ttu-id="b33c5-220">Diese Option ist für Service Bus-Themen und -Warteschlangen nicht gültig.</span><span class="sxs-lookup"><span data-stu-id="b33c5-220">This option is not valid for Service Bus topics and queues.</span></span>

### <a name="rbac"></a><span data-ttu-id="b33c5-221">RBAC</span><span class="sxs-lookup"><span data-stu-id="b33c5-221">RBAC</span></span>

* <span data-ttu-id="b33c5-222">Behebung Nr. 11712: `az ad app/sp show` gibt nicht den Exitcode 3 zurück, wenn die Anwendung oder der Dienstprinzipal nicht vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="b33c5-222">Fix #11712: `az ad app/sp show` does not return exit code 3 when the application or service principal does not exist</span></span>

### <a name="storage"></a><span data-ttu-id="b33c5-223">Storage</span><span class="sxs-lookup"><span data-stu-id="b33c5-223">Storage</span></span>

* <span data-ttu-id="b33c5-224">`az storage account create`: Vorschaukennzeichnung für Parameter „--enable-hierarchical-namespace“ entfernt</span><span class="sxs-lookup"><span data-stu-id="b33c5-224">`az storage account create`: Remove preview flag for --enable-hierarchical-namespace parameter</span></span>
* <span data-ttu-id="b33c5-225">azure-mgmt-storage-Version auf 7.0.0 aktualisiert, um API-Version 2019-06-01 zu verwenden</span><span class="sxs-lookup"><span data-stu-id="b33c5-225">Update azure-mgmt-storage version to 7.0.0 to use api version 2019-06-01</span></span>
* <span data-ttu-id="b33c5-226">Neue Parameter `--enable-delete-retention` und `--delete-retention-days` hinzugefügt, um die Verwaltung der Aufbewahrungsrichtlinie für Löschen für „blob-service-properties“ von Speicherkonten zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="b33c5-226">Add new parameters `--enable-delete-retention` and `--delete-retention-days` to support managing delete retention policy for storage account blob-service-properties.</span></span>

## <a name="december-17-2019"></a><span data-ttu-id="b33c5-227">17. Dezember 2019</span><span class="sxs-lookup"><span data-stu-id="b33c5-227">December 17, 2019</span></span>

<span data-ttu-id="b33c5-228">2.0.78</span><span class="sxs-lookup"><span data-stu-id="b33c5-228">2.0.78</span></span>

### <a name="acr"></a><span data-ttu-id="b33c5-229">ACR</span><span class="sxs-lookup"><span data-stu-id="b33c5-229">ACR</span></span>

* <span data-ttu-id="b33c5-230">Unterstützung für lokalen Kontext in „acr task run“</span><span class="sxs-lookup"><span data-stu-id="b33c5-230">Added support Local context in acr task run</span></span>

### <a name="acs"></a><span data-ttu-id="b33c5-231">ACS</span><span class="sxs-lookup"><span data-stu-id="b33c5-231">ACS</span></span>

* <span data-ttu-id="b33c5-232">[BREAKING CHANGE] az openshift create: `--workspace-resource-id` in `--workspace-id` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-232">[BREAKING CHANGE]az openshift create: rename `--workspace-resource-id` to `--workspace-id`.</span></span>

### <a name="ams"></a><span data-ttu-id="b33c5-233">AMS</span><span class="sxs-lookup"><span data-stu-id="b33c5-233">AMS</span></span>

* <span data-ttu-id="b33c5-234">Befehle zum Anzeigen aktualisiert, sodass 3 zurückgegeben wird, wenn die Ressource nicht gefunden wurde</span><span class="sxs-lookup"><span data-stu-id="b33c5-234">Updated show commands to return 3 when resource not found</span></span>

### <a name="appconfig"></a><span data-ttu-id="b33c5-235">AppConfig</span><span class="sxs-lookup"><span data-stu-id="b33c5-235">AppConfig</span></span>

* <span data-ttu-id="b33c5-236">Fehler beim Anhängen der API-Version an die Anforderungs-URL korrigiert.</span><span class="sxs-lookup"><span data-stu-id="b33c5-236">Fixed bug when appending api-version to request url.</span></span> <span data-ttu-id="b33c5-237">Die vorhandene Lösung funktioniert nicht mit Paginierung.</span><span class="sxs-lookup"><span data-stu-id="b33c5-237">The existing solution doesn't work with pagination.</span></span>
* <span data-ttu-id="b33c5-238">Unterstützung für die Anzeige von weiteren Sprachen neben Englisch hinzugefügt, da der Back-End-Dienst Unicode für die Globalisierung unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-238">Added support for showing languages besides English as our backend service support unicode for globalization.</span></span>

### <a name="appservice"></a><span data-ttu-id="b33c5-239">AppService</span><span class="sxs-lookup"><span data-stu-id="b33c5-239">AppService</span></span>

* <span data-ttu-id="b33c5-240">Problem Nr. 11217 behoben: Web-App: „az webapp config ssl upload“ muss Slot-Parameter unterstützen.</span><span class="sxs-lookup"><span data-stu-id="b33c5-240">Fixed issue #11217: webapp: az webapp config ssl upload should support slot parameter</span></span>
* <span data-ttu-id="b33c5-241">Problem Nr. 10965 behoben: Error: Der Name darf nicht leer sein.</span><span class="sxs-lookup"><span data-stu-id="b33c5-241">Fixed issue #10965: Error: Name cannot be empty.</span></span> <span data-ttu-id="b33c5-242">Entfernen anhand von „ip_address“ und „subnet“ zulassen</span><span class="sxs-lookup"><span data-stu-id="b33c5-242">Allow remove by ip_address and subnet</span></span>
* <span data-ttu-id="b33c5-243">Unterstützung des Imports von Zertifikaten aus Key Vault hinzugefügt `az webapp config ssl import`</span><span class="sxs-lookup"><span data-stu-id="b33c5-243">Added support for importing certificates from Key Vault `az webapp config ssl import`</span></span>

### <a name="arm"></a><span data-ttu-id="b33c5-244">ARM</span><span class="sxs-lookup"><span data-stu-id="b33c5-244">ARM</span></span>

* <span data-ttu-id="b33c5-245">Paket „azure-mgmt-resource“ auf die Verwendung von 6.0.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-245">Updated azure-mgmt-resource package to use 6.0.0</span></span>
* <span data-ttu-id="b33c5-246">Mandantenübergreifende Unterstützung für Befehl `az group deployment create` durch Hinzufügen des neuen Parameters `--aux-subs`</span><span class="sxs-lookup"><span data-stu-id="b33c5-246">Cross Tenant Support for `az group deployment create` command by adding new parameter `--aux-subs`</span></span>
* <span data-ttu-id="b33c5-247">Neuer Parameter `--metadata` hinzugefügt, um das Hinzufügen von Metadateninformationen für Richtliniensatzdefinitionen zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="b33c5-247">Added new parameter `--metadata` to support adding metadata information for policy set definitions.</span></span>

### <a name="backup"></a><span data-ttu-id="b33c5-248">Backup</span><span class="sxs-lookup"><span data-stu-id="b33c5-248">Backup</span></span>

* <span data-ttu-id="b33c5-249">Unterstützung der Sicherung für SQL- und SAP Hana-Workloads hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-249">Added Backup support for SQL and SAP Hana workload.</span></span>

### <a name="botservice"></a><span data-ttu-id="b33c5-250">BotService</span><span class="sxs-lookup"><span data-stu-id="b33c5-250">BotService</span></span>

* <span data-ttu-id="b33c5-251">[Breaking Change] Flag „--version“ aus Vorschaubefehl „az bot create“ entfernt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-251">[Breaking change] Remove '--version' flag from preview command 'az bot create'.</span></span> <span data-ttu-id="b33c5-252">Nur v4-SDK-Bots werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-252">Only v4 SDK bots are supported.</span></span>
* <span data-ttu-id="b33c5-253">Überprüfung der Namensverfügbarkeit für „az bot create“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-253">Added name availability check for 'az bot create'.</span></span>
* <span data-ttu-id="b33c5-254">Unterstützung für das Aktualisieren der Symbol-URL für einen Bot über „az bot update“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-254">Added support for updating the icon URL for a bot via 'az bot update'.</span></span>
* <span data-ttu-id="b33c5-255">Unterstützung für das Aktualisieren eines Direct Line-Kanals über „az bot directline update“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-255">Added support for updating a Direct Line channel via 'az bot directline update'.</span></span>
* <span data-ttu-id="b33c5-256">Unterstützung für Flag „--enable-enhanced-auth“ zu „az bot directline create“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-256">Added '--enable-enhanced-auth' flag support to 'az bot directline create'.</span></span>
* <span data-ttu-id="b33c5-257">Die folgenden Befehlsgruppen sind allgemein verfügbar und befinden sich nicht in der Vorschau: „az bot authsetting“.</span><span class="sxs-lookup"><span data-stu-id="b33c5-257">The following command groups are GA and not in preview: 'az bot authsetting'.</span></span>
* <span data-ttu-id="b33c5-258">Die folgenden Befehle in „az bot“ sind allgemein verfügbar und befinden sich nicht in der Vorschau: „create“, „prepare-deploy“, „show“, „delete“, „update“.</span><span class="sxs-lookup"><span data-stu-id="b33c5-258">The following commands in 'az bot' are GA and not in preview: 'create', 'prepare-deploy', 'show', 'delete', 'update'.</span></span>
* <span data-ttu-id="b33c5-259">„az bot prepare-deploy“ korrigiert, indem der Wert voon „--proj-file-path“ in Kleinschreibung geändert wurde (z. B. „Test.csproj“ in „test.csproj“).</span><span class="sxs-lookup"><span data-stu-id="b33c5-259">Fixed 'az bot prepare-deploy' changing '--proj-file-path' value to lower case (e.g. "Test.csproj" to "test.csproj").</span></span>

### <a name="compute"></a><span data-ttu-id="b33c5-260">Compute</span><span class="sxs-lookup"><span data-stu-id="b33c5-260">Compute</span></span>

* <span data-ttu-id="b33c5-261">vmss create/update: „--scale-in-policy“ hinzugefügt, womit entschieden wird, welche virtuellen Computer beim horizontalen Herunterskalieren einer VM-Skalierungsgruppe zum Entfernen ausgewählt werden.</span><span class="sxs-lookup"><span data-stu-id="b33c5-261">vmss create/update: Added --scale-in-policy, which decides which virtual machines are chosen for removal when a VMSS is scaled-in.</span></span>
* <span data-ttu-id="b33c5-262">vm/vmss update: „--priority“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-262">vm/vmss update: Added --priority.</span></span>
* <span data-ttu-id="b33c5-263">vm/vmss update: „--max-price“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-263">vm/vmss update: Added --max-price.</span></span>
* <span data-ttu-id="b33c5-264">Befehlsgruppe „disk-encryption-set“ hinzugefügt (create, show, update, delete, list).</span><span class="sxs-lookup"><span data-stu-id="b33c5-264">Added disk-encryption-set command group (create, show, update, delete, list).</span></span>
* <span data-ttu-id="b33c5-265">disk create: „--encryption-type“ und „--disk-encryption-set“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-265">disk create: Added --encryption-type and --disk-encryption-set.</span></span>
* <span data-ttu-id="b33c5-266">vm/vmss create: „--os-disk-encryption-set“ und „--data-disk-encryption-sets“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-266">vm/vmss create: Added --os-disk-encryption-set and --data-disk-encryption-sets.</span></span>

### <a name="core"></a><span data-ttu-id="b33c5-267">Core</span><span class="sxs-lookup"><span data-stu-id="b33c5-267">Core</span></span>

* <span data-ttu-id="b33c5-268">Unterstützung für Python 3.4 entfernt</span><span class="sxs-lookup"><span data-stu-id="b33c5-268">Removed support for Python 3.4</span></span>
* <span data-ttu-id="b33c5-269">Plug-In für HaTS-Umfrage in mehreren Befehlen</span><span class="sxs-lookup"><span data-stu-id="b33c5-269">Plug in HaTS survey in multiple commands</span></span>

### <a name="dls"></a><span data-ttu-id="b33c5-270">DLS</span><span class="sxs-lookup"><span data-stu-id="b33c5-270">DLS</span></span>

* <span data-ttu-id="b33c5-271">ADLS-SDK-Version aktualisiert (0.0.48).</span><span class="sxs-lookup"><span data-stu-id="b33c5-271">Updated ADLS sdk version (0.0.48).</span></span>

### <a name="install"></a><span data-ttu-id="b33c5-272">Installieren</span><span class="sxs-lookup"><span data-stu-id="b33c5-272">Install</span></span>

* <span data-ttu-id="b33c5-273">Installationsskript unterstützt Python 3.8</span><span class="sxs-lookup"><span data-stu-id="b33c5-273">Install script support python 3.8</span></span>

### <a name="iot"></a><span data-ttu-id="b33c5-274">IoT</span><span class="sxs-lookup"><span data-stu-id="b33c5-274">IOT</span></span>

* <span data-ttu-id="b33c5-275">[BREAKING CHANGE] Parameter „--failover-region“ aus „manual-failover“ entfernt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-275">[BREAKING CHANGE] Removed --failover-region parameter from manual-failover.</span></span> <span data-ttu-id="b33c5-276">Das Failover erfolgt jetzt in eine zugewiesene, geografisch gekoppelte sekundäre Region.</span><span class="sxs-lookup"><span data-stu-id="b33c5-276">Now it will failover to assigned geo-paired secondary region.</span></span>

### <a name="key-vault"></a><span data-ttu-id="b33c5-277">Key Vault</span><span class="sxs-lookup"><span data-stu-id="b33c5-277">Key Vault</span></span>

* <span data-ttu-id="b33c5-278">Nr. 8095 behoben: `az keyvault storage remove`: Hilfemeldung verbessert</span><span class="sxs-lookup"><span data-stu-id="b33c5-278">Fixed #8095: `az keyvault storage remove`: improve the help message</span></span>
* <span data-ttu-id="b33c5-279">Nr. 8921 behoben: `az keyvault key/secret/certificate list/list-deleted/list-versions`: Validierungsfehler in Parameter `--maxresults` behoben</span><span class="sxs-lookup"><span data-stu-id="b33c5-279">Fixed #8921: `az keyvault key/secret/certificate list/list-deleted/list-versions`: fix the validation bug on parameter `--maxresults`</span></span>
* <span data-ttu-id="b33c5-280">Nr. 10512 behoben: `az keyvault set-policy`: Fehlermeldung verbessert, wenn weder `--object-id`, `--spn` noch `--upn` angegeben ist</span><span class="sxs-lookup"><span data-stu-id="b33c5-280">Fixed #10512: `az keyvault set-policy`: improve the error message when none of `--object-id`, `--spn` or `--upn` is specified</span></span>
* <span data-ttu-id="b33c5-281">Nr. 10846 behoben: `az keyvault secret show-deleted`: Wenn `--id` angegeben ist, ist `--name/-n` nicht erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b33c5-281">Fixed #10846: `az keyvault secret show-deleted`: when `--id` is specified, `--name/-n` is not required</span></span>
* <span data-ttu-id="b33c5-282">Nr. 11084 behoben: `az keyvault secret download`: Hilfemeldung von Parameter `--encoding` verbessert</span><span class="sxs-lookup"><span data-stu-id="b33c5-282">Fixed #11084: `az keyvault secret download`: improve the help message of parameter `--encoding`</span></span>

### <a name="network"></a><span data-ttu-id="b33c5-283">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="b33c5-283">Network</span></span>

* <span data-ttu-id="b33c5-284">az network application-gateway probe: Unterstützung für Option „--port“ hinzugefügt, um einen Port zum Prüfen von Back-End-Servern beim Erstellen und Aktualisieren anzugeben</span><span class="sxs-lookup"><span data-stu-id="b33c5-284">az network application-gateway probe: Added support --port option to specify a port for probing backend servers when create and update</span></span>
* <span data-ttu-id="b33c5-285">az network application-gateway url-path-map create/update: Fehlerbehebung für `--waf-policy`</span><span class="sxs-lookup"><span data-stu-id="b33c5-285">az network application-gateway url-path-map create/update: bug fix for `--waf-policy`</span></span>
* <span data-ttu-id="b33c5-286">az network application-gateway: Unterstützung für `--rewrite-rule-set` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-286">az network application-gateway: Added support `--rewrite-rule-set`</span></span>
* <span data-ttu-id="b33c5-287">az network list-service-aliases: Unterstützung für Listendienstaliase hinzugefügt, die für Dienstendpunktrichtlinien verwendet werden können</span><span class="sxs-lookup"><span data-stu-id="b33c5-287">az network list-service-aliases: Added support list service aliases which can be used for Service Endpoint Policies</span></span>
* <span data-ttu-id="b33c5-288">az network dns zone import: Unterstützung für „.@“ in Datensatzname hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-288">az network dns zone import: Added support .@ in record name</span></span>

### <a name="packaging"></a><span data-ttu-id="b33c5-289">Verpackung</span><span class="sxs-lookup"><span data-stu-id="b33c5-289">Packaging</span></span>

* <span data-ttu-id="b33c5-290">Back-Edge-Builds für PIP-Installation hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-290">Added back edge builds for pip install</span></span>
* <span data-ttu-id="b33c5-291">Ubuntu-Eoan-Paket hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-291">Added Ubuntu eoan package</span></span>

### <a name="policy"></a><span data-ttu-id="b33c5-292">Richtlinie</span><span class="sxs-lookup"><span data-stu-id="b33c5-292">Policy</span></span>

* <span data-ttu-id="b33c5-293">Unterstützung für Version 2019-09-01 der Richtlinien-API hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-293">Added support for Policy API version 2019-09-01.</span></span>
* <span data-ttu-id="b33c5-294">az policy set-definition: Unterstützung der Gruppierung innerhalb von Richtliniensatzdefinitionen mit `--definition-groups`-Parameter hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-294">az policy set-definition: Added support grouping within policy set definitions with `--definition-groups` parameter</span></span>

### <a name="redis"></a><span data-ttu-id="b33c5-295">Redis</span><span class="sxs-lookup"><span data-stu-id="b33c5-295">Redis</span></span>

* <span data-ttu-id="b33c5-296">Vorschauparameter `--replicas-per-master` zu Befehl `az redis create`hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-296">Added preview param `--replicas-per-master` to `az redis create` command</span></span>
* <span data-ttu-id="b33c5-297">„azure-mgmt-redis“ von 6.0.0 auf 7.0.0rc1 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-297">Updated azure-mgmt-redis from 6.0.0 to 7.0.0rc1</span></span>

### <a name="servicefabric"></a><span data-ttu-id="b33c5-298">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="b33c5-298">ServiceFabric</span></span>

* <span data-ttu-id="b33c5-299">Hinzufügen von Logik in Knotentyp korrigiert, einschließlich Nr. 10963: Beim Hinzufügen eines neuen Knotentyps mit Dauerhaftigkeitsstufe „Gold“ wird immer ein CLI-Fehler ausgegeben.</span><span class="sxs-lookup"><span data-stu-id="b33c5-299">Fixed in node-type add logic including #10963: Adding new node type with durability level Gold will always throw CLI error</span></span>
* <span data-ttu-id="b33c5-300">ServiceFabricNodeVmExt-Version in Erstellungsvorlage auf 1.1 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-300">Updated ServiceFabricNodeVmExt version to 1.1 in creation template</span></span>

### <a name="sql"></a><span data-ttu-id="b33c5-301">SQL</span><span class="sxs-lookup"><span data-stu-id="b33c5-301">SQL</span></span>

* <span data-ttu-id="b33c5-302">Parameter „--read-scale“ und „--read-replicas“ zu Befehlen „sql db create“ und „sql db update“ hinzugefügt, um Leseskalierungsverwaltung zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="b33c5-302">Added "--read-scale" and "--read-replicas" parameters to sql db create and update commands, to support read scale management.</span></span>

### <a name="storage"></a><span data-ttu-id="b33c5-303">Storage</span><span class="sxs-lookup"><span data-stu-id="b33c5-303">Storage</span></span>

* <span data-ttu-id="b33c5-304">Allgemein verfügbares Release – Eigenschaft „Large File Shares“ für Befehle „storage account create“ und „storage account update“</span><span class="sxs-lookup"><span data-stu-id="b33c5-304">GA Release Large File Shares property for storage account create and update command</span></span>
* <span data-ttu-id="b33c5-305">Allgemein verfügbares Release – Unterstützung von SAS-Token für die Benutzerdelegierung</span><span class="sxs-lookup"><span data-stu-id="b33c5-305">GA Release User Delegation SAS token Support</span></span>
* <span data-ttu-id="b33c5-306">Neue Befehle `az storage account blob-service-properties show` und `az storage account blob-service-properties update --enable-change-feed` hinzugefügt, um Blob-Diensteigenschaften für das Speicherkonto zu verwalten.</span><span class="sxs-lookup"><span data-stu-id="b33c5-306">Added new commands `az storage account blob-service-properties show` and `az storage account blob-service-properties update --enable-change-feed` to manage blob service properties for storage account.</span></span>
* <span data-ttu-id="b33c5-307">[BEVORSTEHENDER BREAKING CHANGE] `az storage copy`: Das Zeichen `*` wird nicht mehr als Platzhalter in der URL, es werden jedoch die neuen Parameter „--include-pattern“ und „--exclude-pattern“ mit Unterstützung des Platzhalters `*` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-307">[COMING BREAKING CHANGE] `az storage copy`: `*` character is no longer supported as a wildcard in URL, but new parameters --include-pattern and --exclude-pattern will be added with `*` wildcard support.</span></span>
* <span data-ttu-id="b33c5-308">Problem Nr. 11043 behoben: Unterstützung für das Entfernen des gesamten Containers/der gesamten Freigabe in `az storage remove` Befehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-308">Fixed issue #11043: Added support to remove whole container/share in `az storage remove` command</span></span>

## <a name="november-26-2019"></a><span data-ttu-id="b33c5-309">26. November 2019</span><span class="sxs-lookup"><span data-stu-id="b33c5-309">November 26, 2019</span></span>

<span data-ttu-id="b33c5-310">Version 2.0.77</span><span class="sxs-lookup"><span data-stu-id="b33c5-310">Version 2.0.77</span></span>

### <a name="acr"></a><span data-ttu-id="b33c5-311">ACR</span><span class="sxs-lookup"><span data-stu-id="b33c5-311">ACR</span></span>

* <span data-ttu-id="b33c5-312">Parameter `--branch` in „acr task create/update“ als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-312">Deprecated parameter `--branch` from acr task create/update</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="b33c5-313">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="b33c5-313">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="b33c5-314">`--workspace-resource-id`-Flag hinzugefügt, um die Erstellung eines Azure Red Hat OpenShift-Clusters mit Überwachung zuzulassen</span><span class="sxs-lookup"><span data-stu-id="b33c5-314">Added `--workspace-resource-id` flag to allow creation of Azure Red Hat Openshift cluster with monitoring</span></span>
* <span data-ttu-id="b33c5-315">`monitor_profile`-Flag hinzugefügt, um einen Azure Red Hat OpenShift-Clusters mit Überwachung zu erstellen</span><span class="sxs-lookup"><span data-stu-id="b33c5-315">Added `monitor_profile` to create Azure Red Hat OpenShift cluster with monitoring</span></span>

### <a name="aks"></a><span data-ttu-id="b33c5-316">AKS</span><span class="sxs-lookup"><span data-stu-id="b33c5-316">AKS</span></span>

* <span data-ttu-id="b33c5-317">Unterstützung des Rotationsvorgangs für Clusterzertifikate mithilfe von für Cluster Zertifikat Rotation mit „az aks rotate-certs“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-317">Added support cluster certificate rotation operation using "az aks rotate-certs".</span></span>

### <a name="appconfig"></a><span data-ttu-id="b33c5-318">AppConfig</span><span class="sxs-lookup"><span data-stu-id="b33c5-318">AppConfig</span></span>

* <span data-ttu-id="b33c5-319">Unterstützung für die Verwendung von „:“ für `as az appconfig kv import`-Trennzeichen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-319">Added support for using ":" for `as az appconfig kv import` separator</span></span>
* <span data-ttu-id="b33c5-320">Problem beim Auflisten von Schlüsselwerten mit mehreren Bezeichnungen, einschließlich NULL-Bezeichnung, behoben.</span><span class="sxs-lookup"><span data-stu-id="b33c5-320">Fixed issue for listing key values with multiple labels including null label.</span></span> 
* <span data-ttu-id="b33c5-321">Verwaltungsebenen-SDK, „azure-mgmt-appconfiguration“, auf Version 0.3.0 aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="b33c5-321">Updated management plane sdk, azure-mgmt-appconfiguration, to version 0.3.0.</span></span> 

### <a name="appservice"></a><span data-ttu-id="b33c5-322">AppService</span><span class="sxs-lookup"><span data-stu-id="b33c5-322">AppService</span></span>

* <span data-ttu-id="b33c5-323">Problem Nr. 11100 behoben AttributeError für „az webapp up“ beim Erstellen eines Dienstplans</span><span class="sxs-lookup"><span data-stu-id="b33c5-323">Fixed issue #11100: AttributeError for az webapp up when create service plan</span></span>
* <span data-ttu-id="b33c5-324">az webapp up: Erzwingen der Erstellung oder Bereitstellung auf einer Website für unterstützte Sprachen, es werden keine Standardeinstellungen verwendet.</span><span class="sxs-lookup"><span data-stu-id="b33c5-324">az webapp up: Forcing the creation or deployment to a site for supported languages, no defaults used.</span></span>
* <span data-ttu-id="b33c5-325">Unterstützung für App Service-Umgebung hinzugefügt: az appservice ase show | list | list-addresses | list-plans | create | update | delete</span><span class="sxs-lookup"><span data-stu-id="b33c5-325">Added support for App Service Environment: az appservice ase show | list | list-addresses | list-plans | create | update | delete</span></span>

### <a name="backup"></a><span data-ttu-id="b33c5-326">Backup</span><span class="sxs-lookup"><span data-stu-id="b33c5-326">Backup</span></span>

* <span data-ttu-id="b33c5-327">Problem in Az-Sicherungsrichtlinie „list-associated-items“ behoben.</span><span class="sxs-lookup"><span data-stu-id="b33c5-327">Fixed issue in az backup policy list-associated-items.</span></span> <span data-ttu-id="b33c5-328">Optionaler Parameter „BackupManagementType“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-328">Added optional BackupManagementType parameter.</span></span>

### <a name="compute"></a><span data-ttu-id="b33c5-329">Compute</span><span class="sxs-lookup"><span data-stu-id="b33c5-329">Compute</span></span>

* <span data-ttu-id="b33c5-330">API-Version von Compute, Datenträger, Momentaufnahmen auf 2019-07-01 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-330">Upgraded API version of compute, disks, snapshots to 2019-07-01</span></span>
* <span data-ttu-id="b33c5-331">vmss create: Verbesserung für – Orchestrierungsmodus</span><span class="sxs-lookup"><span data-stu-id="b33c5-331">vmss create: Improvement for --orchestration-mode</span></span>
* <span data-ttu-id="b33c5-332">sig image-definition create: „--os-state“ hinzugefügt, um die Angabe zu ermöglichen, ob die unter diesem Image erstellten virtuellen Computer „generalisiert“ oder „spezialisiert“ sind</span><span class="sxs-lookup"><span data-stu-id="b33c5-332">sig image-definition create: Added --os-state to allow specifying whether the virtual machines created under this image are 'Generalized' or 'Specialized'</span></span>
* <span data-ttu-id="b33c5-333">sig image-definition create: „--hyper-v-generation“ hinzugefügt, um die Angabe der Hypervisorgeneration zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="b33c5-333">sig image-definition create: Added --hyper-v-generation to allow specifying the hypervisor generation</span></span>
* <span data-ttu-id="b33c5-334">sig image-version create: Unterstützung für „--os-snapshot“ und „--data-snapshots“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-334">sig image-version create: Added support --os-snapshot and --data-snapshots</span></span>
* <span data-ttu-id="b33c5-335">image create: „--data-disk-caching“ hinzugefügt, um die Angabe der Zwischenspeicherungseinstellung von Datenträger zu ermöflichen</span><span class="sxs-lookup"><span data-stu-id="b33c5-335">image create: Added --data-disk-caching to allow specifying caching setting of data disks</span></span>
* <span data-ttu-id="b33c5-336">Upgrade des Python-Compute-SDK auf 10.0.0</span><span class="sxs-lookup"><span data-stu-id="b33c5-336">Upgraded Python Compute SDK to 10.0.0</span></span>
* <span data-ttu-id="b33c5-337">vm/vmss create: „Spot“ zu Aufzählungseigenschaft „Priority“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-337">vm/vmss create: Added 'Spot' to 'Priority' enum property</span></span>
* <span data-ttu-id="b33c5-338">[Breaking Change] Parameter „--max-billing“ für sowohl VM als auch VMSS in „--max-price“ umbenannt, um die Konsistenz mit Swagger- und PowerShell-Cmdlets sicherzustellen</span><span class="sxs-lookup"><span data-stu-id="b33c5-338">[Breaking change] Renamed '--max-billing' parameter to '--max-price', for both VM and VMSS, to be consistent with Swagger and Powershell cmdlets</span></span>
* <span data-ttu-id="b33c5-339">vm monitor log show: Unterstützung für das Abfragen von Protokollen über verknüpften Protokollanalyse-Arbeitsbereich hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-339">vm monitor log show: Added support for querying log over linked log analytics workspace.</span></span>

### <a name="iot"></a><span data-ttu-id="b33c5-340">IoT</span><span class="sxs-lookup"><span data-stu-id="b33c5-340">IOT</span></span>

* <span data-ttu-id="b33c5-341">Behebung Nr. 2531: Argumente für Benutzerfreundlichkeit für Hub-Update hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-341">Fix #2531: Added convenience arguments for hub update.</span></span>
* <span data-ttu-id="b33c5-342">Behebung Nr. 8323: Fehlende Parameter zum Erstellen eines benutzerdefinierten Speicherendpunkts hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-342">Fix #8323: Added missing parameters to create storage custom endpoint.</span></span>
* <span data-ttu-id="b33c5-343">Regressionsfehler behoben: Die Änderungen wurden rückgängig gemacht, sodass der standardmäßige Speicherendpunkt überschrieben wurde.</span><span class="sxs-lookup"><span data-stu-id="b33c5-343">Fix regression bug: Reverted the changes which overrides the default storage endpoint.</span></span>

### <a name="key-vault"></a><span data-ttu-id="b33c5-344">Key Vault</span><span class="sxs-lookup"><span data-stu-id="b33c5-344">Key Vault</span></span>

* <span data-ttu-id="b33c5-345">Nr. 11121 behoben: Bei der Verwendung von `az keyvault certificate list` erfordert die Übergabe von `--include-pending` jetzt nicht mehr den Wert `true` oder `false`.</span><span class="sxs-lookup"><span data-stu-id="b33c5-345">Fixed #11121: When using `az keyvault certificate list`, passing `--include-pending` now doesn't require a value of `true` or `false`</span></span>

### <a name="netappfiles"></a><span data-ttu-id="b33c5-346">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="b33c5-346">NetAppFiles</span></span>

* <span data-ttu-id="b33c5-347">Upgrade von „azure-mgmt-netapp“ auf Version 0.7.0, die einige zusätzliche Volumeeigenschaften enthält, die bevorstehenden Replikationsvorgängen zugeordnet sind</span><span class="sxs-lookup"><span data-stu-id="b33c5-347">Upgraded azure-mgmt-netapp to 0.7.0 which includes some additional volume properties associated with upcoming replication operations</span></span>

### <a name="network"></a><span data-ttu-id="b33c5-348">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="b33c5-348">Network</span></span>

* <span data-ttu-id="b33c5-349">application-gateway waf-config: veraltet</span><span class="sxs-lookup"><span data-stu-id="b33c5-349">application-gateway waf-config: deprecated</span></span>
* <span data-ttu-id="b33c5-350">application-gateway waf-policy: Untergruppe „managed-rules“ zur Verwaltung von verwalteten Regelsätzen und Ausschlussregeln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-350">application-gateway waf-policy: Added subgroup managed-rules to manage managed rule sets and exclusion rules</span></span>
* <span data-ttu-id="b33c5-351">application-gateway waf-policy: Untergruppe „policy-setting“ zur Verwaltung der globalen Konfiguration von „waf-policy“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-351">application-gateway waf-policy: Added subgroup policy-setting to manage global configuration of a waf-policy</span></span>
* <span data-ttu-id="b33c5-352">[BREAKING CHANGE] application-gateway waf-policy: Untergruppenregel in „custom-rule“ umbenannt</span><span class="sxs-lookup"><span data-stu-id="b33c5-352">[BREAKING CHANGE] application-gateway waf-policy: Renamed subgroup rule to custom-rule</span></span>
* <span data-ttu-id="b33c5-353">application-gateway http-listener: „--firewall-policy“ beim Erstellen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-353">application-gateway http-listener: Added --firewall-policy when create</span></span>
* <span data-ttu-id="b33c5-354">application-gateway url-path-map rule: „--firewall-policy“ beim Erstellen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-354">application-gateway url-path-map rule: Added --firewall-policy when create</span></span>

### <a name="packaging"></a><span data-ttu-id="b33c5-355">Verpackung</span><span class="sxs-lookup"><span data-stu-id="b33c5-355">Packaging</span></span>

* <span data-ttu-id="b33c5-356">Az-Wrapper in Python neu geschrieben</span><span class="sxs-lookup"><span data-stu-id="b33c5-356">Rewrote the az wrapper in Python</span></span>
* <span data-ttu-id="b33c5-357">Unterstützung für Python 3.8 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-357">Added support for Python 3.8</span></span>
* <span data-ttu-id="b33c5-358">Für RPM-Paket in Python 3 geändert</span><span class="sxs-lookup"><span data-stu-id="b33c5-358">Changed to Python 3 for RPM package</span></span>

### <a name="profile"></a><span data-ttu-id="b33c5-359">Profil</span><span class="sxs-lookup"><span data-stu-id="b33c5-359">Profile</span></span>

* <span data-ttu-id="b33c5-360">Fehler beim Ausführen von `az login -u {} -p {}` mit Microsoft-Konto entfernt</span><span class="sxs-lookup"><span data-stu-id="b33c5-360">Polished error when running `az login -u {} -p {}` with Microsoft account</span></span>
* <span data-ttu-id="b33c5-361">`SSLError` beim Ausführen von `az login` hinter einem Proxy mit einem selbstsignierten Stammzertifikat entfernt</span><span class="sxs-lookup"><span data-stu-id="b33c5-361">Polished `SSLError` when running `az login` behind a proxy with self-signed root certificate</span></span>
* <span data-ttu-id="b33c5-362">Nr. 10578 behoben: `az login` hängt, wenn mehrere Instanzen gleichzeitig unter Windows oder WSL gestartet werden.</span><span class="sxs-lookup"><span data-stu-id="b33c5-362">Fixed #10578: `az login` hangs when more than one instances are launched at the same time on Windows or WSL</span></span>
* <span data-ttu-id="b33c5-363">Nr. 11059 behoben: `az login --allow-no-subscriptions` schlägt fehl, wenn Abonnements im Mandanten vorhanden sind.</span><span class="sxs-lookup"><span data-stu-id="b33c5-363">Fixed #11059: `az login --allow-no-subscriptions` fails if there are subscriptions in the tenant</span></span>
* <span data-ttu-id="b33c5-364">Nr. 11238 behoben: Nach dem Umbenennen eines Abonnements führt die Anmeldung mit MSI dazu, dass das gleiche Abonnement zweimal angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="b33c5-364">Fixed #11238: After renaming a subscription, logging in with MSI will result in the same subscription appearing twice</span></span>

### <a name="rbac"></a><span data-ttu-id="b33c5-365">RBAC</span><span class="sxs-lookup"><span data-stu-id="b33c5-365">RBAC</span></span>

* <span data-ttu-id="b33c5-366">Nr. 10996 behoben: Fehler für `--force-change-password-next-login` in `az ad user update` entfernt, wenn `--password` nicht angegeben ist</span><span class="sxs-lookup"><span data-stu-id="b33c5-366">Fixed #10996: Polish error for `--force-change-password-next-login` in `az ad user update` when `--password` is not specified</span></span>

### <a name="redis"></a><span data-ttu-id="b33c5-367">Redis</span><span class="sxs-lookup"><span data-stu-id="b33c5-367">Redis</span></span>

* <span data-ttu-id="b33c5-368">Nr. 2902 behoben: Festlegen von Speicherkonfigurationen beim Aktualisieren des Basic-SKU-Cache vermeiden</span><span class="sxs-lookup"><span data-stu-id="b33c5-368">Fixed #2902: Avoid setting memory configs while updating Basic SKU cache</span></span>

### <a name="reservations"></a><span data-ttu-id="b33c5-369">Reservations</span><span class="sxs-lookup"><span data-stu-id="b33c5-369">Reservations</span></span>

* <span data-ttu-id="b33c5-370">SDK-Version auf 0.6.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-370">Upgraded SDK Version to 0.6.0</span></span>
* <span data-ttu-id="b33c5-371">Abrechnungsplandetails nach dem Aufrufen von „Get-Gatalogs“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-371">Added billingplan details info after calling Get-Gatalogs</span></span>
* <span data-ttu-id="b33c5-372">Neuer Befehl `az reservations reservation-order calculate` zum Berechnen des Preises für eine Reservierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-372">Added new command `az reservations reservation-order calculate` to calculate the price for a reservation</span></span>
* <span data-ttu-id="b33c5-373">Neuer Befehl `az reservations reservation-order purchase` zum Erwerb einer neuen Reservierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-373">Added new command `az reservations reservation-order purchase` to purchase a new reservation</span></span>

### <a name="rest"></a><span data-ttu-id="b33c5-374">REST</span><span class="sxs-lookup"><span data-stu-id="b33c5-374">Rest</span></span>
* <span data-ttu-id="b33c5-375">`az rest` in allgemeine Verfügbarkeit geändert</span><span class="sxs-lookup"><span data-stu-id="b33c5-375">Changed `az rest` to GA</span></span>

### <a name="sql"></a><span data-ttu-id="b33c5-376">SQL</span><span class="sxs-lookup"><span data-stu-id="b33c5-376">SQL</span></span>

* <span data-ttu-id="b33c5-377">„azure-mgmt-sql“ auf Version 0.15.0 aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="b33c5-377">Updated azure-mgmt-sql to version 0.15.0.</span></span>

### <a name="storage"></a><span data-ttu-id="b33c5-378">Storage</span><span class="sxs-lookup"><span data-stu-id="b33c5-378">Storage</span></span>

* <span data-ttu-id="b33c5-379">storage account create: „--enable-hierarchical-namespace“ hinzugefügt, um Dateisystemsemantik in Blobdienst zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="b33c5-379">storage account create: Added --enable-hierarchical-namespace to support filesystem semantics in blob service.</span></span>
* <span data-ttu-id="b33c5-380">Ausnahme ohne Zusammenhang aus Fehlermeldung entfernt</span><span class="sxs-lookup"><span data-stu-id="b33c5-380">Removed unrelated exception from error message</span></span>
* <span data-ttu-id="b33c5-381">Probleme mit falscher Fehlermeldung „Sie verfügen nicht über die erforderlichen Berechtigungen zum Ausführen dieses Vorgangs“ behoben.</span><span class="sxs-lookup"><span data-stu-id="b33c5-381">Fixed issues with incorrect error message "You do not have the required permissions needed to perform this operation."</span></span> <span data-ttu-id="b33c5-382">bei Blockierung durch Netzwerkregeln oder bei „AuthenticationFailed“.</span><span class="sxs-lookup"><span data-stu-id="b33c5-382">when blocked by network rules or AuthenticationFailed.</span></span>

## <a name="november-4-2019"></a><span data-ttu-id="b33c5-383">4\. November 2019</span><span class="sxs-lookup"><span data-stu-id="b33c5-383">November 4, 2019</span></span>

<span data-ttu-id="b33c5-384">Version 2.0.76</span><span class="sxs-lookup"><span data-stu-id="b33c5-384">Version 2.0.76</span></span>

### <a name="acr"></a><span data-ttu-id="b33c5-385">ACR</span><span class="sxs-lookup"><span data-stu-id="b33c5-385">ACR</span></span>

* <span data-ttu-id="b33c5-386">Vorschauparameter `--pack-image-tag` wurde dem Befehl `az acr pack build` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-386">Added a preview parameter `--pack-image-tag` to command `az acr pack build`.</span></span>
* <span data-ttu-id="b33c5-387">Unterstützung der Aktivierung der Überwachung beim Erstellen einer Registrierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-387">Added support for enabling auditing on creating a registry</span></span>
* <span data-ttu-id="b33c5-388">Unterstützung von RBAC mit Repositoryumfang hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-388">Added support for Repository-scoped RBAC</span></span>

### <a name="aks"></a><span data-ttu-id="b33c5-389">AKS</span><span class="sxs-lookup"><span data-stu-id="b33c5-389">AKS</span></span>

* <span data-ttu-id="b33c5-390">`--enable-cluster-autoscaler`, `--min-count` und `--max-count` wurden dem Befehl `az aks create` hinzugefügt, sodass die automatische Clusterskalierung für den Knotenpool aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="b33c5-390">Added `--enable-cluster-autoscaler`, `--min-count` and `--max-count` to the `az aks create` command, which enables cluster autoscaler for the node pool.</span></span>
* <span data-ttu-id="b33c5-391">Die obigen Flags sowie `--update-cluster-autoscaler` und `--disable-cluster-autoscaler` wurden dem Befehl `az aks update` hinzugefügt, sodass Updates der automatischen Clusterskalierung zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="b33c5-391">Added the above flags as well as `--update-cluster-autoscaler` and `--disable-cluster-autoscaler` to the `az aks update` command, allowing updates to cluster autoscaler.</span></span>

### <a name="appconfig"></a><span data-ttu-id="b33c5-392">AppConfig</span><span class="sxs-lookup"><span data-stu-id="b33c5-392">AppConfig</span></span>

* <span data-ttu-id="b33c5-393">Befehlsgruppe der AppConfig-Funktion zum Verwalten von in einer App Configuration-Instanz gespeicherten Featureflags wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-393">Added appconfig feature command group to manage feature flags stored in an App Configuration.</span></span>
* <span data-ttu-id="b33c5-394">Geringfügiger Programmfehler für Befehl „appconfig kv export to file“ wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="b33c5-394">Fixed minor bug for appconfig kv export to file command.</span></span> <span data-ttu-id="b33c5-395">Das Lesen der Zieldateiinhalte wird während des Exports angehalten.</span><span class="sxs-lookup"><span data-stu-id="b33c5-395">Stop reading dest file contents during export.</span></span>

### <a name="appservice"></a><span data-ttu-id="b33c5-396">AppService</span><span class="sxs-lookup"><span data-stu-id="b33c5-396">AppService</span></span>

* <span data-ttu-id="b33c5-397">`az appservice plan create`: Unterstützung für das Festlegen von „persitescalung“ beim Erstellen eines App-Serviceplans wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-397">`az appservice plan create`: Added support to set 'persitescaling' on appservice plan create.</span></span>
* <span data-ttu-id="b33c5-398">Ein Problem wurde behoben, aufgrund dessen der Vorgang „webapp config ssl bind“ vorhandene Tags aus der Ressource entfernt hat.</span><span class="sxs-lookup"><span data-stu-id="b33c5-398">Fixed an issue where webapp config ssl bind operation was removing existing tags from the resource</span></span>
* <span data-ttu-id="b33c5-399">Flag `--build-remote` wurde für `az functionapp deployment source config-zip` hinzugefügt, um die Remotebuildaktion während der Funktions-App-Bereitstellung zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="b33c5-399">Added `--build-remote` flag for `az functionapp deployment source config-zip` to support remote build action during function app deployment.</span></span>
* <span data-ttu-id="b33c5-400">Die Standardknotenversion in Funktions-Apps wurde für Windows in ~ 10 geändert.</span><span class="sxs-lookup"><span data-stu-id="b33c5-400">Changed default node version on function apps to ~10 for Windows</span></span>
* <span data-ttu-id="b33c5-401">`--runtime-version`-Eigenschaft zu `az functionapp create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-401">Added `--runtime-version` property to `az functionapp create`</span></span>

### <a name="arm"></a><span data-ttu-id="b33c5-402">ARM</span><span class="sxs-lookup"><span data-stu-id="b33c5-402">ARM</span></span>

* <span data-ttu-id="b33c5-403">`az deployment/group deployment validate`: Parameter `--handle-extended-json-format` wurde hinzugefügt, um bei der Bereitstellung mehrere Zeilen und Kommentare in der JSON-Vorlage zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="b33c5-403">`az deployment/group deployment validate`: Added `--handle-extended-json-format` parameter to support multiline and comments in json template when deployment.</span></span>
* <span data-ttu-id="b33c5-404">„azure-mgmt-resource“ auf „2019-07-01“ festgelegt</span><span class="sxs-lookup"><span data-stu-id="b33c5-404">Bumped azure-mgmt-resource to 2019-07-01</span></span>

### <a name="backup"></a><span data-ttu-id="b33c5-405">Backup</span><span class="sxs-lookup"><span data-stu-id="b33c5-405">Backup</span></span>

* <span data-ttu-id="b33c5-406">Unterstützung für AzureFiles-Sicherung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-406">Added AzureFiles backup support</span></span>

### <a name="compute"></a><span data-ttu-id="b33c5-407">Compute</span><span class="sxs-lookup"><span data-stu-id="b33c5-407">Compute</span></span>

* <span data-ttu-id="b33c5-408">`az vm create`: Beim gleichzeitigen Festlegen von beschleunigtem Netzwerkbetrieb und einer vorhandenen NIC wurde eine Warnung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-408">`az vm create`: Added warning when specifying accelerated networking and an existing NIC together.</span></span>
* <span data-ttu-id="b33c5-409">`az vm create`: `--vmss` hinzugefügt, um eine vorhandene VM-Skalierungsgruppe anzugeben, welcher der virtuelle Computer zugewiesen werden soll.</span><span class="sxs-lookup"><span data-stu-id="b33c5-409">`az vm create`: Added `--vmss` to specify an existing virtual machine scale set that the virtual machine should be assigned to.</span></span>
* <span data-ttu-id="b33c5-410">`az vm/vmss create`: Eine lokale Kopie der Imagealiasdatei wurde hinzugefügt, sodass in einer eingeschränkten Netzwerkumgebung darauf zugegriffen werden kann.</span><span class="sxs-lookup"><span data-stu-id="b33c5-410">`az vm/vmss create`: Added a local copy of image alias file so that it can be accessed in a restricted network environment.</span></span>
* <span data-ttu-id="b33c5-411">`az vmss create`: `--orchestration-mode` hinzugefügt, um anzugeben, wie virtuelle Computer von der Skalierungsgruppe verwaltet werden.</span><span class="sxs-lookup"><span data-stu-id="b33c5-411">`az vmss create`: Added `--orchestration-mode` to specify how virtual machines are managed by the scale set.</span></span>
* <span data-ttu-id="b33c5-412">`az vm/vmss update`: `--ultra-ssd-enabled` hinzugefügt, um das Aktualisieren der SSD-Einstellung zuzulassen.</span><span class="sxs-lookup"><span data-stu-id="b33c5-412">`az vm/vmss update`: Added `--ultra-ssd-enabled` to allow updating ultra SSD setting.</span></span>
* <span data-ttu-id="b33c5-413">[BREAKING CHANGE] `az vm extension set`: Ein Fehler wurde behoben, aufgrund dessen Benutzer mit `--ids` keine Erweiterung auf einem virtuellen Computer festlegen konnten.</span><span class="sxs-lookup"><span data-stu-id="b33c5-413">[BREAKING CHANGE] `az vm extension set`: Fixed bug where users could not set an extension on a VM with `--ids`.</span></span>
* <span data-ttu-id="b33c5-414">Neue Befehle wurden zu `az vm image terms accept/cancel/show` hinzugefügt , um Azure Marketplace-Imagebedingungen zu verwalten.</span><span class="sxs-lookup"><span data-stu-id="b33c5-414">Added new commands `az vm image terms accept/cancel/show` to manage Azure Marketplace image terms.</span></span>
* <span data-ttu-id="b33c5-415">VMAccessForLinux auf Version 1.5 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-415">Updated VMAccessForLinux to version 1.5</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="b33c5-416">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="b33c5-416">CosmosDB</span></span>

* <span data-ttu-id="b33c5-417">[BREAKING CHANGE] `az sql container create`: `--partition-key-path` in erforderlichen Parameter geändert</span><span class="sxs-lookup"><span data-stu-id="b33c5-417">[BREAKING CHANGE] `az sql container create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="b33c5-418">[BREAKING CHANGE] `az gremlin graph create`: `--partition-key-path` in erforderlichen Parameter geändert</span><span class="sxs-lookup"><span data-stu-id="b33c5-418">[BREAKING CHANGE] `az gremlin graph create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="b33c5-419">`az sql container create`: `--unique-key-policy` und `--conflict-resolution-policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-419">`az sql container create`: Added `--unique-key-policy` and `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="b33c5-420">`az sql container create/update`: Aktualisierung des `--idx`-Standardschemas</span><span class="sxs-lookup"><span data-stu-id="b33c5-420">`az sql container create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="b33c5-421">`gremlin graph create`: `--conflict-resolution-policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-421">`gremlin graph create`: Added `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="b33c5-422">`gremlin graph create/update`: Aktualisierung des `--idx`-Standardschemas</span><span class="sxs-lookup"><span data-stu-id="b33c5-422">`gremlin graph create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="b33c5-423">Tippfehler in Hilfemeldung korrigiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-423">Fixed typo in help message</span></span>
* <span data-ttu-id="b33c5-424">Datenbank: Ablaufinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-424">database: Added deprecation infomation</span></span>
* <span data-ttu-id="b33c5-425">Auflistung: Ablaufinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-425">collection: Added deprecation infomation</span></span>

### <a name="iot"></a><span data-ttu-id="b33c5-426">IoT</span><span class="sxs-lookup"><span data-stu-id="b33c5-426">IoT</span></span>

* <span data-ttu-id="b33c5-427">Neuer Routingquelltyp hinzugefügt: DigitalTwinChangeEvents</span><span class="sxs-lookup"><span data-stu-id="b33c5-427">Added new routing source type: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="b33c5-428">Fehlende Features in `az iot hub create` behoben</span><span class="sxs-lookup"><span data-stu-id="b33c5-428">Fixed missing features in `az iot hub create`</span></span>

### <a name="key-vault"></a><span data-ttu-id="b33c5-429">Key Vault</span><span class="sxs-lookup"><span data-stu-id="b33c5-429">Key Vault</span></span>

* <span data-ttu-id="b33c5-430">Ein unerwarteter Fehler wurde behoben, bei dem keine Zertifikatdatei vorhanden war.</span><span class="sxs-lookup"><span data-stu-id="b33c5-430">Fixed an unexpected error when certificate file does not exist</span></span>
* <span data-ttu-id="b33c5-431">Funktionsunfähigkeit von `az keyvault recover/purge` behoben</span><span class="sxs-lookup"><span data-stu-id="b33c5-431">Fixed `az keyvault recover/purge` not working</span></span>

### <a name="netappfiles"></a><span data-ttu-id="b33c5-432">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="b33c5-432">NetAppFiles</span></span>

* <span data-ttu-id="b33c5-433">„azure-mgmt-netapp“ wurde auf 0.6.0 aktualisiert, um API-Version 2019-07-01 zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="b33c5-433">Upgraded azure-mgmt-netapp to 0.6.0 to use API version 2019-07-01.</span></span> <span data-ttu-id="b33c5-434">Diese neue API-Version umfasst:</span><span class="sxs-lookup"><span data-stu-id="b33c5-434">This new API version includes:</span></span>

    - <span data-ttu-id="b33c5-435">Volumeerstellung `--protocol-types` akzeptiert jetzt „NFSv4.1“ anstelle von „NFSv4“.</span><span class="sxs-lookup"><span data-stu-id="b33c5-435">Volume creation `--protocol-types` accepts now "NFSv4.1" not "NFSv4"</span></span>
    - <span data-ttu-id="b33c5-436">Die Richtlinie der Volumeexportrichtlinie heißt jetzt „nfsv41“ anstelle von „nfsv4“.</span><span class="sxs-lookup"><span data-stu-id="b33c5-436">Volume export policy property now named 'nfsv41' not 'nfsv4'</span></span>
    - <span data-ttu-id="b33c5-437">Volume `--creation-token` wurde in `--file-path` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-437">Volume `--creation-token` renamed to `--file-path`</span></span>
    - <span data-ttu-id="b33c5-438">Das Erstellungsdatum einer Momentaufnahme heißt jetzt einfach „erstellt“.</span><span class="sxs-lookup"><span data-stu-id="b33c5-438">Snapshot creation date now named just 'created'</span></span>

### <a name="network"></a><span data-ttu-id="b33c5-439">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="b33c5-439">Network</span></span>

* <span data-ttu-id="b33c5-440">`az network private-dns link vnet create/update`: Unterstützung für mandantenübergreifende Verknüpfung virtueller Netzwerke.</span><span class="sxs-lookup"><span data-stu-id="b33c5-440">`az network private-dns link vnet create/update`: Support cross-tenant virtual network linking.</span></span>
* <span data-ttu-id="b33c5-441">[BREAKING CHANGE] `az network vnet subnet list`: `--resource-group` und `--vnet-name` wurden geändert und sind jetzt erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b33c5-441">[BREAKING CHANGE] `az network vnet subnet list`: Changed `--resource-group` and `--vnet-name` to be required now.</span></span>
* <span data-ttu-id="b33c5-442">`az network public-ip prefix create`: Unterstützung der Angabe der IP-Adressversion (IPv4, IPv6) bei der Erstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-442">`az network public-ip prefix create`: Added support to specify IP address version (IPv4, IPv6) when creation</span></span>
* <span data-ttu-id="b33c5-443">„azure-mgmt-network“ auf 7.0.0 und „api-version“ auf 2019-09-01 festgelegt</span><span class="sxs-lookup"><span data-stu-id="b33c5-443">Bumped azure-mgmt-network to 7.0.0 and api-version to 2019-09-01</span></span>
* <span data-ttu-id="b33c5-444">`az network vrouter`: Unterstützung für neuen virtuellen Dienstrouter und virtuelles Routerpeering hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-444">`az network vrouter`: Added support for new service virtual router and virtual router peering</span></span>
* <span data-ttu-id="b33c5-445">`az network express-route gateway connection`: Unterstützung für `--internet-security` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-445">`az network express-route gateway connection`: Added support for `--internet-security`</span></span>

### <a name="profile"></a><span data-ttu-id="b33c5-446">Profil</span><span class="sxs-lookup"><span data-stu-id="b33c5-446">Profile</span></span>

* <span data-ttu-id="b33c5-447">Funktionsunfähigkeit von `az account get-access-token --resource-type ms-graph` behoben</span><span class="sxs-lookup"><span data-stu-id="b33c5-447">Fixed `az account get-access-token --resource-type ms-graph` not working</span></span>
* <span data-ttu-id="b33c5-448">Warnung aus `az login` entfernt</span><span class="sxs-lookup"><span data-stu-id="b33c5-448">Removed warning from `az login`</span></span>

### <a name="rbac"></a><span data-ttu-id="b33c5-449">RBAC</span><span class="sxs-lookup"><span data-stu-id="b33c5-449">RBAC</span></span>

* <span data-ttu-id="b33c5-450">Funktionsunfähigkeit von `az ad app update --id {} --display-name {}` behoben</span><span class="sxs-lookup"><span data-stu-id="b33c5-450">Fixed `az ad app update --id {} --display-name {}` doesn't work</span></span>

### <a name="servicefabric"></a><span data-ttu-id="b33c5-451">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="b33c5-451">ServiceFabric</span></span>

* <span data-ttu-id="b33c5-452">`az sf cluster create`: Ein Problem wurde behoben, indem die Compute-VMSS von „template.json“ für Service Fabric unter Linux und Windows von Standarddatenträgern auf verwaltete Datenträger umgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="b33c5-452">`az sf cluster create`: Fixed an issue by modifying service fabric linux and windows template.json compute vmss from standard to managed disks</span></span>

### <a name="sql"></a><span data-ttu-id="b33c5-453">SQL</span><span class="sxs-lookup"><span data-stu-id="b33c5-453">SQL</span></span>

* <span data-ttu-id="b33c5-454">Die Parameter `--compute-model`, `--auto-pause-delay` und `--min-capacity` wurden hinzugefügt, um CRUD-Vorgänge für das neue SQL-Datenbank-Angebot zu unterstützen: Serverloses Computemodell.</span><span class="sxs-lookup"><span data-stu-id="b33c5-454">Added `--compute-model`, `--auto-pause-delay`, and `--min-capacity` parameters to support CRUD operations for new SQL Database offering: Serverless compute model.</span></span>

### <a name="storage"></a><span data-ttu-id="b33c5-455">Storage</span><span class="sxs-lookup"><span data-stu-id="b33c5-455">Storage</span></span>

* <span data-ttu-id="b33c5-456">`az storage account create/update`: Parameter „--enable-files-adds“ und Azure Active Directory-Eigenschaftenargumentgruppe hinzugefügt, um Active Directory Domain-Dienstauthentifizierung für Azure Files zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="b33c5-456">`az storage account create/update`: Added --enable-files-adds parameter and Azure Active Directory Properties Argument group to support Azure Files Active Directory Domain Service Authentication</span></span>
* <span data-ttu-id="b33c5-457">`az storage account keys list/renew` wurde erweitert, um die Auflistung oder erneute Generierung von Kerberos-Schlüsseln des Speicherkontos zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="b33c5-457">Expanded `az storage account keys list/renew` to support listing or regenerating Kerberos keys of storage account.</span></span>

## <a name="october-15-2019"></a><span data-ttu-id="b33c5-458">15. Oktober 2019</span><span class="sxs-lookup"><span data-stu-id="b33c5-458">October 15, 2019</span></span>

<span data-ttu-id="b33c5-459">Version 2.0.75</span><span class="sxs-lookup"><span data-stu-id="b33c5-459">Version 2.0.75</span></span>

### <a name="aks"></a><span data-ttu-id="b33c5-460">AKS</span><span class="sxs-lookup"><span data-stu-id="b33c5-460">AKS</span></span>

* <span data-ttu-id="b33c5-461">Standardwert `--load-balancer-sku` in `standard` geändert, sofern von der Kubernetes-Version unterstützt</span><span class="sxs-lookup"><span data-stu-id="b33c5-461">Changed `--load-balancer-sku` default value to `standard` if supported by the kubernetes version</span></span>
* <span data-ttu-id="b33c5-462">Standardwert `--vm-set-type` in `virtualmachinescalesets` geändert, sofern von der Kubernetes-Version unterstützt</span><span class="sxs-lookup"><span data-stu-id="b33c5-462">Changed `--vm-set-type` default value to `virtualmachinescalesets` if supported by the kubernetes version</span></span>

### <a name="ams"></a><span data-ttu-id="b33c5-463">AMS</span><span class="sxs-lookup"><span data-stu-id="b33c5-463">AMS</span></span>

* <span data-ttu-id="b33c5-464">[BREAKING CHANGE] Name von `job start` in `job create` geändert</span><span class="sxs-lookup"><span data-stu-id="b33c5-464">[BREAKING CHANGE] Changed the name of `job start` to `job create`</span></span>
* <span data-ttu-id="b33c5-465">[BREAKING CHANGE] Parameter `--ask` von `content-key-policy create` geändert, sodass eine hexadezimale Zeichenfolge mit 32 Zeichen anstelle von UTF8 verwendet wird</span><span class="sxs-lookup"><span data-stu-id="b33c5-465">[BREAKING CHANGE] Changed the `--ask` parameter of `content-key-policy create` to use a 32-character hex string instead of UTF8</span></span>

### <a name="appservice"></a><span data-ttu-id="b33c5-466">AppService</span><span class="sxs-lookup"><span data-stu-id="b33c5-466">AppService</span></span>

* <span data-ttu-id="b33c5-467">Befehle vom Typ `webapp config access-restriction show|set|add|remove` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-467">Added commands `webapp config access-restriction show|set|add|remove`</span></span>
* <span data-ttu-id="b33c5-468">Bessere Fehlerbehandlung zu `webapp up` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-468">Added better error handling to `webapp up`</span></span>
* <span data-ttu-id="b33c5-469">Unterstützung für SKU `Isolated` zu `appservice plan update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-469">Added support for `Isolated` SKU to `appservice plan update`</span></span>

### <a name="arm"></a><span data-ttu-id="b33c5-470">ARM</span><span class="sxs-lookup"><span data-stu-id="b33c5-470">ARM</span></span>

* <span data-ttu-id="b33c5-471">Parameter `--handle-extended-json-format` zu `deployment create` hinzugefügt, um mehrere Zeilen und Kommentare in der JSON-Vorlage zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="b33c5-471">Added `--handle-extended-json-format` parameter `deployment create` to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="b33c5-472">Compute</span><span class="sxs-lookup"><span data-stu-id="b33c5-472">Compute</span></span>

* <span data-ttu-id="b33c5-473">Parameter `--enable-agent` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-473">Added `--enable-agent` parameter to `vm create`</span></span>
* <span data-ttu-id="b33c5-474">`vm create` geändert, um bei der Verwendung von Zonen die SKU „Standard“ für die öffentliche IP-Adresse zu verwenden</span><span class="sxs-lookup"><span data-stu-id="b33c5-474">Changed `vm create` to use standard public IP SKU automatically when using zones</span></span>
* <span data-ttu-id="b33c5-475">`vm create` geändert, um automatisch einen gültigen Computernamen für eine VM zu erstellen, falls keiner angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="b33c5-475">Changed `vm create` to automatically create a valid computer name for a VM if none is provided</span></span>
* <span data-ttu-id="b33c5-476">Parameter `--computer-name-prefix` zu `vmss create` hinzugefügt, um das benutzerdefinierte Computernamenspräfix virtueller Computer in VMSS zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="b33c5-476">Added `--computer-name-prefix` parameter to `vmss create` to support custom computer name prefix of virtual machines in the VMSS</span></span>
* <span data-ttu-id="b33c5-477">Parameter `--workspace` zu `vm create` hinzugefügt, um automatisch einen Log Analytics-Arbeitsbereich zu aktivieren</span><span class="sxs-lookup"><span data-stu-id="b33c5-477">Add `--workspace` parameter to `vm create` to enable log analytics workspace automatically</span></span>
* <span data-ttu-id="b33c5-478">API-Version für Kataloge auf 2019-07-01 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-478">Updated galleries API version to 2019-07-01</span></span>

### <a name="core"></a><span data-ttu-id="b33c5-479">Core</span><span class="sxs-lookup"><span data-stu-id="b33c5-479">Core</span></span>

* <span data-ttu-id="b33c5-480">Syntaxprüfung für Parameter `--set` im generischen Updatebefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-480">Added syntax check for `--set` parameter in generic update command</span></span>

### <a name="iot"></a><span data-ttu-id="b33c5-481">IoT</span><span class="sxs-lookup"><span data-stu-id="b33c5-481">IoT</span></span>

* <span data-ttu-id="b33c5-482">Problem behoben, bei dem für `iot hub show` der Fehler „Ressource nicht gefunden.“ zurückgegeben wurde</span><span class="sxs-lookup"><span data-stu-id="b33c5-482">Fixed an issue where `iot hub show` would incorrectly error with "resource not found"</span></span>

### <a name="monitor"></a><span data-ttu-id="b33c5-483">Überwachen</span><span class="sxs-lookup"><span data-stu-id="b33c5-483">Monitor</span></span>

* <span data-ttu-id="b33c5-484">Unterstützung für CRUD zu `monitor log-analytics workspace` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-484">Added support for CRUD to `monitor log-analytics workspace`</span></span>

### <a name="network"></a><span data-ttu-id="b33c5-485">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="b33c5-485">Network</span></span>

* <span data-ttu-id="b33c5-486">Unterstützung für mandantenübergreifende virtuelle Verbindung zu `network private-dns link vnet [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-486">Added support for cross-tenant virtual linking to `network private-dns link vnet [create|update]`</span></span>
* <span data-ttu-id="b33c5-487">[BREAKING CHANGE]`network vnet subnet list` geändert, um Parameter `--resource-group` und `--vnet-name` vorauszusetzen</span><span class="sxs-lookup"><span data-stu-id="b33c5-487">[BREAKING CHANGE] Changed `network vnet subnet list` to require `--resource-group` and `--vnet-name` parameters</span></span>

### <a name="sql"></a><span data-ttu-id="b33c5-488">SQL</span><span class="sxs-lookup"><span data-stu-id="b33c5-488">SQL</span></span>

* <span data-ttu-id="b33c5-489">Befehle zu `sql mi ad-admin` hinzugefügt, die das Festlegen eines AAD-Administrators für verwaltete Instanzen unterstützen</span><span class="sxs-lookup"><span data-stu-id="b33c5-489">Added commands to `sql mi ad-admin` that support setting an AAD administrator on managed instances</span></span>

### <a name="storage"></a><span data-ttu-id="b33c5-490">Storage</span><span class="sxs-lookup"><span data-stu-id="b33c5-490">Storage</span></span>

* <span data-ttu-id="b33c5-491">Parameter `--preserve-s2s-access-tier` zu `storage copy` hinzugefügt, um die Zugriffsebene beim Kopieren von Dienst zu Dienst beizubehalten</span><span class="sxs-lookup"><span data-stu-id="b33c5-491">Added `--preserve-s2s-access-tier` parameter `storage copy` to preserve access tier during service to service copy</span></span>
* <span data-ttu-id="b33c5-492">Parameter `--enable-large-file-share` zu `storage account [create|update]` hinzugefügt, um große Dateifreigaben für ein Speicherkonto zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="b33c5-492">Added `--enable-large-file-share` parameter to `storage account [create|update]` to support large file shares for storage account</span></span>

## <a name="september-24-2019"></a><span data-ttu-id="b33c5-493">24. September 2019</span><span class="sxs-lookup"><span data-stu-id="b33c5-493">September 24, 2019</span></span>

<span data-ttu-id="b33c5-494">Version 2.0.74</span><span class="sxs-lookup"><span data-stu-id="b33c5-494">Version 2.0.74</span></span>

### <a name="acr"></a><span data-ttu-id="b33c5-495">ACR</span><span class="sxs-lookup"><span data-stu-id="b33c5-495">ACR</span></span>

* <span data-ttu-id="b33c5-496">Erforderlicher Parameter `--type` zu `acr config retention update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-496">Added a required `--type` parameter to `acr config retention update`</span></span>
* <span data-ttu-id="b33c5-497">[BREAKING CHANGE] Umbenannter Parameter `--name -n` in `--registry -r ` für Befehlsgruppe `acr config` geändert</span><span class="sxs-lookup"><span data-stu-id="b33c5-497">[BREAKING CHNAGE] Renamed parameter `--name -n` changed to `--registry -r ` for `acr config` command group</span></span>

### <a name="aks"></a><span data-ttu-id="b33c5-498">AKS</span><span class="sxs-lookup"><span data-stu-id="b33c5-498">AKS</span></span>

* <span data-ttu-id="b33c5-499">Parameter `--load-balancer-sku` zum Befehl `aks create` hinzugefügt, um die Erstellung von AKS-Clustern mit SLB zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="b33c5-499">Added `--load-balancer-sku` parameter to `aks create` command, which allows for creating AKS cluster with SLB</span></span>
* <span data-ttu-id="b33c5-500">Parameter `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` und `--load-balancer-outbound-ip-prefixes` zu den Befehlen `aks [create|update]` hinzugefügt,um die Aktualisierung des Lastenausgleichsprofils eines AKS-Clusters mit SLB zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="b33c5-500">Added `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` and `--load-balancer-outbound-ip-prefixes` parameters to `aks [create|update]` commands, which allow for updating load balancer profile of an AKS cluster with SLB</span></span>
* <span data-ttu-id="b33c5-501">Parameter `--vm-set-type` zum Befehl `aks create` hinzugefügt, um die Angabe von VM-Typen eines AKS-Clusters (vmas oder vmss) zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="b33c5-501">Added `--vm-set-type` parameter to `aks create` command, which allows to specify vm types of an AKS Cluster (vmas or vmss)</span></span>

### <a name="arm"></a><span data-ttu-id="b33c5-502">ARM</span><span class="sxs-lookup"><span data-stu-id="b33c5-502">ARM</span></span>

* <span data-ttu-id="b33c5-503">Parameter `--handle-extended-json-format` zum Befehl `group deployment create` hinzugefügt, um mehrere Zeilen und Kommentare in der JSON-Vorlage zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="b33c5-503">Added `--handle-extended-json-format` parameter to `group deployment create` command to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="b33c5-504">Compute</span><span class="sxs-lookup"><span data-stu-id="b33c5-504">Compute</span></span>

* <span data-ttu-id="b33c5-505">Parameter `--terminate-notification-time` zu den Befehlen `vmss [create|update]` hinzugefügt, um die Konfigurierbarkeit der Beendigung geplanter Ereignisse zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="b33c5-505">Added `--terminate-notification-time` parameter to `vmss [create|update]` commands to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="b33c5-506">Parameter `--enable-terminate-notification` zu den Befehlen `vmss update` hinzugefügt, um die Konfigurierbarkeit der Beendigung geplanter Ereignisse zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="b33c5-506">Added `--enable-terminate-notification` parameter to `vmss update` command to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="b33c5-507">Parameter `--priority,` `--eviction-policy,` `--max-billing` zu `[vm|vmss] create`-Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-507">Added `--priority,` `--eviction-policy,` `--max-billing` parameters to `[vm|vmss] create` commands</span></span>
* <span data-ttu-id="b33c5-508">`disk create` geändert, um die Angabe der genauen Größe des Datenträgeruploads zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="b33c5-508">Changed `disk create` to allow specifying the exact size of the disk upload</span></span>
* <span data-ttu-id="b33c5-509">Unterstützung für inkrementelle Momentaufnahmen für verwaltete Datenträger zu `snapshot create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-509">Added support for incremental snapshots for managed disks to `snapshot create`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="b33c5-510">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="b33c5-510">Cosmos DB</span></span>

* <span data-ttu-id="b33c5-511">Parameter `--type <key-type>` zum Befehl `cosmosdb keys list` hinzugefügt, um Schlüssel, schreibgeschützte Schlüssel oder Verbindungszeichenfolgen anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="b33c5-511">Added `--type <key-type>` parameter to `cosmosdb keys list` command to show key, read only keys or connection strings</span></span>
* <span data-ttu-id="b33c5-512">Befehl `cosmosdb keys regenerate` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-512">Added `cosmosdb keys regenerate` command</span></span>
* <span data-ttu-id="b33c5-513">[VERALTET] Befehle `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` und `cosmosdb list-read-only-keys` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-513">[DEPRECATED] Deprecated `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` and `cosmosdb list-read-only-keys` commands</span></span>

### <a name="eventgrid"></a><span data-ttu-id="b33c5-514">EventGrid</span><span class="sxs-lookup"><span data-stu-id="b33c5-514">EventGrid</span></span>

* <span data-ttu-id="b33c5-515">Endpunkthilfetext korrigiert, um auf den richtigen Parameter zu verweisen</span><span class="sxs-lookup"><span data-stu-id="b33c5-515">Fixed the endpoint help text to refer to the right parameter</span></span>

### <a name="key-vault"></a><span data-ttu-id="b33c5-516">Key Vault</span><span class="sxs-lookup"><span data-stu-id="b33c5-516">Key Vault</span></span>

* <span data-ttu-id="b33c5-517">Problem behoben, aufgrund dessen die Anmeldung mit einem Mandanten (`login -t`) unter Umständen zu einem Fehler von `keyvault create` führte</span><span class="sxs-lookup"><span data-stu-id="b33c5-517">Fixed issue where logging in with a tenant (`login -t`) could cause `keyvault create` to fail</span></span>

### <a name="monitor"></a><span data-ttu-id="b33c5-518">Überwachen</span><span class="sxs-lookup"><span data-stu-id="b33c5-518">Monitor</span></span>

* <span data-ttu-id="b33c5-519">Problem behoben, aufgrund dessen das Zeichen `:` in `--condition` für `monitor metrics alert create` nicht zulässig war</span><span class="sxs-lookup"><span data-stu-id="b33c5-519">Fixed issue where `:` character was not allowed in `--condition` argument to `monitor metrics alert create`</span></span>

### <a name="policy"></a><span data-ttu-id="b33c5-520">Richtlinie</span><span class="sxs-lookup"><span data-stu-id="b33c5-520">Policy</span></span>

* <span data-ttu-id="b33c5-521">Unterstützung für Policy-API-Version 2019-06-01 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-521">Added support for Policy API version 2019-06-01</span></span>
* <span data-ttu-id="b33c5-522">Parameter `--enforcement-mode` zum Befehl `policy assignment create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-522">Added `--enforcement-mode` parameter to `policy assignment create` command</span></span>

### <a name="storage"></a><span data-ttu-id="b33c5-523">Storage</span><span class="sxs-lookup"><span data-stu-id="b33c5-523">Storage</span></span>

* <span data-ttu-id="b33c5-524">Parameter `--blob-type` zum Befehl `az storage copy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-524">Added `--blob-type` parameter to `az storage copy` command</span></span>

## <a name="september-10-2019"></a><span data-ttu-id="b33c5-525">10. September 2019</span><span class="sxs-lookup"><span data-stu-id="b33c5-525">September 10, 2019</span></span>

### <a name="acr"></a><span data-ttu-id="b33c5-526">ACR</span><span class="sxs-lookup"><span data-stu-id="b33c5-526">ACR</span></span>

* <span data-ttu-id="b33c5-527">Befehlsgruppe `acr config retention` zum Konfigurieren der Aufbewahrungsrichtlinie hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-527">Added command group `acr config retention` to configure retention policy</span></span>

### <a name="aks"></a><span data-ttu-id="b33c5-528">AKS</span><span class="sxs-lookup"><span data-stu-id="b33c5-528">AKS</span></span>

* <span data-ttu-id="b33c5-529">Unterstützung für die ACR-Integration mit den folgenden Befehlen hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="b33c5-529">Added support for ACR integration with the following commands:</span></span>
  * <span data-ttu-id="b33c5-530">Parameter `--attach-acr` zu `aks [create|update]` hinzugefügt, um einen ACR an einen AKS-Cluster anzufügen</span><span class="sxs-lookup"><span data-stu-id="b33c5-530">Added `--attach-acr` parameter to `aks [create|update]` to attach an ACR to an AKS cluster</span></span>
  * <span data-ttu-id="b33c5-531">Parameter `--detach-acr` zu `aks update` hinzugefügt, um den ACR von einem AKS-Cluster zu trennen</span><span class="sxs-lookup"><span data-stu-id="b33c5-531">Added `--detach-acr` parameter to `aks update` to detach the ACR from an AKS cluster</span></span>

### <a name="arm"></a><span data-ttu-id="b33c5-532">ARM</span><span class="sxs-lookup"><span data-stu-id="b33c5-532">ARM</span></span>

* <span data-ttu-id="b33c5-533">Zur Verwendung der API-Version 2019-05-10 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-533">Updated to use API version 2019-05-10</span></span>

### <a name="batch"></a><span data-ttu-id="b33c5-534">Batch</span><span class="sxs-lookup"><span data-stu-id="b33c5-534">Batch</span></span>

* <span data-ttu-id="b33c5-535">Neue JSON-Konfigurationseinstellungen für `batch pool create` zu `--json-file` hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="b33c5-535">Added new JSON configuration settings to `--json-file` for `batch pool create`:</span></span>
  * <span data-ttu-id="b33c5-536">`MountConfigurations` für Dateisystemeinbindungen hinzugefügt (Details siehe https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body )</span><span class="sxs-lookup"><span data-stu-id="b33c5-536">Added `MountConfigurations` for file system mounts (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
  * <span data-ttu-id="b33c5-537">Optionale Eigenschaft `publicIPs` in `NetworkConfiguration` für öffentliche IP-Adressen für Pools hinzugefügt (Details siehe https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body )</span><span class="sxs-lookup"><span data-stu-id="b33c5-537">Added optional property `publicIPs` on `NetworkConfiguration` for public IPs on pools (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
* <span data-ttu-id="b33c5-538">Unterstützung für Kataloge mit freigegebenen Images zu `--image` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-538">Added support for shared image galleries to `--image`</span></span>
* <span data-ttu-id="b33c5-539">[BREAKING CHANGE] Standardwert von `--start-task-wait-for-success` für `batch pool create` in `true` geändert</span><span class="sxs-lookup"><span data-stu-id="b33c5-539">[BREAKING CHANGE] Changed default value of `--start-task-wait-for-success` on `batch pool create` to be `true`</span></span>
* <span data-ttu-id="b33c5-540">[BREAKING CHANGE] Standardwert von `Scope` für `AutoUserSpecification` geändert, damit immer „Pool“ verwendet wird (vormals `Task` für Windows-Knoten bzw. `Pool` für Linux-Knoten)</span><span class="sxs-lookup"><span data-stu-id="b33c5-540">[BREAKING CHANGE] Changed default value for `Scope` on `AutoUserSpecification` to always be Pool (was `Task` on Windows nodes, `Pool` on Linux nodes)</span></span>
  * <span data-ttu-id="b33c5-541">Dieses Argument kann nur über eine JSON-Konfiguration mit `--json-file` festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="b33c5-541">This argument can only be set from a JSON configuration with `--json-file`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="b33c5-542">HDInsight</span><span class="sxs-lookup"><span data-stu-id="b33c5-542">HDInsight</span></span>

* <span data-ttu-id="b33c5-543">Allgemein verfügbares Release</span><span class="sxs-lookup"><span data-stu-id="b33c5-543">GA release</span></span>
* <span data-ttu-id="b33c5-544">[BREAKING CHANGE] Parameter `--workernode-count/-c` von `az hdinsight resize` in erforderlich geändert</span><span class="sxs-lookup"><span data-stu-id="b33c5-544">[BREAKING CHANGE] Changed parameter `--workernode-count/-c` of `az hdinsight resize` to be required.</span></span>

### <a name="key-vault"></a><span data-ttu-id="b33c5-545">Key Vault</span><span class="sxs-lookup"><span data-stu-id="b33c5-545">Key Vault</span></span>

* <span data-ttu-id="b33c5-546">Problem behoben, aufgrund dessen Subnetze nicht aus Netzwerkregeln gelöscht werden konnten</span><span class="sxs-lookup"><span data-stu-id="b33c5-546">Fixed issue where subnets couldn't be deleted from network rules</span></span>
* <span data-ttu-id="b33c5-547">Problem behoben, aufgrund dessen doppelte Subnetze und IP-Adressen zu Netzwerkregeln hinzugefügt werden konnten</span><span class="sxs-lookup"><span data-stu-id="b33c5-547">Fixed issue where duplicated subnets and IP addresses could be added to network rules</span></span>

### <a name="network"></a><span data-ttu-id="b33c5-548">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="b33c5-548">Network</span></span>

* <span data-ttu-id="b33c5-549">Parameter `--interval` zu `network watcher flow-log` hinzugefügt, um den Wert für das Intervall der Datenverkehrsanalyse festzulegen</span><span class="sxs-lookup"><span data-stu-id="b33c5-549">Added `--interval` parameter to `network watcher flow-log` to set traffic analysis interval value</span></span>
* <span data-ttu-id="b33c5-550">`network application-gateway identity` zum Verwalten der Gatewayidentität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-550">Added `network application-gateway identity` to manage gateway identity</span></span>
* <span data-ttu-id="b33c5-551">Unterstützung zum Festlegen der Key Vault-ID zu `network application-gateway ssl-cert` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-551">Added support for setting Key Vault ID to `network application-gateway ssl-cert`</span></span>
* <span data-ttu-id="b33c5-552">`network express-route peering peer-connection [show|list]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-552">Added `network express-route peering peer-connection [show|list]`</span></span>

### <a name="policy"></a><span data-ttu-id="b33c5-553">Richtlinie</span><span class="sxs-lookup"><span data-stu-id="b33c5-553">Policy</span></span>

* <span data-ttu-id="b33c5-554">Zur Verwendung der API-Version 2019-01-01 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-554">Updated to use API version 2019-01-01</span></span>

## <a name="august-27-2019"></a><span data-ttu-id="b33c5-555">27. August 2019</span><span class="sxs-lookup"><span data-stu-id="b33c5-555">August 27, 2019</span></span>

<span data-ttu-id="b33c5-556">Version 2.0.72</span><span class="sxs-lookup"><span data-stu-id="b33c5-556">Version 2.0.72</span></span>

### <a name="acr"></a><span data-ttu-id="b33c5-557">ACR</span><span class="sxs-lookup"><span data-stu-id="b33c5-557">ACR</span></span>

* <span data-ttu-id="b33c5-558">[BREAKING CHANGE] Unterstützung für SKU `classic` entfernt</span><span class="sxs-lookup"><span data-stu-id="b33c5-558">[BREAKING CHANGE] Removed support for the `classic` SKU</span></span>

### <a name="api-management"></a><span data-ttu-id="b33c5-559">API Management</span><span class="sxs-lookup"><span data-stu-id="b33c5-559">API Management</span></span>

* <span data-ttu-id="b33c5-560">[VORSCHAU] Befehlsgruppe `apim` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-560">[PREVIEW] Added `apim` command group</span></span>

### <a name="appservice"></a><span data-ttu-id="b33c5-561">AppService</span><span class="sxs-lookup"><span data-stu-id="b33c5-561">AppService</span></span>

* <span data-ttu-id="b33c5-562">Problem mit dem Befehl `webapp webjob continuous start` bei Angabe eines Slots behoben</span><span class="sxs-lookup"><span data-stu-id="b33c5-562">Fixed issue with `webapp webjob continuous start` command when specifying a slot</span></span>
* <span data-ttu-id="b33c5-563">`webapp up` geändert, um den Ordner `env` zu erkennen und aus der für die Bereitstellung verwendeten Datei zu entfernen</span><span class="sxs-lookup"><span data-stu-id="b33c5-563">Changed `webapp up` to detect `env` folder and remove it from the file used for deployment</span></span>

### <a name="keyvault"></a><span data-ttu-id="b33c5-564">KeyVault</span><span class="sxs-lookup"><span data-stu-id="b33c5-564">Keyvault</span></span>

* <span data-ttu-id="b33c5-565">Fehler in `keyvault secret set` behoben, aufgrund dessen das Argument `--expires` ignoriert wurde</span><span class="sxs-lookup"><span data-stu-id="b33c5-565">Fixed a bug in `keyvault secret set` that igored the `--expires` argument</span></span>

### <a name="network"></a><span data-ttu-id="b33c5-566">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="b33c5-566">Network</span></span>

* <span data-ttu-id="b33c5-567">Unterstützung für IPv6-Adressen zu Argumenten vom Typ `--private-ip-address-version` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-567">Added support for IPv6 addresses to `--private-ip-address-version` arguments</span></span>
* <span data-ttu-id="b33c5-568">Neue Befehle vom Typ `network private-endpoint [create|update|list-types]` für die Verwaltung privater Endpunkte hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-568">Added new commands `network private-endpoint [create|update|list-types]` for private endpoint management</span></span>
* <span data-ttu-id="b33c5-569">Befehlsgruppe `network private-link-service` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-569">Added command group `network private-link-service`</span></span>
* <span data-ttu-id="b33c5-570">Argumente `--private-endpoint-network-policies` und `--private-link-service-network-policies` zu `network vnet subnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-570">Added `--private-endpoint-network-policies` and `--private-link-service-network-policies` arguments to `network vnet subnet update`</span></span>

### <a name="rbac"></a><span data-ttu-id="b33c5-571">RBAC</span><span class="sxs-lookup"><span data-stu-id="b33c5-571">RBAC</span></span>

* <span data-ttu-id="b33c5-572">Problem mit `ad app update --homepage` behoben, aufgrund dessen die Startseite nicht aktualisiert wurde</span><span class="sxs-lookup"><span data-stu-id="b33c5-572">Fixed issue with `ad app update --homepage` where homepage would not be updated</span></span>

### <a name="servicefabric"></a><span data-ttu-id="b33c5-573">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="b33c5-573">ServiceFabric</span></span>

* <span data-ttu-id="b33c5-574">Unterstützung für Key Vault-Namen mit Groß- und Kleinschreibung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-574">Added support for mixed-case Key Vault names</span></span>
* <span data-ttu-id="b33c5-575">Problem bei der Verwendung von Zertifikaten in Key Vault behoben</span><span class="sxs-lookup"><span data-stu-id="b33c5-575">Fixed issue when using certificates in Key Vault</span></span>
* <span data-ttu-id="b33c5-576">Problem bei der Verwendung von PFX-Zertifikatdateien behoben</span><span class="sxs-lookup"><span data-stu-id="b33c5-576">Fixed issue with using PFX certificate files</span></span>
* <span data-ttu-id="b33c5-577">Problem mit `sf cluster certificate add` behoben, wenn keine Key Vault-Ressourcengruppe angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="b33c5-577">Fixed issue with `sf cluster certificate add` when Key Vault resource group wasn't specified</span></span>
* <span data-ttu-id="b33c5-578">Problem behoben, aufgrund dessen `sf cluster set` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="b33c5-578">Fixed issue with `sf cluster set` not working</span></span>

### <a name="signalr"></a><span data-ttu-id="b33c5-579">SignalR</span><span class="sxs-lookup"><span data-stu-id="b33c5-579">SignalR</span></span>

* <span data-ttu-id="b33c5-580">Neue Befehle hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="b33c5-580">Added new commands:</span></span>
  * <span data-ttu-id="b33c5-581">`signalr cors`: Verwalten von CORS für SignalR</span><span class="sxs-lookup"><span data-stu-id="b33c5-581">`signalr cors`: Manage SignalR CORS</span></span>
  * <span data-ttu-id="b33c5-582">`signalr restart`: Starten eines SignalR-Diensts</span><span class="sxs-lookup"><span data-stu-id="b33c5-582">`signalr restart`: Restart a SignalR service</span></span>
  * <span data-ttu-id="b33c5-583">`signalr update`: Aktualisieren eines SignalR-Diensts</span><span class="sxs-lookup"><span data-stu-id="b33c5-583">`signalr update`: Update a SignalR service</span></span>
* <span data-ttu-id="b33c5-584">Argument `--service-mode` zu `signalr create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-584">Added `--service-mode` argument to `signalr create`</span></span>

### <a name="storage"></a><span data-ttu-id="b33c5-585">Storage</span><span class="sxs-lookup"><span data-stu-id="b33c5-585">Storage</span></span>

* <span data-ttu-id="b33c5-586">Befehl `storage account revoke-delegation-keys` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-586">Added `storage account revoke-delegation-keys` command</span></span>

## <a name="august-13-2019"></a><span data-ttu-id="b33c5-587">13. August 2019</span><span class="sxs-lookup"><span data-stu-id="b33c5-587">August 13, 2019</span></span>

<span data-ttu-id="b33c5-588">Version 2.0.71</span><span class="sxs-lookup"><span data-stu-id="b33c5-588">Version 2.0.71</span></span>

### <a name="appservice"></a><span data-ttu-id="b33c5-589">AppService</span><span class="sxs-lookup"><span data-stu-id="b33c5-589">AppService</span></span>

* <span data-ttu-id="b33c5-590">Problem behoben, aufgrund dessen bei Befehlen vom Typ `webapp webjob continuous` für Slots Fehler auftraten</span><span class="sxs-lookup"><span data-stu-id="b33c5-590">Fixed issue where `webapp webjob continuous` commands were failing for slots</span></span>

### <a name="botservice"></a><span data-ttu-id="b33c5-591">BotService</span><span class="sxs-lookup"><span data-stu-id="b33c5-591">BotService</span></span>

* <span data-ttu-id="b33c5-592">[BREAKING CHANGE] Unterstützung für die Erstellung von Bots der Version 3 entfernt</span><span class="sxs-lookup"><span data-stu-id="b33c5-592">[BREAKING CHANGE] Removed support for creating v3 SDK bots</span></span>

### <a name="cognitiveservices"></a><span data-ttu-id="b33c5-593">CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="b33c5-593">CognitiveServices</span></span>

* <span data-ttu-id="b33c5-594">Befehle vom Typ `cognitiveservices account network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-594">Added `cognitiveservices account network-rule` commands</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="b33c5-595">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="b33c5-595">Cosmos DB</span></span>

* <span data-ttu-id="b33c5-596">Beim Aktualisieren mehrerer Schreibstandorte wurde eine Warnung entfernt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-596">Removed warning when updating multiple write locations</span></span>
* <span data-ttu-id="b33c5-597">CRUD-Befehle für CosmosDB SQL-, MongoDB-, Cassandra-, Gremlin- und Tabellenressourcen sowie den Ressourcendurchsatz hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-597">Added CRUD commands for CosmosDB SQL, MongoDB, Cassandra, Gremlin and Table resources and resource's throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="b33c5-598">HDInsight</span><span class="sxs-lookup"><span data-stu-id="b33c5-598">HDInsight</span></span>

<span data-ttu-id="b33c5-599">Dieses Release enthält zahlreiche wichtige Änderungen.</span><span class="sxs-lookup"><span data-stu-id="b33c5-599">This release contains a large number of breaking changes.</span></span>

* <span data-ttu-id="b33c5-600">[BREAKING CHANGE] Parameter für `hdinsight create` umbenannt:</span><span class="sxs-lookup"><span data-stu-id="b33c5-600">[BREAKING CHANGE] Renamed parameters for `hdinsight create`:</span></span>
  * <span data-ttu-id="b33c5-601">`--storage-default-container` in `--storage-container` umbenannt</span><span class="sxs-lookup"><span data-stu-id="b33c5-601">Renamed `--storage-default-container` to `--storage-container`</span></span>
  * <span data-ttu-id="b33c5-602">`--storage-default-filesystem` in `--storage-filesystem` umbenannt</span><span class="sxs-lookup"><span data-stu-id="b33c5-602">Renamed `--storage-default-filesystem` to `--storage-filesystem`</span></span>
* <span data-ttu-id="b33c5-603">[BREAKING CHANGE] Das Argument `--name` von `application create` wurde so geändert, dass es den Anwendungsnamen anstelle des Clusternamens darstellt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-603">[BREAKING CHANGE] Changed the `--name` argument of `application create` to represent the application name instead of the cluster name</span></span>
* <span data-ttu-id="b33c5-604">Argument `--cluster-name` zu `application create` hinzugefügt, um die alte Funktion `--name` zu ersetzen</span><span class="sxs-lookup"><span data-stu-id="b33c5-604">Added `--cluster-name` argument to `application create` to replace old `--name` functionality</span></span>
* <span data-ttu-id="b33c5-605">[BREAKING CHANGE] Parameter für `application create` umbenannt:</span><span class="sxs-lookup"><span data-stu-id="b33c5-605">[BREAKING CHANGE] Renamed parameters for `application create`:</span></span>
  * <span data-ttu-id="b33c5-606">`--application-type` in `--type` umbenannt</span><span class="sxs-lookup"><span data-stu-id="b33c5-606">Renamed `--application-type` to `--type`</span></span>
  * <span data-ttu-id="b33c5-607">`--marketplace-identifier` in `--marketplace-id` umbenannt</span><span class="sxs-lookup"><span data-stu-id="b33c5-607">Renamed `--marketplace-identifier` to `--marketplace-id`</span></span>
  * <span data-ttu-id="b33c5-608">`--https-endpoint-access-mode` in `--access-mode` umbenannt</span><span class="sxs-lookup"><span data-stu-id="b33c5-608">Renamed `--https-endpoint-access-mode` to `--access-mode`</span></span>
  * <span data-ttu-id="b33c5-609">`--https-endpoint-destination-port` in `--destination-port` umbenannt</span><span class="sxs-lookup"><span data-stu-id="b33c5-609">Renamed  `--https-endpoint-destination-port` to `--destination-port`</span></span>
* <span data-ttu-id="b33c5-610">[BREAKING CHANGE] Parameter für `application create` entfernt:</span><span class="sxs-lookup"><span data-stu-id="b33c5-610">[BREAKING CHANGE] Removed parameters for `application create`:</span></span>
  * `--https-endpoint-location`
  * `--https-endpoint-public-port`
  * `--ssh-endpoint-destination-port`
  * `--ssh-endpoint-location`
  * `--ssh-endpoint-public-port`
* <span data-ttu-id="b33c5-611">[WICHTIGE ÄNDERUNG] `--target-instance-count` für `hdinsight resize` in `--workernode-count` umbenannt</span><span class="sxs-lookup"><span data-stu-id="b33c5-611">[BREAKING CHNAGE] Renamed `--target-instance-count` to `--workernode-count` for `hdinsight resize`</span></span>
* <span data-ttu-id="b33c5-612">[BREAKING CHANGE] Alle Befehle in der Gruppe `hdinsight script-action` wurden so geändert, dass sie den Parameter `--name` als Namen der Skriptaktion verwenden.</span><span class="sxs-lookup"><span data-stu-id="b33c5-612">[BREAKING CHANGE] Changed all commands in the `hdinsight script-action` group to use the `--name` parameter as the name of the script action.</span></span>
* <span data-ttu-id="b33c5-613">Argument `--cluster-name` zu allen Befehlen vom Typ `hdinsight script-action` hinzugefügt, um die alte Funktion `--name` zu ersetzen</span><span class="sxs-lookup"><span data-stu-id="b33c5-613">Added `--cluster-name` argument to all `hdinsight script-action` commands to replace old `--name` functionality</span></span>
* <span data-ttu-id="b33c5-614">[BREAKING CHANGE]`--script-execution-id` für alle Befehle vom Typ `hdinsight script-action` in `--execution-id` umbenannt</span><span class="sxs-lookup"><span data-stu-id="b33c5-614">[BREAKING CHANGE] Renamed `--script-execution-id` to `--execution-id` for all `hdinsight script-action` commands</span></span>
* <span data-ttu-id="b33c5-615">[BREAKING CHANGE]`hdinsight script-action show` in `hdinsight script-action show-execution-details` umbenannt</span><span class="sxs-lookup"><span data-stu-id="b33c5-615">[BREAKING CHANGE] Renamed `hdinsight script-action show` to `hdinsight script-action show-execution-details`</span></span>
* <span data-ttu-id="b33c5-616">[WICHTIGE ÄNDERUNG] Parameter in `hdinsight script-action execute --roles` geändert, sodass sie durch Leerzeichen anstelle von Kommas getrennt sind</span><span class="sxs-lookup"><span data-stu-id="b33c5-616">[BREAKING CHNAGE] Changed parameters to `hdinsight script-action execute --roles` to be space-separated instead of comma-separated</span></span>
* <span data-ttu-id="b33c5-617">[BREAKING CHANGE] Parameter `--persisted` für `hdinsight script-action list` entfernt</span><span class="sxs-lookup"><span data-stu-id="b33c5-617">[BREAKING CHANGE] Removed the `--persisted` parameter of `hdinsight script-action list`</span></span>
* <span data-ttu-id="b33c5-618">Der Parameter `hdinsight create --cluster-configurations` wurde so geändert, dass er einen Pfad zu einer lokalen JSON-Datei oder JSON-Zeichenfolge akzeptiert.</span><span class="sxs-lookup"><span data-stu-id="b33c5-618">Changed the `hdinsight create --cluster-configurations` parameter to accept a path to a local JSON file or a JSON string</span></span>
* <span data-ttu-id="b33c5-619">Befehl `hdinsight script-action list-execution-history` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-619">Added command `hdinsight script-action list-execution-history`</span></span>
* <span data-ttu-id="b33c5-620">`hdinsight monitor enable --workspace` geändert, um die ID oder den Namen eines Log Analytics-Arbeitsbereichs zu akzeptieren</span><span class="sxs-lookup"><span data-stu-id="b33c5-620">Changed `hdinsight monitor enable --workspace` to accept a Log Analytics workspace ID or workspace name</span></span>
* <span data-ttu-id="b33c5-621">Argument `hdinsight monitor enable --primary-key` hinzugefügt. Dieses Argument wird benötigt, wenn eine Arbeitsbereichs-ID als Parameter angegeben wird.</span><span class="sxs-lookup"><span data-stu-id="b33c5-621">Added the `hdinsight monitor enable --primary-key` argument, which is needed if a workspace ID is provided as the parameter</span></span>
* <span data-ttu-id="b33c5-622">Weitere Beispiele und aktualisierte Beschreibungen für Hilfemeldungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-622">Added more examples and updated descriptions for help messages</span></span>

### <a name="interactive"></a><span data-ttu-id="b33c5-623">Interactive</span><span class="sxs-lookup"><span data-stu-id="b33c5-623">Interactive</span></span>

* <span data-ttu-id="b33c5-624">Ladefehler behoben</span><span class="sxs-lookup"><span data-stu-id="b33c5-624">Fixed a loading error</span></span>

### <a name="kubernetes"></a><span data-ttu-id="b33c5-625">Kubernetes</span><span class="sxs-lookup"><span data-stu-id="b33c5-625">Kubernetes</span></span>

* <span data-ttu-id="b33c5-626">Änderung, um `https` zu verwenden, wenn der Dashboardcontainerport `https` verwendet</span><span class="sxs-lookup"><span data-stu-id="b33c5-626">Changed to use `https` if dashboard container port is using `https`</span></span>

### <a name="network"></a><span data-ttu-id="b33c5-627">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="b33c5-627">Network</span></span>

* <span data-ttu-id="b33c5-628">Argument `--yes` hinzugefügt zu `network dns record-set cname delete`</span><span class="sxs-lookup"><span data-stu-id="b33c5-628">Added `--yes` argument `network dns record-set cname delete`</span></span>

### <a name="profile"></a><span data-ttu-id="b33c5-629">Profil</span><span class="sxs-lookup"><span data-stu-id="b33c5-629">Profile</span></span>

* <span data-ttu-id="b33c5-630">Argument `--resource-type` zu `account get-access-token` zum Abrufen von Ressourcenzugriffstoken hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-630">Added `--resource-type` argument to `account get-access-token` to get resource access tokens</span></span>

### <a name="servicefabric"></a><span data-ttu-id="b33c5-631">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="b33c5-631">ServiceFabric</span></span>

* <span data-ttu-id="b33c5-632">Alle unterstützten Betriebssystemversionen für „sf cluster create“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-632">Added all supported os version for sf cluster create</span></span>
* <span data-ttu-id="b33c5-633">Fehler beim Überprüfen des primären Zertifikats behoben</span><span class="sxs-lookup"><span data-stu-id="b33c5-633">Fixed primary certificate validation bug</span></span>

### <a name="storage"></a><span data-ttu-id="b33c5-634">Storage</span><span class="sxs-lookup"><span data-stu-id="b33c5-634">Storage</span></span>

* <span data-ttu-id="b33c5-635">Befehl `storage copy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-635">Added command `storage copy`</span></span>

## <a name="july-30-2019"></a><span data-ttu-id="b33c5-636">30. Juli 2019</span><span class="sxs-lookup"><span data-stu-id="b33c5-636">July 30, 2019</span></span>

<span data-ttu-id="b33c5-637">Version 2.0.70</span><span class="sxs-lookup"><span data-stu-id="b33c5-637">Version 2.0.70</span></span>

### <a name="acr"></a><span data-ttu-id="b33c5-638">ACR</span><span class="sxs-lookup"><span data-stu-id="b33c5-638">ACR</span></span>

* <span data-ttu-id="b33c5-639">Problem #9952 behoben (Regression im Befehl `acr pack build`)</span><span class="sxs-lookup"><span data-stu-id="b33c5-639">Fixed issue #9952 (a regression in the `acr pack build` command)</span></span>
* <span data-ttu-id="b33c5-640">Standardname des Generatorimages in `acr pack build` entfernt</span><span class="sxs-lookup"><span data-stu-id="b33c5-640">Removed the default builder image name in `acr pack build`</span></span>

### <a name="appservice"></a><span data-ttu-id="b33c5-641">AppService</span><span class="sxs-lookup"><span data-stu-id="b33c5-641">Appservice</span></span>

* <span data-ttu-id="b33c5-642">`webapp config ssl` geändert, um eine Meldung anzuzeigen, wenn eine Ressource nicht gefunden wurde</span><span class="sxs-lookup"><span data-stu-id="b33c5-642">Changed `webapp config ssl` to show a message if a resource is not found</span></span>
* <span data-ttu-id="b33c5-643">Problem behoben, aufgrund dessen `functionapp create` den Speicherkontotypen `Standard_RAGRS` nicht akzeptiert hat</span><span class="sxs-lookup"><span data-stu-id="b33c5-643">Fixed issue where `functionapp create` does not accept `Standard_RAGRS` storage account type</span></span>
* <span data-ttu-id="b33c5-644">Problem behoben, aufgrund dessen für `webapp up` ein Fehler auftrat, wenn für die Ausführung ältere Python-Versionen verwendet wurden</span><span class="sxs-lookup"><span data-stu-id="b33c5-644">Fixed an issue where `webapp up` would fail if run using older versions of python</span></span>

### <a name="network"></a><span data-ttu-id="b33c5-645">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="b33c5-645">Network</span></span>

* <span data-ttu-id="b33c5-646">Ungültiger Parameter `--ids` aus `network nic ip-config add` entfernt (Fehlerbehebungen #9861)</span><span class="sxs-lookup"><span data-stu-id="b33c5-646">Removed invalid parameter `--ids` from `network nic ip-config add` (fixes #9861)</span></span>
* <span data-ttu-id="b33c5-647">Fehlerbehebungen #9604.</span><span class="sxs-lookup"><span data-stu-id="b33c5-647">Fixes #9604.</span></span> <span data-ttu-id="b33c5-648">Parameter `--root-certs` zu `network application-gateway http-settings [create|update]` hinzugefügt, um vom Benutzer zugewiesene vertrauenswürdige Stammzertifikate zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="b33c5-648">Added `--root-certs` parameter to `network application-gateway http-settings [create|update]` to support user associate trusted root certificates.</span></span>
* <span data-ttu-id="b33c5-649">Argument `--subscription` für `network dns record-set ns create` korrigiert (#9965)</span><span class="sxs-lookup"><span data-stu-id="b33c5-649">Fixed arguent `--subscription` for `network dns record-set ns create` (#9965)</span></span>

### <a name="rbac"></a><span data-ttu-id="b33c5-650">RBAC</span><span class="sxs-lookup"><span data-stu-id="b33c5-650">RBAC</span></span>

* <span data-ttu-id="b33c5-651">Befehl `user update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-651">Added `user update` command</span></span>
* <span data-ttu-id="b33c5-652">[VERALTET]`--upn-or-object-id` in benutzerbezogenen Befehlen als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-652">[DEPRECATED] Deprecated `--upn-or-object-id` from user-related commands</span></span>
    * <span data-ttu-id="b33c5-653">Verwenden Sie das Ersatzargument `--id`.</span><span class="sxs-lookup"><span data-stu-id="b33c5-653">Use replacement argument `--id`</span></span>
* <span data-ttu-id="b33c5-654">Argument `--id` zu benutzerbezogenen Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-654">Added `--id` argument to user-related commands</span></span>

### <a name="sql"></a><span data-ttu-id="b33c5-655">SQL</span><span class="sxs-lookup"><span data-stu-id="b33c5-655">SQL</span></span>

* <span data-ttu-id="b33c5-656">Verwaltungsbefehle für Schlüssel verwalteter Instanzen und TDE-Schutzvorrichtung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-656">Added management commands for managed instance keys and TDE protector</span></span>

### <a name="storage"></a><span data-ttu-id="b33c5-657">Storage</span><span class="sxs-lookup"><span data-stu-id="b33c5-657">Storage</span></span>

* <span data-ttu-id="b33c5-658">Befehl `storage remove` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-658">Added `storage remove` command</span></span>
* <span data-ttu-id="b33c5-659">Problem mit `storage blob update` behoben</span><span class="sxs-lookup"><span data-stu-id="b33c5-659">Fixed an issue with `storage blob update`</span></span>

### <a name="vm"></a><span data-ttu-id="b33c5-660">VM</span><span class="sxs-lookup"><span data-stu-id="b33c5-660">VM</span></span>

* <span data-ttu-id="b33c5-661">`list-skus` wurde geändert, um eine neuere API-Version für die Ausgabe von Zonendetails zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="b33c5-661">Changed `list-skus` to use newer api-version to output zone details</span></span>
* <span data-ttu-id="b33c5-662">Standardwert `--single-placement-group` für `vmss create` in `false` geändert</span><span class="sxs-lookup"><span data-stu-id="b33c5-662">Changed default of `--single-placement-group` to `false` for `vmss create`</span></span>
* <span data-ttu-id="b33c5-663">Möglichkeit zum Auswählen von ZRS-Speicher-SKUs für `[snapshot|disk] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-663">Added ability to select ZRS storage SKUs for `[snapshot|disk] create`</span></span>
* <span data-ttu-id="b33c5-664">Neue Befehlsgruppe `vm host` zur Unterstützung dedizierter Hosts hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-664">Added new command group `vm host` to support dedicated hosts</span></span>
* <span data-ttu-id="b33c5-665">Parameter `--host` und `--host-group` für `vm create` hinzugefügt, um den dedizierten VM-Host festzulegen</span><span class="sxs-lookup"><span data-stu-id="b33c5-665">Added parameters `--host` and `--host-group` on `vm create` to set VM dedicated host</span></span>

## <a name="july-16-2019"></a><span data-ttu-id="b33c5-666">16. Juli 2019</span><span class="sxs-lookup"><span data-stu-id="b33c5-666">July 16, 2019</span></span>

<span data-ttu-id="b33c5-667">Version 2.0.69</span><span class="sxs-lookup"><span data-stu-id="b33c5-667">Version 2.0.69</span></span>

### <a name="appservice"></a><span data-ttu-id="b33c5-668">AppService</span><span class="sxs-lookup"><span data-stu-id="b33c5-668">Appservice</span></span>

* <span data-ttu-id="b33c5-669">`webapp identity`-Befehle geändert, um eine korrekte Fehlermeldung zurückzugeben, wenn „ResourceGroupName“ oder der App-Name ungültig sind</span><span class="sxs-lookup"><span data-stu-id="b33c5-669">Changed `webapp identity` commands to return a proper error message if ResourceGroupName or App name are invalid</span></span>
* <span data-ttu-id="b33c5-670">`webapp list` korrigiert, sodass der korrekte Wert für „numberOfSites“ zurückgegeben wird, wenn „ResourceGroup“ nicht angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="b33c5-670">Fixed `webapp list` to return the correct value for numberOfSites if no ResourceGroup was provided</span></span>
* <span data-ttu-id="b33c5-671">Nebeneffekte von `appservice plan create` und `webapp create` behoben</span><span class="sxs-lookup"><span data-stu-id="b33c5-671">Fixed side-effects of `appservice plan create` and `webapp create`</span></span>

### <a name="core"></a><span data-ttu-id="b33c5-672">Core</span><span class="sxs-lookup"><span data-stu-id="b33c5-672">Core</span></span>

* <span data-ttu-id="b33c5-673">Problem behoben, aufgrund dessen `--subscription` angezeigt wurde, obwohl nicht anwendbar</span><span class="sxs-lookup"><span data-stu-id="b33c5-673">Fixed issue where `--subscription` would appear despite being not applicable</span></span>

### <a name="batch"></a><span data-ttu-id="b33c5-674">Batch</span><span class="sxs-lookup"><span data-stu-id="b33c5-674">Batch</span></span>

* <span data-ttu-id="b33c5-675">[BREAKING CHANGE]`batch pool node-agent-skus list` durch `batch pool supported-images list` ersetzt</span><span class="sxs-lookup"><span data-stu-id="b33c5-675">[BREAKING CHANGE] Replaced `batch pool node-agent-skus list` with `batch pool supported-images list`</span></span>
* <span data-ttu-id="b33c5-676">Unterstützung für Sicherheitsregeln hinzugefügt, die den Netzwerkzugriff auf einen Pool basierend auf dem Quellport des Datenverkehrs blockieren, wenn die Option `--json-file` von `batch pool create network` verwendet wird</span><span class="sxs-lookup"><span data-stu-id="b33c5-676">Added support for security rules blocking network access to a pool based on the source port of the traffic when using the `--json-file` option of `batch pool create network`</span></span>
* <span data-ttu-id="b33c5-677">Unterstützung für die Ausführung der Aufgabe im Arbeitsverzeichnis des Containers oder der Batch-Aufgabe hinzugefügt, wenn die Option `--json-file` von `batch task create` verwendet wird</span><span class="sxs-lookup"><span data-stu-id="b33c5-677">Added support for executing the task in the container working directory or in the Batch task working directory when using the `--json-file` option of `batch task create`</span></span>
* <span data-ttu-id="b33c5-678">Fehler in Option `--application-package-references` von `batch pool create` behoben, aufgrund dessen nur Standardeinstellungen möglich waren</span><span class="sxs-lookup"><span data-stu-id="b33c5-678">Fixed error in `--application-package-references` option of `batch pool create` where it would only work with defaults</span></span>

### <a name="eventhubs"></a><span data-ttu-id="b33c5-679">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="b33c5-679">Eventhubs</span></span>

* <span data-ttu-id="b33c5-680">Validierung für Parameter `--rights` von `authorizationrule`-Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-680">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="rdbms"></a><span data-ttu-id="b33c5-681">RDBMS</span><span class="sxs-lookup"><span data-stu-id="b33c5-681">RDBMS</span></span>

* <span data-ttu-id="b33c5-682">Optionaler Parameter zum Angeben der Replikat-SKU für den Befehl zum Erstellen von Replikaten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-682">Added optional parameter to specify replica SKU for create replica command</span></span>
* <span data-ttu-id="b33c5-683">Problem mit CI-Testfehler bei der Erstellung von MySQL-Replikaten behoben</span><span class="sxs-lookup"><span data-stu-id="b33c5-683">Fixed the issue with CI test failure with creating MySQL replica</span></span>

### <a name="relay"></a><span data-ttu-id="b33c5-684">Relay</span><span class="sxs-lookup"><span data-stu-id="b33c5-684">Relay</span></span>

* <span data-ttu-id="b33c5-685">Problem mit Hybridverbindung behoben, wenn die Client-Autorisierung deaktiviert ist [#8775](https://github.com/azure/azure-cli/issues/8775)</span><span class="sxs-lookup"><span data-stu-id="b33c5-685">Fixed issue with hybrid connection when client authroization disabled [#8775](https://github.com/azure/azure-cli/issues/8775)</span></span>
* <span data-ttu-id="b33c5-686">Parameter `--requires-transport-security` zu `relay wcfrelay create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-686">Added parameter `--requires-transport-security` to `relay wcfrelay create`</span></span>

### <a name="servicebus"></a><span data-ttu-id="b33c5-687">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="b33c5-687">Servicebus</span></span>

* <span data-ttu-id="b33c5-688">Validierung für Parameter `--rights` von `authorizationrule`-Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-688">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="storage"></a><span data-ttu-id="b33c5-689">Storage</span><span class="sxs-lookup"><span data-stu-id="b33c5-689">Storage</span></span>

* <span data-ttu-id="b33c5-690">AADDS für Files für Speicherkontoaktualisierung aktiviert</span><span class="sxs-lookup"><span data-stu-id="b33c5-690">Enable Files AADDS for storage account update</span></span>
* <span data-ttu-id="b33c5-691">Problem `storage blob service-properties update --set` behoben</span><span class="sxs-lookup"><span data-stu-id="b33c5-691">Fixed issue `storage blob service-properties update --set`</span></span>

## <a name="july-2-2019"></a><span data-ttu-id="b33c5-692">2\. Juli 2019</span><span class="sxs-lookup"><span data-stu-id="b33c5-692">July 2, 2019</span></span>

<span data-ttu-id="b33c5-693">Version 2.0.68</span><span class="sxs-lookup"><span data-stu-id="b33c5-693">Version 2.0.68</span></span>

### <a name="core"></a><span data-ttu-id="b33c5-694">Core</span><span class="sxs-lookup"><span data-stu-id="b33c5-694">Core</span></span>

* <span data-ttu-id="b33c5-695">Befehlsmodule sind jetzt in einer einzelnen verteilbaren Python-Komponente zusammengefasst.</span><span class="sxs-lookup"><span data-stu-id="b33c5-695">Command modules are now consolidated into a single Python distributable.</span></span> <span data-ttu-id="b33c5-696">Die direkte Verwendung zahlreicher Pakete vom Typ `azure-cli-` in PyPI ist daher veraltet.</span><span class="sxs-lookup"><span data-stu-id="b33c5-696">This deprecates direct use of many `azure-cli-` packages on PyPI.</span></span>
  <span data-ttu-id="b33c5-697">Dadurch sollte sich die Installationsgröße reduzieren. Darüber hinaus sollte es nur Benutzer betreffen, die eine direkte Installation über `pip` ausgeführt haben.</span><span class="sxs-lookup"><span data-stu-id="b33c5-697">This should reduce install size and only affect users who have directly installed via `pip`.</span></span>

### <a name="acr"></a><span data-ttu-id="b33c5-698">ACR</span><span class="sxs-lookup"><span data-stu-id="b33c5-698">ACR</span></span>

* <span data-ttu-id="b33c5-699">Unterstützung für Trigger mit Timer zu Aufgabe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-699">Added support for Timer Triggers to Task</span></span>

### <a name="appservice"></a><span data-ttu-id="b33c5-700">AppService</span><span class="sxs-lookup"><span data-stu-id="b33c5-700">Appservice</span></span>

* <span data-ttu-id="b33c5-701">`functionapp create` wurde so geändert, das Application Insights standardmäßig aktiviert wird.</span><span class="sxs-lookup"><span data-stu-id="b33c5-701">Changed `functionapp create` to enable application insights by default</span></span>
* <span data-ttu-id="b33c5-702">[BREAKING CHANGE] Veralteter Befehl `functionapp devops-build` entfernt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-702">[BREAKING CHANGE] Removed deprecated `functionapp devops-build` command.</span></span>
  *  <span data-ttu-id="b33c5-703">Verwenden Sie stattdessen den neuen Befehl `az functionapp devops-pipeline`.</span><span class="sxs-lookup"><span data-stu-id="b33c5-703">Use the new command `az functionapp devops-pipeline` instead</span></span>
* <span data-ttu-id="b33c5-704">Unterstützung des Funktions-App-Plans für Linux-Verbrauch zu `functionapp deployment config-zip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-704">Added Linux Consumption function app plan support to `functionapp deployment config-zip`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="b33c5-705">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="b33c5-705">Cosmos DB</span></span>

* <span data-ttu-id="b33c5-706">Unterstützung für das Deaktivieren von TTL hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-706">Added support for disabling TTL</span></span>

### <a name="dls"></a><span data-ttu-id="b33c5-707">DLS</span><span class="sxs-lookup"><span data-stu-id="b33c5-707">DLS</span></span>

* <span data-ttu-id="b33c5-708">Aktualisierte ADLS-Version (0.0.45)</span><span class="sxs-lookup"><span data-stu-id="b33c5-708">Updated ADLS version (0.0.45)</span></span>

### <a name="feedback"></a><span data-ttu-id="b33c5-709">Feedback</span><span class="sxs-lookup"><span data-stu-id="b33c5-709">Feedback</span></span>

* <span data-ttu-id="b33c5-710">Wird ein fehlgeschlagener Erweiterungsbefehl gemeldet, versucht `az feedback` nun, über den Index die Projekt-/Repository-URL der Erweiterung im Browser zu öffnen.</span><span class="sxs-lookup"><span data-stu-id="b33c5-710">When reporting a failed extension command, `az feedback` now attempts to open the browser to the project/repo url of the extension from the index</span></span>

### <a name="hdinsight"></a><span data-ttu-id="b33c5-711">HDInsight</span><span class="sxs-lookup"><span data-stu-id="b33c5-711">HDInsight</span></span>

* <span data-ttu-id="b33c5-712">[BREAKING CHANGE] Der Befehlsgruppenname `oms` wurde in `monitor` geändert.</span><span class="sxs-lookup"><span data-stu-id="b33c5-712">[BREAKING CHANGE] Changed `oms` command group name to `monitor`</span></span>
* <span data-ttu-id="b33c5-713">[BREAKING CHANGE]`--http-password/-p` als erforderlicher Parameter festgelegt</span><span class="sxs-lookup"><span data-stu-id="b33c5-713">[BREAKING CHANGE] Made `--http-password/-p` a required parameter</span></span> 
* <span data-ttu-id="b33c5-714">Vervollständigungen für `--cluster-admin-account` und `cluster-users-group-dns` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-714">Added completers for `--cluster-admin-account` and `cluster-users-group-dns` parameters completer</span></span> 
* <span data-ttu-id="b33c5-715">Parameter `cluster-users-group-dns` so geändert, dass er erforderlich ist, wenn `—esp` vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="b33c5-715">Changed `cluster-users-group-dns` parameter to be required when `—esp` is present</span></span>
* <span data-ttu-id="b33c5-716">Timeout für alle vorhandenen automatischen Argumentvervollständigungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-716">Added a timeout for all existing argument auto-completers</span></span>
* <span data-ttu-id="b33c5-717">Timeout für das Transformieren des Ressourcennamens in eine Ressourcen-ID hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-717">Added a timeout for transforming resource name to resource id</span></span>
* <span data-ttu-id="b33c5-718">Die automatischen Vervollständigungen wurden so geändert, dass Ressourcen aus einer beliebigen Ressourcengruppe ausgewählt werden.</span><span class="sxs-lookup"><span data-stu-id="b33c5-718">Changed Auto-completers to select resources from any resource group.</span></span> <span data-ttu-id="b33c5-719">Dabei kann es sich um eine andere Ressourcengruppe als die mit `-g` angegebene Gruppe handeln.</span><span class="sxs-lookup"><span data-stu-id="b33c5-719">It can be a different resource group than the one specified with `-g`</span></span>
* <span data-ttu-id="b33c5-720">Unterstützung für die Parameter `--sub-domain-suffix` und `--disable_gateway_auth` im Befehl `hdinsight application create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-720">Added support for `--sub-domain-suffix` and `--disable_gateway_auth` parameters in the `hdinsight application create` command</span></span>

### <a name="managed-services"></a><span data-ttu-id="b33c5-721">Verwaltete Dienste</span><span class="sxs-lookup"><span data-stu-id="b33c5-721">Managed Services</span></span>

* <span data-ttu-id="b33c5-722">Befehlsmodul für verwaltete Dienste als Vorschau eingeführt</span><span class="sxs-lookup"><span data-stu-id="b33c5-722">Introducing managed service command module in preview</span></span>

### <a name="profile"></a><span data-ttu-id="b33c5-723">Profil</span><span class="sxs-lookup"><span data-stu-id="b33c5-723">Profile</span></span>
* <span data-ttu-id="b33c5-724">Argument `--subscription` für Abmeldebefehl unterdrückt</span><span class="sxs-lookup"><span data-stu-id="b33c5-724">Suppress `--subscription` argument for logout command</span></span>

### <a name="rbac"></a><span data-ttu-id="b33c5-725">RBAC</span><span class="sxs-lookup"><span data-stu-id="b33c5-725">RBAC</span></span>

* <span data-ttu-id="b33c5-726">[BREAKING CHANGE] Argument `--password` für `create-for-rbac` entfernt</span><span class="sxs-lookup"><span data-stu-id="b33c5-726">[BREAKING CHANGE] Removed `--password` argument for `create-for-rbac`</span></span>
* <span data-ttu-id="b33c5-727">Parameter `--assignee-principal-type` zum Befehl `create` hinzugefügt, um zeitweilige Fehler zu vermeiden, die durch die Replikationswartezeit des AAD-Graph-Servers verursacht werden</span><span class="sxs-lookup"><span data-stu-id="b33c5-727">Added `--assignee-principal-type` parameter to `create` command to avoid intermittent failures caused by AAD graph server replication latency</span></span>
* <span data-ttu-id="b33c5-728">Absturz in `ad signed-in-user` beim Auflisten von in Besitz befindlichen Objekten behoben</span><span class="sxs-lookup"><span data-stu-id="b33c5-728">Fixed a crash in `ad signed-in-user` when listing owned objects</span></span>
* <span data-ttu-id="b33c5-729">Problem behoben, aufgrund dessen `ad sp` nicht die richtige Anwendung über einen Dienstprinzipal fand</span><span class="sxs-lookup"><span data-stu-id="b33c5-729">Fixed issue where `ad sp` would not find the right application from a service principal</span></span>

### <a name="rdbms"></a><span data-ttu-id="b33c5-730">RDBMS</span><span class="sxs-lookup"><span data-stu-id="b33c5-730">RDBMS</span></span>

* <span data-ttu-id="b33c5-731">Unterstützung für die Replikation für MariaDB hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-731">Added support for replication for MariaDB</span></span>

### <a name="sql"></a><span data-ttu-id="b33c5-732">SQL</span><span class="sxs-lookup"><span data-stu-id="b33c5-732">SQL</span></span>

* <span data-ttu-id="b33c5-733">Zulässige Werte für `sql db create --sample-name` dokumentiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-733">Documented allowed values for `sql db create --sample-name`</span></span>

### <a name="storage"></a><span data-ttu-id="b33c5-734">Storage</span><span class="sxs-lookup"><span data-stu-id="b33c5-734">Storage</span></span>

* <span data-ttu-id="b33c5-735">Unterstützung von SAS-Token für die Benutzerdelegierung mit `--as-user` zu `storage blob generate-sas` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-735">Added user delegation SAS token support with `--as-user` to `storage blob generate-sas`</span></span> 
* <span data-ttu-id="b33c5-736">Unterstützung von SAS-Token für die Benutzerdelegierung mit `--as-user` zu `storage container generate-sas` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-736">Added user delegation SAS token support with `--as-user` to `storage container generate-sas`</span></span> 

### <a name="vm"></a><span data-ttu-id="b33c5-737">VM</span><span class="sxs-lookup"><span data-stu-id="b33c5-737">VM</span></span>

* <span data-ttu-id="b33c5-738">Fehler behoben, aufgrund dessen `vmss create` bei der Ausführung mit `--no-wait` eine Fehlermeldung zurückgab</span><span class="sxs-lookup"><span data-stu-id="b33c5-738">Fixed bug where `vmss create` returns an error message when run with `--no-wait`</span></span>
* <span data-ttu-id="b33c5-739">Die clientseitige Validierung für `vmss create --single-placement-group` wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-739">Removed client-side validation for `vmss create --single-placement-group`.</span></span> <span data-ttu-id="b33c5-740">Es tritt kein Fehler auf, wenn `--single-placement-group` auf `true` und für `--instance-count` ein größerer Wert als 100 festgelegt wird oder wenn Verfügbarkeitszonen angegeben werden. Diese Validierung wird jedoch dem Computedienst überlassen.</span><span class="sxs-lookup"><span data-stu-id="b33c5-740">Does not fail if `--single-placement-group` is set to `true` and`--instance-count` is greater than 100 or availability zones are specified, but leaves this validation to the compute service</span></span>
* <span data-ttu-id="b33c5-741">Problem behoben, aufgrund dessen bei der Verwendung von `--latest` für `[vm|vmss] extension image list` ein Fehler auftrat</span><span class="sxs-lookup"><span data-stu-id="b33c5-741">Fixed bug where `[vm|vmss] extension image list` fails when used with `--latest`</span></span>


## <a name="june-18-2019"></a><span data-ttu-id="b33c5-742">18. Juni 2019</span><span class="sxs-lookup"><span data-stu-id="b33c5-742">June 18, 2019</span></span>

<span data-ttu-id="b33c5-743">Version 2.0.67</span><span class="sxs-lookup"><span data-stu-id="b33c5-743">Version 2.0.67</span></span>

### <a name="core"></a><span data-ttu-id="b33c5-744">Core</span><span class="sxs-lookup"><span data-stu-id="b33c5-744">Core</span></span>

<span data-ttu-id="b33c5-745">In diesem Release wird das neue [Preview]-Tag eingeführt, um Kunden gegenüber deutlich zu machen, dass sich eine Befehlsgruppe, ein Befehl oder ein Argument in der Vorschauphase befindet.</span><span class="sxs-lookup"><span data-stu-id="b33c5-745">This release introduces a new [Preview] tag to more clearly communicate to customers when a command group, command or argument is in preview status.</span></span> <span data-ttu-id="b33c5-746">Diese Information war zuvor im Hilfetext oder implizit durch die Versionsnummer des Befehlsmoduls angegeben.</span><span class="sxs-lookup"><span data-stu-id="b33c5-746">This was previously called out in help text or communicated implicitly by the command module version number.</span></span>
<span data-ttu-id="b33c5-747">Die Befehlszeilenschnittstelle wird künftig Versionsnummern für einzelne Pakete entfernen.</span><span class="sxs-lookup"><span data-stu-id="b33c5-747">The CLI will be removing version numbers for individual packages in the future.</span></span> <span data-ttu-id="b33c5-748">Wenn sich ein Befehl in der Vorschauphase befindet, gilt dies auch für alle seine Argumente.</span><span class="sxs-lookup"><span data-stu-id="b33c5-748">If a command is in preview, all of its arguments are as well.</span></span> <span data-ttu-id="b33c5-749">Wenn eine Befehlsgruppe als Vorschau gekennzeichnet ist, befinden sich auch alle Befehle und Argumente in der Vorschauphase.</span><span class="sxs-lookup"><span data-stu-id="b33c5-749">If a command group is labeled as being in preview, then all commands and arguments are considered to be in preview as well.</span></span>

<span data-ttu-id="b33c5-750">Infolge dieser Änderung befinden sich in diesem Release verschiedene Befehlsgruppen anscheinend „plötzlich“ in der Vorschauphase.</span><span class="sxs-lookup"><span data-stu-id="b33c5-750">As a result of this change, several command groups may seem to "suddenly" appear to be in a preview status with this release.</span></span> <span data-ttu-id="b33c5-751">Tatsächlich ist es jedoch so, dass sich die meisten Pakete in der Vorschauphase befanden, in diesem Release jedoch als allgemein verfügbar gelten.</span><span class="sxs-lookup"><span data-stu-id="b33c5-751">What actually happened is that most packages were in a preview status, but are being deemed GA with this release</span></span>

### <a name="acr"></a><span data-ttu-id="b33c5-752">ACR</span><span class="sxs-lookup"><span data-stu-id="b33c5-752">ACR</span></span>
* <span data-ttu-id="b33c5-753">Befehl „acr check-health“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-753">Added 'acr check-health' command</span></span>
* <span data-ttu-id="b33c5-754">Verbesserte Fehlerbehandlung für AAD-Token und für das Abrufen externer Befehle</span><span class="sxs-lookup"><span data-stu-id="b33c5-754">Improved error handling for AAD tokens and for retrieving external commands</span></span>

### <a name="acs"></a><span data-ttu-id="b33c5-755">ACS</span><span class="sxs-lookup"><span data-stu-id="b33c5-755">ACS</span></span>
* <span data-ttu-id="b33c5-756">Veraltete ACS-Befehle werden jetzt in der Hilfeansicht ausgeblendet.</span><span class="sxs-lookup"><span data-stu-id="b33c5-756">Deprecated ACS commands are now hidden from help view</span></span>

### <a name="ams"></a><span data-ttu-id="b33c5-757">AMS</span><span class="sxs-lookup"><span data-stu-id="b33c5-757">AMS</span></span>
* <span data-ttu-id="b33c5-758">[BREAKING CHANGE] Änderung, damit ISO 8601-Zeitzeichenfolgen für „archive-window-length“ und „key-frame-interval-duration“ zurückgegeben werden</span><span class="sxs-lookup"><span data-stu-id="b33c5-758">[BREAKING CHANGE] Changed to return ISO 8601 time strings for archive-window-length and key-frame-interval-duration</span></span>

### <a name="appservice"></a><span data-ttu-id="b33c5-759">AppService</span><span class="sxs-lookup"><span data-stu-id="b33c5-759">AppService</span></span>
* <span data-ttu-id="b33c5-760">Standortbasiertes Routing für `webapp deleted list` und `webapp deleted restore` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-760">Added location based routing for `webapp deleted list` and `webapp deleted restore`</span></span>
* <span data-ttu-id="b33c5-761">Problem behoben, aufgrund dessen in Azure Cloud Shell nicht auf die von einer Web-App protokollierte Ziel-URL („Sie können die App starten unter...“) geklickt werden konnte</span><span class="sxs-lookup"><span data-stu-id="b33c5-761">Fixed issue where webapp up logged target URL ("You can launch the app at...") was not clickable in Azure Cloud Shell</span></span>
* <span data-ttu-id="b33c5-762">Problem behoben, aufgrund dessen beim Erstellen von Apps bei einigen SKUs ein AlwaysOn-Fehler auftrat</span><span class="sxs-lookup"><span data-stu-id="b33c5-762">Fixed an issue where creating apps with the some SKUs was failing with an AlwaysOn error</span></span>
* <span data-ttu-id="b33c5-763">Vorabüberprüfung zu `[appservice|webapp] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-763">Added pre-validation to `[appservice|webapp] create`</span></span>
* <span data-ttu-id="b33c5-764">`[webapp|functionapp] traffic-routing` korrigiert, damit der richtige actionHostName-Wert verwendet wird</span><span class="sxs-lookup"><span data-stu-id="b33c5-764">Fixed `[webapp|functionapp] traffic-routing` to use the correct actionHostName</span></span>
* <span data-ttu-id="b33c5-765">Slotunterstützung zu `functionapp`-Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-765">Added slot support to `functionapp` commands</span></span>

### <a name="batch"></a><span data-ttu-id="b33c5-766">Batch</span><span class="sxs-lookup"><span data-stu-id="b33c5-766">Batch</span></span>
* <span data-ttu-id="b33c5-767">AAD-Authentifizierungsregression korrigiert, die von übermäßiger Berichterstellung für Authentifizierung mit gemeinsam verwendetem Schlüssel verursacht wurde</span><span class="sxs-lookup"><span data-stu-id="b33c5-767">Fixed AAD auth regression caused by over-aggressive error reporting for Shared Key Auth</span></span>

### <a name="batchai"></a><span data-ttu-id="b33c5-768">Batch AI</span><span class="sxs-lookup"><span data-stu-id="b33c5-768">BatchAI</span></span>
* <span data-ttu-id="b33c5-769">BatchAI-Befehle sind jetzt veraltet und ausgeblendet.</span><span class="sxs-lookup"><span data-stu-id="b33c5-769">BatchAI commands are now deprecated and hidden</span></span>

### <a name="botservice"></a><span data-ttu-id="b33c5-770">BotService</span><span class="sxs-lookup"><span data-stu-id="b33c5-770">BotService</span></span>
* <span data-ttu-id="b33c5-771">Für Befehle, die Version 3 des SDK unterstützen, wurden die Warnmeldungen „Support eingestellt“/„Wartungsmodus“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-771">Added "discontinued support"/"maintenance mode" warning messages for commands that support the v3 SDK</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="b33c5-772">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="b33c5-772">CosmosDB</span></span>
* <span data-ttu-id="b33c5-773">[VERALTET] Der Befehl `cosmosdb list-keys` wurde als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="b33c5-773">[DEPRECATED] Deprecated the `cosmosdb list-keys` command</span></span>
* <span data-ttu-id="b33c5-774">Befehl `cosmosdb keys list` hinzugefügt, er ersetzt `cosmosdb list-keys`.</span><span class="sxs-lookup"><span data-stu-id="b33c5-774">Added the `cosmosdb keys list` command - replaces `cosmosdb list-keys`</span></span>
* <span data-ttu-id="b33c5-775">`cosmsodb create/update`: Neues Format für „--location“ hinzugefügt, um das Festlegen der Eigenschaft „isZoneRedundant“ zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="b33c5-775">`cosmsodb create/update`: Added new format for --location to allow setting "isZoneRedundant" property.</span></span> <span data-ttu-id="b33c5-776">Das alte Format wurde als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="b33c5-776">Deprecated old format</span></span>

### <a name="eventgrid"></a><span data-ttu-id="b33c5-777">EventGrid</span><span class="sxs-lookup"><span data-stu-id="b33c5-777">EventGrid</span></span>
* <span data-ttu-id="b33c5-778">`eventgrid domain`-Befehle für CRUD-Vorgänge für Domänen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-778">Added `eventgrid domain` commands for domain CRUD operations</span></span>
* <span data-ttu-id="b33c5-779">`eventgrid domain topic`-Befehle für CRUD-Vorgänge für Domänenthemen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-779">Added `eventgrid domain topic` commands for domain topics CRUD operations</span></span>
* <span data-ttu-id="b33c5-780">Argument `--odata-query` zu `eventgrid [topic|event-subscription] list` zum Filtern der Ergebnisse mithilfe von OData-Syntax hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-780">Added `--odata-query` argument to `eventgrid [topic|event-subscription] list` for filtering results using OData syntax</span></span>
* <span data-ttu-id="b33c5-781">`event-subscription create/update`: „servicebusqueue“ als neue Werte für den Parameter `--endpoint-type` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-781">`event-subscription create/update`: Added servicebusqueue as new values for the `--endpoint-type` parameter</span></span>
* <span data-ttu-id="b33c5-782">[BREAKING CHANGE] Unterstützung für `--included-event-types All` mit `eventgrid event-subscription [create|update]` entfernt</span><span class="sxs-lookup"><span data-stu-id="b33c5-782">[BREAKING CHANGE] Removed support for `--included-event-types All` with `eventgrid event-subscription [create|update]`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="b33c5-783">HDInsight</span><span class="sxs-lookup"><span data-stu-id="b33c5-783">HDInsight</span></span>
* <span data-ttu-id="b33c5-784">Unterstützung für den Parameter `--ssh-public-key` im Befehl vom Typ `hdinsight create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-784">Added support for `--ssh-public-key` parameter in `hdinsight create` command</span></span>

### <a name="iot"></a><span data-ttu-id="b33c5-785">IoT</span><span class="sxs-lookup"><span data-stu-id="b33c5-785">IoT</span></span>
* <span data-ttu-id="b33c5-786">Unterstützung für das erneute Generieren von Autorisierungsrichtlinienschlüsseln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-786">Added support to regenerate authorization policy keys</span></span>
* <span data-ttu-id="b33c5-787">SDK und Unterstützung für den Bereitstellungsdienst des DigitalTwin-Repositorys hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-787">Added SDK and support for DigitalTwin Repository Provisioning Service</span></span>

### <a name="network"></a><span data-ttu-id="b33c5-788">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="b33c5-788">Network</span></span>
* <span data-ttu-id="b33c5-789">Zonenunterstützung für NAT Gateway hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-789">Added Zone support for Nat Gateway</span></span>
* <span data-ttu-id="b33c5-790">Befehl `network list-service-tags` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-790">Added command `network list-service-tags`</span></span>
* <span data-ttu-id="b33c5-791">Problem mit `dns zone import` behoben, aufgrund dessen Benutzer keine A-Platzhaltereinträge importieren konnten</span><span class="sxs-lookup"><span data-stu-id="b33c5-791">Fixed issue with `dns zone import` where users could not import wildcard A records</span></span>
* <span data-ttu-id="b33c5-792">Problem mit `watcher flow-log configure` behoben, aufgrund dessen die Flowprotokollierung in bestimmten Regionen nicht aktiviert werden konnte</span><span class="sxs-lookup"><span data-stu-id="b33c5-792">Fixed issue with `watcher flow-log configure` where flow logging could not be enabled in certain regions</span></span>

### <a name="resource"></a><span data-ttu-id="b33c5-793">Resource</span><span class="sxs-lookup"><span data-stu-id="b33c5-793">Resource</span></span>
* <span data-ttu-id="b33c5-794">Befehl `az rest` zum Ausführen von REST-Aufrufen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-794">Added `az rest` command for making REST calls</span></span>
* <span data-ttu-id="b33c5-795">Fehler behoben, der bei Verwendung von `policy assignment list` mit `--scope` auf Ressourcengruppen- oder Abonnementebene auftrat</span><span class="sxs-lookup"><span data-stu-id="b33c5-795">Fixed error when using `policy assignment list` with a resource group or subscription level `--scope`</span></span>

### <a name="servicebus"></a><span data-ttu-id="b33c5-796">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="b33c5-796">ServiceBus</span></span>
* <span data-ttu-id="b33c5-797">Problem mit `servicebus topic create --max-size` behoben [Nr. 9319](https://github.com/azure/azure-cli/issues/9319)</span><span class="sxs-lookup"><span data-stu-id="b33c5-797">Fixed issue with `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span></span>

### <a name="sql"></a><span data-ttu-id="b33c5-798">SQL</span><span class="sxs-lookup"><span data-stu-id="b33c5-798">SQL</span></span>
* <span data-ttu-id="b33c5-799">`--location` wurde geändert und ist nun für `sql [server|mi] create` optional. Ohne Angabe wird der Ressourcengruppenstandort verwendet.</span><span class="sxs-lookup"><span data-stu-id="b33c5-799">Changed `--location` to be optional for `sql [server|mi] create` - uses resource group location if not specified</span></span>
* <span data-ttu-id="b33c5-800">Der Fehler, dass das Objekt „NoneType“ nicht wiederholbar ist, wurde für `sql db list-editions --available` behoben.</span><span class="sxs-lookup"><span data-stu-id="b33c5-800">Fixed "'NoneType' object is not iterable" error for `sql db list-editions --available`</span></span>

### <a name="sqlvm"></a><span data-ttu-id="b33c5-801">SQLVm</span><span class="sxs-lookup"><span data-stu-id="b33c5-801">SQLVm</span></span>
* <span data-ttu-id="b33c5-802">[WICHTIGE ÄNDERUNG] `sql vm create` wurde geändert und erfordert nun den Parameter `--license-type`.</span><span class="sxs-lookup"><span data-stu-id="b33c5-802">[BREAKING CHNAGE] Changed `sql vm create` to require `--license-type` parameter</span></span>
* <span data-ttu-id="b33c5-803">Änderung, um beim Erstellen oder Aktualisieren einer SQL-VM das Festlegen der SQL-Image-SKU zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="b33c5-803">Changed to allow setting SQL image SKU when creating or updating a sql vm</span></span>

### <a name="storage"></a><span data-ttu-id="b33c5-804">Storage</span><span class="sxs-lookup"><span data-stu-id="b33c5-804">Storage</span></span>
* <span data-ttu-id="b33c5-805">Problem mit fehlendem Kontoschlüssel für `storage container generate-sas` behoben</span><span class="sxs-lookup"><span data-stu-id="b33c5-805">Fixed issue with missing account key for `storage container generate-sas`</span></span>
* <span data-ttu-id="b33c5-806">Problem mit `storage blob sync` unter Linux behoben</span><span class="sxs-lookup"><span data-stu-id="b33c5-806">Fixed issue with `storage blob sync` on Linux</span></span>

### <a name="vm"></a><span data-ttu-id="b33c5-807">VM</span><span class="sxs-lookup"><span data-stu-id="b33c5-807">VM</span></span>
* <span data-ttu-id="b33c5-808">[VORSCHAU] Befehle vom Typ `vm image template` zum Erstellen von VM-Images hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-808">[PREVIEW] Added `vm image template` commands to build VM images</span></span>

## <a name="june-4-2019"></a><span data-ttu-id="b33c5-809">4\. Juni 2019</span><span class="sxs-lookup"><span data-stu-id="b33c5-809">June 4, 2019</span></span>

<span data-ttu-id="b33c5-810">Version 2.0.66</span><span class="sxs-lookup"><span data-stu-id="b33c5-810">Version 2.0.66</span></span>

### <a name="core"></a><span data-ttu-id="b33c5-811">Core</span><span class="sxs-lookup"><span data-stu-id="b33c5-811">Core</span></span>
* <span data-ttu-id="b33c5-812">Fehler behoben, aufgrund dessen bei Befehlen ein Fehler auftrat, wenn `--output yaml` mit `--query` verwendet wurde</span><span class="sxs-lookup"><span data-stu-id="b33c5-812">Fixed bug where commands fail if `--output yaml` is used with `--query`</span></span>

### <a name="acr"></a><span data-ttu-id="b33c5-813">ACR</span><span class="sxs-lookup"><span data-stu-id="b33c5-813">ACR</span></span>
* <span data-ttu-id="b33c5-814">Befehlsgruppe „acr pack“ zum Erstellen von Aufgaben zur Schnellerstellung mit Buildpacks hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-814">Added 'acr pack' command group for creating quick build Tasks using Buildpacks.</span></span>

### <a name="acs"></a><span data-ttu-id="b33c5-815">ACS</span><span class="sxs-lookup"><span data-stu-id="b33c5-815">ACS</span></span>
* <span data-ttu-id="b33c5-816">Zulassen der Aktivierung/Deaktivierung des AKS-Add-Ons für das Kube-Dashboard</span><span class="sxs-lookup"><span data-stu-id="b33c5-816">Allow enabling/disabling AKS kube-dashboard addon</span></span>
* <span data-ttu-id="b33c5-817">Ausgeben einer benutzerfreundlichen Nachricht, wenn das Abonnement nicht in der Whitelist zur Verwendung von Azure Red Hat OpenShift enthalten ist</span><span class="sxs-lookup"><span data-stu-id="b33c5-817">Print a friendly message when the subscription is not whitelisted to use Azure Red Hat OpenShift</span></span>

### <a name="batch"></a><span data-ttu-id="b33c5-818">Batch</span><span class="sxs-lookup"><span data-stu-id="b33c5-818">Batch</span></span>
* <span data-ttu-id="b33c5-819">Bessere Fehlerbehandlung, wenn der Benutzer nicht bei einem Konto angemeldet ist \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span><span class="sxs-lookup"><span data-stu-id="b33c5-819">Improved error handling when not logged in to an account \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span></span>

### <a name="iot"></a><span data-ttu-id="b33c5-820">IoT</span><span class="sxs-lookup"><span data-stu-id="b33c5-820">IoT</span></span>
* <span data-ttu-id="b33c5-821">Unterstützung für manuelles Failover hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-821">Added support for manual failover</span></span>

### <a name="network"></a><span data-ttu-id="b33c5-822">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="b33c5-822">Network</span></span>
* <span data-ttu-id="b33c5-823">Befehle vom Typ `network application-gateway waf-policy` hinzugefügt, um benutzerdefinierte WAF-Regeln zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="b33c5-823">Added `network application-gateway waf-policy` commands to support custom WAF rules.</span></span>
* <span data-ttu-id="b33c5-824">Argumente `--waf-policy` und `--max-capacity` zu `network application-gateway [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-824">Added `--waf-policy` and `--max-capacity` arguments to `network application-gateway [create|update]`</span></span> 

### <a name="resource"></a><span data-ttu-id="b33c5-825">Resource</span><span class="sxs-lookup"><span data-stu-id="b33c5-825">Resource</span></span>
* <span data-ttu-id="b33c5-826">Verbesserte Fehlermeldungen aus `deployment create`, wenn TTY nicht verfügbar ist</span><span class="sxs-lookup"><span data-stu-id="b33c5-826">Improved error message from `deployment create` when there is no TTY available</span></span>

### <a name="role"></a><span data-ttu-id="b33c5-827">Role</span><span class="sxs-lookup"><span data-stu-id="b33c5-827">Role</span></span>
* <span data-ttu-id="b33c5-828">Hilfetext aktualisiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-828">Updated help text.</span></span>

### <a name="compute"></a><span data-ttu-id="b33c5-829">Compute</span><span class="sxs-lookup"><span data-stu-id="b33c5-829">Compute</span></span>
* <span data-ttu-id="b33c5-830">Unterstützung zu `vm create` für virtuelle Computer aus einem verwalteten Image mit Datenträger-LUNs hinzugefügt, die nicht bei 0 beginnen oder die Nummern überspringen</span><span class="sxs-lookup"><span data-stu-id="b33c5-830">Added support to `vm create` for VMs from a managed image with data-disk luns that do not start from 0 or that skip numbers</span></span>

## <a name="may-21-2019"></a><span data-ttu-id="b33c5-831">21. Mai 2019</span><span class="sxs-lookup"><span data-stu-id="b33c5-831">May 21, 2019</span></span>

<span data-ttu-id="b33c5-832">Version 2.0.65</span><span class="sxs-lookup"><span data-stu-id="b33c5-832">Version 2.0.65</span></span>

### <a name="core"></a><span data-ttu-id="b33c5-833">Core</span><span class="sxs-lookup"><span data-stu-id="b33c5-833">Core</span></span>
* <span data-ttu-id="b33c5-834">Besseres Feedback für Authentifizierungsfehler hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-834">Added better feedback for authentication errors</span></span>
* <span data-ttu-id="b33c5-835">Problem behoben, aufgrund dessen die CLI Erweiterungen lädt, die nicht mit der Core-Version kompatibel waren</span><span class="sxs-lookup"><span data-stu-id="b33c5-835">Fixed issue where the CLI would load extensions that were not compatible with its core version</span></span>
* <span data-ttu-id="b33c5-836">Problem beim Starten behoben, wenn `clouds.config` beschädigt ist</span><span class="sxs-lookup"><span data-stu-id="b33c5-836">Fixed issue with launching when `clouds.config` is corrupted</span></span>

### <a name="acr"></a><span data-ttu-id="b33c5-837">ACR</span><span class="sxs-lookup"><span data-stu-id="b33c5-837">ACR</span></span>
* <span data-ttu-id="b33c5-838">Unterstützung für verwaltete Identitäten zu Aufgaben hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-838">Added support for Managed Identities to Tasks</span></span>

### <a name="acs"></a><span data-ttu-id="b33c5-839">ACS</span><span class="sxs-lookup"><span data-stu-id="b33c5-839">ACS</span></span>
* <span data-ttu-id="b33c5-840">`openshift create`-Befehl bei der Verwendung mit dem AAD-Kundenclient korrigiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-840">Fixed `openshift create` command when used with customer AAD client</span></span>

### <a name="appservice"></a><span data-ttu-id="b33c5-841">AppService</span><span class="sxs-lookup"><span data-stu-id="b33c5-841">AppService</span></span>
* <span data-ttu-id="b33c5-842">[VERALTET] Befehl `functionapp devops-build` als veraltet gekennzeichnet – wird in der nächsten Version entfernt</span><span class="sxs-lookup"><span data-stu-id="b33c5-842">[DEPRECATED] Deprecated `functionapp devops-build` command - will be removed in next release</span></span>
* <span data-ttu-id="b33c5-843">`functionapp devops-pipeline` geändert, um das Buildprotokoll von Azure DevOps im ausführlichen Modus abzurufen</span><span class="sxs-lookup"><span data-stu-id="b33c5-843">Changed `functionapp devops-pipeline` to fetch build log from Azure DevOps in verbose mode</span></span>
* <span data-ttu-id="b33c5-844">[BREAKING CHANGE] Flag `--use_local_settings` aus dem Befehl `functionapp devops-pipeline` entfernt – kein Vorgang wurde ausgeführt</span><span class="sxs-lookup"><span data-stu-id="b33c5-844">[BREAKING CHANGE] Removed `--use_local_settings` flag from `functionapp devops-pipeline` command - was a no-op</span></span>
* <span data-ttu-id="b33c5-845">`webapp up` geändert, sodass die JSON-Ausgabe zurückgegeben wird, wenn `--logs` nicht verwendet wird</span><span class="sxs-lookup"><span data-stu-id="b33c5-845">Changed `webapp up` to return JSON output if `--logs` is not used</span></span>
* <span data-ttu-id="b33c5-846">Unterstützung hinzugefügt zum Schreiben von Standardressourcen in die lokale Konfiguration für `webapp up`</span><span class="sxs-lookup"><span data-stu-id="b33c5-846">Added support for writing default resources to local config for `webapp up`</span></span>
* <span data-ttu-id="b33c5-847">Unterstützung zu `webapp up` hinzugefügt für die erneute Bereitstellung einer App ohne Verwendung des `--location`-Arguments</span><span class="sxs-lookup"><span data-stu-id="b33c5-847">Added support to `webapp up` for redeploying an app without using the `--location` argument</span></span>
* <span data-ttu-id="b33c5-848">Problem behoben, bei dem für die ASP-Erstellung der Linux-SKU „Free“ der SKU-Wert „Free“ nicht funktioniert hat</span><span class="sxs-lookup"><span data-stu-id="b33c5-848">Fixed an issue where for Linux Free SKU ASP creation use Free as SKU value was not working</span></span>

### <a name="botservice"></a><span data-ttu-id="b33c5-849">BotService</span><span class="sxs-lookup"><span data-stu-id="b33c5-849">BotService</span></span>
* <span data-ttu-id="b33c5-850">Geändert, sodass Groß-/Kleinschreibung für `--lang`-Parameter für Befehle zulässig ist</span><span class="sxs-lookup"><span data-stu-id="b33c5-850">Changed to allow all casing for `--lang` parameters for commands</span></span>
* <span data-ttu-id="b33c5-851">Beschreibung für das Befehlsmodul aktualisiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-851">Updated description for command module</span></span>

### <a name="consumption"></a><span data-ttu-id="b33c5-852">Nutzung</span><span class="sxs-lookup"><span data-stu-id="b33c5-852">Consumption</span></span>
* <span data-ttu-id="b33c5-853">Fehlende erforderliche Parameter bei der Ausführung von `consumption usage list --billing-period-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-853">Added missing required parameter when running `consumption usage list --billing-period-name`</span></span>

### <a name="iot"></a><span data-ttu-id="b33c5-854">IoT</span><span class="sxs-lookup"><span data-stu-id="b33c5-854">IoT</span></span>
* <span data-ttu-id="b33c5-855">Unterstützung für das Auflisten aller Schlüssel hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-855">Added support to list all keys</span></span>

### <a name="network"></a><span data-ttu-id="b33c5-856">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="b33c5-856">Network</span></span>
* [BREAKING CHANGE]: Removed `network interface-endpoints` command group - use `network private-endpoints` 
* <span data-ttu-id="b33c5-858">`--nat-gateway`-Argument zu `network vnet subnet [create|update]` für das Anfügen an ein NAT-Gateway hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-858">Added `--nat-gateway` argument to `network vnet subnet [create|update]` for attaching to a NAT gateway</span></span>
* <span data-ttu-id="b33c5-859">Problem mit `dns zone import` behoben, aufgrund dessen Eintragsnamen keinem Datensatztyp entsprochen haben</span><span class="sxs-lookup"><span data-stu-id="b33c5-859">Fixed issue with `dns zone import` where record names could not match a record type</span></span>

### <a name="rdbms"></a><span data-ttu-id="b33c5-860">RDBMS</span><span class="sxs-lookup"><span data-stu-id="b33c5-860">RDBMS</span></span>
* <span data-ttu-id="b33c5-861">Postgres- und MySLQ-Unterstützung für die Georeplikation hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-861">Added postgres and mysql support for geo replication</span></span>

### <a name="rbac"></a><span data-ttu-id="b33c5-862">RBAC</span><span class="sxs-lookup"><span data-stu-id="b33c5-862">RBAC</span></span>
* <span data-ttu-id="b33c5-863">Unterstützung für den Verwaltungsgruppenumfang zu `role assignment` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-863">Added support for management group scope to `role assignment`</span></span>

### <a name="storage"></a><span data-ttu-id="b33c5-864">Storage</span><span class="sxs-lookup"><span data-stu-id="b33c5-864">Storage</span></span>
* <span data-ttu-id="b33c5-865">`storage blob sync`: Synchronisierungsbefehl für Speicherblob hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-865">`storage blob sync`: add sync command for storage blob</span></span>

### <a name="compute"></a><span data-ttu-id="b33c5-866">Compute</span><span class="sxs-lookup"><span data-stu-id="b33c5-866">Compute</span></span>
* <span data-ttu-id="b33c5-867">`--computer-name` zu `vm create` zum Festlegen des Computernamens eines virtuellen Computers hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-867">Added `--computer-name` to `vm create` for setting a VM's computer name</span></span>
* <span data-ttu-id="b33c5-868">`--ssh-key-value` umbenannt in `--ssh-key-values` für `[vm|vmss] create`: Jetzt können mehrere öffentliche SSH-Schlüsselwerte oder -pfade akzeptiert werden.</span><span class="sxs-lookup"><span data-stu-id="b33c5-868">Renamed `--ssh-key-value` renamed to `--ssh-key-values` for `[vm|vmss] create` - can now accept multiple ssh public key values or paths</span></span>
  * <span data-ttu-id="b33c5-869">__Hinweis__: Dies ist **kein** Breaking Change: `--ssh-key-value` wird korrekt analysiert, da nur eine Übereinstimmung mit `--ssh-key-values` besteht.</span><span class="sxs-lookup"><span data-stu-id="b33c5-869">__Note__: This is **not** a breaking change - `--ssh-key-value` will be parsed correctly as it matches only `--ssh-key-values`</span></span>
* <span data-ttu-id="b33c5-870">`--type`-Argument von `ppg create` in optionales Argument geändert</span><span class="sxs-lookup"><span data-stu-id="b33c5-870">Changed the `--type` argument of `ppg create` to be optional</span></span>

## <a name="may-6-2019"></a><span data-ttu-id="b33c5-871">6\. Mai 2019</span><span class="sxs-lookup"><span data-stu-id="b33c5-871">May 6, 2019</span></span>

<span data-ttu-id="b33c5-872">Version 2.0.64</span><span class="sxs-lookup"><span data-stu-id="b33c5-872">Version 2.0.64</span></span>

### <a name="acs"></a><span data-ttu-id="b33c5-873">ACS</span><span class="sxs-lookup"><span data-stu-id="b33c5-873">ACS</span></span>
* <span data-ttu-id="b33c5-874">[BREAKING CHANGE] Flag `--fqdn` aus den `openshift`-Befehlen entfernt</span><span class="sxs-lookup"><span data-stu-id="b33c5-874">[BREAKING CHANGE] Removed `--fqdn` flag on `openshift` commands</span></span>
* <span data-ttu-id="b33c5-875">Geändert, sodass die allgemein verfügbare Azure Red Hat Openshift-API-Version verwendet wird</span><span class="sxs-lookup"><span data-stu-id="b33c5-875">Changed to use Azure Red Hat Openshift GA API Version</span></span>
* <span data-ttu-id="b33c5-876">Flag `customer-admin-group-id` wurde zu `openshift create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-876">Added `customer-admin-group-id` flag to `openshift create`</span></span>
* <span data-ttu-id="b33c5-877">[ALLGEMEIN VERFÜGBAR] `(PREVIEW)` aus der `aks create`-Option `--network-policy` entfernt</span><span class="sxs-lookup"><span data-stu-id="b33c5-877">[GA] Removed `(PREVIEW)` from `aks create` option `--network-policy`</span></span>

### <a name="appservice"></a><span data-ttu-id="b33c5-878">AppService</span><span class="sxs-lookup"><span data-stu-id="b33c5-878">Appservice</span></span>
* <span data-ttu-id="b33c5-879">[VERALTET] Befehl `functionapp devops-build` als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="b33c5-879">[DEPRECATED] Deprecated `functionapp devops-build` command</span></span>
  * <span data-ttu-id="b33c5-880">Umbenannt in `functionapp devops-pipeline`</span><span class="sxs-lookup"><span data-stu-id="b33c5-880">Renamed to `functionapp devops-pipeline`</span></span>
* <span data-ttu-id="b33c5-881">Fehler beim Abrufen des richtigen Benutzernamens für Cloud Shell behoben, der einen Fehler von `webapp up` verursachte</span><span class="sxs-lookup"><span data-stu-id="b33c5-881">Fixed getting the correct username for cloudshell which was causing `webapp up` to fail</span></span>
* <span data-ttu-id="b33c5-882">Dokumentation von `appservice plan --sku` mit den unterstützten App Service-Plänen aktualisiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-882">Updated `appservice plan --sku` documentation updated to reflect the supported appserviceplans</span></span>
* <span data-ttu-id="b33c5-883">Optionale Argumente für Ressourcengruppe und Plan zu `webapp up` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-883">Added optional arguments for resource group and plan to `webapp up`</span></span>
* <span data-ttu-id="b33c5-884">Unterstützung zur Berücksichtigung der Umgebungsvariablen `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` zu `webapp ssh` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-884">Added support to `webapp ssh` to respect `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>
* <span data-ttu-id="b33c5-885">Unterstützung für `appserviceplan create` für die kostenlose Linux-SKU hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-885">Added `appserviceplan create` support for Linux Free SKU</span></span>
* <span data-ttu-id="b33c5-886">`webapp up` geändert, um nach dem Festlegen der App-Einstellung `SCM_DO_BUILD_DURING_DEPLOYMENT=true` zum Verarbeiten des Kudu-Kaltstarts für 30 Sekunden in den Energiesparmodus zu wechseln</span><span class="sxs-lookup"><span data-stu-id="b33c5-886">Changed `webapp up` to have a 30s sleep after setting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` appsetting to handle kudu cold start</span></span>
* <span data-ttu-id="b33c5-887">Unterstützung für die `powershell`-Runtime zu `functionapp create` unter Windows hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-887">Added support for `powershell` runtime to `functionapp create` on Windows</span></span>
* <span data-ttu-id="b33c5-888">Befehl `create-remote-connection` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-888">Added `create-remote-connection` command</span></span>

### <a name="batch"></a><span data-ttu-id="b33c5-889">Batch</span><span class="sxs-lookup"><span data-stu-id="b33c5-889">Batch</span></span>
* <span data-ttu-id="b33c5-890">Fehler im Validierungssteuerelement für `--application-package-references`-Optionen korrigiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-890">Fixed bug in validator for `--application-package-references` options</span></span>

### <a name="botservice"></a><span data-ttu-id="b33c5-891">Botservice</span><span class="sxs-lookup"><span data-stu-id="b33c5-891">Botservice</span></span>
* <span data-ttu-id="b33c5-892">[BREAKING CHANGE]`bot create -v v4 -k webapp` geändert, sodass standardmäßig eine leerer Web-App-Bot erstellt wird (d. h. kein Bot wird in App Service bereitgestellt)</span><span class="sxs-lookup"><span data-stu-id="b33c5-892">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to create an empty Web App Bot by default (i.e. no bot is deployed to the App Service)</span></span>
* <span data-ttu-id="b33c5-893">`--echo`-Flag zu `bot create` hinzugefügt, sodass das alte Verhalten mit `-v v4` verwendet wird</span><span class="sxs-lookup"><span data-stu-id="b33c5-893">Added `--echo` flag to `bot create` to use the old behavior with `-v v4`</span></span>
* <span data-ttu-id="b33c5-894">[BREAKING CHANGE] Standardwert von `--version` in `v4` geändert</span><span class="sxs-lookup"><span data-stu-id="b33c5-894">[BREAKING CHANGE] Changed the default value of  `--version` to `v4`</span></span>
  * <span data-ttu-id="b33c5-895">__HINWEIS:__ `bot prepare-publish` verwendet weiterhin den alten Standard.</span><span class="sxs-lookup"><span data-stu-id="b33c5-895">__NOTE:__ `bot prepare-publish` still uses the its old default</span></span>
* <span data-ttu-id="b33c5-896">[BREAKING CHANGE]`--lang` geändert, sodass der Standard nicht mehr `Csharp` ist.</span><span class="sxs-lookup"><span data-stu-id="b33c5-896">[BREAKING CHANGE] Changed `--lang` to no longer default to `Csharp`.</span></span> <span data-ttu-id="b33c5-897">Wenn der Befehl `--lang` erfordert und dies nicht angegeben ist, wird der Befehl nun mit Fehler beendet.</span><span class="sxs-lookup"><span data-stu-id="b33c5-897">If the command requires `--lang` and it is not provided, the command will now error out</span></span>
* <span data-ttu-id="b33c5-898">[BREAKING CHANGE]`--appid`- und `--password`-Argumente für `bot create` in erforderlich geändert, sie können jetzt über `ad app create` erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="b33c5-898">[BREAKING CHANGE] Changed the `--appid` and `--password` args for `bot create` to be required and can now be created via `ad app create`</span></span>
* <span data-ttu-id="b33c5-899">`--appid`- und `--password`-Validierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-899">Added `--appid` and `--password` validation</span></span>
* <span data-ttu-id="b33c5-900">[BREAKING CHANGE]`bot create -v v4` geändert, sodass kein Speicherkonto bzw. keine Application Insights-Instanz erstellt oder verwendet wird</span><span class="sxs-lookup"><span data-stu-id="b33c5-900">[BREAKING CHANGE] Changed `bot create -v v4` to not create or use a Storage Account or Application Insights</span></span>
* <span data-ttu-id="b33c5-901">[BREAKING CHANGE]`bot create -v v3` geändert, sodass eine Region erforderlich ist, in der Application Insights verfügbar ist</span><span class="sxs-lookup"><span data-stu-id="b33c5-901">[BREAKING CHANGE] Changed `bot create -v v3` to require a region where Application Insights is available</span></span>
* <span data-ttu-id="b33c5-902">[BREAKING CHANGE]`bot update` geändert, sodass es sich jetzt nur auf spezifische Eigenschaften eines Bots auswirkt</span><span class="sxs-lookup"><span data-stu-id="b33c5-902">[BREAKING CHANGE] Changed `bot update` to now affect only specific properties of a bot</span></span>
* <span data-ttu-id="b33c5-903">[BREAKING CHANGE]`--lang`-Flags geändert, sodass `Javascript` anstelle von `Node` akzeptiert wird</span><span class="sxs-lookup"><span data-stu-id="b33c5-903">[BREAKING CHANGE] Changed `--lang` flags to accept `Javascript` instead of `Node`</span></span>
* <span data-ttu-id="b33c5-904">[BREAKING CHANGE]`Node` als zulässiger `--lang`-Wert entfernt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-904">[BREAKING CHANGE] Removed `Node` as an allowed `--lang` value</span></span>
* <span data-ttu-id="b33c5-905">[BREAKING CHANGE]`bot create -v v4 -k webapp` geändert, sodass `SCM_DO_BUILD_DURING_DEPLOYMENT` nicht mehr auf TRUE festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="b33c5-905">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to no longer set `SCM_DO_BUILD_DURING_DEPLOYMENT` to true.</span></span> <span data-ttu-id="b33c5-906">Alle Bereitstellungen über Kudu fungieren ihrem Standardverhalten entsprechend.</span><span class="sxs-lookup"><span data-stu-id="b33c5-906">All deployments through Kudu will act according to their default behavior</span></span>
* <span data-ttu-id="b33c5-907">`bot download` für Bots ohne `.bot`-Dateien geändert, sodass die sprachspezifische Konfigurationsdatei mit Werten aus den Anwendungseinstellungen für den Bot erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="b33c5-907">Changed `bot download` for bots without `.bot` files to create the language-specific configuration file with values from the Application Settings for the bot</span></span>
* <span data-ttu-id="b33c5-908">Unterstützung für `Typescript` zu `bot prepare-deploy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-908">Added `Typescript` support to `bot prepare-deploy`</span></span>
* <span data-ttu-id="b33c5-909">Warnmeldung zu `bot prepare-deploy` für `Javascript`- und `Typescript`-Bots hinzugefügt, wenn `package.json` in `--code-dir` nicht enthalten ist</span><span class="sxs-lookup"><span data-stu-id="b33c5-909">Added warning message to `bot prepare-deploy` for `Javascript` and `Typescript` bots for when `--code-dir` does not contain `package.json`</span></span>
* <span data-ttu-id="b33c5-910">`bot prepare-deploy` geändert, sodass bei Erfolg `true` zurückgegeben wird</span><span class="sxs-lookup"><span data-stu-id="b33c5-910">Changed `bot prepare-deploy` to return `true` if successful</span></span>
* <span data-ttu-id="b33c5-911">Ausführliche Protokollierung zu `bot prepare-deploy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-911">Added verbose logging to `bot prepare-deploy`</span></span>
* <span data-ttu-id="b33c5-912">Mehr verfügbare Application Insights-Regionen zu `az bot create -v v3` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-912">Added more available Application Insights regions to `az bot create -v v3`</span></span>

### <a name="configure"></a><span data-ttu-id="b33c5-913">Konfigurieren</span><span class="sxs-lookup"><span data-stu-id="b33c5-913">Configure</span></span>
* <span data-ttu-id="b33c5-914">Unterstützung für die ordnerbasierte Argument-Standardwertkonfigurationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-914">Added support for folder based argument default value configurations</span></span>

### <a name="eventhubs"></a><span data-ttu-id="b33c5-915">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="b33c5-915">Eventhubs</span></span>
* <span data-ttu-id="b33c5-916">Befehle vom Typ `namespace network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-916">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="b33c5-917">`--default-action`-Argument für Netzwerkregeln zu `namespace [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-917">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="b33c5-918">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="b33c5-918">Network</span></span>
* <span data-ttu-id="b33c5-919">[BREAKING CHANGE]`--cache`-Argument mit `--defer` für `vnet [create|update]` ersetzt</span><span class="sxs-lookup"><span data-stu-id="b33c5-919">[BREAKING CHANGE] Replaced `--cache` arugment with `--defer` for `vnet [create|update]`</span></span> 

### <a name="policy-insights"></a><span data-ttu-id="b33c5-920">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="b33c5-920">Policy Insights</span></span>
* <span data-ttu-id="b33c5-921">Unterstützung für `--expand PolicyEvaluationDetails` hinzugefügt, sodass Richtlinienauswertungsdetails von der Ressource abgefragt werden</span><span class="sxs-lookup"><span data-stu-id="b33c5-921">Added support for `--expand PolicyEvaluationDetails` to query policy evaluation details on the resource</span></span>

### <a name="role"></a><span data-ttu-id="b33c5-922">Role</span><span class="sxs-lookup"><span data-stu-id="b33c5-922">Role</span></span>
* <span data-ttu-id="b33c5-923">[VERALTET]: Ausblenden des „--password"-Arguments von `create-for-rbac` geändert; Unterstützung wird im Mai 2019 entfernt</span><span class="sxs-lookup"><span data-stu-id="b33c5-923">[DEPRECATED] Changed `create-for-rbac` hide '--password' argument - support will be removed in May 2019</span></span>

### <a name="service-bus"></a><span data-ttu-id="b33c5-924">Service Bus</span><span class="sxs-lookup"><span data-stu-id="b33c5-924">Service Bus</span></span>
* <span data-ttu-id="b33c5-925">Befehle vom Typ `namespace network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-925">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="b33c5-926">`--default-action`-Argument für Netzwerkregeln zu `namespace [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-926">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>
* <span data-ttu-id="b33c5-927">`topic [create|update]` korrigiert, sodass `--max-size`-Unterstützung für 10-, 20-, 40- und 80-GB-Werte mit Premium-SKU zulässig ist</span><span class="sxs-lookup"><span data-stu-id="b33c5-927">Fixed `topic [create|update]` to allow `--max-size` support for 10, 20, 40 and 80GB values with premium SKU</span></span>

### <a name="sql"></a><span data-ttu-id="b33c5-928">SQL</span><span class="sxs-lookup"><span data-stu-id="b33c5-928">SQL</span></span>
* <span data-ttu-id="b33c5-929">Befehle vom Typ `sql virtual-cluster [list|show|delete]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-929">Added `sql virtual-cluster [list|show|delete]` commands</span></span>

### <a name="vm"></a><span data-ttu-id="b33c5-930">VM</span><span class="sxs-lookup"><span data-stu-id="b33c5-930">VM</span></span>
* <span data-ttu-id="b33c5-931">`--protect-from-scale-in` und `--protect-from-scale-set-actions` zu `vmss update` hinzugefügt, sodass Aktualisierungen der Schutzrichtlinie von VMSS-VM-Instanzen aktiviert sind</span><span class="sxs-lookup"><span data-stu-id="b33c5-931">Added `--protect-from-scale-in` and `--protect-from-scale-set-actions` to `vmss update` to enable updates to the protection policy of VMSS VM instances</span></span>
* <span data-ttu-id="b33c5-932">`--instance-id` zu `vmss update` hinzugefügt, sodass allgemeine Aktualisierungen von VMSS-VM-Instanzen aktiviert sind</span><span class="sxs-lookup"><span data-stu-id="b33c5-932">Added `--instance-id` to `vmss update` to enable generic update of VMSS VM instances</span></span>
* <span data-ttu-id="b33c5-933">`--instance-id` zu `vmss wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-933">Added `--instance-id` to `vmss wait`</span></span>
* <span data-ttu-id="b33c5-934">Neue `ppg`-Befehlsgruppe für die Verwaltung von Näherungsplatzierungsgruppen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-934">Added new `ppg` command group for managing Proximity Placement Groups</span></span>
* <span data-ttu-id="b33c5-935">`--ppg` zu `[vm|vmss] create` und `vm availability-set create` für die Verwaltung von PPGs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-935">Added `--ppg` to `[vm|vmss] create` and `vm availability-set create` for managing PPGs</span></span>
* <span data-ttu-id="b33c5-936">Parameter `--hyper-v-generation` zu `image create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-936">Added `--hyper-v-generation` parameter to `image create`</span></span>

## <a name="april-23-2019"></a><span data-ttu-id="b33c5-937">23. April 2019</span><span class="sxs-lookup"><span data-stu-id="b33c5-937">April 23, 2019</span></span>

<span data-ttu-id="b33c5-938">Version 2.0.63</span><span class="sxs-lookup"><span data-stu-id="b33c5-938">Version 2.0.63</span></span>

### <a name="acs"></a><span data-ttu-id="b33c5-939">ACS</span><span class="sxs-lookup"><span data-stu-id="b33c5-939">ACS</span></span>
* <span data-ttu-id="b33c5-940">`aks get-credentials` zur Anzeige einer Eingabeaufforderung zum Überschreiben doppelter Werte geändert</span><span class="sxs-lookup"><span data-stu-id="b33c5-940">Changed `aks get-credentials` to prompt to overwrite duplicated values</span></span>
* <span data-ttu-id="b33c5-941">`(PREVIEW)` aus Dev Spaces-Befehlen „aks use-dev-spaces“ und „aks remove-dev-spaces“ entfernt</span><span class="sxs-lookup"><span data-stu-id="b33c5-941">Removed `(PREVIEW)` from Dev Spaces commands "aks use-dev-spaces" and "aks remove-dev-spaces"</span></span>

### <a name="ams"></a><span data-ttu-id="b33c5-942">AMS</span><span class="sxs-lookup"><span data-stu-id="b33c5-942">AMS</span></span>
* <span data-ttu-id="b33c5-943">Fehler bei der Objekt- und Kontofilteraktualisierung behoben</span><span class="sxs-lookup"><span data-stu-id="b33c5-943">Fixed bug with asset and account filters update</span></span>

### <a name="appservice"></a><span data-ttu-id="b33c5-944">AppService</span><span class="sxs-lookup"><span data-stu-id="b33c5-944">AppService</span></span>
* <span data-ttu-id="b33c5-945">Unterstützung für die App Service-Umgebung (App Service Environment, ASE) und Zeitlimit zu `webapp ssh` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-945">Added support for ASE and timeout to `webapp ssh`</span></span>
* <span data-ttu-id="b33c5-946">Unterstützung für die Einrichtung von CI/CD für eine Azure DevOps-Pipeline aus einem GitHub-Repository zu Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-946">Added support for establishing CI CD to an Azure DevOps pipeline from a Github repository to Function apps</span></span>
* <span data-ttu-id="b33c5-947">`--github-pat`-Argument zu `functionapp devops-build create` hinzugefügt, um persönliche GitHub-Zugriffstoken zu akzeptieren</span><span class="sxs-lookup"><span data-stu-id="b33c5-947">Added `--github-pat` argument to `functionapp devops-build create` to accept Github personal access token</span></span>
* <span data-ttu-id="b33c5-948">`--github-repository`-Argument zu `functionapp devops-build create` hinzugefügt, um das GitHub-Repository mit dem Quellcode einer Funktions-App zu akzeptieren</span><span class="sxs-lookup"><span data-stu-id="b33c5-948">Added `--github-repository` argument to `functionapp devops-build create` to accept Github repository that contains a functionapp source code</span></span>
* <span data-ttu-id="b33c5-949">Problem behoben, aufgrund dessen bei `az webapp up --logs` ein Fehler auftrat und die .NET Core-Standardversion auf 2.1 aktualisiert wurde</span><span class="sxs-lookup"><span data-stu-id="b33c5-949">Fixed issue where `az webapp up --logs` was failing with a error and updating default .NETCORE version to 2.1</span></span>
* <span data-ttu-id="b33c5-950">Unnötige Funktions-App-Einstellungen beim Erstellen einer Funktions-App mit Verbrauchsplan entfernt</span><span class="sxs-lookup"><span data-stu-id="b33c5-950">Removed unnecessary functionapp settings when creating a function app with consumption plan</span></span>
* <span data-ttu-id="b33c5-951">`webapp up` geändert, sodass die ASP-Standardzeichenfolge jetzt eine Zahl am Ende anfügt, um einen neuen ASP basierend auf SKU-Optionen zu erstellen</span><span class="sxs-lookup"><span data-stu-id="b33c5-951">Changed `webapp up` so the default asp string now appends number at the end to create a new ASP based on SKU options</span></span>
* <span data-ttu-id="b33c5-952">`-b` als Option für `webapp up` hinzugefügt, um die App im Browser zu starten</span><span class="sxs-lookup"><span data-stu-id="b33c5-952">Added `-b` as an option to `webapp up` to launch the app in the browser</span></span>
* <span data-ttu-id="b33c5-953">`webapp deployment source config zip` geändert, um die `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`-Umgebungsvariable zu behandeln</span><span class="sxs-lookup"><span data-stu-id="b33c5-953">Changed `webapp deployment source config zip` to handle `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="b33c5-954">Bereitstellungs-Manager</span><span class="sxs-lookup"><span data-stu-id="b33c5-954">Deployment Manager</span></span>
* <span data-ttu-id="b33c5-955">[VORSCHAUVERSIPN] Erstellen und Verwalten von Artefakten, die Rollouts unterstützen</span><span class="sxs-lookup"><span data-stu-id="b33c5-955">[PREVIEW] Create and manage artifacts that support rollouts</span></span>

### <a name="lab"></a><span data-ttu-id="b33c5-956">Labor</span><span class="sxs-lookup"><span data-stu-id="b33c5-956">Lab</span></span>
* <span data-ttu-id="b33c5-957">Fehler behoben, der zu einer vorzeitigen Beendigung führen würde</span><span class="sxs-lookup"><span data-stu-id="b33c5-957">Fixed bug which would cause an early exit</span></span>

### <a name="network"></a><span data-ttu-id="b33c5-958">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="b33c5-958">Network</span></span>
* <span data-ttu-id="b33c5-959">Automatische Delegierung des Namenservers im übergeordneten Element während der Erstellung der untergeordneten Zone zu `dns zone create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-959">Added auto name server delegation to `dns zone create` in parent during child zone creation</span></span>

### <a name="resource"></a><span data-ttu-id="b33c5-960">Resource</span><span class="sxs-lookup"><span data-stu-id="b33c5-960">Resource</span></span>
* <span data-ttu-id="b33c5-961">[VERALTET]: Argumente `--link-id`, `--target-id` und `--filter-string` von `resource link` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-961">[DEPRECATED] Deprecated `--link-id`, `--target-id` and `--filter-string` arguments of `resource link`</span></span>
  * <span data-ttu-id="b33c5-962">Verwenden Sie stattdessen die Argumente `--link`, `--target` und `--filter`.</span><span class="sxs-lookup"><span data-stu-id="b33c5-962">Use the arguments `--link`, `--target`, and `--filter` instead</span></span>
* <span data-ttu-id="b33c5-963">Problem behoben, aufgrund dessen `resource link [create|update]`-Befehle nicht verwendet werden konnten</span><span class="sxs-lookup"><span data-stu-id="b33c5-963">Fixed issue where `resource link [create|update]` commands would not work</span></span>
* <span data-ttu-id="b33c5-964">Problem behoben, aufgrund dessen das Löschen anhand einer Ressourcen-ID bei einem Fehler zu einem Absturz führen konnte</span><span class="sxs-lookup"><span data-stu-id="b33c5-964">Fixed an issue where deleting using a resource ID could crash on error</span></span>

### <a name="sql"></a><span data-ttu-id="b33c5-965">SQL</span><span class="sxs-lookup"><span data-stu-id="b33c5-965">SQL</span></span>
* <span data-ttu-id="b33c5-966">Unterstützung für benutzerdefinierte Zeitzonen auf verwalteten Instanzen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-966">Added support for custom time zone on managed instances</span></span>
* <span data-ttu-id="b33c5-967">Geändert, um die Verwendung des Namens eines Pools für elastische Datenbanken mit `sql db update` zuzulassen</span><span class="sxs-lookup"><span data-stu-id="b33c5-967">Changed to allow elastic pool name to be used with `sql db update`</span></span>
* <span data-ttu-id="b33c5-968">Unterstützung für `--no-wait` zu `sql server [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-968">Added `--no-wait` support to `sql server [create|update]`</span></span>
* <span data-ttu-id="b33c5-969">Befehl `sql server wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-969">Added command `sql server wait`</span></span>

### <a name="storage"></a><span data-ttu-id="b33c5-970">Storage</span><span class="sxs-lookup"><span data-stu-id="b33c5-970">Storage</span></span>
* <span data-ttu-id="b33c5-971">Problem mit doppelt codierten SAS-Token in `storage blob generate-sas` behoben</span><span class="sxs-lookup"><span data-stu-id="b33c5-971">Fixed issue with double-encoded SAS tokens in `storage blob generate-sas`</span></span>

### <a name="vm"></a><span data-ttu-id="b33c5-972">VM</span><span class="sxs-lookup"><span data-stu-id="b33c5-972">VM</span></span>
* <span data-ttu-id="b33c5-973">`--skip-shutdown`-Flag zum Ausschalten von VMs ohne Herunterfahren zu `vm|vmss stop` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-973">Added `--skip-shutdown` flag to `vm|vmss stop` to power-off VMs without shutdown</span></span>
* <span data-ttu-id="b33c5-974">`--storage-account-type`-Argument zum Festlegen des Kontotyps des Veröffentlichungsprofils zu `sig image-version create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-974">Added `--storage-account-type` argument to `sig image-version create` to set the publishing profile's account type</span></span>
* <span data-ttu-id="b33c5-975">`--target-regions`-Argument zu `sig image-version create` hinzugefügt, um das Festlegen von regionsspezifischen Speicherkontotypen zuzulassen</span><span class="sxs-lookup"><span data-stu-id="b33c5-975">Added `--target-regions` argument to `sig image-version create` to allow setting region-specific storage account types</span></span>

## <a name="april-9-2019"></a><span data-ttu-id="b33c5-976">9\. April 2019</span><span class="sxs-lookup"><span data-stu-id="b33c5-976">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="b33c5-977">Core</span><span class="sxs-lookup"><span data-stu-id="b33c5-977">Core</span></span>
* <span data-ttu-id="b33c5-978">Problem behoben, aufgrund dessen einige Erweiterungen mit der Version `Unknown` angezeigt wurden und nicht aktualisiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="b33c5-978">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="b33c5-979">ACR</span><span class="sxs-lookup"><span data-stu-id="b33c5-979">ACR</span></span>
* <span data-ttu-id="b33c5-980">Unterstützung für die kontextlose Ausführung eines Images hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-980">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="b33c5-981">AMS</span><span class="sxs-lookup"><span data-stu-id="b33c5-981">AMS</span></span>
* [VERALTET]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
[DEPRECATED]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [BREAKING CHANGE]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="b33c5-984">Unterstützung für neue Verschlüsselungsparameter in `ams streaming-policy create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-984">Added new encryption parameters support in `ams streaming-policy create`</span></span>
* <span data-ttu-id="b33c5-985">Neuer Parameter `--filters` zu `ams streaming-locator create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-985">Added new paramter `--filters` to `ams streaming-locator create`</span></span>

### <a name="appservice"></a><span data-ttu-id="b33c5-986">AppService</span><span class="sxs-lookup"><span data-stu-id="b33c5-986">AppService</span></span>
* <span data-ttu-id="b33c5-987">Unterstützung für `--logs` zu `webapp up` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-987">Added `--logs` support to `webapp up`</span></span>
* <span data-ttu-id="b33c5-988">Probleme bei der Generierung von `azure-pipelines.yml` beim Befehl `functionapp devops-build create` behoben</span><span class="sxs-lookup"><span data-stu-id="b33c5-988">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="b33c5-989">Fehlerbehandlung und Indikatoren für `unctionapp devops-build create` verbessert</span><span class="sxs-lookup"><span data-stu-id="b33c5-989">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="b33c5-990">[BREAKING CHANGE] Flag `--local-git` für den Befehl `devops-build` entfernt; lokale Git-Erkennung und -Verarbeitung sind zum Erstellen von Azure DevOps-Pipelines obligatorisch</span><span class="sxs-lookup"><span data-stu-id="b33c5-990">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="b33c5-991">Unterstützung für das Erstellen von Linux-Functions-Plänen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-991">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="b33c5-992">Möglichkeit zum Wechseln eines Plans unter einer Funktions-App mit `functionapp update --plan` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-992">Added ability to switch a plan underneath a function app using `functionapp update --plan`</span></span>
* <span data-ttu-id="b33c5-993">Unterstützung für Einstellungen zum horizontalen Hochskalieren für den Azure Functions-Premium-Plan hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-993">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="b33c5-994">CDN</span><span class="sxs-lookup"><span data-stu-id="b33c5-994">CDN</span></span>
* <span data-ttu-id="b33c5-995">Unterstützung hinzugefügt für `Microsoft_Standard` und `Standard_ChinaCdn`</span><span class="sxs-lookup"><span data-stu-id="b33c5-995">Added support for `Microsoft_Standard` and `Standard_ChinaCdn`</span></span>

### <a name="feedback"></a><span data-ttu-id="b33c5-996">Feedback</span><span class="sxs-lookup"><span data-stu-id="b33c5-996">Feedback</span></span>
* <span data-ttu-id="b33c5-997">`feedback` zur Anzeige von Metadaten zu den zuletzt ausgeführten Befehlen geändert</span><span class="sxs-lookup"><span data-stu-id="b33c5-997">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="b33c5-998">`feedback` geändert, um den Benutzer zur Unterstützung beim Issueerstellungsprozess aufzufordern (durch Öffnen eines Browsers und Verwenden einer Issuevorlage)</span><span class="sxs-lookup"><span data-stu-id="b33c5-998">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="b33c5-999">`feedback` geändert, um den Issuetext bei der Ausführung mit „--verbose“ auszugeben</span><span class="sxs-lookup"><span data-stu-id="b33c5-999">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="b33c5-1000">Überwachen</span><span class="sxs-lookup"><span data-stu-id="b33c5-1000">Monitor</span></span>
* <span data-ttu-id="b33c5-1001">Problem behoben, aufgrund dessen „Count“ kein zulässiger Wert für `metrics alert [create|update]` war</span><span class="sxs-lookup"><span data-stu-id="b33c5-1001">Fixed issue where "count" was not a permitted value with `metrics alert [create|update]`</span></span> 

### <a name="network"></a><span data-ttu-id="b33c5-1002">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="b33c5-1002">Network</span></span>
* <span data-ttu-id="b33c5-1003">Problem behoben, aufgrund dessen das Tabellenformat mit `vnet-gateway list-bgp-peer-status` nicht angezeigt wurde</span><span class="sxs-lookup"><span data-stu-id="b33c5-1003">Fixed table format not displaying with `vnet-gateway list-bgp-peer-status`</span></span>
* <span data-ttu-id="b33c5-1004">Befehle `list-request-headers` und `list-response-headers` zu `application-gateway rewrite-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1004">Added `list-request-headers` and `list-response-headers` commands to `application-gateway rewrite-rule`</span></span>
* <span data-ttu-id="b33c5-1005">Befehl `list-server-variables` zu `application-gateway rewrite-rule condition` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1005">Added `list-server-variables` command to `application-gateway rewrite-rule condition`</span></span>
* <span data-ttu-id="b33c5-1006">Problem behoben, aufgrund dessen durch das Aktualisieren des Linkstatus für einen ExpressRoute-Port eine Ausnahme vom Typ „unbekanntes Attribut“ ausgelöst wurde: `express-route port update`</span><span class="sxs-lookup"><span data-stu-id="b33c5-1006">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception `express-route port update`</span></span>

### <a name="privatedns"></a><span data-ttu-id="b33c5-1007">PrivateDNS</span><span class="sxs-lookup"><span data-stu-id="b33c5-1007">PrivateDNS</span></span>
* <span data-ttu-id="b33c5-1008">`network private-dns` für private DNS-Zonen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1008">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="b33c5-1009">Resource</span><span class="sxs-lookup"><span data-stu-id="b33c5-1009">Resource</span></span>
* <span data-ttu-id="b33c5-1010">Problem mit `deployment create` und `group deployment create` behoben, aufgrund dessen eine Parameterdatei mit leerem Parametersatz nicht verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="b33c5-1010">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="b33c5-1011">Role</span><span class="sxs-lookup"><span data-stu-id="b33c5-1011">Role</span></span>
* <span data-ttu-id="b33c5-1012">`create-for-rbac` korrigiert, um `--years` korrekt zu verarbeiten</span><span class="sxs-lookup"><span data-stu-id="b33c5-1012">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="b33c5-1013">[BREAKING CHANGE]`role assignment delete` geändert, um eine Eingabeaufforderung anzuzeigen, wenn alle Zuweisungen im Abonnement ohne Bedingungen gelöscht werden</span><span class="sxs-lookup"><span data-stu-id="b33c5-1013">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="b33c5-1014">SQL</span><span class="sxs-lookup"><span data-stu-id="b33c5-1014">SQL</span></span>
* <span data-ttu-id="b33c5-1015">`sql mi [create|update]` mit den Eigenschaften „proxyOverride“ und „publicDataEndpointEnabled“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-1015">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="b33c5-1016">Storage</span><span class="sxs-lookup"><span data-stu-id="b33c5-1016">Storage</span></span>
* <span data-ttu-id="b33c5-1017">[BREAKING CHANGE] Ergebnis von `storage blob delete` entfernt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1017">[BREAKING CHANGE] Removed result of `storage blob delete`</span></span>
* <span data-ttu-id="b33c5-1018">`--full-uri` zu `storage blob generate-sas` hinzugefügt, um den vollständigen URI für das Blob mit SAS zu erstellen</span><span class="sxs-lookup"><span data-stu-id="b33c5-1018">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="b33c5-1019">`--file-snapshot` zu `storage file copy start` hinzugefügt, um die Datei aus der Momentaufnahme zu kopieren</span><span class="sxs-lookup"><span data-stu-id="b33c5-1019">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="b33c5-1020">`storage blob copy cancel` geändert, um anstelle der Ausnahme für „NoPendingCopyOperation“ nur den Fehler anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="b33c5-1020">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="b33c5-1021">26. März 2019</span><span class="sxs-lookup"><span data-stu-id="b33c5-1021">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="b33c5-1022">Core</span><span class="sxs-lookup"><span data-stu-id="b33c5-1022">Core</span></span>
* <span data-ttu-id="b33c5-1023">Probleme mit der Inkompatibilität der Entwicklungserweiterung behoben</span><span class="sxs-lookup"><span data-stu-id="b33c5-1023">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="b33c5-1024">Die Fehlerbehandlung verweist Kunden jetzt auf die Problemseite.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1024">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="b33c5-1025">Cloud</span><span class="sxs-lookup"><span data-stu-id="b33c5-1025">Cloud</span></span>
* <span data-ttu-id="b33c5-1026">Fehler „Abonnement nicht gefunden“ in `cloud set` behoben</span><span class="sxs-lookup"><span data-stu-id="b33c5-1026">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="b33c5-1027">ACR</span><span class="sxs-lookup"><span data-stu-id="b33c5-1027">ACR</span></span>
* <span data-ttu-id="b33c5-1028">Redundante Quellen im Imageimport korrigiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-1028">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="b33c5-1029">`--auth-mode` wurde den Befehlen `acr build`, `acr run`, `acr task create` und `acr task update` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1029">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="b33c5-1030">Befehlsgruppe „acr task credential“ zum Verwalten von Anmeldeinformationen für eine Aufgabe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1030">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="b33c5-1031">„--no-wait“ zum Befehl `acr build` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1031">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="b33c5-1032">AppService</span><span class="sxs-lookup"><span data-stu-id="b33c5-1032">AppService</span></span>
* <span data-ttu-id="b33c5-1033">Problem behoben, das dazu führte, dass die Ausführung aus einem leeren Verzeichnis oder ein Szenario mit unbekannten Code von `webapp up` nicht korrekt behandelt wurde</span><span class="sxs-lookup"><span data-stu-id="b33c5-1033">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="b33c5-1034">Problem behoben, aufgrund dessen Slots für `[webapp|functionapp] config ssl bind` nicht verwendet werden konnten</span><span class="sxs-lookup"><span data-stu-id="b33c5-1034">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="b33c5-1035">Bot Service</span><span class="sxs-lookup"><span data-stu-id="b33c5-1035">BOT Service</span></span>
* <span data-ttu-id="b33c5-1036">`bot prepare-deploy` hinzugefügt, um die Bereitstellung von Bots über `webapp` vorzubereiten</span><span class="sxs-lookup"><span data-stu-id="b33c5-1036">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="b33c5-1037">`bot create --kind registration` geändert, um das Kennwort anzuzeigen, falls kein Kennwort angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="b33c5-1037">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="b33c5-1038">[BREAKING CHANGE]`--endpoint` wurde in `bot create --kind registration` geändert, sodass nun standardmäßig eine leere Zeichenfolge verwendet wird, anstatt eine Angabe zu erfordern.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1038">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="b33c5-1039">`SCM_DO_BUILD_DURING_DEPLOYMENT` zu den Anwendungseinstellungen der ARM-Vorlage für Web-App-Bot (v4) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1039">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="b33c5-1040">CDN</span><span class="sxs-lookup"><span data-stu-id="b33c5-1040">CDN</span></span>
* <span data-ttu-id="b33c5-1041">Unterstützung für `--no-wait` zu `cdn endpoint [create|update|start|stop|delete|load|purge]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1041">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* <span data-ttu-id="b33c5-1042">[BREAKING CHANGE] Das standardmäßige Zwischenspeicherverhalten für Abfragezeichenfolgen von `cdn endpoint create` wurde geändert.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1042">[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour.</span></span> <span data-ttu-id="b33c5-1043">Es wird nicht mehr standardmäßig „IgnoreQueryString“ festgelegt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1043">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="b33c5-1044">Er wird jetzt vom Dienst festgelegt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1044">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="b33c5-1045">Cosmosdb</span><span class="sxs-lookup"><span data-stu-id="b33c5-1045">Cosmosdb</span></span>
* <span data-ttu-id="b33c5-1046">Unterstützung für `--enable-multiple-write-locations` bei Kontoaktualisierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1046">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="b33c5-1047">Untergruppe `network-rule` mit Befehlen `add`, `remove` und `list` zum Verwalten von VNET-Regeln eines Cosmos DB-Kontos hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1047">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="b33c5-1048">Interactive</span><span class="sxs-lookup"><span data-stu-id="b33c5-1048">Interactive</span></span>
* <span data-ttu-id="b33c5-1049">Inkompatibilität mit der über azdev installierten interaktiven Erweiterung korrigiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-1049">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="b33c5-1050">Überwachen</span><span class="sxs-lookup"><span data-stu-id="b33c5-1050">Monitor</span></span>
* <span data-ttu-id="b33c5-1051">Geändert, sodass der Dimensionswert `*` für `monitor metrics alert [create|update]` zulässig ist</span><span class="sxs-lookup"><span data-stu-id="b33c5-1051">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="b33c5-1052">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="b33c5-1052">Network</span></span>
* <span data-ttu-id="b33c5-1053">Befehlsgruppe `rewrite-rule` zu `application-gateway` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1053">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="b33c5-1054">Profil</span><span class="sxs-lookup"><span data-stu-id="b33c5-1054">Profile</span></span>
* <span data-ttu-id="b33c5-1055">Kontounterstützung auf Mandantenebene für verwaltete Dienstidentität zu `login` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1055">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="b33c5-1056">Postgres</span><span class="sxs-lookup"><span data-stu-id="b33c5-1056">Postgres</span></span> 
* <span data-ttu-id="b33c5-1057">postgresql-Befehle vom Typ `replica` und Befehl `restart server` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1057">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="b33c5-1058">Änderungen vorgenommen, um den Standardspeicherort aus der Ressourcengruppe abzurufen, wenn er für die Erstellung von Servern nicht angegeben wurde, und um eine Überprüfung für die Aufbewahrungstage hinzuzufügen</span><span class="sxs-lookup"><span data-stu-id="b33c5-1058">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="b33c5-1059">Resource</span><span class="sxs-lookup"><span data-stu-id="b33c5-1059">Resource</span></span>
* <span data-ttu-id="b33c5-1060">Verbesserte Tabellenausgabe für `deployment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="b33c5-1060">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="b33c5-1061">Problem mit `deployment [create|validate]` behoben, aufgrund dessen der Typ „secureObject“ nicht erkannt wurde</span><span class="sxs-lookup"><span data-stu-id="b33c5-1061">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="b33c5-1062">Graph</span><span class="sxs-lookup"><span data-stu-id="b33c5-1062">Graph</span></span>
* <span data-ttu-id="b33c5-1063">Unterstützung für `--end-date` zu `ad [app|sp] credential reset` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1063">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="b33c5-1064">Unterstützung für das Hinzufügen von Berechtigungen mit `ad app permission add` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1064">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="b33c5-1065">Fehler mit `ad app permission list` behoben, wenn keine Berechtigungen vorlagen</span><span class="sxs-lookup"><span data-stu-id="b33c5-1065">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="b33c5-1066">Änderung an `ad sp delete` vorgenommen, um das Entfernen einer Rollenzuweisung zu überspringen, wenn das aktuelle Konto kein Abonnement enthält</span><span class="sxs-lookup"><span data-stu-id="b33c5-1066">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="b33c5-1067">`ad app create` geändert, sodass ohne Angabe für `--identifier-uris` standardmäßig eine leere Liste verwendet wird</span><span class="sxs-lookup"><span data-stu-id="b33c5-1067">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="b33c5-1068">storage</span><span class="sxs-lookup"><span data-stu-id="b33c5-1068">storage</span></span>
* <span data-ttu-id="b33c5-1069">`--snapshot` zu `storage file download-batch` für den Download von einer Freigabemomentaufnahme hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1069">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="b33c5-1070">Statusanzeige für `storage blob [download-batch|upload-batch]` geändert, damit sie weniger ausführlich dargestellt wird und das aktuelle Blob angibt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1070">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="b33c5-1071">Problem mit `storage account update` behoben, das beim Aktualisieren von Verschlüsselungsparametern auftrat</span><span class="sxs-lookup"><span data-stu-id="b33c5-1071">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="b33c5-1072">Problem behoben, bei dem für `storage blob show` ein Fehler auftrat, wenn oauth (`--auth-mode=login`) verwendet wurde</span><span class="sxs-lookup"><span data-stu-id="b33c5-1072">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="b33c5-1073">VM</span><span class="sxs-lookup"><span data-stu-id="b33c5-1073">VM</span></span>
* <span data-ttu-id="b33c5-1074">Befehl `image update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1074">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="b33c5-1075">12. März 2019</span><span class="sxs-lookup"><span data-stu-id="b33c5-1075">March 12, 2019</span></span>

<span data-ttu-id="b33c5-1076">Version 2.0.60</span><span class="sxs-lookup"><span data-stu-id="b33c5-1076">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="b33c5-1077">Core</span><span class="sxs-lookup"><span data-stu-id="b33c5-1077">Core</span></span>

* <span data-ttu-id="b33c5-1078">Falsche Fehlermeldung in `cloud set` zu nicht gefundenem Abonnement korrigiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-1078">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="b33c5-1079">ACR</span><span class="sxs-lookup"><span data-stu-id="b33c5-1079">ACR</span></span>

* <span data-ttu-id="b33c5-1080">Redundante Quellen im Imageimport korrigiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-1080">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="b33c5-1081">ACS</span><span class="sxs-lookup"><span data-stu-id="b33c5-1081">ACS</span></span>

* <span data-ttu-id="b33c5-1082">Änderung vorgenommen, um den Parameter `--listen-address` für `aks browse` zu ignorieren, wenn er nicht von kubectl unterstützt wird</span><span class="sxs-lookup"><span data-stu-id="b33c5-1082">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="b33c5-1083">AppService</span><span class="sxs-lookup"><span data-stu-id="b33c5-1083">AppService</span></span>

* <span data-ttu-id="b33c5-1084">`[webapp|functionapp] deployment list-publishing-credentials` hinzugefügt, um die Kudu-Veröffentlichungs-URL und die entsprechenden Anmeldeinformationen abzurufen</span><span class="sxs-lookup"><span data-stu-id="b33c5-1084">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="b33c5-1085">Fehlerhafte Ausgabeanweisung für `webapp auth update` entfernt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1085">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="b33c5-1086">`functionapp` korrigiert, um das korrekte Image für die Runtime in App Service-Plänen unter Linux festzulegen</span><span class="sxs-lookup"><span data-stu-id="b33c5-1086">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="b33c5-1087">Vorschau-Tag für `webapp up` entfernt und Verbesserungen am Befehl implementiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-1087">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="b33c5-1088">Botservice</span><span class="sxs-lookup"><span data-stu-id="b33c5-1088">Botservice</span></span>

* <span data-ttu-id="b33c5-1089">`SCM_DO_BUILD_DURING_DEPLOYMENT` zu den Anwendungseinstellungen der ARM-Vorlage für Web-App-Bot (v4) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1089">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="b33c5-1090">`Microsoft-BotFramework-AppId` und `Microsoft-BotFramework-AppPassword` zu den Anwendungseinstellungen der ARM-Vorlage für Web-App-Bot (v4) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1090">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="b33c5-1091">Einfache Anführungszeichen aus der Befehlsausgabe von `bot publish` am Ende von `bot create` entfernt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1091">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="b33c5-1092">`bot publish` wurde geändert und ist jetzt asynchron.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1092">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="b33c5-1093">Container</span><span class="sxs-lookup"><span data-stu-id="b33c5-1093">Container</span></span>

* <span data-ttu-id="b33c5-1094">Argument `--no-wait` zu `container [start|restart]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1094">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="b33c5-1095">EventHub</span><span class="sxs-lookup"><span data-stu-id="b33c5-1095">EventHub</span></span>

* <span data-ttu-id="b33c5-1096">Flag `--skip-empty-archives` zu `eventhub create|update` hinzugefügt, um leere Archive in der Aufzeichnung zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="b33c5-1096">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="b33c5-1097">Suchen</span><span class="sxs-lookup"><span data-stu-id="b33c5-1097">Find</span></span>

* <span data-ttu-id="b33c5-1098">Umfangreiches Funktionsupdate</span><span class="sxs-lookup"><span data-stu-id="b33c5-1098">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="b33c5-1099">HDInsight</span><span class="sxs-lookup"><span data-stu-id="b33c5-1099">HDInsight</span></span>

* <span data-ttu-id="b33c5-1100">Parameter `--storage-account-managed-identity` zu `hdinsight create` hinzugefügt, um MSI in ADLS Gen2 zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="b33c5-1100">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="b33c5-1101">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="b33c5-1101">Network</span></span>

* <span data-ttu-id="b33c5-1102">Problem mit `vpn-connection update` behoben, aufgrund dessen die Aktualisierung einer VPN-Verbindung zwischen Gateways in verschiedenen Abonnements fehlschlug</span><span class="sxs-lookup"><span data-stu-id="b33c5-1102">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="b33c5-1103">Rdbms</span><span class="sxs-lookup"><span data-stu-id="b33c5-1103">Rdbms</span></span>

* <span data-ttu-id="b33c5-1104">Kleinere Korrekturen, um den Standardspeicherort aus der Ressourcengruppe abzurufen, wenn er für die Erstellung von Servern nicht angegeben wurde, und um eine Überprüfung für die Aufbewahrungstage hinzuzufügen</span><span class="sxs-lookup"><span data-stu-id="b33c5-1104">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="b33c5-1105">Role</span><span class="sxs-lookup"><span data-stu-id="b33c5-1105">Role</span></span>

* <span data-ttu-id="b33c5-1106">`role definition update` wurde korrigiert und nutzt nun die ID, um die Definition korrekt aufzulösen.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1106">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="b33c5-1107">`ad app credential reset` geändert, um die Annahme zu entfernen, dass der Dienstprinzipal der App stets vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="b33c5-1107">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="b33c5-1108">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="b33c5-1108">Service Fabric</span></span>

* <span data-ttu-id="b33c5-1109">Das Problem, dass `sf cluster list` nicht wiederholbar war, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1109">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="b33c5-1110">26. Februar 2019</span><span class="sxs-lookup"><span data-stu-id="b33c5-1110">February 26, 2019</span></span>

<span data-ttu-id="b33c5-1111">Version 2.0.59</span><span class="sxs-lookup"><span data-stu-id="b33c5-1111">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="b33c5-1112">Core</span><span class="sxs-lookup"><span data-stu-id="b33c5-1112">Core</span></span>

* <span data-ttu-id="b33c5-1113">Problem behoben, aufgrund dessen die Verwendung von `--subscription NAME` in einigen Instanzen eine Ausnahme ausgelöst hat</span><span class="sxs-lookup"><span data-stu-id="b33c5-1113">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="b33c5-1114">ACR</span><span class="sxs-lookup"><span data-stu-id="b33c5-1114">ACR</span></span>

* <span data-ttu-id="b33c5-1115">Parameter `--target` für die Befehle `acr build`, `acr task create` und `acr task update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1115">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="b33c5-1116">Verbesserte Fehlerbehandlung für Runtimebefehle, wenn keine Anmeldung bei Azure besteht</span><span class="sxs-lookup"><span data-stu-id="b33c5-1116">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="b33c5-1117">ACS</span><span class="sxs-lookup"><span data-stu-id="b33c5-1117">ACS</span></span>

* <span data-ttu-id="b33c5-1118">Option `--listen-address` zu `aks port-forward` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1118">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="b33c5-1119">AppService</span><span class="sxs-lookup"><span data-stu-id="b33c5-1119">AppService</span></span>

* <span data-ttu-id="b33c5-1120">Befehl `functionapp devops-build` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1120">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="b33c5-1121">Batch</span><span class="sxs-lookup"><span data-stu-id="b33c5-1121">Batch</span></span>
* <span data-ttu-id="b33c5-1122">[BREAKING CHANGE] Befehl `batch pool upgrade os` entfernt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1122">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="b33c5-1123">[BREAKING CHANGE]`Pacakges`-Eigenschaft aus `Application`-Antworten entfernt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1123">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="b33c5-1124">Befehl `batch application package list` zum Auflisten von Paketen einer Anwendung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1124">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="b33c5-1125">[BREAKING CHANGE]`--application-id` in allen `batch application`-Befehlen in `--application-name` geändert</span><span class="sxs-lookup"><span data-stu-id="b33c5-1125">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="b33c5-1126">Argument `--json-file` für Befehle zum Anfordern der unformatierten API-Antwort hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1126">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="b33c5-1127">Validierung aktualisiert, sodass das `https://`-Element automatisch in alle Endpunkte aufgenommen wird, wenn es fehlt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1127">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="b33c5-1128">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="b33c5-1128">CosmosDB</span></span>

* <span data-ttu-id="b33c5-1129">Untergruppe `network-rule` mit Befehlen `add`, `remove` und `list` zum Verwalten von VNET-Regeln eines Cosmos DB-Kontos hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1129">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="b33c5-1130">Kusto</span><span class="sxs-lookup"><span data-stu-id="b33c5-1130">Kusto</span></span>

* <span data-ttu-id="b33c5-1131">[BREAKING CHANGE] Typen `hot_cache_period` und `soft_delete_period` für Datenbank in Format der Zeitspanne nach ISO8601 geändert</span><span class="sxs-lookup"><span data-stu-id="b33c5-1131">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="b33c5-1132">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="b33c5-1132">Network</span></span>

* <span data-ttu-id="b33c5-1133">Argument `--express-route-gateway-bypass` zu `vpn-connection [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1133">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="b33c5-1134">Befehlsgruppen aus `express-route`-Erweiterungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1134">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="b33c5-1135">Befehlsgruppen `express-route gateway` und `express-route port` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1135">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="b33c5-1136">Argument `--legacy-mode` zu `express-route peering [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1136">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="b33c5-1137">Argumente `--allow-classic-operations` und `--express-route-port` zu `express-route [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1137">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="b33c5-1138">Argument `--gateway-default-site` zu `vnet-gateway [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1138">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="b33c5-1139">Befehle vom Typ `ipsec-policy` zu `vnet-gateway` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1139">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="b33c5-1140">Resource</span><span class="sxs-lookup"><span data-stu-id="b33c5-1140">Resource</span></span>

* <span data-ttu-id="b33c5-1141">Problem mit `deployment create` behoben, aufgrund dessen beim Feld „Typ“ die Groß-/Kleinschreibung beachtet wurde</span><span class="sxs-lookup"><span data-stu-id="b33c5-1141">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="b33c5-1142">Unterstützung für URI-basierte Parameterdatei zu `policy assignment create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1142">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="b33c5-1143">Unterstützung für URI-basierte Parameter und Definitionen zu `policy set-definition update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1143">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="b33c5-1144">Verarbeitung von Parametern und Regeln für `policy definition update` korrigiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-1144">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="b33c5-1145">Problem mit `resource show/update/delete/tag/invoke-action` behoben, aufgrund dessen bei abonnementübergreifenden IDs die Abonnement-ID nicht ordnungsgemäß berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="b33c5-1145">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="b33c5-1146">Role</span><span class="sxs-lookup"><span data-stu-id="b33c5-1146">Role</span></span>

* <span data-ttu-id="b33c5-1147">Unterstützung für App-Rollen zu `ad app [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1147">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="b33c5-1148">VM</span><span class="sxs-lookup"><span data-stu-id="b33c5-1148">VM</span></span>

* <span data-ttu-id="b33c5-1149">Problem mit `vm create where ` behoben, aufgrund dessen der beschleunigte Netzwerkbetrieb für Ubuntu 18.0 nicht standardmäßig aktiviert war</span><span class="sxs-lookup"><span data-stu-id="b33c5-1149">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="b33c5-1150">12. Februar 2019</span><span class="sxs-lookup"><span data-stu-id="b33c5-1150">February 12, 2019</span></span>

<span data-ttu-id="b33c5-1151">Version 2.0.58</span><span class="sxs-lookup"><span data-stu-id="b33c5-1151">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="b33c5-1152">Core</span><span class="sxs-lookup"><span data-stu-id="b33c5-1152">Core</span></span>

* <span data-ttu-id="b33c5-1153">`az --version` zeigt jetzt eine Benachrichtigung an, wenn Sie Pakete haben, für die ein Update verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1153">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="b33c5-1154">Die Regression, dass `--ids` nicht mehr mit JSON-Ausgaben verwendet werden konnte, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1154">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="b33c5-1155">ACR</span><span class="sxs-lookup"><span data-stu-id="b33c5-1155">ACR</span></span>
* <span data-ttu-id="b33c5-1156">[BREAKING CHANGE] Die Befehlsgruppe `acr build-task` wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1156">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="b33c5-1157">[BREAKING CHANGE] Die Optionen `--tag` und `--manifest` wurden aus `acr repository delete` entfernt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1157">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="b33c5-1158">ACS</span><span class="sxs-lookup"><span data-stu-id="b33c5-1158">ACS</span></span>
* <span data-ttu-id="b33c5-1159">Unterstützung für Namen ohne Berücksichtigung von Groß-/Kleinschreibung wurde zu `aks [enable-addons|disable-addons]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1159">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="b33c5-1160">Unterstützung für Azure Active Directory-Aktualisierungsvorgang mithilfe von `aks update-credentials --reset-aad` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1160">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="b33c5-1161">Die Information, dass `--output` für `aks get-credentials` ignoriert wird, wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1161">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="b33c5-1162">AMS</span><span class="sxs-lookup"><span data-stu-id="b33c5-1162">AMS</span></span>
* <span data-ttu-id="b33c5-1163">Befehle vom Typ `ams streaming-endpoint [start | stop | create | update] wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1163">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="b33c5-1164">Befehle vom Typ `ams live-event [create | start | stop | reset] wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1164">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="b33c5-1165">AppService</span><span class="sxs-lookup"><span data-stu-id="b33c5-1165">Appservice</span></span>
* <span data-ttu-id="b33c5-1166">Die Möglichkeit zum Erstellen und Konfigurieren von Funktionen mithilfe von ACR-Containern wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1166">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="b33c5-1167">Unterstützung für das Aktualisieren von Web-App-Konfigurationen über JSON wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1167">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="b33c5-1168">Die Hilfe für `appservice-plan-update` wurde verbessert.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1168">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="b33c5-1169">Unterstützung für App-Erkenntnisse beim Erstellen von Funktions-Apps wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1169">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="b33c5-1170">Probleme mit der Web-App SSH wurden behoben.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1170">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="b33c5-1171">Botservice</span><span class="sxs-lookup"><span data-stu-id="b33c5-1171">Botservice</span></span>
* <span data-ttu-id="b33c5-1172">Die Benutzeroberfläche für `bot publish` wurde verbessert.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1172">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="b33c5-1173">Eine Warnung für Zeitlimit bei der Ausführung von `npm install` während `az bot publish` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1173">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="b33c5-1174">Ungültiges char-Element wurde `.` aus `--name` in `az bot create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1174">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="b33c5-1175">Eine Änderung wurde vorgenommen, um die zufällige Zuordnung von Ressourcennamen beim Erstellen von Azure Storage-Instanzen, App Service-Plänen, Funktions-/Web-Apps und Application Insights-Instanzen zu verhindern.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1175">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="b33c5-1176">[VERALTET] Argument `--proj-name` zugunsten von `--proj-file-path` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-1176">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="b33c5-1177">`az bot publish` wurde geändert, um abgerufene IIS-Bereitstellungsdateien vom Typ „Node.js“ zu entfernen, wenn sie nicht bereits vorhanden waren.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1177">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="b33c5-1178">Das `--keep-node-modules` Argument wurde zu `az bot publish` hinzugefügt, damit der Ordner `node_modules` in App Service nicht gelöscht wird.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1178">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="b33c5-1179">Das Schlüssel-Wert-Paar `"publishCommand"` wurde der Ausgabe von `az bot create` beim Erstellen einer Funktions-App oder eines Web-App-Bots hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1179">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="b33c5-1180">Der Wert von `"publishCommand"` ist ein `az bot publish`-Befehl, der bereits die erforderlichen Parameter zum Veröffentlichen des neu erstellten Bots enthält.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1180">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="b33c5-1181">`"WEBSITE_NODE_DEFAULT_VERSION"` in der ARM-Vorlage wurde so aktualisiert, dass v4-SDK-Bots 10.14.1 anstelle von 8.9.4 verwenden.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1181">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="b33c5-1182">Key Vault</span><span class="sxs-lookup"><span data-stu-id="b33c5-1182">Key Vault</span></span>
* <span data-ttu-id="b33c5-1183">Ein Problem mit `keyvault secret backup` wurde behoben, aufgrund dessen einige Benutzer bei Verwendung von `--id` einen `unexpected_keyword`-Fehler erhielten.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1183">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="b33c5-1184">Überwachen</span><span class="sxs-lookup"><span data-stu-id="b33c5-1184">Monitor</span></span>
* <span data-ttu-id="b33c5-1185">`monitor metrics alert [create|update]` wurde so geändert, dass der Dimensionswert `*` zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1185">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="b33c5-1186">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="b33c5-1186">Network</span></span>
* <span data-ttu-id="b33c5-1187">`dns zone export` wurde geändert, um sicherzustellen, dass es sich bei exportierten CNAMEs um FQDNs handelt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1187">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="b33c5-1188">Parameter `--gateway-name` wurde zu `nic ip-config address-pool [add|remove]` hinzugefügt, um Back-End-Adresspools von Anwendungsgateways zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1188">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="b33c5-1189">Argumente `--traffic-analytics` und `--workspace` wurden zu `network watcher flow-log configure` hinzugefügt, um Datenverkehrsanalysen über einen Log Analytics-Arbeitsbereich zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1189">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="b33c5-1190">`--idle-timeout` und `--floating-ip` wurden zu `lb inbound-nat-pool [create|update]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1190">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="b33c5-1191">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="b33c5-1191">Policy Insights</span></span>
* <span data-ttu-id="b33c5-1192">`policy remediation`-Befehle wurden hinzugefügt, um Korrekturfunktionen der Ressourcenrichtlinie zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1192">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="b33c5-1193">RDBMS</span><span class="sxs-lookup"><span data-stu-id="b33c5-1193">RDBMS</span></span>
* <span data-ttu-id="b33c5-1194">Hilfemeldung und Befehlsparameter wurden verbessert.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1194">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="b33c5-1195">Redis</span><span class="sxs-lookup"><span data-stu-id="b33c5-1195">Redis</span></span>
* <span data-ttu-id="b33c5-1196">Befehle zum Verwalten von „firewall-rules“ (erstellen, aktualisieren, löschen, anzeigen, auflisten) wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1196">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="b33c5-1197">Befehle zum Verwalten von „server-link“ (erstellen, aktualisieren, löschen, anzeigen, auflisten) wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1197">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="b33c5-1198">Befehle zum Verwalten von „patch-schedule“ (erstellen, aktualisieren, löschen, anzeigen, auflisten) wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1198">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="b33c5-1199">Unterstützung für Verfügbarkeitszonen und TLS-Mindestversion wurden zu „redis create“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1199">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="b33c5-1200">[BREAKING CHANGE] Befehle `redis update-settings` und `redis list-all` wurden entfernt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1200">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="b33c5-1201">[BREAKING CHANGE] Parameter für `redis create`: „Mandanteneinstellungen“ werden im Format „Schlüssel[=Wert] nicht akzeptiert.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1201">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="b33c5-1202">[VERALTET] Warnmeldung zur Markierung des Befehls `redis import-method` als veraltet hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1202">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="b33c5-1203">Role</span><span class="sxs-lookup"><span data-stu-id="b33c5-1203">Role</span></span>
* <span data-ttu-id="b33c5-1204">[BREAKING CHANGE] Befehl `az identity` wurde aus den `vm`-Befehlen hierher verschoben.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1204">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="b33c5-1205">SQL-VM</span><span class="sxs-lookup"><span data-stu-id="b33c5-1205">SQL VM</span></span>
* <span data-ttu-id="b33c5-1206">[VERALTET] Argument `--boostrap-acc-pwd` aufgrund eines Tippfehlers als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-1206">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="b33c5-1207">VM</span><span class="sxs-lookup"><span data-stu-id="b33c5-1207">VM</span></span>
* <span data-ttu-id="b33c5-1208">`vm list-skus` wurde so geändert, dass `--all` anstelle von `--all true` verwendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1208">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="b33c5-1209">`vmss run-command [invoke | list | show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1209">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="b33c5-1210">Ein Fehler wurde behoben, aufgrund dessen bei der Ausführung von `vmss encryption enable` bisher ein Fehler auftrat.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1210">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="b33c5-1211">[BREAKING CHANGE] Die Befehle vom Typ `az identity` wurden zu `role`-Befehlen verschoben.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1211">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="b33c5-1212">31. Januar 2019</span><span class="sxs-lookup"><span data-stu-id="b33c5-1212">January 31, 2019</span></span>

<span data-ttu-id="b33c5-1213">Version 2.0.57</span><span class="sxs-lookup"><span data-stu-id="b33c5-1213">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="b33c5-1214">Core</span><span class="sxs-lookup"><span data-stu-id="b33c5-1214">Core</span></span>

* <span data-ttu-id="b33c5-1215">Hotfix für [Problem 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="b33c5-1215">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="b33c5-1216">28. Januar 2019</span><span class="sxs-lookup"><span data-stu-id="b33c5-1216">January 28, 2019</span></span>

<span data-ttu-id="b33c5-1217">Version 2.0.56</span><span class="sxs-lookup"><span data-stu-id="b33c5-1217">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="b33c5-1218">ACR</span><span class="sxs-lookup"><span data-stu-id="b33c5-1218">ACR</span></span>
* <span data-ttu-id="b33c5-1219">Unterstützung für VNet/IP-Regeln wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1219">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="b33c5-1220">ACS</span><span class="sxs-lookup"><span data-stu-id="b33c5-1220">ACS</span></span>
* <span data-ttu-id="b33c5-1221">Virtuelle Knoten (Vorschau) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1221">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="b33c5-1222">Verwaltete OpenShift-Befehle wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1222">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="b33c5-1223">Unterstützung für den Dienstprinzipal-Updatevorgang mit `aks update-credentials -reset-service-principal` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1223">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="b33c5-1224">AMS</span><span class="sxs-lookup"><span data-stu-id="b33c5-1224">AMS</span></span>
* <span data-ttu-id="b33c5-1225">[BREAKING CHANGE]`ams asset get-streaming-locators` in `ams asset list-streaming-locators` umbenannt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1225">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="b33c5-1226">[BREAKING CHANGE]`ams streaming-locator get-content-keys` in `ams streaming-locator list-content-keys` umbenannt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1226">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="b33c5-1227">AppService</span><span class="sxs-lookup"><span data-stu-id="b33c5-1227">Appservice</span></span>
* <span data-ttu-id="b33c5-1228">Unterstützung für App-Erkenntnisse in `functionapp create` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1228">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="b33c5-1229">Unterstützung für die Erstellung von App Service-Plänen (einschließlich Elastic Premium) wurde zu Funktions-Apps hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1229">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="b33c5-1230">Probleme bei einer App-Einstellung mit Elastic Premium-Plänen wurden behoben.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1230">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="b33c5-1231">Container</span><span class="sxs-lookup"><span data-stu-id="b33c5-1231">Container</span></span>
* <span data-ttu-id="b33c5-1232">Befehl `container start` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1232">Added `container start` command</span></span>
* <span data-ttu-id="b33c5-1233">Eine Änderung wurde vorgenommen, um bei der Containererstellung die Verwendung von Dezimalwerten für die CPU zuzulassen.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1233">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="b33c5-1234">EventGrid</span><span class="sxs-lookup"><span data-stu-id="b33c5-1234">EventGrid</span></span>
* <span data-ttu-id="b33c5-1235">Parameter `--deadletter-endpoint` zu `event-subscription [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1235">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="b33c5-1236">„storagequeue“ und „hybridconnection“ wurden als neue Werte für „event-subscription [create|update] --endpoint-type“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1236">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="b33c5-1237">Parameter `--max-delivery-attempts` und `--event-ttl` wurden zu `event-subscription create` hinzugefügt, um die Wiederholungsrichtlinie für Ereignisse anzugeben.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1237">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="b33c5-1238">Eine Warnmeldung wurde zu `event-subscription [create|update]` hinzugefügt, wenn Webhook als Ziel für ein Ereignisabonnement verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1238">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="b33c5-1239">Parameter „source-resource-id“ wurde für alle Befehle im Zusammenhang mit Ereignisabonnements hinzugefügt, und alle anderen Parameter im Zusammenhang mit Quellressourcen wurden als veraltet markiert.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1239">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="b33c5-1240">HDInsight</span><span class="sxs-lookup"><span data-stu-id="b33c5-1240">HDInsight</span></span>
* <span data-ttu-id="b33c5-1241">[BREAKING CHANGE] Die Parameter `--virtual-network` und `--subnet-name` wurden aus `hdinsight [application] create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1241">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="b33c5-1242">[BREAKING CHANGE]`hdinsight create --storage-account` wurde so geändert, dass der Name oder die ID eines Speicherkontos anstellen von Blobendpunkten akzeptiert wird.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1242">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="b33c5-1243">Parameter `--vnet-name` und `--subnet-name` zu `hdinsight create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1243">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="b33c5-1244">Unterstützung für das Enterprise-Sicherheitspaket und Datenträgerverschlüsselung wurde zu `hdinsight create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1244">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="b33c5-1245">Befehl `hdinsight rotate-disk-encryption-key` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1245">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="b33c5-1246">Befehl `hdinsight update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1246">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="b33c5-1247">IoT</span><span class="sxs-lookup"><span data-stu-id="b33c5-1247">IoT</span></span>
* <span data-ttu-id="b33c5-1248">Codierungsformat wurde zu Befehl „routing-endpoint“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1248">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="b33c5-1249">Kusto</span><span class="sxs-lookup"><span data-stu-id="b33c5-1249">Kusto</span></span>
* <span data-ttu-id="b33c5-1250">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="b33c5-1250">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="b33c5-1251">Überwachen</span><span class="sxs-lookup"><span data-stu-id="b33c5-1251">Monitor</span></span>
* <span data-ttu-id="b33c5-1252">ID-Vergleich wurde so geändert, dass Groß-/Kleinschreibung nicht mehr beachtet wird.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1252">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="b33c5-1253">Profil</span><span class="sxs-lookup"><span data-stu-id="b33c5-1253">Profile</span></span>
* <span data-ttu-id="b33c5-1254">Konto auf Mandantenebene für verwaltete Dienstidentität für `login` wird aktiviert.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1254">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="b33c5-1255">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="b33c5-1255">Network</span></span>
* <span data-ttu-id="b33c5-1256">Ein Problem mit `express-route update` wurde behoben, aufgrund dessen das Argument `--bandwidth` ignoriert wurde.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1256">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="b33c5-1257">Ein Problem mit `ddos-protection update` wurde behoben, aufgrund dessen das festgelegte Verständnis zu einer Stapelüberwachung führte.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1257">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="b33c5-1258">Resource</span><span class="sxs-lookup"><span data-stu-id="b33c5-1258">Resource</span></span>
* <span data-ttu-id="b33c5-1259">Unterstützung für die URI-Parameterdatei wurde zu `group deployment create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1259">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="b33c5-1260">Unterstützung für verwaltete Identitäten wurde zu `policy assignment [create|list|show]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1260">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="b33c5-1261">Virtueller SQL-Computer</span><span class="sxs-lookup"><span data-stu-id="b33c5-1261">SQL Virtual Machine</span></span>
* <span data-ttu-id="b33c5-1262">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="b33c5-1262">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="b33c5-1263">Storage</span><span class="sxs-lookup"><span data-stu-id="b33c5-1263">Storage</span></span>
* <span data-ttu-id="b33c5-1264">Eine Lösung wurde so geändert, dass nur Eigenschaften aktualisiert werden, die im selben Objekt geändert werden.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1264">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="b33c5-1265">Nr. 8021 wurde korrigiert, Binärdaten werden bei der Rückgabe in Base64 codiert.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1265">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="b33c5-1266">VM</span><span class="sxs-lookup"><span data-stu-id="b33c5-1266">VM</span></span>
* <span data-ttu-id="b33c5-1267">`vm encryption enable` wurde geändert, um den Schlüsseltresor für die Datenträgerverschlüsselung zu überprüfen und sicherzustellen, dass der Schlüsseltresor für die Schlüsselverschlüsselung vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1267">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="b33c5-1268">Flag `--force` wurde zu `vm encryption enable` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1268">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="b33c5-1269">15. Januar 2019</span><span class="sxs-lookup"><span data-stu-id="b33c5-1269">January 15, 2019</span></span>

<span data-ttu-id="b33c5-1270">Version 2.0.55</span><span class="sxs-lookup"><span data-stu-id="b33c5-1270">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="b33c5-1271">ACR</span><span class="sxs-lookup"><span data-stu-id="b33c5-1271">ACR</span></span>
* <span data-ttu-id="b33c5-1272">Wurde geändert, um den Push eines nicht vorhandenen Helm-Diagramms zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1272">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="b33c5-1273">Wurde geändert, um Laufzeitvorgänge ohne ARM-Anforderungen zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1273">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="b33c5-1274">[VERALTET] Parameter `--resource-group` in folgenden Befehlen als veraltet markiert:</span><span class="sxs-lookup"><span data-stu-id="b33c5-1274">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="b33c5-1275">ACS</span><span class="sxs-lookup"><span data-stu-id="b33c5-1275">ACS</span></span>
* <span data-ttu-id="b33c5-1276">Unterstützung für neue ACI-Regionen wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1276">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="b33c5-1277">AppService</span><span class="sxs-lookup"><span data-stu-id="b33c5-1277">Appservice</span></span>
* <span data-ttu-id="b33c5-1278">Ein Problem beim Hochladen von Zertifikaten für in einer ASE gehostete Apps wurde behoben, aufgrund dessen die AS-RG und die App-RG nicht übereinstimmten.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1278">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="b33c5-1279">`webapp up` wurde geändert, sodass SKU P1V1 als Standard für Linux verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1279">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="b33c5-1280">`[webapp|functionapp] deployment source config-zip` wurde korrigiert, sodass beim Fehlschlagen einer Bereitstellung die richtige Fehlermeldung angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1280">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="b33c5-1281">Befehl `webapp ssh` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1281">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="b33c5-1282">Botservice</span><span class="sxs-lookup"><span data-stu-id="b33c5-1282">Botservice</span></span>
* <span data-ttu-id="b33c5-1283">Aktualisierungen des Bereitstellungsstatus wurden zu `bot create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1283">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="b33c5-1284">Konfigurieren</span><span class="sxs-lookup"><span data-stu-id="b33c5-1284">Configure</span></span>
* <span data-ttu-id="b33c5-1285">`none` wurde als konfigurierbares Ausgabeformat hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1285">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="b33c5-1286">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="b33c5-1286">CosmosDB</span></span>
* <span data-ttu-id="b33c5-1287">Unterstützung für das Erstellen einer Datenbank mit gemeinsam genutztem Durchsatz wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1287">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="b33c5-1288">HDInsight</span><span class="sxs-lookup"><span data-stu-id="b33c5-1288">HDInsight</span></span>
* <span data-ttu-id="b33c5-1289">Befehle zum Verwalten von Anwendungen wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1289">Added commands for managing applications</span></span>
* <span data-ttu-id="b33c5-1290">Befehle zum Verwalten von Skriptaktionen wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1290">Added commands for managing script actions</span></span>
* <span data-ttu-id="b33c5-1291">Befehle zum Verwalten von der Operations Management Suite (OMS) wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1291">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="b33c5-1292">Unterstützung zum Auflisten der regionalen Nutzung wurde zu `hdinsight list-usage` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1292">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="b33c5-1293">[BREAKING CHANGE] Standardclustertyp wurde aus `hdinsight create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1293">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="b33c5-1294">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="b33c5-1294">Network</span></span>
* <span data-ttu-id="b33c5-1295">Argumente `--custom-headers` und `--status-code-ranges` zu `traffic-manager profile [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1295">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="b33c5-1296">Neue Routingtypen wurden hinzugefügt: Subnetz und MultiValue</span><span class="sxs-lookup"><span data-stu-id="b33c5-1296">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="b33c5-1297">Argumente `--custom-headers` und `--subnets` zu `traffic-manager endpoint [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1297">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="b33c5-1298">Eine Problem wurde behoben, aufgrund dessen die Angabe von `--vnets ""` für `ddos-protection update` einen Fehler verursacht hat.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1298">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="b33c5-1299">Role</span><span class="sxs-lookup"><span data-stu-id="b33c5-1299">Role</span></span>
* <span data-ttu-id="b33c5-1300">[VERALTET] Argument `--password` als veraltet markiert für `create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1300">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="b33c5-1301">Verwenden Sie stattdessen sichere, von der CLI generierte Kennwörter.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1301">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="b33c5-1302">Sicherheit</span><span class="sxs-lookup"><span data-stu-id="b33c5-1302">Security</span></span>
* <span data-ttu-id="b33c5-1303">Erstrelease</span><span class="sxs-lookup"><span data-stu-id="b33c5-1303">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="b33c5-1304">Storage</span><span class="sxs-lookup"><span data-stu-id="b33c5-1304">Storage</span></span>
* <span data-ttu-id="b33c5-1305">[BREAKING CHANGE] Die Standardanzahl von Ergebnissen wurde für `storage [blob|file|container|share] list` in 5.000 geändert.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1305">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="b33c5-1306">Verwenden Sie `--num-results *` für das ursprüngliche Verhalten, alle Ergebnisse zurückzugeben.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1306">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="b33c5-1307">Parameter `--marker` zu `storage [blob|file|container|share] list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1307">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="b33c5-1308">Ein Protokollmarker für die nächste Seite wurde zur STDERR für `storage [blob|file|container|share] list` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1308">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="b33c5-1309">Der Befehl `storage blob service-properties update` mit Unterstützung für statische Websites wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1309">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="b33c5-1310">VM</span><span class="sxs-lookup"><span data-stu-id="b33c5-1310">VM</span></span>
* <span data-ttu-id="b33c5-1311">`vm [disk|unmanaged-disk]` und `vmss disk` wurden geändert, sodass sie konsistentere Parameter enthalten.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1311">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="b33c5-1312">Unterstützung für mandantenübergreifende Imageverweise wurden zu `[vm|vmss] create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1312">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="b33c5-1313">Fehler bei Standardkonfiguration in `vm diagnostics get-default-config --windows-os` wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1313">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="b33c5-1314">Argument `--provision-after-extensions` wurde zu `vmss extension set` hinzugefügt, um zu definieren, welche Erweiterungen vor dem Festlegen der Erweiterung bereitgestellt werden müssen.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1314">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="b33c5-1315">Argument `--replica-count` wurde zu `sig image-version update` hinzugefügt, um die Standardanzahl für die Replikation festzulegen.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1315">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="b33c5-1316">Fehler bei `image create --source` wurde behoben, aufgrund dessen, der Quellbetriebssystem-Datenträger für einen virtuellen Computer mit dem gleichen Namen gehalten wurde, selbst wenn die vollständige Ressourcen-ID angegeben war.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1316">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="b33c5-1317">20. Dezember 2018</span><span class="sxs-lookup"><span data-stu-id="b33c5-1317">December 20, 2018</span></span>

<span data-ttu-id="b33c5-1318">Version 2.0.54</span><span class="sxs-lookup"><span data-stu-id="b33c5-1318">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="b33c5-1319">AppService</span><span class="sxs-lookup"><span data-stu-id="b33c5-1319">Appservice</span></span>
* <span data-ttu-id="b33c5-1320">Problem behoben, bei dem `webapp up` nicht erneut bereitgestellt werden konnte</span><span class="sxs-lookup"><span data-stu-id="b33c5-1320">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="b33c5-1321">Unterstützung für das Auflisten und Wiederherstellen von Web-App-Momentaufnahmen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1321">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="b33c5-1322">Unterstützung für das Flag `--runtime` zu Windows-Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1322">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="b33c5-1323">IoTCentral</span><span class="sxs-lookup"><span data-stu-id="b33c5-1323">IoTCentral</span></span>
* <span data-ttu-id="b33c5-1324">Fehler bei API-Aufruf für update-Befehl behoben</span><span class="sxs-lookup"><span data-stu-id="b33c5-1324">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="b33c5-1325">Role</span><span class="sxs-lookup"><span data-stu-id="b33c5-1325">Role</span></span>
* <span data-ttu-id="b33c5-1326">[BREAKING CHANGE]`ad [app|sp] list` geändert, damit standardmäßig nur die ersten 100 Objekte aufgelistet werden</span><span class="sxs-lookup"><span data-stu-id="b33c5-1326">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="b33c5-1327">SQL</span><span class="sxs-lookup"><span data-stu-id="b33c5-1327">SQL</span></span>
* <span data-ttu-id="b33c5-1328">Unterstützung für die benutzerdefinierte Sortierung auf verwalteten Instanzen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1328">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="b33c5-1329">VM</span><span class="sxs-lookup"><span data-stu-id="b33c5-1329">VM</span></span>
* <span data-ttu-id="b33c5-1330">Parameter `---os-type` zu `disk create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1330">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="b33c5-1331">18. Dezember 2018</span><span class="sxs-lookup"><span data-stu-id="b33c5-1331">December 18, 2018</span></span>

<span data-ttu-id="b33c5-1332">Version 2.0.53</span><span class="sxs-lookup"><span data-stu-id="b33c5-1332">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="b33c5-1333">ACR</span><span class="sxs-lookup"><span data-stu-id="b33c5-1333">ACR</span></span>
* <span data-ttu-id="b33c5-1334">Unterstützung für Imageimport aus externen Containerregistrierungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1334">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="b33c5-1335">Tabellenlayout für Aufgabenliste komprimiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-1335">Condensed the table layout for task list</span></span>
* <span data-ttu-id="b33c5-1336">Unterstützung für Azure DevOps-URLs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1336">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="b33c5-1337">ACS</span><span class="sxs-lookup"><span data-stu-id="b33c5-1337">ACS</span></span>
* <span data-ttu-id="b33c5-1338">Virtuelle Knoten (Vorschau) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1338">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="b33c5-1339">„(PREVIEW)“ aus AAD-Argumenten für `aks create` entfernt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1339">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="b33c5-1340">[VERALTET]`az acs`-Befehle als veraltet markiert.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1340">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="b33c5-1341">ACS wird am 31. Januar 2020 eingestellt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1341">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="b33c5-1342">Unterstützung für Netzwerkrichtlinie bei der Erstellung neuer AKS-Cluster hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1342">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="b33c5-1343">Anforderung des Arguments `--nodepool-name` bei nur einem Knotenpool für `aks scale` entfernt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1343">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="b33c5-1344">AppService</span><span class="sxs-lookup"><span data-stu-id="b33c5-1344">Appservice</span></span>
* <span data-ttu-id="b33c5-1345">Problem behoben, bei dem für `webapp config container` der Parameter `--slot` nicht berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="b33c5-1345">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="b33c5-1346">Botservice</span><span class="sxs-lookup"><span data-stu-id="b33c5-1346">Botservice</span></span>
* <span data-ttu-id="b33c5-1347">Unterstützung für Analyse von `.bot`-Dateien beim Aufrufen von `bot show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1347">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="b33c5-1348">Fehler bei der AppInsights-Bereitstellung behoben</span><span class="sxs-lookup"><span data-stu-id="b33c5-1348">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="b33c5-1349">Leerzeichenfehler bei Dateipfaden behoben</span><span class="sxs-lookup"><span data-stu-id="b33c5-1349">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="b33c5-1350">Kudu-Netzwerkaufrufe reduziert</span><span class="sxs-lookup"><span data-stu-id="b33c5-1350">Reduced Kudu network calls</span></span>
* <span data-ttu-id="b33c5-1351">Allgemeine Verbesserungen bei Befehlen der Benutzeroberfläche durchgeführt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1351">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="b33c5-1352">Nutzung</span><span class="sxs-lookup"><span data-stu-id="b33c5-1352">Consumption</span></span>
* <span data-ttu-id="b33c5-1353">Fehler für Budget-API zum Anzeigen von Benachrichtigungen behoben</span><span class="sxs-lookup"><span data-stu-id="b33c5-1353">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="b33c5-1354">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="b33c5-1354">CosmosDB</span></span>
* <span data-ttu-id="b33c5-1355">Unterstützung für die Aktualisierung des Kontos von „Singlemaster“ auf „Multimaster“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1355">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="b33c5-1356">Karten</span><span class="sxs-lookup"><span data-stu-id="b33c5-1356">Maps</span></span>
* <span data-ttu-id="b33c5-1357">Unterstützung für SKU „S1“ für `maps account [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1357">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="b33c5-1358">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="b33c5-1358">Network</span></span>
* <span data-ttu-id="b33c5-1359">Unterstützung für `--format` und `--log-version` für `watcher flow-log configure` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1359">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="b33c5-1360">Problem mit `dns zone update` behoben, bei dem die Verwendung von "" zum Löschen von Auflösungs- und Registrierungs-VNETs nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="b33c5-1360">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="b33c5-1361">Resource</span><span class="sxs-lookup"><span data-stu-id="b33c5-1361">Resource</span></span>
* <span data-ttu-id="b33c5-1362">Verarbeitung des Bereichsparameters für Verwaltungsgruppen in `policy assignment [create|list|delete|show|update]` behoben</span><span class="sxs-lookup"><span data-stu-id="b33c5-1362">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="b33c5-1363">Neuen Befehl `resource wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1363">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="b33c5-1364">Storage</span><span class="sxs-lookup"><span data-stu-id="b33c5-1364">Storage</span></span>
*  <span data-ttu-id="b33c5-1365">Möglichkeit zum Aktualisieren der Protokollschemaversion für Speicherdienste in `storage logging update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1365">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="b33c5-1366">VM</span><span class="sxs-lookup"><span data-stu-id="b33c5-1366">VM</span></span>
* <span data-ttu-id="b33c5-1367">Absturz in `vm identity remove` behoben, der aufgetreten ist, wenn der angegebenen VM keine verwalteten Dienstidentitäten zugewiesen waren</span><span class="sxs-lookup"><span data-stu-id="b33c5-1367">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="b33c5-1368">4\. Dezember 2018</span><span class="sxs-lookup"><span data-stu-id="b33c5-1368">December 4, 2018</span></span>

<span data-ttu-id="b33c5-1369">Version 2.0.52</span><span class="sxs-lookup"><span data-stu-id="b33c5-1369">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="b33c5-1370">Core</span><span class="sxs-lookup"><span data-stu-id="b33c5-1370">Core</span></span>
* <span data-ttu-id="b33c5-1371">Unterstützung für mandantenübergreifende Ressourcenbereitstellung für mehrinstanzenfähigen Dienstprinzipal hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1371">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="b33c5-1372">Behebung eines Fehlers, aufgrund dessen IDs, die von einem Befehl mit Ausgabe im TSV-Format weitergeleitet wurden, nicht ordnungsgemäß analysiert wurden</span><span class="sxs-lookup"><span data-stu-id="b33c5-1372">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="b33c5-1373">AppService</span><span class="sxs-lookup"><span data-stu-id="b33c5-1373">Appservice</span></span>
* <span data-ttu-id="b33c5-1374">[VORSCHAU] Befehl `webapp up` hinzugefügt, der Benutzer beim Erstellen und Bereitstellen von Inhalten in Apps unterstützt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1374">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="b33c5-1375">Behebung eines Fehlers in einer containerbasierten Windows-App, der aufgrund einer Back-End-Änderung auftrat</span><span class="sxs-lookup"><span data-stu-id="b33c5-1375">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="b33c5-1376">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="b33c5-1376">Network</span></span>
* <span data-ttu-id="b33c5-1377">Argument `--exclusion` zu `application-gateway waf-config set` hinzugefügt, um WAF-Ausschlüsse zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="b33c5-1377">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="b33c5-1378">Role</span><span class="sxs-lookup"><span data-stu-id="b33c5-1378">Role</span></span>
* <span data-ttu-id="b33c5-1379">Unterstützung für benutzerdefinierte Bezeichner für Kennwortanmeldeinformation hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1379">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="b33c5-1380">VM</span><span class="sxs-lookup"><span data-stu-id="b33c5-1380">VM</span></span>
* <span data-ttu-id="b33c5-1381">[VERALTET] Parameter `vm extension [show|wait] --expand` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-1381">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="b33c5-1382">Parameter `--force` zu `vm restart` hinzugefügt, um nicht reagierende virtuelle Computer erneut bereitzustellen</span><span class="sxs-lookup"><span data-stu-id="b33c5-1382">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="b33c5-1383">`[vm|vmss] create --authentication-type` geändert, um „all“ zu akzeptieren und einen virtuellen Computer mit Kennwort- und SSH-Authentifizierung zu erstellen</span><span class="sxs-lookup"><span data-stu-id="b33c5-1383">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="b33c5-1384">Parameter `image create --os-disk-caching` hinzugefügt, um die Zwischenspeicherung von Betriebssystemdatenträgern für ein Image festzulegen</span><span class="sxs-lookup"><span data-stu-id="b33c5-1384">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="b33c5-1385">20. November 2018</span><span class="sxs-lookup"><span data-stu-id="b33c5-1385">November 20, 2018</span></span>

<span data-ttu-id="b33c5-1386">Version 2.0.51</span><span class="sxs-lookup"><span data-stu-id="b33c5-1386">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="b33c5-1387">Core</span><span class="sxs-lookup"><span data-stu-id="b33c5-1387">Core</span></span>
* <span data-ttu-id="b33c5-1388">MSI-Anmeldung geändert, sodass der Abonnementname nicht in der Identität wiederverwendet wird</span><span class="sxs-lookup"><span data-stu-id="b33c5-1388">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="b33c5-1389">ACR</span><span class="sxs-lookup"><span data-stu-id="b33c5-1389">ACR</span></span>
* <span data-ttu-id="b33c5-1390">Kontexttoken zum Aufgabenschritt hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1390">Added context token to task step</span></span>
* <span data-ttu-id="b33c5-1391">Unterstützung für das Festlegen von Geheimnissen in „acr run“ zum Spiegeln der ACR-Aufgabe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1391">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="b33c5-1392">Unterstützung für `--top` und `--orderby` für die Befehle `show-tags` und `show-manifests` verbessert</span><span class="sxs-lookup"><span data-stu-id="b33c5-1392">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="b33c5-1393">AppService</span><span class="sxs-lookup"><span data-stu-id="b33c5-1393">Appservice</span></span>
* <span data-ttu-id="b33c5-1394">Standardtimeout der ZIP-Bereitstellung für das Abrufen des Status auf fünf Minuten erhöht und Timeout-Eigenschaft zum Anpassen dieses Werts hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1394">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="b33c5-1395">Aktualisierung der standardmäßigen `node_version`.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1395">Updated the default `node_version`.</span></span> <span data-ttu-id="b33c5-1396">Während eines Austauschvorgangs mit zwei Phasen werden bei der Austauschaktion zum Zurücksetzen des Slots alle App-Einstellungen und Verbindungszeichenfolgen beibehalten.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1396">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="b33c5-1397">Clientseitige SKU-Überprüfung für die Erstellung eines Linux-App Service-Plans entfernt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1397">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="b33c5-1398">Behebung eines Fehlers beim Abrufen des ZipDeploy-Status</span><span class="sxs-lookup"><span data-stu-id="b33c5-1398">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="b33c5-1399">IotCentral</span><span class="sxs-lookup"><span data-stu-id="b33c5-1399">IotCentral</span></span>
* <span data-ttu-id="b33c5-1400">Verfügbarkeitsprüfung für Unterdomänen beim Erstellen einer IoT Central-Anwendung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1400">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="b33c5-1401">KeyVault</span><span class="sxs-lookup"><span data-stu-id="b33c5-1401">KeyVault</span></span>
* <span data-ttu-id="b33c5-1402">Behebung eines Fehlers, aufgrund dessen Fehler mitunter ignoriert wurden</span><span class="sxs-lookup"><span data-stu-id="b33c5-1402">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="b33c5-1403">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="b33c5-1403">Network</span></span>
* <span data-ttu-id="b33c5-1404">`root-cert`-Unterbefehle zum Behandeln von vertrauenswürdigen Stammzertifikaten zu `application-gateway` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1404">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="b33c5-1405">Optionen `--min-capacity` und `--custom-error-pages` zu `application-gateway [create|update]` hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="b33c5-1405">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="b33c5-1406">`--zones` zur Unterstützung von Verfügbarkeitszonen zu `application-gateway create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1406">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="b33c5-1407">Argumente `--file-upload-limit`, `--max-request-body-size` und `--request-body-check` zu `application-gateway waf-config set` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1407">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="b33c5-1408">Rdbms</span><span class="sxs-lookup"><span data-stu-id="b33c5-1408">Rdbms</span></span>
* <span data-ttu-id="b33c5-1409">MariaDB-VNET-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1409">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="b33c5-1410">RBAC</span><span class="sxs-lookup"><span data-stu-id="b33c5-1410">Rbac</span></span>
* <span data-ttu-id="b33c5-1411">Problem beim Aktualisieren unveränderlicher Anmeldeinformationen in `ad app update` behoben</span><span class="sxs-lookup"><span data-stu-id="b33c5-1411">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="b33c5-1412">Ausgabewarnungen zur Ankündigung bevorstehender Breaking Changes für `ad [app|sp] list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1412">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="b33c5-1413">Storage</span><span class="sxs-lookup"><span data-stu-id="b33c5-1413">Storage</span></span>
* <span data-ttu-id="b33c5-1414">Behandlung von Ausnahmefällen für Speicherkopierbefehle verbessert</span><span class="sxs-lookup"><span data-stu-id="b33c5-1414">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="b33c5-1415">Problem behoben, aufgrund dessen `storage blob copy start-batch` bei identischen Ziel- und Quellkonten keine Anmeldeinformationen verwendete</span><span class="sxs-lookup"><span data-stu-id="b33c5-1415">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="b33c5-1416">Fehler bei `storage [blob|file] url` behoben, aufgrund dessen `sas_token` nicht in die URL eingebunden wurde</span><span class="sxs-lookup"><span data-stu-id="b33c5-1416">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="b33c5-1417">Breaking Change-Warnung zu `[blob|container] list` hinzugefügt: In Kürze werden standardmäßig nur die ersten 5.000 Ergebnisse ausgegeben.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1417">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="b33c5-1418">VM</span><span class="sxs-lookup"><span data-stu-id="b33c5-1418">VM</span></span>
* <span data-ttu-id="b33c5-1419">Unterstützung für die separate Angabe einer Speicherkonto-SKU für verwaltete Betriebssystemdatenträger und Datenträger zu `[vm|vmss] create --storage-sku` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1419">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="b33c5-1420">Parameter für den Versionsnamen von `sig image-version` in `--image-version -e` geändert</span><span class="sxs-lookup"><span data-stu-id="b33c5-1420">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="b33c5-1421">`sig image-version`-Argument `--image-version-name` als veraltet markiert und durch `--image-version` ersetzt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1421">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="b33c5-1422">Unterstützung für die Verwendung des lokalen Betriebssystemdatenträgers für `[vm|vmss] create --ephemeral-os-disk` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1422">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="b33c5-1423">Unterstützung für `--no-wait` zu `snapshot create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1423">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="b33c5-1424">Befehl `snapshot wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1424">Added `snapshot wait` command</span></span>
* <span data-ttu-id="b33c5-1425">Unterstützung für die Verwendung von Instanznamen mit `[vm|vmss] extension set --extension-instance-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1425">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="b33c5-1426">6\. November 2018</span><span class="sxs-lookup"><span data-stu-id="b33c5-1426">November 6, 2018</span></span>

<span data-ttu-id="b33c5-1427">Version 2.0.50</span><span class="sxs-lookup"><span data-stu-id="b33c5-1427">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="b33c5-1428">Core</span><span class="sxs-lookup"><span data-stu-id="b33c5-1428">Core</span></span>
* <span data-ttu-id="b33c5-1429">Unterstützung für die Dienstprinzipalauthentifizierung (SN und Aussteller) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1429">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="b33c5-1430">ACR</span><span class="sxs-lookup"><span data-stu-id="b33c5-1430">ACR</span></span>
* <span data-ttu-id="b33c5-1431">Unterstützung für Commit- und Pull Request-Git-Ereignisse für Aufgabenquellentrigger hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1431">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="b33c5-1432">Auf Verwendung des Standard-Dockerfiles umgestellt, falls im Erstellungsbefehl kein Dockerfile angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="b33c5-1432">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="b33c5-1433">ACS</span><span class="sxs-lookup"><span data-stu-id="b33c5-1433">ACS</span></span>
* <span data-ttu-id="b33c5-1434">[BREAKING CHANGE]`enable_cloud_console_aks_browse` entfernt, um standardmäßig „az aks browse“ zu aktivieren</span><span class="sxs-lookup"><span data-stu-id="b33c5-1434">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="b33c5-1435">Advisor</span><span class="sxs-lookup"><span data-stu-id="b33c5-1435">Advisor</span></span>
* <span data-ttu-id="b33c5-1436">Allgemein verfügbares Release</span><span class="sxs-lookup"><span data-stu-id="b33c5-1436">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="b33c5-1437">AMS</span><span class="sxs-lookup"><span data-stu-id="b33c5-1437">AMS</span></span>
* <span data-ttu-id="b33c5-1438">Neue Befehlsgruppen hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="b33c5-1438">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="b33c5-1439">Neue Befehle hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="b33c5-1439">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="b33c5-1440">Unterstützung von Verschlüsselungsparametern für `ams streaming-policy create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1440">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="b33c5-1441">Für `ams transform output remove` kann jetzt der zu entfernende Ausgabeindex angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1441">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="b33c5-1442">Argumente `--correlation-data` und `--label` zur Befehlsgruppe `ams job` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1442">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="b33c5-1443">Argumente `--storage-account` und `--container` zur Befehlsgruppe `ams asset` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1443">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="b33c5-1444">Standardwerte für Ablaufzeit (aktueller Zeitpunkt + 23 Std.) und Berechtigungen (Lesen) im Befehl `ams asset get-sas-url` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1444">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="b33c5-1445">[BREAKING CHANGE] Befehl `ams streaming locator` durch `ams streaming-locator` ersetzt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1445">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="b33c5-1446">[BREAKING CHANGE] Argument `--content-keys` von `ams streaming locator` aktualisiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-1446">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="b33c5-1447">[BREAKING CHANGE]`--content-policy-name` im Befehl `ams streaming locator` in `--content-key-policy-name` umbenannt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1447">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="b33c5-1448">[BREAKING CHANGE] Befehl `ams streaming policy` durch `ams streaming-policy` ersetzt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1448">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="b33c5-1449">[BREAKING CHANGE] Das Argument `--preset-names` wurde in der Befehlsgruppe `--preset` durch `ams transform` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1449">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="b33c5-1450">Ab sofort kann nur noch eine einzelne Ausgabe/Voreinstellung festgelegt werden. (Wenn Sie weitere hinzufügen möchten, müssen Sie `ams transform output add` ausführen.)</span><span class="sxs-lookup"><span data-stu-id="b33c5-1450">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="b33c5-1451">Darüber hinaus können Sie eine benutzerdefinierte Voreinstellung für den Standard-Encoder (StandardEncoderPreset) festlegen, indem Sie den Pfad an Ihr benutzerdefiniertes JSON-Objekt übergeben.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1451">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="b33c5-1452">[BREAKING CHANGE]`--output-asset-names ` wurde im Befehl `ams job start` in `--output-assets` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1452">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="b33c5-1453">Ab sofort wird eine durch Leerzeichen getrennte Ressourcenliste im Format „assetName=Bezeichnung“ akzeptiert.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1453">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="b33c5-1454">Ressourcen ohne Bezeichnung können wie folgt gesendet werden: „assetName=“.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1454">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="b33c5-1455">AppService</span><span class="sxs-lookup"><span data-stu-id="b33c5-1455">AppService</span></span>
* <span data-ttu-id="b33c5-1456">Fehler in `az webapp config backup update` behoben, der dazu führte, dass kein Sicherungszeitplan festgelegt werden konnte, wenn noch keiner festgelegt war</span><span class="sxs-lookup"><span data-stu-id="b33c5-1456">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="b33c5-1457">Konfigurieren</span><span class="sxs-lookup"><span data-stu-id="b33c5-1457">Configure</span></span>
* <span data-ttu-id="b33c5-1458">YAML zu Ausgabeformatoptionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1458">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="b33c5-1459">Container</span><span class="sxs-lookup"><span data-stu-id="b33c5-1459">Container</span></span>
* <span data-ttu-id="b33c5-1460">Auf Anzeige der Identität umgestellt, wenn eine Containergruppe nach YAML exportiert wird</span><span class="sxs-lookup"><span data-stu-id="b33c5-1460">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="b33c5-1461">EventHub</span><span class="sxs-lookup"><span data-stu-id="b33c5-1461">EventHub</span></span>
* <span data-ttu-id="b33c5-1462">Flag `--enable-kafka` hinzugefügt, um Kafka in `eventhub namespace [create|update]` zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="b33c5-1462">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="b33c5-1463">Interactive</span><span class="sxs-lookup"><span data-stu-id="b33c5-1463">Interactive</span></span>
* <span data-ttu-id="b33c5-1464">Interactive installiert nun die Erweiterung `interactive`, um schnellere Updates und schnelleren Support zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="b33c5-1464">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="b33c5-1465">Überwachen</span><span class="sxs-lookup"><span data-stu-id="b33c5-1465">Monitor</span></span>
* <span data-ttu-id="b33c5-1466">Unterstützung für Metriknamen mit Schrägstrichen und Punkten zu `--condition` in `monitor metrics alert [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1466">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="b33c5-1467">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="b33c5-1467">Network</span></span>
* <span data-ttu-id="b33c5-1468">Befehlsnamen vom Typ `network interface-endpoint` zugunsten von `network private-endpoint` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-1468">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="b33c5-1469">Problem behoben, das dazu führte, dass das Argument `--peer-circuit` in `express-route peering connection create` keine ID akzeptiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-1469">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="b33c5-1470">Problem behoben, das dazu führte, dass `--ip-tags` mit `public-ip create` nicht ordnungsgemäß funktioniert</span><span class="sxs-lookup"><span data-stu-id="b33c5-1470">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="b33c5-1471">Profil</span><span class="sxs-lookup"><span data-stu-id="b33c5-1471">Profile</span></span>
* <span data-ttu-id="b33c5-1472">`--use-cert-sn-issuer` zu `az login` hinzugefügt, um Dienstprinzipalanmeldungen mit automatischem Zertifikatrollover zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="b33c5-1472">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="b33c5-1473">RDBMS</span><span class="sxs-lookup"><span data-stu-id="b33c5-1473">RDBMS</span></span>
* <span data-ttu-id="b33c5-1474">MySQL-Replikatbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1474">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="b33c5-1475">Resource</span><span class="sxs-lookup"><span data-stu-id="b33c5-1475">Resource</span></span>
* <span data-ttu-id="b33c5-1476">Unterstützung für Verwaltungsgruppen und Abonnements zu Befehlen vom Typ `policy definition|set-definition` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1476">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="b33c5-1477">Role</span><span class="sxs-lookup"><span data-stu-id="b33c5-1477">Role</span></span>
* <span data-ttu-id="b33c5-1478">Unterstützung für die API-Berechtigungsverwaltung, den angemeldeten Benutzer und die Verwaltung von Anwendungskennwörtern und Zertifikatanmeldeinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1478">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="b33c5-1479">`ad sp create-for-rbac` geändert, um „displayName“ und Dienstprinzipalname besser unterscheiden zu können</span><span class="sxs-lookup"><span data-stu-id="b33c5-1479">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="b33c5-1480">Unterstützung der Gewährung von Berechtigungen für AAD-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1480">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="b33c5-1481">Storage</span><span class="sxs-lookup"><span data-stu-id="b33c5-1481">Storage</span></span>
* <span data-ttu-id="b33c5-1482">Möglichkeit hinzugefügt, allein mit SAS und Endpunkten (ohne Kontoname oder Schlüssel) eine Verbindung mit Speicherdiensten herzustellen, wie unter `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>` beschrieben</span><span class="sxs-lookup"><span data-stu-id="b33c5-1482">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="b33c5-1483">VM</span><span class="sxs-lookup"><span data-stu-id="b33c5-1483">VM</span></span>
* <span data-ttu-id="b33c5-1484">Argument `storage-sku` zu `image create` hinzugefügt, um das Festlegen des standardmäßigen Speicherkontotyps für das Image zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="b33c5-1484">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="b33c5-1485">Fehler für `vm resize` behoben, durch den die Option `--no-wait` einen Absturz des Befehls verursachte</span><span class="sxs-lookup"><span data-stu-id="b33c5-1485">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="b33c5-1486">Tabellenausgabeformat für `vm encryption show` geändert, um den Status anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="b33c5-1486">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="b33c5-1487">`vm secret format` geändert, um JSON/JSONC-Ausgabe erforderlich zu machen.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1487">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="b33c5-1488">Der Benutzer wird gewarnt, und es wird standardmäßig die JSON-Ausgabe verwendet, wenn ein unzulässiges Ausgabeformat ausgewählt wird.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1488">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="b33c5-1489">Argumentüberprüfung für `vm create --image` verbessert</span><span class="sxs-lookup"><span data-stu-id="b33c5-1489">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="b33c5-1490">23. Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="b33c5-1490">October 23, 2018</span></span>

<span data-ttu-id="b33c5-1491">Version 2.0.49</span><span class="sxs-lookup"><span data-stu-id="b33c5-1491">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="b33c5-1492">Core</span><span class="sxs-lookup"><span data-stu-id="b33c5-1492">Core</span></span>
* <span data-ttu-id="b33c5-1493">Problem mit `--ids` behoben, aufgrund dessen `--subscription` Vorrang vor dem Abonnement in `--ids` hatte</span><span class="sxs-lookup"><span data-stu-id="b33c5-1493">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="b33c5-1494">Ausdrückliche Warnungen hinzugefügt, wenn Parameter durch die Verwendung von `--ids` ignoriert würden</span><span class="sxs-lookup"><span data-stu-id="b33c5-1494">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="b33c5-1495">ACR</span><span class="sxs-lookup"><span data-stu-id="b33c5-1495">ACR</span></span>
* <span data-ttu-id="b33c5-1496">Problem mit der ACR Build-Codierung in Python2 behoben</span><span class="sxs-lookup"><span data-stu-id="b33c5-1496">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="b33c5-1497">CDN</span><span class="sxs-lookup"><span data-stu-id="b33c5-1497">CDN</span></span>
* <span data-ttu-id="b33c5-1498">[BREAKING CHANGE] Standardverhalten beim Zwischenspeichern der Abfragezeichenfolge von `cdn endpoint create` so geändert, dass der Standardwert nicht mehr „IgnoreQueryString“ ist.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1498">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="b33c5-1499">Er wird jetzt vom Dienst festgelegt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1499">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="b33c5-1500">Container</span><span class="sxs-lookup"><span data-stu-id="b33c5-1500">Container</span></span>
* <span data-ttu-id="b33c5-1501">`Private` als gültiger Typ für die Übergabe an „--ip-address“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1501">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="b33c5-1502">Geändert, sodass nur eine Subnetz-ID für das Einrichten eines virtuellen Netzwerks für die Containergruppe zulässig ist</span><span class="sxs-lookup"><span data-stu-id="b33c5-1502">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="b33c5-1503">Geändert, sodass das Verwenden eines VNET-Namens oder einer Ressourcen-ID zulässig ist, um die Verwendung von VNETs aus verschiedenen Ressourcengruppen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="b33c5-1503">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="b33c5-1504">`--assign-identity` hinzugefügt, um einer Containergruppe eine MSI-Identität hinzuzufügen</span><span class="sxs-lookup"><span data-stu-id="b33c5-1504">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="b33c5-1505">`--scope` hinzugefügt, um eine Rollenzuweisung für die vom System zugewiesene MSI-Identität zu erstellen</span><span class="sxs-lookup"><span data-stu-id="b33c5-1505">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="b33c5-1506">Warnung hinzugefügt, wenn eine Containergruppe mit einem Image ohne Prozess mit langer Ausführungszeit erstellt wird</span><span class="sxs-lookup"><span data-stu-id="b33c5-1506">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="b33c5-1507">Probleme mit der Tabellenausgabe für Befehle `list` und `show` behoben</span><span class="sxs-lookup"><span data-stu-id="b33c5-1507">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="b33c5-1508">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="b33c5-1508">CosmosDB</span></span>
* <span data-ttu-id="b33c5-1509">Unterstützung für `--enable-multiple-write-locations` zu `cosmosdb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1509">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="b33c5-1510">Interactive</span><span class="sxs-lookup"><span data-stu-id="b33c5-1510">Interactive</span></span>
* <span data-ttu-id="b33c5-1511">Geändert, um sicherzustellen, dass der Parameter für globales Abonnement in Parametern angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="b33c5-1511">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="b33c5-1512">IoT Central</span><span class="sxs-lookup"><span data-stu-id="b33c5-1512">IoT Central</span></span>
* <span data-ttu-id="b33c5-1513">Optionen für Vorlagen und Anzeigenamen für die Erstellung von IoT Central-Anwendungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1513">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="b33c5-1514">[BREAKING CHANGE] Unterstützung für F1-SKU entfernt; stattdessen ist die S1-SKU zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1514">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="b33c5-1515">Überwachen</span><span class="sxs-lookup"><span data-stu-id="b33c5-1515">Monitor</span></span>
* <span data-ttu-id="b33c5-1516">Änderungen an `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="b33c5-1516">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="b33c5-1517">Unterstützung für das Auflisten aller Ereignisse auf Abonnementebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1517">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="b33c5-1518">`--offset`-Parameter für das einfachere Erstellen von Zeitabfragen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1518">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="b33c5-1519">Validierung für `--start-time` und `--end-time` verbessert, um die Verwendung von mehr ISO8601-Formate und benutzerfreundlicheren datetime-Formaten zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="b33c5-1519">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="b33c5-1520">`--namespace` als Alias für veraltete Option `--resource-provider` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1520">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="b33c5-1521">`--filters` als veraltet markiert, da vom Dienst ausschließlich Werte mit stark typisierten Optionen unterstützt werden</span><span class="sxs-lookup"><span data-stu-id="b33c5-1521">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="b33c5-1522">Änderungen an `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="b33c5-1522">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="b33c5-1523">`--offset`-Parameter für das einfachere Erstellen von Zeitabfragen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1523">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="b33c5-1524">Validierung für `--start-time` und `--end-time` verbessert, um die Verwendung von mehr ISO8601-Formate und benutzerfreundlicheren datetime-Formaten zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="b33c5-1524">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="b33c5-1525">Validierung für `--event-hub`- und `--event-hub-rule`-Argumente an `monitor diagnostic-settings create` verbessert</span><span class="sxs-lookup"><span data-stu-id="b33c5-1525">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="b33c5-1526">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="b33c5-1526">Network</span></span>
* <span data-ttu-id="b33c5-1527">`--app-gateway-address-pools`- und `--gateway-name`-Argumente zu `nic create` hinzugefügt, um das Hinzufügen von Back-End-Adresspools für Anwendungsgateways zu einer NIC zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="b33c5-1527">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="b33c5-1528">`--app-gateway-address-pools`- und `--gateway-name`-Argumente zu `nic ip-config create/update` hinzugefügt, um das Hinzufügen von Back-End-Adresspools für Anwendungsgateways zu einer NIC zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="b33c5-1528">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="b33c5-1529">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="b33c5-1529">ServiceBus</span></span>
* <span data-ttu-id="b33c5-1530">Schreibgeschütztes `migration_state`-Element zu „MigrationConfigProperties“ hinzugefügt, um den aktuellen Status der Migration von Service Bus Standard- zu Premium-Namespace anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="b33c5-1530">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="b33c5-1531">SQL</span><span class="sxs-lookup"><span data-stu-id="b33c5-1531">SQL</span></span>
* <span data-ttu-id="b33c5-1532">`sql failover-group create` und `sql failover-group update` korrigiert, damit die Verwendung einer Richtlinie für manuelles Failover möglich ist</span><span class="sxs-lookup"><span data-stu-id="b33c5-1532">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="b33c5-1533">Storage</span><span class="sxs-lookup"><span data-stu-id="b33c5-1533">Storage</span></span>
* <span data-ttu-id="b33c5-1534">Formatierung der `az storage cors list`-Ausgabe korrigiert, sodass alle Elemente den richtigen Dienstschlüssel anzeigen</span><span class="sxs-lookup"><span data-stu-id="b33c5-1534">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="b33c5-1535">`--bypass-immutability-policy`-Parameter für das Löschen von durch Unveränderlichkeitsrichtlinien blockierten Containern hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1535">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="b33c5-1536">VM</span><span class="sxs-lookup"><span data-stu-id="b33c5-1536">VM</span></span>
* <span data-ttu-id="b33c5-1537">Datenträger-Zwischenspeicherungsmodus `None` für Lv/Lv2-Computerserine in `[vm|vmss] create` erzwungen</span><span class="sxs-lookup"><span data-stu-id="b33c5-1537">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="b33c5-1538">Liste der unterstützten Größen für unterstützenden Netzwerkbeschleuniger für `vm create` aktualisiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-1538">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="b33c5-1539">Stark typisierte Argumente für UltraSSD-IOPS und MBit/s-Konfigurationen für `disk create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1539">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="b33c5-1540">16. Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="b33c5-1540">October 16, 2018</span></span>

<span data-ttu-id="b33c5-1541">Version 2.0.48</span><span class="sxs-lookup"><span data-stu-id="b33c5-1541">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="b33c5-1542">VM</span><span class="sxs-lookup"><span data-stu-id="b33c5-1542">VM</span></span>
* <span data-ttu-id="b33c5-1543">SDK-Problem behoben, das ein Fehlschlagen der Homebrew-Installation verursacht hat</span><span class="sxs-lookup"><span data-stu-id="b33c5-1543">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="b33c5-1544">9\. Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="b33c5-1544">October 9, 2018</span></span>

<span data-ttu-id="b33c5-1545">Version 2.0.47</span><span class="sxs-lookup"><span data-stu-id="b33c5-1545">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="b33c5-1546">Core</span><span class="sxs-lookup"><span data-stu-id="b33c5-1546">Core</span></span>
* <span data-ttu-id="b33c5-1547">Verbesserte Fehlerbehandlung für Fehler vom Typ „Ungültige Anforderung“</span><span class="sxs-lookup"><span data-stu-id="b33c5-1547">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="b33c5-1548">ACR</span><span class="sxs-lookup"><span data-stu-id="b33c5-1548">ACR</span></span>
* <span data-ttu-id="b33c5-1549">Unterstützung für ähnliches Tabellenformat wie Helm-Client hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1549">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="b33c5-1550">ACS</span><span class="sxs-lookup"><span data-stu-id="b33c5-1550">ACS</span></span>
* <span data-ttu-id="b33c5-1551">`aks [create|scale] --nodepool-name` zum Konfigurieren des Knotenpoolnamens hinzugefügt, auf 12 Zeichen gekürzt, Standard: nodepool1</span><span class="sxs-lookup"><span data-stu-id="b33c5-1551">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="b33c5-1552">Korrektur, bei der auf „scp“ zurückgegriffen wird, wenn Parimiko nicht funktioniert</span><span class="sxs-lookup"><span data-stu-id="b33c5-1552">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="b33c5-1553">`aks create` geändert, sodass `--aad-tenant-id` nicht mehr erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="b33c5-1553">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="b33c5-1554">Verbesserte Zusammenführung von Kubernetes-Anmeldeinformationen, wenn doppelte Einträge vorhanden sind</span><span class="sxs-lookup"><span data-stu-id="b33c5-1554">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="b33c5-1555">Container</span><span class="sxs-lookup"><span data-stu-id="b33c5-1555">Container</span></span>
* <span data-ttu-id="b33c5-1556">`functionapp create` geändert, sodass das Erstellen eines Linux-Nutzungsplans mit einer bestimmten Runtime unterstützt wird</span><span class="sxs-lookup"><span data-stu-id="b33c5-1556">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="b33c5-1557">[VORSCHAUVERSION] Unterstützung für das Hosten von Web-Apps in Windows-Containern hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1557">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="b33c5-1558">Event Hub</span><span class="sxs-lookup"><span data-stu-id="b33c5-1558">Event Hub</span></span>
* <span data-ttu-id="b33c5-1559">Befehl `eventhub update` korrigiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-1559">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="b33c5-1560">[BREAKING CHANGE]`list`-Befehle geändert, sodass Fehler von Typ „NotFound(404)“ für Ressourcen mit der typische Vorgehensweise behandelt werden, anstatt eine leere Liste anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="b33c5-1560">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="b33c5-1561">Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="b33c5-1561">Extensions</span></span>
* <span data-ttu-id="b33c5-1562">Problem beim Hinzufügen einer Erweiterung behoben, die bereits installiert ist</span><span class="sxs-lookup"><span data-stu-id="b33c5-1562">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="b33c5-1563">HDInsight</span><span class="sxs-lookup"><span data-stu-id="b33c5-1563">HDInsight</span></span>
* <span data-ttu-id="b33c5-1564">Erste Veröffentlichung</span><span class="sxs-lookup"><span data-stu-id="b33c5-1564">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="b33c5-1565">IoT</span><span class="sxs-lookup"><span data-stu-id="b33c5-1565">IoT</span></span>
* <span data-ttu-id="b33c5-1566">Befehl zur Erweiterungsinstallation zu Banner bei der ersten Ausführung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1566">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="b33c5-1567">KeyVault</span><span class="sxs-lookup"><span data-stu-id="b33c5-1567">KeyVault</span></span>
* <span data-ttu-id="b33c5-1568">Geändert, sodass Key Vault-Speicherbefehle auf das aktuelle API-Profil beschränkt sind</span><span class="sxs-lookup"><span data-stu-id="b33c5-1568">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="b33c5-1569">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="b33c5-1569">Network</span></span>
* <span data-ttu-id="b33c5-1570">`network dns zone create` korrigiert: Befehl ist auch erfolgreich, wenn der Benutzer einen Standardspeicherort konfiguriert hat.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1570">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="b33c5-1571">Siehe Nr. 6052</span><span class="sxs-lookup"><span data-stu-id="b33c5-1571">See #6052</span></span>
* <span data-ttu-id="b33c5-1572">`--remote-vnet-id` für `network vnet peering create` eingestellt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1572">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="b33c5-1573">`--remote-vnet` zum `network vnet peering create`-Element hinzugefügt, das einen Namen oder eine ID akzeptiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-1573">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="b33c5-1574">Unterstützung für mehrere Subnetzpräfixe zu `network vnet create` in `--subnet-prefixes` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1574">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="b33c5-1575">Unterstützung für mehrere Subnetzpräfixe zu `network vnet subnet [create|update]` in `--address-prefixes` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1575">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="b33c5-1576">Problem mit `network application-gateway create` behoben, das die Erstellung von Gateways mit der SKU `WAF_v2` oder `Standard_v2` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="b33c5-1576">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="b33c5-1577">`--service-endpoint-policy`-Argument für Benutzerfreundlichkeit zu `network vnet subnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1577">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="b33c5-1578">Role</span><span class="sxs-lookup"><span data-stu-id="b33c5-1578">Role</span></span>
* <span data-ttu-id="b33c5-1579">Unterstützung für das Auflisten von Azure AD-App-Besitzern in `ad app owner` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1579">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="b33c5-1580">Unterstützung für das Auflisten von Azure AD-Dienstprinzipalbesitzern in `ad sp owner` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1580">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="b33c5-1581">Geändert, um sicherzustellen, dass die Erstellungs- und Aktualisierungsbefehle für die Rollendefinition Konfigurationen mit mehreren Berechtigungen akzeptieren</span><span class="sxs-lookup"><span data-stu-id="b33c5-1581">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="b33c5-1582">`ad sp create-for-rbac` geändert, um sicherzustellen, dass der Homepage-URI immer „https“ ist</span><span class="sxs-lookup"><span data-stu-id="b33c5-1582">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="b33c5-1583">Service Bus</span><span class="sxs-lookup"><span data-stu-id="b33c5-1583">Service Bus</span></span>
* <span data-ttu-id="b33c5-1584">[BREAKING CHANGE]`list`-Befehle geändert, sodass Fehler von Typ „NotFound(404)“ für Ressourcen mit der typische Vorgehensweise behandelt werden, anstatt eine leere Liste anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="b33c5-1584">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="b33c5-1585">VM</span><span class="sxs-lookup"><span data-stu-id="b33c5-1585">VM</span></span>
* <span data-ttu-id="b33c5-1586">Leeres `accessSas`-Feld in `disk grant-access` korrigiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-1586">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="b33c5-1587">`vmss create` geändert, sodass ein ausreichend großer Front-End-Portbereich zur Verarbeitung von Überbereitstellung reserviert ist</span><span class="sxs-lookup"><span data-stu-id="b33c5-1587">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="b33c5-1588">Aktualisierungsbefehle für `sig` korrigiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-1588">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="b33c5-1589">`--no-wait`-Unterstützung für die Verwaltung von Imageversionen in `sig` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1589">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="b33c5-1590">`vm list-ip-addresses` geändert, sodass die Verfügbarkeitszone von öffentlichen IP-Adressen angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="b33c5-1590">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="b33c5-1591">`[vm|vmss] disk attach` geändert, sodass die Standard-LUN eines Datenträgers standardmäßig auf die erste verfügbare Stelle festgelegt wird</span><span class="sxs-lookup"><span data-stu-id="b33c5-1591">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="b33c5-1592">21. September 2018</span><span class="sxs-lookup"><span data-stu-id="b33c5-1592">September 21, 2018</span></span>

<span data-ttu-id="b33c5-1593">Version 2.0.46</span><span class="sxs-lookup"><span data-stu-id="b33c5-1593">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="b33c5-1594">ACR</span><span class="sxs-lookup"><span data-stu-id="b33c5-1594">ACR</span></span>
* <span data-ttu-id="b33c5-1595">ACR-Aufgabenbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1595">Added ACR Task commands</span></span>
* <span data-ttu-id="b33c5-1596">Befehl für die Schnellausführung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1596">Added quick run command</span></span>
* <span data-ttu-id="b33c5-1597">`build-task`-Befehlsgruppe als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-1597">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="b33c5-1598">`helm`-Befehlsgruppe hinzugefügt, um die Verwaltung von Helm-Diagrammen mit ACR zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="b33c5-1598">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="b33c5-1599">Unterstützung für idempotentes Erstellen für die verwaltete Registrierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1599">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="b33c5-1600">Formatfreies Flag für die Anzeige von Buildprotokollen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1600">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="b33c5-1601">ACS</span><span class="sxs-lookup"><span data-stu-id="b33c5-1601">ACS</span></span>
* <span data-ttu-id="b33c5-1602">Befehl `install-connector` zum Festlegen des AKS-Master-FQDN geändert</span><span class="sxs-lookup"><span data-stu-id="b33c5-1602">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="b33c5-1603">Erstellen der Rollenzuweisung für „vnet-subnet-id“ (wenn kein Dienstprinzipal angegeben wurde) und „skip-role-assignment“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-1603">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="b33c5-1604">AppService</span><span class="sxs-lookup"><span data-stu-id="b33c5-1604">AppService</span></span>

* <span data-ttu-id="b33c5-1605">Unterstützung für WebJobs-Vorgangsverwaltung hinzugefügt (kontinuierlich/ausgelöst)</span><span class="sxs-lookup"><span data-stu-id="b33c5-1605">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="b33c5-1606">„az webapp config set“ unterstützt die Eigenschaft „--fts-state“; Unterstützung für „az functionapp config set/show“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1606">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="b33c5-1607">Unterstützung für Bring Your Own Storage für Web-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1607">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="b33c5-1608">Unterstützung für das Auflisten und Wiederherstellen gelöschter Web-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1608">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="b33c5-1609">Batch</span><span class="sxs-lookup"><span data-stu-id="b33c5-1609">Batch</span></span>
* <span data-ttu-id="b33c5-1610">Hinzufügen von Aufgaben über `--json-file` geändert, um die AddTaskCollectionParameter-Syntax zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="b33c5-1610">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="b33c5-1611">Dokumentation akzeptierter `--json-file`-Formate aktualisiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-1611">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="b33c5-1612">`--max-tasks-per-node-option` zu `batch pool create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1612">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="b33c5-1613">Verhalten von `batch account` geändert, um das aktuell angemeldete Konto anzuzeigen, wenn keine Optionen angegeben wurden</span><span class="sxs-lookup"><span data-stu-id="b33c5-1613">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="b33c5-1614">Batch KI</span><span class="sxs-lookup"><span data-stu-id="b33c5-1614">Batch AI</span></span> 
* <span data-ttu-id="b33c5-1615">Fehler bei der automatischen Speicherkontoerstellung im Befehl `batchai cluster create` behoben</span><span class="sxs-lookup"><span data-stu-id="b33c5-1615">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="b33c5-1616">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="b33c5-1616">Cognitive Services</span></span>
* <span data-ttu-id="b33c5-1617">Vervollständigung für die Argumente `--sku`, `--kind` und `--location` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1617">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="b33c5-1618">Befehl `cognitiveservices account list-usage` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1618">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="b33c5-1619">Befehl `cognitiveservices account list-kinds` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1619">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="b33c5-1620">Befehl `cognitiveservices account list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1620">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="b33c5-1621">`cognitiveservices list` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-1621">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="b33c5-1622">`--name` geändert (ist jetzt optional für `cognitiveservices account list-skus`)</span><span class="sxs-lookup"><span data-stu-id="b33c5-1622">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="b33c5-1623">Container</span><span class="sxs-lookup"><span data-stu-id="b33c5-1623">Container</span></span>
* <span data-ttu-id="b33c5-1624">Möglichkeit zum Neustarten und Beenden einer ausgeführten Containergruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1624">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="b33c5-1625">`--network-profile` zum Übergeben eines Netzwerkprofils hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1625">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="b33c5-1626">`--subnet` und `--vnet_name` hinzugefügt, um das Erstellen von Containergruppen in einem VNET zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="b33c5-1626">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="b33c5-1627">Tabellenausgabe geändert, sodass der Status der Containergruppe angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="b33c5-1627">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="b33c5-1628">Data Lake</span><span class="sxs-lookup"><span data-stu-id="b33c5-1628">Datalake</span></span>
* <span data-ttu-id="b33c5-1629">Befehle für VNET-Regeln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1629">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="b33c5-1630">Interaktive Shell</span><span class="sxs-lookup"><span data-stu-id="b33c5-1630">Interactive Shell</span></span>
* <span data-ttu-id="b33c5-1631">Fehler in Windows behoben, durch den Befehle nicht ordnungsgemäß ausgeführt wurden</span><span class="sxs-lookup"><span data-stu-id="b33c5-1631">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="b33c5-1632">Durch veraltete Objekte verursachtes Problem beim Laden von Befehlen im interaktiven Modus behoben</span><span class="sxs-lookup"><span data-stu-id="b33c5-1632">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="b33c5-1633">IoT</span><span class="sxs-lookup"><span data-stu-id="b33c5-1633">IoT</span></span>
* <span data-ttu-id="b33c5-1634">Routingunterstützung für IoT Hubs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1634">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="b33c5-1635">Key Vault</span><span class="sxs-lookup"><span data-stu-id="b33c5-1635">Key Vault</span></span>
* <span data-ttu-id="b33c5-1636">Key Vault-Schlüsselimport für RSA-Schlüssel korrigiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-1636">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="b33c5-1637">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="b33c5-1637">Network</span></span>
* <span data-ttu-id="b33c5-1638">Befehle vom Typ `network public-ip prefix` hinzugefügt, um Präfixe von öffentlichen IP-Adressen zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="b33c5-1638">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="b33c5-1639">Befehle vom Typ `network service-endpoint` hinzugefügt, um Dienstendpunktrichtlinien-Features zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="b33c5-1639">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="b33c5-1640">Befehle vom Typ `network lb outbound-rule` hinzugefügt, um die Erstellung von Ausgangsregeln für Load Balancer Standard zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="b33c5-1640">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="b33c5-1641">`--public-ip-prefix` zu `network lb frontend-ip create/update` hinzugefügt, um Front-End-IP-Konfigurationen mit Präfixen von öffentlichen IP-Adressen zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="b33c5-1641">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="b33c5-1642">`--enable-tcp-reset` zu `network lb rule/inbound-nat-rule/inbound-nat-pool create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1642">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="b33c5-1643">`--disable-outbound-snat` zu `network lb rule create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1643">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="b33c5-1644">Verwendung von `network watcher flow-log show/configure` mit klassischen NSGs ermöglicht</span><span class="sxs-lookup"><span data-stu-id="b33c5-1644">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="b33c5-1645">Hinzufügen des `network watcher run-configuration-diagnostic`-Befehls</span><span class="sxs-lookup"><span data-stu-id="b33c5-1645">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="b33c5-1646">Befehl `network watcher test-connectivity` korrigiert und Eigenschaften `--method`, `--valid-status-codes` und `--headers` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1646">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="b33c5-1647">`network express-route create/update`: Flag `--allow-global-reach` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1647">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="b33c5-1648">`network vnet subnet create/update`: Unterstützung für `--delegation` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1648">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="b33c5-1649">Befehl `network vnet subnet list-available-delegations` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1649">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="b33c5-1650">`network traffic-manager profile create/update`: Unterstützung für `--interval`, `--timeout` und `--max-failures` für die Überwachungskonfiguration hinzugefügt; Optionen `--monitor-path`, `--monitor-port` und `--monitor-protocol` zugunsten von `--path`, `--port` und `--protocol` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-1650">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="b33c5-1651">`network lb frontend-ip create/update`: Logik für das Festlegen der Zuweisungsmethode für private IP-Adressen korrigiert. Bei Angabe einer privaten IP-Adresse ist die Zuweisung statisch. Wird keine private IP-Adresse (oder eine leere Zeichenfolge für die private IP-Adresse) angegeben, erfolgt eine dynamische Zuweisung.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1651">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="b33c5-1652">`dns record-set * create/update`: Unterstützung für `--target-resource` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1652">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="b33c5-1653">Befehle vom Typ `network interface-endpoint` hinzugefügt, um Schnittstellenendpunkt-Objekte abzufragen</span><span class="sxs-lookup"><span data-stu-id="b33c5-1653">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="b33c5-1654">`network profile show/list/delete` für die partielle Verwaltung von Netzwerkprofilen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1654">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="b33c5-1655">Befehle vom Typ `network express-route peering connection` für die Verwaltung von Peeringverbindungen zwischen ExpressRoute-Instanzen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1655">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="b33c5-1656">RDBMS</span><span class="sxs-lookup"><span data-stu-id="b33c5-1656">RDBMS</span></span>
* <span data-ttu-id="b33c5-1657">Unterstützung für den MariaDB-Dienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1657">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="b33c5-1658">Reservierung</span><span class="sxs-lookup"><span data-stu-id="b33c5-1658">Reservation</span></span>
* <span data-ttu-id="b33c5-1659">Cosmos DB im Enumerationstyp für reservierte Ressourcen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1659">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="b33c5-1660">Namenseigenschaft im Patchmodell hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1660">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="b33c5-1661">App-Verwaltung</span><span class="sxs-lookup"><span data-stu-id="b33c5-1661">Manage App</span></span>
* <span data-ttu-id="b33c5-1662">Fehler in `managedapp create --kind MarketPlace` korrigiert, der zum Absturz der Instanzerstellung einer verwalteten Marketplace-App führte</span><span class="sxs-lookup"><span data-stu-id="b33c5-1662">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="b33c5-1663">Befehle vom Typ `feature` geändert, um sie auf unterstützte Profile zu beschränken</span><span class="sxs-lookup"><span data-stu-id="b33c5-1663">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="b33c5-1664">Role</span><span class="sxs-lookup"><span data-stu-id="b33c5-1664">Role</span></span>
* <span data-ttu-id="b33c5-1665">Unterstützung für das Auflisten der Gruppenmitgliedschaften des Benutzers hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1665">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="b33c5-1666">SignalR</span><span class="sxs-lookup"><span data-stu-id="b33c5-1666">SignalR</span></span>
* <span data-ttu-id="b33c5-1667">Erste Version</span><span class="sxs-lookup"><span data-stu-id="b33c5-1667">First release</span></span>

### <a name="storage"></a><span data-ttu-id="b33c5-1668">Storage</span><span class="sxs-lookup"><span data-stu-id="b33c5-1668">Storage</span></span>
* <span data-ttu-id="b33c5-1669">Parameter `--auth-mode login` für die Verwendung der Anmeldeinformationen des Benutzers für die Blob- und Warteschlangenautorisierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1669">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="b33c5-1670">`storage container immutability-policy/legal-hold` für die Verwaltung von unveränderlichem Speicher hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1670">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="b33c5-1671">VM</span><span class="sxs-lookup"><span data-stu-id="b33c5-1671">VM</span></span>
* <span data-ttu-id="b33c5-1672">Problem behoben, das dazu führte, dass die Datei mit dem privaten Schlüssel durch `vm create --generate-ssh-keys` überschrieben wird, wenn die Datei mit dem privaten Schlüssel fehlt (Nr. 4725, 6780)</span><span class="sxs-lookup"><span data-stu-id="b33c5-1672">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="b33c5-1673">Unterstützung für den gemeinsamen Image-Katalog über `az sig` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1673">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="b33c5-1674">28. August 2018</span><span class="sxs-lookup"><span data-stu-id="b33c5-1674">August 28, 2018</span></span>

<span data-ttu-id="b33c5-1675">Version 2.0.45</span><span class="sxs-lookup"><span data-stu-id="b33c5-1675">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="b33c5-1676">Core</span><span class="sxs-lookup"><span data-stu-id="b33c5-1676">Core</span></span>

* <span data-ttu-id="b33c5-1677">Das Problem, aufgrund dessen eine leere Konfigurationsdatei geladen wurde, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1677">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="b33c5-1678">Unterstützung für Profil `2018-03-01-hybrid` für Azure Stack hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1678">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="b33c5-1679">ACR</span><span class="sxs-lookup"><span data-stu-id="b33c5-1679">ACR</span></span>

* <span data-ttu-id="b33c5-1680">Problemumgehung für Laufzeitvorgänge ohne ARM-Anforderungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1680">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="b33c5-1681">Änderung vorgenommen, um im Befehl `build` Versionskontrolldateien (etwa „.git“ und „.gitignore“) standardmäßig aus der TAR-Datei auszuschließen</span><span class="sxs-lookup"><span data-stu-id="b33c5-1681">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="b33c5-1682">ACS</span><span class="sxs-lookup"><span data-stu-id="b33c5-1682">ACS</span></span>

* <span data-ttu-id="b33c5-1683">`aks create` geändert, dass standardmäßig virtuelle Computer vom Typ `Standard_DS2_v2` erstellt werden</span><span class="sxs-lookup"><span data-stu-id="b33c5-1683">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="b33c5-1684">`aks get-credentials` geändert, um nun neue APIs zum Abrufen der Clusteranmeldeinformationen aufzurufen</span><span class="sxs-lookup"><span data-stu-id="b33c5-1684">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="b33c5-1685">AppService</span><span class="sxs-lookup"><span data-stu-id="b33c5-1685">AppService</span></span>

* <span data-ttu-id="b33c5-1686">Unterstützung für CORS in „functionapp“ und „webapp“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1686">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="b33c5-1687">ARM-Tagunterstützung in Erstellungsbefehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1687">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="b33c5-1688">`[webapp|functionapp] identity show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="b33c5-1688">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="b33c5-1689">Backup</span><span class="sxs-lookup"><span data-stu-id="b33c5-1689">Backup</span></span>

* <span data-ttu-id="b33c5-1690">`backup vault backup-properties show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="b33c5-1690">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="b33c5-1691">Botdienst</span><span class="sxs-lookup"><span data-stu-id="b33c5-1691">Bot Service</span></span>

* <span data-ttu-id="b33c5-1692">Anfängliches Release der Botdienst-CLI</span><span class="sxs-lookup"><span data-stu-id="b33c5-1692">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="b33c5-1693">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="b33c5-1693">Cognitive Services</span></span>

* <span data-ttu-id="b33c5-1694">Neuer Parameter `--api-properties,` hinzugefügt, der zum Erstellen einiger Dienste erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="b33c5-1694">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="b33c5-1695">IoT</span><span class="sxs-lookup"><span data-stu-id="b33c5-1695">IoT</span></span>

* <span data-ttu-id="b33c5-1696">Problem mit dem Zuweisen verknüpfter Hubs behoben</span><span class="sxs-lookup"><span data-stu-id="b33c5-1696">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="b33c5-1697">Überwachen</span><span class="sxs-lookup"><span data-stu-id="b33c5-1697">Monitor</span></span>

* <span data-ttu-id="b33c5-1698">`monitor metrics alert`-Befehle für Metrikwarnungen nahezu in Echtzeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1698">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="b33c5-1699">`monitor alert`-Befehle als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-1699">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="b33c5-1700">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="b33c5-1700">Network</span></span>

* <span data-ttu-id="b33c5-1701">`network application-gateway ssl-policy predefined show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="b33c5-1701">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="b33c5-1702">Resource</span><span class="sxs-lookup"><span data-stu-id="b33c5-1702">Resource</span></span>

* <span data-ttu-id="b33c5-1703">`provider operation show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="b33c5-1703">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="b33c5-1704">Storage</span><span class="sxs-lookup"><span data-stu-id="b33c5-1704">Storage</span></span>

* <span data-ttu-id="b33c5-1705">`storage share policy show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="b33c5-1705">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="b33c5-1706">VM</span><span class="sxs-lookup"><span data-stu-id="b33c5-1706">VM</span></span>

* <span data-ttu-id="b33c5-1707">`vm/vmss identity show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="b33c5-1707">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="b33c5-1708">`--storage-caching` für `vm create` eingestellt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1708">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="b33c5-1709">14. August 2018</span><span class="sxs-lookup"><span data-stu-id="b33c5-1709">Auguest 14, 2018</span></span>

<span data-ttu-id="b33c5-1710">Version 2.0.44</span><span class="sxs-lookup"><span data-stu-id="b33c5-1710">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="b33c5-1711">Core</span><span class="sxs-lookup"><span data-stu-id="b33c5-1711">Core</span></span>

* <span data-ttu-id="b33c5-1712">Numerische Anzeige in `table`-Ausgabe korrigiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-1712">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="b33c5-1713">YAML-Ausgabeformat hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1713">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="b33c5-1714">Telemetrie</span><span class="sxs-lookup"><span data-stu-id="b33c5-1714">Telemetry</span></span>

* <span data-ttu-id="b33c5-1715">Verbesserte Berichterstellung für Telemetriedaten</span><span class="sxs-lookup"><span data-stu-id="b33c5-1715">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="b33c5-1716">ACR</span><span class="sxs-lookup"><span data-stu-id="b33c5-1716">ACR</span></span>

* <span data-ttu-id="b33c5-1717">Befehle vom Typ `content-trust policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1717">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="b33c5-1718">Problem behoben, aufgrund dessen `.dockerignore` nicht richtig verarbeitet wurde</span><span class="sxs-lookup"><span data-stu-id="b33c5-1718">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="b33c5-1719">ACS</span><span class="sxs-lookup"><span data-stu-id="b33c5-1719">ACS</span></span>

* <span data-ttu-id="b33c5-1720">`az acs/aks install-cli` für die Installation in `%USERPROFILE%\.azure-kubectl` unter Windows geändert</span><span class="sxs-lookup"><span data-stu-id="b33c5-1720">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="b33c5-1721">`az aks install-connector` geändert, um zu ermitteln, ob der Cluster über RBAC verfügt, und um den ACI-Connector entsprechend zu konfigurieren</span><span class="sxs-lookup"><span data-stu-id="b33c5-1721">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="b33c5-1722">Geändert in Rollenzuweisung zum Subnetz bei entsprechender Angabe</span><span class="sxs-lookup"><span data-stu-id="b33c5-1722">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="b33c5-1723">Neue Option zum Überspringen der Rollenzuweisung für Subnetz hinzugefügt, wenn dieses angegeben ist</span><span class="sxs-lookup"><span data-stu-id="b33c5-1723">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="b33c5-1724">Geändert, um Rollenzuweisung zum Subnetz zu überspringen, wenn bereits eine Zuweisung vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="b33c5-1724">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="b33c5-1725">AppService</span><span class="sxs-lookup"><span data-stu-id="b33c5-1725">AppService</span></span>

* <span data-ttu-id="b33c5-1726">Fehler behoben, der das Erstellen einer Funktions-App mithilfe von Speicherkonten in externen Ressourcengruppen verhinderte</span><span class="sxs-lookup"><span data-stu-id="b33c5-1726">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="b33c5-1727">Absturz bei ZIP-Bereitstellung behoben</span><span class="sxs-lookup"><span data-stu-id="b33c5-1727">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="b33c5-1728">Batch AI</span><span class="sxs-lookup"><span data-stu-id="b33c5-1728">BatchAI</span></span>

* <span data-ttu-id="b33c5-1729">Protokollierungsausgabe für die automatische Speicherkontoerstellung geändert, sodass nun „Ressourcen*gruppe*“ angegeben wird</span><span class="sxs-lookup"><span data-stu-id="b33c5-1729">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="b33c5-1730">Container</span><span class="sxs-lookup"><span data-stu-id="b33c5-1730">Container</span></span>

* <span data-ttu-id="b33c5-1731">`--secure-environment-variables` zum Übergeben sicherer Umgebungsvariablen an einen Container hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1731">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="b33c5-1732">IoT</span><span class="sxs-lookup"><span data-stu-id="b33c5-1732">IoT</span></span>

* <span data-ttu-id="b33c5-1733">[BREAKING CHANGE] Veraltete Befehle entfernt, die in die IoT-Erweiterung verschoben wurden</span><span class="sxs-lookup"><span data-stu-id="b33c5-1733">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="b33c5-1734">Elemente aktualisiert, um nicht die Domäne `azure-devices.net` anzunehmen</span><span class="sxs-lookup"><span data-stu-id="b33c5-1734">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="b33c5-1735">Iot Central</span><span class="sxs-lookup"><span data-stu-id="b33c5-1735">Iot Central</span></span>

* <span data-ttu-id="b33c5-1736">Erstes Release des IoT Central-Moduls</span><span class="sxs-lookup"><span data-stu-id="b33c5-1736">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="b33c5-1737">KeyVault</span><span class="sxs-lookup"><span data-stu-id="b33c5-1737">KeyVault</span></span>


* <span data-ttu-id="b33c5-1738">Befehle zum Verwalten von Speicherkonten und SAS-Definitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1738">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="b33c5-1739">Befehle für Netzwerkregeln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1739">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="b33c5-1740">Parameter `--id` zu Geheimnis-, Schlüssel- und Zertifikatvorgängen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1740">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="b33c5-1741">Unterstützung für Version mit mehreren APIs zur Schlüsseltresorverwaltung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1741">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="b33c5-1742">Unterstützung für Version mit mehreren APIs zur Schlüsseltresordatenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1742">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="b33c5-1743">Relay</span><span class="sxs-lookup"><span data-stu-id="b33c5-1743">Relay</span></span>

* <span data-ttu-id="b33c5-1744">Erste Veröffentlichung</span><span class="sxs-lookup"><span data-stu-id="b33c5-1744">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="b33c5-1745">Sql</span><span class="sxs-lookup"><span data-stu-id="b33c5-1745">Sql</span></span>

* <span data-ttu-id="b33c5-1746">Befehle vom Typ `sql failover-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1746">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="b33c5-1747">Storage</span><span class="sxs-lookup"><span data-stu-id="b33c5-1747">Storage</span></span>

* <span data-ttu-id="b33c5-1748">[BREAKING CHANGE]`storage account show-usage` geändert, um Parameter `--location` erforderlich zu machen. Auflistung nach Region</span><span class="sxs-lookup"><span data-stu-id="b33c5-1748">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="b33c5-1749">Parameter `--resource-group` geändert, sodass er für `storage account`-Befehle optional ist</span><span class="sxs-lookup"><span data-stu-id="b33c5-1749">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="b33c5-1750">Warnungen vom Typ „Fehler bei Vorbedingung“ für einzelne Fehler in Batch-Befehlen für eine aggregiert Nachricht entfernt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1750">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="b33c5-1751">`[blob|file] delete-batch`-Befehle geändert, sodass kein Array mit Null-Werten mehr ausgegeben wird</span><span class="sxs-lookup"><span data-stu-id="b33c5-1751">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="b33c5-1752">`blob [download|upload|delete-batch]`-Befehle geändert, um SAS-Token aus Container-URL zu lesen</span><span class="sxs-lookup"><span data-stu-id="b33c5-1752">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="b33c5-1753">VM</span><span class="sxs-lookup"><span data-stu-id="b33c5-1753">VM</span></span>

* <span data-ttu-id="b33c5-1754">Allgemeine Filter zu `vm list-skus` für höhere Benutzerfreundlichkeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1754">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="b33c5-1755">31. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="b33c5-1755">July 31, 2018</span></span>

<span data-ttu-id="b33c5-1756">Version 2.0.43</span><span class="sxs-lookup"><span data-stu-id="b33c5-1756">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="b33c5-1757">ACR</span><span class="sxs-lookup"><span data-stu-id="b33c5-1757">ACR</span></span>

* <span data-ttu-id="b33c5-1758">Flag `--with-secure-properties` zum Befehl `acr build-task show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1758">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="b33c5-1759">Befehl `acr build-task update-build` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1759">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="b33c5-1760">ACS</span><span class="sxs-lookup"><span data-stu-id="b33c5-1760">ACS</span></span>

* <span data-ttu-id="b33c5-1761">Änderung, um 0 (Erfolg) zurückzugeben, wenn `az aks browse` durch Drücken von [STRG+C] beendet wird</span><span class="sxs-lookup"><span data-stu-id="b33c5-1761">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="b33c5-1762">Batch</span><span class="sxs-lookup"><span data-stu-id="b33c5-1762">Batch</span></span>

* <span data-ttu-id="b33c5-1763">Korrektur eines Fehlers bei der Anzeige des AAD-Tokens in Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="b33c5-1763">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="b33c5-1764">Container</span><span class="sxs-lookup"><span data-stu-id="b33c5-1764">Container</span></span>

* <span data-ttu-id="b33c5-1765">Voraussetzung von `--log-analytics-workspace-key` für Name oder ID im festgelegten Abonnement entfernt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1765">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="b33c5-1766">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="b33c5-1766">Network</span></span>

* <span data-ttu-id="b33c5-1767">DNS-Unterstützung zu „2017-03-09-profile“ für Azure Stack hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1767">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="b33c5-1768">Resource</span><span class="sxs-lookup"><span data-stu-id="b33c5-1768">Resource</span></span>

* <span data-ttu-id="b33c5-1769">`--rollback-on-error` zu `group deployment create` hinzugefügt, um bei einem Fehler eine als funktionierend bekannte Bereitstellung auszuführen</span><span class="sxs-lookup"><span data-stu-id="b33c5-1769">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="b33c5-1770">Problem behoben, aufgrund dessen `--parameters {}` mit `group deployment create` zu einem Fehler führte</span><span class="sxs-lookup"><span data-stu-id="b33c5-1770">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="b33c5-1771">Role</span><span class="sxs-lookup"><span data-stu-id="b33c5-1771">Role</span></span>

* <span data-ttu-id="b33c5-1772">Unterstützung für das Stack-Profil „2017-03-09-profile“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1772">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="b33c5-1773">Problem behoben, aufgrund dessen das generische Update von Parametern auf `app update` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="b33c5-1773">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="b33c5-1774">Suchen,</span><span class="sxs-lookup"><span data-stu-id="b33c5-1774">Search</span></span>

* <span data-ttu-id="b33c5-1775">Befehle für Azure Search-Dienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1775">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="b33c5-1776">Service Bus</span><span class="sxs-lookup"><span data-stu-id="b33c5-1776">Service Bus</span></span>

* <span data-ttu-id="b33c5-1777">Migrationsbefehlsgruppe hinzugefügt, um einen Namespace von Service Bus Standard zu Premium zu migrieren</span><span class="sxs-lookup"><span data-stu-id="b33c5-1777">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="b33c5-1778">Neue optionale Eigenschaften zu Service Bus-Warteschlange und -Abonnement hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1778">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="b33c5-1779">`--enable-batched-operations` und `--enable-dead-lettering-on-message-expiration` in `queue`</span><span class="sxs-lookup"><span data-stu-id="b33c5-1779">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="b33c5-1780">`--dead-letter-on-filter-exceptions` in `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="b33c5-1780">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="b33c5-1781">Storage</span><span class="sxs-lookup"><span data-stu-id="b33c5-1781">Storage</span></span>

* <span data-ttu-id="b33c5-1782">Unterstützung für den Download großer Dateien über eine einzelne Verbindung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1782">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="b33c5-1783">`show`-Befehle konvertiert, bei denen im Falle einer fehlenden Ressource kein Fehler mit dem Exitcode 3 ausgelöst wurde</span><span class="sxs-lookup"><span data-stu-id="b33c5-1783">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="b33c5-1784">VM</span><span class="sxs-lookup"><span data-stu-id="b33c5-1784">VM</span></span>

* <span data-ttu-id="b33c5-1785">Unterstützung zum Auflisten von Verfügbarkeitsgruppen nach Abonnement hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1785">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="b33c5-1786">Unterstützung für `StandardSSD_LRS` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1786">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="b33c5-1787">Unterstützung für Anwendungssicherheitsgruppe beim Erstellen einer VM-Skalierungsgruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1787">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="b33c5-1788">[BREAKING CHANGE]`[vm|vmss] create`, `[vm|vmss] identity assign` und `[vm|vmss] identity remove` wurden geändert, um vom Benutzer zugewiesene Identitäten im Wörterbuchformat auszugeben.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1788">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="b33c5-1789">18. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="b33c5-1789">July 18, 2018</span></span>

<span data-ttu-id="b33c5-1790">Version 2.0.42</span><span class="sxs-lookup"><span data-stu-id="b33c5-1790">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="b33c5-1791">Core</span><span class="sxs-lookup"><span data-stu-id="b33c5-1791">Core</span></span>

* <span data-ttu-id="b33c5-1792">Unterstützung für browserbasierte Anmeldung WSL-Bash-Fenster hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1792">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="b33c5-1793">`--force-string`-Flag für alle generischen Updatebefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1793">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="b33c5-1794">[BREAKING CHANGE] Befehle vom Typ „show“ so geändert, dass die Fehlermeldung protokolliert wird und der Vorgang bei einer fehlenden Ressource mit dem Exitcode 3 fehlschlägt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1794">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="b33c5-1795">ACR</span><span class="sxs-lookup"><span data-stu-id="b33c5-1795">ACR</span></span>

* <span data-ttu-id="b33c5-1796">[BREAKING CHANGE] „--no-push“ in Befehl „acr build“ in reines Flag geändert</span><span class="sxs-lookup"><span data-stu-id="b33c5-1796">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="b33c5-1797">Befehle `show` und `update` unter Gruppe `acr repository` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1797">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="b33c5-1798">`--detail`-Flag für `show-manifests` und `show-tags` hinzugefügt, um ausführlichere Informationen anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="b33c5-1798">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="b33c5-1799">Parameter `--image` zur Unterstützung des Abrufs von Builddetails oder Protokollen anhand eines Images hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1799">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="b33c5-1800">ACS</span><span class="sxs-lookup"><span data-stu-id="b33c5-1800">ACS</span></span>

* <span data-ttu-id="b33c5-1801">`az aks create` so geändert, dass mit Fehler beendet wird, wenn `--max-pods` kleiner als 5 ist</span><span class="sxs-lookup"><span data-stu-id="b33c5-1801">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="b33c5-1802">AppService</span><span class="sxs-lookup"><span data-stu-id="b33c5-1802">AppService</span></span>

* <span data-ttu-id="b33c5-1803">Unterstützung für PremiumV2-SKUs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1803">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="b33c5-1804">Batch</span><span class="sxs-lookup"><span data-stu-id="b33c5-1804">Batch</span></span>

* <span data-ttu-id="b33c5-1805">Korrektur eines Fehlers bei der Verwendung von Anmeldeinformationen im Cloud Shell-Modus</span><span class="sxs-lookup"><span data-stu-id="b33c5-1805">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="b33c5-1806">JSON-Eingabe so geändert, dass Groß-/Kleinschreibung nicht beachtet wird</span><span class="sxs-lookup"><span data-stu-id="b33c5-1806">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="b33c5-1807">Batch KI</span><span class="sxs-lookup"><span data-stu-id="b33c5-1807">Batch AI</span></span>

* <span data-ttu-id="b33c5-1808">Befehl `az batchai job exec` korrigiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-1808">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="b33c5-1809">Container</span><span class="sxs-lookup"><span data-stu-id="b33c5-1809">Container</span></span>

* <span data-ttu-id="b33c5-1810">Anforderung von Benutzername und Kennwort für Nicht-DockerHub-Registrierungen entfernt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1810">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="b33c5-1811">Fehler beim Erstellen von Containergruppen aus YAML-Datei behoben</span><span class="sxs-lookup"><span data-stu-id="b33c5-1811">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="b33c5-1812">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="b33c5-1812">Network</span></span>

* <span data-ttu-id="b33c5-1813">Unterstützung für `--no-wait` zu `network nic [create|update|delete]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1813">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="b33c5-1814">`network nic wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1814">Added `network nic wait`</span></span>
* <span data-ttu-id="b33c5-1815">`--ids`-Argument für `network vnet [subnet|peering] list` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-1815">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="b33c5-1816">`--include-default`-Flag hinzugefügt, um Standardsicherheitsregeln in die Ausgabe von `network nsg rule list` aufzunehmen</span><span class="sxs-lookup"><span data-stu-id="b33c5-1816">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="b33c5-1817">Resource</span><span class="sxs-lookup"><span data-stu-id="b33c5-1817">Resource</span></span>

* <span data-ttu-id="b33c5-1818">Unterstützung für `--no-wait` zu `group deployment delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1818">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="b33c5-1819">Unterstützung für `--no-wait` zu `deployment delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1819">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="b33c5-1820">Befehl `deployment wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1820">Added `deployment wait` command</span></span>
* <span data-ttu-id="b33c5-1821">Problem behoben, aufgrund dessen die `az deployment`-Befehle auf Abonnementebene fälschlicherweise für Profil „2017-03-09-profile“ angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="b33c5-1821">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="b33c5-1822">SQL</span><span class="sxs-lookup"><span data-stu-id="b33c5-1822">SQL</span></span>

* <span data-ttu-id="b33c5-1823">Fehler „Der angegebene Ressourcengruppenname ... entsprach nicht dem Namen in der URL“ beim Angeben des Namens des Pools für elastische Datenbanken für `sql db copy`-und `sql db replica create`-Befehle behoben</span><span class="sxs-lookup"><span data-stu-id="b33c5-1823">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="b33c5-1824">Konfigurieren des Standard-SQL Servers durch Ausführen von `az configure --defaults sql-server=<name>` zulässig</span><span class="sxs-lookup"><span data-stu-id="b33c5-1824">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="b33c5-1825">Tabellenformatierer für Befehle `sql server`, `sql server firewall-rule`, `sql list-usages` und `sql show-usage` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1825">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="b33c5-1826">Storage</span><span class="sxs-lookup"><span data-stu-id="b33c5-1826">Storage</span></span>

* <span data-ttu-id="b33c5-1827">`pageRanges`-Eigenschaft zu `storage blob show`-Ausgabe hinzugefügt, die für Seitenblobs ausgefüllt wird</span><span class="sxs-lookup"><span data-stu-id="b33c5-1827">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="b33c5-1828">VM</span><span class="sxs-lookup"><span data-stu-id="b33c5-1828">VM</span></span>

* <span data-ttu-id="b33c5-1829">[BREAKING CHANGE]`vmss create` so geändert, dass `Standard_DS1_v2` als standardmäßige Instanzgröße verwendet wird</span><span class="sxs-lookup"><span data-stu-id="b33c5-1829">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="b33c5-1830">Unterstützung für `--no-wait` zu `vm extension [set|delete]` und `vmss extension [set|delete]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1830">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="b33c5-1831">`vm extension wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1831">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="b33c5-1832">3\. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="b33c5-1832">July 3, 2018</span></span>

<span data-ttu-id="b33c5-1833">Version 2.0.41</span><span class="sxs-lookup"><span data-stu-id="b33c5-1833">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="b33c5-1834">AKS</span><span class="sxs-lookup"><span data-stu-id="b33c5-1834">AKS</span></span>

* <span data-ttu-id="b33c5-1835">Überwachung geändert, sodass Abonnement-ID verwendet wird</span><span class="sxs-lookup"><span data-stu-id="b33c5-1835">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="b33c5-1836">3\. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="b33c5-1836">July 3, 2018</span></span>

<span data-ttu-id="b33c5-1837">Version 2.0.40</span><span class="sxs-lookup"><span data-stu-id="b33c5-1837">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="b33c5-1838">Core</span><span class="sxs-lookup"><span data-stu-id="b33c5-1838">Core</span></span>

* <span data-ttu-id="b33c5-1839">Neuer Autorisierungscode-Flow für interaktive Anmeldung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1839">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="b33c5-1840">ACR</span><span class="sxs-lookup"><span data-stu-id="b33c5-1840">ACR</span></span>

* <span data-ttu-id="b33c5-1841">Abruf-Buildstatus hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1841">Added polling build status</span></span>
* <span data-ttu-id="b33c5-1842">Unterstützung für Enumerationswerte ohne Berücksichtigung von Groß-/Kleinschreibung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1842">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="b33c5-1843">Parameter `--top` und `--orderby` für `show-manifests` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1843">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="b33c5-1844">ACS</span><span class="sxs-lookup"><span data-stu-id="b33c5-1844">ACS</span></span>

* <span data-ttu-id="b33c5-1845">[BREAKING CHANGE] Standardmäßiges Aktivieren der rollenbasierten Zugriffssteuerung für Kubernetes</span><span class="sxs-lookup"><span data-stu-id="b33c5-1845">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="b33c5-1846">Argument `--disable-rbac` hinzugefügt und `--enable-rbac` als veraltet festgelegt, da es nun der Standard ist</span><span class="sxs-lookup"><span data-stu-id="b33c5-1846">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="b33c5-1847">Optionen für Befehl `aks browse` wurden aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1847">Updated options for `aks browse` command.</span></span> <span data-ttu-id="b33c5-1848">Unterstützung für `--listen-port` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1848">Added `--listen-port` support</span></span>
* <span data-ttu-id="b33c5-1849">Standardmäßiges Helm-Diagrammpaket für Befehl `aks install-connector` wurde aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1849">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="b33c5-1850">Verwenden von „virtual-kubelet-for-aks-latest.tgz“</span><span class="sxs-lookup"><span data-stu-id="b33c5-1850">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="b33c5-1851">Befehle `aks enable-addons` und `aks disable-addons` zum Aktualisieren eines vorhandenen Clusters hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1851">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="b33c5-1852">AppService</span><span class="sxs-lookup"><span data-stu-id="b33c5-1852">AppService</span></span>

* <span data-ttu-id="b33c5-1853">Unterstützung für das Deaktivieren der Identität über `webapp identity remove` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1853">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="b33c5-1854">`preview`-Tag für Identitätsfunktion entfernt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1854">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="b33c5-1855">Backup</span><span class="sxs-lookup"><span data-stu-id="b33c5-1855">Backup</span></span>

* <span data-ttu-id="b33c5-1856">Moduldefinition aktualisiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-1856">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="b33c5-1857">Batch AI</span><span class="sxs-lookup"><span data-stu-id="b33c5-1857">BatchAI</span></span>

* <span data-ttu-id="b33c5-1858">Tabellenausgabe für Befehle `batchai cluster node list` und `batchai job node list` korrigiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-1858">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="b33c5-1859">Cloud</span><span class="sxs-lookup"><span data-stu-id="b33c5-1859">Cloud</span></span>

* <span data-ttu-id="b33c5-1860">Serversuffix `acr login` zu Cloudkonfiguration hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1860">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="b33c5-1861">Container</span><span class="sxs-lookup"><span data-stu-id="b33c5-1861">Container</span></span>

* <span data-ttu-id="b33c5-1862">`container create` zu Standard für Vorgang mit langer Ausführungsdauer geändert</span><span class="sxs-lookup"><span data-stu-id="b33c5-1862">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="b33c5-1863">Log Analytics-Parameter `--log-analytics-workspace` und `--log-analytics-workspace-key` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1863">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="b33c5-1864">Parameter `--protocol` zum Festlegen des zu verwendenden Netzwerkprotokolls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1864">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="b33c5-1865">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="b33c5-1865">Extension</span></span>

* <span data-ttu-id="b33c5-1866">`extension list-available` geändert, sodass nur mit der CLI-Version kompatible Erweiterungen angezeigt werden</span><span class="sxs-lookup"><span data-stu-id="b33c5-1866">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="b33c5-1867">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="b33c5-1867">Network</span></span>

* <span data-ttu-id="b33c5-1868">Problem behoben, aufgrund dessen bei Datensatztypen die Groß-/Kleinschreibung beachtet werden musste ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="b33c5-1868">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="b33c5-1869">Rdbms</span><span class="sxs-lookup"><span data-stu-id="b33c5-1869">Rdbms</span></span>

* <span data-ttu-id="b33c5-1870">Befehle vom Typ `[postgres|myql] server vnet-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1870">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="b33c5-1871">Resource</span><span class="sxs-lookup"><span data-stu-id="b33c5-1871">Resource</span></span>

* <span data-ttu-id="b33c5-1872">Neue Vorgangsgruppe `deployment` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1872">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="b33c5-1873">VM</span><span class="sxs-lookup"><span data-stu-id="b33c5-1873">VM</span></span>

* <span data-ttu-id="b33c5-1874">Unterstützung für das Entfernen der vom System zugewiesenen Identität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1874">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="b33c5-1875">25. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="b33c5-1875">June 25, 2018</span></span>

<span data-ttu-id="b33c5-1876">Version 2.0.39</span><span class="sxs-lookup"><span data-stu-id="b33c5-1876">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="b33c5-1877">Befehlszeilenschnittstelle (CLI)</span><span class="sxs-lookup"><span data-stu-id="b33c5-1877">CLI</span></span>

* <span data-ttu-id="b33c5-1878">Dateieinschränkung in MSI-Installer aktualisiert, um Problem mit der Erweiterungsinstallation zu beheben</span><span class="sxs-lookup"><span data-stu-id="b33c5-1878">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="b33c5-1879">19. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="b33c5-1879">June 19, 2018</span></span>

<span data-ttu-id="b33c5-1880">Version 2.0.38</span><span class="sxs-lookup"><span data-stu-id="b33c5-1880">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="b33c5-1881">Core</span><span class="sxs-lookup"><span data-stu-id="b33c5-1881">Core</span></span>

* <span data-ttu-id="b33c5-1882">Globale Unterstützung für `--subscription` zu den meisten Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1882">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="b33c5-1883">ACR</span><span class="sxs-lookup"><span data-stu-id="b33c5-1883">ACR</span></span>

* <span data-ttu-id="b33c5-1884">`azure-storage-blob` als Abhängigkeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1884">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="b33c5-1885">CPU-Standardkonfiguration für `acr build-task create` geändert, sodass zwei Kerne verwendet werden</span><span class="sxs-lookup"><span data-stu-id="b33c5-1885">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="b33c5-1886">ACS</span><span class="sxs-lookup"><span data-stu-id="b33c5-1886">ACS</span></span>

* <span data-ttu-id="b33c5-1887">Optionen des Befehls `aks use-dev-spaces` wurden aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1887">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="b33c5-1888">Unterstützung für `--update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1888">Added `--update` support</span></span>
* <span data-ttu-id="b33c5-1889">`aks get-credentials --admin` geändert, sodass der Benutzerkontext in `$HOME/.kube/config` ersetzt wird</span><span class="sxs-lookup"><span data-stu-id="b33c5-1889">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="b33c5-1890">Schreibgeschützte `nodeResourceGroup`-Eigenschaft in verwalteten Clustern verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="b33c5-1890">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="b33c5-1891">Befehlsfehler `acs browse` korrigiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-1891">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="b33c5-1892">`--connector-name` für `aks install-connector`, `aks upgrade-connector` und `aks remove-connector` als optional festgelegt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1892">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="b33c5-1893">Neue Azure Container Instances-Regionen für `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1893">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="b33c5-1894">Normalisierter Speicherort im Helm-Versionsnamen und Knotenname zu `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1894">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="b33c5-1895">AppService</span><span class="sxs-lookup"><span data-stu-id="b33c5-1895">AppService</span></span>

* <span data-ttu-id="b33c5-1896">Unterstützung für neuere Versionen von „urllib“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1896">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="b33c5-1897">Unterstützung der Verwendung eines App Service-Plans aus externen Ressourcengruppen zu `functionapp create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1897">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="b33c5-1898">Batch</span><span class="sxs-lookup"><span data-stu-id="b33c5-1898">Batch</span></span>

* <span data-ttu-id="b33c5-1899">`azure-batch-extensions`-Abhängigkeit entfernt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1899">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="b33c5-1900">Batch KI</span><span class="sxs-lookup"><span data-stu-id="b33c5-1900">Batch AI</span></span>

* <span data-ttu-id="b33c5-1901">Unterstützung für Arbeitsbereiche wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1901">Added support for workspaces.</span></span> <span data-ttu-id="b33c5-1902">Arbeitsbereiche ermöglichen das Zusammenfassen von Clustern, Dateiservern und Experimenten in Gruppen ohne Beschränkung der Anzahl von Ressourcen, die erstellt werden können.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1902">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="b33c5-1903">Unterstützung für Experimente wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1903">Added support for experiments.</span></span> <span data-ttu-id="b33c5-1904">Experimente ermöglichen das Zusammenfassen von Aufträgen in Sammlungen ohne Beschränkung der Anzahl von erstellten Aufträgen.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1904">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="b33c5-1905">Unterstützung für das Konfigurieren von `/dev/shm` für Aufträge hinzugefügt, die in einem Docker-Container ausgeführt werden</span><span class="sxs-lookup"><span data-stu-id="b33c5-1905">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="b33c5-1906">Die Befehle `batchai cluster node exec` und `batchai job node exec` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1906">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="b33c5-1907">Diese Befehle ermöglichen die Ausführung aller Befehle direkt auf Knoten und bieten Funktionen zur Portweiterleitung.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1907">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="b33c5-1908">Unterstützung für `--ids` zu `batchai`-Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1908">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="b33c5-1909">[BREAKING CHANGE] Alle Cluster und Dateiserver müssen unter Arbeitsbereichen erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1909">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="b33c5-1910">[BREAKING CHANGE] Aufträge müssen unter Experimenten erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1910">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="b33c5-1911">[BREAKING CHANGE]`--nfs-resource-group` wurde aus den Befehlen `cluster create` und `job create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1911">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="b33c5-1912">Geben Sie zum Bereitstellen eines NFS, das einem anderen Arbeitsbereich/einer anderen Ressourcengruppe angehört, die ARM-ID des Dateiservers über die Option `--nfs` an.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1912">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="b33c5-1913">[BREAKING CHANGE]`--cluster-resource-group` wurde aus dem Befehl `job create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1913">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="b33c5-1914">Geben Sie zum Übermitteln eines Auftrags, der einem anderen Arbeitsbereich/einer anderen Ressourcengruppe angehört, die ARM-ID des Clusters über die Option `--cluster` an.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1914">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="b33c5-1915">[BREAKING CHANGE] Attribut `location` wurde aus Aufträgen, Clustern und Dateiservern entfernt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1915">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="b33c5-1916">„Location“ ist jetzt ein Attribut eines Arbeitsbereichs.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1916">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="b33c5-1917">[BREAKING CHANGE]`--location` wurde aus den Befehlen `job create`, `cluster create` und `file-server create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1917">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="b33c5-1918">[BREAKING CHANGE] Namen von Kurzoptionen wurden geändert, um die Schnittstelle konsistenter zu machen:</span><span class="sxs-lookup"><span data-stu-id="b33c5-1918">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="b33c5-1919">[`--config`, `-c`] in [`--config-file`, `-f`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1919">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="b33c5-1920">[`--cluster`, `-r`] in [`--cluster`, `-c`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1920">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="b33c5-1921">[`--cluster`, `-n`] in [`--cluster`, `-c`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1921">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="b33c5-1922">[`--job`, `-n`] in [`--job`, `-j`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1922">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="b33c5-1923">Karten</span><span class="sxs-lookup"><span data-stu-id="b33c5-1923">Maps</span></span>

* <span data-ttu-id="b33c5-1924">[BREAKING CHANGE]`maps account create` wurde so geändert, dass Nutzungsbedingungen entweder durch interaktive Eingabeaufforderung oder `--accept-tos`-Flag akzeptiert werden müssen.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1924">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="b33c5-1925">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="b33c5-1925">Network</span></span>

* <span data-ttu-id="b33c5-1926">Unterstützung für `https` zu `network lb probe create` hinzugefügt [Nr. 6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="b33c5-1926">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="b33c5-1927">Problem behoben, aufgrund dessen die Groß-/Kleinschreibung von `--endpoint-status` berücksichtigt wurde.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1927">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="b33c5-1928">#6502</span><span class="sxs-lookup"><span data-stu-id="b33c5-1928">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="b33c5-1929">Reservations</span><span class="sxs-lookup"><span data-stu-id="b33c5-1929">Reservations</span></span>

* <span data-ttu-id="b33c5-1930">[BREAKING CHANGE] Erforderlicher Parameter `ReservedResourceType` zu `reservations catalog show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1930">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="b33c5-1931">Parameter `Location` zu `reservations catalog show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1931">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="b33c5-1932">[BREAKING CHANGE]`kind` aus `ReservationProperties` entfernt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1932">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="b33c5-1933">[BREAKING CHANGE]`capabilities` wurde in `Catalog` in `sku_properties` umbenannt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1933">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="b33c5-1934">[BREAKING CHANGE] Eigenschaften `size` und `tier` aus `Catalog` entfernt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1934">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="b33c5-1935">Parameter `InstanceFlexibility` zu `reservations reservation update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1935">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="b33c5-1936">Role</span><span class="sxs-lookup"><span data-stu-id="b33c5-1936">Role</span></span>

* <span data-ttu-id="b33c5-1937">Fehlerbehandlung verbessert</span><span class="sxs-lookup"><span data-stu-id="b33c5-1937">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="b33c5-1938">SQL</span><span class="sxs-lookup"><span data-stu-id="b33c5-1938">SQL</span></span>

* <span data-ttu-id="b33c5-1939">Verwirrender Fehler behoben, der beim Ausführen von `az sql db list-editions` für einen Ort auftrat, der für Ihr Abonnement nicht verfügbar ist</span><span class="sxs-lookup"><span data-stu-id="b33c5-1939">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="b33c5-1940">Storage</span><span class="sxs-lookup"><span data-stu-id="b33c5-1940">Storage</span></span>

* <span data-ttu-id="b33c5-1941">Lesbarkeit der Tabellenausgabe für `storage blob download` verbessert</span><span class="sxs-lookup"><span data-stu-id="b33c5-1941">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="b33c5-1942">VM</span><span class="sxs-lookup"><span data-stu-id="b33c5-1942">VM</span></span>

* <span data-ttu-id="b33c5-1943">Verbesserte Einschränkung der VM-Größenüberprüfung für Unterstützung von beschleunigten Netzwerken in `vm create`</span><span class="sxs-lookup"><span data-stu-id="b33c5-1943">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="b33c5-1944">Warnung für `vmss create` hinzugefügt, dass die VM-Standardgröße von `Standard_D1_v2` auf `Standard_DS1_v2` umgestellt wird</span><span class="sxs-lookup"><span data-stu-id="b33c5-1944">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="b33c5-1945">`--force-update` zu `[vm|vmss] extension set` hinzugefügt, um die Erweiterung auch dann zu aktualisieren, wenn die Konfiguration nicht geändert wurde</span><span class="sxs-lookup"><span data-stu-id="b33c5-1945">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="b33c5-1946">13. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="b33c5-1946">June 13, 2018</span></span>

<span data-ttu-id="b33c5-1947">Version 2.0.37</span><span class="sxs-lookup"><span data-stu-id="b33c5-1947">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="b33c5-1948">Core</span><span class="sxs-lookup"><span data-stu-id="b33c5-1948">Core</span></span>

* <span data-ttu-id="b33c5-1949">Verbesserte interaktive Telemetrie</span><span class="sxs-lookup"><span data-stu-id="b33c5-1949">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="b33c5-1950">13. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="b33c5-1950">June 13, 2018</span></span>

<span data-ttu-id="b33c5-1951">Version 2.0.36</span><span class="sxs-lookup"><span data-stu-id="b33c5-1951">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="b33c5-1952">AKS</span><span class="sxs-lookup"><span data-stu-id="b33c5-1952">AKS</span></span>

* <span data-ttu-id="b33c5-1953">Zusätzliche erweiterte Netzwerkoptionen zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1953">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="b33c5-1954">Argumente zu `aks create` zum Aktivieren der Überwachung und HTTP-Routing hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1954">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="b33c5-1955">Argument `--no-ssh-key` zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1955">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="b33c5-1956">Argument `--enable-rbac` zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1956">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="b33c5-1957">[VORSCHAUVERSION] Unterstützung für Azure Active Directory-Authentifizierung zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1957">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="b33c5-1958">AppService</span><span class="sxs-lookup"><span data-stu-id="b33c5-1958">AppService</span></span>

* <span data-ttu-id="b33c5-1959">Problem mit inkompatiblen urllib-Versionen behoben</span><span class="sxs-lookup"><span data-stu-id="b33c5-1959">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="b33c5-1960">5\. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="b33c5-1960">June 5, 2018</span></span>

<span data-ttu-id="b33c5-1961">Version 2.0.35</span><span class="sxs-lookup"><span data-stu-id="b33c5-1961">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="b33c5-1962">Interactive</span><span class="sxs-lookup"><span data-stu-id="b33c5-1962">Interactive</span></span>

* <span data-ttu-id="b33c5-1963">Grenzwerte für die Abhängigkeiten des interaktiven Modus hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1963">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="b33c5-1964">5\. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="b33c5-1964">June 5, 2018</span></span>

<span data-ttu-id="b33c5-1965">Version 2.0.34</span><span class="sxs-lookup"><span data-stu-id="b33c5-1965">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="b33c5-1966">Core</span><span class="sxs-lookup"><span data-stu-id="b33c5-1966">Core</span></span>

* <span data-ttu-id="b33c5-1967">Unterstützung für mandantenübergreifende Ressourcenverweise hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1967">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="b33c5-1968">Verbesserte Zuverlässigkeit bei Telemetrieuploads</span><span class="sxs-lookup"><span data-stu-id="b33c5-1968">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="b33c5-1969">ACR</span><span class="sxs-lookup"><span data-stu-id="b33c5-1969">ACR</span></span>

* <span data-ttu-id="b33c5-1970">Unterstützung für VSTS als Remotequellort hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1970">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="b33c5-1971">Befehl `acr import` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1971">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="b33c5-1972">AKS</span><span class="sxs-lookup"><span data-stu-id="b33c5-1972">AKS</span></span>

* <span data-ttu-id="b33c5-1973">`aks get-credentials` wurde geändert, um die Kube-Konfigurationsdatei mit sichereren Dateisystemberechtigungen zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1973">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="b33c5-1974">Batch</span><span class="sxs-lookup"><span data-stu-id="b33c5-1974">Batch</span></span>

* <span data-ttu-id="b33c5-1975">Fehler bei der Formatierung der Poollistentabelle behoben [[Problem 4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="b33c5-1975">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="b33c5-1976">IoT</span><span class="sxs-lookup"><span data-stu-id="b33c5-1976">IOT</span></span>

* <span data-ttu-id="b33c5-1977">Unterstützung für das Erstellen von IoT Hub-Instanzen im Tarif „Basic“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1977">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="b33c5-1978">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="b33c5-1978">Network</span></span>

* <span data-ttu-id="b33c5-1979">`network vnet peering` wurde verbessert.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1979">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="b33c5-1980">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="b33c5-1980">Policy Insights</span></span>

* <span data-ttu-id="b33c5-1981">Erstrelease</span><span class="sxs-lookup"><span data-stu-id="b33c5-1981">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="b33c5-1982">ARM</span><span class="sxs-lookup"><span data-stu-id="b33c5-1982">ARM</span></span>

* <span data-ttu-id="b33c5-1983">Befehle vom Typ `account management-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1983">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="b33c5-1984">SQL</span><span class="sxs-lookup"><span data-stu-id="b33c5-1984">SQL</span></span>

* <span data-ttu-id="b33c5-1985">Neue Befehle für verwaltete Instanzen hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="b33c5-1985">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="b33c5-1986">Neue Befehle für verwaltete Datenbanken hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="b33c5-1986">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="b33c5-1987">Storage</span><span class="sxs-lookup"><span data-stu-id="b33c5-1987">Storage</span></span>

* <span data-ttu-id="b33c5-1988">Zusätzliche MimeTypes für JSON und JavaScript hinzugefügt (abzuleiten aus Dateierweiterungen)</span><span class="sxs-lookup"><span data-stu-id="b33c5-1988">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="b33c5-1989">VM</span><span class="sxs-lookup"><span data-stu-id="b33c5-1989">VM</span></span>

* <span data-ttu-id="b33c5-1990">`vm list-skus` wurde geändert, um feste Spalten zu verwenden und eine Warnung hinzuzufügen, dass `Tier` und `Size` entfernt werden.</span><span class="sxs-lookup"><span data-stu-id="b33c5-1990">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="b33c5-1991">Option `--accelerated-networking` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1991">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="b33c5-1992">`--tags` zu `identity create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1992">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="b33c5-1993">22. Mai 2018</span><span class="sxs-lookup"><span data-stu-id="b33c5-1993">May 22, 2018</span></span>

<span data-ttu-id="b33c5-1994">Version 2.0.33</span><span class="sxs-lookup"><span data-stu-id="b33c5-1994">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="b33c5-1995">Core</span><span class="sxs-lookup"><span data-stu-id="b33c5-1995">Core</span></span>

* <span data-ttu-id="b33c5-1996">Unterstützung für das Erweitern von `@` in Dateinamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1996">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="b33c5-1997">ACS</span><span class="sxs-lookup"><span data-stu-id="b33c5-1997">ACS</span></span>

* <span data-ttu-id="b33c5-1998">Neue Dev Spaces-Befehle `aks use-dev-spaces` und `aks remove-dev-spaces` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-1998">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="b33c5-1999">Tippfehler in Hilfemeldung korrigiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-1999">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="b33c5-2000">AppService</span><span class="sxs-lookup"><span data-stu-id="b33c5-2000">AppService</span></span>

* <span data-ttu-id="b33c5-2001">Verbesserte generische Aktualisierungsbefehle</span><span class="sxs-lookup"><span data-stu-id="b33c5-2001">Improved generic update commands</span></span>
* <span data-ttu-id="b33c5-2002">Asynchrone Unterstützung für `webapp deployment source config-zip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2002">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="b33c5-2003">Container</span><span class="sxs-lookup"><span data-stu-id="b33c5-2003">Container</span></span>

* <span data-ttu-id="b33c5-2004">Unterstützung für das Exportieren einer Containergruppe im YAML-Format hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2004">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="b33c5-2005">Unterstützung für die Verwendung einer YAML-Datei zum Erstellen/Aktualisieren einer Containergruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2005">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="b33c5-2006">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="b33c5-2006">Extension</span></span>

* <span data-ttu-id="b33c5-2007">Verbesserte Entfernung von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="b33c5-2007">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="b33c5-2008">Interactive</span><span class="sxs-lookup"><span data-stu-id="b33c5-2008">Interactive</span></span>

* <span data-ttu-id="b33c5-2009">Protokollierung geändert, um Parser für Abschlüsse zu deaktivieren</span><span class="sxs-lookup"><span data-stu-id="b33c5-2009">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="b33c5-2010">Verbesserte Verarbeitung beschädigter Hilfscaches</span><span class="sxs-lookup"><span data-stu-id="b33c5-2010">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="b33c5-2011">KeyVault</span><span class="sxs-lookup"><span data-stu-id="b33c5-2011">KeyVault</span></span>

* <span data-ttu-id="b33c5-2012">keyvault-Befehle wurden korrigiert, damit sie in Cloud Shell oder auf virtuellen Computern mit Identität verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2012">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="b33c5-2013">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="b33c5-2013">Network</span></span>

* <span data-ttu-id="b33c5-2014">Problem behoben, aufgrund dessen `network watcher show-topology` nicht mit einem VNET und/oder Subnetznamen verwendet werden konnte ([#6326](https://github.com/Azure/azure-cli/issues/6326))</span><span class="sxs-lookup"><span data-stu-id="b33c5-2014">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="b33c5-2015">Problem behoben, aufgrund dessen einige `network watcher`-Befehle fälschlicherweise angaben, dass Network Watcher nicht für bestimmte Regionen aktiviert ist ([#6264](https://github.com/Azure/azure-cli/issues/6264))</span><span class="sxs-lookup"><span data-stu-id="b33c5-2015">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="b33c5-2016">SQL</span><span class="sxs-lookup"><span data-stu-id="b33c5-2016">SQL</span></span>

* <span data-ttu-id="b33c5-2017">[BREAKING CHANGE] Von den Befehlen `db` und `dw` zurückgegebene Antwortobjekte geändert:</span><span class="sxs-lookup"><span data-stu-id="b33c5-2017">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="b33c5-2018">Eigenschaft `serviceLevelObjective` in `currentServiceObjectiveName` umbenannt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2018">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="b33c5-2019">Eigenschaften `currentServiceObjectiveId` und `requestedServiceObjectiveId` entfernt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2019">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="b33c5-2020">Eigenschaft `maxSizeBytes` geändert (ist nun keine Zeichenfolge mehr, sondern ein Ganzzahlwert)</span><span class="sxs-lookup"><span data-stu-id="b33c5-2020">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="b33c5-2021">[BREAKING CHANGE] Die folgenden `db`- und `dw`-Eigenschaften wurden geändert und sind jetzt schreibgeschützt:</span><span class="sxs-lookup"><span data-stu-id="b33c5-2021">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="b33c5-2022">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2022">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="b33c5-2023">Verwenden Sie zum Aktualisieren den Parameter `--service-objective`, oder legen Sie die Eigenschaft `sku.name` fest.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2023">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="b33c5-2024">`edition`.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2024">`edition`.</span></span> <span data-ttu-id="b33c5-2025">Verwenden Sie zum Aktualisieren den Parameter `--edition`, oder legen Sie die Eigenschaft `sku.tier` fest.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2025">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="b33c5-2026">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2026">`elasticPoolName`.</span></span> <span data-ttu-id="b33c5-2027">Verwenden Sie zum Aktualisieren den Parameter `--elastic-pool`, oder legen Sie die Eigenschaft `elasticPoolId` fest.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2027">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="b33c5-2028">[BREAKING CHANGE] Die folgenden `elastic-pool`-Eigenschaften wurden geändert und sind jetzt schreibgeschützt:</span><span class="sxs-lookup"><span data-stu-id="b33c5-2028">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="b33c5-2029">`edition`.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2029">`edition`.</span></span> <span data-ttu-id="b33c5-2030">Verwenden Sie zum Aktualisieren den Parameter `--edition`.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2030">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="b33c5-2031">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2031">`dtu`.</span></span> <span data-ttu-id="b33c5-2032">Verwenden Sie zum Aktualisieren den Parameter `--capacity`.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2032">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="b33c5-2033">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2033">`databaseDtuMin`.</span></span> <span data-ttu-id="b33c5-2034">Verwenden Sie zum Aktualisieren den Parameter `--db-min-capacity`.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2034">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="b33c5-2035">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2035">`databaseDtuMax`.</span></span> <span data-ttu-id="b33c5-2036">Verwenden Sie zum Aktualisieren den Parameter `--db-max-capacity`.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2036">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="b33c5-2037">Die Parameter `--family` und `--capacity` wurden zu den `db`-, `dw`- und `elastic-pool`-Befehlen hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2037">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="b33c5-2038">Den `db`-, `dw`- und `elastic-pool`-Befehlen wurden Tabellenformatierer hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2038">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="b33c5-2039">Storage</span><span class="sxs-lookup"><span data-stu-id="b33c5-2039">Storage</span></span>

* <span data-ttu-id="b33c5-2040">Vervollständigung für das Argument `--account-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2040">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="b33c5-2041">Problem mit `storage entity query` behoben</span><span class="sxs-lookup"><span data-stu-id="b33c5-2041">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="b33c5-2042">VM</span><span class="sxs-lookup"><span data-stu-id="b33c5-2042">VM</span></span>

* <span data-ttu-id="b33c5-2043">[BREAKING CHANGE]`--write-accelerator` aus `vm create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2043">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="b33c5-2044">Die gleiche Unterstützung kann über `vm update` oder `vm disk attach` erzielt werden.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2044">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="b33c5-2045">Erweiterungsimageabgleich in `[vm|vmss] extension` korrigiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-2045">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="b33c5-2046">`--boot-diagnostics-storage` zu `vm create` zur Erfassung des Startprotokolls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2046">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="b33c5-2047">`--license-type` zu `[vm|vmss] update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2047">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="b33c5-2048">7\. Mai 2018</span><span class="sxs-lookup"><span data-stu-id="b33c5-2048">May 7, 2018</span></span>

<span data-ttu-id="b33c5-2049">Version 2.0.32</span><span class="sxs-lookup"><span data-stu-id="b33c5-2049">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="b33c5-2050">Core</span><span class="sxs-lookup"><span data-stu-id="b33c5-2050">Core</span></span>

* <span data-ttu-id="b33c5-2051">Ein Ausnahmefehler wurde behoben, der beim Abrufen von Geheimnissen aus einem Dienstprinzipalkonto mit Zertifikat auftrat.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2051">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="b33c5-2052">Eingeschränkte Unterstützung für positionelle Argumente hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2052">Added limited support for positional arguments</span></span>
* <span data-ttu-id="b33c5-2053">Problem behoben, aufgrund dessen `--query` nicht mit `--ids` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="b33c5-2053">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="b33c5-2054">#5591</span><span class="sxs-lookup"><span data-stu-id="b33c5-2054">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="b33c5-2055">Pipingszenarien von Befehlen bei Verwendung von `--ids` verbessert</span><span class="sxs-lookup"><span data-stu-id="b33c5-2055">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="b33c5-2056">Unterstützt `-o tsv` mit angegebener Abfrage bzw. `-o json` ohne angegeben Abfrage</span><span class="sxs-lookup"><span data-stu-id="b33c5-2056">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="b33c5-2057">Befehlsvorschläge bei Fehler hinzugefügt, wenn Befehle Tippfehler enthielten</span><span class="sxs-lookup"><span data-stu-id="b33c5-2057">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="b33c5-2058">Fehler bei der Eingabe von `az ''` behandelt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2058">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="b33c5-2059">Unterstützung für benutzerdefinierte Ressourcentypen für Befehlsmodule und -erweiterungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2059">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="b33c5-2060">ACR</span><span class="sxs-lookup"><span data-stu-id="b33c5-2060">ACR</span></span>

* <span data-ttu-id="b33c5-2061">ACR Build-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2061">Added ACR Build commands</span></span>
* <span data-ttu-id="b33c5-2062">Fehlermeldungen vom Typ „Ressource nicht gefunden.“ verbessert</span><span class="sxs-lookup"><span data-stu-id="b33c5-2062">Improved resource not found error messages</span></span>
* <span data-ttu-id="b33c5-2063">Höhere Leistung bei der Ressourcenerstellung und optimierte Fehlerbehandlung</span><span class="sxs-lookup"><span data-stu-id="b33c5-2063">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="b33c5-2064">ACR-Anmeldung bei nicht standardmäßigen Konsolen und WSL optimiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-2064">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="b33c5-2065">Fehlermeldungen zu Repositorybefehlen optimiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-2065">Improved repository commands error messages</span></span>
* <span data-ttu-id="b33c5-2066">Tabellenspalten und -reihenfolge aktualisiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-2066">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="b33c5-2067">ACS</span><span class="sxs-lookup"><span data-stu-id="b33c5-2067">ACS</span></span>

* <span data-ttu-id="b33c5-2068">Warnung hinzugefügt, dass `az aks` eine Vorschauversion des Diensts ist</span><span class="sxs-lookup"><span data-stu-id="b33c5-2068">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="b33c5-2069">Berechtigungsproblem in `aks install-connector` behoben, wenn `--aci-resource-group` nicht angegeben wird</span><span class="sxs-lookup"><span data-stu-id="b33c5-2069">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="b33c5-2070">AMS</span><span class="sxs-lookup"><span data-stu-id="b33c5-2070">AMS</span></span>

* <span data-ttu-id="b33c5-2071">Erste Version: Verwalten von Azure Media Services-Ressourcen</span><span class="sxs-lookup"><span data-stu-id="b33c5-2071">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="b33c5-2072">AppService</span><span class="sxs-lookup"><span data-stu-id="b33c5-2072">Appservice</span></span>

* <span data-ttu-id="b33c5-2073">Ein Problem in `webapp delete` wurde behoben, das bei Angabe von `--slot` auftrat.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2073">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="b33c5-2074">`--runtime-version` aus `webapp auth update` entfernt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2074">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="b33c5-2075">Unterstützung für „min\_tls\_version“ und „https2.0“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2075">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="b33c5-2076">Unterstützung für mehrere Container hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2076">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="b33c5-2077">Batch KI</span><span class="sxs-lookup"><span data-stu-id="b33c5-2077">Batch AI</span></span>

* <span data-ttu-id="b33c5-2078">`batchai create cluster` wurde geändert, um die in der Konfigurationsdatei des Clusters konfigurierte VM-Priorität zu berücksichtigen.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2078">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="b33c5-2079">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="b33c5-2079">Cognitive Services</span></span>

* <span data-ttu-id="b33c5-2080">Tippfehler im Beispiel für `cognitiveservices account create` behoben [Nr. 5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="b33c5-2080">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="b33c5-2081">Nutzung</span><span class="sxs-lookup"><span data-stu-id="b33c5-2081">Consumption</span></span>

* <span data-ttu-id="b33c5-2082">Neue Befehle für Budget-API hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2082">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="b33c5-2083">Container</span><span class="sxs-lookup"><span data-stu-id="b33c5-2083">Container</span></span>

* <span data-ttu-id="b33c5-2084">`--registry-server` muss nicht mehr für `container create` angegeben werden, wenn ein Registrierungsserver im Imagenamen enthalten ist.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2084">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="b33c5-2085">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="b33c5-2085">Cosmos DB</span></span>

* <span data-ttu-id="b33c5-2086">VNET-Unterstützung für Azure CLI eingeführt: Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="b33c5-2086">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="b33c5-2087">DMS</span><span class="sxs-lookup"><span data-stu-id="b33c5-2087">DMS</span></span>

* <span data-ttu-id="b33c5-2088">Erste Version: Die Migration von SQL zu Azure SQL wird nun unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2088">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="b33c5-2089">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="b33c5-2089">Extension</span></span>

* <span data-ttu-id="b33c5-2090">Fehler behoben, aufgrund dessen Erweiterungsmetadaten nicht mehr angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="b33c5-2090">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="b33c5-2091">Interactive</span><span class="sxs-lookup"><span data-stu-id="b33c5-2091">Interactive</span></span>

* <span data-ttu-id="b33c5-2092">Interaktive Vervollständigung funktioniert nun auch mit positionellen Argumenten.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2092">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="b33c5-2093">Benutzerfreundlichere Ausgabe bei der Eingabe von '\'</span><span class="sxs-lookup"><span data-stu-id="b33c5-2093">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="b33c5-2094">Abschlüsse für Parameter ohne Hilfe korrigiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-2094">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="b33c5-2095">Beschreibungen für Befehlsgruppen korrigiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-2095">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="b33c5-2096">Labor</span><span class="sxs-lookup"><span data-stu-id="b33c5-2096">Lab</span></span>

* <span data-ttu-id="b33c5-2097">Regressionen aus Knack-Umwandlung korrigiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-2097">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="b33c5-2098">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="b33c5-2098">Network</span></span>

* <span data-ttu-id="b33c5-2099">[BREAKING CHANGE] Parameter `--ids` entfernt für:</span><span class="sxs-lookup"><span data-stu-id="b33c5-2099">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="b33c5-2100">Profil</span><span class="sxs-lookup"><span data-stu-id="b33c5-2100">Profile</span></span>

* <span data-ttu-id="b33c5-2101">Quellerkennung für `disk create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-2101">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="b33c5-2102">[BREAKING CHANGE]`--msi-port` und `--identity-port` entfernt, da sie nicht mehr verwendet werden</span><span class="sxs-lookup"><span data-stu-id="b33c5-2102">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="b33c5-2103">Tippfehler in kurzer Zusammenfassung für `account get-access-token` korrigiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-2103">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="b33c5-2104">Redis</span><span class="sxs-lookup"><span data-stu-id="b33c5-2104">Redis</span></span>

* <span data-ttu-id="b33c5-2105">`redis patch-schedule patch-schedule show` wurde durch `redis patch-schedule show` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2105">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="b33c5-2106">`redis list-all` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-2106">Deprecated `redis list-all`.</span></span> <span data-ttu-id="b33c5-2107">Diese Funktion wurde in `redis list` integriert.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2107">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="b33c5-2108">`redis import-method` wurde durch `redis import` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2108">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="b33c5-2109">Unterstützung für `--ids` zu verschiedenen Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2109">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="b33c5-2110">Role</span><span class="sxs-lookup"><span data-stu-id="b33c5-2110">Role</span></span>

* <span data-ttu-id="b33c5-2111">[BREAKING CHANGE] Veralteter Befehl `ad sp reset-credentials` entfernt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2111">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="b33c5-2112">Storage</span><span class="sxs-lookup"><span data-stu-id="b33c5-2112">Storage</span></span>

* <span data-ttu-id="b33c5-2113">Zulassen, dass das Ziel-SAS-Token für die Blobkopie auf die Quelle angewendet wird, wenn Quell-SAS und Kontoschlüssel nicht angegeben werden</span><span class="sxs-lookup"><span data-stu-id="b33c5-2113">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="b33c5-2114">Verfügbar gemacht: Socket-Timeout für Blobuploads und -downloads</span><span class="sxs-lookup"><span data-stu-id="b33c5-2114">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="b33c5-2115">Blobnamen, die mit Pfadtrennzeichen beginnen, als relative Pfade behandeln</span><span class="sxs-lookup"><span data-stu-id="b33c5-2115">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="b33c5-2116">Zulassen, dass `storage blob copy --source-sas` mit dem Abfragezeichen „?“ beginnt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2116">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="b33c5-2117">`storage entity query --marker` korrigiert, um Liste von Schlüsselwerten zu akzeptieren</span><span class="sxs-lookup"><span data-stu-id="b33c5-2117">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="b33c5-2118">VM</span><span class="sxs-lookup"><span data-stu-id="b33c5-2118">VM</span></span>

* <span data-ttu-id="b33c5-2119">Ungültige Erkennungslogik für nicht verwalteten Blob-URI korrigiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-2119">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="b33c5-2120">Unterstützung für Datenträgerverschlüsselung ohne vom Benutzer bereitgestellte Dienstprinzipale hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2120">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="b33c5-2121">[BREAKING CHANGE] Verwenden Sie nicht „ManagedIdentityExtension“ des virtuellen Computers für MSI-Unterstützung.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2121">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="b33c5-2122">Unterstützung für Entfernungsrichtlinie zu `vmss` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2122">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="b33c5-2123">[BREAKING CHANGE]`--ids` entfernt aus:</span><span class="sxs-lookup"><span data-stu-id="b33c5-2123">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="b33c5-2124">Unterstützung für Schreibbeschleunigung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2124">Added write accelerator support</span></span>
* <span data-ttu-id="b33c5-2125">`vmss perform-maintenance` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2125">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="b33c5-2126">`vm diagnostics set` korrigiert, um zuverlässig den Betriebssystemtyp des virtuellen Computers zu erkennen</span><span class="sxs-lookup"><span data-stu-id="b33c5-2126">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="b33c5-2127">`vm resize` geändert, um zu überprüfen, ob die angeforderte Größe von der derzeit festgelegten Größe abweicht, und nur bei einer Änderung eine Aktualisierung auszuführen</span><span class="sxs-lookup"><span data-stu-id="b33c5-2127">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="b33c5-2128">10. April 2018</span><span class="sxs-lookup"><span data-stu-id="b33c5-2128">April 10, 2018</span></span>

<span data-ttu-id="b33c5-2129">Version 2.0.31</span><span class="sxs-lookup"><span data-stu-id="b33c5-2129">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="b33c5-2130">ACR</span><span class="sxs-lookup"><span data-stu-id="b33c5-2130">ACR</span></span>

* <span data-ttu-id="b33c5-2131">Verbesserte Fehlerbehandlung für wincred-Fallback</span><span class="sxs-lookup"><span data-stu-id="b33c5-2131">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="b33c5-2132">ACS</span><span class="sxs-lookup"><span data-stu-id="b33c5-2132">ACS</span></span>

* <span data-ttu-id="b33c5-2133">Gültigkeit von per AKS erstellten SPNs in fünf Jahre geändert</span><span class="sxs-lookup"><span data-stu-id="b33c5-2133">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="b33c5-2134">AppService</span><span class="sxs-lookup"><span data-stu-id="b33c5-2134">Appservice</span></span>

* [BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="b33c5-2136">Nicht abgefangene Ausnahme für nicht vorhandene Web-App-Pläne behoben</span><span class="sxs-lookup"><span data-stu-id="b33c5-2136">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="b33c5-2137">Batch AI</span><span class="sxs-lookup"><span data-stu-id="b33c5-2137">BatchAI</span></span>

* <span data-ttu-id="b33c5-2138">Unterstützung für API 2018-03-01 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2138">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="b33c5-2139">Bereitstellung auf Auftragsebene</span><span class="sxs-lookup"><span data-stu-id="b33c5-2139">Job level mounting</span></span>
  - <span data-ttu-id="b33c5-2140">Umgebungsvariablen mit Geheimniswerten</span><span class="sxs-lookup"><span data-stu-id="b33c5-2140">Environment variables with secret values</span></span>
  - <span data-ttu-id="b33c5-2141">Einstellungen von Leistungsindikatoren</span><span class="sxs-lookup"><span data-stu-id="b33c5-2141">Performance counters settings</span></span>
  - <span data-ttu-id="b33c5-2142">Berichtstellung für auftragsspezifisches Pfadsegment</span><span class="sxs-lookup"><span data-stu-id="b33c5-2142">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="b33c5-2143">Unterstützung für Unterordner in Listendateien-API</span><span class="sxs-lookup"><span data-stu-id="b33c5-2143">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="b33c5-2144">Berichterstellung zur Nutzung und zu Grenzwerten</span><span class="sxs-lookup"><span data-stu-id="b33c5-2144">Usage and limits reporting</span></span>
  - <span data-ttu-id="b33c5-2145">Zulassen der Angabe des Cachetyps für NFS-Server</span><span class="sxs-lookup"><span data-stu-id="b33c5-2145">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="b33c5-2146">Unterstützung für benutzerdefinierte Images</span><span class="sxs-lookup"><span data-stu-id="b33c5-2146">Support for custom images</span></span>
  - <span data-ttu-id="b33c5-2147">Unterstützung für pyTorch-Toolkit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2147">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="b33c5-2148">Befehl `job wait` hinzugefügt, der das Warten auf die Auftragsfertigstellung ermöglicht und den Code für die Auftragsbeendigung meldet</span><span class="sxs-lookup"><span data-stu-id="b33c5-2148">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="b33c5-2149">Befehl `usage show` hinzugefügt, mit dem die aktuelle Nutzung von Batch KI-Ressourcen und die Grenzwerte für verschiedene Regionen aufgelistet werden</span><span class="sxs-lookup"><span data-stu-id="b33c5-2149">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="b33c5-2150">Nationale Clouds werden unterstützt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2150">National clouds are supported</span></span>
* <span data-ttu-id="b33c5-2151">Befehlszeilenargumente für Aufträge hinzugefügt, um das Bereitstellen von Dateisystemen auf Auftragsebene zusätzlich zu Konfigurationsdateien zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="b33c5-2151">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="b33c5-2152">Weitere Optionen zum Anpassen von Clustern hinzugefügt – VM-Priorität, Subnetz, anfängliche Knotenanzahl für Cluster mit automatischer Skalierung, Angeben eines benutzerdefinierten Images</span><span class="sxs-lookup"><span data-stu-id="b33c5-2152">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="b33c5-2153">Befehlszeilenoption zum Angeben des Cachetyps für NFS mit Verwaltung per Batch KI hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2153">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="b33c5-2154">Angeben der Bereitstellung von Dateisystemen in Konfigurationsdateien vereinfacht.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2154">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="b33c5-2155">Weglassen von Anmeldeinformationen für Azure-Dateifreigaben und Azure-Blobcontainer ist jetzt möglich. Die CLI füllt fehlende Anmeldeinformationen auf, indem der Speicherkontoschlüssel verwendet wird, der über Befehlszeilenparameter oder per Umgebungsvariable angegeben wird, oder der Schlüssel wird über Azure Storage abgefragt (sofern das Speicherkonto zum aktuellen Abonnement gehört).</span><span class="sxs-lookup"><span data-stu-id="b33c5-2155">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="b33c5-2156">Der Befehl zum Streamen von Auftragsdateien wird jetzt automatisch abgeschlossen, nachdem der Auftrag beendet ist (Erfolg, Fehler, Beendigung oder Löschung)</span><span class="sxs-lookup"><span data-stu-id="b33c5-2156">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="b33c5-2157">Verbesserte `table`-Ausgabe für `show`-Vorgänge</span><span class="sxs-lookup"><span data-stu-id="b33c5-2157">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="b33c5-2158">Option `--use-auto-storage` für die Clustererstellung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2158">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="b33c5-2159">Diese Option erleichtert die Verwaltung von Speicherkonten und die Bereitstellung von Azure-Dateifreigaben und Azure-Blobcontainern in Clustern.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2159">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="b33c5-2160">`--generate-ssh-keys` für `cluster create` und `file-server create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2160">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="b33c5-2161">Möglichkeit zum Angeben der Knotensetupaufgabe über die Befehlszeile</span><span class="sxs-lookup"><span data-stu-id="b33c5-2161">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="b33c5-2162">[BREAKING CHANGE] Befehl `job stream-file` und `job list-files` in die Gruppe `job file` verschoben</span><span class="sxs-lookup"><span data-stu-id="b33c5-2162">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="b33c5-2163">[BREAKING CHANGE]`--admin-user-name` im Befehl `file-server create` in `--user-name` umbenannt, um Einheitlichkeit mit dem Befehl `cluster create` zu erzielen</span><span class="sxs-lookup"><span data-stu-id="b33c5-2163">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="b33c5-2164">Abrechnung</span><span class="sxs-lookup"><span data-stu-id="b33c5-2164">Billing</span></span>

* <span data-ttu-id="b33c5-2165">Registrierungskontobefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2165">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="b33c5-2166">Nutzung</span><span class="sxs-lookup"><span data-stu-id="b33c5-2166">Consumption</span></span>

* <span data-ttu-id="b33c5-2167">Befehle vom Typ `marketplace` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2167">Added `marketplace` commands</span></span>
* <span data-ttu-id="b33c5-2168">[BREAKING CHANGE]`reservations summaries` in `reservation summary` umbenannt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2168">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="b33c5-2169">[BREAKING CHANGE]`reservations details` in `reservation detail` umbenannt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2169">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="b33c5-2170">[BREAKING CHANGE] Kurzoptionen `--reservation-order-id` und `--reservation-id` für `reservation`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2170">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="b33c5-2171">[BREAKING CHANGE]`--grain`-Kurzoptionen für `reservation summary`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2171">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="b33c5-2172">[BREAKING CHANGE]`--include-meter-details`-Kurzoptionen für `pricesheet`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2172">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="b33c5-2173">Container</span><span class="sxs-lookup"><span data-stu-id="b33c5-2173">Container</span></span>

* <span data-ttu-id="b33c5-2174">Parameter für die Volumebereitstellung für das Git-Repository hinzugefügt: `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` und `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="b33c5-2174">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="b33c5-2175">[#5926](https://github.com/Azure/azure-cli/issues/5926) behoben: Fehler bei `az container exec`, wenn „--container-name“ angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="b33c5-2175">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="b33c5-2176">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="b33c5-2176">Extension</span></span>

* <span data-ttu-id="b33c5-2177">Meldung für Distributionsüberprüfung in Debugebene geändert</span><span class="sxs-lookup"><span data-stu-id="b33c5-2177">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="b33c5-2178">Interactive</span><span class="sxs-lookup"><span data-stu-id="b33c5-2178">Interactive</span></span>

* <span data-ttu-id="b33c5-2179">Geändert: Verhinderung des Abschlusses bei nicht erkannten Befehlen</span><span class="sxs-lookup"><span data-stu-id="b33c5-2179">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="b33c5-2180">Ereignishooks vor und nach der Erstellung der Teilstruktur von Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2180">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="b33c5-2181">Abschluss für `--ids`-Parameter hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2181">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="b33c5-2182">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="b33c5-2182">Network</span></span>

* <span data-ttu-id="b33c5-2183">[#5936](https://github.com/Azure/azure-cli/issues/5936) behoben: `application-gateway create`-Tags konnten nicht festgelegt werden</span><span class="sxs-lookup"><span data-stu-id="b33c5-2183">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="b33c5-2184">Argument `--auth-certs` zum Anfügen von Authentifizierungszertifikaten für `application-gateway http-settings [create|update]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2184">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="b33c5-2185">#4910</span><span class="sxs-lookup"><span data-stu-id="b33c5-2185">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="b33c5-2186">`ddos-protection`-Befehle zum Erstellen von DDoS-Schutzplänen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2186">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="b33c5-2187">Unterstützung von `--ddos-protection-plan` für `vnet [create|update]` hinzugefügt, um das Zuordnen eines VNET zu einem DDoS-Schutzplan zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="b33c5-2187">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="b33c5-2188">Problem mit `--disable-bgp-route-propagation`-Flag in `network route-table [create|update]` behoben</span><span class="sxs-lookup"><span data-stu-id="b33c5-2188">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="b33c5-2189">Dummy-Argumente `--public-ip-address-type` und `--subnet-type` für `network lb [create|update]` entfernt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2189">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="b33c5-2190">Unterstützung für TXT-Datensätze mit RFC 1035-Escapesequenzen für `network dns zone [import|export]` und `network dns record-set txt add-record` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2190">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="b33c5-2191">Profil</span><span class="sxs-lookup"><span data-stu-id="b33c5-2191">Profile</span></span>

* <span data-ttu-id="b33c5-2192">Unterstützung für klassische Azure-Konten in `account list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2192">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="b33c5-2193">[BREAKING CHANGE]`--msi` & `--msi-port`-Argumente entfernt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2193">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="b33c5-2194">RDBMS</span><span class="sxs-lookup"><span data-stu-id="b33c5-2194">RDBMS</span></span>

* <span data-ttu-id="b33c5-2195">Befehl `georestore` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2195">Added `georestore` command</span></span>
* <span data-ttu-id="b33c5-2196">Speichergrößenbeschränkung aus Befehl `create` entfernt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2196">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="b33c5-2197">Resource</span><span class="sxs-lookup"><span data-stu-id="b33c5-2197">Resource</span></span>

* <span data-ttu-id="b33c5-2198">Unterstützung für `--metadata` zu `policy definition create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2198">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="b33c5-2199">Unterstützung von `--metadata`, `--set`, `--add`, `--remove` für `policy definition update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2199">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="b33c5-2200">SQL</span><span class="sxs-lookup"><span data-stu-id="b33c5-2200">SQL</span></span>

* <span data-ttu-id="b33c5-2201">`sql elastic-pool op list` und `sql elastic-pool op cancel` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2201">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="b33c5-2202">Storage</span><span class="sxs-lookup"><span data-stu-id="b33c5-2202">Storage</span></span>

* <span data-ttu-id="b33c5-2203">Fehlermeldungen für falsch formatierte Verbindungszeichenfolgen verbessert</span><span class="sxs-lookup"><span data-stu-id="b33c5-2203">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="b33c5-2204">VM</span><span class="sxs-lookup"><span data-stu-id="b33c5-2204">VM</span></span>

* <span data-ttu-id="b33c5-2205">Unterstützung für die Konfiguration der Plattform-Fehlerdomänenanzahl für `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2205">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="b33c5-2206">`vmss create` geändert, damit standardmäßig „Standard LB“ für zonales, großes oder per einzelner Platzierungsgruppe deaktiviertes Scale Set festgelegt wird</span><span class="sxs-lookup"><span data-stu-id="b33c5-2206">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret`
* <span data-ttu-id="b33c5-2208">Unterstützung für SKU mit öffentlicher IP für `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2208">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="b33c5-2209">Argumente `--keyvault` und `--resource-group` für `vm secret format` hinzugefügt, um Szenarien zu unterstützen, bei denen der Befehl die Tresor-ID nicht auflösen kann.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2209">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="b33c5-2210">#5718</span><span class="sxs-lookup"><span data-stu-id="b33c5-2210">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="b33c5-2211">Bessere Fehler für `[vm|vmss create]`, wenn der Standort einer Ressourcengruppe keine Zonenunterstützung aufweist</span><span class="sxs-lookup"><span data-stu-id="b33c5-2211">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="b33c5-2212">27. März 2018</span><span class="sxs-lookup"><span data-stu-id="b33c5-2212">March 27, 2018</span></span>

<span data-ttu-id="b33c5-2213">Version 2.0.30</span><span class="sxs-lookup"><span data-stu-id="b33c5-2213">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="b33c5-2214">Core</span><span class="sxs-lookup"><span data-stu-id="b33c5-2214">Core</span></span>

* <span data-ttu-id="b33c5-2215">Anzeigen einer Meldung für Erweiterungen, die in der Hilfe als Vorschauversion gekennzeichnet sind</span><span class="sxs-lookup"><span data-stu-id="b33c5-2215">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="b33c5-2216">ACS</span><span class="sxs-lookup"><span data-stu-id="b33c5-2216">ACS</span></span>

* <span data-ttu-id="b33c5-2217">Behebung eines Fehlers bei der SSL-Zertifikatprüfung für `aks install-cli` in Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="b33c5-2217">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="b33c5-2218">AppService</span><span class="sxs-lookup"><span data-stu-id="b33c5-2218">Appservice</span></span>

* <span data-ttu-id="b33c5-2219">Unterstützung nur von HTTPS zu `webapp update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2219">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="b33c5-2220">Unterstützung für Slots zu `az webapp identity [assign|show]` und `az functionapp identity [assign|show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2220">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="b33c5-2221">Backup</span><span class="sxs-lookup"><span data-stu-id="b33c5-2221">Backup</span></span>

* <span data-ttu-id="b33c5-2222">Neuer Befehl `az backup protection isenabled-for-vm` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2222">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="b33c5-2223">Mit diesem Befehl kann überprüft werden, ob ein virtueller Computer von einem beliebigen Tresor im Abonnement gesichert wird.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2223">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="b33c5-2224">Azure-Objekt-IDs für Parameter `--resource-group` und `--vault-name` für die folgenden Befehle aktiviert:</span><span class="sxs-lookup"><span data-stu-id="b33c5-2224">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="b33c5-2225">`--name`-Parameter wurden geändert, um das Ausgabeformat von `backup ... show`-Befehlen zu akzeptieren.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2225">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="b33c5-2226">Container</span><span class="sxs-lookup"><span data-stu-id="b33c5-2226">Container</span></span>

* <span data-ttu-id="b33c5-2227">Befehl `container exec` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2227">Added `container exec` command.</span></span> <span data-ttu-id="b33c5-2228">Ausführung von Befehlen in einem Container für eine ausgeführte Containergruppe</span><span class="sxs-lookup"><span data-stu-id="b33c5-2228">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="b33c5-2229">Zulassen der Tabellenausgabe zum Erstellen und Aktualisieren einer Containergruppe</span><span class="sxs-lookup"><span data-stu-id="b33c5-2229">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="b33c5-2230">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="b33c5-2230">Extension</span></span>

* <span data-ttu-id="b33c5-2231">Meldung für `extension add` hinzugefügt, wenn sich die Erweiterung in der Vorschauphase befindet</span><span class="sxs-lookup"><span data-stu-id="b33c5-2231">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="b33c5-2232">`extension list-available` geändert, um vollständige Erweiterungsdaten mit `--show-details` anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="b33c5-2232">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="b33c5-2233">[BREAKING CHANGE]`extension list-available` geändert, um standardmäßig vereinfachte Erweiterungsdaten anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="b33c5-2233">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="b33c5-2234">Interactive</span><span class="sxs-lookup"><span data-stu-id="b33c5-2234">Interactive</span></span>

* <span data-ttu-id="b33c5-2235">Vervollständigungen wurden geändert und werden jetzt aktiviert, sobald das Laden der Befehlstabelle abgeschlossen ist.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2235">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="b33c5-2236">Fehler bei der Verwendung des Parameters `--style` behoben</span><span class="sxs-lookup"><span data-stu-id="b33c5-2236">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="b33c5-2237">Interaktiver Lexer nach Befehlstabellensicherung instanziiert (sofern nicht vorhanden)</span><span class="sxs-lookup"><span data-stu-id="b33c5-2237">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="b33c5-2238">Verbesserte Unterstützung der Vervollständigung</span><span class="sxs-lookup"><span data-stu-id="b33c5-2238">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="b33c5-2239">Labor</span><span class="sxs-lookup"><span data-stu-id="b33c5-2239">Lab</span></span>

* <span data-ttu-id="b33c5-2240">Probleme mit Befehl `create environment` behoben</span><span class="sxs-lookup"><span data-stu-id="b33c5-2240">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="b33c5-2241">Überwachen</span><span class="sxs-lookup"><span data-stu-id="b33c5-2241">Monitor</span></span>

* <span data-ttu-id="b33c5-2242">Unterstützung für `--top`, `--orderby` und `--namespace` zu `metrics list` hinzugefügt [Nr. 5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="b33c5-2242">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="b33c5-2243">[#4529](https://github.com/Azure/azure-cli/issues/5785) behoben: `metrics list` akzeptiert eine durch Leerzeichen getrennte Liste von abzurufenden Metriken</span><span class="sxs-lookup"><span data-stu-id="b33c5-2243">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="b33c5-2244">Unterstützung für `--namespace` zu `metrics list-definitions` hinzugefügt [Nr. 5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="b33c5-2244">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="b33c5-2245">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="b33c5-2245">Network</span></span>

* <span data-ttu-id="b33c5-2246">Unterstützung für private DNS-Zonen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2246">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="b33c5-2247">Profil</span><span class="sxs-lookup"><span data-stu-id="b33c5-2247">Profile</span></span>

* <span data-ttu-id="b33c5-2248">Warnung für `--identity-port` und `--msi-port` zu `login` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2248">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="b33c5-2249">RDBMS</span><span class="sxs-lookup"><span data-stu-id="b33c5-2249">RDBMS</span></span>

* <span data-ttu-id="b33c5-2250">GA-API-Version 2017-12-01 (Geschäftsmodell) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2250">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="b33c5-2251">Resource</span><span class="sxs-lookup"><span data-stu-id="b33c5-2251">Resource</span></span>

* [BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="b33c5-2253">Role</span><span class="sxs-lookup"><span data-stu-id="b33c5-2253">Role</span></span>

* <span data-ttu-id="b33c5-2254">Unterstützung für erforderliche Zugriffskonfigurationen und native Clients zu `az ad app create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2254">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="b33c5-2255">`rbac`-Befehle geändert, um maximal 1.000 IDs für Objektauflösung zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="b33c5-2255">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="b33c5-2256">Befehle zur Verwaltung von Anmeldeinformationen (`ad sp credential [reset|list|delete]`) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2256">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="b33c5-2257">[BREAKING CHANGE] „properties“ aus `az role assignment [list|show]`-Ausgabe entfernt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2257">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="b33c5-2258">Unterstützung für `dataActions`- und `notDataActions`-Berechtigungen zu `role definition` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2258">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="b33c5-2259">Storage</span><span class="sxs-lookup"><span data-stu-id="b33c5-2259">Storage</span></span>

* <span data-ttu-id="b33c5-2260">Problem beim Hochladen von Dateien mit einer Größe von 195 GB bis 200 GB behoben</span><span class="sxs-lookup"><span data-stu-id="b33c5-2260">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="b33c5-2261">[#4049](https://github.com/Azure/azure-cli/issues/4049) behoben: Probleme bei Uploads von Anfügeblobs behoben, die ein Ignorieren der Bedingungsparameter verursacht haben</span><span class="sxs-lookup"><span data-stu-id="b33c5-2261">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="b33c5-2262">VM</span><span class="sxs-lookup"><span data-stu-id="b33c5-2262">VM</span></span>

* <span data-ttu-id="b33c5-2263">Warnung für anstehende BREAKING CHANGEen für Sätze mit mehr als 100 Instanzen zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2263">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="b33c5-2264">Unterstützung der Zonenresilienz zu `vm [snapshot|image]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2264">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="b33c5-2265">Datenträgerinstanzansicht geändert, um besseren Verschlüsselungsstatus zu melden</span><span class="sxs-lookup"><span data-stu-id="b33c5-2265">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="b33c5-2266">[BREAKING CHANGE]`vm extension delete` geändert, um keine Ausgabe mehr zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="b33c5-2266">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="b33c5-2267">13. März 2018</span><span class="sxs-lookup"><span data-stu-id="b33c5-2267">March 13, 2018</span></span>

<span data-ttu-id="b33c5-2268">Version 2.0.29</span><span class="sxs-lookup"><span data-stu-id="b33c5-2268">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="b33c5-2269">ACR</span><span class="sxs-lookup"><span data-stu-id="b33c5-2269">ACR</span></span>

* <span data-ttu-id="b33c5-2270">Unterstützung für den Parameter `--image` zu `repository delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2270">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="b33c5-2271">Parameter `--manifest` und `--tag` des Befehls `repository delete` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-2271">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="b33c5-2272">Befehl `repository untag` zum Entfernen eines Tags ohne das Löschen von Daten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2272">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="b33c5-2273">ACS</span><span class="sxs-lookup"><span data-stu-id="b33c5-2273">ACS</span></span>

* <span data-ttu-id="b33c5-2274">Befehl `aks upgrade-connector` zum Aktualisieren eines vorhandenen Connectors hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2274">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="b33c5-2275">`kubectl`-Konfigurationsdateien zur Verwendung von besser lesbarem YAML im Blockstil geändert</span><span class="sxs-lookup"><span data-stu-id="b33c5-2275">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="b33c5-2276">Advisor</span><span class="sxs-lookup"><span data-stu-id="b33c5-2276">Advisor</span></span>

* <span data-ttu-id="b33c5-2277">[BREAKING CHANGE]`advisor configuration get` in `advisor configuration list` umbenannt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2277">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="b33c5-2278">[BREAKING CHANGE]`advisor configuration set` in `advisor configuration update` umbenannt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2278">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="b33c5-2279">[BREAKING CHANGE]`advisor recommendation generate` entfernt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2279">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="b33c5-2280">Parameter `--refresh` zu `advisor recommendation list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2280">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="b33c5-2281">Befehl `advisor recommendation show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2281">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="b33c5-2282">AppService</span><span class="sxs-lookup"><span data-stu-id="b33c5-2282">Appservice</span></span>

* <span data-ttu-id="b33c5-2283">`[webapp|functionapp] assign-identity` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-2283">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="b33c5-2284">Befehle `webapp identity [assign|show]` und `functionapp identity [assign|show]` für verwaltete Identität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2284">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="b33c5-2285">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="b33c5-2285">Eventhubs</span></span>

* <span data-ttu-id="b33c5-2286">Erste Veröffentlichung</span><span class="sxs-lookup"><span data-stu-id="b33c5-2286">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="b33c5-2287">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="b33c5-2287">Extension</span></span>

* <span data-ttu-id="b33c5-2288">Überprüfung zum Warnen von Benutzern hinzugefügt, wenn sich die verwendete Distribution von der in der Paketquelldatei gespeicherten Distribution unterscheidet, da dies Fehlern führen kann</span><span class="sxs-lookup"><span data-stu-id="b33c5-2288">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="b33c5-2289">Interactive</span><span class="sxs-lookup"><span data-stu-id="b33c5-2289">Interactive</span></span>

* <span data-ttu-id="b33c5-2290">[#5625](https://github.com/Azure/azure-cli/issues/5625) behoben: Verlauf über verschiedene Sitzungen hinweg beibehalten</span><span class="sxs-lookup"><span data-stu-id="b33c5-2290">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="b33c5-2291">[#3016](https://github.com/Azure/azure-cli/issues/3016) behoben: Verlauf nicht aufgezeichnet, obwohl er innerhalb des Bereichs liegt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2291">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="b33c5-2292">[#5688](https://github.com/Azure/azure-cli/issues/5688) behoben: Abschlüsse wurden nicht angezeigt, wenn beim Laden der Befehlstabelle eine Ausnahme aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="b33c5-2292">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="b33c5-2293">Statusanzeige für lang ausgeführte Vorgänge korrigiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-2293">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="b33c5-2294">Überwachen</span><span class="sxs-lookup"><span data-stu-id="b33c5-2294">Monitor</span></span>

* <span data-ttu-id="b33c5-2295">`monitor autoscale-settings`-Befehle als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-2295">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="b33c5-2296">Befehle vom Typ `monitor autoscale` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2296">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="b33c5-2297">Befehle vom Typ `monitor autoscale profile` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2297">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="b33c5-2298">Befehle vom Typ `monitor autoscale rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2298">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="b33c5-2299">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="b33c5-2299">Network</span></span>

* <span data-ttu-id="b33c5-2300">[BREAKING CHANGE] Parameter `--tags` aus `route-filter rule create` entfernt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2300">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="b33c5-2301">Einige fehlerhafte Standardwerte für die folgenden Befehle entfernt:</span><span class="sxs-lookup"><span data-stu-id="b33c5-2301">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="b33c5-2302">`network watcher connection-monitor`-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2302">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="b33c5-2303">Parameter `--vnet` und `--subnet` zu `network watcher show-topology` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2303">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="b33c5-2304">Profil</span><span class="sxs-lookup"><span data-stu-id="b33c5-2304">Profile</span></span>

* <span data-ttu-id="b33c5-2305">Parameter `--msi` für `az login` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-2305">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="b33c5-2306">Parameter `--identity` für `az login` als Ersatz vor `--msi` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2306">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="b33c5-2307">RDBMS</span><span class="sxs-lookup"><span data-stu-id="b33c5-2307">RDBMS</span></span>

* <span data-ttu-id="b33c5-2308">[VORSCHAU] Geändert, sodass die API „2017-12-01-preview“ verwendet wird</span><span class="sxs-lookup"><span data-stu-id="b33c5-2308">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="b33c5-2309">Service Bus</span><span class="sxs-lookup"><span data-stu-id="b33c5-2309">Service Bus</span></span>

* <span data-ttu-id="b33c5-2310">Erste Veröffentlichung</span><span class="sxs-lookup"><span data-stu-id="b33c5-2310">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="b33c5-2311">Storage</span><span class="sxs-lookup"><span data-stu-id="b33c5-2311">Storage</span></span>

* <span data-ttu-id="b33c5-2312">[#4971](https://github.com/Azure/azure-cli/issues/4971) behoben: `storage blob copy` unterstützt jetzt andere Azure-Clouds.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2312">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="b33c5-2313">[#5286](https://github.com/Azure/azure-cli/issues/5286) behoben: Batchbefehle `storage blob [delete-batch|download-batch|upload-batch]` lösen bei Vorbedingungsfehlern keinen Fehler mehr aus</span><span class="sxs-lookup"><span data-stu-id="b33c5-2313">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="b33c5-2314">VM</span><span class="sxs-lookup"><span data-stu-id="b33c5-2314">VM</span></span>

* <span data-ttu-id="b33c5-2315">`[vm|vmss] create` unterstützt jetzt das Anfügen nicht verwalteter Datenträger und das Konfigurieren der Zwischenspeicherung.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2315">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="b33c5-2316">`[vm|vmss] assign-identity` und `[vm|vmss] remove-identity` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-2316">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="b33c5-2317">Befehle `vm identity [assign|remove|show]` und `vmss identity [assign|remove|show]` als Ersatz für veraltete Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2317">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="b33c5-2318">Standardpriorität in `vmss create` auf „Keine“ geändert</span><span class="sxs-lookup"><span data-stu-id="b33c5-2318">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="b33c5-2319">27. Februar 2018</span><span class="sxs-lookup"><span data-stu-id="b33c5-2319">February 27, 2018</span></span>

<span data-ttu-id="b33c5-2320">Version 2.0.28</span><span class="sxs-lookup"><span data-stu-id="b33c5-2320">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="b33c5-2321">Core</span><span class="sxs-lookup"><span data-stu-id="b33c5-2321">Core</span></span>

* <span data-ttu-id="b33c5-2322">[#5184](https://github.com/Azure/azure-cli/issues/5184) behoben: Problem beim Installieren von Homebrew</span><span class="sxs-lookup"><span data-stu-id="b33c5-2322">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="b33c5-2323">Unterstützung für Erweiterungstelemetrie mit benutzerdefinierten Schlüsseln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2323">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="b33c5-2324">HTTP-Protokollierung zu `--debug` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2324">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="b33c5-2325">ACS</span><span class="sxs-lookup"><span data-stu-id="b33c5-2325">ACS</span></span>

* <span data-ttu-id="b33c5-2326">Geändert, sodass für `aks install-connector` standardmäßig das Helm-Diagramm `virtual-kubelet-for-aks` verwendet wird</span><span class="sxs-lookup"><span data-stu-id="b33c5-2326">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="b33c5-2327">Problem behoben: Unzureichende Berechtigungen für Dienstprinzipale zum Erstellen einer ACI-Containergruppe</span><span class="sxs-lookup"><span data-stu-id="b33c5-2327">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="b33c5-2328">Parameter `--aci-container-group`, `--location` und `--image-tag` zu `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2328">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="b33c5-2329">Veraltungshinweis aus `aks get-versions` entfernt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2329">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="b33c5-2330">AppService</span><span class="sxs-lookup"><span data-stu-id="b33c5-2330">Appservice</span></span>

* <span data-ttu-id="b33c5-2331">Updates für die neue SDK-Version (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="b33c5-2331">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="b33c5-2332">[5538](https://github.com/Azure/azure-cli/issues/5538) behoben: `Free` wurde als ungültige SKU gemeldet.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2332">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="b33c5-2333">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="b33c5-2333">Cognitive Services</span></span>

* <span data-ttu-id="b33c5-2334">Hinweis beim Erstellen eines neuen Cognitive Services-Kontos aktualisiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-2334">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="b33c5-2335">Nutzung</span><span class="sxs-lookup"><span data-stu-id="b33c5-2335">Consumption</span></span>

* <span data-ttu-id="b33c5-2336">Neue Befehle für PriceSheet-API hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2336">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="b33c5-2337">Vorhandene Formate für Nutzungsdetails und Reservierungsdetails aktualisiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-2337">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="b33c5-2338">Container</span><span class="sxs-lookup"><span data-stu-id="b33c5-2338">Container</span></span>

* <span data-ttu-id="b33c5-2339">Argumente `--secrets` und `--secrets-mount-path` zu `container create` hinzugefügt, um Geheimnisse in ACI verwenden zu können</span><span class="sxs-lookup"><span data-stu-id="b33c5-2339">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="b33c5-2340">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="b33c5-2340">Network</span></span>

* <span data-ttu-id="b33c5-2341">[#5559](https://github.com/Azure/azure-cli/issues/5559) behoben: Fehlender Client in `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="b33c5-2341">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="b33c5-2342">Resource</span><span class="sxs-lookup"><span data-stu-id="b33c5-2342">Resource</span></span>

* <span data-ttu-id="b33c5-2343">`group deployment export` geändert, um eine partielle Vorlage und ggf. Fehler anzuzeigen, wenn der Vorgang nicht erfolgreich war</span><span class="sxs-lookup"><span data-stu-id="b33c5-2343">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="b33c5-2344">Role</span><span class="sxs-lookup"><span data-stu-id="b33c5-2344">Role</span></span>

* <span data-ttu-id="b33c5-2345">`role assignment list-changelogs` hinzugefügt, um die Überprüfung von Dienstprinzipalrollen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="b33c5-2345">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="b33c5-2346">SQL</span><span class="sxs-lookup"><span data-stu-id="b33c5-2346">SQL</span></span>

* <span data-ttu-id="b33c5-2347">Zonenredundanzunterstützung für Datenbanken und Pools für elastische Datenbanken hinzugefügt (bei Erstellung und Aktualisierung)</span><span class="sxs-lookup"><span data-stu-id="b33c5-2347">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="b33c5-2348">Storage</span><span class="sxs-lookup"><span data-stu-id="b33c5-2348">Storage</span></span>

* <span data-ttu-id="b33c5-2349">Angabe von Zielpfad/Präfix für `storage blob [upload-batch|download-batch]` ermöglicht</span><span class="sxs-lookup"><span data-stu-id="b33c5-2349">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="b33c5-2350">VM</span><span class="sxs-lookup"><span data-stu-id="b33c5-2350">VM</span></span>

* <span data-ttu-id="b33c5-2351">Unterstützung für das Anfügen/Trennen von Datenträgern für eine einzelne VMSS-Instanz hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2351">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="b33c5-2352">13. Februar 2018</span><span class="sxs-lookup"><span data-stu-id="b33c5-2352">February 13, 2018</span></span>

<span data-ttu-id="b33c5-2353">Version 2.0.27</span><span class="sxs-lookup"><span data-stu-id="b33c5-2353">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="b33c5-2354">Core</span><span class="sxs-lookup"><span data-stu-id="b33c5-2354">Core</span></span>

* <span data-ttu-id="b33c5-2355">Authentifizierung für Abonnement-ID und Namen bei der MSI-Anmeldung in Authentifizierung mit Schlüssel geändert</span><span class="sxs-lookup"><span data-stu-id="b33c5-2355">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="b33c5-2356">ACS</span><span class="sxs-lookup"><span data-stu-id="b33c5-2356">ACS</span></span>

* <span data-ttu-id="b33c5-2357">[BREAKING CHANGE]`aks get-versions` aus Gründen der Genauigkeit in `aks get-upgrades` umbenannt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2357">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="b33c5-2358">`aks get-versions` zur Anzeige der verfügbaren Kubernetes-Versionen für `aks create` geändert</span><span class="sxs-lookup"><span data-stu-id="b33c5-2358">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="b33c5-2359">Standardwerte von `aks create` in Auswahl der Kubernetes-Version durch den Server geändert</span><span class="sxs-lookup"><span data-stu-id="b33c5-2359">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="b33c5-2360">Hilfemeldungen zu dem von AKS generierten Dienstprinzipal aktualisiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-2360">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="b33c5-2361">Standardknotengrößen für `aks create` von „Standard\_D1\_v2“ in „Standard\_DS1\_v2“ geändert</span><span class="sxs-lookup"><span data-stu-id="b33c5-2361">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="b33c5-2362">Zuverlässigkeit der Suche nach dem Dashboardpod für `az aks browse` verbessert</span><span class="sxs-lookup"><span data-stu-id="b33c5-2362">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="b33c5-2363">`aks get-credentials` korrigiert, um Unicode-Fehler beim Laden von Kubernetes-Konfigurationsdateien zu behandeln</span><span class="sxs-lookup"><span data-stu-id="b33c5-2363">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="b33c5-2364">Meldung zu `az aks install-cli` hinzugefügt, um das Abrufen von `kubectl` in `$PATH` zu erleichtern</span><span class="sxs-lookup"><span data-stu-id="b33c5-2364">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="b33c5-2365">AppService</span><span class="sxs-lookup"><span data-stu-id="b33c5-2365">Appservice</span></span>

* <span data-ttu-id="b33c5-2366">Problem behoben, das zu einem Fehler von `webapp [backup|restore]` aufgrund eines Nullverweises führte</span><span class="sxs-lookup"><span data-stu-id="b33c5-2366">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="b33c5-2367">Unterstützung für Standard-App Service-Pläne durch `az configure --defaults appserviceplan=my-asp` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2367">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="b33c5-2368">CDN</span><span class="sxs-lookup"><span data-stu-id="b33c5-2368">CDN</span></span>

* <span data-ttu-id="b33c5-2369">Befehle vom Typ `cdn custom-domain [enable-https|disable-https]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2369">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="b33c5-2370">Container</span><span class="sxs-lookup"><span data-stu-id="b33c5-2370">Container</span></span>

* <span data-ttu-id="b33c5-2371">Option `--follow` zu `az container logs` für Streamingprotokolle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2371">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="b33c5-2372">Befehl `container attach` hinzugefügt, der die lokale Standardausgabe und Fehlerdatenströme an einen Container in einer Containergruppe angefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2372">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="b33c5-2373">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="b33c5-2373">CosmosDB</span></span>

* <span data-ttu-id="b33c5-2374">Unterstützung für Einstellungsfunktionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2374">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="b33c5-2375">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="b33c5-2375">Extension</span></span>

* <span data-ttu-id="b33c5-2376">Unterstützung für den Parameter `--pip-proxy` zu Befehlen vom Typ `az extension [add|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2376">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="b33c5-2377">Unterstützung für das Argument `--pip-extra-index-urls` zu Befehlen vom Typ `az extension [add|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2377">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="b33c5-2378">Feedback</span><span class="sxs-lookup"><span data-stu-id="b33c5-2378">Feedback</span></span>

* <span data-ttu-id="b33c5-2379">Erweiterungsinformationen zu Telemetriedaten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2379">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="b33c5-2380">Interactive</span><span class="sxs-lookup"><span data-stu-id="b33c5-2380">Interactive</span></span>

* <span data-ttu-id="b33c5-2381">Problem behoben, aufgrund dessen der Benutzer bei Verwendung des interaktiven Modus in Cloud Shell zur Anmeldung aufgefordert wird</span><span class="sxs-lookup"><span data-stu-id="b33c5-2381">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="b33c5-2382">Regression mit fehlenden Parametervervollständigungen korrigiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-2382">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="b33c5-2383">IoT</span><span class="sxs-lookup"><span data-stu-id="b33c5-2383">IoT</span></span>

* <span data-ttu-id="b33c5-2384">Problem behoben, aufgrund dessen `iot dps access policy [create|update]` bei erfolgreicher Ausführung einen Fehler „nicht gefunden“ zurückgibt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2384">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="b33c5-2385">Problem behoben, aufgrund dessen `iot dps linked-hub [create|update]` bei erfolgreicher Ausführung einen Fehler „nicht gefunden“ zurückgibt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2385">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="b33c5-2386">Unterstützung für `--no-wait` zu `iot dps access policy [create|update]` und `iot dps linked-hub [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2386">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="b33c5-2387">`iot hub create` geändert, um die Angabe der Anzahl von Partitionen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="b33c5-2387">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="b33c5-2388">Überwachen</span><span class="sxs-lookup"><span data-stu-id="b33c5-2388">Monitor</span></span>

* <span data-ttu-id="b33c5-2389">Befehl `az monitor log-profiles create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-2389">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="b33c5-2390">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="b33c5-2390">Network</span></span>

* <span data-ttu-id="b33c5-2391">Option `--tags` für folgende Befehle korrigiert:</span><span class="sxs-lookup"><span data-stu-id="b33c5-2391">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="b33c5-2392">Profil</span><span class="sxs-lookup"><span data-stu-id="b33c5-2392">Profile</span></span>

* <span data-ttu-id="b33c5-2393">`az login` im interaktiven Modus aktiviert</span><span class="sxs-lookup"><span data-stu-id="b33c5-2393">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="b33c5-2394">Resource</span><span class="sxs-lookup"><span data-stu-id="b33c5-2394">Resource</span></span>

* <span data-ttu-id="b33c5-2395">`feature show` wieder hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2395">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="b33c5-2396">Role</span><span class="sxs-lookup"><span data-stu-id="b33c5-2396">Role</span></span>

* <span data-ttu-id="b33c5-2397">Argument `--available-to-other-tenants` zu `ad app update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2397">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="b33c5-2398">SQL</span><span class="sxs-lookup"><span data-stu-id="b33c5-2398">SQL</span></span>

* <span data-ttu-id="b33c5-2399">Befehle vom Typ `sql server dns-alias` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2399">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="b33c5-2400">`sql db rename` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2400">Added `sql db rename`</span></span>
* <span data-ttu-id="b33c5-2401">Unterstützung für das Argument `--ids` für alle SQL-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2401">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="b33c5-2402">Storage</span><span class="sxs-lookup"><span data-stu-id="b33c5-2402">Storage</span></span>

* <span data-ttu-id="b33c5-2403">Befehle `storage blob service-properties delete-policy` und `storage blob undelete` hinzugefügt, um vorläufiges Löschen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="b33c5-2403">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="b33c5-2404">VM</span><span class="sxs-lookup"><span data-stu-id="b33c5-2404">VM</span></span>

* <span data-ttu-id="b33c5-2405">Absturz bei unvollständiger Initialisierung der VM-Verschlüsselung behoben</span><span class="sxs-lookup"><span data-stu-id="b33c5-2405">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="b33c5-2406">Prinzipal-ID-Ausgabe beim Aktivieren von MSI hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2406">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="b33c5-2407">`vm boot-diagnostics get-boot-log` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="b33c5-2407">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="b33c5-2408">31. Januar 2018</span><span class="sxs-lookup"><span data-stu-id="b33c5-2408">January 31, 2018</span></span>

<span data-ttu-id="b33c5-2409">Version 2.0.26</span><span class="sxs-lookup"><span data-stu-id="b33c5-2409">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="b33c5-2410">Core</span><span class="sxs-lookup"><span data-stu-id="b33c5-2410">Core</span></span>

* <span data-ttu-id="b33c5-2411">Unterstützung für das Abrufen von unformatierten Token im MSI-Kontext hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2411">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="b33c5-2412">Abrufindikator-Zeichenfolge nach Fertigstellung von LRO für die Windows-Datei „cmd.exe“ entfernt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2412">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="b33c5-2413">Warnung hinzugefügt, die angezeigt wird, wenn ein konfigurierter Standardwert in einen Eintrag auf INFO-Ebene geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2413">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="b33c5-2414">`--verbose` zum Anzeigen verwenden.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2414">Use `--verbose` to see</span></span>
* <span data-ttu-id="b33c5-2415">Statusanzeige für Wait-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2415">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="b33c5-2416">ACS</span><span class="sxs-lookup"><span data-stu-id="b33c5-2416">ACS</span></span>

* <span data-ttu-id="b33c5-2417">Argument `--disable-browser` erläutert</span><span class="sxs-lookup"><span data-stu-id="b33c5-2417">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="b33c5-2418">Vervollständigung mit der TAB-TASTE für Argumente vom Typ `--vm-size` verbessert</span><span class="sxs-lookup"><span data-stu-id="b33c5-2418">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="b33c5-2419">AppService</span><span class="sxs-lookup"><span data-stu-id="b33c5-2419">Appservice</span></span>

* <span data-ttu-id="b33c5-2420">`webapp log [tail|download]` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="b33c5-2420">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="b33c5-2421">Überprüfung `kind` für Web-Apps und Funktionen entfernt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2421">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="b33c5-2422">CDN</span><span class="sxs-lookup"><span data-stu-id="b33c5-2422">CDN</span></span>

* <span data-ttu-id="b33c5-2423">Problem mit fehlendem Client für `cdn custom-domain create` behoben</span><span class="sxs-lookup"><span data-stu-id="b33c5-2423">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="b33c5-2424">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="b33c5-2424">CosmosDB</span></span>

* <span data-ttu-id="b33c5-2425">Parameterbeschreibung für Failoverrichtlinien korrigiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-2425">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="b33c5-2426">Interactive</span><span class="sxs-lookup"><span data-stu-id="b33c5-2426">Interactive</span></span>

* <span data-ttu-id="b33c5-2427">Problem behoben, aufgrund dessen Vervollständigungen von Befehlsoptionen nicht mehr angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="b33c5-2427">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="b33c5-2428">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="b33c5-2428">Network</span></span>

* <span data-ttu-id="b33c5-2429">Schutz für `--cert-password` zu `application-gateway create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2429">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="b33c5-2430">Problem mit `application-gateway update` behoben, aufgrund dessen `--sku` fälschlicherweise einen Standardwert anwendete</span><span class="sxs-lookup"><span data-stu-id="b33c5-2430">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="b33c5-2431">Schutz für `--shared-key` und `--authorization-key` zu `vpn-connection create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2431">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="b33c5-2432">Problem mit fehlendem Client für `asg create` behoben</span><span class="sxs-lookup"><span data-stu-id="b33c5-2432">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="b33c5-2433">Parameter `--file-name / -f` für exportierte Namen zu `dns zone export` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2433">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="b33c5-2434">Folgende Probleme mit `dns zone export` behoben:</span><span class="sxs-lookup"><span data-stu-id="b33c5-2434">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="b33c5-2435">Problem behoben, aufgrund dessen lange TXT-Einträge nicht korrekt exportiert wurden</span><span class="sxs-lookup"><span data-stu-id="b33c5-2435">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="b33c5-2436">Problem behoben, aufgrund dessen TXT-Einträge in Anführungszeichen fälschlich ohne Anführungszeichen in Escapezeichen exportiert wurden</span><span class="sxs-lookup"><span data-stu-id="b33c5-2436">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="b33c5-2437">Problem behoben, aufgrund dessen bestimmte Datensätze zweimal mit `dns zone import` importiert wurden</span><span class="sxs-lookup"><span data-stu-id="b33c5-2437">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="b33c5-2438">Befehle `vnet-gateway root-cert` und `vnet-gateway revoked-cert` wiederhergestellt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2438">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="b33c5-2439">Profil</span><span class="sxs-lookup"><span data-stu-id="b33c5-2439">Profile</span></span>

* <span data-ttu-id="b33c5-2440">`get-access-token` zur Verwendung auf einer VM mit Identität korrigiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-2440">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="b33c5-2441">Resource</span><span class="sxs-lookup"><span data-stu-id="b33c5-2441">Resource</span></span>

* <span data-ttu-id="b33c5-2442">Fehler mit `deployment [create|validate]` korrigiert, aufgrund dessen fälschlich eine Warnung angezeigt wurde, wenn ein Vorlagenfeld „Typ“ Werte in Großbuchstaben enthielt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2442">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="b33c5-2443">Storage</span><span class="sxs-lookup"><span data-stu-id="b33c5-2443">Storage</span></span>

* <span data-ttu-id="b33c5-2444">Problem mit der Migration von Storage V1-Konten zu Storage V2 behoben</span><span class="sxs-lookup"><span data-stu-id="b33c5-2444">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="b33c5-2445">Statusberichterstellung für alle Upload-/Downloadbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2445">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="b33c5-2446">Fehler korrigiert, der die Verwendung der arg-Option „-n“ mit `storage account check-name` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="b33c5-2446">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="b33c5-2447">Spalte „Momentaufnahme“ zur Tabellenausgabe für `blob [list|show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2447">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="b33c5-2448">Fehler mit verschiedenen Parametern korrigiert, die als Int-Typen analysiert werden mussten</span><span class="sxs-lookup"><span data-stu-id="b33c5-2448">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="b33c5-2449">VM</span><span class="sxs-lookup"><span data-stu-id="b33c5-2449">VM</span></span>

* <span data-ttu-id="b33c5-2450">Befehl `vm image accept-terms` hinzugefügt, um die Erstellung von VMs aus Images mit zusätzlichen Gebühren zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="b33c5-2450">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="b33c5-2451">`[vm|vmss create]` korrigiert, um sicherzustellen, dass Befehle unter einem Proxy mit nicht signierten Zertifikaten ausgeführt werden können</span><span class="sxs-lookup"><span data-stu-id="b33c5-2451">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="b33c5-2452">[VORSCHAU] Unterstützung für „niedrige“ Priorität zu VMSS hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2452">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="b33c5-2453">Schutz für `--admin-password` zu `[vm|vmss] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2453">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="b33c5-2454">17. Januar 2018</span><span class="sxs-lookup"><span data-stu-id="b33c5-2454">January 17, 2018</span></span>

<span data-ttu-id="b33c5-2455">Version 2.0.25</span><span class="sxs-lookup"><span data-stu-id="b33c5-2455">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="b33c5-2456">ACR</span><span class="sxs-lookup"><span data-stu-id="b33c5-2456">ACR</span></span>

* <span data-ttu-id="b33c5-2457">Fallback auf ACR-Anmeldung bei Fehlern mit Windows-Anmeldeinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2457">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="b33c5-2458">Registrierungsprotokolle aktiviert</span><span class="sxs-lookup"><span data-stu-id="b33c5-2458">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="b33c5-2459">ACS</span><span class="sxs-lookup"><span data-stu-id="b33c5-2459">ACS</span></span>

* <span data-ttu-id="b33c5-2460">Befehl `get-credentials` korrigiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-2460">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="b33c5-2461">SPN-Rollenanforderung entfernt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2461">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="b33c5-2462">AppService</span><span class="sxs-lookup"><span data-stu-id="b33c5-2462">Appservice</span></span>

* <span data-ttu-id="b33c5-2463">Fehler mit `config ssl upload` behoben, bei dem `hosting_environment_profile` NULL war</span><span class="sxs-lookup"><span data-stu-id="b33c5-2463">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="b33c5-2464">Unterstützung benutzerdefinierter URLs zu `browse` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2464">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="b33c5-2465">Slotunterstützung für `log tail` korrigiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-2465">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="b33c5-2466">Backup</span><span class="sxs-lookup"><span data-stu-id="b33c5-2466">Backup</span></span>

* <span data-ttu-id="b33c5-2467">Option `--container-name` von `backup item list` geändert (ist jetzt optional)</span><span class="sxs-lookup"><span data-stu-id="b33c5-2467">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="b33c5-2468">Speicherkontooptionen zu `backup restore restore-disks` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2468">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="b33c5-2469">Standortüberprüfung in `backup protection enable-for-vm` korrigiert (Groß-/Kleinschreibung wird jetzt nicht mehr beachtet)</span><span class="sxs-lookup"><span data-stu-id="b33c5-2469">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="b33c5-2470">Problem behoben, durch das bei Befehlen mit ungültigem Containernamen ein Fehler auftrat</span><span class="sxs-lookup"><span data-stu-id="b33c5-2470">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="b33c5-2471">`backup item list` geändert (Integritätsstatus jetzt standardmäßig enthalten)</span><span class="sxs-lookup"><span data-stu-id="b33c5-2471">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="b33c5-2472">Batch</span><span class="sxs-lookup"><span data-stu-id="b33c5-2472">Batch</span></span>

* <span data-ttu-id="b33c5-2473">`batch login` geändert, um Authentifizierungsdetails zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="b33c5-2473">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="b33c5-2474">Cloud</span><span class="sxs-lookup"><span data-stu-id="b33c5-2474">Cloud</span></span>

* <span data-ttu-id="b33c5-2475">Beim Festlegen von `--profile` für eine Cloud werden nun keine Endpunkte mehr benötigt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2475">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="b33c5-2476">Nutzung</span><span class="sxs-lookup"><span data-stu-id="b33c5-2476">Consumption</span></span>

* <span data-ttu-id="b33c5-2477">Neue Befehle für Reservierungen hinzugefügt: `consumption reservations summaries` und `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="b33c5-2477">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="b33c5-2478">Event Grid</span><span class="sxs-lookup"><span data-stu-id="b33c5-2478">Event Grid</span></span>

* <span data-ttu-id="b33c5-2479">[BREAKING CHANGE] Die Befehle vom Typ `az eventgrid topic event-subscription` wurden in `eventgrid event-subscription` verschoben.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2479">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="b33c5-2480">[BREAKING CHANGE] Die Befehle vom Typ `az eventgrid resource event-subscription` wurden in `eventgrid event-subscription` verschoben.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2480">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="b33c5-2481">[BREAKING CHANGE] Der Befehl `eventgrid event-subscription show-endpoint-url` wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2481">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="b33c5-2482">Verwenden Sie stattdessen `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2482">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="b33c5-2483">Befehl `eventgrid topic update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2483">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="b33c5-2484">Befehl `eventgrid event-subscription update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2484">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="b33c5-2485">Parameter `--ids` für Befehle vom Typ `eventgrid topic` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2485">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="b33c5-2486">Unterstützung der Vervollständigung mit der TAB-TASTE für Themennamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2486">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="b33c5-2487">Interactive</span><span class="sxs-lookup"><span data-stu-id="b33c5-2487">Interactive</span></span>

* <span data-ttu-id="b33c5-2488">Problem behoben, das dazu führte, dass der interaktive Modus nicht mit Python 2.x verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="b33c5-2488">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="b33c5-2489">Fehler beim Start behoben</span><span class="sxs-lookup"><span data-stu-id="b33c5-2489">Fixed errors on startup</span></span>
* <span data-ttu-id="b33c5-2490">Problem behoben, das dazu führte, dass einige Befehle nicht im interaktiven Modus ausgeführt werden konnten</span><span class="sxs-lookup"><span data-stu-id="b33c5-2490">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="b33c5-2491">IoT</span><span class="sxs-lookup"><span data-stu-id="b33c5-2491">IoT</span></span>

* <span data-ttu-id="b33c5-2492">Unterstützung für Gerätebereitstellungsdienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2492">Added support for device provisioning service</span></span>
* <span data-ttu-id="b33c5-2493">Benachrichtigungen zu veralteten Elementen in Befehlen und in der Befehlshilfe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2493">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="b33c5-2494">IoT-Überprüfung hinzugefügt, um Benutzer über die IoT-Erweiterung zu informieren</span><span class="sxs-lookup"><span data-stu-id="b33c5-2494">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="b33c5-2495">Überwachen</span><span class="sxs-lookup"><span data-stu-id="b33c5-2495">Monitor</span></span>

* <span data-ttu-id="b33c5-2496">Unterstützung mehrerer Diagnoseeinstellung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2496">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="b33c5-2497">Der Parameter `--name` ist nun für `az monitor diagnostic-settings create` erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2497">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="b33c5-2498">Befehl `monitor diagnostic-settings categories` zum Abrufen der Diagnoseeinstellungskategorie hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2498">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="b33c5-2499">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="b33c5-2499">Network</span></span>

* <span data-ttu-id="b33c5-2500">Problem behoben, das beim Ändern des aktiven Standbymodus mit `vnet-gateway update` auftrat</span><span class="sxs-lookup"><span data-stu-id="b33c5-2500">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="b33c5-2501">Unterstützung für HTTP2 zu `application-gateway [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2501">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="b33c5-2502">Profil</span><span class="sxs-lookup"><span data-stu-id="b33c5-2502">Profile</span></span>

* <span data-ttu-id="b33c5-2503">Unterstützung für die Anmeldung mit durch Benutzer zugewiesenen Identitäten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2503">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="b33c5-2504">Role</span><span class="sxs-lookup"><span data-stu-id="b33c5-2504">Role</span></span>

* <span data-ttu-id="b33c5-2505">Argument `--assignee-object-id` zu `role assignment create` hinzugefügt, um Graph-Abfrage zu umgehen</span><span class="sxs-lookup"><span data-stu-id="b33c5-2505">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="b33c5-2506">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="b33c5-2506">Service Fabric</span></span>

* <span data-ttu-id="b33c5-2507">Ausführliche Fehler zur Überprüfungsantwort bei der Clustererstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2507">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="b33c5-2508">Problem mit fehlendem Client für verschiedene Befehle behoben</span><span class="sxs-lookup"><span data-stu-id="b33c5-2508">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="b33c5-2509">VM</span><span class="sxs-lookup"><span data-stu-id="b33c5-2509">VM</span></span>

* <span data-ttu-id="b33c5-2510">[VORSCHAUVERSION] Zonenübergreifende Unterstützung für `vmss`</span><span class="sxs-lookup"><span data-stu-id="b33c5-2510">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="b33c5-2511">[BREAKING CHANGE] Standard für Einzelzone (`vmss`) in Standardlastenausgleich geändert</span><span class="sxs-lookup"><span data-stu-id="b33c5-2511">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="b33c5-2512">[BREAKING CHANGE]`externalIdentities` in `userAssignedIdentities` geändert für EMSI</span><span class="sxs-lookup"><span data-stu-id="b33c5-2512">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="b33c5-2513">[VORSCHAUVERSION] Unterstützung für Austausch des Betriebssystemdatenträgers hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2513">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="b33c5-2514">Unterstützung der Verwendung von VM-Images aus anderen Abonnements hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2514">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="b33c5-2515">Argumente `--plan-name`, `--plan-product`, `--plan-promotion-code` und `--plan-publisher` zu `[vm|vmss] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2515">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="b33c5-2516">Fehlerbedingte Probleme mit `[vm|vmss] create` behoben</span><span class="sxs-lookup"><span data-stu-id="b33c5-2516">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="b33c5-2517">Übermäßige Ressourcenverwendung durch `vm image list --all` behoben</span><span class="sxs-lookup"><span data-stu-id="b33c5-2517">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="b33c5-2518">19. Dezember 2017</span><span class="sxs-lookup"><span data-stu-id="b33c5-2518">December 19, 2017</span></span>

<span data-ttu-id="b33c5-2519">Version 2.0.23</span><span class="sxs-lookup"><span data-stu-id="b33c5-2519">Version 2.0.23</span></span>

* <span data-ttu-id="b33c5-2520">Unterstützung für die Anmeldung mit durch Benutzer zugewiesenen Identitäten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2520">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="b33c5-2521">Container</span><span class="sxs-lookup"><span data-stu-id="b33c5-2521">Container</span></span>

* <span data-ttu-id="b33c5-2522">Falsche Reihenfolge der Parameter für Containerprotokolle behoben</span><span class="sxs-lookup"><span data-stu-id="b33c5-2522">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="b33c5-2523">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="b33c5-2523">Network</span></span>

* <span data-ttu-id="b33c5-2524">Argument `--disable-bgp-route-propagation` zu `route-table [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2524">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="b33c5-2525">Argument `--ip-tags` zu `public-ip [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2525">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="b33c5-2526">Storage</span><span class="sxs-lookup"><span data-stu-id="b33c5-2526">Storage</span></span>

* <span data-ttu-id="b33c5-2527">Unterstützung für Storage V2 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2527">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="b33c5-2528">VM</span><span class="sxs-lookup"><span data-stu-id="b33c5-2528">VM</span></span>

* <span data-ttu-id="b33c5-2529">[VORSCHAUVERSION] Unterstützung für durch Benutzer zugewiesene Identitäten für virtuelle Computer und VMSSs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2529">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="b33c5-2530">5\. Dezember 2017</span><span class="sxs-lookup"><span data-stu-id="b33c5-2530">December 5, 2017</span></span>

<span data-ttu-id="b33c5-2531">Version 2.0.22</span><span class="sxs-lookup"><span data-stu-id="b33c5-2531">Version 2.0.22</span></span>

* <span data-ttu-id="b33c5-2532">`az component`-Befehle wurden entfernt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2532">Removed `az component` commands.</span></span> <span data-ttu-id="b33c5-2533">Verwenden Sie stattdessen `az extension`.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2533">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="b33c5-2534">Core</span><span class="sxs-lookup"><span data-stu-id="b33c5-2534">Core</span></span>
* <span data-ttu-id="b33c5-2535">Der `AZURE_US_GOV_CLOUD`-Autoritätsendpunkt von AAD wurde von „login.microsoftonline.com“ in „login.microsoftonline.us“ geändert.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2535">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="b33c5-2536">Problem behoben, aufgrund dessen Telemetriedaten fortlaufend neu gesendet wurden</span><span class="sxs-lookup"><span data-stu-id="b33c5-2536">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="b33c5-2537">ACS</span><span class="sxs-lookup"><span data-stu-id="b33c5-2537">ACS</span></span>

* <span data-ttu-id="b33c5-2538">Die Befehle `aks install-connector` und `aks remove-connector` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2538">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="b33c5-2539">Verbesserte Fehlerberichterstellung für `acs create`</span><span class="sxs-lookup"><span data-stu-id="b33c5-2539">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="b33c5-2540">Feste Verwendung von `aks get-credentials -f` ohne vollqualifizierten Pfad</span><span class="sxs-lookup"><span data-stu-id="b33c5-2540">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="b33c5-2541">Advisor</span><span class="sxs-lookup"><span data-stu-id="b33c5-2541">Advisor</span></span>

* <span data-ttu-id="b33c5-2542">Erste Veröffentlichung</span><span class="sxs-lookup"><span data-stu-id="b33c5-2542">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="b33c5-2543">AppService</span><span class="sxs-lookup"><span data-stu-id="b33c5-2543">Appservice</span></span>

* <span data-ttu-id="b33c5-2544">Erstellung feststehender Zertifikatnamen mit `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="b33c5-2544">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="b33c5-2545">`webapp [list|show]` und `functionapp [list|show]` wurden verbessert, um die richtigen Apps anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="b33c5-2545">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="b33c5-2546">Standardwert für `WEBSITE_NODE_DEFAULT_VERSION` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2546">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="b33c5-2547">Nutzung</span><span class="sxs-lookup"><span data-stu-id="b33c5-2547">Consumption</span></span>

* <span data-ttu-id="b33c5-2548">Unterstützung für API-Version 2017-11-30 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2548">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="b33c5-2549">Container</span><span class="sxs-lookup"><span data-stu-id="b33c5-2549">Container</span></span>

* <span data-ttu-id="b33c5-2550">Feste Regression für Standardports</span><span class="sxs-lookup"><span data-stu-id="b33c5-2550">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="b33c5-2551">Überwachen</span><span class="sxs-lookup"><span data-stu-id="b33c5-2551">Monitor</span></span>

* <span data-ttu-id="b33c5-2552">Unterstützung mehrerer Dimensionen zu Metrikbefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2552">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="b33c5-2553">Resource</span><span class="sxs-lookup"><span data-stu-id="b33c5-2553">Resource</span></span>

* <span data-ttu-id="b33c5-2554">Argument `--include-response-body` zu `resource show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2554">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="b33c5-2555">Role</span><span class="sxs-lookup"><span data-stu-id="b33c5-2555">Role</span></span>

* <span data-ttu-id="b33c5-2556">Anzeige von Standardzuweisungen für „klassische“ Administratoren zu `role assignment list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2556">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="b33c5-2557">Unterstützung für das Hinzufügen (anstelle der Überschreibung) von Anmeldeinformationen zu `ad sp reset-credentials` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2557">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="b33c5-2558">Verbesserte Fehlerberichterstellung für `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="b33c5-2558">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="b33c5-2559">SQL</span><span class="sxs-lookup"><span data-stu-id="b33c5-2559">SQL</span></span>

* <span data-ttu-id="b33c5-2560">Die Befehle `sql db list-usages` und `sql db show-usage` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2560">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="b33c5-2561">Die Befehle `sql server conn-policy show` und `sql server conn-policy update` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2561">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="b33c5-2562">VM</span><span class="sxs-lookup"><span data-stu-id="b33c5-2562">VM</span></span>

* <span data-ttu-id="b33c5-2563">Zoneninformationen zu `az vm list-skus` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2563">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="b33c5-2564">14. November 2017</span><span class="sxs-lookup"><span data-stu-id="b33c5-2564">November 14, 2017</span></span>

<span data-ttu-id="b33c5-2565">Version 2.0.21</span><span class="sxs-lookup"><span data-stu-id="b33c5-2565">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="b33c5-2566">ACR</span><span class="sxs-lookup"><span data-stu-id="b33c5-2566">ACR</span></span>

* <span data-ttu-id="b33c5-2567">Unterstützung für das Erstellen von Webhooks in Replikationsregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2567">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="b33c5-2568">ACS</span><span class="sxs-lookup"><span data-stu-id="b33c5-2568">ACS</span></span>

* <span data-ttu-id="b33c5-2569">Formulierung in AKS von „Agent“ in „Knoten“ geändert</span><span class="sxs-lookup"><span data-stu-id="b33c5-2569">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="b33c5-2570">Option `--orchestrator-release` für `acs create` als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="b33c5-2570">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="b33c5-2571">VM-Standardgröße für AKS in `Standard_D1_v2` geändert</span><span class="sxs-lookup"><span data-stu-id="b33c5-2571">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="b33c5-2572">`az aks browse` für Windows korrigiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-2572">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="b33c5-2573">`az aks get-credentials` für Windows korrigiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-2573">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="b33c5-2574">AppService</span><span class="sxs-lookup"><span data-stu-id="b33c5-2574">Appservice</span></span>

* <span data-ttu-id="b33c5-2575">Bereitstellungsquelle `config-zip` für Web-Apps und Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2575">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="b33c5-2576">Option `--docker-container-logging` zu `az webapp log config` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2576">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="b33c5-2577">Option `storage` aus dem Parameter `--web-server-logging` von `az webapp log config` entfernt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2577">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="b33c5-2578">Fehlermeldungen für `deployment user set` verbessert</span><span class="sxs-lookup"><span data-stu-id="b33c5-2578">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="b33c5-2579">Unterstützung für das Erstellen von Linux-Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2579">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="b33c5-2580">`list-locations` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="b33c5-2580">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="b33c5-2581">Batch</span><span class="sxs-lookup"><span data-stu-id="b33c5-2581">Batch</span></span>

* <span data-ttu-id="b33c5-2582">Fehler im Poolerstellungsbefehl korrigiert, der bei Verwendung einer Ressourcen-ID mit dem Flag `--image` aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="b33c5-2582">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="b33c5-2583">BatchAI</span><span class="sxs-lookup"><span data-stu-id="b33c5-2583">Batchai</span></span>

* <span data-ttu-id="b33c5-2584">Kurzoption (`-s`) für `--vm-size` zur Angabe der VM-Größe im Befehl `file-server create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2584">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="b33c5-2585">Argumente für Speicherkontoname und -schlüssel zum Parameter `cluster create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2585">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="b33c5-2586">Dokumentation für `job list-files` und `job stream-file` korrigiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-2586">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="b33c5-2587">Kurzoption (`-r`) für `--cluster-name` zur Angabe des Clusternamens im Befehl `job create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2587">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="b33c5-2588">Cloud</span><span class="sxs-lookup"><span data-stu-id="b33c5-2588">Cloud</span></span>

* <span data-ttu-id="b33c5-2589">`cloud [register|update]` geändert, um die Registrierung von Clouds ohne erforderliche Endpunkte zu verhindern</span><span class="sxs-lookup"><span data-stu-id="b33c5-2589">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="b33c5-2590">Container</span><span class="sxs-lookup"><span data-stu-id="b33c5-2590">Container</span></span>

* <span data-ttu-id="b33c5-2591">Unterstützung für das Öffnen mehrerer Ports hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2591">Added support to open multiple ports</span></span>
* <span data-ttu-id="b33c5-2592">Neustartrichtlinie für Containergruppen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2592">Added container group restart policy</span></span>
* <span data-ttu-id="b33c5-2593">Unterstützung zum Einbinden einer Azure-Dateifreigabe als Volume hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2593">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="b33c5-2594">Hilfedokumente aktualisiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-2594">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="b33c5-2595">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="b33c5-2595">Data Lake Analytics</span></span>

* <span data-ttu-id="b33c5-2596">`[job|account] list` geändert, um präzisere Informationen zu erhalten</span><span class="sxs-lookup"><span data-stu-id="b33c5-2596">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="b33c5-2597">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="b33c5-2597">Data Lake Store</span></span>

* <span data-ttu-id="b33c5-2598">`account list` geändert, um präzisere Informationen zu erhalten</span><span class="sxs-lookup"><span data-stu-id="b33c5-2598">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="b33c5-2599">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="b33c5-2599">Extension</span></span>

* <span data-ttu-id="b33c5-2600">`extension list-available` hinzugefügt, um das Auflisten offizieller Microsoft-Erweiterungen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="b33c5-2600">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="b33c5-2601">`--name` zu `extension [add|update]` hinzugefügt, um das Installieren von Erweiterungen nach Name zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="b33c5-2601">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="b33c5-2602">IoT</span><span class="sxs-lookup"><span data-stu-id="b33c5-2602">IoT</span></span>

* <span data-ttu-id="b33c5-2603">Unterstützung für Zertifizierungsstellen (CAs) und Zertifikatketten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2603">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="b33c5-2604">Überwachen</span><span class="sxs-lookup"><span data-stu-id="b33c5-2604">Monitor</span></span>

* <span data-ttu-id="b33c5-2605">Befehle vom Typ `activity-log alert` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2605">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="b33c5-2606">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="b33c5-2606">Network</span></span>

* <span data-ttu-id="b33c5-2607">Unterstützung für CAA-DNS-Einträge hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2607">Added support for CAA DNS records</span></span>
* <span data-ttu-id="b33c5-2608">Problem behoben, durch das Endpunkte nicht mit `traffic-manager profile update` aktualisiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="b33c5-2608">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="b33c5-2609">Problem behoben, durch das `vnet update --dns-servers` je nach VNet-Erstellungsmethode nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="b33c5-2609">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="b33c5-2610">Problem behoben, durch das relative DNS-Namen durch `dns zone import` nicht korrekt importiert wurden</span><span class="sxs-lookup"><span data-stu-id="b33c5-2610">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="b33c5-2611">Reservations</span><span class="sxs-lookup"><span data-stu-id="b33c5-2611">Reservations</span></span>

* <span data-ttu-id="b33c5-2612">Erste Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="b33c5-2612">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="b33c5-2613">Resource</span><span class="sxs-lookup"><span data-stu-id="b33c5-2613">Resource</span></span>

* <span data-ttu-id="b33c5-2614">Unterstützung für Ressourcen-IDs zum Parameter `--resource` und Sperren auf Ressourcenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2614">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="b33c5-2615">SQL</span><span class="sxs-lookup"><span data-stu-id="b33c5-2615">SQL</span></span>

* <span data-ttu-id="b33c5-2616">Parameter `--ignore-missing-vnet-service-endpoint` zu `sql server vnet-rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2616">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="b33c5-2617">Storage</span><span class="sxs-lookup"><span data-stu-id="b33c5-2617">Storage</span></span>

* <span data-ttu-id="b33c5-2618">`storage account create` geändert, sodass die SKU `Standard_RAGRS` als Standard verwendet wird</span><span class="sxs-lookup"><span data-stu-id="b33c5-2618">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="b33c5-2619">Fehler im Zusammenhang mit Datei-/Blobnamen korrigiert, die ASCII-fremde Zeichen enthalten</span><span class="sxs-lookup"><span data-stu-id="b33c5-2619">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="b33c5-2620">Fehler korrigiert, der die Verwendung von `--source-uri` mit `storage [blob|file] copy start-batch` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="b33c5-2620">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="b33c5-2621">Befehle zum Globalisieren und Löschen mehrerer Objekte mit `storage [blob|file] delete-batch` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2621">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="b33c5-2622">Problem beim Aktivieren von Metriken mit `storage metrics update` behoben</span><span class="sxs-lookup"><span data-stu-id="b33c5-2622">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="b33c5-2623">Problem mit Dateien über 200 GB bei Verwendung von `storage blob upload-batch` behoben</span><span class="sxs-lookup"><span data-stu-id="b33c5-2623">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="b33c5-2624">Problem behoben, durch das `--bypass` und `--default-action` von `storage account [create|update]` ignoriert wurden</span><span class="sxs-lookup"><span data-stu-id="b33c5-2624">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="b33c5-2625">VM</span><span class="sxs-lookup"><span data-stu-id="b33c5-2625">VM</span></span>

* <span data-ttu-id="b33c5-2626">Fehler mit `vmss create` korrigiert, der die Verwendung der Größenebene `Basic` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="b33c5-2626">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="b33c5-2627">`--plan`-Argumente zu `[vm|vmss] create` für benutzerdefinierte Images mit Abrechnungsinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2627">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="b33c5-2628">Befehle hinzugefügt: `vm secret `[add|remove|list]</span><span class="sxs-lookup"><span data-stu-id="b33c5-2628">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="b33c5-2629">`vm format-secret` in `vm secret format` umbenannt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2629">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="b33c5-2630">Argument `--encrypt format` zu `vm encryption enable` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2630">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="b33c5-2631">24. Oktober 2017</span><span class="sxs-lookup"><span data-stu-id="b33c5-2631">October 24, 2017</span></span>

<span data-ttu-id="b33c5-2632">Version 2.0.20</span><span class="sxs-lookup"><span data-stu-id="b33c5-2632">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="b33c5-2633">Core</span><span class="sxs-lookup"><span data-stu-id="b33c5-2633">Core</span></span>

* <span data-ttu-id="b33c5-2634">Aktualisierung von `2017-03-09-profile` zur Verwendung von Version `2016-01-01` der `MGMT_STORAGE`-API</span><span class="sxs-lookup"><span data-stu-id="b33c5-2634">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="b33c5-2635">ACR</span><span class="sxs-lookup"><span data-stu-id="b33c5-2635">ACR</span></span>

* <span data-ttu-id="b33c5-2636">Die Ressourcenverwaltung wurde aktualisiert und verweist nun auf die API-Version `2017-10-01`.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2636">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="b33c5-2637">SKU „Bring Your Own Storage“ wurde in „Klassisch“ geändert.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2637">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="b33c5-2638">Die Registrierungs-SKUs wurden in „Basic“, „Standard“ und „Premium“ umbenannt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2638">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="b33c5-2639">ACS</span><span class="sxs-lookup"><span data-stu-id="b33c5-2639">ACS</span></span>

* <span data-ttu-id="b33c5-2640">[VORSCHAUVERSION] Befehle vom Typ `az aks` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2640">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="b33c5-2641">Problem mit `get-credentials` in Kubernetes behoben</span><span class="sxs-lookup"><span data-stu-id="b33c5-2641">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="b33c5-2642">AppService</span><span class="sxs-lookup"><span data-stu-id="b33c5-2642">Appservice</span></span>

* <span data-ttu-id="b33c5-2643">Problem behoben, aufgrund dessen heruntergeladene `webapp`-Protokolle unter Umständen ungültig waren</span><span class="sxs-lookup"><span data-stu-id="b33c5-2643">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="b33c5-2644">Komponente</span><span class="sxs-lookup"><span data-stu-id="b33c5-2644">Component</span></span>

* <span data-ttu-id="b33c5-2645">Deutlichere Meldung zur Einstellung für alle Installer und für Bestätigungsaufforderung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2645">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="b33c5-2646">Überwachen</span><span class="sxs-lookup"><span data-stu-id="b33c5-2646">Monitor</span></span>

* <span data-ttu-id="b33c5-2647">Befehle vom Typ `action-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2647">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="b33c5-2648">Resource</span><span class="sxs-lookup"><span data-stu-id="b33c5-2648">Resource</span></span>

* <span data-ttu-id="b33c5-2649">Inkompatibilität mit der aktuellen Version der msrest-Abhängigkeit in `group export` behoben</span><span class="sxs-lookup"><span data-stu-id="b33c5-2649">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="b33c5-2650">Problem mit `policy assignment create` behoben, sodass der Befehl mit integrierten Richtliniendefinitionen und Richtliniensatzdefinitionen verwendet werden kann</span><span class="sxs-lookup"><span data-stu-id="b33c5-2650">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="b33c5-2651">VM</span><span class="sxs-lookup"><span data-stu-id="b33c5-2651">VM</span></span>

* <span data-ttu-id="b33c5-2652">Argument `--accelerated-networking` zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2652">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="b33c5-2653">9\. Oktober 2017</span><span class="sxs-lookup"><span data-stu-id="b33c5-2653">October 9, 2017</span></span>

<span data-ttu-id="b33c5-2654">Version 2.0.19</span><span class="sxs-lookup"><span data-stu-id="b33c5-2654">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="b33c5-2655">Core</span><span class="sxs-lookup"><span data-stu-id="b33c5-2655">Core</span></span>

* <span data-ttu-id="b33c5-2656">Verarbeitung von ADFS-Autoritäts-URLs wurde mit einem nachgestellten Schrägstrich zu Azure Stack hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2656">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="b33c5-2657">AppService</span><span class="sxs-lookup"><span data-stu-id="b33c5-2657">Appservice</span></span>

* <span data-ttu-id="b33c5-2658">Mit dem neuen Befehl `webapp update` wurde ein allgemeines Update hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2658">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="b33c5-2659">Batch</span><span class="sxs-lookup"><span data-stu-id="b33c5-2659">Batch</span></span>

* <span data-ttu-id="b33c5-2660">Aktualisierung auf Batch SDK 4.0.0</span><span class="sxs-lookup"><span data-stu-id="b33c5-2660">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="b33c5-2661">Die Option `--image` von „VirtualMachineConfiguration“ wurde aktualisiert, um zusätzlich zu „publish:offer:sku:version“ ARM-Imageverweise zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2661">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="b33c5-2662">Unterstützung für das neue CLI-Erweiterungsmodell für Batch-Erweiterungsbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2662">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="b33c5-2663">Batch-Unterstützung aus dem Komponentenmodell entfernt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2663">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="b33c5-2664">BatchAI</span><span class="sxs-lookup"><span data-stu-id="b33c5-2664">Batchai</span></span>

* <span data-ttu-id="b33c5-2665">Erste Version des Batch KI-Moduls</span><span class="sxs-lookup"><span data-stu-id="b33c5-2665">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="b33c5-2666">KeyVault</span><span class="sxs-lookup"><span data-stu-id="b33c5-2666">Keyvault</span></span>

* <span data-ttu-id="b33c5-2667">Key Vault-Authentifizierungsproblem behoben, das bei Verwendung von ADFS in Azure Stack auftrat.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2667">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="b33c5-2668">(#4448)</span><span class="sxs-lookup"><span data-stu-id="b33c5-2668">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="b33c5-2669">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="b33c5-2669">Network</span></span>

* <span data-ttu-id="b33c5-2670">Das Argument `--server` von `application-gateway address-pool create` ist nun optional, sodass leere Adresspools zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2670">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="b33c5-2671">`traffic-manager` wurde aktualisiert, um aktuelle Features zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2671">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="b33c5-2672">Resource</span><span class="sxs-lookup"><span data-stu-id="b33c5-2672">Resource</span></span>

* <span data-ttu-id="b33c5-2673">Zusätzliche Unterstützung für `--resource-group/-g`-Optionen für Ressourcengruppennamen zu `group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2673">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="b33c5-2674">Befehle für `account lock` hinzugefügt, um die Verwendung mit Sperren auf Abonnementebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2674">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="b33c5-2675">Befehle für `group lock` hinzugefügt, um die Verwendung mit Sperren auf Gruppenebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2675">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="b33c5-2676">Befehle für `resource lock` hinzugefügt, um die Verwendung mit Sperren auf Ressourcenebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2676">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="b33c5-2677">Sql</span><span class="sxs-lookup"><span data-stu-id="b33c5-2677">Sql</span></span>

* <span data-ttu-id="b33c5-2678">Unterstützung für SQL Transparent Data Encryption (TDE) und TDE für Bring Your Own Key-Szenarien hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2678">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="b33c5-2679">Der Befehl `db list-deleted` und der Parameter `db restore --deleted-time` wurden hinzugefügt, um die Ermittlung und Wiederherstellung gelöschter Datenbanken zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2679">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="b33c5-2680">`db op list` und `db op cancel` wurden hinzugefügt, um das Auflisten und Abbrechen ausgeführter Vorgänge für eine Datenbank zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2680">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="b33c5-2681">Storage</span><span class="sxs-lookup"><span data-stu-id="b33c5-2681">Storage</span></span>

* <span data-ttu-id="b33c5-2682">Unterstützung für Momentaufnahme von Dateifreigaben hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2682">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="b33c5-2683">VM</span><span class="sxs-lookup"><span data-stu-id="b33c5-2683">Vm</span></span>

* <span data-ttu-id="b33c5-2684">Korrektur eines Fehlers in `vm show`, bei dem die Verwendung von `-d` in Verbindung mit fehlenden privaten IP-Adressen einen Absturz verursachte</span><span class="sxs-lookup"><span data-stu-id="b33c5-2684">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="b33c5-2685">[VORSCHAUVERSION] Unterstützung für paralleles Upgrade zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2685">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="b33c5-2686">Unterstützung für das Aktualisieren der Verschlüsselungseinstellungen mit `vm encryption enable` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2686">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="b33c5-2687">Parameter `--os-disk-size-gb` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2687">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="b33c5-2688">Parameter `--license-type` für Windows zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2688">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="b33c5-2689">22. September 2017</span><span class="sxs-lookup"><span data-stu-id="b33c5-2689">September 22, 2017</span></span>

<span data-ttu-id="b33c5-2690">Version 2.0.18</span><span class="sxs-lookup"><span data-stu-id="b33c5-2690">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="b33c5-2691">Resource</span><span class="sxs-lookup"><span data-stu-id="b33c5-2691">Resource</span></span>

* <span data-ttu-id="b33c5-2692">Unterstützung für das Anzeigen integrierter Richtliniendefinitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2692">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="b33c5-2693">Unterstützungsmodusparameter zum Erstellen von Richtliniendefinitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2693">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="b33c5-2694">Unterstützung für UI-Definitionen und -Vorlagen zu `managedapp definition create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2694">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="b33c5-2695">[BREAKING CHANGE] Der Ressourcentyp `managedapp` wurde von `appliances` in `applications` und von `applianceDefinitions` in `applicationDefinitions` geändert.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2695">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="b33c5-2696">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="b33c5-2696">Network</span></span>

* <span data-ttu-id="b33c5-2697">Unterstützung für Verfügbarkeitszone zu Unterbefehlen `network lb` und `network public-ip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2697">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="b33c5-2698">Unterstützung für IPv6-Microsoft-Peering zu `express-route` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2698">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="b33c5-2699">Befehle für Anwendungssicherheitsgruppe `asg` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2699">Added `asg` application security group commands</span></span>
* <span data-ttu-id="b33c5-2700">Argument `--application-security-groups` zu `nic [create|ip-config create|ip-config update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2700">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="b33c5-2701">Argumente `--source-asgs` und `--destination-asgs` zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2701">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="b33c5-2702">Argumente `--ddos-protection` und `--vm-protection` zu `vnet [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2702">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="b33c5-2703">Befehle vom Typ `network [vnet-gateway|vpn-client|show-url]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2703">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="b33c5-2704">Storage</span><span class="sxs-lookup"><span data-stu-id="b33c5-2704">Storage</span></span>

* <span data-ttu-id="b33c5-2705">Problem behoben, das nach der Aktualisierung des SDK unter Umständen einen Fehler der `storage account network-rule`-Befehle zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="b33c5-2705">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="b33c5-2706">Eventgrid</span><span class="sxs-lookup"><span data-stu-id="b33c5-2706">Eventgrid</span></span>

* <span data-ttu-id="b33c5-2707">Azure Event Grid Python SDK für die Verwendung der neueren API-Version „2017-09-15-preview“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-2707">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="b33c5-2708">SQL</span><span class="sxs-lookup"><span data-stu-id="b33c5-2708">SQL</span></span>

* <span data-ttu-id="b33c5-2709">`sql server list`-Argument `--resource-group` geändert, sodass es nun optional ist.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2709">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="b33c5-2710">Wird es nicht angegeben, werden alle SQL Server-Instanzen im Abonnement zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2710">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="b33c5-2711">Parameter `--no-wait` zu `db [create|copy|restore|update|replica create|create|update]` und `dw [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2711">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="b33c5-2712">KeyVault</span><span class="sxs-lookup"><span data-stu-id="b33c5-2712">Keyvault</span></span>

* <span data-ttu-id="b33c5-2713">Unterstützung für die Keyvault-Befehlsausführung hinter einem Proxy hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2713">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="b33c5-2714">VM</span><span class="sxs-lookup"><span data-stu-id="b33c5-2714">VM</span></span>

* <span data-ttu-id="b33c5-2715">Unterstützung für Verfügbarkeitszone zu `[vm|vmss|disk] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2715">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="b33c5-2716">Problem behoben, das bei Verwendung von `--app-gateway ID` mit `vmss create` einen Fehler zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="b33c5-2716">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="b33c5-2717">Argument `--asgs` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2717">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="b33c5-2718">Unterstützung für die Ausführung von Befehlen auf virtuellen Computern mit `vm run-command` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2718">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="b33c5-2719">[VORSCHAU] Unterstützung für VMSS-Datenträgerverschlüsselung mit `vmss encryption` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2719">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="b33c5-2720">Unterstützung für die Durchführung der Wartung auf virtuellen Computern mit `vm perform-maintenance` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2720">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="b33c5-2721">ACS</span><span class="sxs-lookup"><span data-stu-id="b33c5-2721">ACS</span></span>

* <span data-ttu-id="b33c5-2722">[VORSCHAU] Argument `--orchestrator-release` zu `acs create` für ACS-Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2722">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="b33c5-2723">AppService</span><span class="sxs-lookup"><span data-stu-id="b33c5-2723">Appservice</span></span>

* <span data-ttu-id="b33c5-2724">Neue Möglichkeit zum Aktualisieren und Anzeigen der Authentifizierungseinstellungen mit `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="b33c5-2724">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="b33c5-2725">Backup</span><span class="sxs-lookup"><span data-stu-id="b33c5-2725">Backup</span></span>

* <span data-ttu-id="b33c5-2726">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="b33c5-2726">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="b33c5-2727">11. September 2017</span><span class="sxs-lookup"><span data-stu-id="b33c5-2727">September 11, 2017</span></span>

<span data-ttu-id="b33c5-2728">Version 2.0.17</span><span class="sxs-lookup"><span data-stu-id="b33c5-2728">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="b33c5-2729">Core</span><span class="sxs-lookup"><span data-stu-id="b33c5-2729">Core</span></span>

* <span data-ttu-id="b33c5-2730">Festlegung einer eigenen Korrelations-ID in Telemetrie durch das Befehlsmodul aktiviert</span><span class="sxs-lookup"><span data-stu-id="b33c5-2730">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="b33c5-2731">Ein Problem mit der JSON-Sicherungsdatei wurde behoben, das beim Festlegen des Diagnosemodus für Telemetrie auftrat</span><span class="sxs-lookup"><span data-stu-id="b33c5-2731">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="b33c5-2732">ACS</span><span class="sxs-lookup"><span data-stu-id="b33c5-2732">Acs</span></span>

* <span data-ttu-id="b33c5-2733">Befehl `acs list-locations` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2733">Added `acs list-locations` command</span></span>
* <span data-ttu-id="b33c5-2734">`ssh-key-file` wird mit dem erwarteten Standardwert versehen.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2734">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="b33c5-2735">AppService</span><span class="sxs-lookup"><span data-stu-id="b33c5-2735">Appservice</span></span>

* <span data-ttu-id="b33c5-2736">Neue Möglichkeit zum Erstellen einer Web-App in einer anderen Ressourcengruppe als der des aktiven Diensttarifs</span><span class="sxs-lookup"><span data-stu-id="b33c5-2736">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="b33c5-2737">CDN</span><span class="sxs-lookup"><span data-stu-id="b33c5-2737">CDN</span></span>

* <span data-ttu-id="b33c5-2738">Der Fehler bei `cdn custom-domain create`, dass „CustomDomain“ nicht wiederholbar ist, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2738">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="b33c5-2739">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="b33c5-2739">Extension</span></span>

* <span data-ttu-id="b33c5-2740">Erstrelease</span><span class="sxs-lookup"><span data-stu-id="b33c5-2740">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="b33c5-2741">KeyVault</span><span class="sxs-lookup"><span data-stu-id="b33c5-2741">Keyvault</span></span>

* <span data-ttu-id="b33c5-2742">Problem behoben, aufgrund dessen bei den Berechtigungen für `keyvault set-policy` die Groß-/Kleinschreibung beachtet werden musste</span><span class="sxs-lookup"><span data-stu-id="b33c5-2742">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="b33c5-2743">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="b33c5-2743">Network</span></span>

* <span data-ttu-id="b33c5-2744">`vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2744">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="b33c5-2745">Das Argument `--private-access-services` wurde für `vnet subnet create/update` in `--service-endpoints` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2745">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="b33c5-2746">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2746">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="b33c5-2747">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2747">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="b33c5-2748">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2748">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="b33c5-2749">Resource</span><span class="sxs-lookup"><span data-stu-id="b33c5-2749">Resource</span></span>

* <span data-ttu-id="b33c5-2750">Übergabe von Parameterdefinitionen für Ressourcenrichtlinien in `policy definition create` und `policy definition update` zulassen</span><span class="sxs-lookup"><span data-stu-id="b33c5-2750">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="b33c5-2751">Übergabe von Parameterwerten für `policy assignment create` zulassen</span><span class="sxs-lookup"><span data-stu-id="b33c5-2751">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="b33c5-2752">Übergabe von JSON-Code oder einer Datei für alle Parameter zulassen</span><span class="sxs-lookup"><span data-stu-id="b33c5-2752">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="b33c5-2753">Inkrementierte API-Version</span><span class="sxs-lookup"><span data-stu-id="b33c5-2753">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="b33c5-2754">SQL</span><span class="sxs-lookup"><span data-stu-id="b33c5-2754">SQL</span></span>

* <span data-ttu-id="b33c5-2755">Befehle vom Typ `sql server vnet-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2755">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="b33c5-2756">VM</span><span class="sxs-lookup"><span data-stu-id="b33c5-2756">VM</span></span>

* <span data-ttu-id="b33c5-2757">Behoben: Zugriff nur zuweisen, wenn `--scope` angegeben wird</span><span class="sxs-lookup"><span data-stu-id="b33c5-2757">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="b33c5-2758">Behoben: Gleiche Erweiterungsbenennung wie Portal verwenden</span><span class="sxs-lookup"><span data-stu-id="b33c5-2758">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="b33c5-2759">`subscription` aus der Ausgabe von `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2759">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="b33c5-2760">Behoben: Speicher-SKU vom Typ `[vm|vmss] create` wird nicht auf Datenträger mit einem Image angewendet.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2760">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="b33c5-2761">Behoben: `vm format-secret --secrets` akzeptierte keine durch neue Zeilen getrennte IDs.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2761">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="b33c5-2762">31. August 2017</span><span class="sxs-lookup"><span data-stu-id="b33c5-2762">August 31, 2017</span></span>

<span data-ttu-id="b33c5-2763">Version 2.0.16</span><span class="sxs-lookup"><span data-stu-id="b33c5-2763">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="b33c5-2764">KeyVault</span><span class="sxs-lookup"><span data-stu-id="b33c5-2764">Keyvault</span></span>

* <span data-ttu-id="b33c5-2765">Fehler behoben, der beim Versuch auftrat, die Geheimniscodierung mit `secret download` automatisch aufzulösen</span><span class="sxs-lookup"><span data-stu-id="b33c5-2765">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="b33c5-2766">Sf</span><span class="sxs-lookup"><span data-stu-id="b33c5-2766">Sf</span></span>

* <span data-ttu-id="b33c5-2767">Alle Befehle wurden durch die Service Fabric-Befehlszeilenschnittstelle (sfctl) ersetzt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2767">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="b33c5-2768">Storage</span><span class="sxs-lookup"><span data-stu-id="b33c5-2768">Storage</span></span>

* <span data-ttu-id="b33c5-2769">Problem behoben, aufgrund dessen Speicherkonten nicht in Regionen erstellt werden konnten, die die NetworkACLs-Funktion nicht unterstützen</span><span class="sxs-lookup"><span data-stu-id="b33c5-2769">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="b33c5-2770">Festlegen des Inhaltstyps und der Inhaltscodierung während Blob- und Dateiuploads, wenn weder Inhaltstyp noch Inhaltscodierung angegeben sind</span><span class="sxs-lookup"><span data-stu-id="b33c5-2770">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="b33c5-2771">28. August 2017</span><span class="sxs-lookup"><span data-stu-id="b33c5-2771">August 28, 2017</span></span>

<span data-ttu-id="b33c5-2772">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="b33c5-2772">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="b33c5-2773">Befehlszeilenschnittstelle (CLI)</span><span class="sxs-lookup"><span data-stu-id="b33c5-2773">CLI</span></span>

* <span data-ttu-id="b33c5-2774">Rechtlichen Hinweis zu `--version` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2774">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="b33c5-2775">ACS</span><span class="sxs-lookup"><span data-stu-id="b33c5-2775">ACS</span></span>

* <span data-ttu-id="b33c5-2776">Vorschauregionen korrigiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-2776">Corrected preview regions</span></span>
* <span data-ttu-id="b33c5-2777">Standardmäßiges DNS-Namenspräfix (`dns_name_prefix`) ordnungsgemäß formatiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-2777">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="b33c5-2778">ACS-Befehlsausgabe optimiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-2778">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="b33c5-2779">AppService</span><span class="sxs-lookup"><span data-stu-id="b33c5-2779">Appservice</span></span>

* <span data-ttu-id="b33c5-2780">[BREAKING CHANGE] Inkonsistenzen in der Ausgabe von `az webapp config appsettings [delete|set]` behoben</span><span class="sxs-lookup"><span data-stu-id="b33c5-2780">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="b33c5-2781">Neuen Alias (`-i`) für `az webapp config container set --docker-custom-image-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2781">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="b33c5-2782">`az webapp log show` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="b33c5-2782">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="b33c5-2783">Neue Argumente aus `az webapp delete` verfügbar gemacht, um App Service-Plan, Metriken oder DNS-Registrierung beizubehalten</span><span class="sxs-lookup"><span data-stu-id="b33c5-2783">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="b33c5-2784">Behoben: Korrekte Erkennung der Sloteinstellungen</span><span class="sxs-lookup"><span data-stu-id="b33c5-2784">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="b33c5-2785">IoT</span><span class="sxs-lookup"><span data-stu-id="b33c5-2785">IoT</span></span>

* <span data-ttu-id="b33c5-2786">#3934 behoben: Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="b33c5-2786">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="b33c5-2787">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="b33c5-2787">Network</span></span>

* <span data-ttu-id="b33c5-2788">[BREAKING CHANGE]`vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2788">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="b33c5-2789">[BREAKING CHANGE] Option `--private-access-services` für `--service-endpoints` in `vnet subnet [create|update]` umbenannt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2789">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="b33c5-2790">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2790">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="b33c5-2791">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2791">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="b33c5-2792">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2792">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="b33c5-2793">Profil</span><span class="sxs-lookup"><span data-stu-id="b33c5-2793">Profile</span></span>

* <span data-ttu-id="b33c5-2794">`--msi` und `--msi-port` für die Anmeldung mit der Identität eines virtuellen Computers verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="b33c5-2794">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="b33c5-2795">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="b33c5-2795">Service Fabric</span></span>

* <span data-ttu-id="b33c5-2796">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="b33c5-2796">Preview release</span></span>
* <span data-ttu-id="b33c5-2797">Registrierungsbenutzer-/-kennwortregeln für Befehl vereinfacht</span><span class="sxs-lookup"><span data-stu-id="b33c5-2797">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="b33c5-2798">Kennwortanforderung für Benutzer trotz Parameterübergabe behoben</span><span class="sxs-lookup"><span data-stu-id="b33c5-2798">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="b33c5-2799">Unterstützung für leere Registrierungsanmeldeinformationen (`registry_cred`) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2799">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="b33c5-2800">Storage</span><span class="sxs-lookup"><span data-stu-id="b33c5-2800">Storage</span></span>

* <span data-ttu-id="b33c5-2801">Festlegen des Blobtarifs ermöglicht</span><span class="sxs-lookup"><span data-stu-id="b33c5-2801">Enabled setting blob tier</span></span>
* <span data-ttu-id="b33c5-2802">Argumente `--bypass` und `--default-action` zur Unterstützung von Diensttunneling zu `storage account [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2802">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="b33c5-2803">Befehle zum Hinzufügen von VNet-Regeln und IP-basierten Regeln zu `storage account network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2803">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="b33c5-2804">Dienstverschlüsselung durch vom Kunden verwalteten Schlüssel ermöglicht</span><span class="sxs-lookup"><span data-stu-id="b33c5-2804">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="b33c5-2805">[BREAKING CHANGE] Option `--encryption` für Befehl `az storage account create and az storage account update` in `--encryption-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2805">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="b33c5-2806">Behoben (4220): `az storage account update encryption` – Syntaxkonflikt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2806">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="b33c5-2807">VM</span><span class="sxs-lookup"><span data-stu-id="b33c5-2807">VM</span></span>

* <span data-ttu-id="b33c5-2808">Problem behoben, aufgrund dessen bei Verwendung von `--instance-id *` zusätzliche, fehlerhafte Informationen für `vmss get-instance-view` angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="b33c5-2808">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="b33c5-2809">Unterstützung für `--lb-sku` zu `vmss create` hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="b33c5-2809">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="b33c5-2810">Menschliche Namen aus der Administratornamen-Blacklist für `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2810">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="b33c5-2811">Problem behoben, aufgrund dessen `[vm|vmss] create` einen Fehler ausgelöst hat, wenn aus einem Image keine Tarifinformationen extrahiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="b33c5-2811">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="b33c5-2812">Absturzproblem beim Erstellen einer VMMS-Skalierungsgruppe mit einem internen Lastenausgleich behoben</span><span class="sxs-lookup"><span data-stu-id="b33c5-2812">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="b33c5-2813">Problem behoben, aufgrund dessen das Argument `--no-wait` nicht mit `vm availability-set create` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="b33c5-2813">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="b33c5-2814">15. August 2017</span><span class="sxs-lookup"><span data-stu-id="b33c5-2814">August 15, 2017</span></span>

<span data-ttu-id="b33c5-2815">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="b33c5-2815">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="b33c5-2816">ACS</span><span class="sxs-lookup"><span data-stu-id="b33c5-2816">ACS</span></span>

* <span data-ttu-id="b33c5-2817">sshMaster0-Portnummer für Kubernetes korrigiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-2817">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="b33c5-2818">AppService</span><span class="sxs-lookup"><span data-stu-id="b33c5-2818">Appservice</span></span>

* <span data-ttu-id="b33c5-2819">Ausnahme beim Erstellen einer neuen Git-basierten Linux-Web-App behoben</span><span class="sxs-lookup"><span data-stu-id="b33c5-2819">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="b33c5-2820">Event Grid</span><span class="sxs-lookup"><span data-stu-id="b33c5-2820">Event Grid</span></span>

* <span data-ttu-id="b33c5-2821">SDK-Abhängigkeiten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2821">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="b33c5-2822">11. August 2017</span><span class="sxs-lookup"><span data-stu-id="b33c5-2822">August 11, 2017</span></span>

<span data-ttu-id="b33c5-2823">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="b33c5-2823">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="b33c5-2824">ACS</span><span class="sxs-lookup"><span data-stu-id="b33c5-2824">ACS</span></span>

* <span data-ttu-id="b33c5-2825">Weitere Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2825">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="b33c5-2826">Batch</span><span class="sxs-lookup"><span data-stu-id="b33c5-2826">Batch</span></span>

* <span data-ttu-id="b33c5-2827">Auf Batch SDK 3.1.0 und Batch Management SDK 4.1.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-2827">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="b33c5-2828">Neuen Befehl zum Anzeigen der Aufgabenanzahl eines Auftrags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2828">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="b33c5-2829">Fehler in der SAS-URL-Verarbeitung der Ressourcendatei behoben</span><span class="sxs-lookup"><span data-stu-id="b33c5-2829">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="b33c5-2830">Batch-Kontoendpunkt unterstützt nun optionales Präfix „https://“</span><span class="sxs-lookup"><span data-stu-id="b33c5-2830">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="b33c5-2831">Unterstützung für das Hinzufügen von Listen mit mehr als 100 Aufgaben zu einem Auftrag</span><span class="sxs-lookup"><span data-stu-id="b33c5-2831">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="b33c5-2832">Debugprotokollierung für das Laden des Erweiterungsbefehlsmoduls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2832">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="b33c5-2833">Komponente</span><span class="sxs-lookup"><span data-stu-id="b33c5-2833">Component</span></span>

* <span data-ttu-id="b33c5-2834">Warnung für veraltete Befehle vom Typ „az component“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2834">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="b33c5-2835">Container</span><span class="sxs-lookup"><span data-stu-id="b33c5-2835">Container</span></span>

* <span data-ttu-id="b33c5-2836">`create`: Problem behoben, aufgrund dessen das Gleichheitszeichen innerhalb einer Umgebungsvariablen nicht zulässig war</span><span class="sxs-lookup"><span data-stu-id="b33c5-2836">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="b33c5-2837">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="b33c5-2837">Data Lake Store</span></span>

* <span data-ttu-id="b33c5-2838">Fortschrittsüberwachung ermöglicht</span><span class="sxs-lookup"><span data-stu-id="b33c5-2838">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="b33c5-2839">Event Grid</span><span class="sxs-lookup"><span data-stu-id="b33c5-2839">Event Grid</span></span>

* <span data-ttu-id="b33c5-2840">Erste Veröffentlichung</span><span class="sxs-lookup"><span data-stu-id="b33c5-2840">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="b33c5-2841">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="b33c5-2841">Network</span></span>

* <span data-ttu-id="b33c5-2842">`lb`: Problem behoben, aufgrund dessen bestimmte Namen untergeordneter Ressourcen bei Auslassung nicht richtig aufgelöst wurden</span><span class="sxs-lookup"><span data-stu-id="b33c5-2842">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="b33c5-2843">`application-gateway {subresource} delete`: Problem behoben, aufgrund dessen `--no-wait` nicht berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="b33c5-2843">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="b33c5-2844">`application-gateway http-settings update`: Problem behoben, aufgrund dessen `--connection-draining-timeout` nicht deaktiviert werden konnte</span><span class="sxs-lookup"><span data-stu-id="b33c5-2844">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="b33c5-2845">Fehler behoben: Unerwartetes Schlüsselwortargument `sa_data_size_kilobyes` bei `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="b33c5-2845">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="b33c5-2846">Profil</span><span class="sxs-lookup"><span data-stu-id="b33c5-2846">Profile</span></span>

* <span data-ttu-id="b33c5-2847">`account list`: `--refresh` hinzugefügt, um die neuesten Abonnements vom Server zu synchronisieren</span><span class="sxs-lookup"><span data-stu-id="b33c5-2847">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="b33c5-2848">Storage</span><span class="sxs-lookup"><span data-stu-id="b33c5-2848">Storage</span></span>

* <span data-ttu-id="b33c5-2849">Aktualisieren des Speicherkontos mit vom System zugewiesener Identität ermöglicht</span><span class="sxs-lookup"><span data-stu-id="b33c5-2849">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="b33c5-2850">VM</span><span class="sxs-lookup"><span data-stu-id="b33c5-2850">VM</span></span>

* <span data-ttu-id="b33c5-2851">`availability-set`: Fehlerdomänenanzahl bei Konvertierung verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="b33c5-2851">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="b33c5-2852">Befehl `list-skus` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="b33c5-2852">Exposed `list-skus` command</span></span>
* <span data-ttu-id="b33c5-2853">Unterstützung der Identitätszuweisung ohne Erstellung von Rollenzuweisungen</span><span class="sxs-lookup"><span data-stu-id="b33c5-2853">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="b33c5-2854">Anwenden von Speicher-SKU beim Anfügen von Datenträgern</span><span class="sxs-lookup"><span data-stu-id="b33c5-2854">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="b33c5-2855">Standardmäßiger Betriebssystemdatenträger-Name und Speicher-SKU bei Verwendung verwalteter Datenträger entfernt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2855">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="b33c5-2856">28. Juli 2017</span><span class="sxs-lookup"><span data-stu-id="b33c5-2856">July 28, 2017</span></span>

<span data-ttu-id="b33c5-2857">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="b33c5-2857">Version 2.0.12</span></span>

* <span data-ttu-id="b33c5-2858">Containerbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2858">Added container commands</span></span>
* <span data-ttu-id="b33c5-2859">Abrechnungs- und Nutzungsmodule hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2859">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="b33c5-2860">Core</span><span class="sxs-lookup"><span data-stu-id="b33c5-2860">Core</span></span>

* <span data-ttu-id="b33c5-2861">Ausgabe von SDK-Authentifizierungsinformationen für Dienstprinzipale mit Zertifikaten</span><span class="sxs-lookup"><span data-stu-id="b33c5-2861">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="b33c5-2862">Ausnahmen beim Bereitstellungsfortschritt behoben</span><span class="sxs-lookup"><span data-stu-id="b33c5-2862">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="b33c5-2863">Verwendung des ARM-Endpunkts aus der aktuellen Cloud für die Erstellung des Abonnementclients</span><span class="sxs-lookup"><span data-stu-id="b33c5-2863">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="b33c5-2864">Gleichzeitige Verarbeitung der Datei „clouds.config“ verbessert (3636)</span><span class="sxs-lookup"><span data-stu-id="b33c5-2864">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="b33c5-2865">Aktualisierung der Clientanforderungs-ID für jede Befehlsausführung</span><span class="sxs-lookup"><span data-stu-id="b33c5-2865">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="b33c5-2866">Erstellung von Abonnementclients mit richtigem SDK-Profil (3635)</span><span class="sxs-lookup"><span data-stu-id="b33c5-2866">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="b33c5-2867">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="b33c5-2867">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="b33c5-2868">Unterstützung für Auswahl von Tabellenausgabefeldern über jmespath Abfrage hinzugefügt (3581)</span><span class="sxs-lookup"><span data-stu-id="b33c5-2868">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="b33c5-2869">Stummschaltung von Analyseargumenten und Anfügeverlauf mit Gesten verbessert (3434)</span><span class="sxs-lookup"><span data-stu-id="b33c5-2869">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="b33c5-2870">Erstellung von Abonnementclients mit richtigem SDK-Profil</span><span class="sxs-lookup"><span data-stu-id="b33c5-2870">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="b33c5-2871">Verschiebung aller vorhandenen Erfassungsdateien in den neuesten Ordner</span><span class="sxs-lookup"><span data-stu-id="b33c5-2871">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="b33c5-2872">Idempotenz für VM-/VMSS-Erstellung behoben (3586)</span><span class="sxs-lookup"><span data-stu-id="b33c5-2872">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="b33c5-2873">Bei Befehlspfaden wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2873">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="b33c5-2874">Bei bestimmten booleschen Parametern wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2874">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="b33c5-2875">Unterstützung der Anmeldung bei lokalem AD FS-Server wie Azure Stack</span><span class="sxs-lookup"><span data-stu-id="b33c5-2875">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="b33c5-2876">Gleichzeitige Schreibvorgänge in „clouds.config“ behoben (3255)</span><span class="sxs-lookup"><span data-stu-id="b33c5-2876">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="b33c5-2877">ACR</span><span class="sxs-lookup"><span data-stu-id="b33c5-2877">ACR</span></span>

* <span data-ttu-id="b33c5-2878">Befehl `show-usage` für verwaltete Registrierungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2878">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="b33c5-2879">Unterstützung der SKU-Aktualisierung für verwaltete Registrierungen</span><span class="sxs-lookup"><span data-stu-id="b33c5-2879">Support SKU update for managed registries</span></span>
* <span data-ttu-id="b33c5-2880">Verwaltete Registrierungen mit verwalteter SKU hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2880">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="b33c5-2881">Webhooks für verwaltete Registrierungen mit ACR-Webhook-Befehlsmodul hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2881">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="b33c5-2882">AAD-Authentifizierung mit ACR-Anmeldebefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2882">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="b33c5-2883">Löschbefehl für Docker-Repositorys, Manifeste und Tags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2883">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="b33c5-2884">ACS</span><span class="sxs-lookup"><span data-stu-id="b33c5-2884">ACS</span></span>

* <span data-ttu-id="b33c5-2885">Unterstützung der API-Version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="b33c5-2885">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="b33c5-2886">AppService</span><span class="sxs-lookup"><span data-stu-id="b33c5-2886">Appservice</span></span>

* <span data-ttu-id="b33c5-2887">Fehler behoben, aufgrund dessen die Auflistung der Linux-Web-App keine Werte zurückgegeben hat</span><span class="sxs-lookup"><span data-stu-id="b33c5-2887">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="b33c5-2888">Unterstützung für das Abrufen von Anmeldeinformationen aus dem ACR</span><span class="sxs-lookup"><span data-stu-id="b33c5-2888">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="b33c5-2889">Entfernung aller Befehle unter `appservice web`</span><span class="sxs-lookup"><span data-stu-id="b33c5-2889">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="b33c5-2890">Maskierung von Docker-Registrierungskennwörtern aus der Befehlsausgabe (3656)</span><span class="sxs-lookup"><span data-stu-id="b33c5-2890">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="b33c5-2891">Gewährleistung der fehlerfreien Verwendung des Standardbrowsers unter macOS (3623)</span><span class="sxs-lookup"><span data-stu-id="b33c5-2891">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="b33c5-2892">Verbesserung des Nutzens von `webapp log tail` und `webapp log download` (3624)</span><span class="sxs-lookup"><span data-stu-id="b33c5-2892">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="b33c5-2893">Befehl `traffic-routing` zum Konfigurieren des statischen Routings verfügbar gemacht (3566)</span><span class="sxs-lookup"><span data-stu-id="b33c5-2893">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="b33c5-2894">Zuverlässigkeit beim Konfigurieren der Quellcodeverwaltung verbessert (3245)</span><span class="sxs-lookup"><span data-stu-id="b33c5-2894">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="b33c5-2895">Nicht unterstütztes Argument `--node-version` aus `webapp config update` für Windows-Web-Apps entfernt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2895">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="b33c5-2896">Verwenden Sie stattdessen `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2896">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="b33c5-2897">Batch</span><span class="sxs-lookup"><span data-stu-id="b33c5-2897">Batch</span></span>

* <span data-ttu-id="b33c5-2898">Auf Batch SDK 3.0.0 mit Unterstützung virtueller Computer mit niedriger Priorität in Pools aktualisiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-2898">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="b33c5-2899">`pool create`-Option `--target-dedicated` in `--target-dedicated-nodes` umbenannt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2899">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="b33c5-2900">`pool create`-Optionen `--target-low-priority-nodes` und `--application-licenses` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2900">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="b33c5-2901">CDN</span><span class="sxs-lookup"><span data-stu-id="b33c5-2901">CDN</span></span>

* <span data-ttu-id="b33c5-2902">Besser verständliche Fehlermeldung für `cdn endpoint list`, wenn das von `--profile-name` angegebene Profil nicht vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="b33c5-2902">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="b33c5-2903">Cloud</span><span class="sxs-lookup"><span data-stu-id="b33c5-2903">Cloud</span></span>

* <span data-ttu-id="b33c5-2904">API-Version des Cloudmetadaten-Endpunkts in das Format JJJJ-MM-TT umgewandelt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2904">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="b33c5-2905">Katalogendpunkt nicht erforderlich</span><span class="sxs-lookup"><span data-stu-id="b33c5-2905">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="b33c5-2906">Unterstützung für die Cloudregistrierung nur mit ARM-Endpunkt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2906">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="b33c5-2907">Option für `cloud set` bereitgestellt, um beim Auswählen der aktuellen Cloud das Profil auswählen zu können</span><span class="sxs-lookup"><span data-stu-id="b33c5-2907">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="b33c5-2908">`endpoint_vm_image_alias_doc` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="b33c5-2908">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="b33c5-2909">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="b33c5-2909">CosmosDB</span></span>

* <span data-ttu-id="b33c5-2910">Möglichkeit zum Erstellen einer Auflistung mit benutzerdefiniertem Partitionsschlüssel behoben</span><span class="sxs-lookup"><span data-stu-id="b33c5-2910">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="b33c5-2911">Unterstützung für Auflistungs-Standardgültigkeitsdauer hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2911">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="b33c5-2912">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="b33c5-2912">Data Lake Analytics</span></span>

* <span data-ttu-id="b33c5-2913">Zusätzliche Befehle für Compute-Richtlinienverwaltung unter der Überschrift `dla account compute-policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2913">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="b33c5-2914">`dla job pipeline show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2914">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="b33c5-2915">`dla job recurrence list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2915">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="b33c5-2916">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="b33c5-2916">Data Lake Store</span></span>

* <span data-ttu-id="b33c5-2917">Unterstützung für vom Benutzer verwaltete Schlüsseltresor-Schlüsselrotation in `dls account update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2917">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="b33c5-2918">Zugrunde liegende SDK-Version des Data Lake Store-Dateisystems aktualisiert, um ein Leistungsproblem zu behandeln</span><span class="sxs-lookup"><span data-stu-id="b33c5-2918">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="b33c5-2919">Befehl `dls enable-key-vault` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2919">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="b33c5-2920">Dieser Befehl versucht, eine vom Benutzer angegebene Key Vault-Instanz zur Verschlüsselung der Daten in einem Data Lake Store-Konto zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2920">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="b33c5-2921">Interactive</span><span class="sxs-lookup"><span data-stu-id="b33c5-2921">Interactive</span></span>

* <span data-ttu-id="b33c5-2922">Startzeit durch Verwendung zwischengespeicherter Befehle verbessert</span><span class="sxs-lookup"><span data-stu-id="b33c5-2922">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="b33c5-2923">Testabdeckung verbessert</span><span class="sxs-lookup"><span data-stu-id="b33c5-2923">Increased test coverage</span></span>
* <span data-ttu-id="b33c5-2924">?-Geste erweitert, sodass sie auch in den nächsten Befehl eingefügt wird</span><span class="sxs-lookup"><span data-stu-id="b33c5-2924">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="b33c5-2925">Interaktive Fehler mit dem Profil „2017-03-09-profile-preview“ behoben (3587)</span><span class="sxs-lookup"><span data-stu-id="b33c5-2925">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="b33c5-2926">`--version` als Parameter für den interaktiven Modus zugelassen (3645)</span><span class="sxs-lookup"><span data-stu-id="b33c5-2926">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="b33c5-2927">Beseitigung von Fehlern im interaktiven Modus beim Abschluss von Überprüfungen (3570)</span><span class="sxs-lookup"><span data-stu-id="b33c5-2927">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="b33c5-2928">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="b33c5-2928">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="b33c5-2929">Flag `--progress` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2929">Added `--progress` flag</span></span>
* <span data-ttu-id="b33c5-2930">`--debug` und `--verbose` aus Abschlüssen entfernt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2930">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="b33c5-2931">`interactive` aus Abschlüssen entfernt (3324)</span><span class="sxs-lookup"><span data-stu-id="b33c5-2931">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="b33c5-2932">IoT</span><span class="sxs-lookup"><span data-stu-id="b33c5-2932">IoT</span></span>

* <span data-ttu-id="b33c5-2933">Behoben: Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="b33c5-2933">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="b33c5-2934">(3934)</span><span class="sxs-lookup"><span data-stu-id="b33c5-2934">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="b33c5-2935">Schlüsseltresor</span><span class="sxs-lookup"><span data-stu-id="b33c5-2935">Key vault</span></span>

* <span data-ttu-id="b33c5-2936">Befehle für Schlüsseltresor-Wiederherstellungsfeatures hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="b33c5-2936">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="b33c5-2937">`keyvault`-Unterbefehle: `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="b33c5-2937">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="b33c5-2938">`keyvault secret`-Unterbefehle: `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="b33c5-2938">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="b33c5-2939">`keyvault certificate`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="b33c5-2939">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="b33c5-2940">`keyvault key`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="b33c5-2940">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="b33c5-2941">Dienstprinzipal-Schlüsseltresorintegration hinzugefügt (3133)</span><span class="sxs-lookup"><span data-stu-id="b33c5-2941">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="b33c5-2942">Schlüsseltresor-Datenebene auf 0.3.2. aktualisiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-2942">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="b33c5-2943">(3307)</span><span class="sxs-lookup"><span data-stu-id="b33c5-2943">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="b33c5-2944">Labor</span><span class="sxs-lookup"><span data-stu-id="b33c5-2944">Lab</span></span>

* <span data-ttu-id="b33c5-2945">Unterstützung für Übernahme eines beliebigen virtuellen Computers im Labor über `az lab vm claim` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2945">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="b33c5-2946">Tabellenausgabeformatierer für `az lab vm list` und `az lab vm show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2946">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="b33c5-2947">Überwachen</span><span class="sxs-lookup"><span data-stu-id="b33c5-2947">Monitor</span></span>

* <span data-ttu-id="b33c5-2948">Korrektur für Vorlagendatei mit Befehl `monitor autoscale-settings get-parameters-template` (3349)</span><span class="sxs-lookup"><span data-stu-id="b33c5-2948">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="b33c5-2949">`monitor alert-rule-incidents list` in `monitor alert list-incidents` umbenannt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2949">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="b33c5-2950">`monitor alert-rule-incidents show` in `monitor alert show-incident` umbenannt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2950">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="b33c5-2951">`monitor metric-defintions list` in `monitor metrics list-definitions` umbenannt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2951">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="b33c5-2952">`monitor alert-rules` in `monitor alert` umbenannt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2952">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="b33c5-2953">`monitor alert create` geändert:</span><span class="sxs-lookup"><span data-stu-id="b33c5-2953">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="b33c5-2954">Unterbefehle vom Typ `condition` und `action` akzeptieren keinen JSON-Code mehr.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2954">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="b33c5-2955">Hinzufügung zahlreicher Parameter zur Vereinfachung der Regelerstellung</span><span class="sxs-lookup"><span data-stu-id="b33c5-2955">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="b33c5-2956">`location` nicht mehr erforderlich</span><span class="sxs-lookup"><span data-stu-id="b33c5-2956">`location` no longer required</span></span>
  * <span data-ttu-id="b33c5-2957">Hinzufügung von Namen- und ID-Unterstützung für Ziel</span><span class="sxs-lookup"><span data-stu-id="b33c5-2957">Add name and ID support for target</span></span>
  * <span data-ttu-id="b33c5-2958">Entfernung von `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="b33c5-2958">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="b33c5-2959">Umbenennung von `is-enabled` in `enabled` (nicht mehr erforderlich)</span><span class="sxs-lookup"><span data-stu-id="b33c5-2959">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="b33c5-2960">`description` wird nun abhängig von der angegebenen Bedingung auf einen Standardwert festgelegt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-2960">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="b33c5-2961">Hinzufügung von Beispielen zur Verdeutlichung des neuen Formats</span><span class="sxs-lookup"><span data-stu-id="b33c5-2961">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="b33c5-2962">Unterstützung von Namen oder IDs für Befehle vom Typ `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="b33c5-2962">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="b33c5-2963">Komfortargumente und Beispiele zu `monitor alert rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2963">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="b33c5-2964">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="b33c5-2964">Network</span></span>

* <span data-ttu-id="b33c5-2965">Befehl `list-private-access-services` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2965">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="b33c5-2966">Argument `--private-access-services` zu `vnet subnet create` und `vnet subnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2966">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="b33c5-2967">Problem behoben, das einen Fehler für `application-gateway redirect-config create` zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="b33c5-2967">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="b33c5-2968">Problem behoben, aufgrund dessen `application-gateway redirect-config update` nicht mit `--no-wait` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="b33c5-2968">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="b33c5-2969">Fehler behoben, der bei der Verwendung des Arguments `--servers` mit `application-gateway address-pool create` und `application-gateway address-pool update` aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="b33c5-2969">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="b33c5-2970">Befehle vom Typ `application-gateway redirect-config` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2970">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="b33c5-2971">Befehle zu `application-gateway ssl-policy` hinzugefügt: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="b33c5-2971">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="b33c5-2972">Argumente zu `application-gateway ssl-policy set` hinzugefügt: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="b33c5-2972">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="b33c5-2973">Argumente zu `application-gateway http-settings create` und `application-gateway http-settings update` hinzugefügt: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="b33c5-2973">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="b33c5-2974">Argumente zu `application-gateway url-path-map create` und `application-gateway url-path-map update` hinzugefügt: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="b33c5-2974">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="b33c5-2975">Argument `--redirect-config` zu `application-gateway url-path-map rule create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2975">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="b33c5-2976">Unterstützung für `--no-wait` zu `application-gateway url-path-map rule delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2976">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="b33c5-2977">Argumente zu `application-gateway probe create` und `application-gateway probe update` hinzugefügt: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="b33c5-2977">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="b33c5-2978">Argument `--redirect-config` zu `application-gateway rule create` und `application-gateway rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2978">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="b33c5-2979">Unterstützung für `--accelerated-networking` zu `nic create` und `nic update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2979">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="b33c5-2980">Argument `--internal-dns-name-suffix` von `nic create` entfernt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2980">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="b33c5-2981">Unterstützung für `--dns-servers` zu `nic update` und `nic create` hinzugefügt: Hinzufügung von Unterstützung für --dns-servers</span><span class="sxs-lookup"><span data-stu-id="b33c5-2981">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="b33c5-2982">Fehler korrigiert, aufgrund dessen `--local-address-prefixes` von `local-gateway create` ignoriert wurde</span><span class="sxs-lookup"><span data-stu-id="b33c5-2982">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="b33c5-2983">Unterstützung für `--dns-servers` zu `vnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2983">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="b33c5-2984">Fehler beim Erstellen eines Peerings ohne Routenfilterung mit `express-route peering create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-2984">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="b33c5-2985">Fehler korrigiert, aufgrund dessen die Argumente `--provider` und `--bandwidth` nicht mit `express-route update` verwendet werden konnten</span><span class="sxs-lookup"><span data-stu-id="b33c5-2985">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="b33c5-2986">Fehler mit Standardlogik von `network watcher show-topology` korrigiert</span><span class="sxs-lookup"><span data-stu-id="b33c5-2986">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="b33c5-2987">Ausgabeformatierung für `network list-usages` verbessert</span><span class="sxs-lookup"><span data-stu-id="b33c5-2987">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="b33c5-2988">Verwendung der standardmäßigen Front-End-IP-Adresse für `application-gateway http-listener create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="b33c5-2988">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="b33c5-2989">Verwendung des Standardadresspools, der HTTP-Standardeinstellungen und des HTTP-Standardlisteners für `application-gateway rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="b33c5-2989">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="b33c5-2990">Verwendung der standardmäßigen Front-End-IP-Adresse und des standardmäßigen Back-End-Pools für `lb rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="b33c5-2990">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="b33c5-2991">Verwendung der standardmäßigen Front-End-IP-Adresse für `lb inbound-nat-rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="b33c5-2991">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="b33c5-2992">Profil</span><span class="sxs-lookup"><span data-stu-id="b33c5-2992">Profile</span></span>

* <span data-ttu-id="b33c5-2993">Unterstützung der Anmeldung innerhalb eines virtuellen Computers mit einer verwalteten Identität</span><span class="sxs-lookup"><span data-stu-id="b33c5-2993">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="b33c5-2994">Unterstützung der Ausgabe für `account show` im SDK-Authentifizierungsdateiformat</span><span class="sxs-lookup"><span data-stu-id="b33c5-2994">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="b33c5-2995">Anzeige von Warnungen für veraltete Befehle bei Verwendung von „--expanded-view“</span><span class="sxs-lookup"><span data-stu-id="b33c5-2995">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="b33c5-2996">Befehl `get-access-token` für die Bereitstellung eines unformatierten AAD-Tokens hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-2996">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="b33c5-2997">Unterstützung der Anmeldung mit einem Benutzerkonto ohne zugeordnete Abonnements</span><span class="sxs-lookup"><span data-stu-id="b33c5-2997">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="b33c5-2998">RDBMS</span><span class="sxs-lookup"><span data-stu-id="b33c5-2998">RDBMS</span></span>

* <span data-ttu-id="b33c5-2999">Unterstützung der abonnementübergreifenden Auflistung von Servern (3417)</span><span class="sxs-lookup"><span data-stu-id="b33c5-2999">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="b33c5-3000">Behoben: `%s` wird aufgrund von fehlendem `% server_type` nicht verarbeitet (3393)</span><span class="sxs-lookup"><span data-stu-id="b33c5-3000">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="b33c5-3001">Dokumentquellenzuordnung behoben und CI-Aufgabe zur Überprüfung hinzugefügt (3361)</span><span class="sxs-lookup"><span data-stu-id="b33c5-3001">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="b33c5-3002">MySQL- und PostgreSQL-Hilfe korrigiert (3369)</span><span class="sxs-lookup"><span data-stu-id="b33c5-3002">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="b33c5-3003">Resource</span><span class="sxs-lookup"><span data-stu-id="b33c5-3003">Resource</span></span>

* <span data-ttu-id="b33c5-3004">Eingabeaufforderungen bei fehlenden Parametern für `group deployment create` verbessert</span><span class="sxs-lookup"><span data-stu-id="b33c5-3004">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="b33c5-3005">Analyse der Syntax `--parameters KEY=VALUE` verbessert</span><span class="sxs-lookup"><span data-stu-id="b33c5-3005">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="b33c5-3006">Probleme behoben, durch die Parameterdateien von `group deployment create` bei Verwendung der Syntax `@<file>` nicht mehr erkannt wurden</span><span class="sxs-lookup"><span data-stu-id="b33c5-3006">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="b33c5-3007">Unterstützung des Arguments `--ids` für Befehle vom Typ `resource` und `managedapp`</span><span class="sxs-lookup"><span data-stu-id="b33c5-3007">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="b33c5-3008">Einige Analyse- und Fehlermeldungen korrigiert (3584)</span><span class="sxs-lookup"><span data-stu-id="b33c5-3008">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="b33c5-3009">Analyse vom Typ `--resource-type` für den Befehl `lock` korrigiert, sodass `<resource-namespace>` und `<resource-type>` akzeptiert werden</span><span class="sxs-lookup"><span data-stu-id="b33c5-3009">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="b33c5-3010">Parameterüberprüfung für Vorlagenlinkvorlagen hinzugefügt (3629)</span><span class="sxs-lookup"><span data-stu-id="b33c5-3010">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="b33c5-3011">Unterstützung für die Angabe von Bereitstellungsparametern mit der Syntax `KEY=VALUE` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-3011">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="b33c5-3012">Role</span><span class="sxs-lookup"><span data-stu-id="b33c5-3012">Role</span></span>

* <span data-ttu-id="b33c5-3013">Unterstützung der Ausgabe im SDK-Authentifizierungsdateiformat für `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="b33c5-3013">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="b33c5-3014">Rollenzuweisungen und dazugehörige AAD-Anwendung beim Löschen eines Dienstprinzipals bereinigt (3610)</span><span class="sxs-lookup"><span data-stu-id="b33c5-3014">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="b33c5-3015">Einbeziehung des Zeitformats in Beschreibungen vom Typ `--start-date` und `--end-date` für `app create`-Argumente</span><span class="sxs-lookup"><span data-stu-id="b33c5-3015">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="b33c5-3016">Anzeige von Warnungen für veraltete Befehle bei Verwendung von `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="b33c5-3016">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="b33c5-3017">Schlüsseltresorintegration zu den Befehlen `create-for-rbac` und `reset-credentials` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-3017">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="b33c5-3018">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="b33c5-3018">Service Fabric</span></span>
* <span data-ttu-id="b33c5-3019">Problem behoben, aufgrund dessen große Dateien in Anwendungen beim Hochladen gekürzt wurden (3666)</span><span class="sxs-lookup"><span data-stu-id="b33c5-3019">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="b33c5-3020">Tests für Service Fabric-Befehle hinzugefügt (3424)</span><span class="sxs-lookup"><span data-stu-id="b33c5-3020">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="b33c5-3021">Zahlreiche Service Fabric-Befehle korrigiert (3234)</span><span class="sxs-lookup"><span data-stu-id="b33c5-3021">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="b33c5-3022">SQL</span><span class="sxs-lookup"><span data-stu-id="b33c5-3022">SQL</span></span>

* <span data-ttu-id="b33c5-3023">Fehlerhafte1 Parameter `--identity` für `sql server create` entfernt</span><span class="sxs-lookup"><span data-stu-id="b33c5-3023">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="b33c5-3024">Kennwortwerte aus der Befehlsausgabe von `sql server create` und `sql server update` entfernt</span><span class="sxs-lookup"><span data-stu-id="b33c5-3024">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="b33c5-3025">Befehle `sql db list-editions` und `sql elastic-pool list-editions` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-3025">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="b33c5-3026">Storage</span><span class="sxs-lookup"><span data-stu-id="b33c5-3026">Storage</span></span>

* <span data-ttu-id="b33c5-3027">Option `--marker` für die Befehle `storage blob list`, `storage container list` und `storage share list` entfernt (3745)</span><span class="sxs-lookup"><span data-stu-id="b33c5-3027">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="b33c5-3028">Erstellung eines reinen HTTPS-Speicherkontos ermöglicht</span><span class="sxs-lookup"><span data-stu-id="b33c5-3028">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="b33c5-3029">Speichermetriken, Protokollierung und CORS-Befehle aktualisiert (3495)</span><span class="sxs-lookup"><span data-stu-id="b33c5-3029">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="b33c5-3030">Ausnahmemeldung von „cors add“ umformuliert (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="b33c5-3030">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="b33c5-3031">Generator im Probelaufmodus des Downloadbatchbefehls in eine Liste konvertiert (3592)</span><span class="sxs-lookup"><span data-stu-id="b33c5-3031">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="b33c5-3032">Problem bei Probelauf des Blobdownloadbatchs behoben (3640) (3592)</span><span class="sxs-lookup"><span data-stu-id="b33c5-3032">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="b33c5-3033">VM</span><span class="sxs-lookup"><span data-stu-id="b33c5-3033">VM</span></span>

* <span data-ttu-id="b33c5-3034">Unterstützung der NSG-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="b33c5-3034">Support configuring nsg</span></span>
* <span data-ttu-id="b33c5-3035">Fehler behoben, aufgrund dessen der DNS-Server nicht ordnungsgemäß konfiguriert wurde</span><span class="sxs-lookup"><span data-stu-id="b33c5-3035">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="b33c5-3036">Unterstützung verwalteter Dienstidentitäten</span><span class="sxs-lookup"><span data-stu-id="b33c5-3036">Support managed service identities</span></span>
* <span data-ttu-id="b33c5-3037">Problem behoben, aufgrund dessen `cmss create` mit einem vorhandenen Lastenausgleich `--backend-pool-name` benötigte</span><span class="sxs-lookup"><span data-stu-id="b33c5-3037">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="b33c5-3038">Festlegung, dass die LUN von mit `vm image create` erstellten Datenträgern mit 0 beginnt</span><span class="sxs-lookup"><span data-stu-id="b33c5-3038">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="b33c5-3039">10. Mai 2017</span><span class="sxs-lookup"><span data-stu-id="b33c5-3039">May 10, 2017</span></span>

<span data-ttu-id="b33c5-3040">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="b33c5-3040">Version 2.0.6</span></span>

* <span data-ttu-id="b33c5-3041">Umbenennen von „documentdb“ in „cosmosdb“</span><span class="sxs-lookup"><span data-stu-id="b33c5-3041">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="b33c5-3042">Hinzufügen von rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="b33c5-3042">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="b33c5-3043">Einbeziehen der Data Lake Analytics- und Data Lake Store-Module</span><span class="sxs-lookup"><span data-stu-id="b33c5-3043">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="b33c5-3044">Einbeziehen des Cognitive Services-Moduls</span><span class="sxs-lookup"><span data-stu-id="b33c5-3044">Include Cognitive Services module</span></span>
* <span data-ttu-id="b33c5-3045">Einbeziehen des Service Fabric-Moduls</span><span class="sxs-lookup"><span data-stu-id="b33c5-3045">Include Service Fabric module</span></span>
* <span data-ttu-id="b33c5-3046">Einbeziehen des interaktiven Moduls (Umbenennen von „az-shell“)</span><span class="sxs-lookup"><span data-stu-id="b33c5-3046">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="b33c5-3047">Hinzufügen von Unterstützung für CDN-Befehle</span><span class="sxs-lookup"><span data-stu-id="b33c5-3047">Add support for CDN commands</span></span>
* <span data-ttu-id="b33c5-3048">Entfernen des Containermoduls</span><span class="sxs-lookup"><span data-stu-id="b33c5-3048">Remove Container module</span></span>
* <span data-ttu-id="b33c5-3049">Hinzufügen von „az -v“ als Verknüpfung für „az --version“ ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="b33c5-3049">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="b33c5-3050">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="b33c5-3050">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="b33c5-3051">Core</span><span class="sxs-lookup"><span data-stu-id="b33c5-3051">Core</span></span>

* <span data-ttu-id="b33c5-3052">Core: Erfassen von Ausnahmen, die durch einen nicht registrierten Anbieter verursacht werden, und automatische Registrierung</span><span class="sxs-lookup"><span data-stu-id="b33c5-3052">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="b33c5-3053">Leistung: Dauerhaftes Speichern des ADAL-Tokencaches im Arbeitsspeicher bis zum Prozessende ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="b33c5-3053">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="b33c5-3054">Korrigieren der vom hexadezimalen Fingerabdruck -o tsv zurückgegebenen Bytes ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="b33c5-3054">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="b33c5-3055">Verbessern des Downloads des Schlüsseltresorzertifikats und der AAD-SP-Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="b33c5-3055">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="b33c5-3056">Hinzufügen des Python-Speicherorts zu „az –version“ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="b33c5-3056">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="b33c5-3057">Anmeldung: Unterstützung der Anmeldung, wenn keine Abonnements vorhanden sind ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="b33c5-3057">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="b33c5-3058">Core: Beheben eines Fehlers bei zweimaliger Verwendung eines Dienstprinzipals bei der Anmeldung ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="b33c5-3058">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="b33c5-3059">Core: Ermöglichen der Konfiguration des Dateipfads von „accessTokens.json“ über eine Umgebungsvariable ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="b33c5-3059">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="b33c5-3060">Core: Zulassen der Anwendung konfigurierter Standardwerte auf optionale Argumente ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="b33c5-3060">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="b33c5-3061">Core: Verbesserte Leistung</span><span class="sxs-lookup"><span data-stu-id="b33c5-3061">core: Improved performance</span></span>
* <span data-ttu-id="b33c5-3062">Core: Zertifikate von benutzerdefinierter Zertifizierungsstelle – Unterstützung für das Festlegen der REQUESTS_CA_BUNDLE-Umgebungsvariablen</span><span class="sxs-lookup"><span data-stu-id="b33c5-3062">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="b33c5-3063">Core: Cloudkonfiguration – Verwenden des Endpunkts „resource manager“, wenn Endpunkt „management“ nicht festgelegt ist</span><span class="sxs-lookup"><span data-stu-id="b33c5-3063">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="b33c5-3064">ACS</span><span class="sxs-lookup"><span data-stu-id="b33c5-3064">ACS</span></span>

* <span data-ttu-id="b33c5-3065">Korrigieren der Master- und Agentanzahl als ganze Zahl statt Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b33c5-3065">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="b33c5-3066">Verfügbarmachen von „az acs create --no-wait“ und „az acs wait“ für die asynchrone Erstellung</span><span class="sxs-lookup"><span data-stu-id="b33c5-3066">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="b33c5-3067">Verfügbarmachen von „az acs create --validate“ für Probelaufüberprüfungen</span><span class="sxs-lookup"><span data-stu-id="b33c5-3067">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="b33c5-3068">Entfernen von Windows-Profil vor PUT-Aufruf für Skalierungsbefehl ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="b33c5-3068">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="b33c5-3069">AppService</span><span class="sxs-lookup"><span data-stu-id="b33c5-3069">AppService</span></span>

* <span data-ttu-id="b33c5-3070">functionapp: Hinzufügen der vollständigen functionapp-Unterstützung, einschließlich Erstellen, Anzeigen, Auflisten, Löschen, Hostname, SSL usw.</span><span class="sxs-lookup"><span data-stu-id="b33c5-3070">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="b33c5-3071">Hinzufügen von Team Services (vsts) als Continuous Delivery-Option zu „appservice web source-control config“</span><span class="sxs-lookup"><span data-stu-id="b33c5-3071">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="b33c5-3072">Erstellen von „az webapp“ als Ersatz für „az appservice web“ (für Abwärtskompatibilität bleibt „az appservice web“ für 2 weitere Releases erhalten)</span><span class="sxs-lookup"><span data-stu-id="b33c5-3072">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="b33c5-3073">Verfügbarmachen von Argumenten zum Konfigurieren von Bereitstellung und Laufzeitstapeln beim Erstellen von Web-Apps</span><span class="sxs-lookup"><span data-stu-id="b33c5-3073">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="b33c5-3074">Verfügbarmachen von „webapp list-runtimes“</span><span class="sxs-lookup"><span data-stu-id="b33c5-3074">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="b33c5-3075">Unterstützen der Konfiguration von Verbindungszeichenfolgen ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="b33c5-3075">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="b33c5-3076">Unterstützen des Slottauschs mit Vorschau</span><span class="sxs-lookup"><span data-stu-id="b33c5-3076">support slot swap with preview</span></span>
* <span data-ttu-id="b33c5-3077">Beheben von Fehlern in appservice-Befehlen ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="b33c5-3077">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="b33c5-3078">Verwenden der Ressourcengruppe des App Service-Plans für Zertifizierungsvorgänge ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="b33c5-3078">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="b33c5-3079">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="b33c5-3079">CosmosDB</span></span>

* <span data-ttu-id="b33c5-3080">Umbenennen des documentdb-Moduls in cosmosdb</span><span class="sxs-lookup"><span data-stu-id="b33c5-3080">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="b33c5-3081">Zusätzliche Unterstützung für documentdb-APIs auf Datenebene: Datenbank- und Sammlungsverwaltung</span><span class="sxs-lookup"><span data-stu-id="b33c5-3081">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="b33c5-3082">Zusätzliche Unterstützung für das Aktivieren des automatischen Failovers für Datenbankkonten</span><span class="sxs-lookup"><span data-stu-id="b33c5-3082">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="b33c5-3083">Zusätzliche Unterstützung für die neue ConsistentPrefix-Konsistenzrichtlinie</span><span class="sxs-lookup"><span data-stu-id="b33c5-3083">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="b33c5-3084">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="b33c5-3084">Data Lake Analytics</span></span>

* <span data-ttu-id="b33c5-3085">Beheben eines Fehlers, bei dem das Filtern von Auftragslisten nach Ergebnis und Status einen Fehler auslöst</span><span class="sxs-lookup"><span data-stu-id="b33c5-3085">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="b33c5-3086">Hinzufügen von Unterstützung für den neuen Katalogelementtyp „Paket“</span><span class="sxs-lookup"><span data-stu-id="b33c5-3086">Add support for new catalog item type: package.</span></span> <span data-ttu-id="b33c5-3087">Zugriff über: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="b33c5-3087">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="b33c5-3088">Ermöglichen der Auflistung folgender Katalogelemente innerhalb einer Datenbank (keine Schemaspezifikation erforderlich):</span><span class="sxs-lookup"><span data-stu-id="b33c5-3088">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="b33c5-3089">Tabelle</span><span class="sxs-lookup"><span data-stu-id="b33c5-3089">Table</span></span>
  * <span data-ttu-id="b33c5-3090">Tabellenwertfunktion</span><span class="sxs-lookup"><span data-stu-id="b33c5-3090">Table valued function</span></span>
  * <span data-ttu-id="b33c5-3091">Sicht</span><span class="sxs-lookup"><span data-stu-id="b33c5-3091">View</span></span>
  * <span data-ttu-id="b33c5-3092">Tabellenstatistiken.</span><span class="sxs-lookup"><span data-stu-id="b33c5-3092">Table Statistics.</span></span> <span data-ttu-id="b33c5-3093">Können auch mit einem Schema, jedoch ohne Angabe eines Tabellennamens aufgelistet werden.</span><span class="sxs-lookup"><span data-stu-id="b33c5-3093">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="b33c5-3094">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="b33c5-3094">Data Lake Store</span></span>

* <span data-ttu-id="b33c5-3095">Aktualisieren der Version des zugrunde liegenden Dateisystem-SDK, wodurch eine bessere Unterstützung für die Verarbeitung von Drosselungsszenarien auf Serverseite gewährt wird</span><span class="sxs-lookup"><span data-stu-id="b33c5-3095">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="b33c5-3096">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="b33c5-3096">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="b33c5-3097">Fehlende Hilfe für Zugriffsanzeige</span><span class="sxs-lookup"><span data-stu-id="b33c5-3097">missed help for access show.</span></span> <span data-ttu-id="b33c5-3098">hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="b33c5-3098">adding it.</span></span> <span data-ttu-id="b33c5-3099">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="b33c5-3099">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="b33c5-3100">Suchen</span><span class="sxs-lookup"><span data-stu-id="b33c5-3100">Find</span></span>

* <span data-ttu-id="b33c5-3101">Verbessern von Suchergebnissen und Ermöglichen der Versionsverwaltung des Suchindex</span><span class="sxs-lookup"><span data-stu-id="b33c5-3101">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="b33c5-3102">KeyVault</span><span class="sxs-lookup"><span data-stu-id="b33c5-3102">KeyVault</span></span>

* <span data-ttu-id="b33c5-3103">BC:`az keyvault certificate download` Ändern von „-e“ von Zeichenfolge oder Binärdatentyp in PEM oder DER zur besseren Darstellung der Optionen</span><span class="sxs-lookup"><span data-stu-id="b33c5-3103">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="b33c5-3104">BC: Entfernen von „--expires“ und „--not-before“ aus `keyvault certificate create`, da diese Parameter nicht vom Dienst unterstützt werden</span><span class="sxs-lookup"><span data-stu-id="b33c5-3104">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="b33c5-3105">Hinzufügen des Parameters „--validity“ zu `keyvault certificate create`, um gezielt den Wert in „--policy“ zu überschreiben</span><span class="sxs-lookup"><span data-stu-id="b33c5-3105">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="b33c5-3106">Beheben des Problems in `keyvault certificate get-default-policy`, bei dem „expires“ und „not_before“ verfügbar gemacht wurden, „validity_in_months“ hingegen nicht</span><span class="sxs-lookup"><span data-stu-id="b33c5-3106">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="b33c5-3107">Keyvault-Korrektur für den Import von PEM und PFX ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="b33c5-3107">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="b33c5-3108">Labor</span><span class="sxs-lookup"><span data-stu-id="b33c5-3108">Lab</span></span>

* <span data-ttu-id="b33c5-3109">Hinzufügen der Befehle „create“, „show“, „delete“ und „list“ für die Laborumgebung</span><span class="sxs-lookup"><span data-stu-id="b33c5-3109">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="b33c5-3110">Hinzufügen der Befehle „show“ und „list“ zur Anzeige von ARM-Vorlagen im Labor</span><span class="sxs-lookup"><span data-stu-id="b33c5-3110">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="b33c5-3111">Hinzufügen des Kennzeichens „--environment“ in `az lab vm list`, um virtuelle Computer nach Umgebung im Labor zu filtern</span><span class="sxs-lookup"><span data-stu-id="b33c5-3111">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="b33c5-3112">Hinzufügen des benutzerfreundlichen Befehls `az lab formula export-artifacts` zum Exportieren des Artefaktgerüsts innerhalb der Formel eines Labors</span><span class="sxs-lookup"><span data-stu-id="b33c5-3112">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="b33c5-3113">Hinzufügen von Befehlen zum Verwalten von Geheimnissen in einem Labor</span><span class="sxs-lookup"><span data-stu-id="b33c5-3113">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="b33c5-3114">Überwachen</span><span class="sxs-lookup"><span data-stu-id="b33c5-3114">Monitor</span></span>

* <span data-ttu-id="b33c5-3115">Fehlerbehebung: Modellieren von `--actions` von `az alert-rules create` zum Verarbeiten von JSON-Zeichenfolgen ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="b33c5-3115">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="b33c5-3116">Programmfehlerbehebung: Beim Erstellen von Diagnoseeinstellungen werden Protokolle/Metriken aus Anzeigebefehlen nicht akzeptiert ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="b33c5-3116">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="b33c5-3117">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="b33c5-3117">Network</span></span>

* <span data-ttu-id="b33c5-3118">Hinzufügen des `network watcher test-connectivity`-Befehls</span><span class="sxs-lookup"><span data-stu-id="b33c5-3118">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="b33c5-3119">Hinzufügen von Unterstützung für den `--filters`-Parameter für `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="b33c5-3119">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="b33c5-3120">Hinzufügen von Unterstützung für den Application Gateway-Verbindungsausgleich</span><span class="sxs-lookup"><span data-stu-id="b33c5-3120">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="b33c5-3121">Hinzufügen von Unterstützung für die Konfiguration von Application Gateway-WAF-Regelsätzen</span><span class="sxs-lookup"><span data-stu-id="b33c5-3121">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="b33c5-3122">Hinzufügen von Unterstützung für ExpressRoute-Routenfilter und -Regeln</span><span class="sxs-lookup"><span data-stu-id="b33c5-3122">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="b33c5-3123">Hinzufügen von Unterstützung für geografisches TrafficManager-Routing</span><span class="sxs-lookup"><span data-stu-id="b33c5-3123">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="b33c5-3124">Hinzufügen von Unterstützung für richtlinienbasierte Datenverkehrsselektoren für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="b33c5-3124">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="b33c5-3125">Hinzufügen von Unterstützung für IPSec-Richtlinien für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="b33c5-3125">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="b33c5-3126">Korrektur eines Fehlers bei `vpn-connection create` bei Verwendung der Parameter `--no-wait` oder `--validate`</span><span class="sxs-lookup"><span data-stu-id="b33c5-3126">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="b33c5-3127">Hinzufügen von Unterstützung für Aktiv/Aktiv-VNET-Gateways</span><span class="sxs-lookup"><span data-stu-id="b33c5-3127">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="b33c5-3128">Entfernen von NULL-Werten aus der Ausgabe von `network vpn-connection list/show`-Befehlen</span><span class="sxs-lookup"><span data-stu-id="b33c5-3128">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="b33c5-3129">BC: Korrektur eines Fehlers in der Ausgabe von `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="b33c5-3129">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="b33c5-3130">Korrektur eines Fehlers, bei dem das Argument „--key-length“ von „vpn-connection create“ nicht ordnungsgemäß analysiert wurde</span><span class="sxs-lookup"><span data-stu-id="b33c5-3130">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="b33c5-3131">Korrektur eines Fehlers in `dns zone import`, bei dem Datensätze nicht ordnungsgemäß importiert wurden</span><span class="sxs-lookup"><span data-stu-id="b33c5-3131">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="b33c5-3132">Korrektur eines Fehlers, bei dem `traffic-manager endpoint update` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="b33c5-3132">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="b33c5-3133">Hinzufügen von Network Watcher-Vorschaubefehlen</span><span class="sxs-lookup"><span data-stu-id="b33c5-3133">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="b33c5-3134">Profil</span><span class="sxs-lookup"><span data-stu-id="b33c5-3134">Profile</span></span>

* <span data-ttu-id="b33c5-3135">Unterstützung der Anmeldung, wenn keine Abonnements gefunden werden ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="b33c5-3135">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="b33c5-3136">Unterstützung für kurze Parameternamen in „az account set --subscription“ ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="b33c5-3136">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="b33c5-3137">Redis</span><span class="sxs-lookup"><span data-stu-id="b33c5-3137">Redis</span></span>

* <span data-ttu-id="b33c5-3138">Hinzufügen des Updatebefehls, durch den auch die Möglichkeit zum Skalieren für Redis Cache hinzugefügt wird</span><span class="sxs-lookup"><span data-stu-id="b33c5-3138">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="b33c5-3139">Verwerfen des Befehls „update-settings“</span><span class="sxs-lookup"><span data-stu-id="b33c5-3139">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="b33c5-3140">Resource</span><span class="sxs-lookup"><span data-stu-id="b33c5-3140">Resource</span></span>

* <span data-ttu-id="b33c5-3141">Hinzufügen der Befehle „managedapp“ und „managedapp definition“ ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="b33c5-3141">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="b33c5-3142">Unterstützung für die „provider operation“-Befehle ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="b33c5-3142">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="b33c5-3143">Unterstützung für die Erstellung generischer Ressourcen ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="b33c5-3143">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="b33c5-3144">Korrigieren der Ressourcenanalyse und der API-Versionssuche</span><span class="sxs-lookup"><span data-stu-id="b33c5-3144">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="b33c5-3145">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="b33c5-3145">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="b33c5-3146">Hinzufügen von Dokumenten für „az lock update“</span><span class="sxs-lookup"><span data-stu-id="b33c5-3146">Add docs for az lock update.</span></span> <span data-ttu-id="b33c5-3147">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="b33c5-3147">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="b33c5-3148">Beenden mit Fehler bei dem Versuch, Ressourcen für eine nicht vorhandene Gruppe aufzulisten</span><span class="sxs-lookup"><span data-stu-id="b33c5-3148">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="b33c5-3149">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="b33c5-3149">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="b33c5-3150">[Compute] Beheben von Problemen mit dem Update von VMSS- und VM-Verfügbarkeitsgruppen</span><span class="sxs-lookup"><span data-stu-id="b33c5-3150">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="b33c5-3151">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="b33c5-3151">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="b33c5-3152">Korrigieren des Erstellungs- und Löschvorgangs für Sperren, wenn „parent-resource-path“ auf „None“ festgelegt ist ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="b33c5-3152">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="b33c5-3153">Role</span><span class="sxs-lookup"><span data-stu-id="b33c5-3153">Role</span></span>

* <span data-ttu-id="b33c5-3154">create-for-rbac: Sicherstellen, dass das SP-Enddatum nicht das Ablaufdatum des Zertifikats überschreitet ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="b33c5-3154">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="b33c5-3155">RBAC: Hinzufügen vollständiger Unterstützung für „ad group“ ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="b33c5-3155">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="b33c5-3156">Rolle: Beheben von Probleme beim Rollendefinitionsupdate ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="b33c5-3156">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="b33c5-3157">create-for-rbac: Sicherstellen, dass das angegebene Benutzerkennwort übernommen wird</span><span class="sxs-lookup"><span data-stu-id="b33c5-3157">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="b33c5-3158">SQL</span><span class="sxs-lookup"><span data-stu-id="b33c5-3158">SQL</span></span>

* <span data-ttu-id="b33c5-3159">Hinzufügen der Befehle „az sql server list-usages“ und „az sql db list-usages“</span><span class="sxs-lookup"><span data-stu-id="b33c5-3159">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="b33c5-3160">SQL: Möglichkeit zur direkten Verbindung mit Ressourcenanbieter ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="b33c5-3160">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="b33c5-3161">Storage</span><span class="sxs-lookup"><span data-stu-id="b33c5-3161">Storage</span></span>

* <span data-ttu-id="b33c5-3162">Festlegen des Ressourcengruppenstandorts als Standardstandort für `storage account create`</span><span class="sxs-lookup"><span data-stu-id="b33c5-3162">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="b33c5-3163">Hinzufügen von Unterstützung für das inkrementelle Kopieren von Blobs</span><span class="sxs-lookup"><span data-stu-id="b33c5-3163">Add support for incremental blob copy</span></span>
* <span data-ttu-id="b33c5-3164">Hinzufügen von Unterstützung für den Upload umfangreicher Blockblobs</span><span class="sxs-lookup"><span data-stu-id="b33c5-3164">Add support for large block blob upload</span></span>
* <span data-ttu-id="b33c5-3165">Ändern der Blockgröße auf 100 MB, wenn die hochzuladende Datei größer als 200 GB ist</span><span class="sxs-lookup"><span data-stu-id="b33c5-3165">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="b33c5-3166">VM</span><span class="sxs-lookup"><span data-stu-id="b33c5-3166">VM</span></span>

* <span data-ttu-id="b33c5-3167">avail-set: Festlegen der UD- und FD-Domänenanzahl als optional</span><span class="sxs-lookup"><span data-stu-id="b33c5-3167">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="b33c5-3168">Hinweis: VM-Befehle in unabhängigen Clouds: Vermeiden Sie Features im Zusammenhang mit verwalteten Datenträgern, einschließlich der folgenden:</span><span class="sxs-lookup"><span data-stu-id="b33c5-3168">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="b33c5-3169">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="b33c5-3169">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="b33c5-3170">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="b33c5-3170">az vm/vmss disk</span></span>
  3. <span data-ttu-id="b33c5-3171">Verwenden Sie in „az vm/vmss create“ den Befehl „—use-unmanaged-disk“, um verwaltete Datenträger zu vermeiden. Andere Befehle sollten funktionieren.</span><span class="sxs-lookup"><span data-stu-id="b33c5-3171">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="b33c5-3172">vm/vmss: Verbessern des Warnungstexts beim Generieren von SSH-Schlüsselpaaren</span><span class="sxs-lookup"><span data-stu-id="b33c5-3172">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="b33c5-3173">vm/vmss: Unterstützen der Erstellung über ein Marketplace-Image, für das Planinformationen erforderlich sind ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="b33c5-3173">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="b33c5-3174">3\. April 2017</span><span class="sxs-lookup"><span data-stu-id="b33c5-3174">April 3, 2017</span></span>

<span data-ttu-id="b33c5-3175">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="b33c5-3175">Version 2.0.2</span></span>

<span data-ttu-id="b33c5-3176">In dieser Version wurden die Komponenten ACR, Batch, KeyVault und SQL eingeführt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-3176">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="b33c5-3177">Core</span><span class="sxs-lookup"><span data-stu-id="b33c5-3177">Core</span></span>

* <span data-ttu-id="b33c5-3178">Hinzufügen der Module „acr“, „lab“, „monitor“ und „find“ zur Standardliste</span><span class="sxs-lookup"><span data-stu-id="b33c5-3178">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="b33c5-3179">Anmeldung: Überspringen des fehlerhaften Mandanten ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="b33c5-3179">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="b33c5-3180">Anmeldung: Festlegen des Standardabonnements auf ein Abonnement mit dem Status „Enabled“ ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="b33c5-3180">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="b33c5-3181">Hinzufügen von wait-Befehlen und Unterstützung von „--no-wait“ für mehr Befehle ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="b33c5-3181">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="b33c5-3182">Core: Unterstützen der Anmeldung per Dienstprinzipal mit einem Zertifikat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="b33c5-3182">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="b33c5-3183">Hinzufügen der Meldung zu fehlenden Vorlagenparametern</span><span class="sxs-lookup"><span data-stu-id="b33c5-3183">Add prompting for missing template parameters.</span></span> <span data-ttu-id="b33c5-3184">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="b33c5-3184">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="b33c5-3185">Unterstützen des Festlegens von Standardwerten für häufig verwendete Argumente, z.B. Standardressourcengruppe, Standardweb und Standard-VM</span><span class="sxs-lookup"><span data-stu-id="b33c5-3185">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="b33c5-3186">Unterstützen der Anmeldung an einem bestimmten Mandanten</span><span class="sxs-lookup"><span data-stu-id="b33c5-3186">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="b33c5-3187">ACS</span><span class="sxs-lookup"><span data-stu-id="b33c5-3187">ACS</span></span>

* <span data-ttu-id="b33c5-3188">[ACS] Hinzufügen von Unterstützung für die Konfiguration eines ACS-Standardclusters ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="b33c5-3188">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="b33c5-3189">Hinzufügen von Unterstützung der Aufforderung zur Kennworteingabe für SSH-Schlüssel</span><span class="sxs-lookup"><span data-stu-id="b33c5-3189">Add support for ssh key password prompting.</span></span> <span data-ttu-id="b33c5-3190">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="b33c5-3190">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="b33c5-3191">Hinzufügen von Unterstützung für Windows-Cluster</span><span class="sxs-lookup"><span data-stu-id="b33c5-3191">Add support for windows clusters.</span></span> <span data-ttu-id="b33c5-3192">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="b33c5-3192">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="b33c5-3193">Wechseln von der Rolle „Besitzer“ zur Rolle „Mitwirkender“</span><span class="sxs-lookup"><span data-stu-id="b33c5-3193">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="b33c5-3194">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="b33c5-3194">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="b33c5-3195">AppService</span><span class="sxs-lookup"><span data-stu-id="b33c5-3195">AppService</span></span>

* <span data-ttu-id="b33c5-3196">appservice: Unterstützung für das Abrufen der externen IP-Adresse für DNS A-Einträge ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="b33c5-3196">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="b33c5-3197">appservice: Unterstützung der Bindung von Platzhalterzertifikaten ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="b33c5-3197">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="b33c5-3198">appservice: Unterstützung von Veröffentlichungsprofilen für Listen ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="b33c5-3198">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="b33c5-3199">AppService: Auslösen der Synchronisierung der Quellcodeverwaltung nach der Konfiguration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="b33c5-3199">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="b33c5-3200">DataLake</span><span class="sxs-lookup"><span data-stu-id="b33c5-3200">DataLake</span></span>

* <span data-ttu-id="b33c5-3201">Erste Version des Data Lake Analytics-Moduls</span><span class="sxs-lookup"><span data-stu-id="b33c5-3201">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="b33c5-3202">Erste Version des Data Lake Store-Moduls</span><span class="sxs-lookup"><span data-stu-id="b33c5-3202">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="b33c5-3203">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="b33c5-3203">DocuemntDB</span></span>

* <span data-ttu-id="b33c5-3204">DocumentDB: Hinzufügen von Unterstützung für das Auflisten von Verbindungszeichenfolgen ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="b33c5-3204">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="b33c5-3205">VM</span><span class="sxs-lookup"><span data-stu-id="b33c5-3205">VM</span></span>

* <span data-ttu-id="b33c5-3206">[Compute] Hinzufügen von AppGateway-Unterstützung für Erstellung von VM-Skalierungsgruppen ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="b33c5-3206">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="b33c5-3207">[VM/VMSS] Verbesserte Unterstützung für die Datenträgerzwischenspeicherung ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="b33c5-3207">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="b33c5-3208">VM/VMSS: Einbinden der vom Portal verwendeten Logik zur Überprüfung von Anmeldeinformationen ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="b33c5-3208">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="b33c5-3209">Hinzufügen von wait-Befehlen und Unterstützung für „--no-wait“ ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="b33c5-3209">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="b33c5-3210">VM-Skalierungsgruppe: Unterstützung von „\*“ zum Auflisten der übergreifenden Instanzansicht für VMs ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="b33c5-3210">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="b33c5-3211">Hinzufügen – Geheimnisse für virtuellen Computer und VM-Skalierungsgruppe ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="b33c5-3211">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="b33c5-3212">Zulassen der VM-Erstellung mit spezialisierter VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="b33c5-3212">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="b33c5-3213">27. Februar 2017</span><span class="sxs-lookup"><span data-stu-id="b33c5-3213">February 27, 2017</span></span>

<span data-ttu-id="b33c5-3214">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="b33c5-3214">Version 2.0.0</span></span>

<span data-ttu-id="b33c5-3215">Diese Version der Azure CLI 2.0 ist die erste „allgemein verfügbare“ Version. Die allgemeine Verfügbarkeit gilt für die folgenden Befehlsmodule:</span><span class="sxs-lookup"><span data-stu-id="b33c5-3215">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="b33c5-3216">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="b33c5-3216">Container Service (acs)</span></span>
- <span data-ttu-id="b33c5-3217">Compute (einschließlich Resource Manager, VM, VM-Skalierungsgruppen, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="b33c5-3217">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="b33c5-3218">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="b33c5-3218">Networking</span></span>
- <span data-ttu-id="b33c5-3219">Storage</span><span class="sxs-lookup"><span data-stu-id="b33c5-3219">Storage</span></span>

<span data-ttu-id="b33c5-3220">Diese Befehlsmodule können in der Produktion verwendet werden und verfügen über Unterstützung durch eine Standard-SLA von Microsoft. Sie können Anfragen zu Problemen direkt beim Microsoft-Support oder in der [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/) öffnen. Sie haben die Möglichkeit, Fragen in [StackOverflow mit dem Tag „azure-cli“](http://stackoverflow.com/questions/tagged/azure-cli) zu stellen oder sich unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) an das Produktteam zu wenden. Außerdem können Sie über die Befehlszeile mit dem Befehl `az feedback` Feedback senden.</span><span class="sxs-lookup"><span data-stu-id="b33c5-3220">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="b33c5-3221">Die Befehle in diesen Modulen sind stabil, und es ist nicht zu erwarten, dass sich die Syntax in den anstehenden Veröffentlichungen dieser Version der Azure CLI ändern.</span><span class="sxs-lookup"><span data-stu-id="b33c5-3221">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="b33c5-3222">Verwenden Sie zum Überprüfen der Version der CLI den Befehl `az --version`. In der Ausgabe werden die Version der CLI selbst (für diese Veröffentlichung 2.0.0), die einzelnen Befehlsmodule und die von Ihnen genutzten Versionen von Python und GCC aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="b33c5-3222">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="b33c5-3223">Einige Befehlsmodule verfügen über das Postfix „b*n*“ oder „rc*n*“. Diese Befehlsmodule befinden sich noch in der Vorschauphase und werden später die allgemeine Verfügbarkeit erlangen.</span><span class="sxs-lookup"><span data-stu-id="b33c5-3223">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="b33c5-3224">Außerdem werden jeden Abend Vorschaubuilds der CLI bereitgestellt. Informationen hierzu finden Sie in der [Anleitung zum Abrufen der abendlichen Builds](https://github.com/Azure/azure-cli#nightly-builds) und im Abschnitt zum [Setup für Entwickler und Beitragen von Code](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="b33c5-3224">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="b33c5-3225">Sie können für die abendlichen Vorschaubuilds wie folgt Probleme melden:</span><span class="sxs-lookup"><span data-stu-id="b33c5-3225">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="b33c5-3226">Über die [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="b33c5-3226">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="b33c5-3227">Per Kontaktaufnahme mit dem Produktteam unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="b33c5-3227">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="b33c5-3228">Senden von Feedback über die Befehlszeile mit dem Befehl `az feedback`</span><span class="sxs-lookup"><span data-stu-id="b33c5-3228">Provide feedback from the command line with the `az feedback` command</span></span>


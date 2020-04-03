---
title: Versionshinweise für die Azure CLI
description: Enthält Informationen zu den aktuellen Updates der Azure CLI.
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 03/31/2020
ms.topic: article
ms.service: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: aed043bcb900937a405fd71dafe24016fa0972d7
ms.sourcegitcommit: b5ecfc168489cd0d96462d6decf83e8b26a10194
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/31/2020
ms.locfileid: "80417824"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="fc109-103">Versionshinweise für die Azure CLI</span><span class="sxs-lookup"><span data-stu-id="fc109-103">Azure CLI release notes</span></span>

## <a name="march-31-2020"></a><span data-ttu-id="fc109-104">31. März 2020</span><span class="sxs-lookup"><span data-stu-id="fc109-104">March 31, 2020</span></span>

<span data-ttu-id="fc109-105">Version 2.3.0</span><span class="sxs-lookup"><span data-stu-id="fc109-105">Version 2.3.0</span></span>

### <a name="acr"></a><span data-ttu-id="fc109-106">ACR</span><span class="sxs-lookup"><span data-stu-id="fc109-106">ACR</span></span>

* <span data-ttu-id="fc109-107">„az acr task update“: NULL-Zeiger-Ausnahme</span><span class="sxs-lookup"><span data-stu-id="fc109-107">'az acr task update': null pointer exception</span></span>
* <span data-ttu-id="fc109-108">`az acr import`: Hilfe und Fehlermeldung geändert, um die Verwendung von „--source“ und „--registry“ zu verdeutlichen</span><span class="sxs-lookup"><span data-stu-id="fc109-108">`az acr import`: Modify help and error message to clarify the usage of --source and --registry</span></span>
* <span data-ttu-id="fc109-109">Überprüfung für das Argument „registry_name“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-109">Add a validator for argument 'registry_name'</span></span>
* <span data-ttu-id="fc109-110">`az acr login`: Vorschauflag für „--expose-token“ entfernt</span><span class="sxs-lookup"><span data-stu-id="fc109-110">`az acr login`:Remove the preview flag on '--expose-token'</span></span>
* <span data-ttu-id="fc109-111">[BREAKING CHANGE] Branch-Parameter „az acr task create/update“ entfernt</span><span class="sxs-lookup"><span data-stu-id="fc109-111">[BREAKING CHANGE] 'az acr task create/update' Branch parameter is removed</span></span>
* <span data-ttu-id="fc109-112">„az acr task update“: Kunde kann nun Kontext, Git-Token und/oder Trigger einzeln aktualisieren</span><span class="sxs-lookup"><span data-stu-id="fc109-112">'az acr task update' Customer now can update context, git-token, and or triggers individually</span></span>
* <span data-ttu-id="fc109-113">„az acr agentpool“: Neues Feature</span><span class="sxs-lookup"><span data-stu-id="fc109-113">'az acr agentpool': new feature</span></span>

### <a name="aks"></a><span data-ttu-id="fc109-114">AKS</span><span class="sxs-lookup"><span data-stu-id="fc109-114">AKS</span></span>

* <span data-ttu-id="fc109-115">„apiServerAccessProfile“ bei der Aktualisierung von „--api-server-authorized-ip-ranges“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="fc109-115">Fix apiServerAccessProfile when updating --api-server-authorized-ip-ranges</span></span>
* <span data-ttu-id="fc109-116">aks update: Überschreibung ausgehender IP-Adressen mit Eingabewerten bei der Aktualisierung</span><span class="sxs-lookup"><span data-stu-id="fc109-116">aks update: Override outbound IPs with input values when update</span></span>
* <span data-ttu-id="fc109-117">Keine SPN-Erstellung für MSI-Cluster sowie Unterstützung der Anfügung von ACR an MSI-Cluster</span><span class="sxs-lookup"><span data-stu-id="fc109-117">Do not create SPN for MSI clusters and support attach acr to MSI clusters</span></span>

### <a name="ams"></a><span data-ttu-id="fc109-118">AMS</span><span class="sxs-lookup"><span data-stu-id="fc109-118">AMS</span></span>

* <span data-ttu-id="fc109-119">Fix 12469: Hinzufügen von „content-key-policy“ für Fairplay aufgrund von Problemen mit dem Parameter „ask“ nicht erfolgreich</span><span class="sxs-lookup"><span data-stu-id="fc109-119">Fix #12469: adding Fairplay content-key-policy fails due to problems with 'ask' parameter</span></span>

### <a name="appconfig"></a><span data-ttu-id="fc109-120">AppConfig</span><span class="sxs-lookup"><span data-stu-id="fc109-120">AppConfig</span></span>

* <span data-ttu-id="fc109-121">„--skip-keyvault“ für „kv export“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-121">Add --skip-keyvault for kv export</span></span>

### <a name="appservice"></a><span data-ttu-id="fc109-122">AppService</span><span class="sxs-lookup"><span data-stu-id="fc109-122">AppService</span></span>

* <span data-ttu-id="fc109-123">Fix 12509: Tag für „az webapp up“ standardmäßig entfernt</span><span class="sxs-lookup"><span data-stu-id="fc109-123">Fix #12509: Remove the tag to az webapp up by default</span></span>
* <span data-ttu-id="fc109-124">az functionapp create: Hilfemenü für „--runtime-version“ aktualisiert und Warnung hinzugefügt, wenn der Benutzer „--runtime-version“ für .NET angibt</span><span class="sxs-lookup"><span data-stu-id="fc109-124">az functionapp create: Updated --runtime-version help menu and added warning when user specifies --runtime-version for dotnet</span></span>
* <span data-ttu-id="fc109-125">az functionapp create: Methode zum Festlegen von „javaVersion“ für Windows-Funktions-Apps aktualisiert</span><span class="sxs-lookup"><span data-stu-id="fc109-125">az functionapp create: Updated the way javaVersion was being set for Windows function apps</span></span>

### <a name="arm"></a><span data-ttu-id="fc109-126">ARM</span><span class="sxs-lookup"><span data-stu-id="fc109-126">ARM</span></span>

* <span data-ttu-id="fc109-127">az deployment create/validate: Standardmäßige Verwendung von „--handle-extended-json-format“</span><span class="sxs-lookup"><span data-stu-id="fc109-127">az deployment create/validate: Use --handle-extended-json-format by default</span></span>
* <span data-ttu-id="fc109-128">az lock create: Beispiele für die Erstellung einer Unterressource in der Hilfedokumentation hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-128">az lock create: Add examples of creating subresource in the help documentation</span></span>
* <span data-ttu-id="fc109-129">az deployment {group/mg/sub/tenant} list: Unterstützung der provisioningState-Filterung</span><span class="sxs-lookup"><span data-stu-id="fc109-129">az deployment {group/mg/sub/tenant} list: Support provisioningState filtering</span></span>
* <span data-ttu-id="fc109-130">az deployment: Analysefehler für Kommentar unter letztem Argument behoben</span><span class="sxs-lookup"><span data-stu-id="fc109-130">az deployment: Fix the parse bug for comment under the last argument</span></span>

### <a name="backup"></a><span data-ttu-id="fc109-131">Backup</span><span class="sxs-lookup"><span data-stu-id="fc109-131">Backup</span></span>

* <span data-ttu-id="fc109-132">Mehrere Dateiwiederherstellungsfunktionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-132">Added multiple files restore capabilities</span></span>
* <span data-ttu-id="fc109-133">Unterstützung der ausschließlichen Sicherung von Betriebssystemdatenträgern hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-133">Added support for Backing up OS Disks only</span></span>
* <span data-ttu-id="fc109-134">Parameter „restore-as-unmanaged-disk“ für die Angabe einer nicht verwalteten Wiederherstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-134">Added restore-as-unmanaged-disk parameter to specify unmanaged restore</span></span>

### <a name="compute"></a><span data-ttu-id="fc109-135">Compute</span><span class="sxs-lookup"><span data-stu-id="fc109-135">Compute</span></span>

* <span data-ttu-id="fc109-136">az vm create: Option „NONE“ von „--nsg-rule“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-136">az vm create: Add NONE option of --nsg-rule</span></span>
* <span data-ttu-id="fc109-137">az vmss create/update: Vorschautag für automatische VMSS-Reparaturen entfernt</span><span class="sxs-lookup"><span data-stu-id="fc109-137">az vmss create/update: remove vmss automatic repairs preview tag</span></span>
* <span data-ttu-id="fc109-138">az vm update: Unterstützung von „--workspace“</span><span class="sxs-lookup"><span data-stu-id="fc109-138">az vm update: Support --workspace</span></span>
* <span data-ttu-id="fc109-139">Fehler im VirtualMachineScaleSetExtension-Initialisierungscode behoben</span><span class="sxs-lookup"><span data-stu-id="fc109-139">Fix a bug in VirtualMachineScaleSetExtension initialization code</span></span>
* <span data-ttu-id="fc109-140">Upgrade der VMAccessAgent-Version auf 2.4 durchgeführt</span><span class="sxs-lookup"><span data-stu-id="fc109-140">Upgrade VMAccessAgent version to 2.4</span></span>
* <span data-ttu-id="fc109-141">az vmss set-orchestration-service-state: Unterstützung zum Festlegen des Orchestrierungdienstzustands für VMSS</span><span class="sxs-lookup"><span data-stu-id="fc109-141">az vmss set-orchestration-service-state: support vmss set orchestration service state</span></span>
* <span data-ttu-id="fc109-142">Upgrade der Datenträger-API-Version auf 2019-11-01 durchgeführt</span><span class="sxs-lookup"><span data-stu-id="fc109-142">Upgrade disk API version to 2019-11-01</span></span>
* <span data-ttu-id="fc109-143">az disk create: add --disk-iops-read-only, --disk-mbps-read-only, --max-shares, --image-reference, --image-reference-lun, --gallery-image-reference, --gallery-image-reference-lun</span><span class="sxs-lookup"><span data-stu-id="fc109-143">az disk create: add --disk-iops-read-only, --disk-mbps-read-only, --max-shares, --image-reference, --image-reference-lun, --gallery-image-reference, --gallery-image-reference-lun</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="fc109-144">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="fc109-144">Cosmos DB</span></span>

* <span data-ttu-id="fc109-145">Fehlende Option „--type“ für Veraltungsumleitungen korrigiert</span><span class="sxs-lookup"><span data-stu-id="fc109-145">Fix missing --type option for deprecation redirections</span></span>

### <a name="docker"></a><span data-ttu-id="fc109-146">Docker</span><span class="sxs-lookup"><span data-stu-id="fc109-146">Docker</span></span>

* <span data-ttu-id="fc109-147">Update auf Alpine 3.11 und Python 3.6.10 durchgeführt</span><span class="sxs-lookup"><span data-stu-id="fc109-147">Update to Alpine 3.11 and Python 3.6.10</span></span>

### <a name="extension"></a><span data-ttu-id="fc109-148">Erweiterung</span><span class="sxs-lookup"><span data-stu-id="fc109-148">Extension</span></span>

* <span data-ttu-id="fc109-149">Laden von Erweiterungen im Systempfad mittels Paketen ermöglicht</span><span class="sxs-lookup"><span data-stu-id="fc109-149">Allow to load extensions in the system path via packages</span></span>

### <a name="hdinsight"></a><span data-ttu-id="fc109-150">HDInsight</span><span class="sxs-lookup"><span data-stu-id="fc109-150">HDInsight</span></span>

* <span data-ttu-id="fc109-151">(az hdinsight create:) Unterstützung der Angabe der unterstützten TLS-Mindestversion durch Kunden unter Verwendung des Parameters `--minimal-tls-version`.</span><span class="sxs-lookup"><span data-stu-id="fc109-151">(az hdinsight create:) Support customers specify minimal supported tls version by using parameter `--minimal-tls-version`.</span></span> <span data-ttu-id="fc109-152">Zulässiger Wert: 1.0,1.1,1.2</span><span class="sxs-lookup"><span data-stu-id="fc109-152">The allowed value is 1.0,1.1,1.2</span></span>

### <a name="iot"></a><span data-ttu-id="fc109-153">IoT</span><span class="sxs-lookup"><span data-stu-id="fc109-153">IoT</span></span>

* <span data-ttu-id="fc109-154">Codebesitzer hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-154">Add codeowner</span></span>
* <span data-ttu-id="fc109-155">az iot hub create: Standard-SKU von F1 in S1 geändert</span><span class="sxs-lookup"><span data-stu-id="fc109-155">az iot hub create : Change default sku to S1 from F1</span></span>
* <span data-ttu-id="fc109-156">iot hub: Unterstützung von „IotHub“ im Profil „2019-03-01-hybrid“</span><span class="sxs-lookup"><span data-stu-id="fc109-156">iot hub: Support IotHub in the profile of 2019-03-01-hybrid</span></span>

### <a name="iotcentral"></a><span data-ttu-id="fc109-157">IoTCentral</span><span class="sxs-lookup"><span data-stu-id="fc109-157">IoTCentral</span></span>

* <span data-ttu-id="fc109-158">Fehlerdetails sowie Standardanwendungsvorlage und Aufforderungsmeldung aktualisiert</span><span class="sxs-lookup"><span data-stu-id="fc109-158">Update error details, update default application template and prompt message</span></span>

### <a name="keyvault"></a><span data-ttu-id="fc109-159">KeyVault</span><span class="sxs-lookup"><span data-stu-id="fc109-159">KeyVault</span></span>

* <span data-ttu-id="fc109-160">Unterstützung von Zertifikatsicherung/-wiederherstellung</span><span class="sxs-lookup"><span data-stu-id="fc109-160">Support certificate backup/restore</span></span>
* <span data-ttu-id="fc109-161">keyvault create/update: Unterstützung von „--retention-days“</span><span class="sxs-lookup"><span data-stu-id="fc109-161">keyvault create/update: Support --retention-days</span></span>
* <span data-ttu-id="fc109-162">Keine Anzeige von verwalteten Schlüsseln/Geheimnissen bei der Auflistung mehr</span><span class="sxs-lookup"><span data-stu-id="fc109-162">No longer display managed keys/secrets while listing</span></span>
* <span data-ttu-id="fc109-163">az keyvault create: Unterstützung von `--network-acls`, `--network-acls-ips` und `--network-acls-vnets` zur Angabe von Netzwerkregeln bei der Tresorerstellung</span><span class="sxs-lookup"><span data-stu-id="fc109-163">az keyvault create: support `--network-acls`, `--network-acls-ips` and `--network-acls-vnets` for specifying network rules while creating vault</span></span>

### <a name="lock"></a><span data-ttu-id="fc109-164">Sperre</span><span class="sxs-lookup"><span data-stu-id="fc109-164">Lock</span></span>

* <span data-ttu-id="fc109-165">Fehlerbehebung für „az lock delete“: „az lock delete“ funktioniert für „Microsoft.DocumentDB“ nicht.</span><span class="sxs-lookup"><span data-stu-id="fc109-165">az lock delete fix bug: az lock delete does not work on Microsoft.DocumentDB</span></span>

### <a name="monitor"></a><span data-ttu-id="fc109-166">Überwachen</span><span class="sxs-lookup"><span data-stu-id="fc109-166">Monitor</span></span>

* <span data-ttu-id="fc109-167">az monitor clone: Unterstützung des Klonens von Metrikregeln zwischen Ressourcen</span><span class="sxs-lookup"><span data-stu-id="fc109-167">az monitor clone: support clone metric rules from one resource to another</span></span>
* <span data-ttu-id="fc109-168">Fix IcM179210086: Erstellung einer benutzerdefinierten Metrikwarnung für die Application Insights-Metrik nicht möglich</span><span class="sxs-lookup"><span data-stu-id="fc109-168">Fix IcM179210086: unable to create custom metric alert for their Application Insights metric</span></span>

### <a name="netappfiles"></a><span data-ttu-id="fc109-169">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="fc109-169">NetAppFiles</span></span>

* <span data-ttu-id="fc109-170">az volume create: Datenschutzvolumes zum Hinzufügen von Replikationsvorgängen zugelassen: Genehmigen, Aussetzen, Fortsetzen, Status, Entfernen</span><span class="sxs-lookup"><span data-stu-id="fc109-170">az volume create: Allow data protection volumes adding replication operations: approve, suspend, resume, status, remove</span></span>

### <a name="network"></a><span data-ttu-id="fc109-171">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="fc109-171">Network</span></span>

* <span data-ttu-id="fc109-172">az network application-gateway waf-policy managed-rule rule-set add: Unterstützung von „ Microsoft_BotManagerRuleSet“</span><span class="sxs-lookup"><span data-stu-id="fc109-172">az network application-gateway waf-policy managed-rule rule-set add: support Microsoft_BotManagerRuleSet</span></span>
* <span data-ttu-id="fc109-173">network watcher flow-log show: Falsche Veraltungsinformationen behoben</span><span class="sxs-lookup"><span data-stu-id="fc109-173">network watcher flow-log show: fix wrong deprecating info</span></span>
* <span data-ttu-id="fc109-174">Unterstützung von Hostnamen im Application Gateway-Listener</span><span class="sxs-lookup"><span data-stu-id="fc109-174">support host names in application gateway listener</span></span>
* <span data-ttu-id="fc109-175">az network nat gateway: Unterstützung der Erstellung einer leeren Ressource ohne öffentliche IP-Adresse oder Präfix für öffentliche IP-Adressen</span><span class="sxs-lookup"><span data-stu-id="fc109-175">az network nat gateway: support create empty resource without public ip or public ip prefix</span></span>
* <span data-ttu-id="fc109-176">Unterstützung der VPN-Gateway-Generierung</span><span class="sxs-lookup"><span data-stu-id="fc109-176">Support vpn gateway generation</span></span>
* <span data-ttu-id="fc109-177">Unterstützung von `--if-none-match` in `az network dns record-set {} add-record`</span><span class="sxs-lookup"><span data-stu-id="fc109-177">Support `--if-none-match` in `az network dns record-set {} add-record`</span></span>

### <a name="packaging"></a><span data-ttu-id="fc109-178">Verpackung</span><span class="sxs-lookup"><span data-stu-id="fc109-178">Packaging</span></span>

* <span data-ttu-id="fc109-179">Unterstützung von Python 3.5 eingestellt</span><span class="sxs-lookup"><span data-stu-id="fc109-179">Drop support for python 3.5</span></span>

### <a name="profile"></a><span data-ttu-id="fc109-180">Profil</span><span class="sxs-lookup"><span data-stu-id="fc109-180">Profile</span></span>

* <span data-ttu-id="fc109-181">az login: Warnung für MFA-Fehler</span><span class="sxs-lookup"><span data-stu-id="fc109-181">az login: Show warning for MFA error</span></span>

### <a name="rdbms"></a><span data-ttu-id="fc109-182">RDBMS</span><span class="sxs-lookup"><span data-stu-id="fc109-182">RDBMS</span></span>

* <span data-ttu-id="fc109-183">Befehle zur Verwaltung von Verschlüsselungsschlüsseln für Serverdaten für PostgreSQL und MySQL hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-183">Add server data encryption key management commands for PostgreSQL and MySQL</span></span>

## <a name="march-10-2020"></a><span data-ttu-id="fc109-184">10. März 2020</span><span class="sxs-lookup"><span data-stu-id="fc109-184">March 10, 2020</span></span>

<span data-ttu-id="fc109-185">Version 2.2.0</span><span class="sxs-lookup"><span data-stu-id="fc109-185">Version 2.2.0</span></span>

### <a name="acr"></a><span data-ttu-id="fc109-186">ACR</span><span class="sxs-lookup"><span data-stu-id="fc109-186">ACR</span></span>

* <span data-ttu-id="fc109-187">Fix: `az acr login` löst fälschlicherweise Fehler aus</span><span class="sxs-lookup"><span data-stu-id="fc109-187">Fix: `az acr login` wrongly raise error</span></span>
* <span data-ttu-id="fc109-188">Neuer Befehl `az acr helm install-cli` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-188">Add new command `az acr helm install-cli`</span></span>
* <span data-ttu-id="fc109-189">Privater Link und CMK-Unterstützung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-189">Add private link and CMK support</span></span>
* <span data-ttu-id="fc109-190">Befehl „private-link-resource list“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-190">add 'private-link-resource list' command</span></span>

### <a name="aks"></a><span data-ttu-id="fc109-191">AKS</span><span class="sxs-lookup"><span data-stu-id="fc109-191">AKS</span></span>

* <span data-ttu-id="fc109-192">Durchsuchen von AKS in Cloud-Shell korrigiert</span><span class="sxs-lookup"><span data-stu-id="fc109-192">fix the aks browse in cloud shell</span></span>
* <span data-ttu-id="fc109-193">az aks: NoneType-Fehler beim Überwachen von „addon“ und „agentpool“ behoben</span><span class="sxs-lookup"><span data-stu-id="fc109-193">az aks: Fix monitoring addon and agentpool NoneType errors</span></span>
* <span data-ttu-id="fc109-194">„--nodepool-tags“ zum Knotenpool beim Erstellen von Azure-Kubernetes-Clustern hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-194">Add --nodepool-tags to node pool when creating azure kubernetes cluster</span></span>
* <span data-ttu-id="fc109-195">„--tags“ beim Hinzufügen oder Aktualisieren eines Knotenpool in einem Cluster hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-195">Add --tags when adding or updating a nodepool to cluster</span></span>
* <span data-ttu-id="fc109-196">aks create: `--enable-private-cluster` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-196">aks create: add `--enable-private-cluster`</span></span>
* <span data-ttu-id="fc109-197">„--nodepool-labels“ beim Erstellen von Azure-Kubernetes-Clustern hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-197">add --nodepool-labels when creating azure kubernetes cluster</span></span>
* <span data-ttu-id="fc109-198">„--labels“ beim Hinzufügen eines neuen Knotenpools zu einem Azure-Kubernetes-Cluster hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-198">add --labels when adding a new nodepool to azure kubernetes cluster</span></span>
* <span data-ttu-id="fc109-199">Fehlender Schrägstrich (/) in der Dashboard-URL hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-199">add missing / in the dashboard url</span></span>
* <span data-ttu-id="fc109-200">Unterstützung der Erstellung von AKS-Clustern, sodass verwaltete Identitäten möglich sind</span><span class="sxs-lookup"><span data-stu-id="fc109-200">Support create aks clusters enabling managed identity</span></span>
* <span data-ttu-id="fc109-201">az aks: Überprüfen, ob das Netzwerk-Plug-In entweder „azure“ oder „kubenet“ ist</span><span class="sxs-lookup"><span data-stu-id="fc109-201">az aks: Validate network plugin to be either "azure" or "kubenet"</span></span>
* <span data-ttu-id="fc109-202">az aks: Unterstützung für AAD-Sitzungsschlüssel hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-202">az aks: Add aad session key support</span></span>
* <span data-ttu-id="fc109-203">[BREAKING CHANGE] az aks: Unterstützung von MSI-Änderungen für GF und BF für omsagent (Containerüberwachung)(#1)</span><span class="sxs-lookup"><span data-stu-id="fc109-203">[BREAKING CHANGE] az aks: support msi changes for GF and BF for omsagent (Container monitoring)(#1)</span></span>
* <span data-ttu-id="fc109-204">az aks use-dev-spaces: Endpunkt-Typoption zum Befehl „use-dev-spaces“, hinzugefügt, um den auf einem Azure Dev Spaces-Controller erstellten Endpunkt anzupassen</span><span class="sxs-lookup"><span data-stu-id="fc109-204">az aks use-dev-spaces: Adding endpoint type option to the use-dev-spaces command to customize the endpoint created on an Azure Dev Spaces controller</span></span>

### <a name="appconfig"></a><span data-ttu-id="fc109-205">AppConfig</span><span class="sxs-lookup"><span data-stu-id="fc109-205">AppConfig</span></span>

* <span data-ttu-id="fc109-206">Verwendung von „kv set“ entsperrt, um Schlüsseltresorverweis und -funktion hinzuzufügen …</span><span class="sxs-lookup"><span data-stu-id="fc109-206">Unblock using "kv set" to add keyvault reference and feature …</span></span>

### <a name="appservice"></a><span data-ttu-id="fc109-207">AppService</span><span class="sxs-lookup"><span data-stu-id="fc109-207">AppService</span></span>

* <span data-ttu-id="fc109-208">az webapp create : Beheben eines Problems beim Ausführen des Befehls mit „--runtime“</span><span class="sxs-lookup"><span data-stu-id="fc109-208">az webapp create : Fix issue when running the command with --runtime</span></span>
* <span data-ttu-id="fc109-209">az functionapp deployment source config-zip: Fehlermeldung hinzugefügt, wenn der Ressourcengruppen- oder Funktionsname ungültig oder nicht vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="fc109-209">az functionapp deployment source config-zip: Add an error message if resource group or function name are invalid/don't exist</span></span>
* <span data-ttu-id="fc109-210">functionapp create: Warnmeldung korrigiert, die derzeit mit `functionapp create` angezeigt wird und ein `--functions_version`-Flag angibt, aber irrtümlich ein `_` anstelle eines `-` im Flagnamen verwendet</span><span class="sxs-lookup"><span data-stu-id="fc109-210">functionapp create: Fix the warning message that appears with `functionapp create` today which cites a `--functions_version` flag but erroneously uses a `_` instead of a `-` in the flag name</span></span>
* <span data-ttu-id="fc109-211">az functionapp create: Es wurde aktualisiert, wie linuxFxVersion und der Containerimagename für Linux-Funktions-Apps festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="fc109-211">az functionapp create: Updated the way linuxFxVersion and container image name were being set for linux function apps</span></span>
* <span data-ttu-id="fc109-212">az functionapp deployment source config-zip: Problems behoben, das durch die Racebedingung für die Änderung von App-Einstellungen während der ZIP-Bereitstellung verursacht wird und während der Bereitstellung 5xx-Fehler ausgibt</span><span class="sxs-lookup"><span data-stu-id="fc109-212">az functionapp deployment source config-zip: Fix an issue caused by app settings change racing condition during zip deploy, giving 5xx errors during deployment</span></span>
* <span data-ttu-id="fc109-213">Fix #5720946: „az webapp backup“ legt Namen nicht fest</span><span class="sxs-lookup"><span data-stu-id="fc109-213">Fix #5720946: az webapp backup fails to set name</span></span>

### <a name="arm"></a><span data-ttu-id="fc109-214">ARM</span><span class="sxs-lookup"><span data-stu-id="fc109-214">ARM</span></span>

* <span data-ttu-id="fc109-215">az resource: Beispiele für das Ressourcenmodul verbessert</span><span class="sxs-lookup"><span data-stu-id="fc109-215">az resource: Improve the examples of the resource module</span></span>
* <span data-ttu-id="fc109-216">az policy assignment list: Unterstützung für das Auflisten von Richtlinienzuweisungen im Verwaltungsgruppenbereich</span><span class="sxs-lookup"><span data-stu-id="fc109-216">az policy assignment list: Support listing policy assignments at Management Group scope</span></span>
* <span data-ttu-id="fc109-217">`az deployment group` und `az deployment operation group` für Vorlagenbereitstellung in Ressourcengruppen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-217">Add `az deployment group` and `az deployment operation group` for template deployment at resource groups.</span></span> <span data-ttu-id="fc109-218">Dies ist ein Duplikat von `az group deployment` und `az group deployment operation`.</span><span class="sxs-lookup"><span data-stu-id="fc109-218">This is a duplicate of `az group deployment` and `az group deployment operation`</span></span>
* <span data-ttu-id="fc109-219">`az deployment sub` und `az deployment operation sub` für Vorlagenbereitstellung im Abonnementbereich hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-219">Add `az deployment sub` and `az deployment operation sub` for template deployment at subscription scope.</span></span> <span data-ttu-id="fc109-220">Dies ist ein Duplikat von `az deployment` und `az deployment operation`.</span><span class="sxs-lookup"><span data-stu-id="fc109-220">This is a duplicate of `az deployment` and `az deployment operation`</span></span>
* <span data-ttu-id="fc109-221">`az deployment mg` und `az deployment operation mg` für Vorlagenbereitstellung in Verwaltungsgruppen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-221">Add `az deployment mg` and `az deployment operation mg` for template deployment at management groups</span></span>
* <span data-ttu-id="fc109-222">`az deployment tenant` und `az deployment operation tenant` für Vorlagenbereitstellung im Mandantenbereich hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-222">Add `az deployment tenant` and `az deployment operation tenant` for template deployment at tenant scope</span></span>
* <span data-ttu-id="fc109-223">az policy assignment create: Beschreibung zu Parameter `--location` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-223">az policy assignment create: Add a description to the `--location` parameter</span></span>
* <span data-ttu-id="fc109-224">az group deployment create: Parameter `--aux-tenants` zur mandantenübergreifenden Unterstützung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-224">az group deployment create: Add parameter `--aux-tenants` to support cross tenants</span></span>

### <a name="cdn"></a><span data-ttu-id="fc109-225">CDN</span><span class="sxs-lookup"><span data-stu-id="fc109-225">CDN</span></span>

* <span data-ttu-id="fc109-226">CDN-WAF-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-226">Add CDN WAF commands</span></span>

### <a name="compute"></a><span data-ttu-id="fc109-227">Compute</span><span class="sxs-lookup"><span data-stu-id="fc109-227">Compute</span></span>

* <span data-ttu-id="fc109-228">az sig image-version: „--data-snapshot-luns“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-228">az sig image-version: add --data-snapshot-luns</span></span>
* <span data-ttu-id="fc109-229">az ppg show: „--colocation-status“ hinzugefügt, um das Abrufen des Zusammenstellungsstatus aller Ressourcen in der Näherungsplatzierungsgruppe zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="fc109-229">az ppg show: add --colocation-status to enable fetching the colocation status of all the resources in the proximity placement group</span></span>
* <span data-ttu-id="fc109-230">az vmss create/update: Unterstützung automatischer Reparaturen</span><span class="sxs-lookup"><span data-stu-id="fc109-230">az vmss create/update: support automatic repairs</span></span>
* <span data-ttu-id="fc109-231">[BREAKING CHANGE] az image template: „template“ in „builder“ umbenannt</span><span class="sxs-lookup"><span data-stu-id="fc109-231">[BREAKING CHANGE] az image template: rename template to builder</span></span>
* <span data-ttu-id="fc109-232">az image builder create: „--image-template“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-232">az image builder create: add --image-template</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="fc109-233">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="fc109-233">Cosmos DB</span></span>

* <span data-ttu-id="fc109-234">Gespeicherte Prozedur „Add Sql“, udf- und trigger-Cmdlets hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-234">Add Sql stored procedure, udf and trigger cmdlets</span></span>
* <span data-ttu-id="fc109-235">az cosmosdb create: „--key-uri“ hinzugefügt, um das Hinzufügen von Schlüsseltresor-Verschlüsselungsinformationen zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="fc109-235">az cosmosdb create: add --key-uri to support adding key vault encryption information</span></span>

### <a name="keyvault"></a><span data-ttu-id="fc109-236">KeyVault</span><span class="sxs-lookup"><span data-stu-id="fc109-236">KeyVault</span></span>

* <span data-ttu-id="fc109-237">keyvault create: „soft-delete“ standardmäßig aktiviert</span><span class="sxs-lookup"><span data-stu-id="fc109-237">keyvault create: enable soft-delete by default</span></span>

### <a name="monitor"></a><span data-ttu-id="fc109-238">Überwachen</span><span class="sxs-lookup"><span data-stu-id="fc109-238">Monitor</span></span>

* <span data-ttu-id="fc109-239">az monitor metrics alert create: Unterstützung von `~` in `--condition`</span><span class="sxs-lookup"><span data-stu-id="fc109-239">az monitor metrics alert create: support `~` in `--condition`</span></span>

### <a name="network"></a><span data-ttu-id="fc109-240">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="fc109-240">Network</span></span>

* <span data-ttu-id="fc109-241">az network application-gateway rewrite-rule create: Unterstützung der URL-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="fc109-241">az network application-gateway rewrite-rule create: support url configuration</span></span>
* <span data-ttu-id="fc109-242">az network dns zone import: Bei „--zone-name“ wird die Groß-/Kleinschreibung künftig nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="fc109-242">az network dns zone import: --zone-name will be case insensitive in the future</span></span>
* <span data-ttu-id="fc109-243">az network private-endpoint/private-link-service: Vorschaubezeichnung entfernt</span><span class="sxs-lookup"><span data-stu-id="fc109-243">az network private-endpoint/private-link-service: remove preview label</span></span>
* <span data-ttu-id="fc109-244">az network bastion: Unterstützung von „bastion“</span><span class="sxs-lookup"><span data-stu-id="fc109-244">az network bastion: support bastion</span></span>
* <span data-ttu-id="fc109-245">az network vnet list-available-ips: Unterstützung für das Auflisten verfügbarer IPs in einem VNET</span><span class="sxs-lookup"><span data-stu-id="fc109-245">az network vnet list-available-ips: support list available ips in a vnet</span></span>
* <span data-ttu-id="fc109-246">az network watcher flow-log create/list/delete/update: neue Befehle hinzugefügt, um Watcher-Datenflussprotokolle zu verwalten und „--location“ zur expliziten Identifizierung von Watcher verfügbar zu machen</span><span class="sxs-lookup"><span data-stu-id="fc109-246">az network watcher flow-log create/list/delete/update: add new commands to manage watcher flow log and exposing --location to identify watcher explicitly</span></span>
* <span data-ttu-id="fc109-247">az network watcher flow-log configure: veraltet</span><span class="sxs-lookup"><span data-stu-id="fc109-247">az network watcher flow-log configure: deprecated</span></span>
* <span data-ttu-id="fc109-248">az network watcher flow-log show: Unterstützung von „--location“ und „--name“, um ein ARM-formatiertes Ergebnis zu erhalten; alte formatierte Ausgabe als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="fc109-248">az network watcher flow-log show: support --location and --name to get ARM-formatted result, deprecated old formatted output</span></span>

### <a name="policy"></a><span data-ttu-id="fc109-249">Richtlinie</span><span class="sxs-lookup"><span data-stu-id="fc109-249">Policy</span></span>

* <span data-ttu-id="fc109-250">az policy assignment create: Fehler behoben, dass automatisch generierter Name der Richtlinienzuweisung den Grenzwert überschreitet</span><span class="sxs-lookup"><span data-stu-id="fc109-250">az policy assignment create: Fix the bug that automatically generated name of policy assignment exceeds the limit</span></span>

### <a name="rbac"></a><span data-ttu-id="fc109-251">RBAC</span><span class="sxs-lookup"><span data-stu-id="fc109-251">RBAC</span></span>

* <span data-ttu-id="fc109-252">az ad group show: Problem behoben, dass „--group“-Wert als regulärer Ausdruck behandelt wurde</span><span class="sxs-lookup"><span data-stu-id="fc109-252">az ad group show: fix --group value treated as regex problem</span></span>

### <a name="rdbms"></a><span data-ttu-id="fc109-253">RDBMS</span><span class="sxs-lookup"><span data-stu-id="fc109-253">RDBMS</span></span>

* <span data-ttu-id="fc109-254">SDK-Version von „azure-mgmt-rdbms“ auf 2.0.0 festgelegt</span><span class="sxs-lookup"><span data-stu-id="fc109-254">Bump the azure-mgmt-rdbms SDK version to 2.0.0</span></span>
* <span data-ttu-id="fc109-255">az postgres private-endpoint-connection: Verwalten von Verbindungen mit privatem Postgres-Endpunkt</span><span class="sxs-lookup"><span data-stu-id="fc109-255">az postgres private-endpoint-connection: manage postgres private endpoint connections</span></span>
* <span data-ttu-id="fc109-256">az postgres private-link-resource: Verwalten von privaten Postgres-Linkressourcen</span><span class="sxs-lookup"><span data-stu-id="fc109-256">az postgres private-link-resource: manage postgres private link resources</span></span>
* <span data-ttu-id="fc109-257">az mysql private-endpoint-connection: Verwalten von Verbindungen mit privatem MySQL-Endpunkt</span><span class="sxs-lookup"><span data-stu-id="fc109-257">az mysql private-endpoint-connection: manage mysql private endpoint connections</span></span>
* <span data-ttu-id="fc109-258">az mysql private-link-resource: Verwalten von privaten MySQL-Linkressourcen</span><span class="sxs-lookup"><span data-stu-id="fc109-258">az mysql private-link-resource: manage mysql private link resources</span></span>
* <span data-ttu-id="fc109-259">az mariadb private-endpoint-connection: Verwalten von Verbindungen mit privatem MariaDB-Endpunkt</span><span class="sxs-lookup"><span data-stu-id="fc109-259">az mariadb private-endpoint-connection: manage mariadb private endpoint connections</span></span>
* <span data-ttu-id="fc109-260">az mariadb private-link-resource: Verwalten von privaten MariaDB-Linkressourcen</span><span class="sxs-lookup"><span data-stu-id="fc109-260">az mariadb private-link-resource: manage mariadb private link resources</span></span>
* <span data-ttu-id="fc109-261">Aktualisieren von Tests von privaten RDBMS-Endpunkten</span><span class="sxs-lookup"><span data-stu-id="fc109-261">Updating RDBMS Private Endpoint Tests</span></span>

### <a name="sql"></a><span data-ttu-id="fc109-262">SQL</span><span class="sxs-lookup"><span data-stu-id="fc109-262">SQL</span></span>

* <span data-ttu-id="fc109-263">Sql midb: list-deleted, show-deleted, update-retention, show-retention hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-263">Sql midb Add: list-deleted, show-deleted, update-retention, show-retention</span></span>
* <span data-ttu-id="fc109-264">(sql server create:) Optionales Flag „Enable“/„Disable“ für public-network-access zu „sql server create“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-264">(sql server create:) Add optional public-network-access 'Enable'/'Disable' flag to sql server create</span></span>
* <span data-ttu-id="fc109-265">(sql server update): kundenorientierte Änderung vorgenommen</span><span class="sxs-lookup"><span data-stu-id="fc109-265">(sql server update:) make some customer-facing change</span></span>
* <span data-ttu-id="fc109-266">Eigenschaft „minimal_tls_version“ für MI und SQL-Datenbank hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-266">Add minimal_tls_version property for MI and SQL DB</span></span>

### <a name="storage"></a><span data-ttu-id="fc109-267">Storage</span><span class="sxs-lookup"><span data-stu-id="fc109-267">Storage</span></span>

* <span data-ttu-id="fc109-268">az storage blob delete-batch: Flag `--dryrun` mit Fehlverhalten</span><span class="sxs-lookup"><span data-stu-id="fc109-268">az storage blob delete-batch: Misbehaving `--dryrun` flag</span></span>
* <span data-ttu-id="fc109-269">az storage account network-rule hinzugefügt (Fehlerbehebung): Hinzufügen von Vorgängen muss idempotent sein</span><span class="sxs-lookup"><span data-stu-id="fc109-269">az storage account network-rule add (bug fix): add operation should be idempotent</span></span>
* <span data-ttu-id="fc109-270">az storage account create/update: Unterstützung für Routingpräferenz hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-270">az storage account create/update: Add Routing Preference support</span></span>
* <span data-ttu-id="fc109-271">„azure-mgmt-storage“ auf Version 8.0.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="fc109-271">Upgrade azure-mgmt-storage version to 8.0.0</span></span>
* <span data-ttu-id="fc109-272">az storage container immutability create: Parameter „--allow-protected-append-write“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-272">az storage container immutability create: add --allow-protected-append-write parameter</span></span>
* <span data-ttu-id="fc109-273">az storage account private-link-resource list: Unterstützung zum Auflisten privater Linkressourcen für Speicherkonto hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-273">az storage account private-link-resource list: Add support to list private link resources for storage account</span></span>
* <span data-ttu-id="fc109-274">az storage account private-endpoint-connection approve/reject/show/delete: Unterstützung der Verwaltung von Verbindungen mit privaten Endpunkten</span><span class="sxs-lookup"><span data-stu-id="fc109-274">az storage account private-endpoint-connection approve/reject/show/delete: Support to manage private endpoint connections</span></span>
* <span data-ttu-id="fc109-275">az storage account blob-service-properties update: „--enable-restore-policy“ und „--restore-days“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-275">az storage account blob-service-properties update: add --enable-restore-policy and --restore-days</span></span>
* <span data-ttu-id="fc109-276">az storage blob restore: Unterstützung für die Wiederherstellung von Blobbereichen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-276">az storage blob restore: Add support to restore blob ranges</span></span>

## <a name="february-18-2020"></a><span data-ttu-id="fc109-277">18. Februar 2020</span><span class="sxs-lookup"><span data-stu-id="fc109-277">February 18, 2020</span></span>

<span data-ttu-id="fc109-278">Version 2.1.0</span><span class="sxs-lookup"><span data-stu-id="fc109-278">Version 2.1.0</span></span>

### <a name="acr"></a><span data-ttu-id="fc109-279">ACR</span><span class="sxs-lookup"><span data-stu-id="fc109-279">ACR</span></span>

* <span data-ttu-id="fc109-280">Neues Argument `--expose-token` für `az acr login` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-280">Add a new argument `--expose-token` for `az acr login`</span></span>
* <span data-ttu-id="fc109-281">Falsche Ausgabe für `az acr task identity show -n Name -r Registry -o table` korrigiert</span><span class="sxs-lookup"><span data-stu-id="fc109-281">Fix the incorrect output of `az acr task identity show -n Name -r Registry -o table`</span></span>
* <span data-ttu-id="fc109-282">az acr login: Auslösen von „CLIError“, wenn vom Docker-Befehl Fehler zurückgegeben werden</span><span class="sxs-lookup"><span data-stu-id="fc109-282">az acr login: Throw a CLIError if there are errors returned by docker command</span></span>

### <a name="acs"></a><span data-ttu-id="fc109-283">ACS</span><span class="sxs-lookup"><span data-stu-id="fc109-283">ACS</span></span>

* <span data-ttu-id="fc109-284">aks create/update: Validierung für `--vnet-subnet-id` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-284">aks create/update: add `--vnet-subnet-id` validation</span></span>

### <a name="aladdin"></a><span data-ttu-id="fc109-285">Aladdin</span><span class="sxs-lookup"><span data-stu-id="fc109-285">Aladdin</span></span>

* <span data-ttu-id="fc109-286">Analysieren der generierten Beispiele in „_help.py“ der Befehle</span><span class="sxs-lookup"><span data-stu-id="fc109-286">Parse generated examples into commands' _help.py</span></span>

### <a name="ams"></a><span data-ttu-id="fc109-287">AMS</span><span class="sxs-lookup"><span data-stu-id="fc109-287">AMS</span></span>

* <span data-ttu-id="fc109-288">az ams ist jetzt allgemein verfügbar.</span><span class="sxs-lookup"><span data-stu-id="fc109-288">az ams is GA now</span></span>

### <a name="appconfig"></a><span data-ttu-id="fc109-289">AppConfig</span><span class="sxs-lookup"><span data-stu-id="fc109-289">AppConfig</span></span>

* <span data-ttu-id="fc109-290">Hilfenachricht überarbeitet, um nicht unterstützte Schlüssel-/Bezeichnungsfilter auszuschließen</span><span class="sxs-lookup"><span data-stu-id="fc109-290">Revise help message to exclude unsupported key/label filter</span></span>
* <span data-ttu-id="fc109-291">Vorschautag für die meisten Befehle entfernt (mit Ausnahme der Flags für verwaltete Identitäten und Features)</span><span class="sxs-lookup"><span data-stu-id="fc109-291">Remove preview tag for most commands excluding managed identity and feature flags</span></span>
* <span data-ttu-id="fc109-292">Kundenseitig verwalteter Schlüssel beim Aktualisieren der Speicher hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-292">Add customer managed key when updating stores</span></span>

### <a name="appservice"></a><span data-ttu-id="fc109-293">AppService</span><span class="sxs-lookup"><span data-stu-id="fc109-293">AppService</span></span>

* <span data-ttu-id="fc109-294">az webapp list-runtimes: Fehler bei „list-runtimes“ behoben</span><span class="sxs-lookup"><span data-stu-id="fc109-294">az webapp list-runtimes: Fix the bug for list-runtimes</span></span>
* <span data-ttu-id="fc109-295">„az webapp|functionapp config ssl create“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-295">Add az webapp|functionapp config ssl create</span></span>
* <span data-ttu-id="fc109-296">Unterstützung für v3-Funktions-Apps und Node 12</span><span class="sxs-lookup"><span data-stu-id="fc109-296">Add support for v3 function apps and node 12</span></span>

### <a name="arm"></a><span data-ttu-id="fc109-297">ARM</span><span class="sxs-lookup"><span data-stu-id="fc109-297">ARM</span></span>

* <span data-ttu-id="fc109-298">az policy assignment create: Fehlermeldung korrigiert, die angezeigt wird, wenn der Parameter `--policy` ungültig ist</span><span class="sxs-lookup"><span data-stu-id="fc109-298">az policy assignment create: Fix the error message when the `--policy` parameter is invalid</span></span>
* <span data-ttu-id="fc109-299">az group deployment create: Fehler „stat: path too long for Windows" korrigiert, der angezeigt wird, wenn eine zu große Datei vom Typ „parameters.json“ verwendet wird</span><span class="sxs-lookup"><span data-stu-id="fc109-299">az group deployment create: Fix "stat: path too long for Windows" error when using large parameters.json file</span></span>

### <a name="backup"></a><span data-ttu-id="fc109-300">Backup</span><span class="sxs-lookup"><span data-stu-id="fc109-300">Backup</span></span>

* <span data-ttu-id="fc109-301">Korrektur des Wiederherstellungsflows auf Elementebene am ursprünglichen Speicherort</span><span class="sxs-lookup"><span data-stu-id="fc109-301">Fix for item level recovery flow in OLR</span></span>
* <span data-ttu-id="fc109-302">Unterstützung von „Als Dateien wiederherstellen“ für SQL- und SAP-Datenbanken hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-302">Add restore as files support for SQL and SAP Databases</span></span>

### <a name="compute"></a><span data-ttu-id="fc109-303">Compute</span><span class="sxs-lookup"><span data-stu-id="fc109-303">Compute</span></span>

* <span data-ttu-id="fc109-304">vm/vmss/availability-set update: „--ppg“ hinzugefügt, um die Aktualisierung von „ProximityPlacementGroup“ zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="fc109-304">vm/vmss/availability-set update: add --ppg to allowing updating ProximityPlacementGroup</span></span>
* <span data-ttu-id="fc109-305">vmss create: „--data-disk-iops“ und „--data-disk-mbps“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-305">vmss create: add --data-disk-iops and --data-disk-mbps</span></span>
* <span data-ttu-id="fc109-306">az vm host: Vorschautag für `vm host` und `vm host group` entfernt</span><span class="sxs-lookup"><span data-stu-id="fc109-306">az vm host: remove preview tag for `vm host` and `vm host group`</span></span>
* <span data-ttu-id="fc109-307">[BREAKING CHANGE] Behebung Nr. 10728: `az vm create`: Automatisches Erstellen des Subnetzes, wenn das VNET angegeben wird und das Subnetz nicht vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="fc109-307">[BREAKING CHANGE] Fix #10728: `az vm create`: create subnet automatically if vnet is specified and subnet not exists</span></span>
* <span data-ttu-id="fc109-308">Erhöhen der Stabilität von „vm image list“</span><span class="sxs-lookup"><span data-stu-id="fc109-308">Increase robustness of vm image list</span></span>

### <a name="eventhub"></a><span data-ttu-id="fc109-309">Eventhub</span><span class="sxs-lookup"><span data-stu-id="fc109-309">Eventhub</span></span>

* <span data-ttu-id="fc109-310">Azure Stack-Unterstützung für Profil „2019-03-01-hybrid“</span><span class="sxs-lookup"><span data-stu-id="fc109-310">Azure Stack support for 2019-03-01-hybrid profile</span></span>

### <a name="keyvault"></a><span data-ttu-id="fc109-311">KeyVault</span><span class="sxs-lookup"><span data-stu-id="fc109-311">KeyVault</span></span>

* <span data-ttu-id="fc109-312">az keyvault key create: neuer Wert `import` für Parameter `--ops` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-312">az keyvault key create: add a new value `import` for parameter `--ops`</span></span>
* <span data-ttu-id="fc109-313">az keyvault key list-versions: Unterstützung des Parameters `--id` für die Angabe von Schlüsseln</span><span class="sxs-lookup"><span data-stu-id="fc109-313">az keyvault key list-versions: support parameter `--id` for specifying keys</span></span>
* <span data-ttu-id="fc109-314">Unterstützung für Verbindungen mit privaten Endpunkten</span><span class="sxs-lookup"><span data-stu-id="fc109-314">Support private endpoint connections</span></span>

### <a name="network"></a><span data-ttu-id="fc109-315">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="fc109-315">Network</span></span>

* <span data-ttu-id="fc109-316">Geändert in „azure-mgmt-network 9.0.0“</span><span class="sxs-lookup"><span data-stu-id="fc109-316">Bump to azure-mgmt-network 9.0.0</span></span>
* <span data-ttu-id="fc109-317">az network private-link-service update/create: Unterstützung von „--enable-proxy-protocol“</span><span class="sxs-lookup"><span data-stu-id="fc109-317">az network private-link-service update/create: support --enable-proxy-protocol</span></span>
* <span data-ttu-id="fc109-318">Feature für Version 2 von Verbindungsmonitor hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-318">Add connection Monitor V2 feature</span></span>

### <a name="packaging"></a><span data-ttu-id="fc109-319">Verpackung</span><span class="sxs-lookup"><span data-stu-id="fc109-319">Packaging</span></span>

* <span data-ttu-id="fc109-320">[BREAKING CHANGE] Unterstützung für Python 2.7 eingestellt</span><span class="sxs-lookup"><span data-stu-id="fc109-320">[BREAKING CHANGE] Drop support for Python 2.7</span></span>

### <a name="profile"></a><span data-ttu-id="fc109-321">Profil</span><span class="sxs-lookup"><span data-stu-id="fc109-321">Profile</span></span>

* <span data-ttu-id="fc109-322">Vorschau: Neue Attribute `homeTenantId` und `managedByTenants` zu Abonnementkonten hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-322">Preview: Add new attributes `homeTenantId` and `managedByTenants` to subscription accounts.</span></span> <span data-ttu-id="fc109-323">Führen Sie `az login` erneut aus, damit die Änderungen wirksam werden.</span><span class="sxs-lookup"><span data-stu-id="fc109-323">Please re-run `az login` for the changes to take effect</span></span>
* <span data-ttu-id="fc109-324">az login: Eine Warnung wird angezeigt, wenn ein Abonnement von mehren Mandanten aufgeführt wird und der erste als Standard festgelegt wird.</span><span class="sxs-lookup"><span data-stu-id="fc109-324">az login: Show a warning when a subscription is listed from more than one tenants and default to the first one.</span></span> <span data-ttu-id="fc109-325">Fügen Sie `--tenant` in `az login` ein, um beim Zugreifen auf dieses Abonnement einen bestimmten Mandanten auszuwählen.</span><span class="sxs-lookup"><span data-stu-id="fc109-325">To select a specific tenant when accessing this subscription, please include `--tenant` in `az login`</span></span>

### <a name="role"></a><span data-ttu-id="fc109-326">Role</span><span class="sxs-lookup"><span data-stu-id="fc109-326">Role</span></span>

* <span data-ttu-id="fc109-327">az role assignment create: Problem behoben, das beim Zuweisen einer Rolle zu einem Dienstprinzipal nach Anzeigename einen Fehler vom Typ „HTTP 400“ verursachte</span><span class="sxs-lookup"><span data-stu-id="fc109-327">az role assignment create: Fix the error that assigning a role to a service principal by display name yields a HTTP 400</span></span>

### <a name="sql"></a><span data-ttu-id="fc109-328">SQL</span><span class="sxs-lookup"><span data-stu-id="fc109-328">SQL</span></span>

* <span data-ttu-id="fc109-329">Cmdlet `az sql mi update` der verwalteten SQL-Instanz mit zwei neuen Parametern aktualisiert: tier und family</span><span class="sxs-lookup"><span data-stu-id="fc109-329">Update SQL Managed Instance cmdlet `az sql mi update` with two new parameters: tier and family</span></span>

### <a name="storage"></a><span data-ttu-id="fc109-330">Storage</span><span class="sxs-lookup"><span data-stu-id="fc109-330">Storage</span></span>

* <span data-ttu-id="fc109-331">[BREAKING CHANGE] `az storage account create`: Art des Standardspeicherkontos in StorageV2 geändert</span><span class="sxs-lookup"><span data-stu-id="fc109-331">[BREAKING CHANGE] `az storage account create`: Change default storage account kind to StorageV2</span></span>

## <a name="february-04-2020"></a><span data-ttu-id="fc109-332">04. Februar 2020</span><span class="sxs-lookup"><span data-stu-id="fc109-332">February 04, 2020</span></span>

<span data-ttu-id="fc109-333">Version 2.0.81</span><span class="sxs-lookup"><span data-stu-id="fc109-333">Version 2.0.81</span></span>

### <a name="acs"></a><span data-ttu-id="fc109-334">ACS</span><span class="sxs-lookup"><span data-stu-id="fc109-334">ACS</span></span>

* <span data-ttu-id="fc109-335">Unterstützung für das Festlegen zugeordneter Ausgangsports und Leerlauftimeouts für Load Balancer Standard hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-335">Add support to set outbound allocated ports and idle timeouts on standard load balancer</span></span>
* <span data-ttu-id="fc109-336">Aktualisierung auf API-Version 2019-11-01</span><span class="sxs-lookup"><span data-stu-id="fc109-336">Update to API Version 2019-11-01</span></span>

### <a name="acr"></a><span data-ttu-id="fc109-337">ACR</span><span class="sxs-lookup"><span data-stu-id="fc109-337">ACR</span></span>

* <span data-ttu-id="fc109-338">[BREAKING CHANGE] `az acr delete` löst eine Eingabeaufforderung aus.</span><span class="sxs-lookup"><span data-stu-id="fc109-338">[BREAKING CHANGE] `az acr delete` will prompt</span></span>
* <span data-ttu-id="fc109-339">[BREAKING CHANGE] „az acr task delete“ löst eine Eingabeaufforderung aus.</span><span class="sxs-lookup"><span data-stu-id="fc109-339">[BREAKING CHANGE] 'az acr task delete' will prompt</span></span>
* <span data-ttu-id="fc109-340">Neue Befehlsgruppe „az acr taskrun show/list/delete“ für die Aufgabenausführungsverwaltung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-340">Add a new command group 'az acr taskrun show/list/delete' for taskrun management</span></span>

### <a name="aks"></a><span data-ttu-id="fc109-341">AKS</span><span class="sxs-lookup"><span data-stu-id="fc109-341">AKS</span></span>

* <span data-ttu-id="fc109-342">Jeder Cluster erhält einen separaten Dienstprinzipal zur Verbesserung der Isolation.</span><span class="sxs-lookup"><span data-stu-id="fc109-342">Each cluster gets a separate service principal to improve isolation</span></span>

### <a name="appconfig"></a><span data-ttu-id="fc109-343">AppConfig</span><span class="sxs-lookup"><span data-stu-id="fc109-343">AppConfig</span></span>

* <span data-ttu-id="fc109-344">Unterstützung für den Import/Export von KeyVault-Verweisen in/aus AppService</span><span class="sxs-lookup"><span data-stu-id="fc109-344">Support import/export of keyvault references from/to appservice</span></span>
* <span data-ttu-id="fc109-345">Unterstützung für den Import/Export aller Bezeichnungen in appconfig und aus appconfig</span><span class="sxs-lookup"><span data-stu-id="fc109-345">Support import/export of all labels from appconfig to appconfig</span></span>
* <span data-ttu-id="fc109-346">Überprüfen der Schlüssel- und Featurenamen vor dem Festlegen und Importieren</span><span class="sxs-lookup"><span data-stu-id="fc109-346">Validate key and feature names before setting and importing</span></span>
* <span data-ttu-id="fc109-347">Verfügbarmachen der SKU-Änderung für den Konfigurationsspeicher</span><span class="sxs-lookup"><span data-stu-id="fc109-347">Expose sku modification for configuration store.</span></span>
* <span data-ttu-id="fc109-348">Befehlsgruppe für die verwaltete Identität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-348">Add command group for managed identity.</span></span>

### <a name="appservice"></a><span data-ttu-id="fc109-349">AppService</span><span class="sxs-lookup"><span data-stu-id="fc109-349">AppService</span></span>

* <span data-ttu-id="fc109-350">Azure Stack: Oberflächenbefehle im Profil „2019-03-01-hybrid“</span><span class="sxs-lookup"><span data-stu-id="fc109-350">Azure Stack: surface commands under the profile of 2019-03-01-hybrid</span></span>
* <span data-ttu-id="fc109-351">functionapp: Funktion zum Erstellen von Java-Funktions-Apps in Linux hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-351">functionapp: Add ability to create Java function apps in Linux</span></span>

### <a name="arm"></a><span data-ttu-id="fc109-352">ARM</span><span class="sxs-lookup"><span data-stu-id="fc109-352">ARM</span></span>

* <span data-ttu-id="fc109-353">Behebung von Problem Nr. 10246: `az resource tag` stürzt ab, wenn der übergebene Parameter `--ids` der Ressourcengruppen-ID entspricht.</span><span class="sxs-lookup"><span data-stu-id="fc109-353">Fix issue #10246: `az resource tag` crashes when the parameter `--ids` passed in is resource group ID</span></span>
* <span data-ttu-id="fc109-354">Behebung von Problem Nr. 11658: Der Befehl `az group export` unterstützt die Parameter `--query` und `--output` nicht.</span><span class="sxs-lookup"><span data-stu-id="fc109-354">Fix issue #11658: `az group export` command does not support `--query` and `--output` parameters</span></span>
* <span data-ttu-id="fc109-355">Behebung von Problem Nr. 10279: Der Exitcode von `az group deployment validate` ist 0, wenn bei der Überprüfung ein Fehler auftritt.</span><span class="sxs-lookup"><span data-stu-id="fc109-355">Fix issue #10279: The exit code of `az group deployment validate` is 0 when the verification fails</span></span>
* <span data-ttu-id="fc109-356">Behebung von Problem Nr. 9916: Fehlermeldung des Konflikts zwischen Tag und anderen Filterbedingungen für Befehl `az resource list` verbessert</span><span class="sxs-lookup"><span data-stu-id="fc109-356">Fix issue #9916: Improve the error message of the conflict between tag and other filter conditions for `az resource list` command</span></span>
* <span data-ttu-id="fc109-357">Neuer Parameter `--managed-by` hinzugefügt, um das Hinzufügen der Informationen vom Typ „managedBy“ für Befehl `az group create` zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="fc109-357">Add new parameter `--managed-by` to support adding managedBy information for command `az group create`</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="fc109-358">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="fc109-358">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="fc109-359">Untergruppe `monitor` hinzugefügt, um Log Analytics-Überwachung im Azure Red Hat OpenShift-Cluster zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="fc109-359">Add `monitor` subgroup to manage Log Analytics monitoring in Azure Red Hat OpensShift cluster</span></span>

### <a name="botservice"></a><span data-ttu-id="fc109-360">BotService</span><span class="sxs-lookup"><span data-stu-id="fc109-360">BotService</span></span>

* <span data-ttu-id="fc109-361">Behebung von Problem Nr. 11697: `az bot create` ist nicht idempotent.</span><span class="sxs-lookup"><span data-stu-id="fc109-361">Fix issue #11697: `az bot create` is not idempotent</span></span>
* <span data-ttu-id="fc109-362">Tests zur Namenskorrektur geändert, sodass sie nur im Livemodus ausgeführt werden</span><span class="sxs-lookup"><span data-stu-id="fc109-362">Change name-correcting tests to run in Live-mode only</span></span>

### <a name="cdn"></a><span data-ttu-id="fc109-363">CDN</span><span class="sxs-lookup"><span data-stu-id="fc109-363">CDN</span></span>

* <span data-ttu-id="fc109-364">Unterstützung für das rulesEngine-Feature hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-364">Add support for rulesEngine feature</span></span>
* <span data-ttu-id="fc109-365">Neue Befehlsgruppe „cdn endpoint rule“ zum Verwalten von Regeln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-365">Add new commands group 'cdn endpoint rule' to manage rules</span></span>
* <span data-ttu-id="fc109-366">azure-mgmt-cdn-Version auf 4.0.0 aktualisiert, um API-Version 2019-04-15 zu verwenden</span><span class="sxs-lookup"><span data-stu-id="fc109-366">Update azure-mgmt-cdn version to 4.0.0 to use api version 2019-04-15</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="fc109-367">Bereitstellungs-Manager</span><span class="sxs-lookup"><span data-stu-id="fc109-367">Deployment Manager</span></span>

* <span data-ttu-id="fc109-368">Auflistungsvorgang für alle Ressourcen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-368">Add list operation for all resources.</span></span>
* <span data-ttu-id="fc109-369">Schrittressource für neuen Schritttyp optimiert</span><span class="sxs-lookup"><span data-stu-id="fc109-369">Enhance step resource for new step type.</span></span>
* <span data-ttu-id="fc109-370">Paket „azure-mgmt-deploymentmanager“ zur Verwendung von Version 0.2.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="fc109-370">Update azure-mgmt-deploymentmanager package to use version 0.2.0.</span></span>

### <a name="iot"></a><span data-ttu-id="fc109-371">IoT</span><span class="sxs-lookup"><span data-stu-id="fc109-371">IoT</span></span>

* <span data-ttu-id="fc109-372">Befehle vom Typ „IoT hub Job“ als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="fc109-372">Deprecate 'IoT hub Job' commands.</span></span>

### <a name="iot-central"></a><span data-ttu-id="fc109-373">IoT Central</span><span class="sxs-lookup"><span data-stu-id="fc109-373">IoT Central</span></span>

* <span data-ttu-id="fc109-374">Unterstützung der App-Erstellung/-Aktualisierung mit neuem SKU-Namen ST0, ST1, ST2</span><span class="sxs-lookup"><span data-stu-id="fc109-374">Support app creation/update with the new sku name ST0, ST1, ST2.</span></span>

### <a name="key-vault"></a><span data-ttu-id="fc109-375">Key Vault</span><span class="sxs-lookup"><span data-stu-id="fc109-375">Key Vault</span></span>

* <span data-ttu-id="fc109-376">Neuer Befehl `az keyvault key download` zum Herunterladen von Schlüsseln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-376">Add a new command `az keyvault key download` for downloading keys.</span></span>

### <a name="misc"></a><span data-ttu-id="fc109-377">Sonstiges</span><span class="sxs-lookup"><span data-stu-id="fc109-377">Misc</span></span>

* <span data-ttu-id="fc109-378">Behebung Nr. 6371: Unterstützung für die Vervollständigung von Dateinamen und Umgebungsvariablen in Bash</span><span class="sxs-lookup"><span data-stu-id="fc109-378">Fix #6371: Support filename and environment variable completion in Bash</span></span>

### <a name="network"></a><span data-ttu-id="fc109-379">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="fc109-379">Network</span></span>

* <span data-ttu-id="fc109-380">Behebung Nr. 2092: az network dns record-set add/remove: Warnung hinzugefügt, wenn Datensatzgruppe nicht gefunden wurde.</span><span class="sxs-lookup"><span data-stu-id="fc109-380">Fix #2092: az network dns record-set add/remove: add warning when record-set is not found.</span></span> <span data-ttu-id="fc109-381">In Zukunft wird ein zusätzliches Argument unterstützt, um diese automatische Erstellung zu bestätigen.</span><span class="sxs-lookup"><span data-stu-id="fc109-381">In the future, an extra argument will be supported to confirm this auto creation.</span></span>

### <a name="policy"></a><span data-ttu-id="fc109-382">Richtlinie</span><span class="sxs-lookup"><span data-stu-id="fc109-382">Policy</span></span>

* <span data-ttu-id="fc109-383">Neuer Befehl `az policy metadata` hinzugefügt, um umfangreiche Richtlinienmetadatenressourcen abzurufen</span><span class="sxs-lookup"><span data-stu-id="fc109-383">Add new command `az policy metadata` to retrieve rich policy metadata resources</span></span>
* <span data-ttu-id="fc109-384">`az policy remediation create`: Geben Sie mit dem Parameter `--resource-discovery-mode` an, ob die Konformität vor der Wartung neu bewertet werden soll.</span><span class="sxs-lookup"><span data-stu-id="fc109-384">`az policy remediation create`: Specify whether compliance should be re-evaluated prior to remediation with the `--resource-discovery-mode` parameter</span></span>

### <a name="profile"></a><span data-ttu-id="fc109-385">Profil</span><span class="sxs-lookup"><span data-stu-id="fc109-385">Profile</span></span>

* <span data-ttu-id="fc109-386">`az account get-access-token`: Parameter `--tenant` hinzugefügt, um das Token für den Mandanten direkt abzurufen. Es muss kein Abonnement angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="fc109-386">`az account get-access-token`: Add `--tenant` parameter to acquire token for the tenant directly, needless to specify a subscription</span></span>

### <a name="rbac"></a><span data-ttu-id="fc109-387">RBAC</span><span class="sxs-lookup"><span data-stu-id="fc109-387">RBAC</span></span>

* <span data-ttu-id="fc109-388">[BREAKING CHANGE] Behebung Nr. 11883: `az role assignment create`: Bei leerem Bereich wird ein Fehler ausgegeben.</span><span class="sxs-lookup"><span data-stu-id="fc109-388">[BREAKING CHANGE] Fix #11883: `az role assignment create`: empty scope will prompt error</span></span>

### <a name="security"></a><span data-ttu-id="fc109-389">Sicherheit</span><span class="sxs-lookup"><span data-stu-id="fc109-389">Security</span></span>

* <span data-ttu-id="fc109-390">Neue Befehle `az atp show` und `az atp update` hinzugefügt, um erweiterte Einstellungen für den Bedrohungsschutz für Speicherkonten anzuzeigen und zu verwalten</span><span class="sxs-lookup"><span data-stu-id="fc109-390">Add new commands `az atp show` and `az atp update` to view and manage advanced threat protection settings for storage accounts.</span></span>

### <a name="sql"></a><span data-ttu-id="fc109-391">SQL</span><span class="sxs-lookup"><span data-stu-id="fc109-391">SQL</span></span>

* <span data-ttu-id="fc109-392">`sql dw create`: Parameter `--zone-redundant` und `--read-replica-count` als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="fc109-392">`sql dw create`: deprecate `--zone-redundant` and `--read-replica-count` parameters.</span></span> <span data-ttu-id="fc109-393">Diese Parameter gelten nicht für Datawarehouse.</span><span class="sxs-lookup"><span data-stu-id="fc109-393">These parameters do not apply to DataWarehouse.</span></span>
* <span data-ttu-id="fc109-394">[BREAKING CHANGE] `az sql db create`: „WideWorldImportersStd“ und „WideWorldImportersFull“ als dokumentierte zulässige Werte für „az sql db create --sample-name“ entfernt.</span><span class="sxs-lookup"><span data-stu-id="fc109-394">[BREAKING CHANGE] `az sql db create`: Remove "WideWorldImportersStd" and "WideWorldImportersFull" as documented allowed values for "az sql db create --sample-name".</span></span> <span data-ttu-id="fc109-395">Diese Beispieldatenbanken führen immer zu einem Fehler bei der Erstellung.</span><span class="sxs-lookup"><span data-stu-id="fc109-395">These sample databases would always cause creation to fail.</span></span>
* <span data-ttu-id="fc109-396">Neue Befehle `sql db classification show/list/update/delete` und `sql db classification recommendation list/enable/disable` zur Verwaltung von Vertraulichkeitsklassifizierungen für SQL-Datenbanken hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-396">Add New commands `sql db classification show/list/update/delete` and `sql db classification recommendation list/enable/disable` to manage sensitivity classifications for SQL databases.</span></span>
* <span data-ttu-id="fc109-397">`az sql db audit-policy`: Behebung für leere Überwachungsaktionen und -gruppen</span><span class="sxs-lookup"><span data-stu-id="fc109-397">`az sql db audit-policy`: Fix for empty audit actions and groups</span></span>

### <a name="storage"></a><span data-ttu-id="fc109-398">Storage</span><span class="sxs-lookup"><span data-stu-id="fc109-398">Storage</span></span>

* <span data-ttu-id="fc109-399">Neue Befehlsgruppe `az storage share-rm` hinzugefügt, um den Ressourcenanbieter „Microsoft.Storage“ für Verwaltungsvorgänge der Azure-Dateifreigabe zu verwenden</span><span class="sxs-lookup"><span data-stu-id="fc109-399">Add a new command group `az storage share-rm` to use the Microsoft.Storage resource provider for Azure file share management operations.</span></span>
* <span data-ttu-id="fc109-400">Behebung für Problem Nr. 11415: Berechtigungsfehler für `az storage blob update`</span><span class="sxs-lookup"><span data-stu-id="fc109-400">Fix issue #11415: permission error for `az storage blob update`</span></span>
* <span data-ttu-id="fc109-401">Integration von Azcopy 10.3.3 und Unterstützung von Win32</span><span class="sxs-lookup"><span data-stu-id="fc109-401">Integrate Azcopy 10.3.3 and support Win32.</span></span>
* <span data-ttu-id="fc109-402">`az storage copy`: Parameter `--include-path`, `--include-pattern`, `--exclude-path` und`--exclude-pattern` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-402">`az storage copy`: Add `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="fc109-403">`az storage remove`: Parameter `--inlcude` und `--exclude` in Parameter `--include-path`, `--include-pattern`, `--exclude-path` und`--exclude-pattern` geändert</span><span class="sxs-lookup"><span data-stu-id="fc109-403">`az storage remove`: Change `--inlcude` and `--exclude` parameters to `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="fc109-404">`az storage sync`: Parameter `--include-pattern`, `--exclude-path` und`--exclude-pattern` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-404">`az storage sync`: Add `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>

### <a name="servicefabric"></a><span data-ttu-id="fc109-405">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="fc109-405">ServiceFabric</span></span>

* <span data-ttu-id="fc109-406">Neue Befehle zum Verwalten von Anwendung und Diensten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-406">Add new commands to manage appliaction and services.</span></span>

## <a name="january-13-2020"></a><span data-ttu-id="fc109-407">13. Januar 2020</span><span class="sxs-lookup"><span data-stu-id="fc109-407">January 13, 2020</span></span>

<span data-ttu-id="fc109-408">Version 2.0.80</span><span class="sxs-lookup"><span data-stu-id="fc109-408">Version 2.0.80</span></span>

### <a name="compute"></a><span data-ttu-id="fc109-409">Compute</span><span class="sxs-lookup"><span data-stu-id="fc109-409">Compute</span></span>

* <span data-ttu-id="fc109-410">Datenträgeraktualisierung: „--disk-encryption-set“ und „--encryption-type“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-410">disk update: Add --disk-encryption-set and --encryption-type</span></span>
* <span data-ttu-id="fc109-411">Momentaufnahmeerstellung/-aktualisierung: „--disk-encryption-set“ und „--encryption-type“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-411">snapshot create/update: Add --disk-encryption-set and --encryption-type</span></span>

### <a name="storage"></a><span data-ttu-id="fc109-412">Storage</span><span class="sxs-lookup"><span data-stu-id="fc109-412">Storage</span></span>

* <span data-ttu-id="fc109-413">„azure-mgmt-storage“ auf Version 7.1.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="fc109-413">Upgrade azure-mgmt-storage version to 7.1.0</span></span>
* <span data-ttu-id="fc109-414">`az storage account create`: `--encryption-key-type-for-table` und `--encryption-key-type-for-queue` zur Unterstützung des Tabellen- und Warteschlangenverschlüsselungsdiensts hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-414">`az storage account create`: Add `--encryption-key-type-for-table` and `--encryption-key-type-for-queue` to support Table and Queue Encryption Service</span></span>

## <a name="january-07-2020"></a><span data-ttu-id="fc109-415">7\. Januar 2020</span><span class="sxs-lookup"><span data-stu-id="fc109-415">January 07, 2020</span></span>

<span data-ttu-id="fc109-416">Version 2.0.79</span><span class="sxs-lookup"><span data-stu-id="fc109-416">Version 2.0.79</span></span>

### <a name="acr"></a><span data-ttu-id="fc109-417">ACR</span><span class="sxs-lookup"><span data-stu-id="fc109-417">ACR</span></span>

* <span data-ttu-id="fc109-418">[BREAKING CHANGE] Parameter „--os“ für „acr build“, „acr task create/update“, „acr run“ und „acr pack“ wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="fc109-418">[BREAKING CHANGE] Remove '--os' parameter for 'acr build', 'acr task create/update', 'acr run', and 'acr pack'.</span></span> <span data-ttu-id="fc109-419">Verwenden Sie stattdessen „--platform“.</span><span class="sxs-lookup"><span data-stu-id="fc109-419">Use '--platform' instead.</span></span>

### <a name="appconfig"></a><span data-ttu-id="fc109-420">AppConfig</span><span class="sxs-lookup"><span data-stu-id="fc109-420">AppConfig</span></span>

* <span data-ttu-id="fc109-421">Unterstützung für das Importieren/Exportieren von Featureflags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-421">Add support for importing/exporting feature flags</span></span>
* <span data-ttu-id="fc109-422">Neuer Befehl „az appconfig kv set-keyvault“ für das Erstellen einer KeyVault-Referenz hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-422">Add new command 'az appconfig kv set-keyvault' for creating keyvault reference</span></span>
* <span data-ttu-id="fc109-423">Unterstützung verschiedener Benennungskonventionen beim Exportieren von Featureflags in eine Datei</span><span class="sxs-lookup"><span data-stu-id="fc109-423">Support various naming conventions when exporting feature flags to file</span></span>

### <a name="appservice"></a><span data-ttu-id="fc109-424">AppService</span><span class="sxs-lookup"><span data-stu-id="fc109-424">AppService</span></span>

* <span data-ttu-id="fc109-425">Behebung von Problem Nr. 7154: Aktualisierung der Dokumentation für Befehl „<>“, sodass Backticks anstelle von einfachen Anführungszeichen verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="fc109-425">Fix issue #7154: Updating documentation for command <> to use back ticks instead of single quotes</span></span>
* <span data-ttu-id="fc109-426">Behebung von Problem Nr. 11287: „webapp up“: Für die mit „up“ erstellte App muss standardmäßig SSL aktiviert sein.</span><span class="sxs-lookup"><span data-stu-id="fc109-426">Fix issue #11287: webapp up: By default make the app created using up 'should be 'SSL enabled'</span></span>
* <span data-ttu-id="fc109-427">Behebung von Problem Nr. 11592: Flag „az webapp up“ für statische HTML-Websites hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-427">Fix issue #11592: Add az webapp up flag for html static sites</span></span>

### <a name="arm"></a><span data-ttu-id="fc109-428">ARM</span><span class="sxs-lookup"><span data-stu-id="fc109-428">ARM</span></span>

* <span data-ttu-id="fc109-429">Behebung `az resource tag`: Recovery Services-Tresor-Tags können nicht aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="fc109-429">Fix `az resource tag`: Recovery Services Vault tags cannot be updated</span></span>

### <a name="backup"></a><span data-ttu-id="fc109-430">Backup</span><span class="sxs-lookup"><span data-stu-id="fc109-430">Backup</span></span>

* <span data-ttu-id="fc109-431">Neuer Befehl „backup protection undelete“ hinzugefügt, um die Funktion zum vorläufigen Löschen für IaasVM-Workloads zu aktivieren</span><span class="sxs-lookup"><span data-stu-id="fc109-431">Added new command 'backup protection undelete' to enable soft-delete feature for IaasVM workload</span></span>
* <span data-ttu-id="fc109-432">Neuer Parameter „--soft-delete-feature-state“ hinzugefügt, um den Befehl „backup-properties“ festzulegen</span><span class="sxs-lookup"><span data-stu-id="fc109-432">Added new parameter '--soft-delete-feature-state' to set backup-properties command</span></span>
* <span data-ttu-id="fc109-433">Unterstützung für den Ausschluss von Datenträgern für IaasVM-Workload hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-433">Added disk exclusion support for IaasVM workload</span></span>

### <a name="compute"></a><span data-ttu-id="fc109-434">Compute</span><span class="sxs-lookup"><span data-stu-id="fc109-434">Compute</span></span>

* <span data-ttu-id="fc109-435">Fehler `vm create` in Azure Stack-Profil behoben.</span><span class="sxs-lookup"><span data-stu-id="fc109-435">Fix `vm create` failure in Azure Stack profile.</span></span>
* <span data-ttu-id="fc109-436">vm monitor metrics tail/list-definitions: Unterstützung einer Abfragemetrik und von Listendefinitionen für eine VM.</span><span class="sxs-lookup"><span data-stu-id="fc109-436">vm monitor metrics tail/list-definitions: support query metric and list definitions for a vm.</span></span>
* <span data-ttu-id="fc109-437">Neue Aktion des Befehls zum erneuten Anwenden für „az vm“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-437">Add new reapply command action for az vm</span></span>

### <a name="hdinsight"></a><span data-ttu-id="fc109-438">HDInsight</span><span class="sxs-lookup"><span data-stu-id="fc109-438">HDInsight</span></span>

* <span data-ttu-id="fc109-439">Unterstützung für das Erstellen eines Kafka-Clusters mit Kafka-REST-Proxy</span><span class="sxs-lookup"><span data-stu-id="fc109-439">Support for creating a Kafka cluster with Kafka Rest Proxy</span></span>
* <span data-ttu-id="fc109-440">„azure-mgmt-hdinsight“ auf 1.3.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="fc109-440">Upgrade azure-mgmt-hdinsight to 1.3.0</span></span>

### <a name="misc"></a><span data-ttu-id="fc109-441">Verschiedenes:</span><span class="sxs-lookup"><span data-stu-id="fc109-441">Misc.</span></span>

* <span data-ttu-id="fc109-442">Vorschaubefehl `az version show` hinzugefügt, um die Versionen der Azure CLI-Module und Erweiterungen standardmäßig im JSON-Format oder im mit „--output“ konfigurierten Format anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="fc109-442">Add preview command `az version show` to show the versions of Azure CLI modules and extensions in JSON format by default or format configured by --output</span></span>

### <a name="event-hubs"></a><span data-ttu-id="fc109-443">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="fc109-443">Event Hubs</span></span>

* <span data-ttu-id="fc109-444">[BREAKING CHANGE] Statusoption „ReceiveDisabled“ aus „az eventhubs eventhub update“ und „az eventhubs eventhub create“ entfernt.</span><span class="sxs-lookup"><span data-stu-id="fc109-444">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az eventhubs eventhub update' and 'az eventhubs eventhub create'.</span></span> <span data-ttu-id="fc109-445">Diese Option ist für Event Hub-Entitäten nicht gültig.</span><span class="sxs-lookup"><span data-stu-id="fc109-445">This option is not valid for Event Hub entities.</span></span>

### <a name="service-bus"></a><span data-ttu-id="fc109-446">Service Bus</span><span class="sxs-lookup"><span data-stu-id="fc109-446">Service Bus</span></span>

* <span data-ttu-id="fc109-447">[BREAKING CHANGE] Statusoption „ReceiveDisabled“ aus Befehlen „az servicebus topic create“, „az servicebus topic update“, „az servicebus queue create“ und „az servicebus queue update“ entfernt.</span><span class="sxs-lookup"><span data-stu-id="fc109-447">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az servicebus topic create', 'az servicebus topic update', 'az servicebus queue create', and 'az servicebus queue update'.</span></span> <span data-ttu-id="fc109-448">Diese Option ist für Service Bus-Themen und -Warteschlangen nicht gültig.</span><span class="sxs-lookup"><span data-stu-id="fc109-448">This option is not valid for Service Bus topics and queues.</span></span>

### <a name="rbac"></a><span data-ttu-id="fc109-449">RBAC</span><span class="sxs-lookup"><span data-stu-id="fc109-449">RBAC</span></span>

* <span data-ttu-id="fc109-450">Behebung Nr. 11712: `az ad app/sp show` gibt nicht den Exitcode 3 zurück, wenn die Anwendung oder der Dienstprinzipal nicht vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="fc109-450">Fix #11712: `az ad app/sp show` does not return exit code 3 when the application or service principal does not exist</span></span>

### <a name="storage"></a><span data-ttu-id="fc109-451">Storage</span><span class="sxs-lookup"><span data-stu-id="fc109-451">Storage</span></span>

* <span data-ttu-id="fc109-452">`az storage account create`: Vorschaukennzeichnung für Parameter „--enable-hierarchical-namespace“ entfernt</span><span class="sxs-lookup"><span data-stu-id="fc109-452">`az storage account create`: Remove preview flag for --enable-hierarchical-namespace parameter</span></span>
* <span data-ttu-id="fc109-453">azure-mgmt-storage-Version auf 7.0.0 aktualisiert, um API-Version 2019-06-01 zu verwenden</span><span class="sxs-lookup"><span data-stu-id="fc109-453">Update azure-mgmt-storage version to 7.0.0 to use api version 2019-06-01</span></span>
* <span data-ttu-id="fc109-454">Neue Parameter `--enable-delete-retention` und `--delete-retention-days` hinzugefügt, um die Verwaltung der Aufbewahrungsrichtlinie für Löschen für „blob-service-properties“ von Speicherkonten zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="fc109-454">Add new parameters `--enable-delete-retention` and `--delete-retention-days` to support managing delete retention policy for storage account blob-service-properties.</span></span>

## <a name="december-17-2019"></a><span data-ttu-id="fc109-455">17. Dezember 2019</span><span class="sxs-lookup"><span data-stu-id="fc109-455">December 17, 2019</span></span>

<span data-ttu-id="fc109-456">2.0.78</span><span class="sxs-lookup"><span data-stu-id="fc109-456">2.0.78</span></span>

### <a name="acr"></a><span data-ttu-id="fc109-457">ACR</span><span class="sxs-lookup"><span data-stu-id="fc109-457">ACR</span></span>

* <span data-ttu-id="fc109-458">Unterstützung für lokalen Kontext in „acr task run“</span><span class="sxs-lookup"><span data-stu-id="fc109-458">Added support Local context in acr task run</span></span>

### <a name="acs"></a><span data-ttu-id="fc109-459">ACS</span><span class="sxs-lookup"><span data-stu-id="fc109-459">ACS</span></span>

* <span data-ttu-id="fc109-460">[BREAKING CHANGE] az openshift create: `--workspace-resource-id` in `--workspace-id` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="fc109-460">[BREAKING CHANGE]az openshift create: rename `--workspace-resource-id` to `--workspace-id`.</span></span>

### <a name="ams"></a><span data-ttu-id="fc109-461">AMS</span><span class="sxs-lookup"><span data-stu-id="fc109-461">AMS</span></span>

* <span data-ttu-id="fc109-462">Befehle zum Anzeigen aktualisiert, sodass 3 zurückgegeben wird, wenn die Ressource nicht gefunden wurde</span><span class="sxs-lookup"><span data-stu-id="fc109-462">Updated show commands to return 3 when resource not found</span></span>

### <a name="appconfig"></a><span data-ttu-id="fc109-463">AppConfig</span><span class="sxs-lookup"><span data-stu-id="fc109-463">AppConfig</span></span>

* <span data-ttu-id="fc109-464">Fehler beim Anhängen der API-Version an die Anforderungs-URL korrigiert.</span><span class="sxs-lookup"><span data-stu-id="fc109-464">Fixed bug when appending api-version to request url.</span></span> <span data-ttu-id="fc109-465">Die vorhandene Lösung funktioniert nicht mit Paginierung.</span><span class="sxs-lookup"><span data-stu-id="fc109-465">The existing solution doesn't work with pagination.</span></span>
* <span data-ttu-id="fc109-466">Unterstützung für die Anzeige von weiteren Sprachen neben Englisch hinzugefügt, da der Back-End-Dienst Unicode für die Globalisierung unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fc109-466">Added support for showing languages besides English as our backend service support unicode for globalization.</span></span>

### <a name="appservice"></a><span data-ttu-id="fc109-467">AppService</span><span class="sxs-lookup"><span data-stu-id="fc109-467">AppService</span></span>

* <span data-ttu-id="fc109-468">Problem Nr. 11217 behoben: Web-App: „az webapp config ssl upload“ muss Slot-Parameter unterstützen.</span><span class="sxs-lookup"><span data-stu-id="fc109-468">Fixed issue #11217: webapp: az webapp config ssl upload should support slot parameter</span></span>
* <span data-ttu-id="fc109-469">Problem Nr. 10965 behoben: Error: Der Name darf nicht leer sein.</span><span class="sxs-lookup"><span data-stu-id="fc109-469">Fixed issue #10965: Error: Name cannot be empty.</span></span> <span data-ttu-id="fc109-470">Entfernen anhand von „ip_address“ und „subnet“ zulassen</span><span class="sxs-lookup"><span data-stu-id="fc109-470">Allow remove by ip_address and subnet</span></span>
* <span data-ttu-id="fc109-471">Unterstützung des Imports von Zertifikaten aus Key Vault hinzugefügt `az webapp config ssl import`</span><span class="sxs-lookup"><span data-stu-id="fc109-471">Added support for importing certificates from Key Vault `az webapp config ssl import`</span></span>

### <a name="arm"></a><span data-ttu-id="fc109-472">ARM</span><span class="sxs-lookup"><span data-stu-id="fc109-472">ARM</span></span>

* <span data-ttu-id="fc109-473">Paket „azure-mgmt-resource“ auf die Verwendung von 6.0.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="fc109-473">Updated azure-mgmt-resource package to use 6.0.0</span></span>
* <span data-ttu-id="fc109-474">Mandantenübergreifende Unterstützung für Befehl `az group deployment create` durch Hinzufügen des neuen Parameters `--aux-subs`</span><span class="sxs-lookup"><span data-stu-id="fc109-474">Cross Tenant Support for `az group deployment create` command by adding new parameter `--aux-subs`</span></span>
* <span data-ttu-id="fc109-475">Neuer Parameter `--metadata` hinzugefügt, um das Hinzufügen von Metadateninformationen für Richtliniensatzdefinitionen zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="fc109-475">Added new parameter `--metadata` to support adding metadata information for policy set definitions.</span></span>

### <a name="backup"></a><span data-ttu-id="fc109-476">Backup</span><span class="sxs-lookup"><span data-stu-id="fc109-476">Backup</span></span>

* <span data-ttu-id="fc109-477">Unterstützung der Sicherung für SQL- und SAP Hana-Workloads hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-477">Added Backup support for SQL and SAP Hana workload.</span></span>

### <a name="botservice"></a><span data-ttu-id="fc109-478">BotService</span><span class="sxs-lookup"><span data-stu-id="fc109-478">BotService</span></span>

* <span data-ttu-id="fc109-479">[Breaking Change] Flag „--version“ aus Vorschaubefehl „az bot create“ entfernt.</span><span class="sxs-lookup"><span data-stu-id="fc109-479">[Breaking change] Remove '--version' flag from preview command 'az bot create'.</span></span> <span data-ttu-id="fc109-480">Nur v4-SDK-Bots werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fc109-480">Only v4 SDK bots are supported.</span></span>
* <span data-ttu-id="fc109-481">Überprüfung der Namensverfügbarkeit für „az bot create“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-481">Added name availability check for 'az bot create'.</span></span>
* <span data-ttu-id="fc109-482">Unterstützung für das Aktualisieren der Symbol-URL für einen Bot über „az bot update“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-482">Added support for updating the icon URL for a bot via 'az bot update'.</span></span>
* <span data-ttu-id="fc109-483">Unterstützung für das Aktualisieren eines Direct Line-Kanals über „az bot directline update“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-483">Added support for updating a Direct Line channel via 'az bot directline update'.</span></span>
* <span data-ttu-id="fc109-484">Unterstützung für Flag „--enable-enhanced-auth“ zu „az bot directline create“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-484">Added '--enable-enhanced-auth' flag support to 'az bot directline create'.</span></span>
* <span data-ttu-id="fc109-485">Die folgenden Befehlsgruppen sind allgemein verfügbar und befinden sich nicht in der Vorschau: „az bot authsetting“.</span><span class="sxs-lookup"><span data-stu-id="fc109-485">The following command groups are GA and not in preview: 'az bot authsetting'.</span></span>
* <span data-ttu-id="fc109-486">Die folgenden Befehle in „az bot“ sind allgemein verfügbar und befinden sich nicht in der Vorschau: „create“, „prepare-deploy“, „show“, „delete“, „update“.</span><span class="sxs-lookup"><span data-stu-id="fc109-486">The following commands in 'az bot' are GA and not in preview: 'create', 'prepare-deploy', 'show', 'delete', 'update'.</span></span>
* <span data-ttu-id="fc109-487">„az bot prepare-deploy“ korrigiert, indem der Wert voon „--proj-file-path“ in Kleinschreibung geändert wurde (z. B. „Test.csproj“ in „test.csproj“).</span><span class="sxs-lookup"><span data-stu-id="fc109-487">Fixed 'az bot prepare-deploy' changing '--proj-file-path' value to lower case (e.g. "Test.csproj" to "test.csproj").</span></span>

### <a name="compute"></a><span data-ttu-id="fc109-488">Compute</span><span class="sxs-lookup"><span data-stu-id="fc109-488">Compute</span></span>

* <span data-ttu-id="fc109-489">vmss create/update: „--scale-in-policy“ hinzugefügt, womit entschieden wird, welche virtuellen Computer beim horizontalen Herunterskalieren einer VM-Skalierungsgruppe zum Entfernen ausgewählt werden.</span><span class="sxs-lookup"><span data-stu-id="fc109-489">vmss create/update: Added --scale-in-policy, which decides which virtual machines are chosen for removal when a VMSS is scaled-in.</span></span>
* <span data-ttu-id="fc109-490">vm/vmss update: „--priority“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-490">vm/vmss update: Added --priority.</span></span>
* <span data-ttu-id="fc109-491">vm/vmss update: „--max-price“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-491">vm/vmss update: Added --max-price.</span></span>
* <span data-ttu-id="fc109-492">Befehlsgruppe „disk-encryption-set“ hinzugefügt (create, show, update, delete, list).</span><span class="sxs-lookup"><span data-stu-id="fc109-492">Added disk-encryption-set command group (create, show, update, delete, list).</span></span>
* <span data-ttu-id="fc109-493">disk create: „--encryption-type“ und „--disk-encryption-set“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-493">disk create: Added --encryption-type and --disk-encryption-set.</span></span>
* <span data-ttu-id="fc109-494">vm/vmss create: „--os-disk-encryption-set“ und „--data-disk-encryption-sets“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-494">vm/vmss create: Added --os-disk-encryption-set and --data-disk-encryption-sets.</span></span>

### <a name="core"></a><span data-ttu-id="fc109-495">Core</span><span class="sxs-lookup"><span data-stu-id="fc109-495">Core</span></span>

* <span data-ttu-id="fc109-496">Unterstützung für Python 3.4 entfernt</span><span class="sxs-lookup"><span data-stu-id="fc109-496">Removed support for Python 3.4</span></span>
* <span data-ttu-id="fc109-497">Plug-In für HaTS-Umfrage in mehreren Befehlen</span><span class="sxs-lookup"><span data-stu-id="fc109-497">Plug in HaTS survey in multiple commands</span></span>

### <a name="dls"></a><span data-ttu-id="fc109-498">DLS</span><span class="sxs-lookup"><span data-stu-id="fc109-498">DLS</span></span>

* <span data-ttu-id="fc109-499">ADLS-SDK-Version aktualisiert (0.0.48).</span><span class="sxs-lookup"><span data-stu-id="fc109-499">Updated ADLS sdk version (0.0.48).</span></span>

### <a name="install"></a><span data-ttu-id="fc109-500">Installieren</span><span class="sxs-lookup"><span data-stu-id="fc109-500">Install</span></span>

* <span data-ttu-id="fc109-501">Installationsskript unterstützt Python 3.8</span><span class="sxs-lookup"><span data-stu-id="fc109-501">Install script support python 3.8</span></span>

### <a name="iot"></a><span data-ttu-id="fc109-502">IoT</span><span class="sxs-lookup"><span data-stu-id="fc109-502">IOT</span></span>

* <span data-ttu-id="fc109-503">[BREAKING CHANGE] Parameter „--failover-region“ aus „manual-failover“ entfernt.</span><span class="sxs-lookup"><span data-stu-id="fc109-503">[BREAKING CHANGE] Removed --failover-region parameter from manual-failover.</span></span> <span data-ttu-id="fc109-504">Das Failover erfolgt jetzt in eine zugewiesene, geografisch gekoppelte sekundäre Region.</span><span class="sxs-lookup"><span data-stu-id="fc109-504">Now it will failover to assigned geo-paired secondary region.</span></span>

### <a name="key-vault"></a><span data-ttu-id="fc109-505">Key Vault</span><span class="sxs-lookup"><span data-stu-id="fc109-505">Key Vault</span></span>

* <span data-ttu-id="fc109-506">Nr. 8095 behoben: `az keyvault storage remove`: Hilfemeldung verbessert</span><span class="sxs-lookup"><span data-stu-id="fc109-506">Fixed #8095: `az keyvault storage remove`: improve the help message</span></span>
* <span data-ttu-id="fc109-507">Nr. 8921 behoben: `az keyvault key/secret/certificate list/list-deleted/list-versions`: Validierungsfehler in Parameter `--maxresults` behoben</span><span class="sxs-lookup"><span data-stu-id="fc109-507">Fixed #8921: `az keyvault key/secret/certificate list/list-deleted/list-versions`: fix the validation bug on parameter `--maxresults`</span></span>
* <span data-ttu-id="fc109-508">Nr. 10512 behoben: `az keyvault set-policy`: Fehlermeldung verbessert, wenn weder `--object-id`, `--spn` noch `--upn` angegeben ist</span><span class="sxs-lookup"><span data-stu-id="fc109-508">Fixed #10512: `az keyvault set-policy`: improve the error message when none of `--object-id`, `--spn` or `--upn` is specified</span></span>
* <span data-ttu-id="fc109-509">Nr. 10846 behoben: `az keyvault secret show-deleted`: Wenn `--id` angegeben ist, ist `--name/-n` nicht erforderlich.</span><span class="sxs-lookup"><span data-stu-id="fc109-509">Fixed #10846: `az keyvault secret show-deleted`: when `--id` is specified, `--name/-n` is not required</span></span>
* <span data-ttu-id="fc109-510">Nr. 11084 behoben: `az keyvault secret download`: Hilfemeldung von Parameter `--encoding` verbessert</span><span class="sxs-lookup"><span data-stu-id="fc109-510">Fixed #11084: `az keyvault secret download`: improve the help message of parameter `--encoding`</span></span>

### <a name="network"></a><span data-ttu-id="fc109-511">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="fc109-511">Network</span></span>

* <span data-ttu-id="fc109-512">az network application-gateway probe: Unterstützung für Option „--port“ hinzugefügt, um einen Port zum Prüfen von Back-End-Servern beim Erstellen und Aktualisieren anzugeben</span><span class="sxs-lookup"><span data-stu-id="fc109-512">az network application-gateway probe: Added support --port option to specify a port for probing backend servers when create and update</span></span>
* <span data-ttu-id="fc109-513">az network application-gateway url-path-map create/update: Fehlerbehebung für `--waf-policy`</span><span class="sxs-lookup"><span data-stu-id="fc109-513">az network application-gateway url-path-map create/update: bug fix for `--waf-policy`</span></span>
* <span data-ttu-id="fc109-514">az network application-gateway: Unterstützung für `--rewrite-rule-set` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-514">az network application-gateway: Added support `--rewrite-rule-set`</span></span>
* <span data-ttu-id="fc109-515">az network list-service-aliases: Unterstützung für Listendienstaliase hinzugefügt, die für Dienstendpunktrichtlinien verwendet werden können</span><span class="sxs-lookup"><span data-stu-id="fc109-515">az network list-service-aliases: Added support list service aliases which can be used for Service Endpoint Policies</span></span>
* <span data-ttu-id="fc109-516">az network dns zone import: Unterstützung für „.@“ in Datensatzname hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-516">az network dns zone import: Added support .@ in record name</span></span>

### <a name="packaging"></a><span data-ttu-id="fc109-517">Verpackung</span><span class="sxs-lookup"><span data-stu-id="fc109-517">Packaging</span></span>

* <span data-ttu-id="fc109-518">Back-Edge-Builds für PIP-Installation hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-518">Added back edge builds for pip install</span></span>
* <span data-ttu-id="fc109-519">Ubuntu-Eoan-Paket hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-519">Added Ubuntu eoan package</span></span>

### <a name="policy"></a><span data-ttu-id="fc109-520">Richtlinie</span><span class="sxs-lookup"><span data-stu-id="fc109-520">Policy</span></span>

* <span data-ttu-id="fc109-521">Unterstützung für Version 2019-09-01 der Richtlinien-API hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-521">Added support for Policy API version 2019-09-01.</span></span>
* <span data-ttu-id="fc109-522">az policy set-definition: Unterstützung der Gruppierung innerhalb von Richtliniensatzdefinitionen mit `--definition-groups`-Parameter hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-522">az policy set-definition: Added support grouping within policy set definitions with `--definition-groups` parameter</span></span>

### <a name="redis"></a><span data-ttu-id="fc109-523">Redis</span><span class="sxs-lookup"><span data-stu-id="fc109-523">Redis</span></span>

* <span data-ttu-id="fc109-524">Vorschauparameter `--replicas-per-master` zu Befehl `az redis create`hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-524">Added preview param `--replicas-per-master` to `az redis create` command</span></span>
* <span data-ttu-id="fc109-525">„azure-mgmt-redis“ von 6.0.0 auf 7.0.0rc1 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="fc109-525">Updated azure-mgmt-redis from 6.0.0 to 7.0.0rc1</span></span>

### <a name="servicefabric"></a><span data-ttu-id="fc109-526">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="fc109-526">ServiceFabric</span></span>

* <span data-ttu-id="fc109-527">Hinzufügen von Logik in Knotentyp korrigiert, einschließlich Nr. 10963: Beim Hinzufügen eines neuen Knotentyps mit Dauerhaftigkeitsstufe „Gold“ wird immer ein CLI-Fehler ausgegeben.</span><span class="sxs-lookup"><span data-stu-id="fc109-527">Fixed in node-type add logic including #10963: Adding new node type with durability level Gold will always throw CLI error</span></span>
* <span data-ttu-id="fc109-528">ServiceFabricNodeVmExt-Version in Erstellungsvorlage auf 1.1 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="fc109-528">Updated ServiceFabricNodeVmExt version to 1.1 in creation template</span></span>

### <a name="sql"></a><span data-ttu-id="fc109-529">SQL</span><span class="sxs-lookup"><span data-stu-id="fc109-529">SQL</span></span>

* <span data-ttu-id="fc109-530">Parameter „--read-scale“ und „--read-replicas“ zu Befehlen „sql db create“ und „sql db update“ hinzugefügt, um Leseskalierungsverwaltung zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="fc109-530">Added "--read-scale" and "--read-replicas" parameters to sql db create and update commands, to support read scale management.</span></span>

### <a name="storage"></a><span data-ttu-id="fc109-531">Storage</span><span class="sxs-lookup"><span data-stu-id="fc109-531">Storage</span></span>

* <span data-ttu-id="fc109-532">Allgemein verfügbares Release – Eigenschaft „Large File Shares“ für Befehle „storage account create“ und „storage account update“</span><span class="sxs-lookup"><span data-stu-id="fc109-532">GA Release Large File Shares property for storage account create and update command</span></span>
* <span data-ttu-id="fc109-533">Allgemein verfügbares Release – Unterstützung von SAS-Token für die Benutzerdelegierung</span><span class="sxs-lookup"><span data-stu-id="fc109-533">GA Release User Delegation SAS token Support</span></span>
* <span data-ttu-id="fc109-534">Neue Befehle `az storage account blob-service-properties show` und `az storage account blob-service-properties update --enable-change-feed` hinzugefügt, um Blob-Diensteigenschaften für das Speicherkonto zu verwalten.</span><span class="sxs-lookup"><span data-stu-id="fc109-534">Added new commands `az storage account blob-service-properties show` and `az storage account blob-service-properties update --enable-change-feed` to manage blob service properties for storage account.</span></span>
* <span data-ttu-id="fc109-535">[BEVORSTEHENDER BREAKING CHANGE] `az storage copy`: Das Zeichen `*` wird nicht mehr als Platzhalter in der URL, es werden jedoch die neuen Parameter „--include-pattern“ und „--exclude-pattern“ mit Unterstützung des Platzhalters `*` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-535">[COMING BREAKING CHANGE] `az storage copy`: `*` character is no longer supported as a wildcard in URL, but new parameters --include-pattern and --exclude-pattern will be added with `*` wildcard support.</span></span>
* <span data-ttu-id="fc109-536">Problem Nr. 11043 behoben: Unterstützung für das Entfernen des gesamten Containers/der gesamten Freigabe in `az storage remove` Befehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-536">Fixed issue #11043: Added support to remove whole container/share in `az storage remove` command</span></span>

## <a name="november-26-2019"></a><span data-ttu-id="fc109-537">26. November 2019</span><span class="sxs-lookup"><span data-stu-id="fc109-537">November 26, 2019</span></span>

<span data-ttu-id="fc109-538">Version 2.0.77</span><span class="sxs-lookup"><span data-stu-id="fc109-538">Version 2.0.77</span></span>

### <a name="acr"></a><span data-ttu-id="fc109-539">ACR</span><span class="sxs-lookup"><span data-stu-id="fc109-539">ACR</span></span>

* <span data-ttu-id="fc109-540">Parameter `--branch` in „acr task create/update“ als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="fc109-540">Deprecated parameter `--branch` from acr task create/update</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="fc109-541">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="fc109-541">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="fc109-542">`--workspace-resource-id`-Flag hinzugefügt, um die Erstellung eines Azure Red Hat OpenShift-Clusters mit Überwachung zuzulassen</span><span class="sxs-lookup"><span data-stu-id="fc109-542">Added `--workspace-resource-id` flag to allow creation of Azure Red Hat Openshift cluster with monitoring</span></span>
* <span data-ttu-id="fc109-543">`monitor_profile`-Flag hinzugefügt, um einen Azure Red Hat OpenShift-Clusters mit Überwachung zu erstellen</span><span class="sxs-lookup"><span data-stu-id="fc109-543">Added `monitor_profile` to create Azure Red Hat OpenShift cluster with monitoring</span></span>

### <a name="aks"></a><span data-ttu-id="fc109-544">AKS</span><span class="sxs-lookup"><span data-stu-id="fc109-544">AKS</span></span>

* <span data-ttu-id="fc109-545">Unterstützung des Rotationsvorgangs für Clusterzertifikate mithilfe von für Cluster Zertifikat Rotation mit „az aks rotate-certs“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-545">Added support cluster certificate rotation operation using "az aks rotate-certs".</span></span>

### <a name="appconfig"></a><span data-ttu-id="fc109-546">AppConfig</span><span class="sxs-lookup"><span data-stu-id="fc109-546">AppConfig</span></span>

* <span data-ttu-id="fc109-547">Unterstützung für die Verwendung von „:“ für `as az appconfig kv import`-Trennzeichen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-547">Added support for using ":" for `as az appconfig kv import` separator</span></span>
* <span data-ttu-id="fc109-548">Problem beim Auflisten von Schlüsselwerten mit mehreren Bezeichnungen, einschließlich NULL-Bezeichnung, behoben.</span><span class="sxs-lookup"><span data-stu-id="fc109-548">Fixed issue for listing key values with multiple labels including null label.</span></span> 
* <span data-ttu-id="fc109-549">Verwaltungsebenen-SDK, „azure-mgmt-appconfiguration“, auf Version 0.3.0 aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="fc109-549">Updated management plane sdk, azure-mgmt-appconfiguration, to version 0.3.0.</span></span> 

### <a name="appservice"></a><span data-ttu-id="fc109-550">AppService</span><span class="sxs-lookup"><span data-stu-id="fc109-550">AppService</span></span>

* <span data-ttu-id="fc109-551">Problem Nr. 11100 behoben AttributeError für „az webapp up“ beim Erstellen eines Dienstplans</span><span class="sxs-lookup"><span data-stu-id="fc109-551">Fixed issue #11100: AttributeError for az webapp up when create service plan</span></span>
* <span data-ttu-id="fc109-552">az webapp up: Erzwingen der Erstellung oder Bereitstellung auf einer Website für unterstützte Sprachen, es werden keine Standardeinstellungen verwendet.</span><span class="sxs-lookup"><span data-stu-id="fc109-552">az webapp up: Forcing the creation or deployment to a site for supported languages, no defaults used.</span></span>
* <span data-ttu-id="fc109-553">Unterstützung für App Service-Umgebung hinzugefügt: az appservice ase show | list | list-addresses | list-plans | create | update | delete</span><span class="sxs-lookup"><span data-stu-id="fc109-553">Added support for App Service Environment: az appservice ase show | list | list-addresses | list-plans | create | update | delete</span></span>

### <a name="backup"></a><span data-ttu-id="fc109-554">Backup</span><span class="sxs-lookup"><span data-stu-id="fc109-554">Backup</span></span>

* <span data-ttu-id="fc109-555">Problem in Az-Sicherungsrichtlinie „list-associated-items“ behoben.</span><span class="sxs-lookup"><span data-stu-id="fc109-555">Fixed issue in az backup policy list-associated-items.</span></span> <span data-ttu-id="fc109-556">Optionaler Parameter „BackupManagementType“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-556">Added optional BackupManagementType parameter.</span></span>

### <a name="compute"></a><span data-ttu-id="fc109-557">Compute</span><span class="sxs-lookup"><span data-stu-id="fc109-557">Compute</span></span>

* <span data-ttu-id="fc109-558">API-Version von Compute, Datenträger, Momentaufnahmen auf 2019-07-01 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="fc109-558">Upgraded API version of compute, disks, snapshots to 2019-07-01</span></span>
* <span data-ttu-id="fc109-559">vmss create: Verbesserung für – Orchestrierungsmodus</span><span class="sxs-lookup"><span data-stu-id="fc109-559">vmss create: Improvement for --orchestration-mode</span></span>
* <span data-ttu-id="fc109-560">sig image-definition create: „--os-state“ hinzugefügt, um die Angabe zu ermöglichen, ob die unter diesem Image erstellten virtuellen Computer „generalisiert“ oder „spezialisiert“ sind</span><span class="sxs-lookup"><span data-stu-id="fc109-560">sig image-definition create: Added --os-state to allow specifying whether the virtual machines created under this image are 'Generalized' or 'Specialized'</span></span>
* <span data-ttu-id="fc109-561">sig image-definition create: „--hyper-v-generation“ hinzugefügt, um die Angabe der Hypervisorgeneration zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="fc109-561">sig image-definition create: Added --hyper-v-generation to allow specifying the hypervisor generation</span></span>
* <span data-ttu-id="fc109-562">sig image-version create: Unterstützung für „--os-snapshot“ und „--data-snapshots“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-562">sig image-version create: Added support --os-snapshot and --data-snapshots</span></span>
* <span data-ttu-id="fc109-563">image create: „--data-disk-caching“ hinzugefügt, um die Angabe der Zwischenspeicherungseinstellung von Datenträger zu ermöflichen</span><span class="sxs-lookup"><span data-stu-id="fc109-563">image create: Added --data-disk-caching to allow specifying caching setting of data disks</span></span>
* <span data-ttu-id="fc109-564">Upgrade des Python-Compute-SDK auf 10.0.0</span><span class="sxs-lookup"><span data-stu-id="fc109-564">Upgraded Python Compute SDK to 10.0.0</span></span>
* <span data-ttu-id="fc109-565">vm/vmss create: „Spot“ zu Aufzählungseigenschaft „Priority“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-565">vm/vmss create: Added 'Spot' to 'Priority' enum property</span></span>
* <span data-ttu-id="fc109-566">[Breaking Change] Parameter „--max-billing“ für sowohl VM als auch VMSS in „--max-price“ umbenannt, um die Konsistenz mit Swagger- und PowerShell-Cmdlets sicherzustellen</span><span class="sxs-lookup"><span data-stu-id="fc109-566">[Breaking change] Renamed '--max-billing' parameter to '--max-price', for both VM and VMSS, to be consistent with Swagger and Powershell cmdlets</span></span>
* <span data-ttu-id="fc109-567">vm monitor log show: Unterstützung für das Abfragen von Protokollen über verknüpften Protokollanalyse-Arbeitsbereich hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-567">vm monitor log show: Added support for querying log over linked log analytics workspace.</span></span>

### <a name="iot"></a><span data-ttu-id="fc109-568">IoT</span><span class="sxs-lookup"><span data-stu-id="fc109-568">IOT</span></span>

* <span data-ttu-id="fc109-569">Behebung Nr. 2531: Argumente für Benutzerfreundlichkeit für Hub-Update hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-569">Fix #2531: Added convenience arguments for hub update.</span></span>
* <span data-ttu-id="fc109-570">Behebung Nr. 8323: Fehlende Parameter zum Erstellen eines benutzerdefinierten Speicherendpunkts hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-570">Fix #8323: Added missing parameters to create storage custom endpoint.</span></span>
* <span data-ttu-id="fc109-571">Regressionsfehler behoben: Die Änderungen wurden rückgängig gemacht, sodass der standardmäßige Speicherendpunkt überschrieben wurde.</span><span class="sxs-lookup"><span data-stu-id="fc109-571">Fix regression bug: Reverted the changes which overrides the default storage endpoint.</span></span>

### <a name="key-vault"></a><span data-ttu-id="fc109-572">Key Vault</span><span class="sxs-lookup"><span data-stu-id="fc109-572">Key Vault</span></span>

* <span data-ttu-id="fc109-573">Nr. 11121 behoben: Bei der Verwendung von `az keyvault certificate list` erfordert die Übergabe von `--include-pending` jetzt nicht mehr den Wert `true` oder `false`.</span><span class="sxs-lookup"><span data-stu-id="fc109-573">Fixed #11121: When using `az keyvault certificate list`, passing `--include-pending` now doesn't require a value of `true` or `false`</span></span>

### <a name="netappfiles"></a><span data-ttu-id="fc109-574">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="fc109-574">NetAppFiles</span></span>

* <span data-ttu-id="fc109-575">Upgrade von „azure-mgmt-netapp“ auf Version 0.7.0, die einige zusätzliche Volumeeigenschaften enthält, die bevorstehenden Replikationsvorgängen zugeordnet sind</span><span class="sxs-lookup"><span data-stu-id="fc109-575">Upgraded azure-mgmt-netapp to 0.7.0 which includes some additional volume properties associated with upcoming replication operations</span></span>

### <a name="network"></a><span data-ttu-id="fc109-576">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="fc109-576">Network</span></span>

* <span data-ttu-id="fc109-577">application-gateway waf-config: veraltet</span><span class="sxs-lookup"><span data-stu-id="fc109-577">application-gateway waf-config: deprecated</span></span>
* <span data-ttu-id="fc109-578">application-gateway waf-policy: Untergruppe „managed-rules“ zur Verwaltung von verwalteten Regelsätzen und Ausschlussregeln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-578">application-gateway waf-policy: Added subgroup managed-rules to manage managed rule sets and exclusion rules</span></span>
* <span data-ttu-id="fc109-579">application-gateway waf-policy: Untergruppe „policy-setting“ zur Verwaltung der globalen Konfiguration von „waf-policy“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-579">application-gateway waf-policy: Added subgroup policy-setting to manage global configuration of a waf-policy</span></span>
* <span data-ttu-id="fc109-580">[BREAKING CHANGE] application-gateway waf-policy: Untergruppenregel in „custom-rule“ umbenannt</span><span class="sxs-lookup"><span data-stu-id="fc109-580">[BREAKING CHANGE] application-gateway waf-policy: Renamed subgroup rule to custom-rule</span></span>
* <span data-ttu-id="fc109-581">application-gateway http-listener: „--firewall-policy“ beim Erstellen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-581">application-gateway http-listener: Added --firewall-policy when create</span></span>
* <span data-ttu-id="fc109-582">application-gateway url-path-map rule: „--firewall-policy“ beim Erstellen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-582">application-gateway url-path-map rule: Added --firewall-policy when create</span></span>

### <a name="packaging"></a><span data-ttu-id="fc109-583">Verpackung</span><span class="sxs-lookup"><span data-stu-id="fc109-583">Packaging</span></span>

* <span data-ttu-id="fc109-584">Az-Wrapper in Python neu geschrieben</span><span class="sxs-lookup"><span data-stu-id="fc109-584">Rewrote the az wrapper in Python</span></span>
* <span data-ttu-id="fc109-585">Unterstützung für Python 3.8 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-585">Added support for Python 3.8</span></span>
* <span data-ttu-id="fc109-586">Für RPM-Paket in Python 3 geändert</span><span class="sxs-lookup"><span data-stu-id="fc109-586">Changed to Python 3 for RPM package</span></span>

### <a name="profile"></a><span data-ttu-id="fc109-587">Profil</span><span class="sxs-lookup"><span data-stu-id="fc109-587">Profile</span></span>

* <span data-ttu-id="fc109-588">Fehler beim Ausführen von `az login -u {} -p {}` mit Microsoft-Konto entfernt</span><span class="sxs-lookup"><span data-stu-id="fc109-588">Polished error when running `az login -u {} -p {}` with Microsoft account</span></span>
* <span data-ttu-id="fc109-589">`SSLError` beim Ausführen von `az login` hinter einem Proxy mit einem selbstsignierten Stammzertifikat entfernt</span><span class="sxs-lookup"><span data-stu-id="fc109-589">Polished `SSLError` when running `az login` behind a proxy with self-signed root certificate</span></span>
* <span data-ttu-id="fc109-590">Nr. 10578 behoben: `az login` hängt, wenn mehrere Instanzen gleichzeitig unter Windows oder WSL gestartet werden.</span><span class="sxs-lookup"><span data-stu-id="fc109-590">Fixed #10578: `az login` hangs when more than one instances are launched at the same time on Windows or WSL</span></span>
* <span data-ttu-id="fc109-591">Nr. 11059 behoben: `az login --allow-no-subscriptions` schlägt fehl, wenn Abonnements im Mandanten vorhanden sind.</span><span class="sxs-lookup"><span data-stu-id="fc109-591">Fixed #11059: `az login --allow-no-subscriptions` fails if there are subscriptions in the tenant</span></span>
* <span data-ttu-id="fc109-592">Nr. 11238 behoben: Nach dem Umbenennen eines Abonnements führt die Anmeldung mit MSI dazu, dass das gleiche Abonnement zweimal angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="fc109-592">Fixed #11238: After renaming a subscription, logging in with MSI will result in the same subscription appearing twice</span></span>

### <a name="rbac"></a><span data-ttu-id="fc109-593">RBAC</span><span class="sxs-lookup"><span data-stu-id="fc109-593">RBAC</span></span>

* <span data-ttu-id="fc109-594">Nr. 10996 behoben: Fehler für `--force-change-password-next-login` in `az ad user update` entfernt, wenn `--password` nicht angegeben ist</span><span class="sxs-lookup"><span data-stu-id="fc109-594">Fixed #10996: Polish error for `--force-change-password-next-login` in `az ad user update` when `--password` is not specified</span></span>

### <a name="redis"></a><span data-ttu-id="fc109-595">Redis</span><span class="sxs-lookup"><span data-stu-id="fc109-595">Redis</span></span>

* <span data-ttu-id="fc109-596">Nr. 2902 behoben: Festlegen von Speicherkonfigurationen beim Aktualisieren des Basic-SKU-Cache vermeiden</span><span class="sxs-lookup"><span data-stu-id="fc109-596">Fixed #2902: Avoid setting memory configs while updating Basic SKU cache</span></span>

### <a name="reservations"></a><span data-ttu-id="fc109-597">Reservations</span><span class="sxs-lookup"><span data-stu-id="fc109-597">Reservations</span></span>

* <span data-ttu-id="fc109-598">SDK-Version auf 0.6.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="fc109-598">Upgraded SDK Version to 0.6.0</span></span>
* <span data-ttu-id="fc109-599">Abrechnungsplandetails nach dem Aufrufen von „Get-Gatalogs“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-599">Added billingplan details info after calling Get-Gatalogs</span></span>
* <span data-ttu-id="fc109-600">Neuer Befehl `az reservations reservation-order calculate` zum Berechnen des Preises für eine Reservierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-600">Added new command `az reservations reservation-order calculate` to calculate the price for a reservation</span></span>
* <span data-ttu-id="fc109-601">Neuer Befehl `az reservations reservation-order purchase` zum Erwerb einer neuen Reservierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-601">Added new command `az reservations reservation-order purchase` to purchase a new reservation</span></span>

### <a name="rest"></a><span data-ttu-id="fc109-602">REST</span><span class="sxs-lookup"><span data-stu-id="fc109-602">Rest</span></span>
* <span data-ttu-id="fc109-603">`az rest` in allgemeine Verfügbarkeit geändert</span><span class="sxs-lookup"><span data-stu-id="fc109-603">Changed `az rest` to GA</span></span>

### <a name="sql"></a><span data-ttu-id="fc109-604">SQL</span><span class="sxs-lookup"><span data-stu-id="fc109-604">SQL</span></span>

* <span data-ttu-id="fc109-605">„azure-mgmt-sql“ auf Version 0.15.0 aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="fc109-605">Updated azure-mgmt-sql to version 0.15.0.</span></span>

### <a name="storage"></a><span data-ttu-id="fc109-606">Storage</span><span class="sxs-lookup"><span data-stu-id="fc109-606">Storage</span></span>

* <span data-ttu-id="fc109-607">storage account create: „--enable-hierarchical-namespace“ hinzugefügt, um Dateisystemsemantik in Blobdienst zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="fc109-607">storage account create: Added --enable-hierarchical-namespace to support filesystem semantics in blob service.</span></span>
* <span data-ttu-id="fc109-608">Ausnahme ohne Zusammenhang aus Fehlermeldung entfernt</span><span class="sxs-lookup"><span data-stu-id="fc109-608">Removed unrelated exception from error message</span></span>
* <span data-ttu-id="fc109-609">Probleme mit falscher Fehlermeldung „Sie verfügen nicht über die erforderlichen Berechtigungen zum Ausführen dieses Vorgangs“ behoben.</span><span class="sxs-lookup"><span data-stu-id="fc109-609">Fixed issues with incorrect error message "You do not have the required permissions needed to perform this operation."</span></span> <span data-ttu-id="fc109-610">bei Blockierung durch Netzwerkregeln oder bei „AuthenticationFailed“.</span><span class="sxs-lookup"><span data-stu-id="fc109-610">when blocked by network rules or AuthenticationFailed.</span></span>

## <a name="november-4-2019"></a><span data-ttu-id="fc109-611">4\. November 2019</span><span class="sxs-lookup"><span data-stu-id="fc109-611">November 4, 2019</span></span>

<span data-ttu-id="fc109-612">Version 2.0.76</span><span class="sxs-lookup"><span data-stu-id="fc109-612">Version 2.0.76</span></span>

### <a name="acr"></a><span data-ttu-id="fc109-613">ACR</span><span class="sxs-lookup"><span data-stu-id="fc109-613">ACR</span></span>

* <span data-ttu-id="fc109-614">Vorschauparameter `--pack-image-tag` wurde dem Befehl `az acr pack build` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-614">Added a preview parameter `--pack-image-tag` to command `az acr pack build`.</span></span>
* <span data-ttu-id="fc109-615">Unterstützung der Aktivierung der Überwachung beim Erstellen einer Registrierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-615">Added support for enabling auditing on creating a registry</span></span>
* <span data-ttu-id="fc109-616">Unterstützung von RBAC mit Repositoryumfang hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-616">Added support for Repository-scoped RBAC</span></span>

### <a name="aks"></a><span data-ttu-id="fc109-617">AKS</span><span class="sxs-lookup"><span data-stu-id="fc109-617">AKS</span></span>

* <span data-ttu-id="fc109-618">`--enable-cluster-autoscaler`, `--min-count` und `--max-count` wurden dem Befehl `az aks create` hinzugefügt, sodass die automatische Clusterskalierung für den Knotenpool aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="fc109-618">Added `--enable-cluster-autoscaler`, `--min-count` and `--max-count` to the `az aks create` command, which enables cluster autoscaler for the node pool.</span></span>
* <span data-ttu-id="fc109-619">Die obigen Flags sowie `--update-cluster-autoscaler` und `--disable-cluster-autoscaler` wurden dem Befehl `az aks update` hinzugefügt, sodass Updates der automatischen Clusterskalierung zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="fc109-619">Added the above flags as well as `--update-cluster-autoscaler` and `--disable-cluster-autoscaler` to the `az aks update` command, allowing updates to cluster autoscaler.</span></span>

### <a name="appconfig"></a><span data-ttu-id="fc109-620">AppConfig</span><span class="sxs-lookup"><span data-stu-id="fc109-620">AppConfig</span></span>

* <span data-ttu-id="fc109-621">Befehlsgruppe der AppConfig-Funktion zum Verwalten von in einer App Configuration-Instanz gespeicherten Featureflags wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-621">Added appconfig feature command group to manage feature flags stored in an App Configuration.</span></span>
* <span data-ttu-id="fc109-622">Geringfügiger Programmfehler für Befehl „appconfig kv export to file“ wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="fc109-622">Fixed minor bug for appconfig kv export to file command.</span></span> <span data-ttu-id="fc109-623">Das Lesen der Zieldateiinhalte wird während des Exports angehalten.</span><span class="sxs-lookup"><span data-stu-id="fc109-623">Stop reading dest file contents during export.</span></span>

### <a name="appservice"></a><span data-ttu-id="fc109-624">AppService</span><span class="sxs-lookup"><span data-stu-id="fc109-624">AppService</span></span>

* <span data-ttu-id="fc109-625">`az appservice plan create`: Unterstützung für das Festlegen von „persitescalung“ beim Erstellen eines App-Serviceplans wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-625">`az appservice plan create`: Added support to set 'persitescaling' on appservice plan create.</span></span>
* <span data-ttu-id="fc109-626">Ein Problem wurde behoben, aufgrund dessen der Vorgang „webapp config ssl bind“ vorhandene Tags aus der Ressource entfernt hat.</span><span class="sxs-lookup"><span data-stu-id="fc109-626">Fixed an issue where webapp config ssl bind operation was removing existing tags from the resource</span></span>
* <span data-ttu-id="fc109-627">Flag `--build-remote` wurde für `az functionapp deployment source config-zip` hinzugefügt, um die Remotebuildaktion während der Funktions-App-Bereitstellung zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="fc109-627">Added `--build-remote` flag for `az functionapp deployment source config-zip` to support remote build action during function app deployment.</span></span>
* <span data-ttu-id="fc109-628">Die Standardknotenversion in Funktions-Apps wurde für Windows in ~ 10 geändert.</span><span class="sxs-lookup"><span data-stu-id="fc109-628">Changed default node version on function apps to ~10 for Windows</span></span>
* <span data-ttu-id="fc109-629">`--runtime-version`-Eigenschaft zu `az functionapp create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-629">Added `--runtime-version` property to `az functionapp create`</span></span>

### <a name="arm"></a><span data-ttu-id="fc109-630">ARM</span><span class="sxs-lookup"><span data-stu-id="fc109-630">ARM</span></span>

* <span data-ttu-id="fc109-631">`az deployment/group deployment validate`: Parameter `--handle-extended-json-format` wurde hinzugefügt, um bei der Bereitstellung mehrere Zeilen und Kommentare in der JSON-Vorlage zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="fc109-631">`az deployment/group deployment validate`: Added `--handle-extended-json-format` parameter to support multiline and comments in json template when deployment.</span></span>
* <span data-ttu-id="fc109-632">„azure-mgmt-resource“ auf „2019-07-01“ festgelegt</span><span class="sxs-lookup"><span data-stu-id="fc109-632">Bumped azure-mgmt-resource to 2019-07-01</span></span>

### <a name="backup"></a><span data-ttu-id="fc109-633">Backup</span><span class="sxs-lookup"><span data-stu-id="fc109-633">Backup</span></span>

* <span data-ttu-id="fc109-634">Unterstützung für AzureFiles-Sicherung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-634">Added AzureFiles backup support</span></span>

### <a name="compute"></a><span data-ttu-id="fc109-635">Compute</span><span class="sxs-lookup"><span data-stu-id="fc109-635">Compute</span></span>

* <span data-ttu-id="fc109-636">`az vm create`: Beim gleichzeitigen Festlegen von beschleunigtem Netzwerkbetrieb und einer vorhandenen NIC wurde eine Warnung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-636">`az vm create`: Added warning when specifying accelerated networking and an existing NIC together.</span></span>
* <span data-ttu-id="fc109-637">`az vm create`: `--vmss` hinzugefügt, um eine vorhandene VM-Skalierungsgruppe anzugeben, welcher der virtuelle Computer zugewiesen werden soll.</span><span class="sxs-lookup"><span data-stu-id="fc109-637">`az vm create`: Added `--vmss` to specify an existing virtual machine scale set that the virtual machine should be assigned to.</span></span>
* <span data-ttu-id="fc109-638">`az vm/vmss create`: Eine lokale Kopie der Imagealiasdatei wurde hinzugefügt, sodass in einer eingeschränkten Netzwerkumgebung darauf zugegriffen werden kann.</span><span class="sxs-lookup"><span data-stu-id="fc109-638">`az vm/vmss create`: Added a local copy of image alias file so that it can be accessed in a restricted network environment.</span></span>
* <span data-ttu-id="fc109-639">`az vmss create`: `--orchestration-mode` hinzugefügt, um anzugeben, wie virtuelle Computer von der Skalierungsgruppe verwaltet werden.</span><span class="sxs-lookup"><span data-stu-id="fc109-639">`az vmss create`: Added `--orchestration-mode` to specify how virtual machines are managed by the scale set.</span></span>
* <span data-ttu-id="fc109-640">`az vm/vmss update`: `--ultra-ssd-enabled` hinzugefügt, um das Aktualisieren der SSD-Einstellung zuzulassen.</span><span class="sxs-lookup"><span data-stu-id="fc109-640">`az vm/vmss update`: Added `--ultra-ssd-enabled` to allow updating ultra SSD setting.</span></span>
* <span data-ttu-id="fc109-641">[BREAKING CHANGE] `az vm extension set`: Ein Fehler wurde behoben, aufgrund dessen Benutzer mit `--ids` keine Erweiterung auf einem virtuellen Computer festlegen konnten.</span><span class="sxs-lookup"><span data-stu-id="fc109-641">[BREAKING CHANGE] `az vm extension set`: Fixed bug where users could not set an extension on a VM with `--ids`.</span></span>
* <span data-ttu-id="fc109-642">Neue Befehle wurden zu `az vm image terms accept/cancel/show` hinzugefügt , um Azure Marketplace-Imagebedingungen zu verwalten.</span><span class="sxs-lookup"><span data-stu-id="fc109-642">Added new commands `az vm image terms accept/cancel/show` to manage Azure Marketplace image terms.</span></span>
* <span data-ttu-id="fc109-643">VMAccessForLinux auf Version 1.5 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="fc109-643">Updated VMAccessForLinux to version 1.5</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="fc109-644">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="fc109-644">CosmosDB</span></span>

* <span data-ttu-id="fc109-645">[BREAKING CHANGE] `az sql container create`: `--partition-key-path` in erforderlichen Parameter geändert</span><span class="sxs-lookup"><span data-stu-id="fc109-645">[BREAKING CHANGE] `az sql container create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="fc109-646">[BREAKING CHANGE] `az gremlin graph create`: `--partition-key-path` in erforderlichen Parameter geändert</span><span class="sxs-lookup"><span data-stu-id="fc109-646">[BREAKING CHANGE] `az gremlin graph create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="fc109-647">`az sql container create`: `--unique-key-policy` und `--conflict-resolution-policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-647">`az sql container create`: Added `--unique-key-policy` and `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="fc109-648">`az sql container create/update`: Aktualisierung des `--idx`-Standardschemas</span><span class="sxs-lookup"><span data-stu-id="fc109-648">`az sql container create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="fc109-649">`gremlin graph create`: `--conflict-resolution-policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-649">`gremlin graph create`: Added `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="fc109-650">`gremlin graph create/update`: Aktualisierung des `--idx`-Standardschemas</span><span class="sxs-lookup"><span data-stu-id="fc109-650">`gremlin graph create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="fc109-651">Tippfehler in Hilfemeldung korrigiert</span><span class="sxs-lookup"><span data-stu-id="fc109-651">Fixed typo in help message</span></span>
* <span data-ttu-id="fc109-652">Datenbank: Informationen zur eingestellten Unterstützung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-652">database: Added deprecation information</span></span>
* <span data-ttu-id="fc109-653">Auflistung: Informationen zur eingestellten Unterstützung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-653">collection: Added deprecation information</span></span>

### <a name="iot"></a><span data-ttu-id="fc109-654">IoT</span><span class="sxs-lookup"><span data-stu-id="fc109-654">IoT</span></span>

* <span data-ttu-id="fc109-655">Neuer Routingquelltyp hinzugefügt: DigitalTwinChangeEvents</span><span class="sxs-lookup"><span data-stu-id="fc109-655">Added new routing source type: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="fc109-656">Fehlende Features in `az iot hub create` behoben</span><span class="sxs-lookup"><span data-stu-id="fc109-656">Fixed missing features in `az iot hub create`</span></span>

### <a name="key-vault"></a><span data-ttu-id="fc109-657">Key Vault</span><span class="sxs-lookup"><span data-stu-id="fc109-657">Key Vault</span></span>

* <span data-ttu-id="fc109-658">Ein unerwarteter Fehler wurde behoben, bei dem keine Zertifikatdatei vorhanden war.</span><span class="sxs-lookup"><span data-stu-id="fc109-658">Fixed an unexpected error when certificate file does not exist</span></span>
* <span data-ttu-id="fc109-659">Funktionsunfähigkeit von `az keyvault recover/purge` behoben</span><span class="sxs-lookup"><span data-stu-id="fc109-659">Fixed `az keyvault recover/purge` not working</span></span>

### <a name="netappfiles"></a><span data-ttu-id="fc109-660">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="fc109-660">NetAppFiles</span></span>

* <span data-ttu-id="fc109-661">„azure-mgmt-netapp“ wurde auf 0.6.0 aktualisiert, um API-Version 2019-07-01 zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="fc109-661">Upgraded azure-mgmt-netapp to 0.6.0 to use API version 2019-07-01.</span></span> <span data-ttu-id="fc109-662">Diese neue API-Version umfasst:</span><span class="sxs-lookup"><span data-stu-id="fc109-662">This new API version includes:</span></span>

    - <span data-ttu-id="fc109-663">Volumeerstellung `--protocol-types` akzeptiert jetzt „NFSv4.1“ anstelle von „NFSv4“.</span><span class="sxs-lookup"><span data-stu-id="fc109-663">Volume creation `--protocol-types` accepts now "NFSv4.1" not "NFSv4"</span></span>
    - <span data-ttu-id="fc109-664">Die Richtlinie der Volumeexportrichtlinie heißt jetzt „nfsv41“ anstelle von „nfsv4“.</span><span class="sxs-lookup"><span data-stu-id="fc109-664">Volume export policy property now named 'nfsv41' not 'nfsv4'</span></span>
    - <span data-ttu-id="fc109-665">Volume `--creation-token` wurde in `--file-path` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="fc109-665">Volume `--creation-token` renamed to `--file-path`</span></span>
    - <span data-ttu-id="fc109-666">Das Erstellungsdatum einer Momentaufnahme heißt jetzt einfach „erstellt“.</span><span class="sxs-lookup"><span data-stu-id="fc109-666">Snapshot creation date now named just 'created'</span></span>

### <a name="network"></a><span data-ttu-id="fc109-667">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="fc109-667">Network</span></span>

* <span data-ttu-id="fc109-668">`az network private-dns link vnet create/update`: Unterstützung für mandantenübergreifende Verknüpfung virtueller Netzwerke.</span><span class="sxs-lookup"><span data-stu-id="fc109-668">`az network private-dns link vnet create/update`: Support cross-tenant virtual network linking.</span></span>
* <span data-ttu-id="fc109-669">[BREAKING CHANGE] `az network vnet subnet list`: `--resource-group` und `--vnet-name` wurden geändert und sind jetzt erforderlich.</span><span class="sxs-lookup"><span data-stu-id="fc109-669">[BREAKING CHANGE] `az network vnet subnet list`: Changed `--resource-group` and `--vnet-name` to be required now.</span></span>
* <span data-ttu-id="fc109-670">`az network public-ip prefix create`: Unterstützung der Angabe der IP-Adressversion (IPv4, IPv6) bei der Erstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-670">`az network public-ip prefix create`: Added support to specify IP address version (IPv4, IPv6) when creation</span></span>
* <span data-ttu-id="fc109-671">„azure-mgmt-network“ auf 7.0.0 und „api-version“ auf 2019-09-01 festgelegt</span><span class="sxs-lookup"><span data-stu-id="fc109-671">Bumped azure-mgmt-network to 7.0.0 and api-version to 2019-09-01</span></span>
* <span data-ttu-id="fc109-672">`az network vrouter`: Unterstützung für neuen virtuellen Dienstrouter und virtuelles Routerpeering hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-672">`az network vrouter`: Added support for new service virtual router and virtual router peering</span></span>
* <span data-ttu-id="fc109-673">`az network express-route gateway connection`: Unterstützung für `--internet-security` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-673">`az network express-route gateway connection`: Added support for `--internet-security`</span></span>

### <a name="profile"></a><span data-ttu-id="fc109-674">Profil</span><span class="sxs-lookup"><span data-stu-id="fc109-674">Profile</span></span>

* <span data-ttu-id="fc109-675">Funktionsunfähigkeit von `az account get-access-token --resource-type ms-graph` behoben</span><span class="sxs-lookup"><span data-stu-id="fc109-675">Fixed `az account get-access-token --resource-type ms-graph` not working</span></span>
* <span data-ttu-id="fc109-676">Warnung aus `az login` entfernt</span><span class="sxs-lookup"><span data-stu-id="fc109-676">Removed warning from `az login`</span></span>

### <a name="rbac"></a><span data-ttu-id="fc109-677">RBAC</span><span class="sxs-lookup"><span data-stu-id="fc109-677">RBAC</span></span>

* <span data-ttu-id="fc109-678">Funktionsunfähigkeit von `az ad app update --id {} --display-name {}` behoben</span><span class="sxs-lookup"><span data-stu-id="fc109-678">Fixed `az ad app update --id {} --display-name {}` doesn't work</span></span>

### <a name="servicefabric"></a><span data-ttu-id="fc109-679">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="fc109-679">ServiceFabric</span></span>

* <span data-ttu-id="fc109-680">`az sf cluster create`: Ein Problem wurde behoben, indem die Compute-VMSS von „template.json“ für Service Fabric unter Linux und Windows von Standarddatenträgern auf verwaltete Datenträger umgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="fc109-680">`az sf cluster create`: Fixed an issue by modifying service fabric linux and windows template.json compute vmss from standard to managed disks</span></span>

### <a name="sql"></a><span data-ttu-id="fc109-681">SQL</span><span class="sxs-lookup"><span data-stu-id="fc109-681">SQL</span></span>

* <span data-ttu-id="fc109-682">Die Parameter `--compute-model`, `--auto-pause-delay` und `--min-capacity` wurden hinzugefügt, um CRUD-Vorgänge für das neue SQL-Datenbank-Angebot zu unterstützen: Serverloses Computemodell.</span><span class="sxs-lookup"><span data-stu-id="fc109-682">Added `--compute-model`, `--auto-pause-delay`, and `--min-capacity` parameters to support CRUD operations for new SQL Database offering: Serverless compute model.</span></span>

### <a name="storage"></a><span data-ttu-id="fc109-683">Storage</span><span class="sxs-lookup"><span data-stu-id="fc109-683">Storage</span></span>

* <span data-ttu-id="fc109-684">`az storage account create/update`: Parameter „--enable-files-adds“ und Azure Active Directory-Eigenschaftenargumentgruppe hinzugefügt, um Active Directory Domain-Dienstauthentifizierung für Azure Files zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="fc109-684">`az storage account create/update`: Added --enable-files-adds parameter and Azure Active Directory Properties Argument group to support Azure Files Active Directory Domain Service Authentication</span></span>
* <span data-ttu-id="fc109-685">`az storage account keys list/renew` wurde erweitert, um die Auflistung oder erneute Generierung von Kerberos-Schlüsseln des Speicherkontos zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="fc109-685">Expanded `az storage account keys list/renew` to support listing or regenerating Kerberos keys of storage account.</span></span>

## <a name="october-15-2019"></a><span data-ttu-id="fc109-686">15. Oktober 2019</span><span class="sxs-lookup"><span data-stu-id="fc109-686">October 15, 2019</span></span>

<span data-ttu-id="fc109-687">Version 2.0.75</span><span class="sxs-lookup"><span data-stu-id="fc109-687">Version 2.0.75</span></span>

### <a name="aks"></a><span data-ttu-id="fc109-688">AKS</span><span class="sxs-lookup"><span data-stu-id="fc109-688">AKS</span></span>

* <span data-ttu-id="fc109-689">Standardwert `--load-balancer-sku` in `standard` geändert, sofern von der Kubernetes-Version unterstützt</span><span class="sxs-lookup"><span data-stu-id="fc109-689">Changed `--load-balancer-sku` default value to `standard` if supported by the kubernetes version</span></span>
* <span data-ttu-id="fc109-690">Standardwert `--vm-set-type` in `virtualmachinescalesets` geändert, sofern von der Kubernetes-Version unterstützt</span><span class="sxs-lookup"><span data-stu-id="fc109-690">Changed `--vm-set-type` default value to `virtualmachinescalesets` if supported by the kubernetes version</span></span>

### <a name="ams"></a><span data-ttu-id="fc109-691">AMS</span><span class="sxs-lookup"><span data-stu-id="fc109-691">AMS</span></span>

* <span data-ttu-id="fc109-692">[BREAKING CHANGE] Name von `job start` in `job create` geändert</span><span class="sxs-lookup"><span data-stu-id="fc109-692">[BREAKING CHANGE] Changed the name of `job start` to `job create`</span></span>
* <span data-ttu-id="fc109-693">[BREAKING CHANGE] Parameter `--ask` von `content-key-policy create` geändert, sodass eine hexadezimale Zeichenfolge mit 32 Zeichen anstelle von UTF8 verwendet wird</span><span class="sxs-lookup"><span data-stu-id="fc109-693">[BREAKING CHANGE] Changed the `--ask` parameter of `content-key-policy create` to use a 32-character hex string instead of UTF8</span></span>

### <a name="appservice"></a><span data-ttu-id="fc109-694">AppService</span><span class="sxs-lookup"><span data-stu-id="fc109-694">AppService</span></span>

* <span data-ttu-id="fc109-695">Befehle vom Typ `webapp config access-restriction show|set|add|remove` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-695">Added commands `webapp config access-restriction show|set|add|remove`</span></span>
* <span data-ttu-id="fc109-696">Bessere Fehlerbehandlung zu `webapp up` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-696">Added better error handling to `webapp up`</span></span>
* <span data-ttu-id="fc109-697">Unterstützung für SKU `Isolated` zu `appservice plan update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-697">Added support for `Isolated` SKU to `appservice plan update`</span></span>

### <a name="arm"></a><span data-ttu-id="fc109-698">ARM</span><span class="sxs-lookup"><span data-stu-id="fc109-698">ARM</span></span>

* <span data-ttu-id="fc109-699">Parameter `--handle-extended-json-format` zu `deployment create` hinzugefügt, um mehrere Zeilen und Kommentare in der JSON-Vorlage zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="fc109-699">Added `--handle-extended-json-format` parameter `deployment create` to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="fc109-700">Compute</span><span class="sxs-lookup"><span data-stu-id="fc109-700">Compute</span></span>

* <span data-ttu-id="fc109-701">Parameter `--enable-agent` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-701">Added `--enable-agent` parameter to `vm create`</span></span>
* <span data-ttu-id="fc109-702">`vm create` geändert, um bei der Verwendung von Zonen die SKU „Standard“ für die öffentliche IP-Adresse zu verwenden</span><span class="sxs-lookup"><span data-stu-id="fc109-702">Changed `vm create` to use standard public IP SKU automatically when using zones</span></span>
* <span data-ttu-id="fc109-703">`vm create` geändert, um automatisch einen gültigen Computernamen für eine VM zu erstellen, falls keiner angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="fc109-703">Changed `vm create` to automatically create a valid computer name for a VM if none is provided</span></span>
* <span data-ttu-id="fc109-704">Parameter `--computer-name-prefix` zu `vmss create` hinzugefügt, um das benutzerdefinierte Computernamenspräfix virtueller Computer in VMSS zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="fc109-704">Added `--computer-name-prefix` parameter to `vmss create` to support custom computer name prefix of virtual machines in the VMSS</span></span>
* <span data-ttu-id="fc109-705">Parameter `--workspace` zu `vm create` hinzugefügt, um automatisch einen Log Analytics-Arbeitsbereich zu aktivieren</span><span class="sxs-lookup"><span data-stu-id="fc109-705">Add `--workspace` parameter to `vm create` to enable log analytics workspace automatically</span></span>
* <span data-ttu-id="fc109-706">API-Version für Kataloge auf 2019-07-01 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="fc109-706">Updated galleries API version to 2019-07-01</span></span>

### <a name="core"></a><span data-ttu-id="fc109-707">Core</span><span class="sxs-lookup"><span data-stu-id="fc109-707">Core</span></span>

* <span data-ttu-id="fc109-708">Syntaxprüfung für Parameter `--set` im generischen Updatebefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-708">Added syntax check for `--set` parameter in generic update command</span></span>

### <a name="iot"></a><span data-ttu-id="fc109-709">IoT</span><span class="sxs-lookup"><span data-stu-id="fc109-709">IoT</span></span>

* <span data-ttu-id="fc109-710">Problem behoben, bei dem für `iot hub show` der Fehler „Ressource nicht gefunden.“ zurückgegeben wurde</span><span class="sxs-lookup"><span data-stu-id="fc109-710">Fixed an issue where `iot hub show` would incorrectly error with "resource not found"</span></span>

### <a name="monitor"></a><span data-ttu-id="fc109-711">Überwachen</span><span class="sxs-lookup"><span data-stu-id="fc109-711">Monitor</span></span>

* <span data-ttu-id="fc109-712">Unterstützung für CRUD zu `monitor log-analytics workspace` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-712">Added support for CRUD to `monitor log-analytics workspace`</span></span>

### <a name="network"></a><span data-ttu-id="fc109-713">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="fc109-713">Network</span></span>

* <span data-ttu-id="fc109-714">Unterstützung für mandantenübergreifende virtuelle Verbindung zu `network private-dns link vnet [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-714">Added support for cross-tenant virtual linking to `network private-dns link vnet [create|update]`</span></span>
* <span data-ttu-id="fc109-715">[BREAKING CHANGE]`network vnet subnet list` geändert, um Parameter `--resource-group` und `--vnet-name` vorauszusetzen</span><span class="sxs-lookup"><span data-stu-id="fc109-715">[BREAKING CHANGE] Changed `network vnet subnet list` to require `--resource-group` and `--vnet-name` parameters</span></span>

### <a name="sql"></a><span data-ttu-id="fc109-716">SQL</span><span class="sxs-lookup"><span data-stu-id="fc109-716">SQL</span></span>

* <span data-ttu-id="fc109-717">Befehle zu `sql mi ad-admin` hinzugefügt, die das Festlegen eines AAD-Administrators für verwaltete Instanzen unterstützen</span><span class="sxs-lookup"><span data-stu-id="fc109-717">Added commands to `sql mi ad-admin` that support setting an AAD administrator on managed instances</span></span>

### <a name="storage"></a><span data-ttu-id="fc109-718">Storage</span><span class="sxs-lookup"><span data-stu-id="fc109-718">Storage</span></span>

* <span data-ttu-id="fc109-719">Parameter `--preserve-s2s-access-tier` zu `storage copy` hinzugefügt, um die Zugriffsebene beim Kopieren von Dienst zu Dienst beizubehalten</span><span class="sxs-lookup"><span data-stu-id="fc109-719">Added `--preserve-s2s-access-tier` parameter `storage copy` to preserve access tier during service to service copy</span></span>
* <span data-ttu-id="fc109-720">Parameter `--enable-large-file-share` zu `storage account [create|update]` hinzugefügt, um große Dateifreigaben für ein Speicherkonto zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="fc109-720">Added `--enable-large-file-share` parameter to `storage account [create|update]` to support large file shares for storage account</span></span>

## <a name="september-24-2019"></a><span data-ttu-id="fc109-721">24. September 2019</span><span class="sxs-lookup"><span data-stu-id="fc109-721">September 24, 2019</span></span>

<span data-ttu-id="fc109-722">Version 2.0.74</span><span class="sxs-lookup"><span data-stu-id="fc109-722">Version 2.0.74</span></span>

### <a name="acr"></a><span data-ttu-id="fc109-723">ACR</span><span class="sxs-lookup"><span data-stu-id="fc109-723">ACR</span></span>

* <span data-ttu-id="fc109-724">Erforderlicher Parameter `--type` zu `acr config retention update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-724">Added a required `--type` parameter to `acr config retention update`</span></span>
* <span data-ttu-id="fc109-725">[BREAKING CHANGE] Umbenannter Parameter `--name -n` in `--registry -r ` für Befehlsgruppe `acr config` geändert</span><span class="sxs-lookup"><span data-stu-id="fc109-725">[BREAKING CHANGE] Renamed parameter `--name -n` changed to `--registry -r ` for `acr config` command group</span></span>

### <a name="aks"></a><span data-ttu-id="fc109-726">AKS</span><span class="sxs-lookup"><span data-stu-id="fc109-726">AKS</span></span>

* <span data-ttu-id="fc109-727">Parameter `--load-balancer-sku` zum Befehl `aks create` hinzugefügt, um die Erstellung von AKS-Clustern mit SLB zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="fc109-727">Added `--load-balancer-sku` parameter to `aks create` command, which allows for creating AKS cluster with SLB</span></span>
* <span data-ttu-id="fc109-728">Parameter `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` und `--load-balancer-outbound-ip-prefixes` zu den Befehlen `aks [create|update]` hinzugefügt,um die Aktualisierung des Lastenausgleichsprofils eines AKS-Clusters mit SLB zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="fc109-728">Added `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` and `--load-balancer-outbound-ip-prefixes` parameters to `aks [create|update]` commands, which allow for updating load balancer profile of an AKS cluster with SLB</span></span>
* <span data-ttu-id="fc109-729">Parameter `--vm-set-type` zum Befehl `aks create` hinzugefügt, um die Angabe von VM-Typen eines AKS-Clusters (vmas oder vmss) zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="fc109-729">Added `--vm-set-type` parameter to `aks create` command, which allows to specify vm types of an AKS Cluster (vmas or vmss)</span></span>

### <a name="arm"></a><span data-ttu-id="fc109-730">ARM</span><span class="sxs-lookup"><span data-stu-id="fc109-730">ARM</span></span>

* <span data-ttu-id="fc109-731">Parameter `--handle-extended-json-format` zum Befehl `group deployment create` hinzugefügt, um mehrere Zeilen und Kommentare in der JSON-Vorlage zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="fc109-731">Added `--handle-extended-json-format` parameter to `group deployment create` command to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="fc109-732">Compute</span><span class="sxs-lookup"><span data-stu-id="fc109-732">Compute</span></span>

* <span data-ttu-id="fc109-733">Parameter `--terminate-notification-time` zu den Befehlen `vmss [create|update]` hinzugefügt, um die Konfigurierbarkeit der Beendigung geplanter Ereignisse zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="fc109-733">Added `--terminate-notification-time` parameter to `vmss [create|update]` commands to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="fc109-734">Parameter `--enable-terminate-notification` zu den Befehlen `vmss update` hinzugefügt, um die Konfigurierbarkeit der Beendigung geplanter Ereignisse zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="fc109-734">Added `--enable-terminate-notification` parameter to `vmss update` command to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="fc109-735">Parameter `--priority,` `--eviction-policy,` `--max-billing` zu `[vm|vmss] create`-Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-735">Added `--priority,` `--eviction-policy,` `--max-billing` parameters to `[vm|vmss] create` commands</span></span>
* <span data-ttu-id="fc109-736">`disk create` geändert, um die Angabe der genauen Größe des Datenträgeruploads zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="fc109-736">Changed `disk create` to allow specifying the exact size of the disk upload</span></span>
* <span data-ttu-id="fc109-737">Unterstützung für inkrementelle Momentaufnahmen für verwaltete Datenträger zu `snapshot create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-737">Added support for incremental snapshots for managed disks to `snapshot create`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="fc109-738">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="fc109-738">Cosmos DB</span></span>

* <span data-ttu-id="fc109-739">Parameter `--type <key-type>` zum Befehl `cosmosdb keys list` hinzugefügt, um Schlüssel, schreibgeschützte Schlüssel oder Verbindungszeichenfolgen anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="fc109-739">Added `--type <key-type>` parameter to `cosmosdb keys list` command to show key, read only keys or connection strings</span></span>
* <span data-ttu-id="fc109-740">Befehl `cosmosdb keys regenerate` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-740">Added `cosmosdb keys regenerate` command</span></span>
* <span data-ttu-id="fc109-741">[VERALTET] Befehle `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` und `cosmosdb list-read-only-keys` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="fc109-741">[DEPRECATED] Deprecated `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` and `cosmosdb list-read-only-keys` commands</span></span>

### <a name="eventgrid"></a><span data-ttu-id="fc109-742">EventGrid</span><span class="sxs-lookup"><span data-stu-id="fc109-742">EventGrid</span></span>

* <span data-ttu-id="fc109-743">Endpunkthilfetext korrigiert, um auf den richtigen Parameter zu verweisen</span><span class="sxs-lookup"><span data-stu-id="fc109-743">Fixed the endpoint help text to refer to the right parameter</span></span>

### <a name="key-vault"></a><span data-ttu-id="fc109-744">Key Vault</span><span class="sxs-lookup"><span data-stu-id="fc109-744">Key Vault</span></span>

* <span data-ttu-id="fc109-745">Problem behoben, aufgrund dessen die Anmeldung mit einem Mandanten (`login -t`) unter Umständen zu einem Fehler von `keyvault create` führte</span><span class="sxs-lookup"><span data-stu-id="fc109-745">Fixed issue where logging in with a tenant (`login -t`) could cause `keyvault create` to fail</span></span>

### <a name="monitor"></a><span data-ttu-id="fc109-746">Überwachen</span><span class="sxs-lookup"><span data-stu-id="fc109-746">Monitor</span></span>

* <span data-ttu-id="fc109-747">Problem behoben, aufgrund dessen das Zeichen `:` in `--condition` für `monitor metrics alert create` nicht zulässig war</span><span class="sxs-lookup"><span data-stu-id="fc109-747">Fixed issue where `:` character was not allowed in `--condition` argument to `monitor metrics alert create`</span></span>

### <a name="policy"></a><span data-ttu-id="fc109-748">Richtlinie</span><span class="sxs-lookup"><span data-stu-id="fc109-748">Policy</span></span>

* <span data-ttu-id="fc109-749">Unterstützung für Policy-API-Version 2019-06-01 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-749">Added support for Policy API version 2019-06-01</span></span>
* <span data-ttu-id="fc109-750">Parameter `--enforcement-mode` zum Befehl `policy assignment create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-750">Added `--enforcement-mode` parameter to `policy assignment create` command</span></span>

### <a name="storage"></a><span data-ttu-id="fc109-751">Storage</span><span class="sxs-lookup"><span data-stu-id="fc109-751">Storage</span></span>

* <span data-ttu-id="fc109-752">Parameter `--blob-type` zum Befehl `az storage copy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-752">Added `--blob-type` parameter to `az storage copy` command</span></span>

## <a name="september-10-2019"></a><span data-ttu-id="fc109-753">10. September 2019</span><span class="sxs-lookup"><span data-stu-id="fc109-753">September 10, 2019</span></span>

### <a name="acr"></a><span data-ttu-id="fc109-754">ACR</span><span class="sxs-lookup"><span data-stu-id="fc109-754">ACR</span></span>

* <span data-ttu-id="fc109-755">Befehlsgruppe `acr config retention` zum Konfigurieren der Aufbewahrungsrichtlinie hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-755">Added command group `acr config retention` to configure retention policy</span></span>

### <a name="aks"></a><span data-ttu-id="fc109-756">AKS</span><span class="sxs-lookup"><span data-stu-id="fc109-756">AKS</span></span>

* <span data-ttu-id="fc109-757">Unterstützung für die ACR-Integration mit den folgenden Befehlen hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="fc109-757">Added support for ACR integration with the following commands:</span></span>
  * <span data-ttu-id="fc109-758">Parameter `--attach-acr` zu `aks [create|update]` hinzugefügt, um einen ACR an einen AKS-Cluster anzufügen</span><span class="sxs-lookup"><span data-stu-id="fc109-758">Added `--attach-acr` parameter to `aks [create|update]` to attach an ACR to an AKS cluster</span></span>
  * <span data-ttu-id="fc109-759">Parameter `--detach-acr` zu `aks update` hinzugefügt, um den ACR von einem AKS-Cluster zu trennen</span><span class="sxs-lookup"><span data-stu-id="fc109-759">Added `--detach-acr` parameter to `aks update` to detach the ACR from an AKS cluster</span></span>

### <a name="arm"></a><span data-ttu-id="fc109-760">ARM</span><span class="sxs-lookup"><span data-stu-id="fc109-760">ARM</span></span>

* <span data-ttu-id="fc109-761">Zur Verwendung der API-Version 2019-05-10 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="fc109-761">Updated to use API version 2019-05-10</span></span>

### <a name="batch"></a><span data-ttu-id="fc109-762">Batch</span><span class="sxs-lookup"><span data-stu-id="fc109-762">Batch</span></span>

* <span data-ttu-id="fc109-763">Neue JSON-Konfigurationseinstellungen für `batch pool create` zu `--json-file` hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="fc109-763">Added new JSON configuration settings to `--json-file` for `batch pool create`:</span></span>
  * <span data-ttu-id="fc109-764">`MountConfigurations` für Dateisystemeinbindungen hinzugefügt (Details siehe https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body )</span><span class="sxs-lookup"><span data-stu-id="fc109-764">Added `MountConfigurations` for file system mounts (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
  * <span data-ttu-id="fc109-765">Optionale Eigenschaft `publicIPs` in `NetworkConfiguration` für öffentliche IP-Adressen für Pools hinzugefügt (Details siehe https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body )</span><span class="sxs-lookup"><span data-stu-id="fc109-765">Added optional property `publicIPs` on `NetworkConfiguration` for public IPs on pools (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
* <span data-ttu-id="fc109-766">Unterstützung für Kataloge mit freigegebenen Images zu `--image` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-766">Added support for shared image galleries to `--image`</span></span>
* <span data-ttu-id="fc109-767">[BREAKING CHANGE] Standardwert von `--start-task-wait-for-success` für `batch pool create` in `true` geändert</span><span class="sxs-lookup"><span data-stu-id="fc109-767">[BREAKING CHANGE] Changed default value of `--start-task-wait-for-success` on `batch pool create` to be `true`</span></span>
* <span data-ttu-id="fc109-768">[BREAKING CHANGE] Standardwert von `Scope` für `AutoUserSpecification` geändert, damit immer „Pool“ verwendet wird (vormals `Task` für Windows-Knoten bzw. `Pool` für Linux-Knoten)</span><span class="sxs-lookup"><span data-stu-id="fc109-768">[BREAKING CHANGE] Changed default value for `Scope` on `AutoUserSpecification` to always be Pool (was `Task` on Windows nodes, `Pool` on Linux nodes)</span></span>
  * <span data-ttu-id="fc109-769">Dieses Argument kann nur über eine JSON-Konfiguration mit `--json-file` festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="fc109-769">This argument can only be set from a JSON configuration with `--json-file`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="fc109-770">HDInsight</span><span class="sxs-lookup"><span data-stu-id="fc109-770">HDInsight</span></span>

* <span data-ttu-id="fc109-771">Allgemein verfügbares Release</span><span class="sxs-lookup"><span data-stu-id="fc109-771">GA release</span></span>
* <span data-ttu-id="fc109-772">[BREAKING CHANGE] Parameter `--workernode-count/-c` von `az hdinsight resize` in erforderlich geändert</span><span class="sxs-lookup"><span data-stu-id="fc109-772">[BREAKING CHANGE] Changed parameter `--workernode-count/-c` of `az hdinsight resize` to be required.</span></span>

### <a name="key-vault"></a><span data-ttu-id="fc109-773">Key Vault</span><span class="sxs-lookup"><span data-stu-id="fc109-773">Key Vault</span></span>

* <span data-ttu-id="fc109-774">Problem behoben, aufgrund dessen Subnetze nicht aus Netzwerkregeln gelöscht werden konnten</span><span class="sxs-lookup"><span data-stu-id="fc109-774">Fixed issue where subnets couldn't be deleted from network rules</span></span>
* <span data-ttu-id="fc109-775">Problem behoben, aufgrund dessen doppelte Subnetze und IP-Adressen zu Netzwerkregeln hinzugefügt werden konnten</span><span class="sxs-lookup"><span data-stu-id="fc109-775">Fixed issue where duplicated subnets and IP addresses could be added to network rules</span></span>

### <a name="network"></a><span data-ttu-id="fc109-776">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="fc109-776">Network</span></span>

* <span data-ttu-id="fc109-777">Parameter `--interval` zu `network watcher flow-log` hinzugefügt, um den Wert für das Intervall der Datenverkehrsanalyse festzulegen</span><span class="sxs-lookup"><span data-stu-id="fc109-777">Added `--interval` parameter to `network watcher flow-log` to set traffic analysis interval value</span></span>
* <span data-ttu-id="fc109-778">`network application-gateway identity` zum Verwalten der Gatewayidentität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-778">Added `network application-gateway identity` to manage gateway identity</span></span>
* <span data-ttu-id="fc109-779">Unterstützung zum Festlegen der Key Vault-ID zu `network application-gateway ssl-cert` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-779">Added support for setting Key Vault ID to `network application-gateway ssl-cert`</span></span>
* <span data-ttu-id="fc109-780">`network express-route peering peer-connection [show|list]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-780">Added `network express-route peering peer-connection [show|list]`</span></span>

### <a name="policy"></a><span data-ttu-id="fc109-781">Richtlinie</span><span class="sxs-lookup"><span data-stu-id="fc109-781">Policy</span></span>

* <span data-ttu-id="fc109-782">Zur Verwendung der API-Version 2019-01-01 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="fc109-782">Updated to use API version 2019-01-01</span></span>

## <a name="august-27-2019"></a><span data-ttu-id="fc109-783">27. August 2019</span><span class="sxs-lookup"><span data-stu-id="fc109-783">August 27, 2019</span></span>

<span data-ttu-id="fc109-784">Version 2.0.72</span><span class="sxs-lookup"><span data-stu-id="fc109-784">Version 2.0.72</span></span>

### <a name="acr"></a><span data-ttu-id="fc109-785">ACR</span><span class="sxs-lookup"><span data-stu-id="fc109-785">ACR</span></span>

* <span data-ttu-id="fc109-786">[BREAKING CHANGE] Unterstützung für SKU `classic` entfernt</span><span class="sxs-lookup"><span data-stu-id="fc109-786">[BREAKING CHANGE] Removed support for the `classic` SKU</span></span>

### <a name="api-management"></a><span data-ttu-id="fc109-787">API Management</span><span class="sxs-lookup"><span data-stu-id="fc109-787">API Management</span></span>

* <span data-ttu-id="fc109-788">[VORSCHAU] Befehlsgruppe `apim` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-788">[PREVIEW] Added `apim` command group</span></span>

### <a name="appservice"></a><span data-ttu-id="fc109-789">AppService</span><span class="sxs-lookup"><span data-stu-id="fc109-789">AppService</span></span>

* <span data-ttu-id="fc109-790">Problem mit dem Befehl `webapp webjob continuous start` bei Angabe eines Slots behoben</span><span class="sxs-lookup"><span data-stu-id="fc109-790">Fixed issue with `webapp webjob continuous start` command when specifying a slot</span></span>
* <span data-ttu-id="fc109-791">`webapp up` geändert, um den Ordner `env` zu erkennen und aus der für die Bereitstellung verwendeten Datei zu entfernen</span><span class="sxs-lookup"><span data-stu-id="fc109-791">Changed `webapp up` to detect `env` folder and remove it from the file used for deployment</span></span>

### <a name="keyvault"></a><span data-ttu-id="fc109-792">KeyVault</span><span class="sxs-lookup"><span data-stu-id="fc109-792">Keyvault</span></span>

* <span data-ttu-id="fc109-793">Fehler in `keyvault secret set` behoben, aufgrund dessen das Argument `--expires` ignoriert wurde</span><span class="sxs-lookup"><span data-stu-id="fc109-793">Fixed a bug in `keyvault secret set` that igored the `--expires` argument</span></span>

### <a name="network"></a><span data-ttu-id="fc109-794">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="fc109-794">Network</span></span>

* <span data-ttu-id="fc109-795">Unterstützung für IPv6-Adressen zu Argumenten vom Typ `--private-ip-address-version` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-795">Added support for IPv6 addresses to `--private-ip-address-version` arguments</span></span>
* <span data-ttu-id="fc109-796">Neue Befehle vom Typ `network private-endpoint [create|update|list-types]` für die Verwaltung privater Endpunkte hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-796">Added new commands `network private-endpoint [create|update|list-types]` for private endpoint management</span></span>
* <span data-ttu-id="fc109-797">Befehlsgruppe `network private-link-service` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-797">Added command group `network private-link-service`</span></span>
* <span data-ttu-id="fc109-798">Argumente `--private-endpoint-network-policies` und `--private-link-service-network-policies` zu `network vnet subnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-798">Added `--private-endpoint-network-policies` and `--private-link-service-network-policies` arguments to `network vnet subnet update`</span></span>

### <a name="rbac"></a><span data-ttu-id="fc109-799">RBAC</span><span class="sxs-lookup"><span data-stu-id="fc109-799">RBAC</span></span>

* <span data-ttu-id="fc109-800">Problem mit `ad app update --homepage` behoben, aufgrund dessen die Startseite nicht aktualisiert wurde</span><span class="sxs-lookup"><span data-stu-id="fc109-800">Fixed issue with `ad app update --homepage` where homepage would not be updated</span></span>

### <a name="servicefabric"></a><span data-ttu-id="fc109-801">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="fc109-801">ServiceFabric</span></span>

* <span data-ttu-id="fc109-802">Unterstützung für Key Vault-Namen mit Groß- und Kleinschreibung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-802">Added support for mixed-case Key Vault names</span></span>
* <span data-ttu-id="fc109-803">Problem bei der Verwendung von Zertifikaten in Key Vault behoben</span><span class="sxs-lookup"><span data-stu-id="fc109-803">Fixed issue when using certificates in Key Vault</span></span>
* <span data-ttu-id="fc109-804">Problem bei der Verwendung von PFX-Zertifikatdateien behoben</span><span class="sxs-lookup"><span data-stu-id="fc109-804">Fixed issue with using PFX certificate files</span></span>
* <span data-ttu-id="fc109-805">Problem mit `sf cluster certificate add` behoben, wenn keine Key Vault-Ressourcengruppe angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="fc109-805">Fixed issue with `sf cluster certificate add` when Key Vault resource group wasn't specified</span></span>
* <span data-ttu-id="fc109-806">Problem behoben, aufgrund dessen `sf cluster set` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="fc109-806">Fixed issue with `sf cluster set` not working</span></span>

### <a name="signalr"></a><span data-ttu-id="fc109-807">SignalR</span><span class="sxs-lookup"><span data-stu-id="fc109-807">SignalR</span></span>

* <span data-ttu-id="fc109-808">Neue Befehle hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="fc109-808">Added new commands:</span></span>
  * <span data-ttu-id="fc109-809">`signalr cors`: Verwalten von CORS für SignalR</span><span class="sxs-lookup"><span data-stu-id="fc109-809">`signalr cors`: Manage SignalR CORS</span></span>
  * <span data-ttu-id="fc109-810">`signalr restart`: Starten eines SignalR-Diensts</span><span class="sxs-lookup"><span data-stu-id="fc109-810">`signalr restart`: Restart a SignalR service</span></span>
  * <span data-ttu-id="fc109-811">`signalr update`: Aktualisieren eines SignalR-Diensts</span><span class="sxs-lookup"><span data-stu-id="fc109-811">`signalr update`: Update a SignalR service</span></span>
* <span data-ttu-id="fc109-812">Argument `--service-mode` zu `signalr create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-812">Added `--service-mode` argument to `signalr create`</span></span>

### <a name="storage"></a><span data-ttu-id="fc109-813">Storage</span><span class="sxs-lookup"><span data-stu-id="fc109-813">Storage</span></span>

* <span data-ttu-id="fc109-814">Befehl `storage account revoke-delegation-keys` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-814">Added `storage account revoke-delegation-keys` command</span></span>

## <a name="august-13-2019"></a><span data-ttu-id="fc109-815">13. August 2019</span><span class="sxs-lookup"><span data-stu-id="fc109-815">August 13, 2019</span></span>

<span data-ttu-id="fc109-816">Version 2.0.71</span><span class="sxs-lookup"><span data-stu-id="fc109-816">Version 2.0.71</span></span>

### <a name="appservice"></a><span data-ttu-id="fc109-817">AppService</span><span class="sxs-lookup"><span data-stu-id="fc109-817">AppService</span></span>

* <span data-ttu-id="fc109-818">Problem behoben, aufgrund dessen bei Befehlen vom Typ `webapp webjob continuous` für Slots Fehler auftraten</span><span class="sxs-lookup"><span data-stu-id="fc109-818">Fixed issue where `webapp webjob continuous` commands were failing for slots</span></span>

### <a name="botservice"></a><span data-ttu-id="fc109-819">BotService</span><span class="sxs-lookup"><span data-stu-id="fc109-819">BotService</span></span>

* <span data-ttu-id="fc109-820">[BREAKING CHANGE] Unterstützung für die Erstellung von Bots der Version 3 entfernt</span><span class="sxs-lookup"><span data-stu-id="fc109-820">[BREAKING CHANGE] Removed support for creating v3 SDK bots</span></span>

### <a name="cognitiveservices"></a><span data-ttu-id="fc109-821">CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="fc109-821">CognitiveServices</span></span>

* <span data-ttu-id="fc109-822">Befehle vom Typ `cognitiveservices account network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-822">Added `cognitiveservices account network-rule` commands</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="fc109-823">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="fc109-823">Cosmos DB</span></span>

* <span data-ttu-id="fc109-824">Beim Aktualisieren mehrerer Schreibstandorte wurde eine Warnung entfernt.</span><span class="sxs-lookup"><span data-stu-id="fc109-824">Removed warning when updating multiple write locations</span></span>
* <span data-ttu-id="fc109-825">CRUD-Befehle für CosmosDB SQL-, MongoDB-, Cassandra-, Gremlin- und Tabellenressourcen sowie den Ressourcendurchsatz hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-825">Added CRUD commands for CosmosDB SQL, MongoDB, Cassandra, Gremlin and Table resources and resource's throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="fc109-826">HDInsight</span><span class="sxs-lookup"><span data-stu-id="fc109-826">HDInsight</span></span>

<span data-ttu-id="fc109-827">Dieses Release enthält zahlreiche wichtige Änderungen.</span><span class="sxs-lookup"><span data-stu-id="fc109-827">This release contains a large number of breaking changes.</span></span>

* <span data-ttu-id="fc109-828">[BREAKING CHANGE] Parameter für `hdinsight create` umbenannt:</span><span class="sxs-lookup"><span data-stu-id="fc109-828">[BREAKING CHANGE] Renamed parameters for `hdinsight create`:</span></span>
  * <span data-ttu-id="fc109-829">`--storage-default-container` in `--storage-container` umbenannt</span><span class="sxs-lookup"><span data-stu-id="fc109-829">Renamed `--storage-default-container` to `--storage-container`</span></span>
  * <span data-ttu-id="fc109-830">`--storage-default-filesystem` in `--storage-filesystem` umbenannt</span><span class="sxs-lookup"><span data-stu-id="fc109-830">Renamed `--storage-default-filesystem` to `--storage-filesystem`</span></span>
* <span data-ttu-id="fc109-831">[BREAKING CHANGE] Das Argument `--name` von `application create` wurde so geändert, dass es den Anwendungsnamen anstelle des Clusternamens darstellt.</span><span class="sxs-lookup"><span data-stu-id="fc109-831">[BREAKING CHANGE] Changed the `--name` argument of `application create` to represent the application name instead of the cluster name</span></span>
* <span data-ttu-id="fc109-832">Argument `--cluster-name` zu `application create` hinzugefügt, um die alte Funktion `--name` zu ersetzen</span><span class="sxs-lookup"><span data-stu-id="fc109-832">Added `--cluster-name` argument to `application create` to replace old `--name` functionality</span></span>
* <span data-ttu-id="fc109-833">[BREAKING CHANGE] Parameter für `application create` umbenannt:</span><span class="sxs-lookup"><span data-stu-id="fc109-833">[BREAKING CHANGE] Renamed parameters for `application create`:</span></span>
  * <span data-ttu-id="fc109-834">`--application-type` in `--type` umbenannt</span><span class="sxs-lookup"><span data-stu-id="fc109-834">Renamed `--application-type` to `--type`</span></span>
  * <span data-ttu-id="fc109-835">`--marketplace-identifier` in `--marketplace-id` umbenannt</span><span class="sxs-lookup"><span data-stu-id="fc109-835">Renamed `--marketplace-identifier` to `--marketplace-id`</span></span>
  * <span data-ttu-id="fc109-836">`--https-endpoint-access-mode` in `--access-mode` umbenannt</span><span class="sxs-lookup"><span data-stu-id="fc109-836">Renamed `--https-endpoint-access-mode` to `--access-mode`</span></span>
  * <span data-ttu-id="fc109-837">`--https-endpoint-destination-port` in `--destination-port` umbenannt</span><span class="sxs-lookup"><span data-stu-id="fc109-837">Renamed  `--https-endpoint-destination-port` to `--destination-port`</span></span>
* <span data-ttu-id="fc109-838">[BREAKING CHANGE] Parameter für `application create` entfernt:</span><span class="sxs-lookup"><span data-stu-id="fc109-838">[BREAKING CHANGE] Removed parameters for `application create`:</span></span>
  * `--https-endpoint-location`
  * `--https-endpoint-public-port`
  * `--ssh-endpoint-destination-port`
  * `--ssh-endpoint-location`
  * `--ssh-endpoint-public-port`
* <span data-ttu-id="fc109-839">[WICHTIGE ÄNDERUNG] `--target-instance-count` für `hdinsight resize` in `--workernode-count` umbenannt</span><span class="sxs-lookup"><span data-stu-id="fc109-839">[BREAKING CHNAGE] Renamed `--target-instance-count` to `--workernode-count` for `hdinsight resize`</span></span>
* <span data-ttu-id="fc109-840">[BREAKING CHANGE] Alle Befehle in der Gruppe `hdinsight script-action` wurden so geändert, dass sie den Parameter `--name` als Namen der Skriptaktion verwenden.</span><span class="sxs-lookup"><span data-stu-id="fc109-840">[BREAKING CHANGE] Changed all commands in the `hdinsight script-action` group to use the `--name` parameter as the name of the script action.</span></span>
* <span data-ttu-id="fc109-841">Argument `--cluster-name` zu allen Befehlen vom Typ `hdinsight script-action` hinzugefügt, um die alte Funktion `--name` zu ersetzen</span><span class="sxs-lookup"><span data-stu-id="fc109-841">Added `--cluster-name` argument to all `hdinsight script-action` commands to replace old `--name` functionality</span></span>
* <span data-ttu-id="fc109-842">[BREAKING CHANGE]`--script-execution-id` für alle Befehle vom Typ `hdinsight script-action` in `--execution-id` umbenannt</span><span class="sxs-lookup"><span data-stu-id="fc109-842">[BREAKING CHANGE] Renamed `--script-execution-id` to `--execution-id` for all `hdinsight script-action` commands</span></span>
* <span data-ttu-id="fc109-843">[BREAKING CHANGE]`hdinsight script-action show` in `hdinsight script-action show-execution-details` umbenannt</span><span class="sxs-lookup"><span data-stu-id="fc109-843">[BREAKING CHANGE] Renamed `hdinsight script-action show` to `hdinsight script-action show-execution-details`</span></span>
* <span data-ttu-id="fc109-844">[WICHTIGE ÄNDERUNG] Parameter in `hdinsight script-action execute --roles` geändert, sodass sie durch Leerzeichen anstelle von Kommas getrennt sind</span><span class="sxs-lookup"><span data-stu-id="fc109-844">[BREAKING CHNAGE] Changed parameters to `hdinsight script-action execute --roles` to be space-separated instead of comma-separated</span></span>
* <span data-ttu-id="fc109-845">[BREAKING CHANGE] Parameter `--persisted` für `hdinsight script-action list` entfernt</span><span class="sxs-lookup"><span data-stu-id="fc109-845">[BREAKING CHANGE] Removed the `--persisted` parameter of `hdinsight script-action list`</span></span>
* <span data-ttu-id="fc109-846">Der Parameter `hdinsight create --cluster-configurations` wurde so geändert, dass er einen Pfad zu einer lokalen JSON-Datei oder JSON-Zeichenfolge akzeptiert.</span><span class="sxs-lookup"><span data-stu-id="fc109-846">Changed the `hdinsight create --cluster-configurations` parameter to accept a path to a local JSON file or a JSON string</span></span>
* <span data-ttu-id="fc109-847">Befehl `hdinsight script-action list-execution-history` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-847">Added command `hdinsight script-action list-execution-history`</span></span>
* <span data-ttu-id="fc109-848">`hdinsight monitor enable --workspace` geändert, um die ID oder den Namen eines Log Analytics-Arbeitsbereichs zu akzeptieren</span><span class="sxs-lookup"><span data-stu-id="fc109-848">Changed `hdinsight monitor enable --workspace` to accept a Log Analytics workspace ID or workspace name</span></span>
* <span data-ttu-id="fc109-849">Argument `hdinsight monitor enable --primary-key` hinzugefügt. Dieses Argument wird benötigt, wenn eine Arbeitsbereichs-ID als Parameter angegeben wird.</span><span class="sxs-lookup"><span data-stu-id="fc109-849">Added the `hdinsight monitor enable --primary-key` argument, which is needed if a workspace ID is provided as the parameter</span></span>
* <span data-ttu-id="fc109-850">Weitere Beispiele und aktualisierte Beschreibungen für Hilfemeldungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-850">Added more examples and updated descriptions for help messages</span></span>

### <a name="interactive"></a><span data-ttu-id="fc109-851">Interactive</span><span class="sxs-lookup"><span data-stu-id="fc109-851">Interactive</span></span>

* <span data-ttu-id="fc109-852">Ladefehler behoben</span><span class="sxs-lookup"><span data-stu-id="fc109-852">Fixed a loading error</span></span>

### <a name="kubernetes"></a><span data-ttu-id="fc109-853">Kubernetes</span><span class="sxs-lookup"><span data-stu-id="fc109-853">Kubernetes</span></span>

* <span data-ttu-id="fc109-854">Änderung, um `https` zu verwenden, wenn der Dashboardcontainerport `https` verwendet</span><span class="sxs-lookup"><span data-stu-id="fc109-854">Changed to use `https` if dashboard container port is using `https`</span></span>

### <a name="network"></a><span data-ttu-id="fc109-855">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="fc109-855">Network</span></span>

* <span data-ttu-id="fc109-856">Argument `--yes` hinzugefügt zu `network dns record-set cname delete`</span><span class="sxs-lookup"><span data-stu-id="fc109-856">Added `--yes` argument `network dns record-set cname delete`</span></span>

### <a name="profile"></a><span data-ttu-id="fc109-857">Profil</span><span class="sxs-lookup"><span data-stu-id="fc109-857">Profile</span></span>

* <span data-ttu-id="fc109-858">Argument `--resource-type` zu `account get-access-token` zum Abrufen von Ressourcenzugriffstoken hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-858">Added `--resource-type` argument to `account get-access-token` to get resource access tokens</span></span>

### <a name="servicefabric"></a><span data-ttu-id="fc109-859">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="fc109-859">ServiceFabric</span></span>

* <span data-ttu-id="fc109-860">Alle unterstützten Betriebssystemversionen für „sf cluster create“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-860">Added all supported os version for sf cluster create</span></span>
* <span data-ttu-id="fc109-861">Fehler beim Überprüfen des primären Zertifikats behoben</span><span class="sxs-lookup"><span data-stu-id="fc109-861">Fixed primary certificate validation bug</span></span>

### <a name="storage"></a><span data-ttu-id="fc109-862">Storage</span><span class="sxs-lookup"><span data-stu-id="fc109-862">Storage</span></span>

* <span data-ttu-id="fc109-863">Befehl `storage copy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-863">Added command `storage copy`</span></span>

## <a name="july-30-2019"></a><span data-ttu-id="fc109-864">30. Juli 2019</span><span class="sxs-lookup"><span data-stu-id="fc109-864">July 30, 2019</span></span>

<span data-ttu-id="fc109-865">Version 2.0.70</span><span class="sxs-lookup"><span data-stu-id="fc109-865">Version 2.0.70</span></span>

### <a name="acr"></a><span data-ttu-id="fc109-866">ACR</span><span class="sxs-lookup"><span data-stu-id="fc109-866">ACR</span></span>

* <span data-ttu-id="fc109-867">Problem #9952 behoben (Regression im Befehl `acr pack build`)</span><span class="sxs-lookup"><span data-stu-id="fc109-867">Fixed issue #9952 (a regression in the `acr pack build` command)</span></span>
* <span data-ttu-id="fc109-868">Standardname des Generatorimages in `acr pack build` entfernt</span><span class="sxs-lookup"><span data-stu-id="fc109-868">Removed the default builder image name in `acr pack build`</span></span>

### <a name="appservice"></a><span data-ttu-id="fc109-869">AppService</span><span class="sxs-lookup"><span data-stu-id="fc109-869">Appservice</span></span>

* <span data-ttu-id="fc109-870">`webapp config ssl` geändert, um eine Meldung anzuzeigen, wenn eine Ressource nicht gefunden wurde</span><span class="sxs-lookup"><span data-stu-id="fc109-870">Changed `webapp config ssl` to show a message if a resource is not found</span></span>
* <span data-ttu-id="fc109-871">Problem behoben, aufgrund dessen `functionapp create` den Speicherkontotypen `Standard_RAGRS` nicht akzeptiert hat</span><span class="sxs-lookup"><span data-stu-id="fc109-871">Fixed issue where `functionapp create` does not accept `Standard_RAGRS` storage account type</span></span>
* <span data-ttu-id="fc109-872">Problem behoben, aufgrund dessen für `webapp up` ein Fehler auftrat, wenn für die Ausführung ältere Python-Versionen verwendet wurden</span><span class="sxs-lookup"><span data-stu-id="fc109-872">Fixed an issue where `webapp up` would fail if run using older versions of python</span></span>

### <a name="network"></a><span data-ttu-id="fc109-873">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="fc109-873">Network</span></span>

* <span data-ttu-id="fc109-874">Ungültiger Parameter `--ids` aus `network nic ip-config add` entfernt (Fehlerbehebungen #9861)</span><span class="sxs-lookup"><span data-stu-id="fc109-874">Removed invalid parameter `--ids` from `network nic ip-config add` (fixes #9861)</span></span>
* <span data-ttu-id="fc109-875">Fehlerbehebungen #9604.</span><span class="sxs-lookup"><span data-stu-id="fc109-875">Fixes #9604.</span></span> <span data-ttu-id="fc109-876">Parameter `--root-certs` zu `network application-gateway http-settings [create|update]` hinzugefügt, um vom Benutzer zugewiesene vertrauenswürdige Stammzertifikate zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="fc109-876">Added `--root-certs` parameter to `network application-gateway http-settings [create|update]` to support user associate trusted root certificates.</span></span>
* <span data-ttu-id="fc109-877">Argument `--subscription` für `network dns record-set ns create` korrigiert (#9965)</span><span class="sxs-lookup"><span data-stu-id="fc109-877">Fixed arguent `--subscription` for `network dns record-set ns create` (#9965)</span></span>

### <a name="rbac"></a><span data-ttu-id="fc109-878">RBAC</span><span class="sxs-lookup"><span data-stu-id="fc109-878">RBAC</span></span>

* <span data-ttu-id="fc109-879">Befehl `user update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-879">Added `user update` command</span></span>
* <span data-ttu-id="fc109-880">[VERALTET]`--upn-or-object-id` in benutzerbezogenen Befehlen als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="fc109-880">[DEPRECATED] Deprecated `--upn-or-object-id` from user-related commands</span></span>
    * <span data-ttu-id="fc109-881">Verwenden Sie das Ersatzargument `--id`.</span><span class="sxs-lookup"><span data-stu-id="fc109-881">Use replacement argument `--id`</span></span>
* <span data-ttu-id="fc109-882">Argument `--id` zu benutzerbezogenen Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-882">Added `--id` argument to user-related commands</span></span>

### <a name="sql"></a><span data-ttu-id="fc109-883">SQL</span><span class="sxs-lookup"><span data-stu-id="fc109-883">SQL</span></span>

* <span data-ttu-id="fc109-884">Verwaltungsbefehle für Schlüssel verwalteter Instanzen und TDE-Schutzvorrichtung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-884">Added management commands for managed instance keys and TDE protector</span></span>

### <a name="storage"></a><span data-ttu-id="fc109-885">Storage</span><span class="sxs-lookup"><span data-stu-id="fc109-885">Storage</span></span>

* <span data-ttu-id="fc109-886">Befehl `storage remove` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-886">Added `storage remove` command</span></span>
* <span data-ttu-id="fc109-887">Problem mit `storage blob update` behoben</span><span class="sxs-lookup"><span data-stu-id="fc109-887">Fixed an issue with `storage blob update`</span></span>

### <a name="vm"></a><span data-ttu-id="fc109-888">VM</span><span class="sxs-lookup"><span data-stu-id="fc109-888">VM</span></span>

* <span data-ttu-id="fc109-889">`list-skus` wurde geändert, um eine neuere API-Version für die Ausgabe von Zonendetails zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="fc109-889">Changed `list-skus` to use newer api-version to output zone details</span></span>
* <span data-ttu-id="fc109-890">Standardwert `--single-placement-group` für `vmss create` in `false` geändert</span><span class="sxs-lookup"><span data-stu-id="fc109-890">Changed default of `--single-placement-group` to `false` for `vmss create`</span></span>
* <span data-ttu-id="fc109-891">Möglichkeit zum Auswählen von ZRS-Speicher-SKUs für `[snapshot|disk] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-891">Added ability to select ZRS storage SKUs for `[snapshot|disk] create`</span></span>
* <span data-ttu-id="fc109-892">Neue Befehlsgruppe `vm host` zur Unterstützung dedizierter Hosts hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-892">Added new command group `vm host` to support dedicated hosts</span></span>
* <span data-ttu-id="fc109-893">Parameter `--host` und `--host-group` für `vm create` hinzugefügt, um den dedizierten VM-Host festzulegen</span><span class="sxs-lookup"><span data-stu-id="fc109-893">Added parameters `--host` and `--host-group` on `vm create` to set VM dedicated host</span></span>

## <a name="july-16-2019"></a><span data-ttu-id="fc109-894">16. Juli 2019</span><span class="sxs-lookup"><span data-stu-id="fc109-894">July 16, 2019</span></span>

<span data-ttu-id="fc109-895">Version 2.0.69</span><span class="sxs-lookup"><span data-stu-id="fc109-895">Version 2.0.69</span></span>

### <a name="appservice"></a><span data-ttu-id="fc109-896">AppService</span><span class="sxs-lookup"><span data-stu-id="fc109-896">Appservice</span></span>

* <span data-ttu-id="fc109-897">`webapp identity`-Befehle geändert, um eine korrekte Fehlermeldung zurückzugeben, wenn „ResourceGroupName“ oder der App-Name ungültig sind</span><span class="sxs-lookup"><span data-stu-id="fc109-897">Changed `webapp identity` commands to return a proper error message if ResourceGroupName or App name are invalid</span></span>
* <span data-ttu-id="fc109-898">`webapp list` korrigiert, sodass der korrekte Wert für „numberOfSites“ zurückgegeben wird, wenn „ResourceGroup“ nicht angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="fc109-898">Fixed `webapp list` to return the correct value for numberOfSites if no ResourceGroup was provided</span></span>
* <span data-ttu-id="fc109-899">Nebeneffekte von `appservice plan create` und `webapp create` behoben</span><span class="sxs-lookup"><span data-stu-id="fc109-899">Fixed side-effects of `appservice plan create` and `webapp create`</span></span>

### <a name="core"></a><span data-ttu-id="fc109-900">Core</span><span class="sxs-lookup"><span data-stu-id="fc109-900">Core</span></span>

* <span data-ttu-id="fc109-901">Problem behoben, aufgrund dessen `--subscription` angezeigt wurde, obwohl nicht anwendbar</span><span class="sxs-lookup"><span data-stu-id="fc109-901">Fixed issue where `--subscription` would appear despite being not applicable</span></span>

### <a name="batch"></a><span data-ttu-id="fc109-902">Batch</span><span class="sxs-lookup"><span data-stu-id="fc109-902">Batch</span></span>

* <span data-ttu-id="fc109-903">[BREAKING CHANGE]`batch pool node-agent-skus list` durch `batch pool supported-images list` ersetzt</span><span class="sxs-lookup"><span data-stu-id="fc109-903">[BREAKING CHANGE] Replaced `batch pool node-agent-skus list` with `batch pool supported-images list`</span></span>
* <span data-ttu-id="fc109-904">Unterstützung für Sicherheitsregeln hinzugefügt, die den Netzwerkzugriff auf einen Pool basierend auf dem Quellport des Datenverkehrs blockieren, wenn die Option `--json-file` von `batch pool create network` verwendet wird</span><span class="sxs-lookup"><span data-stu-id="fc109-904">Added support for security rules blocking network access to a pool based on the source port of the traffic when using the `--json-file` option of `batch pool create network`</span></span>
* <span data-ttu-id="fc109-905">Unterstützung für die Ausführung der Aufgabe im Arbeitsverzeichnis des Containers oder der Batch-Aufgabe hinzugefügt, wenn die Option `--json-file` von `batch task create` verwendet wird</span><span class="sxs-lookup"><span data-stu-id="fc109-905">Added support for executing the task in the container working directory or in the Batch task working directory when using the `--json-file` option of `batch task create`</span></span>
* <span data-ttu-id="fc109-906">Fehler in Option `--application-package-references` von `batch pool create` behoben, aufgrund dessen nur Standardeinstellungen möglich waren</span><span class="sxs-lookup"><span data-stu-id="fc109-906">Fixed error in `--application-package-references` option of `batch pool create` where it would only work with defaults</span></span>

### <a name="eventhubs"></a><span data-ttu-id="fc109-907">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="fc109-907">Eventhubs</span></span>

* <span data-ttu-id="fc109-908">Validierung für Parameter `--rights` von `authorizationrule`-Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-908">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="rdbms"></a><span data-ttu-id="fc109-909">RDBMS</span><span class="sxs-lookup"><span data-stu-id="fc109-909">RDBMS</span></span>

* <span data-ttu-id="fc109-910">Optionaler Parameter zum Angeben der Replikat-SKU für den Befehl zum Erstellen von Replikaten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-910">Added optional parameter to specify replica SKU for create replica command</span></span>
* <span data-ttu-id="fc109-911">Problem mit CI-Testfehler bei der Erstellung von MySQL-Replikaten behoben</span><span class="sxs-lookup"><span data-stu-id="fc109-911">Fixed the issue with CI test failure with creating MySQL replica</span></span>

### <a name="relay"></a><span data-ttu-id="fc109-912">Relay</span><span class="sxs-lookup"><span data-stu-id="fc109-912">Relay</span></span>

* <span data-ttu-id="fc109-913">Problem mit Hybridverbindung behoben, wenn die Client-Autorisierung deaktiviert ist [#8775](https://github.com/azure/azure-cli/issues/8775)</span><span class="sxs-lookup"><span data-stu-id="fc109-913">Fixed issue with hybrid connection when client authroization disabled [#8775](https://github.com/azure/azure-cli/issues/8775)</span></span>
* <span data-ttu-id="fc109-914">Parameter `--requires-transport-security` zu `relay wcfrelay create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-914">Added parameter `--requires-transport-security` to `relay wcfrelay create`</span></span>

### <a name="servicebus"></a><span data-ttu-id="fc109-915">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="fc109-915">Servicebus</span></span>

* <span data-ttu-id="fc109-916">Validierung für Parameter `--rights` von `authorizationrule`-Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-916">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="storage"></a><span data-ttu-id="fc109-917">Storage</span><span class="sxs-lookup"><span data-stu-id="fc109-917">Storage</span></span>

* <span data-ttu-id="fc109-918">AADDS für Files für Speicherkontoaktualisierung aktiviert</span><span class="sxs-lookup"><span data-stu-id="fc109-918">Enable Files AADDS for storage account update</span></span>
* <span data-ttu-id="fc109-919">Problem `storage blob service-properties update --set` behoben</span><span class="sxs-lookup"><span data-stu-id="fc109-919">Fixed issue `storage blob service-properties update --set`</span></span>

## <a name="july-2-2019"></a><span data-ttu-id="fc109-920">2\. Juli 2019</span><span class="sxs-lookup"><span data-stu-id="fc109-920">July 2, 2019</span></span>

<span data-ttu-id="fc109-921">Version 2.0.68</span><span class="sxs-lookup"><span data-stu-id="fc109-921">Version 2.0.68</span></span>

### <a name="core"></a><span data-ttu-id="fc109-922">Core</span><span class="sxs-lookup"><span data-stu-id="fc109-922">Core</span></span>

* <span data-ttu-id="fc109-923">Befehlsmodule sind jetzt in einer einzelnen verteilbaren Python-Komponente zusammengefasst.</span><span class="sxs-lookup"><span data-stu-id="fc109-923">Command modules are now consolidated into a single Python distributable.</span></span> <span data-ttu-id="fc109-924">Die direkte Verwendung zahlreicher Pakete vom Typ `azure-cli-` in PyPI ist daher veraltet.</span><span class="sxs-lookup"><span data-stu-id="fc109-924">This deprecates direct use of many `azure-cli-` packages on PyPI.</span></span>
  <span data-ttu-id="fc109-925">Dadurch sollte sich die Installationsgröße reduzieren. Darüber hinaus sollte es nur Benutzer betreffen, die eine direkte Installation über `pip` ausgeführt haben.</span><span class="sxs-lookup"><span data-stu-id="fc109-925">This should reduce install size and only affect users who have directly installed via `pip`.</span></span>

### <a name="acr"></a><span data-ttu-id="fc109-926">ACR</span><span class="sxs-lookup"><span data-stu-id="fc109-926">ACR</span></span>

* <span data-ttu-id="fc109-927">Unterstützung für Trigger mit Timer zu Aufgabe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-927">Added support for Timer Triggers to Task</span></span>

### <a name="appservice"></a><span data-ttu-id="fc109-928">AppService</span><span class="sxs-lookup"><span data-stu-id="fc109-928">Appservice</span></span>

* <span data-ttu-id="fc109-929">`functionapp create` wurde so geändert, das Application Insights standardmäßig aktiviert wird.</span><span class="sxs-lookup"><span data-stu-id="fc109-929">Changed `functionapp create` to enable application insights by default</span></span>
* <span data-ttu-id="fc109-930">[BREAKING CHANGE] Veralteter Befehl `functionapp devops-build` entfernt.</span><span class="sxs-lookup"><span data-stu-id="fc109-930">[BREAKING CHANGE] Removed deprecated `functionapp devops-build` command.</span></span>
  *  <span data-ttu-id="fc109-931">Verwenden Sie stattdessen den neuen Befehl `az functionapp devops-pipeline`.</span><span class="sxs-lookup"><span data-stu-id="fc109-931">Use the new command `az functionapp devops-pipeline` instead</span></span>
* <span data-ttu-id="fc109-932">Unterstützung des Funktions-App-Plans für Linux-Verbrauch zu `functionapp deployment config-zip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-932">Added Linux Consumption function app plan support to `functionapp deployment config-zip`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="fc109-933">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="fc109-933">Cosmos DB</span></span>

* <span data-ttu-id="fc109-934">Unterstützung für das Deaktivieren von TTL hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-934">Added support for disabling TTL</span></span>

### <a name="dls"></a><span data-ttu-id="fc109-935">DLS</span><span class="sxs-lookup"><span data-stu-id="fc109-935">DLS</span></span>

* <span data-ttu-id="fc109-936">Aktualisierte ADLS-Version (0.0.45)</span><span class="sxs-lookup"><span data-stu-id="fc109-936">Updated ADLS version (0.0.45)</span></span>

### <a name="feedback"></a><span data-ttu-id="fc109-937">Feedback</span><span class="sxs-lookup"><span data-stu-id="fc109-937">Feedback</span></span>

* <span data-ttu-id="fc109-938">Wird ein fehlgeschlagener Erweiterungsbefehl gemeldet, versucht `az feedback` nun, über den Index die Projekt-/Repository-URL der Erweiterung im Browser zu öffnen.</span><span class="sxs-lookup"><span data-stu-id="fc109-938">When reporting a failed extension command, `az feedback` now attempts to open the browser to the project/repo url of the extension from the index</span></span>

### <a name="hdinsight"></a><span data-ttu-id="fc109-939">HDInsight</span><span class="sxs-lookup"><span data-stu-id="fc109-939">HDInsight</span></span>

* <span data-ttu-id="fc109-940">[BREAKING CHANGE] Der Befehlsgruppenname `oms` wurde in `monitor` geändert.</span><span class="sxs-lookup"><span data-stu-id="fc109-940">[BREAKING CHANGE] Changed `oms` command group name to `monitor`</span></span>
* <span data-ttu-id="fc109-941">[BREAKING CHANGE]`--http-password/-p` als erforderlicher Parameter festgelegt</span><span class="sxs-lookup"><span data-stu-id="fc109-941">[BREAKING CHANGE] Made `--http-password/-p` a required parameter</span></span> 
* <span data-ttu-id="fc109-942">Vervollständigungen für `--cluster-admin-account` und `cluster-users-group-dns` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-942">Added completers for `--cluster-admin-account` and `cluster-users-group-dns` parameters completer</span></span> 
* <span data-ttu-id="fc109-943">Parameter `cluster-users-group-dns` so geändert, dass er erforderlich ist, wenn `—esp` vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="fc109-943">Changed `cluster-users-group-dns` parameter to be required when `—esp` is present</span></span>
* <span data-ttu-id="fc109-944">Timeout für alle vorhandenen automatischen Argumentvervollständigungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-944">Added a timeout for all existing argument auto-completers</span></span>
* <span data-ttu-id="fc109-945">Timeout für das Transformieren des Ressourcennamens in eine Ressourcen-ID hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-945">Added a timeout for transforming resource name to resource id</span></span>
* <span data-ttu-id="fc109-946">Die automatischen Vervollständigungen wurden so geändert, dass Ressourcen aus einer beliebigen Ressourcengruppe ausgewählt werden.</span><span class="sxs-lookup"><span data-stu-id="fc109-946">Changed Auto-completers to select resources from any resource group.</span></span> <span data-ttu-id="fc109-947">Dabei kann es sich um eine andere Ressourcengruppe als die mit `-g` angegebene Gruppe handeln.</span><span class="sxs-lookup"><span data-stu-id="fc109-947">It can be a different resource group than the one specified with `-g`</span></span>
* <span data-ttu-id="fc109-948">Unterstützung für die Parameter `--sub-domain-suffix` und `--disable_gateway_auth` im Befehl `hdinsight application create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-948">Added support for `--sub-domain-suffix` and `--disable_gateway_auth` parameters in the `hdinsight application create` command</span></span>

### <a name="managed-services"></a><span data-ttu-id="fc109-949">Verwaltete Dienste</span><span class="sxs-lookup"><span data-stu-id="fc109-949">Managed Services</span></span>

* <span data-ttu-id="fc109-950">Befehlsmodul für verwaltete Dienste als Vorschau eingeführt</span><span class="sxs-lookup"><span data-stu-id="fc109-950">Introducing managed service command module in preview</span></span>

### <a name="profile"></a><span data-ttu-id="fc109-951">Profil</span><span class="sxs-lookup"><span data-stu-id="fc109-951">Profile</span></span>
* <span data-ttu-id="fc109-952">Argument `--subscription` für Abmeldebefehl unterdrückt</span><span class="sxs-lookup"><span data-stu-id="fc109-952">Suppress `--subscription` argument for logout command</span></span>

### <a name="rbac"></a><span data-ttu-id="fc109-953">RBAC</span><span class="sxs-lookup"><span data-stu-id="fc109-953">RBAC</span></span>

* <span data-ttu-id="fc109-954">[BREAKING CHANGE] Argument `--password` für `create-for-rbac` entfernt</span><span class="sxs-lookup"><span data-stu-id="fc109-954">[BREAKING CHANGE] Removed `--password` argument for `create-for-rbac`</span></span>
* <span data-ttu-id="fc109-955">Parameter `--assignee-principal-type` zum Befehl `create` hinzugefügt, um zeitweilige Fehler zu vermeiden, die durch die Replikationswartezeit des AAD-Graph-Servers verursacht werden</span><span class="sxs-lookup"><span data-stu-id="fc109-955">Added `--assignee-principal-type` parameter to `create` command to avoid intermittent failures caused by AAD graph server replication latency</span></span>
* <span data-ttu-id="fc109-956">Absturz in `ad signed-in-user` beim Auflisten von in Besitz befindlichen Objekten behoben</span><span class="sxs-lookup"><span data-stu-id="fc109-956">Fixed a crash in `ad signed-in-user` when listing owned objects</span></span>
* <span data-ttu-id="fc109-957">Problem behoben, aufgrund dessen `ad sp` nicht die richtige Anwendung über einen Dienstprinzipal fand</span><span class="sxs-lookup"><span data-stu-id="fc109-957">Fixed issue where `ad sp` would not find the right application from a service principal</span></span>

### <a name="rdbms"></a><span data-ttu-id="fc109-958">RDBMS</span><span class="sxs-lookup"><span data-stu-id="fc109-958">RDBMS</span></span>

* <span data-ttu-id="fc109-959">Unterstützung für die Replikation für MariaDB hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-959">Added support for replication for MariaDB</span></span>

### <a name="sql"></a><span data-ttu-id="fc109-960">SQL</span><span class="sxs-lookup"><span data-stu-id="fc109-960">SQL</span></span>

* <span data-ttu-id="fc109-961">Zulässige Werte für `sql db create --sample-name` dokumentiert</span><span class="sxs-lookup"><span data-stu-id="fc109-961">Documented allowed values for `sql db create --sample-name`</span></span>

### <a name="storage"></a><span data-ttu-id="fc109-962">Storage</span><span class="sxs-lookup"><span data-stu-id="fc109-962">Storage</span></span>

* <span data-ttu-id="fc109-963">Unterstützung von SAS-Token für die Benutzerdelegierung mit `--as-user` zu `storage blob generate-sas` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-963">Added user delegation SAS token support with `--as-user` to `storage blob generate-sas`</span></span> 
* <span data-ttu-id="fc109-964">Unterstützung von SAS-Token für die Benutzerdelegierung mit `--as-user` zu `storage container generate-sas` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-964">Added user delegation SAS token support with `--as-user` to `storage container generate-sas`</span></span> 

### <a name="vm"></a><span data-ttu-id="fc109-965">VM</span><span class="sxs-lookup"><span data-stu-id="fc109-965">VM</span></span>

* <span data-ttu-id="fc109-966">Fehler behoben, aufgrund dessen `vmss create` bei der Ausführung mit `--no-wait` eine Fehlermeldung zurückgab</span><span class="sxs-lookup"><span data-stu-id="fc109-966">Fixed bug where `vmss create` returns an error message when run with `--no-wait`</span></span>
* <span data-ttu-id="fc109-967">Die clientseitige Validierung für `vmss create --single-placement-group` wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="fc109-967">Removed client-side validation for `vmss create --single-placement-group`.</span></span> <span data-ttu-id="fc109-968">Es tritt kein Fehler auf, wenn `--single-placement-group` auf `true` und für `--instance-count` ein größerer Wert als 100 festgelegt wird oder wenn Verfügbarkeitszonen angegeben werden. Diese Validierung wird jedoch dem Computedienst überlassen.</span><span class="sxs-lookup"><span data-stu-id="fc109-968">Does not fail if `--single-placement-group` is set to `true` and`--instance-count` is greater than 100 or availability zones are specified, but leaves this validation to the compute service</span></span>
* <span data-ttu-id="fc109-969">Problem behoben, aufgrund dessen bei der Verwendung von `--latest` für `[vm|vmss] extension image list` ein Fehler auftrat</span><span class="sxs-lookup"><span data-stu-id="fc109-969">Fixed bug where `[vm|vmss] extension image list` fails when used with `--latest`</span></span>


## <a name="june-18-2019"></a><span data-ttu-id="fc109-970">18. Juni 2019</span><span class="sxs-lookup"><span data-stu-id="fc109-970">June 18, 2019</span></span>

<span data-ttu-id="fc109-971">Version 2.0.67</span><span class="sxs-lookup"><span data-stu-id="fc109-971">Version 2.0.67</span></span>

### <a name="core"></a><span data-ttu-id="fc109-972">Core</span><span class="sxs-lookup"><span data-stu-id="fc109-972">Core</span></span>

<span data-ttu-id="fc109-973">In diesem Release wird das neue [Preview]-Tag eingeführt, um Kunden gegenüber deutlich zu machen, dass sich eine Befehlsgruppe, ein Befehl oder ein Argument in der Vorschauphase befindet.</span><span class="sxs-lookup"><span data-stu-id="fc109-973">This release introduces a new [Preview] tag to more clearly communicate to customers when a command group, command or argument is in preview status.</span></span> <span data-ttu-id="fc109-974">Diese Information war zuvor im Hilfetext oder implizit durch die Versionsnummer des Befehlsmoduls angegeben.</span><span class="sxs-lookup"><span data-stu-id="fc109-974">This was previously called out in help text or communicated implicitly by the command module version number.</span></span>
<span data-ttu-id="fc109-975">Die Befehlszeilenschnittstelle wird künftig Versionsnummern für einzelne Pakete entfernen.</span><span class="sxs-lookup"><span data-stu-id="fc109-975">The CLI will be removing version numbers for individual packages in the future.</span></span> <span data-ttu-id="fc109-976">Wenn sich ein Befehl in der Vorschauphase befindet, gilt dies auch für alle seine Argumente.</span><span class="sxs-lookup"><span data-stu-id="fc109-976">If a command is in preview, all of its arguments are as well.</span></span> <span data-ttu-id="fc109-977">Wenn eine Befehlsgruppe als Vorschau gekennzeichnet ist, befinden sich auch alle Befehle und Argumente in der Vorschauphase.</span><span class="sxs-lookup"><span data-stu-id="fc109-977">If a command group is labeled as being in preview, then all commands and arguments are considered to be in preview as well.</span></span>

<span data-ttu-id="fc109-978">Infolge dieser Änderung befinden sich in diesem Release verschiedene Befehlsgruppen anscheinend „plötzlich“ in der Vorschauphase.</span><span class="sxs-lookup"><span data-stu-id="fc109-978">As a result of this change, several command groups may seem to "suddenly" appear to be in a preview status with this release.</span></span> <span data-ttu-id="fc109-979">Tatsächlich ist es jedoch so, dass sich die meisten Pakete in der Vorschauphase befanden, in diesem Release jedoch als allgemein verfügbar gelten.</span><span class="sxs-lookup"><span data-stu-id="fc109-979">What actually happened is that most packages were in a preview status, but are being deemed GA with this release</span></span>

### <a name="acr"></a><span data-ttu-id="fc109-980">ACR</span><span class="sxs-lookup"><span data-stu-id="fc109-980">ACR</span></span>
* <span data-ttu-id="fc109-981">Befehl „acr check-health“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-981">Added 'acr check-health' command</span></span>
* <span data-ttu-id="fc109-982">Verbesserte Fehlerbehandlung für AAD-Token und für das Abrufen externer Befehle</span><span class="sxs-lookup"><span data-stu-id="fc109-982">Improved error handling for AAD tokens and for retrieving external commands</span></span>

### <a name="acs"></a><span data-ttu-id="fc109-983">ACS</span><span class="sxs-lookup"><span data-stu-id="fc109-983">ACS</span></span>
* <span data-ttu-id="fc109-984">Veraltete ACS-Befehle werden jetzt in der Hilfeansicht ausgeblendet.</span><span class="sxs-lookup"><span data-stu-id="fc109-984">Deprecated ACS commands are now hidden from help view</span></span>

### <a name="ams"></a><span data-ttu-id="fc109-985">AMS</span><span class="sxs-lookup"><span data-stu-id="fc109-985">AMS</span></span>
* <span data-ttu-id="fc109-986">[BREAKING CHANGE] Änderung, damit ISO 8601-Zeitzeichenfolgen für „archive-window-length“ und „key-frame-interval-duration“ zurückgegeben werden</span><span class="sxs-lookup"><span data-stu-id="fc109-986">[BREAKING CHANGE] Changed to return ISO 8601 time strings for archive-window-length and key-frame-interval-duration</span></span>

### <a name="appservice"></a><span data-ttu-id="fc109-987">AppService</span><span class="sxs-lookup"><span data-stu-id="fc109-987">AppService</span></span>
* <span data-ttu-id="fc109-988">Standortbasiertes Routing für `webapp deleted list` und `webapp deleted restore` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-988">Added location based routing for `webapp deleted list` and `webapp deleted restore`</span></span>
* <span data-ttu-id="fc109-989">Problem behoben, aufgrund dessen in Azure Cloud Shell nicht auf die von einer Web-App protokollierte Ziel-URL („Sie können die App starten unter...“) geklickt werden konnte</span><span class="sxs-lookup"><span data-stu-id="fc109-989">Fixed issue where webapp up logged target URL ("You can launch the app at...") was not clickable in Azure Cloud Shell</span></span>
* <span data-ttu-id="fc109-990">Problem behoben, aufgrund dessen beim Erstellen von Apps bei einigen SKUs ein AlwaysOn-Fehler auftrat</span><span class="sxs-lookup"><span data-stu-id="fc109-990">Fixed an issue where creating apps with the some SKUs was failing with an AlwaysOn error</span></span>
* <span data-ttu-id="fc109-991">Vorabüberprüfung zu `[appservice|webapp] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-991">Added pre-validation to `[appservice|webapp] create`</span></span>
* <span data-ttu-id="fc109-992">`[webapp|functionapp] traffic-routing` korrigiert, damit der richtige actionHostName-Wert verwendet wird</span><span class="sxs-lookup"><span data-stu-id="fc109-992">Fixed `[webapp|functionapp] traffic-routing` to use the correct actionHostName</span></span>
* <span data-ttu-id="fc109-993">Slotunterstützung zu `functionapp`-Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-993">Added slot support to `functionapp` commands</span></span>

### <a name="batch"></a><span data-ttu-id="fc109-994">Batch</span><span class="sxs-lookup"><span data-stu-id="fc109-994">Batch</span></span>
* <span data-ttu-id="fc109-995">AAD-Authentifizierungsregression korrigiert, die von übermäßiger Berichterstellung für Authentifizierung mit gemeinsam verwendetem Schlüssel verursacht wurde</span><span class="sxs-lookup"><span data-stu-id="fc109-995">Fixed AAD auth regression caused by over-aggressive error reporting for Shared Key Auth</span></span>

### <a name="batchai"></a><span data-ttu-id="fc109-996">Batch AI</span><span class="sxs-lookup"><span data-stu-id="fc109-996">BatchAI</span></span>
* <span data-ttu-id="fc109-997">BatchAI-Befehle sind jetzt veraltet und ausgeblendet.</span><span class="sxs-lookup"><span data-stu-id="fc109-997">BatchAI commands are now deprecated and hidden</span></span>

### <a name="botservice"></a><span data-ttu-id="fc109-998">BotService</span><span class="sxs-lookup"><span data-stu-id="fc109-998">BotService</span></span>
* <span data-ttu-id="fc109-999">Für Befehle, die Version 3 des SDK unterstützen, wurden die Warnmeldungen „Support eingestellt“/„Wartungsmodus“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-999">Added "discontinued support"/"maintenance mode" warning messages for commands that support the v3 SDK</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="fc109-1000">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="fc109-1000">CosmosDB</span></span>
* <span data-ttu-id="fc109-1001">[VERALTET] Der Befehl `cosmosdb list-keys` wurde als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="fc109-1001">[DEPRECATED] Deprecated the `cosmosdb list-keys` command</span></span>
* <span data-ttu-id="fc109-1002">Befehl `cosmosdb keys list` hinzugefügt, er ersetzt `cosmosdb list-keys`.</span><span class="sxs-lookup"><span data-stu-id="fc109-1002">Added the `cosmosdb keys list` command - replaces `cosmosdb list-keys`</span></span>
* <span data-ttu-id="fc109-1003">`cosmsodb create/update`: Neues Format für „--location“ hinzugefügt, um das Festlegen der Eigenschaft „isZoneRedundant“ zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="fc109-1003">`cosmsodb create/update`: Added new format for --location to allow setting "isZoneRedundant" property.</span></span> <span data-ttu-id="fc109-1004">Das alte Format wurde als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="fc109-1004">Deprecated old format</span></span>

### <a name="eventgrid"></a><span data-ttu-id="fc109-1005">EventGrid</span><span class="sxs-lookup"><span data-stu-id="fc109-1005">EventGrid</span></span>
* <span data-ttu-id="fc109-1006">`eventgrid domain`-Befehle für CRUD-Vorgänge für Domänen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1006">Added `eventgrid domain` commands for domain CRUD operations</span></span>
* <span data-ttu-id="fc109-1007">`eventgrid domain topic`-Befehle für CRUD-Vorgänge für Domänenthemen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1007">Added `eventgrid domain topic` commands for domain topics CRUD operations</span></span>
* <span data-ttu-id="fc109-1008">Argument `--odata-query` zu `eventgrid [topic|event-subscription] list` zum Filtern der Ergebnisse mithilfe von OData-Syntax hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1008">Added `--odata-query` argument to `eventgrid [topic|event-subscription] list` for filtering results using OData syntax</span></span>
* <span data-ttu-id="fc109-1009">`event-subscription create/update`: „servicebusqueue“ als neue Werte für den Parameter `--endpoint-type` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1009">`event-subscription create/update`: Added servicebusqueue as new values for the `--endpoint-type` parameter</span></span>
* <span data-ttu-id="fc109-1010">[BREAKING CHANGE] Unterstützung für `--included-event-types All` mit `eventgrid event-subscription [create|update]` entfernt</span><span class="sxs-lookup"><span data-stu-id="fc109-1010">[BREAKING CHANGE] Removed support for `--included-event-types All` with `eventgrid event-subscription [create|update]`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="fc109-1011">HDInsight</span><span class="sxs-lookup"><span data-stu-id="fc109-1011">HDInsight</span></span>
* <span data-ttu-id="fc109-1012">Unterstützung für den Parameter `--ssh-public-key` im Befehl vom Typ `hdinsight create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1012">Added support for `--ssh-public-key` parameter in `hdinsight create` command</span></span>

### <a name="iot"></a><span data-ttu-id="fc109-1013">IoT</span><span class="sxs-lookup"><span data-stu-id="fc109-1013">IoT</span></span>
* <span data-ttu-id="fc109-1014">Unterstützung für das erneute Generieren von Autorisierungsrichtlinienschlüsseln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1014">Added support to regenerate authorization policy keys</span></span>
* <span data-ttu-id="fc109-1015">SDK und Unterstützung für den Bereitstellungsdienst des DigitalTwin-Repositorys hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1015">Added SDK and support for DigitalTwin Repository Provisioning Service</span></span>

### <a name="network"></a><span data-ttu-id="fc109-1016">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="fc109-1016">Network</span></span>
* <span data-ttu-id="fc109-1017">Zonenunterstützung für NAT Gateway hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1017">Added Zone support for Nat Gateway</span></span>
* <span data-ttu-id="fc109-1018">Befehl `network list-service-tags` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1018">Added command `network list-service-tags`</span></span>
* <span data-ttu-id="fc109-1019">Problem mit `dns zone import` behoben, aufgrund dessen Benutzer keine A-Platzhaltereinträge importieren konnten</span><span class="sxs-lookup"><span data-stu-id="fc109-1019">Fixed issue with `dns zone import` where users could not import wildcard A records</span></span>
* <span data-ttu-id="fc109-1020">Problem mit `watcher flow-log configure` behoben, aufgrund dessen die Flowprotokollierung in bestimmten Regionen nicht aktiviert werden konnte</span><span class="sxs-lookup"><span data-stu-id="fc109-1020">Fixed issue with `watcher flow-log configure` where flow logging could not be enabled in certain regions</span></span>

### <a name="resource"></a><span data-ttu-id="fc109-1021">Resource</span><span class="sxs-lookup"><span data-stu-id="fc109-1021">Resource</span></span>
* <span data-ttu-id="fc109-1022">Befehl `az rest` zum Ausführen von REST-Aufrufen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1022">Added `az rest` command for making REST calls</span></span>
* <span data-ttu-id="fc109-1023">Fehler behoben, der bei Verwendung von `policy assignment list` mit `--scope` auf Ressourcengruppen- oder Abonnementebene auftrat</span><span class="sxs-lookup"><span data-stu-id="fc109-1023">Fixed error when using `policy assignment list` with a resource group or subscription level `--scope`</span></span>

### <a name="servicebus"></a><span data-ttu-id="fc109-1024">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="fc109-1024">ServiceBus</span></span>
* <span data-ttu-id="fc109-1025">Problem mit `servicebus topic create --max-size` behoben [Nr. 9319](https://github.com/azure/azure-cli/issues/9319)</span><span class="sxs-lookup"><span data-stu-id="fc109-1025">Fixed issue with `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span></span>

### <a name="sql"></a><span data-ttu-id="fc109-1026">SQL</span><span class="sxs-lookup"><span data-stu-id="fc109-1026">SQL</span></span>
* <span data-ttu-id="fc109-1027">`--location` wurde geändert und ist nun für `sql [server|mi] create` optional. Ohne Angabe wird der Ressourcengruppenstandort verwendet.</span><span class="sxs-lookup"><span data-stu-id="fc109-1027">Changed `--location` to be optional for `sql [server|mi] create` - uses resource group location if not specified</span></span>
* <span data-ttu-id="fc109-1028">Der Fehler, dass das Objekt „NoneType“ nicht wiederholbar ist, wurde für `sql db list-editions --available` behoben.</span><span class="sxs-lookup"><span data-stu-id="fc109-1028">Fixed "'NoneType' object is not iterable" error for `sql db list-editions --available`</span></span>

### <a name="sqlvm"></a><span data-ttu-id="fc109-1029">SQLVm</span><span class="sxs-lookup"><span data-stu-id="fc109-1029">SQLVm</span></span>
* <span data-ttu-id="fc109-1030">[WICHTIGE ÄNDERUNG] `sql vm create` wurde geändert und erfordert nun den Parameter `--license-type`.</span><span class="sxs-lookup"><span data-stu-id="fc109-1030">[BREAKING CHNAGE] Changed `sql vm create` to require `--license-type` parameter</span></span>
* <span data-ttu-id="fc109-1031">Änderung, um beim Erstellen oder Aktualisieren einer SQL-VM das Festlegen der SQL-Image-SKU zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="fc109-1031">Changed to allow setting SQL image SKU when creating or updating a sql vm</span></span>

### <a name="storage"></a><span data-ttu-id="fc109-1032">Storage</span><span class="sxs-lookup"><span data-stu-id="fc109-1032">Storage</span></span>
* <span data-ttu-id="fc109-1033">Problem mit fehlendem Kontoschlüssel für `storage container generate-sas` behoben</span><span class="sxs-lookup"><span data-stu-id="fc109-1033">Fixed issue with missing account key for `storage container generate-sas`</span></span>
* <span data-ttu-id="fc109-1034">Problem mit `storage blob sync` unter Linux behoben</span><span class="sxs-lookup"><span data-stu-id="fc109-1034">Fixed issue with `storage blob sync` on Linux</span></span>

### <a name="vm"></a><span data-ttu-id="fc109-1035">VM</span><span class="sxs-lookup"><span data-stu-id="fc109-1035">VM</span></span>
* <span data-ttu-id="fc109-1036">[VORSCHAU] Befehle vom Typ `vm image template` zum Erstellen von VM-Images hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1036">[PREVIEW] Added `vm image template` commands to build VM images</span></span>

## <a name="june-4-2019"></a><span data-ttu-id="fc109-1037">4\. Juni 2019</span><span class="sxs-lookup"><span data-stu-id="fc109-1037">June 4, 2019</span></span>

<span data-ttu-id="fc109-1038">Version 2.0.66</span><span class="sxs-lookup"><span data-stu-id="fc109-1038">Version 2.0.66</span></span>

### <a name="core"></a><span data-ttu-id="fc109-1039">Core</span><span class="sxs-lookup"><span data-stu-id="fc109-1039">Core</span></span>
* <span data-ttu-id="fc109-1040">Fehler behoben, aufgrund dessen bei Befehlen ein Fehler auftrat, wenn `--output yaml` mit `--query` verwendet wurde</span><span class="sxs-lookup"><span data-stu-id="fc109-1040">Fixed bug where commands fail if `--output yaml` is used with `--query`</span></span>

### <a name="acr"></a><span data-ttu-id="fc109-1041">ACR</span><span class="sxs-lookup"><span data-stu-id="fc109-1041">ACR</span></span>
* <span data-ttu-id="fc109-1042">Befehlsgruppe „acr pack“ zum Erstellen von Aufgaben zur Schnellerstellung mit Buildpacks hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1042">Added 'acr pack' command group for creating quick build Tasks using Buildpacks.</span></span>

### <a name="acs"></a><span data-ttu-id="fc109-1043">ACS</span><span class="sxs-lookup"><span data-stu-id="fc109-1043">ACS</span></span>
* <span data-ttu-id="fc109-1044">Zulassen der Aktivierung/Deaktivierung des AKS-Add-Ons für das Kube-Dashboard</span><span class="sxs-lookup"><span data-stu-id="fc109-1044">Allow enabling/disabling AKS kube-dashboard addon</span></span>
* <span data-ttu-id="fc109-1045">Ausgeben einer benutzerfreundlichen Nachricht, wenn das Abonnement nicht in der Whitelist zur Verwendung von Azure Red Hat OpenShift enthalten ist</span><span class="sxs-lookup"><span data-stu-id="fc109-1045">Print a friendly message when the subscription is not whitelisted to use Azure Red Hat OpenShift</span></span>

### <a name="batch"></a><span data-ttu-id="fc109-1046">Batch</span><span class="sxs-lookup"><span data-stu-id="fc109-1046">Batch</span></span>
* <span data-ttu-id="fc109-1047">Bessere Fehlerbehandlung, wenn der Benutzer nicht bei einem Konto angemeldet ist \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span><span class="sxs-lookup"><span data-stu-id="fc109-1047">Improved error handling when not logged in to an account \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span></span>

### <a name="iot"></a><span data-ttu-id="fc109-1048">IoT</span><span class="sxs-lookup"><span data-stu-id="fc109-1048">IoT</span></span>
* <span data-ttu-id="fc109-1049">Unterstützung für manuelles Failover hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1049">Added support for manual failover</span></span>

### <a name="network"></a><span data-ttu-id="fc109-1050">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="fc109-1050">Network</span></span>
* <span data-ttu-id="fc109-1051">Befehle vom Typ `network application-gateway waf-policy` hinzugefügt, um benutzerdefinierte WAF-Regeln zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="fc109-1051">Added `network application-gateway waf-policy` commands to support custom WAF rules.</span></span>
* <span data-ttu-id="fc109-1052">Argumente `--waf-policy` und `--max-capacity` zu `network application-gateway [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1052">Added `--waf-policy` and `--max-capacity` arguments to `network application-gateway [create|update]`</span></span> 

### <a name="resource"></a><span data-ttu-id="fc109-1053">Resource</span><span class="sxs-lookup"><span data-stu-id="fc109-1053">Resource</span></span>
* <span data-ttu-id="fc109-1054">Verbesserte Fehlermeldungen aus `deployment create`, wenn TTY nicht verfügbar ist</span><span class="sxs-lookup"><span data-stu-id="fc109-1054">Improved error message from `deployment create` when there is no TTY available</span></span>

### <a name="role"></a><span data-ttu-id="fc109-1055">Role</span><span class="sxs-lookup"><span data-stu-id="fc109-1055">Role</span></span>
* <span data-ttu-id="fc109-1056">Hilfetext aktualisiert</span><span class="sxs-lookup"><span data-stu-id="fc109-1056">Updated help text.</span></span>

### <a name="compute"></a><span data-ttu-id="fc109-1057">Compute</span><span class="sxs-lookup"><span data-stu-id="fc109-1057">Compute</span></span>
* <span data-ttu-id="fc109-1058">Unterstützung zu `vm create` für virtuelle Computer aus einem verwalteten Image mit Datenträger-LUNs hinzugefügt, die nicht bei 0 beginnen oder die Nummern überspringen</span><span class="sxs-lookup"><span data-stu-id="fc109-1058">Added support to `vm create` for VMs from a managed image with data-disk luns that do not start from 0 or that skip numbers</span></span>

## <a name="may-21-2019"></a><span data-ttu-id="fc109-1059">21. Mai 2019</span><span class="sxs-lookup"><span data-stu-id="fc109-1059">May 21, 2019</span></span>

<span data-ttu-id="fc109-1060">Version 2.0.65</span><span class="sxs-lookup"><span data-stu-id="fc109-1060">Version 2.0.65</span></span>

### <a name="core"></a><span data-ttu-id="fc109-1061">Core</span><span class="sxs-lookup"><span data-stu-id="fc109-1061">Core</span></span>
* <span data-ttu-id="fc109-1062">Besseres Feedback für Authentifizierungsfehler hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1062">Added better feedback for authentication errors</span></span>
* <span data-ttu-id="fc109-1063">Problem behoben, aufgrund dessen die CLI Erweiterungen lädt, die nicht mit der Core-Version kompatibel waren</span><span class="sxs-lookup"><span data-stu-id="fc109-1063">Fixed issue where the CLI would load extensions that were not compatible with its core version</span></span>
* <span data-ttu-id="fc109-1064">Problem beim Starten behoben, wenn `clouds.config` beschädigt ist</span><span class="sxs-lookup"><span data-stu-id="fc109-1064">Fixed issue with launching when `clouds.config` is corrupted</span></span>

### <a name="acr"></a><span data-ttu-id="fc109-1065">ACR</span><span class="sxs-lookup"><span data-stu-id="fc109-1065">ACR</span></span>
* <span data-ttu-id="fc109-1066">Unterstützung für verwaltete Identitäten zu Aufgaben hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1066">Added support for Managed Identities to Tasks</span></span>

### <a name="acs"></a><span data-ttu-id="fc109-1067">ACS</span><span class="sxs-lookup"><span data-stu-id="fc109-1067">ACS</span></span>
* <span data-ttu-id="fc109-1068">`openshift create`-Befehl bei der Verwendung mit dem AAD-Kundenclient korrigiert</span><span class="sxs-lookup"><span data-stu-id="fc109-1068">Fixed `openshift create` command when used with customer AAD client</span></span>

### <a name="appservice"></a><span data-ttu-id="fc109-1069">AppService</span><span class="sxs-lookup"><span data-stu-id="fc109-1069">AppService</span></span>
* <span data-ttu-id="fc109-1070">[VERALTET] Befehl `functionapp devops-build` als veraltet gekennzeichnet – wird in der nächsten Version entfernt</span><span class="sxs-lookup"><span data-stu-id="fc109-1070">[DEPRECATED] Deprecated `functionapp devops-build` command - will be removed in next release</span></span>
* <span data-ttu-id="fc109-1071">`functionapp devops-pipeline` geändert, um das Buildprotokoll von Azure DevOps im ausführlichen Modus abzurufen</span><span class="sxs-lookup"><span data-stu-id="fc109-1071">Changed `functionapp devops-pipeline` to fetch build log from Azure DevOps in verbose mode</span></span>
* <span data-ttu-id="fc109-1072">[BREAKING CHANGE] Flag `--use_local_settings` aus dem Befehl `functionapp devops-pipeline` entfernt – kein Vorgang wurde ausgeführt</span><span class="sxs-lookup"><span data-stu-id="fc109-1072">[BREAKING CHANGE] Removed `--use_local_settings` flag from `functionapp devops-pipeline` command - was a no-op</span></span>
* <span data-ttu-id="fc109-1073">`webapp up` geändert, sodass die JSON-Ausgabe zurückgegeben wird, wenn `--logs` nicht verwendet wird</span><span class="sxs-lookup"><span data-stu-id="fc109-1073">Changed `webapp up` to return JSON output if `--logs` is not used</span></span>
* <span data-ttu-id="fc109-1074">Unterstützung hinzugefügt zum Schreiben von Standardressourcen in die lokale Konfiguration für `webapp up`</span><span class="sxs-lookup"><span data-stu-id="fc109-1074">Added support for writing default resources to local config for `webapp up`</span></span>
* <span data-ttu-id="fc109-1075">Unterstützung zu `webapp up` hinzugefügt für die erneute Bereitstellung einer App ohne Verwendung des `--location`-Arguments</span><span class="sxs-lookup"><span data-stu-id="fc109-1075">Added support to `webapp up` for redeploying an app without using the `--location` argument</span></span>
* <span data-ttu-id="fc109-1076">Problem behoben, bei dem für die ASP-Erstellung der Linux-SKU „Free“ der SKU-Wert „Free“ nicht funktioniert hat</span><span class="sxs-lookup"><span data-stu-id="fc109-1076">Fixed an issue where for Linux Free SKU ASP creation use Free as SKU value was not working</span></span>

### <a name="botservice"></a><span data-ttu-id="fc109-1077">BotService</span><span class="sxs-lookup"><span data-stu-id="fc109-1077">BotService</span></span>
* <span data-ttu-id="fc109-1078">Geändert, sodass Groß-/Kleinschreibung für `--lang`-Parameter für Befehle zulässig ist</span><span class="sxs-lookup"><span data-stu-id="fc109-1078">Changed to allow all casing for `--lang` parameters for commands</span></span>
* <span data-ttu-id="fc109-1079">Beschreibung für das Befehlsmodul aktualisiert</span><span class="sxs-lookup"><span data-stu-id="fc109-1079">Updated description for command module</span></span>

### <a name="consumption"></a><span data-ttu-id="fc109-1080">Nutzung</span><span class="sxs-lookup"><span data-stu-id="fc109-1080">Consumption</span></span>
* <span data-ttu-id="fc109-1081">Fehlende erforderliche Parameter bei der Ausführung von `consumption usage list --billing-period-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1081">Added missing required parameter when running `consumption usage list --billing-period-name`</span></span>

### <a name="iot"></a><span data-ttu-id="fc109-1082">IoT</span><span class="sxs-lookup"><span data-stu-id="fc109-1082">IoT</span></span>
* <span data-ttu-id="fc109-1083">Unterstützung für das Auflisten aller Schlüssel hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1083">Added support to list all keys</span></span>

### <a name="network"></a><span data-ttu-id="fc109-1084">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="fc109-1084">Network</span></span>
* [BREAKING CHANGE]: Removed `network interface-endpoints` command group - use `network private-endpoints` 
* <span data-ttu-id="fc109-1086">`--nat-gateway`-Argument zu `network vnet subnet [create|update]` für das Anfügen an ein NAT-Gateway hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1086">Added `--nat-gateway` argument to `network vnet subnet [create|update]` for attaching to a NAT gateway</span></span>
* <span data-ttu-id="fc109-1087">Problem mit `dns zone import` behoben, aufgrund dessen Eintragsnamen keinem Datensatztyp entsprochen haben</span><span class="sxs-lookup"><span data-stu-id="fc109-1087">Fixed issue with `dns zone import` where record names could not match a record type</span></span>

### <a name="rdbms"></a><span data-ttu-id="fc109-1088">RDBMS</span><span class="sxs-lookup"><span data-stu-id="fc109-1088">RDBMS</span></span>
* <span data-ttu-id="fc109-1089">Postgres- und MySLQ-Unterstützung für die Georeplikation hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1089">Added postgres and mysql support for geo replication</span></span>

### <a name="rbac"></a><span data-ttu-id="fc109-1090">RBAC</span><span class="sxs-lookup"><span data-stu-id="fc109-1090">RBAC</span></span>
* <span data-ttu-id="fc109-1091">Unterstützung für den Verwaltungsgruppenumfang zu `role assignment` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1091">Added support for management group scope to `role assignment`</span></span>

### <a name="storage"></a><span data-ttu-id="fc109-1092">Storage</span><span class="sxs-lookup"><span data-stu-id="fc109-1092">Storage</span></span>
* <span data-ttu-id="fc109-1093">`storage blob sync`: Synchronisierungsbefehl für Speicherblob hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1093">`storage blob sync`: add sync command for storage blob</span></span>

### <a name="compute"></a><span data-ttu-id="fc109-1094">Compute</span><span class="sxs-lookup"><span data-stu-id="fc109-1094">Compute</span></span>
* <span data-ttu-id="fc109-1095">`--computer-name` zu `vm create` zum Festlegen des Computernamens eines virtuellen Computers hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1095">Added `--computer-name` to `vm create` for setting a VM's computer name</span></span>
* <span data-ttu-id="fc109-1096">`--ssh-key-value` umbenannt in `--ssh-key-values` für `[vm|vmss] create`: Jetzt können mehrere öffentliche SSH-Schlüsselwerte oder -pfade akzeptiert werden.</span><span class="sxs-lookup"><span data-stu-id="fc109-1096">Renamed `--ssh-key-value` renamed to `--ssh-key-values` for `[vm|vmss] create` - can now accept multiple ssh public key values or paths</span></span>
  * <span data-ttu-id="fc109-1097">__Hinweis__: Dies ist **kein** Breaking Change: `--ssh-key-value` wird korrekt analysiert, da nur eine Übereinstimmung mit `--ssh-key-values` besteht.</span><span class="sxs-lookup"><span data-stu-id="fc109-1097">__Note__: This is **not** a breaking change - `--ssh-key-value` will be parsed correctly as it matches only `--ssh-key-values`</span></span>
* <span data-ttu-id="fc109-1098">`--type`-Argument von `ppg create` in optionales Argument geändert</span><span class="sxs-lookup"><span data-stu-id="fc109-1098">Changed the `--type` argument of `ppg create` to be optional</span></span>

## <a name="may-6-2019"></a><span data-ttu-id="fc109-1099">6\. Mai 2019</span><span class="sxs-lookup"><span data-stu-id="fc109-1099">May 6, 2019</span></span>

<span data-ttu-id="fc109-1100">Version 2.0.64</span><span class="sxs-lookup"><span data-stu-id="fc109-1100">Version 2.0.64</span></span>

### <a name="acs"></a><span data-ttu-id="fc109-1101">ACS</span><span class="sxs-lookup"><span data-stu-id="fc109-1101">ACS</span></span>
* <span data-ttu-id="fc109-1102">[BREAKING CHANGE] Flag `--fqdn` aus den `openshift`-Befehlen entfernt</span><span class="sxs-lookup"><span data-stu-id="fc109-1102">[BREAKING CHANGE] Removed `--fqdn` flag on `openshift` commands</span></span>
* <span data-ttu-id="fc109-1103">Geändert, sodass die allgemein verfügbare Azure Red Hat Openshift-API-Version verwendet wird</span><span class="sxs-lookup"><span data-stu-id="fc109-1103">Changed to use Azure Red Hat Openshift GA API Version</span></span>
* <span data-ttu-id="fc109-1104">Flag `customer-admin-group-id` wurde zu `openshift create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-1104">Added `customer-admin-group-id` flag to `openshift create`</span></span>
* <span data-ttu-id="fc109-1105">[ALLGEMEIN VERFÜGBAR] `(PREVIEW)` aus der `aks create`-Option `--network-policy` entfernt</span><span class="sxs-lookup"><span data-stu-id="fc109-1105">[GA] Removed `(PREVIEW)` from `aks create` option `--network-policy`</span></span>

### <a name="appservice"></a><span data-ttu-id="fc109-1106">AppService</span><span class="sxs-lookup"><span data-stu-id="fc109-1106">Appservice</span></span>
* <span data-ttu-id="fc109-1107">[VERALTET] Befehl `functionapp devops-build` als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="fc109-1107">[DEPRECATED] Deprecated `functionapp devops-build` command</span></span>
  * <span data-ttu-id="fc109-1108">Umbenannt in `functionapp devops-pipeline`</span><span class="sxs-lookup"><span data-stu-id="fc109-1108">Renamed to `functionapp devops-pipeline`</span></span>
* <span data-ttu-id="fc109-1109">Fehler beim Abrufen des richtigen Benutzernamens für Cloud Shell behoben, der einen Fehler von `webapp up` verursachte</span><span class="sxs-lookup"><span data-stu-id="fc109-1109">Fixed getting the correct username for cloudshell which was causing `webapp up` to fail</span></span>
* <span data-ttu-id="fc109-1110">Dokumentation von `appservice plan --sku` mit den unterstützten App Service-Plänen aktualisiert</span><span class="sxs-lookup"><span data-stu-id="fc109-1110">Updated `appservice plan --sku` documentation updated to reflect the supported appserviceplans</span></span>
* <span data-ttu-id="fc109-1111">Optionale Argumente für Ressourcengruppe und Plan zu `webapp up` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1111">Added optional arguments for resource group and plan to `webapp up`</span></span>
* <span data-ttu-id="fc109-1112">Unterstützung zur Berücksichtigung der Umgebungsvariablen `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` zu `webapp ssh` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1112">Added support to `webapp ssh` to respect `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>
* <span data-ttu-id="fc109-1113">Unterstützung für `appserviceplan create` für die kostenlose Linux-SKU hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1113">Added `appserviceplan create` support for Linux Free SKU</span></span>
* <span data-ttu-id="fc109-1114">`webapp up` geändert, um nach dem Festlegen der App-Einstellung `SCM_DO_BUILD_DURING_DEPLOYMENT=true` zum Verarbeiten des Kudu-Kaltstarts für 30 Sekunden in den Energiesparmodus zu wechseln</span><span class="sxs-lookup"><span data-stu-id="fc109-1114">Changed `webapp up` to have a 30s sleep after setting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` appsetting to handle kudu cold start</span></span>
* <span data-ttu-id="fc109-1115">Unterstützung für die `powershell`-Runtime zu `functionapp create` unter Windows hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1115">Added support for `powershell` runtime to `functionapp create` on Windows</span></span>
* <span data-ttu-id="fc109-1116">Befehl `create-remote-connection` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1116">Added `create-remote-connection` command</span></span>

### <a name="batch"></a><span data-ttu-id="fc109-1117">Batch</span><span class="sxs-lookup"><span data-stu-id="fc109-1117">Batch</span></span>
* <span data-ttu-id="fc109-1118">Fehler im Validierungssteuerelement für `--application-package-references`-Optionen korrigiert</span><span class="sxs-lookup"><span data-stu-id="fc109-1118">Fixed bug in validator for `--application-package-references` options</span></span>

### <a name="botservice"></a><span data-ttu-id="fc109-1119">Botservice</span><span class="sxs-lookup"><span data-stu-id="fc109-1119">Botservice</span></span>
* <span data-ttu-id="fc109-1120">[BREAKING CHANGE]`bot create -v v4 -k webapp` geändert, sodass standardmäßig eine leerer Web-App-Bot erstellt wird (d. h. kein Bot wird in App Service bereitgestellt)</span><span class="sxs-lookup"><span data-stu-id="fc109-1120">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to create an empty Web App Bot by default (i.e. no bot is deployed to the App Service)</span></span>
* <span data-ttu-id="fc109-1121">`--echo`-Flag zu `bot create` hinzugefügt, sodass das alte Verhalten mit `-v v4` verwendet wird</span><span class="sxs-lookup"><span data-stu-id="fc109-1121">Added `--echo` flag to `bot create` to use the old behavior with `-v v4`</span></span>
* <span data-ttu-id="fc109-1122">[BREAKING CHANGE] Standardwert von `--version` in `v4` geändert</span><span class="sxs-lookup"><span data-stu-id="fc109-1122">[BREAKING CHANGE] Changed the default value of  `--version` to `v4`</span></span>
  * <span data-ttu-id="fc109-1123">__HINWEIS:__ `bot prepare-publish` verwendet weiterhin den alten Standard.</span><span class="sxs-lookup"><span data-stu-id="fc109-1123">__NOTE:__ `bot prepare-publish` still uses the its old default</span></span>
* <span data-ttu-id="fc109-1124">[BREAKING CHANGE]`--lang` geändert, sodass der Standard nicht mehr `Csharp` ist.</span><span class="sxs-lookup"><span data-stu-id="fc109-1124">[BREAKING CHANGE] Changed `--lang` to no longer default to `Csharp`.</span></span> <span data-ttu-id="fc109-1125">Wenn der Befehl `--lang` erfordert und dies nicht angegeben ist, wird der Befehl nun mit Fehler beendet.</span><span class="sxs-lookup"><span data-stu-id="fc109-1125">If the command requires `--lang` and it is not provided, the command will now error out</span></span>
* <span data-ttu-id="fc109-1126">[BREAKING CHANGE]`--appid`- und `--password`-Argumente für `bot create` in erforderlich geändert, sie können jetzt über `ad app create` erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="fc109-1126">[BREAKING CHANGE] Changed the `--appid` and `--password` args for `bot create` to be required and can now be created via `ad app create`</span></span>
* <span data-ttu-id="fc109-1127">`--appid`- und `--password`-Validierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1127">Added `--appid` and `--password` validation</span></span>
* <span data-ttu-id="fc109-1128">[BREAKING CHANGE]`bot create -v v4` geändert, sodass kein Speicherkonto bzw. keine Application Insights-Instanz erstellt oder verwendet wird</span><span class="sxs-lookup"><span data-stu-id="fc109-1128">[BREAKING CHANGE] Changed `bot create -v v4` to not create or use a Storage Account or Application Insights</span></span>
* <span data-ttu-id="fc109-1129">[BREAKING CHANGE]`bot create -v v3` geändert, sodass eine Region erforderlich ist, in der Application Insights verfügbar ist</span><span class="sxs-lookup"><span data-stu-id="fc109-1129">[BREAKING CHANGE] Changed `bot create -v v3` to require a region where Application Insights is available</span></span>
* <span data-ttu-id="fc109-1130">[BREAKING CHANGE]`bot update` geändert, sodass es sich jetzt nur auf spezifische Eigenschaften eines Bots auswirkt</span><span class="sxs-lookup"><span data-stu-id="fc109-1130">[BREAKING CHANGE] Changed `bot update` to now affect only specific properties of a bot</span></span>
* <span data-ttu-id="fc109-1131">[BREAKING CHANGE]`--lang`-Flags geändert, sodass `Javascript` anstelle von `Node` akzeptiert wird</span><span class="sxs-lookup"><span data-stu-id="fc109-1131">[BREAKING CHANGE] Changed `--lang` flags to accept `Javascript` instead of `Node`</span></span>
* <span data-ttu-id="fc109-1132">[BREAKING CHANGE]`Node` als zulässiger `--lang`-Wert entfernt.</span><span class="sxs-lookup"><span data-stu-id="fc109-1132">[BREAKING CHANGE] Removed `Node` as an allowed `--lang` value</span></span>
* <span data-ttu-id="fc109-1133">[BREAKING CHANGE]`bot create -v v4 -k webapp` geändert, sodass `SCM_DO_BUILD_DURING_DEPLOYMENT` nicht mehr auf TRUE festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="fc109-1133">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to no longer set `SCM_DO_BUILD_DURING_DEPLOYMENT` to true.</span></span> <span data-ttu-id="fc109-1134">Alle Bereitstellungen über Kudu fungieren ihrem Standardverhalten entsprechend.</span><span class="sxs-lookup"><span data-stu-id="fc109-1134">All deployments through Kudu will act according to their default behavior</span></span>
* <span data-ttu-id="fc109-1135">`bot download` für Bots ohne `.bot`-Dateien geändert, sodass die sprachspezifische Konfigurationsdatei mit Werten aus den Anwendungseinstellungen für den Bot erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="fc109-1135">Changed `bot download` for bots without `.bot` files to create the language-specific configuration file with values from the Application Settings for the bot</span></span>
* <span data-ttu-id="fc109-1136">Unterstützung für `Typescript` zu `bot prepare-deploy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1136">Added `Typescript` support to `bot prepare-deploy`</span></span>
* <span data-ttu-id="fc109-1137">Warnmeldung zu `bot prepare-deploy` für `Javascript`- und `Typescript`-Bots hinzugefügt, wenn `package.json` in `--code-dir` nicht enthalten ist</span><span class="sxs-lookup"><span data-stu-id="fc109-1137">Added warning message to `bot prepare-deploy` for `Javascript` and `Typescript` bots for when `--code-dir` does not contain `package.json`</span></span>
* <span data-ttu-id="fc109-1138">`bot prepare-deploy` geändert, sodass bei Erfolg `true` zurückgegeben wird</span><span class="sxs-lookup"><span data-stu-id="fc109-1138">Changed `bot prepare-deploy` to return `true` if successful</span></span>
* <span data-ttu-id="fc109-1139">Ausführliche Protokollierung zu `bot prepare-deploy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1139">Added verbose logging to `bot prepare-deploy`</span></span>
* <span data-ttu-id="fc109-1140">Mehr verfügbare Application Insights-Regionen zu `az bot create -v v3` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1140">Added more available Application Insights regions to `az bot create -v v3`</span></span>

### <a name="configure"></a><span data-ttu-id="fc109-1141">Konfigurieren</span><span class="sxs-lookup"><span data-stu-id="fc109-1141">Configure</span></span>
* <span data-ttu-id="fc109-1142">Unterstützung für die ordnerbasierte Argument-Standardwertkonfigurationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1142">Added support for folder based argument default value configurations</span></span>

### <a name="eventhubs"></a><span data-ttu-id="fc109-1143">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="fc109-1143">Eventhubs</span></span>
* <span data-ttu-id="fc109-1144">Befehle vom Typ `namespace network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1144">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="fc109-1145">`--default-action`-Argument für Netzwerkregeln zu `namespace [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1145">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="fc109-1146">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="fc109-1146">Network</span></span>
* <span data-ttu-id="fc109-1147">[BREAKING CHANGE]`--cache`-Argument mit `--defer` für `vnet [create|update]` ersetzt</span><span class="sxs-lookup"><span data-stu-id="fc109-1147">[BREAKING CHANGE] Replaced `--cache` arugment with `--defer` for `vnet [create|update]`</span></span> 

### <a name="policy-insights"></a><span data-ttu-id="fc109-1148">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="fc109-1148">Policy Insights</span></span>
* <span data-ttu-id="fc109-1149">Unterstützung für `--expand PolicyEvaluationDetails` hinzugefügt, sodass Richtlinienauswertungsdetails von der Ressource abgefragt werden</span><span class="sxs-lookup"><span data-stu-id="fc109-1149">Added support for `--expand PolicyEvaluationDetails` to query policy evaluation details on the resource</span></span>

### <a name="role"></a><span data-ttu-id="fc109-1150">Role</span><span class="sxs-lookup"><span data-stu-id="fc109-1150">Role</span></span>
* <span data-ttu-id="fc109-1151">[VERALTET]: Ausblenden des „--password"-Arguments von `create-for-rbac` geändert; Unterstützung wird im Mai 2019 entfernt</span><span class="sxs-lookup"><span data-stu-id="fc109-1151">[DEPRECATED] Changed `create-for-rbac` hide '--password' argument - support will be removed in May 2019</span></span>

### <a name="service-bus"></a><span data-ttu-id="fc109-1152">Service Bus</span><span class="sxs-lookup"><span data-stu-id="fc109-1152">Service Bus</span></span>
* <span data-ttu-id="fc109-1153">Befehle vom Typ `namespace network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1153">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="fc109-1154">`--default-action`-Argument für Netzwerkregeln zu `namespace [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1154">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>
* <span data-ttu-id="fc109-1155">`topic [create|update]` korrigiert, sodass `--max-size`-Unterstützung für 10-, 20-, 40- und 80-GB-Werte mit Premium-SKU zulässig ist</span><span class="sxs-lookup"><span data-stu-id="fc109-1155">Fixed `topic [create|update]` to allow `--max-size` support for 10, 20, 40 and 80GB values with premium SKU</span></span>

### <a name="sql"></a><span data-ttu-id="fc109-1156">SQL</span><span class="sxs-lookup"><span data-stu-id="fc109-1156">SQL</span></span>
* <span data-ttu-id="fc109-1157">Befehle vom Typ `sql virtual-cluster [list|show|delete]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1157">Added `sql virtual-cluster [list|show|delete]` commands</span></span>

### <a name="vm"></a><span data-ttu-id="fc109-1158">VM</span><span class="sxs-lookup"><span data-stu-id="fc109-1158">VM</span></span>
* <span data-ttu-id="fc109-1159">`--protect-from-scale-in` und `--protect-from-scale-set-actions` zu `vmss update` hinzugefügt, sodass Aktualisierungen der Schutzrichtlinie von VMSS-VM-Instanzen aktiviert sind</span><span class="sxs-lookup"><span data-stu-id="fc109-1159">Added `--protect-from-scale-in` and `--protect-from-scale-set-actions` to `vmss update` to enable updates to the protection policy of VMSS VM instances</span></span>
* <span data-ttu-id="fc109-1160">`--instance-id` zu `vmss update` hinzugefügt, sodass allgemeine Aktualisierungen von VMSS-VM-Instanzen aktiviert sind</span><span class="sxs-lookup"><span data-stu-id="fc109-1160">Added `--instance-id` to `vmss update` to enable generic update of VMSS VM instances</span></span>
* <span data-ttu-id="fc109-1161">`--instance-id` zu `vmss wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1161">Added `--instance-id` to `vmss wait`</span></span>
* <span data-ttu-id="fc109-1162">Neue `ppg`-Befehlsgruppe für die Verwaltung von Näherungsplatzierungsgruppen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1162">Added new `ppg` command group for managing Proximity Placement Groups</span></span>
* <span data-ttu-id="fc109-1163">`--ppg` zu `[vm|vmss] create` und `vm availability-set create` für die Verwaltung von PPGs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1163">Added `--ppg` to `[vm|vmss] create` and `vm availability-set create` for managing PPGs</span></span>
* <span data-ttu-id="fc109-1164">Parameter `--hyper-v-generation` zu `image create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1164">Added `--hyper-v-generation` parameter to `image create`</span></span>

## <a name="april-23-2019"></a><span data-ttu-id="fc109-1165">23. April 2019</span><span class="sxs-lookup"><span data-stu-id="fc109-1165">April 23, 2019</span></span>

<span data-ttu-id="fc109-1166">Version 2.0.63</span><span class="sxs-lookup"><span data-stu-id="fc109-1166">Version 2.0.63</span></span>

### <a name="acs"></a><span data-ttu-id="fc109-1167">ACS</span><span class="sxs-lookup"><span data-stu-id="fc109-1167">ACS</span></span>
* <span data-ttu-id="fc109-1168">`aks get-credentials` zur Anzeige einer Eingabeaufforderung zum Überschreiben doppelter Werte geändert</span><span class="sxs-lookup"><span data-stu-id="fc109-1168">Changed `aks get-credentials` to prompt to overwrite duplicated values</span></span>
* <span data-ttu-id="fc109-1169">`(PREVIEW)` aus Dev Spaces-Befehlen „aks use-dev-spaces“ und „aks remove-dev-spaces“ entfernt</span><span class="sxs-lookup"><span data-stu-id="fc109-1169">Removed `(PREVIEW)` from Dev Spaces commands "aks use-dev-spaces" and "aks remove-dev-spaces"</span></span>

### <a name="ams"></a><span data-ttu-id="fc109-1170">AMS</span><span class="sxs-lookup"><span data-stu-id="fc109-1170">AMS</span></span>
* <span data-ttu-id="fc109-1171">Fehler bei der Objekt- und Kontofilteraktualisierung behoben</span><span class="sxs-lookup"><span data-stu-id="fc109-1171">Fixed bug with asset and account filters update</span></span>

### <a name="appservice"></a><span data-ttu-id="fc109-1172">AppService</span><span class="sxs-lookup"><span data-stu-id="fc109-1172">AppService</span></span>
* <span data-ttu-id="fc109-1173">Unterstützung für die App Service-Umgebung (App Service Environment, ASE) und Zeitlimit zu `webapp ssh` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1173">Added support for ASE and timeout to `webapp ssh`</span></span>
* <span data-ttu-id="fc109-1174">Unterstützung für die Einrichtung von CI/CD für eine Azure DevOps-Pipeline aus einem GitHub-Repository zu Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1174">Added support for establishing CI CD to an Azure DevOps pipeline from a Github repository to Function apps</span></span>
* <span data-ttu-id="fc109-1175">`--github-pat`-Argument zu `functionapp devops-build create` hinzugefügt, um persönliche GitHub-Zugriffstoken zu akzeptieren</span><span class="sxs-lookup"><span data-stu-id="fc109-1175">Added `--github-pat` argument to `functionapp devops-build create` to accept Github personal access token</span></span>
* <span data-ttu-id="fc109-1176">`--github-repository`-Argument zu `functionapp devops-build create` hinzugefügt, um das GitHub-Repository mit dem Quellcode einer Funktions-App zu akzeptieren</span><span class="sxs-lookup"><span data-stu-id="fc109-1176">Added `--github-repository` argument to `functionapp devops-build create` to accept Github repository that contains a functionapp source code</span></span>
* <span data-ttu-id="fc109-1177">Problem behoben, aufgrund dessen bei `az webapp up --logs` ein Fehler auftrat und die .NET Core-Standardversion auf 2.1 aktualisiert wurde</span><span class="sxs-lookup"><span data-stu-id="fc109-1177">Fixed issue where `az webapp up --logs` was failing with a error and updating default .NETCORE version to 2.1</span></span>
* <span data-ttu-id="fc109-1178">Unnötige Funktions-App-Einstellungen beim Erstellen einer Funktions-App mit Verbrauchsplan entfernt</span><span class="sxs-lookup"><span data-stu-id="fc109-1178">Removed unnecessary functionapp settings when creating a function app with consumption plan</span></span>
* <span data-ttu-id="fc109-1179">`webapp up` geändert, sodass die ASP-Standardzeichenfolge jetzt eine Zahl am Ende anfügt, um einen neuen ASP basierend auf SKU-Optionen zu erstellen</span><span class="sxs-lookup"><span data-stu-id="fc109-1179">Changed `webapp up` so the default asp string now appends number at the end to create a new ASP based on SKU options</span></span>
* <span data-ttu-id="fc109-1180">`-b` als Option für `webapp up` hinzugefügt, um die App im Browser zu starten</span><span class="sxs-lookup"><span data-stu-id="fc109-1180">Added `-b` as an option to `webapp up` to launch the app in the browser</span></span>
* <span data-ttu-id="fc109-1181">`webapp deployment source config zip` geändert, um die `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`-Umgebungsvariable zu behandeln</span><span class="sxs-lookup"><span data-stu-id="fc109-1181">Changed `webapp deployment source config zip` to handle `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="fc109-1182">Bereitstellungs-Manager</span><span class="sxs-lookup"><span data-stu-id="fc109-1182">Deployment Manager</span></span>
* <span data-ttu-id="fc109-1183">[VORSCHAUVERSIPN] Erstellen und Verwalten von Artefakten, die Rollouts unterstützen</span><span class="sxs-lookup"><span data-stu-id="fc109-1183">[PREVIEW] Create and manage artifacts that support rollouts</span></span>

### <a name="lab"></a><span data-ttu-id="fc109-1184">Labor</span><span class="sxs-lookup"><span data-stu-id="fc109-1184">Lab</span></span>
* <span data-ttu-id="fc109-1185">Fehler behoben, der zu einer vorzeitigen Beendigung führen würde</span><span class="sxs-lookup"><span data-stu-id="fc109-1185">Fixed bug which would cause an early exit</span></span>

### <a name="network"></a><span data-ttu-id="fc109-1186">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="fc109-1186">Network</span></span>
* <span data-ttu-id="fc109-1187">Automatische Delegierung des Namenservers im übergeordneten Element während der Erstellung der untergeordneten Zone zu `dns zone create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1187">Added auto name server delegation to `dns zone create` in parent during child zone creation</span></span>

### <a name="resource"></a><span data-ttu-id="fc109-1188">Resource</span><span class="sxs-lookup"><span data-stu-id="fc109-1188">Resource</span></span>
* <span data-ttu-id="fc109-1189">[VERALTET]: Argumente `--link-id`, `--target-id` und `--filter-string` von `resource link` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="fc109-1189">[DEPRECATED] Deprecated `--link-id`, `--target-id` and `--filter-string` arguments of `resource link`</span></span>
  * <span data-ttu-id="fc109-1190">Verwenden Sie stattdessen die Argumente `--link`, `--target` und `--filter`.</span><span class="sxs-lookup"><span data-stu-id="fc109-1190">Use the arguments `--link`, `--target`, and `--filter` instead</span></span>
* <span data-ttu-id="fc109-1191">Problem behoben, aufgrund dessen `resource link [create|update]`-Befehle nicht verwendet werden konnten</span><span class="sxs-lookup"><span data-stu-id="fc109-1191">Fixed issue where `resource link [create|update]` commands would not work</span></span>
* <span data-ttu-id="fc109-1192">Problem behoben, aufgrund dessen das Löschen anhand einer Ressourcen-ID bei einem Fehler zu einem Absturz führen konnte</span><span class="sxs-lookup"><span data-stu-id="fc109-1192">Fixed an issue where deleting using a resource ID could crash on error</span></span>

### <a name="sql"></a><span data-ttu-id="fc109-1193">SQL</span><span class="sxs-lookup"><span data-stu-id="fc109-1193">SQL</span></span>
* <span data-ttu-id="fc109-1194">Unterstützung für benutzerdefinierte Zeitzonen auf verwalteten Instanzen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1194">Added support for custom time zone on managed instances</span></span>
* <span data-ttu-id="fc109-1195">Geändert, um die Verwendung des Namens eines Pools für elastische Datenbanken mit `sql db update` zuzulassen</span><span class="sxs-lookup"><span data-stu-id="fc109-1195">Changed to allow elastic pool name to be used with `sql db update`</span></span>
* <span data-ttu-id="fc109-1196">Unterstützung für `--no-wait` zu `sql server [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1196">Added `--no-wait` support to `sql server [create|update]`</span></span>
* <span data-ttu-id="fc109-1197">Befehl `sql server wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1197">Added command `sql server wait`</span></span>

### <a name="storage"></a><span data-ttu-id="fc109-1198">Storage</span><span class="sxs-lookup"><span data-stu-id="fc109-1198">Storage</span></span>
* <span data-ttu-id="fc109-1199">Problem mit doppelt codierten SAS-Token in `storage blob generate-sas` behoben</span><span class="sxs-lookup"><span data-stu-id="fc109-1199">Fixed issue with double-encoded SAS tokens in `storage blob generate-sas`</span></span>

### <a name="vm"></a><span data-ttu-id="fc109-1200">VM</span><span class="sxs-lookup"><span data-stu-id="fc109-1200">VM</span></span>
* <span data-ttu-id="fc109-1201">`--skip-shutdown`-Flag zum Ausschalten von VMs ohne Herunterfahren zu `vm|vmss stop` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1201">Added `--skip-shutdown` flag to `vm|vmss stop` to power-off VMs without shutdown</span></span>
* <span data-ttu-id="fc109-1202">`--storage-account-type`-Argument zum Festlegen des Kontotyps des Veröffentlichungsprofils zu `sig image-version create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1202">Added `--storage-account-type` argument to `sig image-version create` to set the publishing profile's account type</span></span>
* <span data-ttu-id="fc109-1203">`--target-regions`-Argument zu `sig image-version create` hinzugefügt, um das Festlegen von regionsspezifischen Speicherkontotypen zuzulassen</span><span class="sxs-lookup"><span data-stu-id="fc109-1203">Added `--target-regions` argument to `sig image-version create` to allow setting region-specific storage account types</span></span>

## <a name="april-9-2019"></a><span data-ttu-id="fc109-1204">9\. April 2019</span><span class="sxs-lookup"><span data-stu-id="fc109-1204">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="fc109-1205">Core</span><span class="sxs-lookup"><span data-stu-id="fc109-1205">Core</span></span>
* <span data-ttu-id="fc109-1206">Problem behoben, aufgrund dessen einige Erweiterungen mit der Version `Unknown` angezeigt wurden und nicht aktualisiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="fc109-1206">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="fc109-1207">ACR</span><span class="sxs-lookup"><span data-stu-id="fc109-1207">ACR</span></span>
* <span data-ttu-id="fc109-1208">Unterstützung für die kontextlose Ausführung eines Images hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1208">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="fc109-1209">AMS</span><span class="sxs-lookup"><span data-stu-id="fc109-1209">AMS</span></span>
* [VERALTET]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
[DEPRECATED]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [BREAKING CHANGE]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="fc109-1212">Unterstützung für neue Verschlüsselungsparameter in `ams streaming-policy create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1212">Added new encryption parameters support in `ams streaming-policy create`</span></span>
* <span data-ttu-id="fc109-1213">Neuer Parameter `--filters` zu `ams streaming-locator create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1213">Added new paramter `--filters` to `ams streaming-locator create`</span></span>

### <a name="appservice"></a><span data-ttu-id="fc109-1214">AppService</span><span class="sxs-lookup"><span data-stu-id="fc109-1214">AppService</span></span>
* <span data-ttu-id="fc109-1215">Unterstützung für `--logs` zu `webapp up` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1215">Added `--logs` support to `webapp up`</span></span>
* <span data-ttu-id="fc109-1216">Probleme bei der Generierung von `azure-pipelines.yml` beim Befehl `functionapp devops-build create` behoben</span><span class="sxs-lookup"><span data-stu-id="fc109-1216">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="fc109-1217">Fehlerbehandlung und Indikatoren für `unctionapp devops-build create` verbessert</span><span class="sxs-lookup"><span data-stu-id="fc109-1217">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="fc109-1218">[BREAKING CHANGE] Flag `--local-git` für den Befehl `devops-build` entfernt; lokale Git-Erkennung und -Verarbeitung sind zum Erstellen von Azure DevOps-Pipelines obligatorisch</span><span class="sxs-lookup"><span data-stu-id="fc109-1218">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="fc109-1219">Unterstützung für das Erstellen von Linux-Functions-Plänen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1219">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="fc109-1220">Möglichkeit zum Wechseln eines Plans unter einer Funktions-App mit `functionapp update --plan` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1220">Added ability to switch a plan underneath a function app using `functionapp update --plan`</span></span>
* <span data-ttu-id="fc109-1221">Unterstützung für Einstellungen zum Aufskalieren für den Azure Functions-Premium-Plan hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1221">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="fc109-1222">CDN</span><span class="sxs-lookup"><span data-stu-id="fc109-1222">CDN</span></span>
* <span data-ttu-id="fc109-1223">Unterstützung hinzugefügt für `Microsoft_Standard` und `Standard_ChinaCdn`</span><span class="sxs-lookup"><span data-stu-id="fc109-1223">Added support for `Microsoft_Standard` and `Standard_ChinaCdn`</span></span>

### <a name="feedback"></a><span data-ttu-id="fc109-1224">Feedback</span><span class="sxs-lookup"><span data-stu-id="fc109-1224">Feedback</span></span>
* <span data-ttu-id="fc109-1225">`feedback` zur Anzeige von Metadaten zu den zuletzt ausgeführten Befehlen geändert</span><span class="sxs-lookup"><span data-stu-id="fc109-1225">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="fc109-1226">`feedback` geändert, um den Benutzer zur Unterstützung beim Issueerstellungsprozess aufzufordern (durch Öffnen eines Browsers und Verwenden einer Issuevorlage)</span><span class="sxs-lookup"><span data-stu-id="fc109-1226">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="fc109-1227">`feedback` geändert, um den Issuetext bei der Ausführung mit „--verbose“ auszugeben</span><span class="sxs-lookup"><span data-stu-id="fc109-1227">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="fc109-1228">Überwachen</span><span class="sxs-lookup"><span data-stu-id="fc109-1228">Monitor</span></span>
* <span data-ttu-id="fc109-1229">Problem behoben, aufgrund dessen „Count“ kein zulässiger Wert für `metrics alert [create|update]` war</span><span class="sxs-lookup"><span data-stu-id="fc109-1229">Fixed issue where "count" was not a permitted value with `metrics alert [create|update]`</span></span> 

### <a name="network"></a><span data-ttu-id="fc109-1230">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="fc109-1230">Network</span></span>
* <span data-ttu-id="fc109-1231">Problem behoben, aufgrund dessen das Tabellenformat mit `vnet-gateway list-bgp-peer-status` nicht angezeigt wurde</span><span class="sxs-lookup"><span data-stu-id="fc109-1231">Fixed table format not displaying with `vnet-gateway list-bgp-peer-status`</span></span>
* <span data-ttu-id="fc109-1232">Befehle `list-request-headers` und `list-response-headers` zu `application-gateway rewrite-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1232">Added `list-request-headers` and `list-response-headers` commands to `application-gateway rewrite-rule`</span></span>
* <span data-ttu-id="fc109-1233">Befehl `list-server-variables` zu `application-gateway rewrite-rule condition` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1233">Added `list-server-variables` command to `application-gateway rewrite-rule condition`</span></span>
* <span data-ttu-id="fc109-1234">Problem behoben, aufgrund dessen durch das Aktualisieren des Linkstatus für einen ExpressRoute-Port eine Ausnahme vom Typ „unbekanntes Attribut“ ausgelöst wurde: `express-route port update`</span><span class="sxs-lookup"><span data-stu-id="fc109-1234">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception `express-route port update`</span></span>

### <a name="privatedns"></a><span data-ttu-id="fc109-1235">PrivateDNS</span><span class="sxs-lookup"><span data-stu-id="fc109-1235">PrivateDNS</span></span>
* <span data-ttu-id="fc109-1236">`network private-dns` für private DNS-Zonen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1236">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="fc109-1237">Resource</span><span class="sxs-lookup"><span data-stu-id="fc109-1237">Resource</span></span>
* <span data-ttu-id="fc109-1238">Problem mit `deployment create` und `group deployment create` behoben, aufgrund dessen eine Parameterdatei mit leerem Parametersatz nicht verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="fc109-1238">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="fc109-1239">Role</span><span class="sxs-lookup"><span data-stu-id="fc109-1239">Role</span></span>
* <span data-ttu-id="fc109-1240">`create-for-rbac` korrigiert, um `--years` korrekt zu verarbeiten</span><span class="sxs-lookup"><span data-stu-id="fc109-1240">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="fc109-1241">[BREAKING CHANGE]`role assignment delete` geändert, um eine Eingabeaufforderung anzuzeigen, wenn alle Zuweisungen im Abonnement ohne Bedingungen gelöscht werden</span><span class="sxs-lookup"><span data-stu-id="fc109-1241">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="fc109-1242">SQL</span><span class="sxs-lookup"><span data-stu-id="fc109-1242">SQL</span></span>
* <span data-ttu-id="fc109-1243">`sql mi [create|update]` mit den Eigenschaften „proxyOverride“ und „publicDataEndpointEnabled“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="fc109-1243">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="fc109-1244">Storage</span><span class="sxs-lookup"><span data-stu-id="fc109-1244">Storage</span></span>
* <span data-ttu-id="fc109-1245">[BREAKING CHANGE] Ergebnis von `storage blob delete` entfernt</span><span class="sxs-lookup"><span data-stu-id="fc109-1245">[BREAKING CHANGE] Removed result of `storage blob delete`</span></span>
* <span data-ttu-id="fc109-1246">`--full-uri` zu `storage blob generate-sas` hinzugefügt, um den vollständigen URI für das Blob mit SAS zu erstellen</span><span class="sxs-lookup"><span data-stu-id="fc109-1246">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="fc109-1247">`--file-snapshot` zu `storage file copy start` hinzugefügt, um die Datei aus der Momentaufnahme zu kopieren</span><span class="sxs-lookup"><span data-stu-id="fc109-1247">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="fc109-1248">`storage blob copy cancel` geändert, um anstelle der Ausnahme für „NoPendingCopyOperation“ nur den Fehler anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="fc109-1248">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="fc109-1249">26. März 2019</span><span class="sxs-lookup"><span data-stu-id="fc109-1249">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="fc109-1250">Core</span><span class="sxs-lookup"><span data-stu-id="fc109-1250">Core</span></span>
* <span data-ttu-id="fc109-1251">Probleme mit der Inkompatibilität der Entwicklungserweiterung behoben</span><span class="sxs-lookup"><span data-stu-id="fc109-1251">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="fc109-1252">Die Fehlerbehandlung verweist Kunden jetzt auf die Problemseite.</span><span class="sxs-lookup"><span data-stu-id="fc109-1252">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="fc109-1253">Cloud</span><span class="sxs-lookup"><span data-stu-id="fc109-1253">Cloud</span></span>
* <span data-ttu-id="fc109-1254">Fehler „Abonnement nicht gefunden“ in `cloud set` behoben</span><span class="sxs-lookup"><span data-stu-id="fc109-1254">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="fc109-1255">ACR</span><span class="sxs-lookup"><span data-stu-id="fc109-1255">ACR</span></span>
* <span data-ttu-id="fc109-1256">Redundante Quellen im Imageimport korrigiert</span><span class="sxs-lookup"><span data-stu-id="fc109-1256">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="fc109-1257">`--auth-mode` wurde den Befehlen `acr build`, `acr run`, `acr task create` und `acr task update` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-1257">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="fc109-1258">Befehlsgruppe „acr task credential“ zum Verwalten von Anmeldeinformationen für eine Aufgabe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1258">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="fc109-1259">„--no-wait“ zum Befehl `acr build` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1259">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="fc109-1260">AppService</span><span class="sxs-lookup"><span data-stu-id="fc109-1260">AppService</span></span>
* <span data-ttu-id="fc109-1261">Problem behoben, das dazu führte, dass die Ausführung aus einem leeren Verzeichnis oder ein Szenario mit unbekannten Code von `webapp up` nicht korrekt behandelt wurde</span><span class="sxs-lookup"><span data-stu-id="fc109-1261">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="fc109-1262">Problem behoben, aufgrund dessen Slots für `[webapp|functionapp] config ssl bind` nicht verwendet werden konnten</span><span class="sxs-lookup"><span data-stu-id="fc109-1262">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="fc109-1263">Bot Service</span><span class="sxs-lookup"><span data-stu-id="fc109-1263">BOT Service</span></span>
* <span data-ttu-id="fc109-1264">`bot prepare-deploy` hinzugefügt, um die Bereitstellung von Bots über `webapp` vorzubereiten</span><span class="sxs-lookup"><span data-stu-id="fc109-1264">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="fc109-1265">`bot create --kind registration` geändert, um das Kennwort anzuzeigen, falls kein Kennwort angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="fc109-1265">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="fc109-1266">[BREAKING CHANGE]`--endpoint` wurde in `bot create --kind registration` geändert, sodass nun standardmäßig eine leere Zeichenfolge verwendet wird, anstatt eine Angabe zu erfordern.</span><span class="sxs-lookup"><span data-stu-id="fc109-1266">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="fc109-1267">`SCM_DO_BUILD_DURING_DEPLOYMENT` zu den Anwendungseinstellungen der ARM-Vorlage für Web-App-Bot (v4) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1267">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="fc109-1268">CDN</span><span class="sxs-lookup"><span data-stu-id="fc109-1268">CDN</span></span>
* <span data-ttu-id="fc109-1269">Unterstützung für `--no-wait` zu `cdn endpoint [create|update|start|stop|delete|load|purge]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1269">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* <span data-ttu-id="fc109-1270">[BREAKING CHANGE] Das standardmäßige Zwischenspeicherverhalten für Abfragezeichenfolgen von `cdn endpoint create` wurde geändert.</span><span class="sxs-lookup"><span data-stu-id="fc109-1270">[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour.</span></span> <span data-ttu-id="fc109-1271">Es wird nicht mehr standardmäßig „IgnoreQueryString“ festgelegt.</span><span class="sxs-lookup"><span data-stu-id="fc109-1271">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="fc109-1272">Er wird jetzt vom Dienst festgelegt.</span><span class="sxs-lookup"><span data-stu-id="fc109-1272">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="fc109-1273">Cosmosdb</span><span class="sxs-lookup"><span data-stu-id="fc109-1273">Cosmosdb</span></span>
* <span data-ttu-id="fc109-1274">Unterstützung für `--enable-multiple-write-locations` bei Kontoaktualisierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1274">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="fc109-1275">Untergruppe `network-rule` mit Befehlen `add`, `remove` und `list` zum Verwalten von VNET-Regeln eines Cosmos DB-Kontos hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1275">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="fc109-1276">Interactive</span><span class="sxs-lookup"><span data-stu-id="fc109-1276">Interactive</span></span>
* <span data-ttu-id="fc109-1277">Inkompatibilität mit der über azdev installierten interaktiven Erweiterung korrigiert</span><span class="sxs-lookup"><span data-stu-id="fc109-1277">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="fc109-1278">Überwachen</span><span class="sxs-lookup"><span data-stu-id="fc109-1278">Monitor</span></span>
* <span data-ttu-id="fc109-1279">Geändert, sodass der Dimensionswert `*` für `monitor metrics alert [create|update]` zulässig ist</span><span class="sxs-lookup"><span data-stu-id="fc109-1279">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="fc109-1280">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="fc109-1280">Network</span></span>
* <span data-ttu-id="fc109-1281">Befehlsgruppe `rewrite-rule` zu `application-gateway` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1281">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="fc109-1282">Profil</span><span class="sxs-lookup"><span data-stu-id="fc109-1282">Profile</span></span>
* <span data-ttu-id="fc109-1283">Kontounterstützung auf Mandantenebene für verwaltete Dienstidentität zu `login` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1283">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="fc109-1284">Postgres</span><span class="sxs-lookup"><span data-stu-id="fc109-1284">Postgres</span></span> 
* <span data-ttu-id="fc109-1285">postgresql-Befehle vom Typ `replica` und Befehl `restart server` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1285">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="fc109-1286">Änderungen vorgenommen, um den Standardspeicherort aus der Ressourcengruppe abzurufen, wenn er für die Erstellung von Servern nicht angegeben wurde, und um eine Überprüfung für die Aufbewahrungstage hinzuzufügen</span><span class="sxs-lookup"><span data-stu-id="fc109-1286">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="fc109-1287">Resource</span><span class="sxs-lookup"><span data-stu-id="fc109-1287">Resource</span></span>
* <span data-ttu-id="fc109-1288">Verbesserte Tabellenausgabe für `deployment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="fc109-1288">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="fc109-1289">Problem mit `deployment [create|validate]` behoben, aufgrund dessen der Typ „secureObject“ nicht erkannt wurde</span><span class="sxs-lookup"><span data-stu-id="fc109-1289">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="fc109-1290">Graph</span><span class="sxs-lookup"><span data-stu-id="fc109-1290">Graph</span></span>
* <span data-ttu-id="fc109-1291">Unterstützung für `--end-date` zu `ad [app|sp] credential reset` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1291">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="fc109-1292">Unterstützung für das Hinzufügen von Berechtigungen mit `ad app permission add` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1292">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="fc109-1293">Fehler mit `ad app permission list` behoben, wenn keine Berechtigungen vorlagen</span><span class="sxs-lookup"><span data-stu-id="fc109-1293">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="fc109-1294">Änderung an `ad sp delete` vorgenommen, um das Entfernen einer Rollenzuweisung zu überspringen, wenn das aktuelle Konto kein Abonnement enthält</span><span class="sxs-lookup"><span data-stu-id="fc109-1294">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="fc109-1295">`ad app create` geändert, sodass ohne Angabe für `--identifier-uris` standardmäßig eine leere Liste verwendet wird</span><span class="sxs-lookup"><span data-stu-id="fc109-1295">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="fc109-1296">storage</span><span class="sxs-lookup"><span data-stu-id="fc109-1296">storage</span></span>
* <span data-ttu-id="fc109-1297">`--snapshot` zu `storage file download-batch` für den Download von einer Freigabemomentaufnahme hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1297">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="fc109-1298">Statusanzeige für `storage blob [download-batch|upload-batch]` geändert, damit sie weniger ausführlich dargestellt wird und das aktuelle Blob angibt</span><span class="sxs-lookup"><span data-stu-id="fc109-1298">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="fc109-1299">Problem mit `storage account update` behoben, das beim Aktualisieren von Verschlüsselungsparametern auftrat</span><span class="sxs-lookup"><span data-stu-id="fc109-1299">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="fc109-1300">Problem behoben, bei dem für `storage blob show` ein Fehler auftrat, wenn oauth (`--auth-mode=login`) verwendet wurde</span><span class="sxs-lookup"><span data-stu-id="fc109-1300">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="fc109-1301">VM</span><span class="sxs-lookup"><span data-stu-id="fc109-1301">VM</span></span>
* <span data-ttu-id="fc109-1302">Befehl `image update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1302">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="fc109-1303">12. März 2019</span><span class="sxs-lookup"><span data-stu-id="fc109-1303">March 12, 2019</span></span>

<span data-ttu-id="fc109-1304">Version 2.0.60</span><span class="sxs-lookup"><span data-stu-id="fc109-1304">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="fc109-1305">Core</span><span class="sxs-lookup"><span data-stu-id="fc109-1305">Core</span></span>

* <span data-ttu-id="fc109-1306">Falsche Fehlermeldung in `cloud set` zu nicht gefundenem Abonnement korrigiert</span><span class="sxs-lookup"><span data-stu-id="fc109-1306">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="fc109-1307">ACR</span><span class="sxs-lookup"><span data-stu-id="fc109-1307">ACR</span></span>

* <span data-ttu-id="fc109-1308">Redundante Quellen im Imageimport korrigiert</span><span class="sxs-lookup"><span data-stu-id="fc109-1308">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="fc109-1309">ACS</span><span class="sxs-lookup"><span data-stu-id="fc109-1309">ACS</span></span>

* <span data-ttu-id="fc109-1310">Änderung vorgenommen, um den Parameter `--listen-address` für `aks browse` zu ignorieren, wenn er nicht von kubectl unterstützt wird</span><span class="sxs-lookup"><span data-stu-id="fc109-1310">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="fc109-1311">AppService</span><span class="sxs-lookup"><span data-stu-id="fc109-1311">AppService</span></span>

* <span data-ttu-id="fc109-1312">`[webapp|functionapp] deployment list-publishing-credentials` hinzugefügt, um die Kudu-Veröffentlichungs-URL und die entsprechenden Anmeldeinformationen abzurufen</span><span class="sxs-lookup"><span data-stu-id="fc109-1312">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="fc109-1313">Fehlerhafte Ausgabeanweisung für `webapp auth update` entfernt</span><span class="sxs-lookup"><span data-stu-id="fc109-1313">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="fc109-1314">`functionapp` korrigiert, um das korrekte Image für die Runtime in App Service-Plänen unter Linux festzulegen</span><span class="sxs-lookup"><span data-stu-id="fc109-1314">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="fc109-1315">Vorschau-Tag für `webapp up` entfernt und Verbesserungen am Befehl implementiert</span><span class="sxs-lookup"><span data-stu-id="fc109-1315">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="fc109-1316">Botservice</span><span class="sxs-lookup"><span data-stu-id="fc109-1316">Botservice</span></span>

* <span data-ttu-id="fc109-1317">`SCM_DO_BUILD_DURING_DEPLOYMENT` zu den Anwendungseinstellungen der ARM-Vorlage für Web-App-Bot (v4) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1317">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="fc109-1318">`Microsoft-BotFramework-AppId` und `Microsoft-BotFramework-AppPassword` zu den Anwendungseinstellungen der ARM-Vorlage für Web-App-Bot (v4) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1318">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="fc109-1319">Einfache Anführungszeichen aus der Befehlsausgabe von `bot publish` am Ende von `bot create` entfernt</span><span class="sxs-lookup"><span data-stu-id="fc109-1319">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="fc109-1320">`bot publish` wurde geändert und ist jetzt asynchron.</span><span class="sxs-lookup"><span data-stu-id="fc109-1320">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="fc109-1321">Container</span><span class="sxs-lookup"><span data-stu-id="fc109-1321">Container</span></span>

* <span data-ttu-id="fc109-1322">Argument `--no-wait` zu `container [start|restart]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1322">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="fc109-1323">EventHub</span><span class="sxs-lookup"><span data-stu-id="fc109-1323">EventHub</span></span>

* <span data-ttu-id="fc109-1324">Flag `--skip-empty-archives` zu `eventhub create|update` hinzugefügt, um leere Archive in der Aufzeichnung zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="fc109-1324">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="fc109-1325">Suchen</span><span class="sxs-lookup"><span data-stu-id="fc109-1325">Find</span></span>

* <span data-ttu-id="fc109-1326">Umfangreiches Funktionsupdate</span><span class="sxs-lookup"><span data-stu-id="fc109-1326">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="fc109-1327">HDInsight</span><span class="sxs-lookup"><span data-stu-id="fc109-1327">HDInsight</span></span>

* <span data-ttu-id="fc109-1328">Parameter `--storage-account-managed-identity` zu `hdinsight create` hinzugefügt, um MSI in ADLS Gen2 zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="fc109-1328">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="fc109-1329">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="fc109-1329">Network</span></span>

* <span data-ttu-id="fc109-1330">Problem mit `vpn-connection update` behoben, aufgrund dessen die Aktualisierung einer VPN-Verbindung zwischen Gateways in verschiedenen Abonnements fehlschlug</span><span class="sxs-lookup"><span data-stu-id="fc109-1330">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="fc109-1331">Rdbms</span><span class="sxs-lookup"><span data-stu-id="fc109-1331">Rdbms</span></span>

* <span data-ttu-id="fc109-1332">Kleinere Korrekturen, um den Standardspeicherort aus der Ressourcengruppe abzurufen, wenn er für die Erstellung von Servern nicht angegeben wurde, und um eine Überprüfung für die Aufbewahrungstage hinzuzufügen</span><span class="sxs-lookup"><span data-stu-id="fc109-1332">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="fc109-1333">Role</span><span class="sxs-lookup"><span data-stu-id="fc109-1333">Role</span></span>

* <span data-ttu-id="fc109-1334">`role definition update` wurde korrigiert und nutzt nun die ID, um die Definition korrekt aufzulösen.</span><span class="sxs-lookup"><span data-stu-id="fc109-1334">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="fc109-1335">`ad app credential reset` geändert, um die Annahme zu entfernen, dass der Dienstprinzipal der App stets vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="fc109-1335">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="fc109-1336">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="fc109-1336">Service Fabric</span></span>

* <span data-ttu-id="fc109-1337">Das Problem, dass `sf cluster list` nicht wiederholbar war, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="fc109-1337">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="fc109-1338">26. Februar 2019</span><span class="sxs-lookup"><span data-stu-id="fc109-1338">February 26, 2019</span></span>

<span data-ttu-id="fc109-1339">Version 2.0.59</span><span class="sxs-lookup"><span data-stu-id="fc109-1339">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="fc109-1340">Core</span><span class="sxs-lookup"><span data-stu-id="fc109-1340">Core</span></span>

* <span data-ttu-id="fc109-1341">Problem behoben, aufgrund dessen die Verwendung von `--subscription NAME` in einigen Instanzen eine Ausnahme ausgelöst hat</span><span class="sxs-lookup"><span data-stu-id="fc109-1341">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="fc109-1342">ACR</span><span class="sxs-lookup"><span data-stu-id="fc109-1342">ACR</span></span>

* <span data-ttu-id="fc109-1343">Parameter `--target` für die Befehle `acr build`, `acr task create` und `acr task update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1343">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="fc109-1344">Verbesserte Fehlerbehandlung für Runtimebefehle, wenn keine Anmeldung bei Azure besteht</span><span class="sxs-lookup"><span data-stu-id="fc109-1344">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="fc109-1345">ACS</span><span class="sxs-lookup"><span data-stu-id="fc109-1345">ACS</span></span>

* <span data-ttu-id="fc109-1346">Option `--listen-address` zu `aks port-forward` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1346">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="fc109-1347">AppService</span><span class="sxs-lookup"><span data-stu-id="fc109-1347">AppService</span></span>

* <span data-ttu-id="fc109-1348">Befehl `functionapp devops-build` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1348">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="fc109-1349">Batch</span><span class="sxs-lookup"><span data-stu-id="fc109-1349">Batch</span></span>
* <span data-ttu-id="fc109-1350">[BREAKING CHANGE] Befehl `batch pool upgrade os` entfernt</span><span class="sxs-lookup"><span data-stu-id="fc109-1350">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="fc109-1351">[BREAKING CHANGE]`Pacakges`-Eigenschaft aus `Application`-Antworten entfernt</span><span class="sxs-lookup"><span data-stu-id="fc109-1351">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="fc109-1352">Befehl `batch application package list` zum Auflisten von Paketen einer Anwendung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1352">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="fc109-1353">[BREAKING CHANGE]`--application-id` in allen `batch application`-Befehlen in `--application-name` geändert</span><span class="sxs-lookup"><span data-stu-id="fc109-1353">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="fc109-1354">Argument `--json-file` für Befehle zum Anfordern der unformatierten API-Antwort hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1354">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="fc109-1355">Validierung aktualisiert, sodass das `https://`-Element automatisch in alle Endpunkte aufgenommen wird, wenn es fehlt</span><span class="sxs-lookup"><span data-stu-id="fc109-1355">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="fc109-1356">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="fc109-1356">CosmosDB</span></span>

* <span data-ttu-id="fc109-1357">Untergruppe `network-rule` mit Befehlen `add`, `remove` und `list` zum Verwalten von VNET-Regeln eines Cosmos DB-Kontos hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1357">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="fc109-1358">Kusto</span><span class="sxs-lookup"><span data-stu-id="fc109-1358">Kusto</span></span>

* <span data-ttu-id="fc109-1359">[BREAKING CHANGE] Typen `hot_cache_period` und `soft_delete_period` für Datenbank in Format der Zeitspanne nach ISO8601 geändert</span><span class="sxs-lookup"><span data-stu-id="fc109-1359">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="fc109-1360">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="fc109-1360">Network</span></span>

* <span data-ttu-id="fc109-1361">Argument `--express-route-gateway-bypass` zu `vpn-connection [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1361">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="fc109-1362">Befehlsgruppen aus `express-route`-Erweiterungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1362">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="fc109-1363">Befehlsgruppen `express-route gateway` und `express-route port` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1363">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="fc109-1364">Argument `--legacy-mode` zu `express-route peering [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1364">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="fc109-1365">Argumente `--allow-classic-operations` und `--express-route-port` zu `express-route [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1365">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="fc109-1366">Argument `--gateway-default-site` zu `vnet-gateway [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1366">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="fc109-1367">Befehle vom Typ `ipsec-policy` zu `vnet-gateway` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1367">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="fc109-1368">Resource</span><span class="sxs-lookup"><span data-stu-id="fc109-1368">Resource</span></span>

* <span data-ttu-id="fc109-1369">Problem mit `deployment create` behoben, aufgrund dessen beim Feld „Typ“ die Groß-/Kleinschreibung beachtet wurde</span><span class="sxs-lookup"><span data-stu-id="fc109-1369">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="fc109-1370">Unterstützung für URI-basierte Parameterdatei zu `policy assignment create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1370">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="fc109-1371">Unterstützung für URI-basierte Parameter und Definitionen zu `policy set-definition update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1371">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="fc109-1372">Verarbeitung von Parametern und Regeln für `policy definition update` korrigiert</span><span class="sxs-lookup"><span data-stu-id="fc109-1372">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="fc109-1373">Problem mit `resource show/update/delete/tag/invoke-action` behoben, aufgrund dessen bei abonnementübergreifenden IDs die Abonnement-ID nicht ordnungsgemäß berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="fc109-1373">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="fc109-1374">Role</span><span class="sxs-lookup"><span data-stu-id="fc109-1374">Role</span></span>

* <span data-ttu-id="fc109-1375">Unterstützung für App-Rollen zu `ad app [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1375">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="fc109-1376">VM</span><span class="sxs-lookup"><span data-stu-id="fc109-1376">VM</span></span>

* <span data-ttu-id="fc109-1377">Problem mit `vm create where ` behoben, aufgrund dessen der beschleunigte Netzwerkbetrieb für Ubuntu 18.0 nicht standardmäßig aktiviert war</span><span class="sxs-lookup"><span data-stu-id="fc109-1377">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="fc109-1378">12. Februar 2019</span><span class="sxs-lookup"><span data-stu-id="fc109-1378">February 12, 2019</span></span>

<span data-ttu-id="fc109-1379">Version 2.0.58</span><span class="sxs-lookup"><span data-stu-id="fc109-1379">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="fc109-1380">Core</span><span class="sxs-lookup"><span data-stu-id="fc109-1380">Core</span></span>

* <span data-ttu-id="fc109-1381">`az --version` zeigt jetzt eine Benachrichtigung an, wenn Sie Pakete haben, für die ein Update verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="fc109-1381">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="fc109-1382">Die Regression, dass `--ids` nicht mehr mit JSON-Ausgaben verwendet werden konnte, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="fc109-1382">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="fc109-1383">ACR</span><span class="sxs-lookup"><span data-stu-id="fc109-1383">ACR</span></span>
* <span data-ttu-id="fc109-1384">[BREAKING CHANGE] Die Befehlsgruppe `acr build-task` wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="fc109-1384">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="fc109-1385">[BREAKING CHANGE] Die Optionen `--tag` und `--manifest` wurden aus `acr repository delete` entfernt.</span><span class="sxs-lookup"><span data-stu-id="fc109-1385">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="fc109-1386">ACS</span><span class="sxs-lookup"><span data-stu-id="fc109-1386">ACS</span></span>
* <span data-ttu-id="fc109-1387">Unterstützung für Namen ohne Berücksichtigung von Groß-/Kleinschreibung wurde zu `aks [enable-addons|disable-addons]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-1387">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="fc109-1388">Unterstützung für Azure Active Directory-Aktualisierungsvorgang mithilfe von `aks update-credentials --reset-aad` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-1388">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="fc109-1389">Die Information, dass `--output` für `aks get-credentials` ignoriert wird, wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-1389">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="fc109-1390">AMS</span><span class="sxs-lookup"><span data-stu-id="fc109-1390">AMS</span></span>
* <span data-ttu-id="fc109-1391">Befehle vom Typ `ams streaming-endpoint [start | stop | create | update] wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1391">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="fc109-1392">Befehle vom Typ `ams live-event [create | start | stop | reset] wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1392">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="fc109-1393">AppService</span><span class="sxs-lookup"><span data-stu-id="fc109-1393">Appservice</span></span>
* <span data-ttu-id="fc109-1394">Die Möglichkeit zum Erstellen und Konfigurieren von Funktionen mithilfe von ACR-Containern wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-1394">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="fc109-1395">Unterstützung für das Aktualisieren von Web-App-Konfigurationen über JSON wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-1395">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="fc109-1396">Die Hilfe für `appservice-plan-update` wurde verbessert.</span><span class="sxs-lookup"><span data-stu-id="fc109-1396">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="fc109-1397">Unterstützung für App-Erkenntnisse beim Erstellen von Funktions-Apps wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-1397">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="fc109-1398">Probleme mit der Web-App SSH wurden behoben.</span><span class="sxs-lookup"><span data-stu-id="fc109-1398">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="fc109-1399">Botservice</span><span class="sxs-lookup"><span data-stu-id="fc109-1399">Botservice</span></span>
* <span data-ttu-id="fc109-1400">Die Benutzeroberfläche für `bot publish` wurde verbessert.</span><span class="sxs-lookup"><span data-stu-id="fc109-1400">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="fc109-1401">Eine Warnung für Zeitlimit bei der Ausführung von `npm install` während `az bot publish` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-1401">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="fc109-1402">Ungültiges char-Element wurde `.` aus `--name` in `az bot create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="fc109-1402">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="fc109-1403">Eine Änderung wurde vorgenommen, um die zufällige Zuordnung von Ressourcennamen beim Erstellen von Azure Storage-Instanzen, App Service-Plänen, Funktions-/Web-Apps und Application Insights-Instanzen zu verhindern.</span><span class="sxs-lookup"><span data-stu-id="fc109-1403">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="fc109-1404">[VERALTET] Argument `--proj-name` zugunsten von `--proj-file-path` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="fc109-1404">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="fc109-1405">`az bot publish` wurde geändert, um abgerufene IIS-Bereitstellungsdateien vom Typ „Node.js“ zu entfernen, wenn sie nicht bereits vorhanden waren.</span><span class="sxs-lookup"><span data-stu-id="fc109-1405">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="fc109-1406">Das `--keep-node-modules` Argument wurde zu `az bot publish` hinzugefügt, damit der Ordner `node_modules` in App Service nicht gelöscht wird.</span><span class="sxs-lookup"><span data-stu-id="fc109-1406">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="fc109-1407">Das Schlüssel-Wert-Paar `"publishCommand"` wurde der Ausgabe von `az bot create` beim Erstellen einer Funktions-App oder eines Web-App-Bots hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-1407">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="fc109-1408">Der Wert von `"publishCommand"` ist ein `az bot publish`-Befehl, der bereits die erforderlichen Parameter zum Veröffentlichen des neu erstellten Bots enthält.</span><span class="sxs-lookup"><span data-stu-id="fc109-1408">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="fc109-1409">`"WEBSITE_NODE_DEFAULT_VERSION"` in der ARM-Vorlage wurde so aktualisiert, dass v4-SDK-Bots 10.14.1 anstelle von 8.9.4 verwenden.</span><span class="sxs-lookup"><span data-stu-id="fc109-1409">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="fc109-1410">Key Vault</span><span class="sxs-lookup"><span data-stu-id="fc109-1410">Key Vault</span></span>
* <span data-ttu-id="fc109-1411">Ein Problem mit `keyvault secret backup` wurde behoben, aufgrund dessen einige Benutzer bei Verwendung von `--id` einen `unexpected_keyword`-Fehler erhielten.</span><span class="sxs-lookup"><span data-stu-id="fc109-1411">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="fc109-1412">Überwachen</span><span class="sxs-lookup"><span data-stu-id="fc109-1412">Monitor</span></span>
* <span data-ttu-id="fc109-1413">`monitor metrics alert [create|update]` wurde so geändert, dass der Dimensionswert `*` zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="fc109-1413">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="fc109-1414">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="fc109-1414">Network</span></span>
* <span data-ttu-id="fc109-1415">`dns zone export` wurde geändert, um sicherzustellen, dass es sich bei exportierten CNAMEs um FQDNs handelt.</span><span class="sxs-lookup"><span data-stu-id="fc109-1415">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="fc109-1416">Parameter `--gateway-name` wurde zu `nic ip-config address-pool [add|remove]` hinzugefügt, um Back-End-Adresspools von Anwendungsgateways zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="fc109-1416">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="fc109-1417">Argumente `--traffic-analytics` und `--workspace` wurden zu `network watcher flow-log configure` hinzugefügt, um Datenverkehrsanalysen über einen Log Analytics-Arbeitsbereich zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="fc109-1417">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="fc109-1418">`--idle-timeout` und `--floating-ip` wurden zu `lb inbound-nat-pool [create|update]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-1418">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="fc109-1419">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="fc109-1419">Policy Insights</span></span>
* <span data-ttu-id="fc109-1420">`policy remediation`-Befehle wurden hinzugefügt, um Korrekturfunktionen der Ressourcenrichtlinie zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="fc109-1420">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="fc109-1421">RDBMS</span><span class="sxs-lookup"><span data-stu-id="fc109-1421">RDBMS</span></span>
* <span data-ttu-id="fc109-1422">Hilfemeldung und Befehlsparameter wurden verbessert.</span><span class="sxs-lookup"><span data-stu-id="fc109-1422">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="fc109-1423">Redis</span><span class="sxs-lookup"><span data-stu-id="fc109-1423">Redis</span></span>
* <span data-ttu-id="fc109-1424">Befehle zum Verwalten von „firewall-rules“ (erstellen, aktualisieren, löschen, anzeigen, auflisten) wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-1424">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="fc109-1425">Befehle zum Verwalten von „server-link“ (erstellen, aktualisieren, löschen, anzeigen, auflisten) wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-1425">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="fc109-1426">Befehle zum Verwalten von „patch-schedule“ (erstellen, aktualisieren, löschen, anzeigen, auflisten) wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-1426">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="fc109-1427">Unterstützung für Verfügbarkeitszonen und TLS-Mindestversion wurden zu „redis create“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-1427">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="fc109-1428">[BREAKING CHANGE] Befehle `redis update-settings` und `redis list-all` wurden entfernt.</span><span class="sxs-lookup"><span data-stu-id="fc109-1428">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="fc109-1429">[BREAKING CHANGE] Parameter für `redis create`: „Mandanteneinstellungen“ werden im Format „Schlüssel[=Wert] nicht akzeptiert.</span><span class="sxs-lookup"><span data-stu-id="fc109-1429">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="fc109-1430">[VERALTET] Warnmeldung zur Markierung des Befehls `redis import-method` als veraltet hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1430">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="fc109-1431">Role</span><span class="sxs-lookup"><span data-stu-id="fc109-1431">Role</span></span>
* <span data-ttu-id="fc109-1432">[BREAKING CHANGE] Befehl `az identity` wurde aus den `vm`-Befehlen hierher verschoben.</span><span class="sxs-lookup"><span data-stu-id="fc109-1432">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="fc109-1433">SQL-VM</span><span class="sxs-lookup"><span data-stu-id="fc109-1433">SQL VM</span></span>
* <span data-ttu-id="fc109-1434">[VERALTET] Argument `--boostrap-acc-pwd` aufgrund eines Tippfehlers als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="fc109-1434">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="fc109-1435">VM</span><span class="sxs-lookup"><span data-stu-id="fc109-1435">VM</span></span>
* <span data-ttu-id="fc109-1436">`vm list-skus` wurde so geändert, dass `--all` anstelle von `--all true` verwendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="fc109-1436">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="fc109-1437">`vmss run-command [invoke | list | show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1437">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="fc109-1438">Ein Fehler wurde behoben, aufgrund dessen bei der Ausführung von `vmss encryption enable` bisher ein Fehler auftrat.</span><span class="sxs-lookup"><span data-stu-id="fc109-1438">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="fc109-1439">[BREAKING CHANGE] Die Befehle vom Typ `az identity` wurden zu `role`-Befehlen verschoben.</span><span class="sxs-lookup"><span data-stu-id="fc109-1439">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="fc109-1440">31. Januar 2019</span><span class="sxs-lookup"><span data-stu-id="fc109-1440">January 31, 2019</span></span>

<span data-ttu-id="fc109-1441">Version 2.0.57</span><span class="sxs-lookup"><span data-stu-id="fc109-1441">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="fc109-1442">Core</span><span class="sxs-lookup"><span data-stu-id="fc109-1442">Core</span></span>

* <span data-ttu-id="fc109-1443">Hotfix für [Problem 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="fc109-1443">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="fc109-1444">28. Januar 2019</span><span class="sxs-lookup"><span data-stu-id="fc109-1444">January 28, 2019</span></span>

<span data-ttu-id="fc109-1445">Version 2.0.56</span><span class="sxs-lookup"><span data-stu-id="fc109-1445">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="fc109-1446">ACR</span><span class="sxs-lookup"><span data-stu-id="fc109-1446">ACR</span></span>
* <span data-ttu-id="fc109-1447">Unterstützung für VNet/IP-Regeln wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-1447">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="fc109-1448">ACS</span><span class="sxs-lookup"><span data-stu-id="fc109-1448">ACS</span></span>
* <span data-ttu-id="fc109-1449">Virtuelle Knoten (Vorschau) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1449">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="fc109-1450">Verwaltete OpenShift-Befehle wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-1450">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="fc109-1451">Unterstützung für den Dienstprinzipal-Updatevorgang mit `aks update-credentials -reset-service-principal` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-1451">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="fc109-1452">AMS</span><span class="sxs-lookup"><span data-stu-id="fc109-1452">AMS</span></span>
* <span data-ttu-id="fc109-1453">[BREAKING CHANGE]`ams asset get-streaming-locators` in `ams asset list-streaming-locators` umbenannt</span><span class="sxs-lookup"><span data-stu-id="fc109-1453">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="fc109-1454">[BREAKING CHANGE]`ams streaming-locator get-content-keys` in `ams streaming-locator list-content-keys` umbenannt</span><span class="sxs-lookup"><span data-stu-id="fc109-1454">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="fc109-1455">AppService</span><span class="sxs-lookup"><span data-stu-id="fc109-1455">Appservice</span></span>
* <span data-ttu-id="fc109-1456">Unterstützung für App-Erkenntnisse in `functionapp create` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-1456">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="fc109-1457">Unterstützung für die Erstellung von App Service-Plänen (einschließlich Elastic Premium) wurde zu Funktions-Apps hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-1457">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="fc109-1458">Probleme bei einer App-Einstellung mit Elastic Premium-Plänen wurden behoben.</span><span class="sxs-lookup"><span data-stu-id="fc109-1458">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="fc109-1459">Container</span><span class="sxs-lookup"><span data-stu-id="fc109-1459">Container</span></span>
* <span data-ttu-id="fc109-1460">Befehl `container start` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1460">Added `container start` command</span></span>
* <span data-ttu-id="fc109-1461">Eine Änderung wurde vorgenommen, um bei der Containererstellung die Verwendung von Dezimalwerten für die CPU zuzulassen.</span><span class="sxs-lookup"><span data-stu-id="fc109-1461">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="fc109-1462">EventGrid</span><span class="sxs-lookup"><span data-stu-id="fc109-1462">EventGrid</span></span>
* <span data-ttu-id="fc109-1463">Parameter `--deadletter-endpoint` zu `event-subscription [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1463">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="fc109-1464">„storagequeue“ und „hybridconnection“ wurden als neue Werte für „event-subscription [create|update] --endpoint-type“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-1464">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="fc109-1465">Parameter `--max-delivery-attempts` und `--event-ttl` wurden zu `event-subscription create` hinzugefügt, um die Wiederholungsrichtlinie für Ereignisse anzugeben.</span><span class="sxs-lookup"><span data-stu-id="fc109-1465">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="fc109-1466">Eine Warnmeldung wurde zu `event-subscription [create|update]` hinzugefügt, wenn Webhook als Ziel für ein Ereignisabonnement verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="fc109-1466">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="fc109-1467">Parameter „source-resource-id“ wurde für alle Befehle im Zusammenhang mit Ereignisabonnements hinzugefügt, und alle anderen Parameter im Zusammenhang mit Quellressourcen wurden als veraltet markiert.</span><span class="sxs-lookup"><span data-stu-id="fc109-1467">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="fc109-1468">HDInsight</span><span class="sxs-lookup"><span data-stu-id="fc109-1468">HDInsight</span></span>
* <span data-ttu-id="fc109-1469">[BREAKING CHANGE] Die Parameter `--virtual-network` und `--subnet-name` wurden aus `hdinsight [application] create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="fc109-1469">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="fc109-1470">[BREAKING CHANGE]`hdinsight create --storage-account` wurde so geändert, dass der Name oder die ID eines Speicherkontos anstellen von Blobendpunkten akzeptiert wird.</span><span class="sxs-lookup"><span data-stu-id="fc109-1470">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="fc109-1471">Parameter `--vnet-name` und `--subnet-name` zu `hdinsight create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1471">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="fc109-1472">Unterstützung für das Enterprise-Sicherheitspaket und Datenträgerverschlüsselung wurde zu `hdinsight create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-1472">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="fc109-1473">Befehl `hdinsight rotate-disk-encryption-key` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1473">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="fc109-1474">Befehl `hdinsight update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1474">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="fc109-1475">IoT</span><span class="sxs-lookup"><span data-stu-id="fc109-1475">IoT</span></span>
* <span data-ttu-id="fc109-1476">Codierungsformat wurde zu Befehl „routing-endpoint“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-1476">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="fc109-1477">Kusto</span><span class="sxs-lookup"><span data-stu-id="fc109-1477">Kusto</span></span>
* <span data-ttu-id="fc109-1478">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="fc109-1478">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="fc109-1479">Überwachen</span><span class="sxs-lookup"><span data-stu-id="fc109-1479">Monitor</span></span>
* <span data-ttu-id="fc109-1480">ID-Vergleich wurde so geändert, dass Groß-/Kleinschreibung nicht mehr beachtet wird.</span><span class="sxs-lookup"><span data-stu-id="fc109-1480">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="fc109-1481">Profil</span><span class="sxs-lookup"><span data-stu-id="fc109-1481">Profile</span></span>
* <span data-ttu-id="fc109-1482">Konto auf Mandantenebene für verwaltete Dienstidentität für `login` wird aktiviert.</span><span class="sxs-lookup"><span data-stu-id="fc109-1482">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="fc109-1483">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="fc109-1483">Network</span></span>
* <span data-ttu-id="fc109-1484">Ein Problem mit `express-route update` wurde behoben, aufgrund dessen das Argument `--bandwidth` ignoriert wurde.</span><span class="sxs-lookup"><span data-stu-id="fc109-1484">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="fc109-1485">Ein Problem mit `ddos-protection update` wurde behoben, aufgrund dessen das festgelegte Verständnis zu einer Stapelüberwachung führte.</span><span class="sxs-lookup"><span data-stu-id="fc109-1485">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="fc109-1486">Resource</span><span class="sxs-lookup"><span data-stu-id="fc109-1486">Resource</span></span>
* <span data-ttu-id="fc109-1487">Unterstützung für die URI-Parameterdatei wurde zu `group deployment create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-1487">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="fc109-1488">Unterstützung für verwaltete Identitäten wurde zu `policy assignment [create|list|show]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-1488">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="fc109-1489">Virtueller SQL-Computer</span><span class="sxs-lookup"><span data-stu-id="fc109-1489">SQL Virtual Machine</span></span>
* <span data-ttu-id="fc109-1490">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="fc109-1490">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="fc109-1491">Storage</span><span class="sxs-lookup"><span data-stu-id="fc109-1491">Storage</span></span>
* <span data-ttu-id="fc109-1492">Eine Lösung wurde so geändert, dass nur Eigenschaften aktualisiert werden, die im selben Objekt geändert werden.</span><span class="sxs-lookup"><span data-stu-id="fc109-1492">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="fc109-1493">Nr. 8021 wurde korrigiert, Binärdaten werden bei der Rückgabe in Base64 codiert.</span><span class="sxs-lookup"><span data-stu-id="fc109-1493">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="fc109-1494">VM</span><span class="sxs-lookup"><span data-stu-id="fc109-1494">VM</span></span>
* <span data-ttu-id="fc109-1495">`vm encryption enable` wurde geändert, um den Schlüsseltresor für die Datenträgerverschlüsselung zu überprüfen und sicherzustellen, dass der Schlüsseltresor für die Schlüsselverschlüsselung vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="fc109-1495">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="fc109-1496">Flag `--force` wurde zu `vm encryption enable` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-1496">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="fc109-1497">15. Januar 2019</span><span class="sxs-lookup"><span data-stu-id="fc109-1497">January 15, 2019</span></span>

<span data-ttu-id="fc109-1498">Version 2.0.55</span><span class="sxs-lookup"><span data-stu-id="fc109-1498">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="fc109-1499">ACR</span><span class="sxs-lookup"><span data-stu-id="fc109-1499">ACR</span></span>
* <span data-ttu-id="fc109-1500">Wurde geändert, um den Push eines nicht vorhandenen Helm-Diagramms zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="fc109-1500">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="fc109-1501">Wurde geändert, um Laufzeitvorgänge ohne ARM-Anforderungen zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="fc109-1501">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="fc109-1502">[VERALTET] Parameter `--resource-group` in folgenden Befehlen als veraltet markiert:</span><span class="sxs-lookup"><span data-stu-id="fc109-1502">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="fc109-1503">ACS</span><span class="sxs-lookup"><span data-stu-id="fc109-1503">ACS</span></span>
* <span data-ttu-id="fc109-1504">Unterstützung für neue ACI-Regionen wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-1504">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="fc109-1505">AppService</span><span class="sxs-lookup"><span data-stu-id="fc109-1505">Appservice</span></span>
* <span data-ttu-id="fc109-1506">Ein Problem beim Hochladen von Zertifikaten für in einer ASE gehostete Apps wurde behoben, aufgrund dessen die AS-RG und die App-RG nicht übereinstimmten.</span><span class="sxs-lookup"><span data-stu-id="fc109-1506">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="fc109-1507">`webapp up` wurde geändert, sodass SKU P1V1 als Standard für Linux verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="fc109-1507">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="fc109-1508">`[webapp|functionapp] deployment source config-zip` wurde korrigiert, sodass beim Fehlschlagen einer Bereitstellung die richtige Fehlermeldung angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="fc109-1508">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="fc109-1509">Befehl `webapp ssh` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1509">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="fc109-1510">Botservice</span><span class="sxs-lookup"><span data-stu-id="fc109-1510">Botservice</span></span>
* <span data-ttu-id="fc109-1511">Aktualisierungen des Bereitstellungsstatus wurden zu `bot create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-1511">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="fc109-1512">Konfigurieren</span><span class="sxs-lookup"><span data-stu-id="fc109-1512">Configure</span></span>
* <span data-ttu-id="fc109-1513">`none` wurde als konfigurierbares Ausgabeformat hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-1513">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="fc109-1514">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="fc109-1514">CosmosDB</span></span>
* <span data-ttu-id="fc109-1515">Unterstützung für das Erstellen einer Datenbank mit gemeinsam genutztem Durchsatz wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-1515">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="fc109-1516">HDInsight</span><span class="sxs-lookup"><span data-stu-id="fc109-1516">HDInsight</span></span>
* <span data-ttu-id="fc109-1517">Befehle zum Verwalten von Anwendungen wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-1517">Added commands for managing applications</span></span>
* <span data-ttu-id="fc109-1518">Befehle zum Verwalten von Skriptaktionen wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-1518">Added commands for managing script actions</span></span>
* <span data-ttu-id="fc109-1519">Befehle zum Verwalten von der Operations Management Suite (OMS) wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-1519">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="fc109-1520">Unterstützung zum Auflisten der regionalen Nutzung wurde zu `hdinsight list-usage` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-1520">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="fc109-1521">[BREAKING CHANGE] Standardclustertyp wurde aus `hdinsight create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="fc109-1521">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="fc109-1522">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="fc109-1522">Network</span></span>
* <span data-ttu-id="fc109-1523">Argumente `--custom-headers` und `--status-code-ranges` zu `traffic-manager profile [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1523">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="fc109-1524">Neue Routingtypen wurden hinzugefügt: Subnetz und MultiValue</span><span class="sxs-lookup"><span data-stu-id="fc109-1524">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="fc109-1525">Argumente `--custom-headers` und `--subnets` zu `traffic-manager endpoint [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1525">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="fc109-1526">Eine Problem wurde behoben, aufgrund dessen die Angabe von `--vnets ""` für `ddos-protection update` einen Fehler verursacht hat.</span><span class="sxs-lookup"><span data-stu-id="fc109-1526">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="fc109-1527">Role</span><span class="sxs-lookup"><span data-stu-id="fc109-1527">Role</span></span>
* <span data-ttu-id="fc109-1528">[VERALTET] Argument `--password` als veraltet markiert für `create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="fc109-1528">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="fc109-1529">Verwenden Sie stattdessen sichere, von der CLI generierte Kennwörter.</span><span class="sxs-lookup"><span data-stu-id="fc109-1529">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="fc109-1530">Sicherheit</span><span class="sxs-lookup"><span data-stu-id="fc109-1530">Security</span></span>
* <span data-ttu-id="fc109-1531">Erstrelease</span><span class="sxs-lookup"><span data-stu-id="fc109-1531">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="fc109-1532">Storage</span><span class="sxs-lookup"><span data-stu-id="fc109-1532">Storage</span></span>
* <span data-ttu-id="fc109-1533">[BREAKING CHANGE] Die Standardanzahl von Ergebnissen wurde für `storage [blob|file|container|share] list` in 5.000 geändert.</span><span class="sxs-lookup"><span data-stu-id="fc109-1533">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="fc109-1534">Verwenden Sie `--num-results *` für das ursprüngliche Verhalten, alle Ergebnisse zurückzugeben.</span><span class="sxs-lookup"><span data-stu-id="fc109-1534">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="fc109-1535">Parameter `--marker` zu `storage [blob|file|container|share] list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1535">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="fc109-1536">Ein Protokollmarker für die nächste Seite wurde zur STDERR für `storage [blob|file|container|share] list` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-1536">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="fc109-1537">Der Befehl `storage blob service-properties update` mit Unterstützung für statische Websites wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-1537">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="fc109-1538">VM</span><span class="sxs-lookup"><span data-stu-id="fc109-1538">VM</span></span>
* <span data-ttu-id="fc109-1539">`vm [disk|unmanaged-disk]` und `vmss disk` wurden geändert, sodass sie konsistentere Parameter enthalten.</span><span class="sxs-lookup"><span data-stu-id="fc109-1539">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="fc109-1540">Unterstützung für mandantenübergreifende Imageverweise wurden zu `[vm|vmss] create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-1540">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="fc109-1541">Fehler bei Standardkonfiguration in `vm diagnostics get-default-config --windows-os` wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="fc109-1541">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="fc109-1542">Argument `--provision-after-extensions` wurde zu `vmss extension set` hinzugefügt, um zu definieren, welche Erweiterungen vor dem Festlegen der Erweiterung bereitgestellt werden müssen.</span><span class="sxs-lookup"><span data-stu-id="fc109-1542">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="fc109-1543">Argument `--replica-count` wurde zu `sig image-version update` hinzugefügt, um die Standardanzahl für die Replikation festzulegen.</span><span class="sxs-lookup"><span data-stu-id="fc109-1543">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="fc109-1544">Fehler bei `image create --source` wurde behoben, aufgrund dessen, der Quellbetriebssystem-Datenträger für einen virtuellen Computer mit dem gleichen Namen gehalten wurde, selbst wenn die vollständige Ressourcen-ID angegeben war.</span><span class="sxs-lookup"><span data-stu-id="fc109-1544">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="fc109-1545">20. Dezember 2018</span><span class="sxs-lookup"><span data-stu-id="fc109-1545">December 20, 2018</span></span>

<span data-ttu-id="fc109-1546">Version 2.0.54</span><span class="sxs-lookup"><span data-stu-id="fc109-1546">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="fc109-1547">AppService</span><span class="sxs-lookup"><span data-stu-id="fc109-1547">Appservice</span></span>
* <span data-ttu-id="fc109-1548">Problem behoben, bei dem `webapp up` nicht erneut bereitgestellt werden konnte</span><span class="sxs-lookup"><span data-stu-id="fc109-1548">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="fc109-1549">Unterstützung für das Auflisten und Wiederherstellen von Web-App-Momentaufnahmen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1549">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="fc109-1550">Unterstützung für das Flag `--runtime` zu Windows-Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1550">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="fc109-1551">IoTCentral</span><span class="sxs-lookup"><span data-stu-id="fc109-1551">IoTCentral</span></span>
* <span data-ttu-id="fc109-1552">Fehler bei API-Aufruf für update-Befehl behoben</span><span class="sxs-lookup"><span data-stu-id="fc109-1552">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="fc109-1553">Role</span><span class="sxs-lookup"><span data-stu-id="fc109-1553">Role</span></span>
* <span data-ttu-id="fc109-1554">[BREAKING CHANGE]`ad [app|sp] list` geändert, damit standardmäßig nur die ersten 100 Objekte aufgelistet werden</span><span class="sxs-lookup"><span data-stu-id="fc109-1554">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="fc109-1555">SQL</span><span class="sxs-lookup"><span data-stu-id="fc109-1555">SQL</span></span>
* <span data-ttu-id="fc109-1556">Unterstützung für die benutzerdefinierte Sortierung auf verwalteten Instanzen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1556">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="fc109-1557">VM</span><span class="sxs-lookup"><span data-stu-id="fc109-1557">VM</span></span>
* <span data-ttu-id="fc109-1558">Parameter `---os-type` zu `disk create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1558">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="fc109-1559">18. Dezember 2018</span><span class="sxs-lookup"><span data-stu-id="fc109-1559">December 18, 2018</span></span>

<span data-ttu-id="fc109-1560">Version 2.0.53</span><span class="sxs-lookup"><span data-stu-id="fc109-1560">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="fc109-1561">ACR</span><span class="sxs-lookup"><span data-stu-id="fc109-1561">ACR</span></span>
* <span data-ttu-id="fc109-1562">Unterstützung für Imageimport aus externen Containerregistrierungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1562">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="fc109-1563">Tabellenlayout für Aufgabenliste komprimiert</span><span class="sxs-lookup"><span data-stu-id="fc109-1563">Condensed the table layout for task list</span></span>
* <span data-ttu-id="fc109-1564">Unterstützung für Azure DevOps-URLs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1564">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="fc109-1565">ACS</span><span class="sxs-lookup"><span data-stu-id="fc109-1565">ACS</span></span>
* <span data-ttu-id="fc109-1566">Virtuelle Knoten (Vorschau) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1566">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="fc109-1567">„(PREVIEW)“ aus AAD-Argumenten für `aks create` entfernt</span><span class="sxs-lookup"><span data-stu-id="fc109-1567">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="fc109-1568">[VERALTET]`az acs`-Befehle als veraltet markiert.</span><span class="sxs-lookup"><span data-stu-id="fc109-1568">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="fc109-1569">ACS wird am 31. Januar 2020 eingestellt</span><span class="sxs-lookup"><span data-stu-id="fc109-1569">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="fc109-1570">Unterstützung für Netzwerkrichtlinie bei der Erstellung neuer AKS-Cluster hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1570">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="fc109-1571">Anforderung des Arguments `--nodepool-name` bei nur einem Knotenpool für `aks scale` entfernt</span><span class="sxs-lookup"><span data-stu-id="fc109-1571">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="fc109-1572">AppService</span><span class="sxs-lookup"><span data-stu-id="fc109-1572">Appservice</span></span>
* <span data-ttu-id="fc109-1573">Problem behoben, bei dem für `webapp config container` der Parameter `--slot` nicht berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="fc109-1573">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="fc109-1574">Botservice</span><span class="sxs-lookup"><span data-stu-id="fc109-1574">Botservice</span></span>
* <span data-ttu-id="fc109-1575">Unterstützung für Analyse von `.bot`-Dateien beim Aufrufen von `bot show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1575">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="fc109-1576">Fehler bei der AppInsights-Bereitstellung behoben</span><span class="sxs-lookup"><span data-stu-id="fc109-1576">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="fc109-1577">Leerzeichenfehler bei Dateipfaden behoben</span><span class="sxs-lookup"><span data-stu-id="fc109-1577">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="fc109-1578">Kudu-Netzwerkaufrufe reduziert</span><span class="sxs-lookup"><span data-stu-id="fc109-1578">Reduced Kudu network calls</span></span>
* <span data-ttu-id="fc109-1579">Allgemeine Verbesserungen bei Befehlen der Benutzeroberfläche durchgeführt</span><span class="sxs-lookup"><span data-stu-id="fc109-1579">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="fc109-1580">Nutzung</span><span class="sxs-lookup"><span data-stu-id="fc109-1580">Consumption</span></span>
* <span data-ttu-id="fc109-1581">Fehler für Budget-API zum Anzeigen von Benachrichtigungen behoben</span><span class="sxs-lookup"><span data-stu-id="fc109-1581">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="fc109-1582">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="fc109-1582">CosmosDB</span></span>
* <span data-ttu-id="fc109-1583">Unterstützung für die Aktualisierung des Kontos von „Singlemaster“ auf „Multimaster“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1583">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="fc109-1584">Karten</span><span class="sxs-lookup"><span data-stu-id="fc109-1584">Maps</span></span>
* <span data-ttu-id="fc109-1585">Unterstützung für SKU „S1“ für `maps account [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1585">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="fc109-1586">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="fc109-1586">Network</span></span>
* <span data-ttu-id="fc109-1587">Unterstützung für `--format` und `--log-version` für `watcher flow-log configure` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1587">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="fc109-1588">Problem mit `dns zone update` behoben, bei dem die Verwendung von "" zum Löschen von Auflösungs- und Registrierungs-VNETs nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="fc109-1588">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="fc109-1589">Resource</span><span class="sxs-lookup"><span data-stu-id="fc109-1589">Resource</span></span>
* <span data-ttu-id="fc109-1590">Verarbeitung des Bereichsparameters für Verwaltungsgruppen in `policy assignment [create|list|delete|show|update]` behoben</span><span class="sxs-lookup"><span data-stu-id="fc109-1590">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="fc109-1591">Neuen Befehl `resource wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1591">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="fc109-1592">Storage</span><span class="sxs-lookup"><span data-stu-id="fc109-1592">Storage</span></span>
*  <span data-ttu-id="fc109-1593">Möglichkeit zum Aktualisieren der Protokollschemaversion für Speicherdienste in `storage logging update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1593">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="fc109-1594">VM</span><span class="sxs-lookup"><span data-stu-id="fc109-1594">VM</span></span>
* <span data-ttu-id="fc109-1595">Absturz in `vm identity remove` behoben, der aufgetreten ist, wenn der angegebenen VM keine verwalteten Dienstidentitäten zugewiesen waren</span><span class="sxs-lookup"><span data-stu-id="fc109-1595">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="fc109-1596">4\. Dezember 2018</span><span class="sxs-lookup"><span data-stu-id="fc109-1596">December 4, 2018</span></span>

<span data-ttu-id="fc109-1597">Version 2.0.52</span><span class="sxs-lookup"><span data-stu-id="fc109-1597">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="fc109-1598">Core</span><span class="sxs-lookup"><span data-stu-id="fc109-1598">Core</span></span>
* <span data-ttu-id="fc109-1599">Unterstützung für mandantenübergreifende Ressourcenbereitstellung für mehrinstanzenfähigen Dienstprinzipal hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1599">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="fc109-1600">Behebung eines Fehlers, aufgrund dessen IDs, die von einem Befehl mit Ausgabe im TSV-Format weitergeleitet wurden, nicht ordnungsgemäß analysiert wurden</span><span class="sxs-lookup"><span data-stu-id="fc109-1600">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="fc109-1601">AppService</span><span class="sxs-lookup"><span data-stu-id="fc109-1601">Appservice</span></span>
* <span data-ttu-id="fc109-1602">[VORSCHAU] Befehl `webapp up` hinzugefügt, der Benutzer beim Erstellen und Bereitstellen von Inhalten in Apps unterstützt</span><span class="sxs-lookup"><span data-stu-id="fc109-1602">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="fc109-1603">Behebung eines Fehlers in einer containerbasierten Windows-App, der aufgrund einer Back-End-Änderung auftrat</span><span class="sxs-lookup"><span data-stu-id="fc109-1603">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="fc109-1604">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="fc109-1604">Network</span></span>
* <span data-ttu-id="fc109-1605">Argument `--exclusion` zu `application-gateway waf-config set` hinzugefügt, um WAF-Ausschlüsse zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="fc109-1605">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="fc109-1606">Role</span><span class="sxs-lookup"><span data-stu-id="fc109-1606">Role</span></span>
* <span data-ttu-id="fc109-1607">Unterstützung für benutzerdefinierte Bezeichner für Kennwortanmeldeinformation hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1607">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="fc109-1608">VM</span><span class="sxs-lookup"><span data-stu-id="fc109-1608">VM</span></span>
* <span data-ttu-id="fc109-1609">[VERALTET] Parameter `vm extension [show|wait] --expand` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="fc109-1609">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="fc109-1610">Parameter `--force` zu `vm restart` hinzugefügt, um nicht reagierende virtuelle Computer erneut bereitzustellen</span><span class="sxs-lookup"><span data-stu-id="fc109-1610">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="fc109-1611">`[vm|vmss] create --authentication-type` geändert, um „all“ zu akzeptieren und einen virtuellen Computer mit Kennwort- und SSH-Authentifizierung zu erstellen</span><span class="sxs-lookup"><span data-stu-id="fc109-1611">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="fc109-1612">Parameter `image create --os-disk-caching` hinzugefügt, um die Zwischenspeicherung von Betriebssystemdatenträgern für ein Image festzulegen</span><span class="sxs-lookup"><span data-stu-id="fc109-1612">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="fc109-1613">20. November 2018</span><span class="sxs-lookup"><span data-stu-id="fc109-1613">November 20, 2018</span></span>

<span data-ttu-id="fc109-1614">Version 2.0.51</span><span class="sxs-lookup"><span data-stu-id="fc109-1614">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="fc109-1615">Core</span><span class="sxs-lookup"><span data-stu-id="fc109-1615">Core</span></span>
* <span data-ttu-id="fc109-1616">MSI-Anmeldung geändert, sodass der Abonnementname nicht in der Identität wiederverwendet wird</span><span class="sxs-lookup"><span data-stu-id="fc109-1616">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="fc109-1617">ACR</span><span class="sxs-lookup"><span data-stu-id="fc109-1617">ACR</span></span>
* <span data-ttu-id="fc109-1618">Kontexttoken zum Aufgabenschritt hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1618">Added context token to task step</span></span>
* <span data-ttu-id="fc109-1619">Unterstützung für das Festlegen von Geheimnissen in „acr run“ zum Spiegeln der ACR-Aufgabe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1619">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="fc109-1620">Unterstützung für `--top` und `--orderby` für die Befehle `show-tags` und `show-manifests` verbessert</span><span class="sxs-lookup"><span data-stu-id="fc109-1620">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="fc109-1621">AppService</span><span class="sxs-lookup"><span data-stu-id="fc109-1621">Appservice</span></span>
* <span data-ttu-id="fc109-1622">Standardtimeout der ZIP-Bereitstellung für das Abrufen des Status auf fünf Minuten erhöht und Timeout-Eigenschaft zum Anpassen dieses Werts hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1622">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="fc109-1623">Aktualisierung der standardmäßigen `node_version`.</span><span class="sxs-lookup"><span data-stu-id="fc109-1623">Updated the default `node_version`.</span></span> <span data-ttu-id="fc109-1624">Während eines Austauschvorgangs mit zwei Phasen werden bei der Austauschaktion zum Zurücksetzen des Slots alle App-Einstellungen und Verbindungszeichenfolgen beibehalten.</span><span class="sxs-lookup"><span data-stu-id="fc109-1624">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="fc109-1625">Clientseitige SKU-Überprüfung für die Erstellung eines Linux-App Service-Plans entfernt</span><span class="sxs-lookup"><span data-stu-id="fc109-1625">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="fc109-1626">Behebung eines Fehlers beim Abrufen des ZipDeploy-Status</span><span class="sxs-lookup"><span data-stu-id="fc109-1626">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="fc109-1627">IotCentral</span><span class="sxs-lookup"><span data-stu-id="fc109-1627">IotCentral</span></span>
* <span data-ttu-id="fc109-1628">Verfügbarkeitsprüfung für Unterdomänen beim Erstellen einer IoT Central-Anwendung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1628">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="fc109-1629">KeyVault</span><span class="sxs-lookup"><span data-stu-id="fc109-1629">KeyVault</span></span>
* <span data-ttu-id="fc109-1630">Behebung eines Fehlers, aufgrund dessen Fehler mitunter ignoriert wurden</span><span class="sxs-lookup"><span data-stu-id="fc109-1630">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="fc109-1631">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="fc109-1631">Network</span></span>
* <span data-ttu-id="fc109-1632">`root-cert`-Unterbefehle zum Behandeln von vertrauenswürdigen Stammzertifikaten zu `application-gateway` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1632">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="fc109-1633">Optionen `--min-capacity` und `--custom-error-pages` zu `application-gateway [create|update]` hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="fc109-1633">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="fc109-1634">`--zones` zur Unterstützung von Verfügbarkeitszonen zu `application-gateway create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1634">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="fc109-1635">Argumente `--file-upload-limit`, `--max-request-body-size` und `--request-body-check` zu `application-gateway waf-config set` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1635">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="fc109-1636">Rdbms</span><span class="sxs-lookup"><span data-stu-id="fc109-1636">Rdbms</span></span>
* <span data-ttu-id="fc109-1637">MariaDB-VNET-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1637">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="fc109-1638">RBAC</span><span class="sxs-lookup"><span data-stu-id="fc109-1638">Rbac</span></span>
* <span data-ttu-id="fc109-1639">Problem beim Aktualisieren unveränderlicher Anmeldeinformationen in `ad app update` behoben</span><span class="sxs-lookup"><span data-stu-id="fc109-1639">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="fc109-1640">Ausgabewarnungen zur Ankündigung bevorstehender Breaking Changes für `ad [app|sp] list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1640">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="fc109-1641">Storage</span><span class="sxs-lookup"><span data-stu-id="fc109-1641">Storage</span></span>
* <span data-ttu-id="fc109-1642">Behandlung von Ausnahmefällen für Speicherkopierbefehle verbessert</span><span class="sxs-lookup"><span data-stu-id="fc109-1642">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="fc109-1643">Problem behoben, aufgrund dessen `storage blob copy start-batch` bei identischen Ziel- und Quellkonten keine Anmeldeinformationen verwendete</span><span class="sxs-lookup"><span data-stu-id="fc109-1643">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="fc109-1644">Fehler bei `storage [blob|file] url` behoben, aufgrund dessen `sas_token` nicht in die URL eingebunden wurde</span><span class="sxs-lookup"><span data-stu-id="fc109-1644">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="fc109-1645">Breaking Change-Warnung zu `[blob|container] list` hinzugefügt: In Kürze werden standardmäßig nur die ersten 5.000 Ergebnisse ausgegeben.</span><span class="sxs-lookup"><span data-stu-id="fc109-1645">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="fc109-1646">VM</span><span class="sxs-lookup"><span data-stu-id="fc109-1646">VM</span></span>
* <span data-ttu-id="fc109-1647">Unterstützung für die separate Angabe einer Speicherkonto-SKU für verwaltete Betriebssystemdatenträger und Datenträger zu `[vm|vmss] create --storage-sku` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1647">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="fc109-1648">Parameter für den Versionsnamen von `sig image-version` in `--image-version -e` geändert</span><span class="sxs-lookup"><span data-stu-id="fc109-1648">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="fc109-1649">`sig image-version`-Argument `--image-version-name` als veraltet markiert und durch `--image-version` ersetzt</span><span class="sxs-lookup"><span data-stu-id="fc109-1649">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="fc109-1650">Unterstützung für die Verwendung des lokalen Betriebssystemdatenträgers für `[vm|vmss] create --ephemeral-os-disk` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1650">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="fc109-1651">Unterstützung für `--no-wait` zu `snapshot create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1651">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="fc109-1652">Befehl `snapshot wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1652">Added `snapshot wait` command</span></span>
* <span data-ttu-id="fc109-1653">Unterstützung für die Verwendung von Instanznamen mit `[vm|vmss] extension set --extension-instance-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1653">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="fc109-1654">6\. November 2018</span><span class="sxs-lookup"><span data-stu-id="fc109-1654">November 6, 2018</span></span>

<span data-ttu-id="fc109-1655">Version 2.0.50</span><span class="sxs-lookup"><span data-stu-id="fc109-1655">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="fc109-1656">Core</span><span class="sxs-lookup"><span data-stu-id="fc109-1656">Core</span></span>
* <span data-ttu-id="fc109-1657">Unterstützung für die Dienstprinzipalauthentifizierung (SN und Aussteller) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1657">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="fc109-1658">ACR</span><span class="sxs-lookup"><span data-stu-id="fc109-1658">ACR</span></span>
* <span data-ttu-id="fc109-1659">Unterstützung für Commit- und Pull Request-Git-Ereignisse für Aufgabenquellentrigger hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1659">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="fc109-1660">Auf Verwendung des Standard-Dockerfiles umgestellt, falls im Erstellungsbefehl kein Dockerfile angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="fc109-1660">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="fc109-1661">ACS</span><span class="sxs-lookup"><span data-stu-id="fc109-1661">ACS</span></span>
* <span data-ttu-id="fc109-1662">[BREAKING CHANGE]`enable_cloud_console_aks_browse` entfernt, um standardmäßig „az aks browse“ zu aktivieren</span><span class="sxs-lookup"><span data-stu-id="fc109-1662">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="fc109-1663">Advisor</span><span class="sxs-lookup"><span data-stu-id="fc109-1663">Advisor</span></span>
* <span data-ttu-id="fc109-1664">Allgemein verfügbares Release</span><span class="sxs-lookup"><span data-stu-id="fc109-1664">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="fc109-1665">AMS</span><span class="sxs-lookup"><span data-stu-id="fc109-1665">AMS</span></span>
* <span data-ttu-id="fc109-1666">Neue Befehlsgruppen hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="fc109-1666">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="fc109-1667">Neue Befehle hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="fc109-1667">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="fc109-1668">Unterstützung von Verschlüsselungsparametern für `ams streaming-policy create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1668">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="fc109-1669">Für `ams transform output remove` kann jetzt der zu entfernende Ausgabeindex angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="fc109-1669">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="fc109-1670">Argumente `--correlation-data` und `--label` zur Befehlsgruppe `ams job` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1670">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="fc109-1671">Argumente `--storage-account` und `--container` zur Befehlsgruppe `ams asset` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1671">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="fc109-1672">Standardwerte für Ablaufzeit (aktueller Zeitpunkt + 23 Std.) und Berechtigungen (Lesen) im Befehl `ams asset get-sas-url` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1672">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="fc109-1673">[BREAKING CHANGE] Befehl `ams streaming locator` durch `ams streaming-locator` ersetzt</span><span class="sxs-lookup"><span data-stu-id="fc109-1673">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="fc109-1674">[BREAKING CHANGE] Argument `--content-keys` von `ams streaming locator` aktualisiert</span><span class="sxs-lookup"><span data-stu-id="fc109-1674">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="fc109-1675">[BREAKING CHANGE]`--content-policy-name` im Befehl `ams streaming locator` in `--content-key-policy-name` umbenannt</span><span class="sxs-lookup"><span data-stu-id="fc109-1675">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="fc109-1676">[BREAKING CHANGE] Befehl `ams streaming policy` durch `ams streaming-policy` ersetzt</span><span class="sxs-lookup"><span data-stu-id="fc109-1676">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="fc109-1677">[BREAKING CHANGE] Das Argument `--preset-names` wurde in der Befehlsgruppe `--preset` durch `ams transform` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="fc109-1677">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="fc109-1678">Ab sofort kann nur noch eine einzelne Ausgabe/Voreinstellung festgelegt werden. (Wenn Sie weitere hinzufügen möchten, müssen Sie `ams transform output add` ausführen.)</span><span class="sxs-lookup"><span data-stu-id="fc109-1678">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="fc109-1679">Darüber hinaus können Sie eine benutzerdefinierte Voreinstellung für den Standard-Encoder (StandardEncoderPreset) festlegen, indem Sie den Pfad an Ihr benutzerdefiniertes JSON-Objekt übergeben.</span><span class="sxs-lookup"><span data-stu-id="fc109-1679">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="fc109-1680">[BREAKING CHANGE]`--output-asset-names ` wurde im Befehl `ams job start` in `--output-assets` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="fc109-1680">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="fc109-1681">Ab sofort wird eine durch Leerzeichen getrennte Ressourcenliste im Format „assetName=Bezeichnung“ akzeptiert.</span><span class="sxs-lookup"><span data-stu-id="fc109-1681">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="fc109-1682">Ressourcen ohne Bezeichnung können wie folgt gesendet werden: „assetName=“.</span><span class="sxs-lookup"><span data-stu-id="fc109-1682">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="fc109-1683">AppService</span><span class="sxs-lookup"><span data-stu-id="fc109-1683">AppService</span></span>
* <span data-ttu-id="fc109-1684">Fehler in `az webapp config backup update` behoben, der dazu führte, dass kein Sicherungszeitplan festgelegt werden konnte, wenn noch keiner festgelegt war</span><span class="sxs-lookup"><span data-stu-id="fc109-1684">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="fc109-1685">Konfigurieren</span><span class="sxs-lookup"><span data-stu-id="fc109-1685">Configure</span></span>
* <span data-ttu-id="fc109-1686">YAML zu Ausgabeformatoptionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1686">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="fc109-1687">Container</span><span class="sxs-lookup"><span data-stu-id="fc109-1687">Container</span></span>
* <span data-ttu-id="fc109-1688">Auf Anzeige der Identität umgestellt, wenn eine Containergruppe nach YAML exportiert wird</span><span class="sxs-lookup"><span data-stu-id="fc109-1688">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="fc109-1689">EventHub</span><span class="sxs-lookup"><span data-stu-id="fc109-1689">EventHub</span></span>
* <span data-ttu-id="fc109-1690">Flag `--enable-kafka` hinzugefügt, um Kafka in `eventhub namespace [create|update]` zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="fc109-1690">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="fc109-1691">Interactive</span><span class="sxs-lookup"><span data-stu-id="fc109-1691">Interactive</span></span>
* <span data-ttu-id="fc109-1692">Interactive installiert nun die Erweiterung `interactive`, um schnellere Updates und schnelleren Support zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="fc109-1692">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="fc109-1693">Überwachen</span><span class="sxs-lookup"><span data-stu-id="fc109-1693">Monitor</span></span>
* <span data-ttu-id="fc109-1694">Unterstützung für Metriknamen mit Schrägstrichen und Punkten zu `--condition` in `monitor metrics alert [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1694">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="fc109-1695">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="fc109-1695">Network</span></span>
* <span data-ttu-id="fc109-1696">Befehlsnamen vom Typ `network interface-endpoint` zugunsten von `network private-endpoint` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="fc109-1696">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="fc109-1697">Problem behoben, das dazu führte, dass das Argument `--peer-circuit` in `express-route peering connection create` keine ID akzeptiert</span><span class="sxs-lookup"><span data-stu-id="fc109-1697">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="fc109-1698">Problem behoben, das dazu führte, dass `--ip-tags` mit `public-ip create` nicht ordnungsgemäß funktioniert</span><span class="sxs-lookup"><span data-stu-id="fc109-1698">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="fc109-1699">Profil</span><span class="sxs-lookup"><span data-stu-id="fc109-1699">Profile</span></span>
* <span data-ttu-id="fc109-1700">`--use-cert-sn-issuer` zu `az login` hinzugefügt, um Dienstprinzipalanmeldungen mit automatischem Zertifikatrollover zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="fc109-1700">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="fc109-1701">RDBMS</span><span class="sxs-lookup"><span data-stu-id="fc109-1701">RDBMS</span></span>
* <span data-ttu-id="fc109-1702">MySQL-Replikatbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1702">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="fc109-1703">Resource</span><span class="sxs-lookup"><span data-stu-id="fc109-1703">Resource</span></span>
* <span data-ttu-id="fc109-1704">Unterstützung für Verwaltungsgruppen und Abonnements zu Befehlen vom Typ `policy definition|set-definition` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1704">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="fc109-1705">Role</span><span class="sxs-lookup"><span data-stu-id="fc109-1705">Role</span></span>
* <span data-ttu-id="fc109-1706">Unterstützung für die API-Berechtigungsverwaltung, den angemeldeten Benutzer und die Verwaltung von Anwendungskennwörtern und Zertifikatanmeldeinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1706">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="fc109-1707">`ad sp create-for-rbac` geändert, um „displayName“ und Dienstprinzipalname besser unterscheiden zu können</span><span class="sxs-lookup"><span data-stu-id="fc109-1707">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="fc109-1708">Unterstützung der Gewährung von Berechtigungen für AAD-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1708">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="fc109-1709">Storage</span><span class="sxs-lookup"><span data-stu-id="fc109-1709">Storage</span></span>
* <span data-ttu-id="fc109-1710">Möglichkeit hinzugefügt, allein mit SAS und Endpunkten (ohne Kontoname oder Schlüssel) eine Verbindung mit Speicherdiensten herzustellen, wie unter `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>` beschrieben</span><span class="sxs-lookup"><span data-stu-id="fc109-1710">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="fc109-1711">VM</span><span class="sxs-lookup"><span data-stu-id="fc109-1711">VM</span></span>
* <span data-ttu-id="fc109-1712">Argument `storage-sku` zu `image create` hinzugefügt, um das Festlegen des standardmäßigen Speicherkontotyps für das Image zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="fc109-1712">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="fc109-1713">Fehler für `vm resize` behoben, durch den die Option `--no-wait` einen Absturz des Befehls verursachte</span><span class="sxs-lookup"><span data-stu-id="fc109-1713">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="fc109-1714">Tabellenausgabeformat für `vm encryption show` geändert, um den Status anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="fc109-1714">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="fc109-1715">`vm secret format` geändert, um JSON/JSONC-Ausgabe erforderlich zu machen.</span><span class="sxs-lookup"><span data-stu-id="fc109-1715">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="fc109-1716">Der Benutzer wird gewarnt, und es wird standardmäßig die JSON-Ausgabe verwendet, wenn ein unzulässiges Ausgabeformat ausgewählt wird.</span><span class="sxs-lookup"><span data-stu-id="fc109-1716">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="fc109-1717">Argumentüberprüfung für `vm create --image` verbessert</span><span class="sxs-lookup"><span data-stu-id="fc109-1717">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="fc109-1718">23. Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="fc109-1718">October 23, 2018</span></span>

<span data-ttu-id="fc109-1719">Version 2.0.49</span><span class="sxs-lookup"><span data-stu-id="fc109-1719">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="fc109-1720">Core</span><span class="sxs-lookup"><span data-stu-id="fc109-1720">Core</span></span>
* <span data-ttu-id="fc109-1721">Problem mit `--ids` behoben, aufgrund dessen `--subscription` Vorrang vor dem Abonnement in `--ids` hatte</span><span class="sxs-lookup"><span data-stu-id="fc109-1721">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="fc109-1722">Ausdrückliche Warnungen hinzugefügt, wenn Parameter durch die Verwendung von `--ids` ignoriert würden</span><span class="sxs-lookup"><span data-stu-id="fc109-1722">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="fc109-1723">ACR</span><span class="sxs-lookup"><span data-stu-id="fc109-1723">ACR</span></span>
* <span data-ttu-id="fc109-1724">Problem mit der ACR Build-Codierung in Python2 behoben</span><span class="sxs-lookup"><span data-stu-id="fc109-1724">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="fc109-1725">CDN</span><span class="sxs-lookup"><span data-stu-id="fc109-1725">CDN</span></span>
* <span data-ttu-id="fc109-1726">[BREAKING CHANGE] Standardverhalten beim Zwischenspeichern der Abfragezeichenfolge von `cdn endpoint create` so geändert, dass der Standardwert nicht mehr „IgnoreQueryString“ ist.</span><span class="sxs-lookup"><span data-stu-id="fc109-1726">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="fc109-1727">Er wird jetzt vom Dienst festgelegt.</span><span class="sxs-lookup"><span data-stu-id="fc109-1727">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="fc109-1728">Container</span><span class="sxs-lookup"><span data-stu-id="fc109-1728">Container</span></span>
* <span data-ttu-id="fc109-1729">`Private` als gültiger Typ für die Übergabe an „--ip-address“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1729">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="fc109-1730">Geändert, sodass nur eine Subnetz-ID für das Einrichten eines virtuellen Netzwerks für die Containergruppe zulässig ist</span><span class="sxs-lookup"><span data-stu-id="fc109-1730">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="fc109-1731">Geändert, sodass das Verwenden eines VNET-Namens oder einer Ressourcen-ID zulässig ist, um die Verwendung von VNETs aus verschiedenen Ressourcengruppen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="fc109-1731">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="fc109-1732">`--assign-identity` hinzugefügt, um einer Containergruppe eine MSI-Identität hinzuzufügen</span><span class="sxs-lookup"><span data-stu-id="fc109-1732">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="fc109-1733">`--scope` hinzugefügt, um eine Rollenzuweisung für die vom System zugewiesene MSI-Identität zu erstellen</span><span class="sxs-lookup"><span data-stu-id="fc109-1733">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="fc109-1734">Warnung hinzugefügt, wenn eine Containergruppe mit einem Image ohne Prozess mit langer Ausführungszeit erstellt wird</span><span class="sxs-lookup"><span data-stu-id="fc109-1734">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="fc109-1735">Probleme mit der Tabellenausgabe für Befehle `list` und `show` behoben</span><span class="sxs-lookup"><span data-stu-id="fc109-1735">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="fc109-1736">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="fc109-1736">CosmosDB</span></span>
* <span data-ttu-id="fc109-1737">Unterstützung für `--enable-multiple-write-locations` zu `cosmosdb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1737">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="fc109-1738">Interactive</span><span class="sxs-lookup"><span data-stu-id="fc109-1738">Interactive</span></span>
* <span data-ttu-id="fc109-1739">Geändert, um sicherzustellen, dass der Parameter für globales Abonnement in Parametern angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="fc109-1739">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="fc109-1740">IoT Central</span><span class="sxs-lookup"><span data-stu-id="fc109-1740">IoT Central</span></span>
* <span data-ttu-id="fc109-1741">Optionen für Vorlagen und Anzeigenamen für die Erstellung von IoT Central-Anwendungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1741">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="fc109-1742">[BREAKING CHANGE] Unterstützung für F1-SKU entfernt; stattdessen ist die S1-SKU zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="fc109-1742">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="fc109-1743">Überwachen</span><span class="sxs-lookup"><span data-stu-id="fc109-1743">Monitor</span></span>
* <span data-ttu-id="fc109-1744">Änderungen an `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="fc109-1744">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="fc109-1745">Unterstützung für das Auflisten aller Ereignisse auf Abonnementebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1745">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="fc109-1746">`--offset`-Parameter für das einfachere Erstellen von Zeitabfragen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1746">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="fc109-1747">Validierung für `--start-time` und `--end-time` verbessert, um die Verwendung von mehr ISO8601-Formate und benutzerfreundlicheren datetime-Formaten zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="fc109-1747">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="fc109-1748">`--namespace` als Alias für veraltete Option `--resource-provider` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1748">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="fc109-1749">`--filters` als veraltet markiert, da vom Dienst ausschließlich Werte mit stark typisierten Optionen unterstützt werden</span><span class="sxs-lookup"><span data-stu-id="fc109-1749">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="fc109-1750">Änderungen an `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="fc109-1750">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="fc109-1751">`--offset`-Parameter für das einfachere Erstellen von Zeitabfragen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1751">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="fc109-1752">Validierung für `--start-time` und `--end-time` verbessert, um die Verwendung von mehr ISO8601-Formate und benutzerfreundlicheren datetime-Formaten zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="fc109-1752">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="fc109-1753">Validierung für `--event-hub`- und `--event-hub-rule`-Argumente an `monitor diagnostic-settings create` verbessert</span><span class="sxs-lookup"><span data-stu-id="fc109-1753">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="fc109-1754">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="fc109-1754">Network</span></span>
* <span data-ttu-id="fc109-1755">`--app-gateway-address-pools`- und `--gateway-name`-Argumente zu `nic create` hinzugefügt, um das Hinzufügen von Back-End-Adresspools für Anwendungsgateways zu einer NIC zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="fc109-1755">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="fc109-1756">`--app-gateway-address-pools`- und `--gateway-name`-Argumente zu `nic ip-config create/update` hinzugefügt, um das Hinzufügen von Back-End-Adresspools für Anwendungsgateways zu einer NIC zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="fc109-1756">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="fc109-1757">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="fc109-1757">ServiceBus</span></span>
* <span data-ttu-id="fc109-1758">Schreibgeschütztes `migration_state`-Element zu „MigrationConfigProperties“ hinzugefügt, um den aktuellen Status der Migration von Service Bus Standard- zu Premium-Namespace anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="fc109-1758">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="fc109-1759">SQL</span><span class="sxs-lookup"><span data-stu-id="fc109-1759">SQL</span></span>
* <span data-ttu-id="fc109-1760">`sql failover-group create` und `sql failover-group update` korrigiert, damit die Verwendung einer Richtlinie für manuelles Failover möglich ist</span><span class="sxs-lookup"><span data-stu-id="fc109-1760">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="fc109-1761">Storage</span><span class="sxs-lookup"><span data-stu-id="fc109-1761">Storage</span></span>
* <span data-ttu-id="fc109-1762">Formatierung der `az storage cors list`-Ausgabe korrigiert, sodass alle Elemente den richtigen Dienstschlüssel anzeigen</span><span class="sxs-lookup"><span data-stu-id="fc109-1762">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="fc109-1763">`--bypass-immutability-policy`-Parameter für das Löschen von durch Unveränderlichkeitsrichtlinien blockierten Containern hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1763">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="fc109-1764">VM</span><span class="sxs-lookup"><span data-stu-id="fc109-1764">VM</span></span>
* <span data-ttu-id="fc109-1765">Datenträger-Zwischenspeicherungsmodus `None` für Lv/Lv2-Computerserine in `[vm|vmss] create` erzwungen</span><span class="sxs-lookup"><span data-stu-id="fc109-1765">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="fc109-1766">Liste der unterstützten Größen für unterstützenden Netzwerkbeschleuniger für `vm create` aktualisiert</span><span class="sxs-lookup"><span data-stu-id="fc109-1766">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="fc109-1767">Stark typisierte Argumente für UltraSSD-IOPS und MBit/s-Konfigurationen für `disk create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1767">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="fc109-1768">16. Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="fc109-1768">October 16, 2018</span></span>

<span data-ttu-id="fc109-1769">Version 2.0.48</span><span class="sxs-lookup"><span data-stu-id="fc109-1769">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="fc109-1770">VM</span><span class="sxs-lookup"><span data-stu-id="fc109-1770">VM</span></span>
* <span data-ttu-id="fc109-1771">SDK-Problem behoben, das ein Fehlschlagen der Homebrew-Installation verursacht hat</span><span class="sxs-lookup"><span data-stu-id="fc109-1771">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="fc109-1772">9\. Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="fc109-1772">October 9, 2018</span></span>

<span data-ttu-id="fc109-1773">Version 2.0.47</span><span class="sxs-lookup"><span data-stu-id="fc109-1773">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="fc109-1774">Core</span><span class="sxs-lookup"><span data-stu-id="fc109-1774">Core</span></span>
* <span data-ttu-id="fc109-1775">Verbesserte Fehlerbehandlung für Fehler vom Typ „Ungültige Anforderung“</span><span class="sxs-lookup"><span data-stu-id="fc109-1775">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="fc109-1776">ACR</span><span class="sxs-lookup"><span data-stu-id="fc109-1776">ACR</span></span>
* <span data-ttu-id="fc109-1777">Unterstützung für ähnliches Tabellenformat wie Helm-Client hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1777">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="fc109-1778">ACS</span><span class="sxs-lookup"><span data-stu-id="fc109-1778">ACS</span></span>
* <span data-ttu-id="fc109-1779">`aks [create|scale] --nodepool-name` zum Konfigurieren des Knotenpoolnamens hinzugefügt, auf 12 Zeichen gekürzt, Standard: nodepool1</span><span class="sxs-lookup"><span data-stu-id="fc109-1779">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="fc109-1780">Korrektur, bei der auf „scp“ zurückgegriffen wird, wenn Parimiko nicht funktioniert</span><span class="sxs-lookup"><span data-stu-id="fc109-1780">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="fc109-1781">`aks create` geändert, sodass `--aad-tenant-id` nicht mehr erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="fc109-1781">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="fc109-1782">Verbesserte Zusammenführung von Kubernetes-Anmeldeinformationen, wenn doppelte Einträge vorhanden sind</span><span class="sxs-lookup"><span data-stu-id="fc109-1782">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="fc109-1783">Container</span><span class="sxs-lookup"><span data-stu-id="fc109-1783">Container</span></span>
* <span data-ttu-id="fc109-1784">`functionapp create` geändert, sodass das Erstellen eines Linux-Nutzungsplans mit einer bestimmten Runtime unterstützt wird</span><span class="sxs-lookup"><span data-stu-id="fc109-1784">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="fc109-1785">[VORSCHAUVERSION] Unterstützung für das Hosten von Web-Apps in Windows-Containern hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1785">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="fc109-1786">Event Hub</span><span class="sxs-lookup"><span data-stu-id="fc109-1786">Event Hub</span></span>
* <span data-ttu-id="fc109-1787">Befehl `eventhub update` korrigiert</span><span class="sxs-lookup"><span data-stu-id="fc109-1787">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="fc109-1788">[BREAKING CHANGE]`list`-Befehle geändert, sodass Fehler von Typ „NotFound(404)“ für Ressourcen mit der typische Vorgehensweise behandelt werden, anstatt eine leere Liste anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="fc109-1788">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="fc109-1789">Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="fc109-1789">Extensions</span></span>
* <span data-ttu-id="fc109-1790">Problem beim Hinzufügen einer Erweiterung behoben, die bereits installiert ist</span><span class="sxs-lookup"><span data-stu-id="fc109-1790">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="fc109-1791">HDInsight</span><span class="sxs-lookup"><span data-stu-id="fc109-1791">HDInsight</span></span>
* <span data-ttu-id="fc109-1792">Erste Veröffentlichung</span><span class="sxs-lookup"><span data-stu-id="fc109-1792">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="fc109-1793">IoT</span><span class="sxs-lookup"><span data-stu-id="fc109-1793">IoT</span></span>
* <span data-ttu-id="fc109-1794">Befehl zur Erweiterungsinstallation zu Banner bei der ersten Ausführung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1794">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="fc109-1795">KeyVault</span><span class="sxs-lookup"><span data-stu-id="fc109-1795">KeyVault</span></span>
* <span data-ttu-id="fc109-1796">Geändert, sodass Key Vault-Speicherbefehle auf das aktuelle API-Profil beschränkt sind</span><span class="sxs-lookup"><span data-stu-id="fc109-1796">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="fc109-1797">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="fc109-1797">Network</span></span>
* <span data-ttu-id="fc109-1798">`network dns zone create` korrigiert: Befehl ist auch erfolgreich, wenn der Benutzer einen Standardspeicherort konfiguriert hat.</span><span class="sxs-lookup"><span data-stu-id="fc109-1798">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="fc109-1799">Siehe Nr. 6052</span><span class="sxs-lookup"><span data-stu-id="fc109-1799">See #6052</span></span>
* <span data-ttu-id="fc109-1800">`--remote-vnet-id` für `network vnet peering create` eingestellt</span><span class="sxs-lookup"><span data-stu-id="fc109-1800">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="fc109-1801">`--remote-vnet` zum `network vnet peering create`-Element hinzugefügt, das einen Namen oder eine ID akzeptiert</span><span class="sxs-lookup"><span data-stu-id="fc109-1801">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="fc109-1802">Unterstützung für mehrere Subnetzpräfixe zu `network vnet create` in `--subnet-prefixes` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1802">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="fc109-1803">Unterstützung für mehrere Subnetzpräfixe zu `network vnet subnet [create|update]` in `--address-prefixes` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1803">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="fc109-1804">Problem mit `network application-gateway create` behoben, das die Erstellung von Gateways mit der SKU `WAF_v2` oder `Standard_v2` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="fc109-1804">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="fc109-1805">`--service-endpoint-policy`-Argument für Benutzerfreundlichkeit zu `network vnet subnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1805">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="fc109-1806">Role</span><span class="sxs-lookup"><span data-stu-id="fc109-1806">Role</span></span>
* <span data-ttu-id="fc109-1807">Unterstützung für das Auflisten von Azure AD-App-Besitzern in `ad app owner` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1807">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="fc109-1808">Unterstützung für das Auflisten von Azure AD-Dienstprinzipalbesitzern in `ad sp owner` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1808">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="fc109-1809">Geändert, um sicherzustellen, dass die Erstellungs- und Aktualisierungsbefehle für die Rollendefinition Konfigurationen mit mehreren Berechtigungen akzeptieren</span><span class="sxs-lookup"><span data-stu-id="fc109-1809">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="fc109-1810">`ad sp create-for-rbac` geändert, um sicherzustellen, dass der Homepage-URI immer „https“ ist</span><span class="sxs-lookup"><span data-stu-id="fc109-1810">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="fc109-1811">Service Bus</span><span class="sxs-lookup"><span data-stu-id="fc109-1811">Service Bus</span></span>
* <span data-ttu-id="fc109-1812">[BREAKING CHANGE]`list`-Befehle geändert, sodass Fehler von Typ „NotFound(404)“ für Ressourcen mit der typische Vorgehensweise behandelt werden, anstatt eine leere Liste anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="fc109-1812">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="fc109-1813">VM</span><span class="sxs-lookup"><span data-stu-id="fc109-1813">VM</span></span>
* <span data-ttu-id="fc109-1814">Leeres `accessSas`-Feld in `disk grant-access` korrigiert</span><span class="sxs-lookup"><span data-stu-id="fc109-1814">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="fc109-1815">`vmss create` geändert, sodass ein ausreichend großer Front-End-Portbereich zur Verarbeitung von Überbereitstellung reserviert ist</span><span class="sxs-lookup"><span data-stu-id="fc109-1815">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="fc109-1816">Aktualisierungsbefehle für `sig` korrigiert</span><span class="sxs-lookup"><span data-stu-id="fc109-1816">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="fc109-1817">`--no-wait`-Unterstützung für die Verwaltung von Imageversionen in `sig` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1817">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="fc109-1818">`vm list-ip-addresses` geändert, sodass die Verfügbarkeitszone von öffentlichen IP-Adressen angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="fc109-1818">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="fc109-1819">`[vm|vmss] disk attach` geändert, sodass die Standard-LUN eines Datenträgers standardmäßig auf die erste verfügbare Stelle festgelegt wird</span><span class="sxs-lookup"><span data-stu-id="fc109-1819">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="fc109-1820">21. September 2018</span><span class="sxs-lookup"><span data-stu-id="fc109-1820">September 21, 2018</span></span>

<span data-ttu-id="fc109-1821">Version 2.0.46</span><span class="sxs-lookup"><span data-stu-id="fc109-1821">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="fc109-1822">ACR</span><span class="sxs-lookup"><span data-stu-id="fc109-1822">ACR</span></span>
* <span data-ttu-id="fc109-1823">ACR-Aufgabenbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1823">Added ACR Task commands</span></span>
* <span data-ttu-id="fc109-1824">Befehl für die Schnellausführung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1824">Added quick run command</span></span>
* <span data-ttu-id="fc109-1825">`build-task`-Befehlsgruppe als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="fc109-1825">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="fc109-1826">`helm`-Befehlsgruppe hinzugefügt, um die Verwaltung von Helm-Diagrammen mit ACR zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="fc109-1826">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="fc109-1827">Unterstützung für idempotentes Erstellen für die verwaltete Registrierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1827">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="fc109-1828">Formatfreies Flag für die Anzeige von Buildprotokollen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1828">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="fc109-1829">ACS</span><span class="sxs-lookup"><span data-stu-id="fc109-1829">ACS</span></span>
* <span data-ttu-id="fc109-1830">Befehl `install-connector` zum Festlegen des AKS-Master-FQDN geändert</span><span class="sxs-lookup"><span data-stu-id="fc109-1830">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="fc109-1831">Erstellen der Rollenzuweisung für „vnet-subnet-id“ (wenn kein Dienstprinzipal angegeben wurde) und „skip-role-assignment“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="fc109-1831">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="fc109-1832">AppService</span><span class="sxs-lookup"><span data-stu-id="fc109-1832">AppService</span></span>

* <span data-ttu-id="fc109-1833">Unterstützung für WebJobs-Vorgangsverwaltung hinzugefügt (kontinuierlich/ausgelöst)</span><span class="sxs-lookup"><span data-stu-id="fc109-1833">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="fc109-1834">„az webapp config set“ unterstützt die Eigenschaft „--fts-state“; Unterstützung für „az functionapp config set/show“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1834">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="fc109-1835">Unterstützung für Bring Your Own Storage für Web-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1835">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="fc109-1836">Unterstützung für das Auflisten und Wiederherstellen gelöschter Web-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1836">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="fc109-1837">Batch</span><span class="sxs-lookup"><span data-stu-id="fc109-1837">Batch</span></span>
* <span data-ttu-id="fc109-1838">Hinzufügen von Aufgaben über `--json-file` geändert, um die AddTaskCollectionParameter-Syntax zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="fc109-1838">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="fc109-1839">Dokumentation akzeptierter `--json-file`-Formate aktualisiert</span><span class="sxs-lookup"><span data-stu-id="fc109-1839">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="fc109-1840">`--max-tasks-per-node-option` zu `batch pool create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1840">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="fc109-1841">Verhalten von `batch account` geändert, um das aktuell angemeldete Konto anzuzeigen, wenn keine Optionen angegeben wurden</span><span class="sxs-lookup"><span data-stu-id="fc109-1841">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="fc109-1842">Batch KI</span><span class="sxs-lookup"><span data-stu-id="fc109-1842">Batch AI</span></span> 
* <span data-ttu-id="fc109-1843">Fehler bei der automatischen Speicherkontoerstellung im Befehl `batchai cluster create` behoben</span><span class="sxs-lookup"><span data-stu-id="fc109-1843">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="fc109-1844">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="fc109-1844">Cognitive Services</span></span>
* <span data-ttu-id="fc109-1845">Vervollständigung für die Argumente `--sku`, `--kind` und `--location` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1845">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="fc109-1846">Befehl `cognitiveservices account list-usage` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1846">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="fc109-1847">Befehl `cognitiveservices account list-kinds` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1847">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="fc109-1848">Befehl `cognitiveservices account list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1848">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="fc109-1849">`cognitiveservices list` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="fc109-1849">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="fc109-1850">`--name` geändert (ist jetzt optional für `cognitiveservices account list-skus`)</span><span class="sxs-lookup"><span data-stu-id="fc109-1850">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="fc109-1851">Container</span><span class="sxs-lookup"><span data-stu-id="fc109-1851">Container</span></span>
* <span data-ttu-id="fc109-1852">Möglichkeit zum Neustarten und Beenden einer ausgeführten Containergruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1852">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="fc109-1853">`--network-profile` zum Übergeben eines Netzwerkprofils hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1853">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="fc109-1854">`--subnet` und `--vnet_name` hinzugefügt, um das Erstellen von Containergruppen in einem VNET zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="fc109-1854">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="fc109-1855">Tabellenausgabe geändert, sodass der Status der Containergruppe angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="fc109-1855">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="fc109-1856">Data Lake</span><span class="sxs-lookup"><span data-stu-id="fc109-1856">Datalake</span></span>
* <span data-ttu-id="fc109-1857">Befehle für VNET-Regeln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1857">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="fc109-1858">Interaktive Shell</span><span class="sxs-lookup"><span data-stu-id="fc109-1858">Interactive Shell</span></span>
* <span data-ttu-id="fc109-1859">Fehler in Windows behoben, durch den Befehle nicht ordnungsgemäß ausgeführt wurden</span><span class="sxs-lookup"><span data-stu-id="fc109-1859">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="fc109-1860">Durch veraltete Objekte verursachtes Problem beim Laden von Befehlen im interaktiven Modus behoben</span><span class="sxs-lookup"><span data-stu-id="fc109-1860">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="fc109-1861">IoT</span><span class="sxs-lookup"><span data-stu-id="fc109-1861">IoT</span></span>
* <span data-ttu-id="fc109-1862">Routingunterstützung für IoT Hubs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1862">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="fc109-1863">Key Vault</span><span class="sxs-lookup"><span data-stu-id="fc109-1863">Key Vault</span></span>
* <span data-ttu-id="fc109-1864">Key Vault-Schlüsselimport für RSA-Schlüssel korrigiert</span><span class="sxs-lookup"><span data-stu-id="fc109-1864">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="fc109-1865">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="fc109-1865">Network</span></span>
* <span data-ttu-id="fc109-1866">Befehle vom Typ `network public-ip prefix` hinzugefügt, um Präfixe von öffentlichen IP-Adressen zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="fc109-1866">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="fc109-1867">Befehle vom Typ `network service-endpoint` hinzugefügt, um Dienstendpunktrichtlinien-Features zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="fc109-1867">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="fc109-1868">Befehle vom Typ `network lb outbound-rule` hinzugefügt, um die Erstellung von Ausgangsregeln für Load Balancer Standard zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="fc109-1868">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="fc109-1869">`--public-ip-prefix` zu `network lb frontend-ip create/update` hinzugefügt, um Front-End-IP-Konfigurationen mit Präfixen von öffentlichen IP-Adressen zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="fc109-1869">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="fc109-1870">`--enable-tcp-reset` zu `network lb rule/inbound-nat-rule/inbound-nat-pool create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1870">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="fc109-1871">`--disable-outbound-snat` zu `network lb rule create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1871">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="fc109-1872">Verwendung von `network watcher flow-log show/configure` mit klassischen NSGs ermöglicht</span><span class="sxs-lookup"><span data-stu-id="fc109-1872">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="fc109-1873">Hinzufügen des `network watcher run-configuration-diagnostic`-Befehls</span><span class="sxs-lookup"><span data-stu-id="fc109-1873">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="fc109-1874">Befehl `network watcher test-connectivity` korrigiert und Eigenschaften `--method`, `--valid-status-codes` und `--headers` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1874">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="fc109-1875">`network express-route create/update`: Flag `--allow-global-reach` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1875">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="fc109-1876">`network vnet subnet create/update`: Unterstützung für `--delegation` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1876">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="fc109-1877">Befehl `network vnet subnet list-available-delegations` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1877">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="fc109-1878">`network traffic-manager profile create/update`: Unterstützung für `--interval`, `--timeout` und `--max-failures` für die Überwachungskonfiguration hinzugefügt; Optionen `--monitor-path`, `--monitor-port` und `--monitor-protocol` zugunsten von `--path`, `--port` und `--protocol` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="fc109-1878">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="fc109-1879">`network lb frontend-ip create/update`: Logik für das Festlegen der Zuweisungsmethode für private IP-Adressen korrigiert. Bei Angabe einer privaten IP-Adresse ist die Zuweisung statisch. Wird keine private IP-Adresse (oder eine leere Zeichenfolge für die private IP-Adresse) angegeben, erfolgt eine dynamische Zuweisung.</span><span class="sxs-lookup"><span data-stu-id="fc109-1879">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="fc109-1880">`dns record-set * create/update`: Unterstützung für `--target-resource` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1880">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="fc109-1881">Befehle vom Typ `network interface-endpoint` hinzugefügt, um Schnittstellenendpunkt-Objekte abzufragen</span><span class="sxs-lookup"><span data-stu-id="fc109-1881">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="fc109-1882">`network profile show/list/delete` für die partielle Verwaltung von Netzwerkprofilen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1882">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="fc109-1883">Befehle vom Typ `network express-route peering connection` für die Verwaltung von Peeringverbindungen zwischen ExpressRoute-Instanzen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1883">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="fc109-1884">RDBMS</span><span class="sxs-lookup"><span data-stu-id="fc109-1884">RDBMS</span></span>
* <span data-ttu-id="fc109-1885">Unterstützung für den MariaDB-Dienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1885">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="fc109-1886">Reservierung</span><span class="sxs-lookup"><span data-stu-id="fc109-1886">Reservation</span></span>
* <span data-ttu-id="fc109-1887">Cosmos DB im Enumerationstyp für reservierte Ressourcen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1887">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="fc109-1888">Namenseigenschaft im Patchmodell hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1888">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="fc109-1889">App-Verwaltung</span><span class="sxs-lookup"><span data-stu-id="fc109-1889">Manage App</span></span>
* <span data-ttu-id="fc109-1890">Fehler in `managedapp create --kind MarketPlace` korrigiert, der zum Absturz der Instanzerstellung einer verwalteten Marketplace-App führte</span><span class="sxs-lookup"><span data-stu-id="fc109-1890">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="fc109-1891">Befehle vom Typ `feature` geändert, um sie auf unterstützte Profile zu beschränken</span><span class="sxs-lookup"><span data-stu-id="fc109-1891">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="fc109-1892">Role</span><span class="sxs-lookup"><span data-stu-id="fc109-1892">Role</span></span>
* <span data-ttu-id="fc109-1893">Unterstützung für das Auflisten der Gruppenmitgliedschaften des Benutzers hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1893">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="fc109-1894">SignalR</span><span class="sxs-lookup"><span data-stu-id="fc109-1894">SignalR</span></span>
* <span data-ttu-id="fc109-1895">Erste Version</span><span class="sxs-lookup"><span data-stu-id="fc109-1895">First release</span></span>

### <a name="storage"></a><span data-ttu-id="fc109-1896">Storage</span><span class="sxs-lookup"><span data-stu-id="fc109-1896">Storage</span></span>
* <span data-ttu-id="fc109-1897">Parameter `--auth-mode login` für die Verwendung der Anmeldeinformationen des Benutzers für die Blob- und Warteschlangenautorisierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1897">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="fc109-1898">`storage container immutability-policy/legal-hold` für die Verwaltung von unveränderlichem Speicher hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1898">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="fc109-1899">VM</span><span class="sxs-lookup"><span data-stu-id="fc109-1899">VM</span></span>
* <span data-ttu-id="fc109-1900">Problem behoben, das dazu führte, dass die Datei mit dem privaten Schlüssel durch `vm create --generate-ssh-keys` überschrieben wird, wenn die Datei mit dem privaten Schlüssel fehlt (Nr. 4725, 6780)</span><span class="sxs-lookup"><span data-stu-id="fc109-1900">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="fc109-1901">Unterstützung für den gemeinsamen Image-Katalog über `az sig` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1901">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="fc109-1902">28. August 2018</span><span class="sxs-lookup"><span data-stu-id="fc109-1902">August 28, 2018</span></span>

<span data-ttu-id="fc109-1903">Version 2.0.45</span><span class="sxs-lookup"><span data-stu-id="fc109-1903">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="fc109-1904">Core</span><span class="sxs-lookup"><span data-stu-id="fc109-1904">Core</span></span>

* <span data-ttu-id="fc109-1905">Das Problem, aufgrund dessen eine leere Konfigurationsdatei geladen wurde, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="fc109-1905">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="fc109-1906">Unterstützung für Profil `2018-03-01-hybrid` für Azure Stack hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1906">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="fc109-1907">ACR</span><span class="sxs-lookup"><span data-stu-id="fc109-1907">ACR</span></span>

* <span data-ttu-id="fc109-1908">Problemumgehung für Laufzeitvorgänge ohne ARM-Anforderungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1908">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="fc109-1909">Änderung vorgenommen, um im Befehl `build` Versionskontrolldateien (etwa „.git“ und „.gitignore“) standardmäßig aus der TAR-Datei auszuschließen</span><span class="sxs-lookup"><span data-stu-id="fc109-1909">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="fc109-1910">ACS</span><span class="sxs-lookup"><span data-stu-id="fc109-1910">ACS</span></span>

* <span data-ttu-id="fc109-1911">`aks create` geändert, dass standardmäßig virtuelle Computer vom Typ `Standard_DS2_v2` erstellt werden</span><span class="sxs-lookup"><span data-stu-id="fc109-1911">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="fc109-1912">`aks get-credentials` geändert, um nun neue APIs zum Abrufen der Clusteranmeldeinformationen aufzurufen</span><span class="sxs-lookup"><span data-stu-id="fc109-1912">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="fc109-1913">AppService</span><span class="sxs-lookup"><span data-stu-id="fc109-1913">AppService</span></span>

* <span data-ttu-id="fc109-1914">Unterstützung für CORS in „functionapp“ und „webapp“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1914">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="fc109-1915">ARM-Tagunterstützung in Erstellungsbefehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1915">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="fc109-1916">`[webapp|functionapp] identity show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="fc109-1916">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="fc109-1917">Backup</span><span class="sxs-lookup"><span data-stu-id="fc109-1917">Backup</span></span>

* <span data-ttu-id="fc109-1918">`backup vault backup-properties show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="fc109-1918">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="fc109-1919">Botdienst</span><span class="sxs-lookup"><span data-stu-id="fc109-1919">Bot Service</span></span>

* <span data-ttu-id="fc109-1920">Anfängliches Release der Botdienst-CLI</span><span class="sxs-lookup"><span data-stu-id="fc109-1920">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="fc109-1921">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="fc109-1921">Cognitive Services</span></span>

* <span data-ttu-id="fc109-1922">Neuer Parameter `--api-properties,` hinzugefügt, der zum Erstellen einiger Dienste erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="fc109-1922">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="fc109-1923">IoT</span><span class="sxs-lookup"><span data-stu-id="fc109-1923">IoT</span></span>

* <span data-ttu-id="fc109-1924">Problem mit dem Zuweisen verknüpfter Hubs behoben</span><span class="sxs-lookup"><span data-stu-id="fc109-1924">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="fc109-1925">Überwachen</span><span class="sxs-lookup"><span data-stu-id="fc109-1925">Monitor</span></span>

* <span data-ttu-id="fc109-1926">`monitor metrics alert`-Befehle für Metrikwarnungen nahezu in Echtzeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1926">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="fc109-1927">`monitor alert`-Befehle als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="fc109-1927">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="fc109-1928">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="fc109-1928">Network</span></span>

* <span data-ttu-id="fc109-1929">`network application-gateway ssl-policy predefined show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="fc109-1929">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="fc109-1930">Resource</span><span class="sxs-lookup"><span data-stu-id="fc109-1930">Resource</span></span>

* <span data-ttu-id="fc109-1931">`provider operation show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="fc109-1931">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="fc109-1932">Storage</span><span class="sxs-lookup"><span data-stu-id="fc109-1932">Storage</span></span>

* <span data-ttu-id="fc109-1933">`storage share policy show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="fc109-1933">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="fc109-1934">VM</span><span class="sxs-lookup"><span data-stu-id="fc109-1934">VM</span></span>

* <span data-ttu-id="fc109-1935">`vm/vmss identity show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="fc109-1935">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="fc109-1936">`--storage-caching` für `vm create` eingestellt</span><span class="sxs-lookup"><span data-stu-id="fc109-1936">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="fc109-1937">14. August 2018</span><span class="sxs-lookup"><span data-stu-id="fc109-1937">Auguest 14, 2018</span></span>

<span data-ttu-id="fc109-1938">Version 2.0.44</span><span class="sxs-lookup"><span data-stu-id="fc109-1938">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="fc109-1939">Core</span><span class="sxs-lookup"><span data-stu-id="fc109-1939">Core</span></span>

* <span data-ttu-id="fc109-1940">Numerische Anzeige in `table`-Ausgabe korrigiert</span><span class="sxs-lookup"><span data-stu-id="fc109-1940">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="fc109-1941">YAML-Ausgabeformat hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1941">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="fc109-1942">Telemetrie</span><span class="sxs-lookup"><span data-stu-id="fc109-1942">Telemetry</span></span>

* <span data-ttu-id="fc109-1943">Verbesserte Berichterstellung für Telemetriedaten</span><span class="sxs-lookup"><span data-stu-id="fc109-1943">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="fc109-1944">ACR</span><span class="sxs-lookup"><span data-stu-id="fc109-1944">ACR</span></span>

* <span data-ttu-id="fc109-1945">Befehle vom Typ `content-trust policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1945">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="fc109-1946">Problem behoben, aufgrund dessen `.dockerignore` nicht richtig verarbeitet wurde</span><span class="sxs-lookup"><span data-stu-id="fc109-1946">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="fc109-1947">ACS</span><span class="sxs-lookup"><span data-stu-id="fc109-1947">ACS</span></span>

* <span data-ttu-id="fc109-1948">`az acs/aks install-cli` für die Installation in `%USERPROFILE%\.azure-kubectl` unter Windows geändert</span><span class="sxs-lookup"><span data-stu-id="fc109-1948">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="fc109-1949">`az aks install-connector` geändert, um zu ermitteln, ob der Cluster über RBAC verfügt, und um den ACI-Connector entsprechend zu konfigurieren</span><span class="sxs-lookup"><span data-stu-id="fc109-1949">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="fc109-1950">Geändert in Rollenzuweisung zum Subnetz bei entsprechender Angabe</span><span class="sxs-lookup"><span data-stu-id="fc109-1950">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="fc109-1951">Neue Option zum Überspringen der Rollenzuweisung für Subnetz hinzugefügt, wenn dieses angegeben ist</span><span class="sxs-lookup"><span data-stu-id="fc109-1951">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="fc109-1952">Geändert, um Rollenzuweisung zum Subnetz zu überspringen, wenn bereits eine Zuweisung vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="fc109-1952">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="fc109-1953">AppService</span><span class="sxs-lookup"><span data-stu-id="fc109-1953">AppService</span></span>

* <span data-ttu-id="fc109-1954">Fehler behoben, der das Erstellen einer Funktions-App mithilfe von Speicherkonten in externen Ressourcengruppen verhinderte</span><span class="sxs-lookup"><span data-stu-id="fc109-1954">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="fc109-1955">Absturz bei ZIP-Bereitstellung behoben</span><span class="sxs-lookup"><span data-stu-id="fc109-1955">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="fc109-1956">Batch AI</span><span class="sxs-lookup"><span data-stu-id="fc109-1956">BatchAI</span></span>

* <span data-ttu-id="fc109-1957">Protokollierungsausgabe für die automatische Speicherkontoerstellung geändert, sodass nun „Ressourcen*gruppe*“ angegeben wird</span><span class="sxs-lookup"><span data-stu-id="fc109-1957">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="fc109-1958">Container</span><span class="sxs-lookup"><span data-stu-id="fc109-1958">Container</span></span>

* <span data-ttu-id="fc109-1959">`--secure-environment-variables` zum Übergeben sicherer Umgebungsvariablen an einen Container hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1959">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="fc109-1960">IoT</span><span class="sxs-lookup"><span data-stu-id="fc109-1960">IoT</span></span>

* <span data-ttu-id="fc109-1961">[BREAKING CHANGE] Veraltete Befehle entfernt, die in die IoT-Erweiterung verschoben wurden</span><span class="sxs-lookup"><span data-stu-id="fc109-1961">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="fc109-1962">Elemente aktualisiert, um nicht die Domäne `azure-devices.net` anzunehmen</span><span class="sxs-lookup"><span data-stu-id="fc109-1962">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="fc109-1963">Iot Central</span><span class="sxs-lookup"><span data-stu-id="fc109-1963">Iot Central</span></span>

* <span data-ttu-id="fc109-1964">Erstes Release des IoT Central-Moduls</span><span class="sxs-lookup"><span data-stu-id="fc109-1964">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="fc109-1965">KeyVault</span><span class="sxs-lookup"><span data-stu-id="fc109-1965">KeyVault</span></span>


* <span data-ttu-id="fc109-1966">Befehle zum Verwalten von Speicherkonten und SAS-Definitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1966">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="fc109-1967">Befehle für Netzwerkregeln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1967">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="fc109-1968">Parameter `--id` zu Geheimnis-, Schlüssel- und Zertifikatvorgängen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1968">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="fc109-1969">Unterstützung für Version mit mehreren APIs zur Schlüsseltresorverwaltung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1969">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="fc109-1970">Unterstützung für Version mit mehreren APIs zur Schlüsseltresordatenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1970">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="fc109-1971">Relay</span><span class="sxs-lookup"><span data-stu-id="fc109-1971">Relay</span></span>

* <span data-ttu-id="fc109-1972">Erste Veröffentlichung</span><span class="sxs-lookup"><span data-stu-id="fc109-1972">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="fc109-1973">Sql</span><span class="sxs-lookup"><span data-stu-id="fc109-1973">Sql</span></span>

* <span data-ttu-id="fc109-1974">Befehle vom Typ `sql failover-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1974">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="fc109-1975">Storage</span><span class="sxs-lookup"><span data-stu-id="fc109-1975">Storage</span></span>

* <span data-ttu-id="fc109-1976">[BREAKING CHANGE]`storage account show-usage` geändert, um Parameter `--location` erforderlich zu machen. Auflistung nach Region</span><span class="sxs-lookup"><span data-stu-id="fc109-1976">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="fc109-1977">Parameter `--resource-group` geändert, sodass er für `storage account`-Befehle optional ist</span><span class="sxs-lookup"><span data-stu-id="fc109-1977">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="fc109-1978">Warnungen vom Typ „Fehler bei Vorbedingung“ für einzelne Fehler in Batch-Befehlen für eine aggregiert Nachricht entfernt</span><span class="sxs-lookup"><span data-stu-id="fc109-1978">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="fc109-1979">`[blob|file] delete-batch`-Befehle geändert, sodass kein Array mit Null-Werten mehr ausgegeben wird</span><span class="sxs-lookup"><span data-stu-id="fc109-1979">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="fc109-1980">`blob [download|upload|delete-batch]`-Befehle geändert, um SAS-Token aus Container-URL zu lesen</span><span class="sxs-lookup"><span data-stu-id="fc109-1980">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="fc109-1981">VM</span><span class="sxs-lookup"><span data-stu-id="fc109-1981">VM</span></span>

* <span data-ttu-id="fc109-1982">Allgemeine Filter zu `vm list-skus` für höhere Benutzerfreundlichkeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1982">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="fc109-1983">31. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="fc109-1983">July 31, 2018</span></span>

<span data-ttu-id="fc109-1984">Version 2.0.43</span><span class="sxs-lookup"><span data-stu-id="fc109-1984">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="fc109-1985">ACR</span><span class="sxs-lookup"><span data-stu-id="fc109-1985">ACR</span></span>

* <span data-ttu-id="fc109-1986">Flag `--with-secure-properties` zum Befehl `acr build-task show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1986">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="fc109-1987">Befehl `acr build-task update-build` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1987">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="fc109-1988">ACS</span><span class="sxs-lookup"><span data-stu-id="fc109-1988">ACS</span></span>

* <span data-ttu-id="fc109-1989">Änderung, um 0 (Erfolg) zurückzugeben, wenn `az aks browse` durch Drücken von [STRG+C] beendet wird</span><span class="sxs-lookup"><span data-stu-id="fc109-1989">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="fc109-1990">Batch</span><span class="sxs-lookup"><span data-stu-id="fc109-1990">Batch</span></span>

* <span data-ttu-id="fc109-1991">Korrektur eines Fehlers bei der Anzeige des AAD-Tokens in Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="fc109-1991">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="fc109-1992">Container</span><span class="sxs-lookup"><span data-stu-id="fc109-1992">Container</span></span>

* <span data-ttu-id="fc109-1993">Voraussetzung von `--log-analytics-workspace-key` für Name oder ID im festgelegten Abonnement entfernt</span><span class="sxs-lookup"><span data-stu-id="fc109-1993">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="fc109-1994">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="fc109-1994">Network</span></span>

* <span data-ttu-id="fc109-1995">DNS-Unterstützung zu „2017-03-09-profile“ für Azure Stack hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-1995">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="fc109-1996">Resource</span><span class="sxs-lookup"><span data-stu-id="fc109-1996">Resource</span></span>

* <span data-ttu-id="fc109-1997">`--rollback-on-error` zu `group deployment create` hinzugefügt, um bei einem Fehler eine als funktionierend bekannte Bereitstellung auszuführen</span><span class="sxs-lookup"><span data-stu-id="fc109-1997">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="fc109-1998">Problem behoben, aufgrund dessen `--parameters {}` mit `group deployment create` zu einem Fehler führte</span><span class="sxs-lookup"><span data-stu-id="fc109-1998">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="fc109-1999">Role</span><span class="sxs-lookup"><span data-stu-id="fc109-1999">Role</span></span>

* <span data-ttu-id="fc109-2000">Unterstützung für das Stack-Profil „2017-03-09-profile“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2000">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="fc109-2001">Problem behoben, aufgrund dessen das generische Update von Parametern auf `app update` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="fc109-2001">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="fc109-2002">Suchen,</span><span class="sxs-lookup"><span data-stu-id="fc109-2002">Search</span></span>

* <span data-ttu-id="fc109-2003">Befehle für Azure Search-Dienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2003">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="fc109-2004">Service Bus</span><span class="sxs-lookup"><span data-stu-id="fc109-2004">Service Bus</span></span>

* <span data-ttu-id="fc109-2005">Migrationsbefehlsgruppe hinzugefügt, um einen Namespace von Service Bus Standard zu Premium zu migrieren</span><span class="sxs-lookup"><span data-stu-id="fc109-2005">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="fc109-2006">Neue optionale Eigenschaften zu Service Bus-Warteschlange und -Abonnement hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2006">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="fc109-2007">`--enable-batched-operations` und `--enable-dead-lettering-on-message-expiration` in `queue`</span><span class="sxs-lookup"><span data-stu-id="fc109-2007">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="fc109-2008">`--dead-letter-on-filter-exceptions` in `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="fc109-2008">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="fc109-2009">Storage</span><span class="sxs-lookup"><span data-stu-id="fc109-2009">Storage</span></span>

* <span data-ttu-id="fc109-2010">Unterstützung für den Download großer Dateien über eine einzelne Verbindung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2010">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="fc109-2011">`show`-Befehle konvertiert, bei denen im Falle einer fehlenden Ressource kein Fehler mit dem Exitcode 3 ausgelöst wurde</span><span class="sxs-lookup"><span data-stu-id="fc109-2011">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="fc109-2012">VM</span><span class="sxs-lookup"><span data-stu-id="fc109-2012">VM</span></span>

* <span data-ttu-id="fc109-2013">Unterstützung zum Auflisten von Verfügbarkeitsgruppen nach Abonnement hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2013">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="fc109-2014">Unterstützung für `StandardSSD_LRS` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-2014">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="fc109-2015">Unterstützung für Anwendungssicherheitsgruppe beim Erstellen einer VM-Skalierungsgruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2015">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="fc109-2016">[BREAKING CHANGE]`[vm|vmss] create`, `[vm|vmss] identity assign` und `[vm|vmss] identity remove` wurden geändert, um vom Benutzer zugewiesene Identitäten im Wörterbuchformat auszugeben.</span><span class="sxs-lookup"><span data-stu-id="fc109-2016">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="fc109-2017">18. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="fc109-2017">July 18, 2018</span></span>

<span data-ttu-id="fc109-2018">Version 2.0.42</span><span class="sxs-lookup"><span data-stu-id="fc109-2018">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="fc109-2019">Core</span><span class="sxs-lookup"><span data-stu-id="fc109-2019">Core</span></span>

* <span data-ttu-id="fc109-2020">Unterstützung für browserbasierte Anmeldung WSL-Bash-Fenster hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2020">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="fc109-2021">`--force-string`-Flag für alle generischen Updatebefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2021">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="fc109-2022">[BREAKING CHANGE] Befehle vom Typ „show“ so geändert, dass die Fehlermeldung protokolliert wird und der Vorgang bei einer fehlenden Ressource mit dem Exitcode 3 fehlschlägt</span><span class="sxs-lookup"><span data-stu-id="fc109-2022">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="fc109-2023">ACR</span><span class="sxs-lookup"><span data-stu-id="fc109-2023">ACR</span></span>

* <span data-ttu-id="fc109-2024">[BREAKING CHANGE] „--no-push“ in Befehl „acr build“ in reines Flag geändert</span><span class="sxs-lookup"><span data-stu-id="fc109-2024">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="fc109-2025">Befehle `show` und `update` unter Gruppe `acr repository` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2025">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="fc109-2026">`--detail`-Flag für `show-manifests` und `show-tags` hinzugefügt, um ausführlichere Informationen anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="fc109-2026">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="fc109-2027">Parameter `--image` zur Unterstützung des Abrufs von Builddetails oder Protokollen anhand eines Images hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2027">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="fc109-2028">ACS</span><span class="sxs-lookup"><span data-stu-id="fc109-2028">ACS</span></span>

* <span data-ttu-id="fc109-2029">`az aks create` so geändert, dass mit Fehler beendet wird, wenn `--max-pods` kleiner als 5 ist</span><span class="sxs-lookup"><span data-stu-id="fc109-2029">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="fc109-2030">AppService</span><span class="sxs-lookup"><span data-stu-id="fc109-2030">AppService</span></span>

* <span data-ttu-id="fc109-2031">Unterstützung für PremiumV2-SKUs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2031">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="fc109-2032">Batch</span><span class="sxs-lookup"><span data-stu-id="fc109-2032">Batch</span></span>

* <span data-ttu-id="fc109-2033">Korrektur eines Fehlers bei der Verwendung von Anmeldeinformationen im Cloud Shell-Modus</span><span class="sxs-lookup"><span data-stu-id="fc109-2033">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="fc109-2034">JSON-Eingabe so geändert, dass Groß-/Kleinschreibung nicht beachtet wird</span><span class="sxs-lookup"><span data-stu-id="fc109-2034">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="fc109-2035">Batch KI</span><span class="sxs-lookup"><span data-stu-id="fc109-2035">Batch AI</span></span>

* <span data-ttu-id="fc109-2036">Befehl `az batchai job exec` korrigiert</span><span class="sxs-lookup"><span data-stu-id="fc109-2036">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="fc109-2037">Container</span><span class="sxs-lookup"><span data-stu-id="fc109-2037">Container</span></span>

* <span data-ttu-id="fc109-2038">Anforderung von Benutzername und Kennwort für Nicht-DockerHub-Registrierungen entfernt</span><span class="sxs-lookup"><span data-stu-id="fc109-2038">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="fc109-2039">Fehler beim Erstellen von Containergruppen aus YAML-Datei behoben</span><span class="sxs-lookup"><span data-stu-id="fc109-2039">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="fc109-2040">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="fc109-2040">Network</span></span>

* <span data-ttu-id="fc109-2041">Unterstützung für `--no-wait` zu `network nic [create|update|delete]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2041">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="fc109-2042">`network nic wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2042">Added `network nic wait`</span></span>
* <span data-ttu-id="fc109-2043">`--ids`-Argument für `network vnet [subnet|peering] list` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="fc109-2043">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="fc109-2044">`--include-default`-Flag hinzugefügt, um Standardsicherheitsregeln in die Ausgabe von `network nsg rule list` aufzunehmen</span><span class="sxs-lookup"><span data-stu-id="fc109-2044">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="fc109-2045">Resource</span><span class="sxs-lookup"><span data-stu-id="fc109-2045">Resource</span></span>

* <span data-ttu-id="fc109-2046">Unterstützung für `--no-wait` zu `group deployment delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2046">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="fc109-2047">Unterstützung für `--no-wait` zu `deployment delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2047">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="fc109-2048">Befehl `deployment wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2048">Added `deployment wait` command</span></span>
* <span data-ttu-id="fc109-2049">Problem behoben, aufgrund dessen die `az deployment`-Befehle auf Abonnementebene fälschlicherweise für Profil „2017-03-09-profile“ angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="fc109-2049">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="fc109-2050">SQL</span><span class="sxs-lookup"><span data-stu-id="fc109-2050">SQL</span></span>

* <span data-ttu-id="fc109-2051">Fehler „Der angegebene Ressourcengruppenname ... entsprach nicht dem Namen in der URL“ beim Angeben des Namens des Pools für elastische Datenbanken für `sql db copy`-und `sql db replica create`-Befehle behoben</span><span class="sxs-lookup"><span data-stu-id="fc109-2051">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="fc109-2052">Konfigurieren des Standard-SQL Servers durch Ausführen von `az configure --defaults sql-server=<name>` zulässig</span><span class="sxs-lookup"><span data-stu-id="fc109-2052">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="fc109-2053">Tabellenformatierer für Befehle `sql server`, `sql server firewall-rule`, `sql list-usages` und `sql show-usage` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2053">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="fc109-2054">Storage</span><span class="sxs-lookup"><span data-stu-id="fc109-2054">Storage</span></span>

* <span data-ttu-id="fc109-2055">`pageRanges`-Eigenschaft zu `storage blob show`-Ausgabe hinzugefügt, die für Seitenblobs ausgefüllt wird</span><span class="sxs-lookup"><span data-stu-id="fc109-2055">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="fc109-2056">VM</span><span class="sxs-lookup"><span data-stu-id="fc109-2056">VM</span></span>

* <span data-ttu-id="fc109-2057">[BREAKING CHANGE]`vmss create` so geändert, dass `Standard_DS1_v2` als standardmäßige Instanzgröße verwendet wird</span><span class="sxs-lookup"><span data-stu-id="fc109-2057">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="fc109-2058">Unterstützung für `--no-wait` zu `vm extension [set|delete]` und `vmss extension [set|delete]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2058">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="fc109-2059">`vm extension wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2059">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="fc109-2060">3\. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="fc109-2060">July 3, 2018</span></span>

<span data-ttu-id="fc109-2061">Version 2.0.41</span><span class="sxs-lookup"><span data-stu-id="fc109-2061">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="fc109-2062">AKS</span><span class="sxs-lookup"><span data-stu-id="fc109-2062">AKS</span></span>

* <span data-ttu-id="fc109-2063">Überwachung geändert, sodass Abonnement-ID verwendet wird</span><span class="sxs-lookup"><span data-stu-id="fc109-2063">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="fc109-2064">3\. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="fc109-2064">July 3, 2018</span></span>

<span data-ttu-id="fc109-2065">Version 2.0.40</span><span class="sxs-lookup"><span data-stu-id="fc109-2065">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="fc109-2066">Core</span><span class="sxs-lookup"><span data-stu-id="fc109-2066">Core</span></span>

* <span data-ttu-id="fc109-2067">Neuer Autorisierungscode-Flow für interaktive Anmeldung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2067">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="fc109-2068">ACR</span><span class="sxs-lookup"><span data-stu-id="fc109-2068">ACR</span></span>

* <span data-ttu-id="fc109-2069">Abruf-Buildstatus hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2069">Added polling build status</span></span>
* <span data-ttu-id="fc109-2070">Unterstützung für Enumerationswerte ohne Berücksichtigung von Groß-/Kleinschreibung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2070">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="fc109-2071">Parameter `--top` und `--orderby` für `show-manifests` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2071">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="fc109-2072">ACS</span><span class="sxs-lookup"><span data-stu-id="fc109-2072">ACS</span></span>

* <span data-ttu-id="fc109-2073">[BREAKING CHANGE] Standardmäßiges Aktivieren der rollenbasierten Zugriffssteuerung für Kubernetes</span><span class="sxs-lookup"><span data-stu-id="fc109-2073">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="fc109-2074">Argument `--disable-rbac` hinzugefügt und `--enable-rbac` als veraltet festgelegt, da es nun der Standard ist</span><span class="sxs-lookup"><span data-stu-id="fc109-2074">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="fc109-2075">Optionen für Befehl `aks browse` wurden aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="fc109-2075">Updated options for `aks browse` command.</span></span> <span data-ttu-id="fc109-2076">Unterstützung für `--listen-port` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2076">Added `--listen-port` support</span></span>
* <span data-ttu-id="fc109-2077">Standardmäßiges Helm-Diagrammpaket für Befehl `aks install-connector` wurde aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="fc109-2077">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="fc109-2078">Verwenden von „virtual-kubelet-for-aks-latest.tgz“</span><span class="sxs-lookup"><span data-stu-id="fc109-2078">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="fc109-2079">Befehle `aks enable-addons` und `aks disable-addons` zum Aktualisieren eines vorhandenen Clusters hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2079">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="fc109-2080">AppService</span><span class="sxs-lookup"><span data-stu-id="fc109-2080">AppService</span></span>

* <span data-ttu-id="fc109-2081">Unterstützung für das Deaktivieren der Identität über `webapp identity remove` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2081">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="fc109-2082">`preview`-Tag für Identitätsfunktion entfernt</span><span class="sxs-lookup"><span data-stu-id="fc109-2082">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="fc109-2083">Backup</span><span class="sxs-lookup"><span data-stu-id="fc109-2083">Backup</span></span>

* <span data-ttu-id="fc109-2084">Moduldefinition aktualisiert</span><span class="sxs-lookup"><span data-stu-id="fc109-2084">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="fc109-2085">Batch AI</span><span class="sxs-lookup"><span data-stu-id="fc109-2085">BatchAI</span></span>

* <span data-ttu-id="fc109-2086">Tabellenausgabe für Befehle `batchai cluster node list` und `batchai job node list` korrigiert</span><span class="sxs-lookup"><span data-stu-id="fc109-2086">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="fc109-2087">Cloud</span><span class="sxs-lookup"><span data-stu-id="fc109-2087">Cloud</span></span>

* <span data-ttu-id="fc109-2088">Serversuffix `acr login` zu Cloudkonfiguration hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2088">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="fc109-2089">Container</span><span class="sxs-lookup"><span data-stu-id="fc109-2089">Container</span></span>

* <span data-ttu-id="fc109-2090">`container create` zu Standard für Vorgang mit langer Ausführungsdauer geändert</span><span class="sxs-lookup"><span data-stu-id="fc109-2090">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="fc109-2091">Log Analytics-Parameter `--log-analytics-workspace` und `--log-analytics-workspace-key` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2091">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="fc109-2092">Parameter `--protocol` zum Festlegen des zu verwendenden Netzwerkprotokolls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2092">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="fc109-2093">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="fc109-2093">Extension</span></span>

* <span data-ttu-id="fc109-2094">`extension list-available` geändert, sodass nur mit der CLI-Version kompatible Erweiterungen angezeigt werden</span><span class="sxs-lookup"><span data-stu-id="fc109-2094">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="fc109-2095">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="fc109-2095">Network</span></span>

* <span data-ttu-id="fc109-2096">Problem behoben, aufgrund dessen bei Datensatztypen die Groß-/Kleinschreibung beachtet werden musste ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="fc109-2096">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="fc109-2097">Rdbms</span><span class="sxs-lookup"><span data-stu-id="fc109-2097">Rdbms</span></span>

* <span data-ttu-id="fc109-2098">Befehle vom Typ `[postgres|myql] server vnet-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2098">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="fc109-2099">Resource</span><span class="sxs-lookup"><span data-stu-id="fc109-2099">Resource</span></span>

* <span data-ttu-id="fc109-2100">Neue Vorgangsgruppe `deployment` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2100">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="fc109-2101">VM</span><span class="sxs-lookup"><span data-stu-id="fc109-2101">VM</span></span>

* <span data-ttu-id="fc109-2102">Unterstützung für das Entfernen der vom System zugewiesenen Identität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2102">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="fc109-2103">25. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="fc109-2103">June 25, 2018</span></span>

<span data-ttu-id="fc109-2104">Version 2.0.39</span><span class="sxs-lookup"><span data-stu-id="fc109-2104">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="fc109-2105">Befehlszeilenschnittstelle (CLI)</span><span class="sxs-lookup"><span data-stu-id="fc109-2105">CLI</span></span>

* <span data-ttu-id="fc109-2106">Dateieinschränkung in MSI-Installer aktualisiert, um Problem mit der Erweiterungsinstallation zu beheben</span><span class="sxs-lookup"><span data-stu-id="fc109-2106">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="fc109-2107">19. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="fc109-2107">June 19, 2018</span></span>

<span data-ttu-id="fc109-2108">Version 2.0.38</span><span class="sxs-lookup"><span data-stu-id="fc109-2108">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="fc109-2109">Core</span><span class="sxs-lookup"><span data-stu-id="fc109-2109">Core</span></span>

* <span data-ttu-id="fc109-2110">Globale Unterstützung für `--subscription` zu den meisten Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2110">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="fc109-2111">ACR</span><span class="sxs-lookup"><span data-stu-id="fc109-2111">ACR</span></span>

* <span data-ttu-id="fc109-2112">`azure-storage-blob` als Abhängigkeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2112">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="fc109-2113">CPU-Standardkonfiguration für `acr build-task create` geändert, sodass zwei Kerne verwendet werden</span><span class="sxs-lookup"><span data-stu-id="fc109-2113">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="fc109-2114">ACS</span><span class="sxs-lookup"><span data-stu-id="fc109-2114">ACS</span></span>

* <span data-ttu-id="fc109-2115">Optionen des Befehls `aks use-dev-spaces` wurden aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="fc109-2115">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="fc109-2116">Unterstützung für `--update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2116">Added `--update` support</span></span>
* <span data-ttu-id="fc109-2117">`aks get-credentials --admin` geändert, sodass der Benutzerkontext in `$HOME/.kube/config` ersetzt wird</span><span class="sxs-lookup"><span data-stu-id="fc109-2117">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="fc109-2118">Schreibgeschützte `nodeResourceGroup`-Eigenschaft in verwalteten Clustern verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="fc109-2118">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="fc109-2119">Befehlsfehler `acs browse` korrigiert</span><span class="sxs-lookup"><span data-stu-id="fc109-2119">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="fc109-2120">`--connector-name` für `aks install-connector`, `aks upgrade-connector` und `aks remove-connector` als optional festgelegt</span><span class="sxs-lookup"><span data-stu-id="fc109-2120">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="fc109-2121">Neue Azure Container Instances-Regionen für `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2121">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="fc109-2122">Normalisierter Speicherort im Helm-Versionsnamen und Knotenname zu `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2122">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="fc109-2123">AppService</span><span class="sxs-lookup"><span data-stu-id="fc109-2123">AppService</span></span>

* <span data-ttu-id="fc109-2124">Unterstützung für neuere Versionen von „urllib“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2124">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="fc109-2125">Unterstützung der Verwendung eines App Service-Plans aus externen Ressourcengruppen zu `functionapp create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2125">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="fc109-2126">Batch</span><span class="sxs-lookup"><span data-stu-id="fc109-2126">Batch</span></span>

* <span data-ttu-id="fc109-2127">`azure-batch-extensions`-Abhängigkeit entfernt</span><span class="sxs-lookup"><span data-stu-id="fc109-2127">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="fc109-2128">Batch KI</span><span class="sxs-lookup"><span data-stu-id="fc109-2128">Batch AI</span></span>

* <span data-ttu-id="fc109-2129">Unterstützung für Arbeitsbereiche wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-2129">Added support for workspaces.</span></span> <span data-ttu-id="fc109-2130">Arbeitsbereiche ermöglichen das Zusammenfassen von Clustern, Dateiservern und Experimenten in Gruppen ohne Beschränkung der Anzahl von Ressourcen, die erstellt werden können.</span><span class="sxs-lookup"><span data-stu-id="fc109-2130">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="fc109-2131">Unterstützung für Experimente wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-2131">Added support for experiments.</span></span> <span data-ttu-id="fc109-2132">Experimente ermöglichen das Zusammenfassen von Aufträgen in Sammlungen ohne Beschränkung der Anzahl von erstellten Aufträgen.</span><span class="sxs-lookup"><span data-stu-id="fc109-2132">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="fc109-2133">Unterstützung für das Konfigurieren von `/dev/shm` für Aufträge hinzugefügt, die in einem Docker-Container ausgeführt werden</span><span class="sxs-lookup"><span data-stu-id="fc109-2133">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="fc109-2134">Die Befehle `batchai cluster node exec` und `batchai job node exec` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-2134">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="fc109-2135">Diese Befehle ermöglichen die Ausführung aller Befehle direkt auf Knoten und bieten Funktionen zur Portweiterleitung.</span><span class="sxs-lookup"><span data-stu-id="fc109-2135">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="fc109-2136">Unterstützung für `--ids` zu `batchai`-Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2136">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="fc109-2137">[BREAKING CHANGE] Alle Cluster und Dateiserver müssen unter Arbeitsbereichen erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="fc109-2137">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="fc109-2138">[BREAKING CHANGE] Aufträge müssen unter Experimenten erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="fc109-2138">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="fc109-2139">[BREAKING CHANGE]`--nfs-resource-group` wurde aus den Befehlen `cluster create` und `job create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="fc109-2139">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="fc109-2140">Geben Sie zum Bereitstellen eines NFS, das einem anderen Arbeitsbereich/einer anderen Ressourcengruppe angehört, die ARM-ID des Dateiservers über die Option `--nfs` an.</span><span class="sxs-lookup"><span data-stu-id="fc109-2140">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="fc109-2141">[BREAKING CHANGE]`--cluster-resource-group` wurde aus dem Befehl `job create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="fc109-2141">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="fc109-2142">Geben Sie zum Übermitteln eines Auftrags, der einem anderen Arbeitsbereich/einer anderen Ressourcengruppe angehört, die ARM-ID des Clusters über die Option `--cluster` an.</span><span class="sxs-lookup"><span data-stu-id="fc109-2142">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="fc109-2143">[BREAKING CHANGE] Attribut `location` wurde aus Aufträgen, Clustern und Dateiservern entfernt.</span><span class="sxs-lookup"><span data-stu-id="fc109-2143">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="fc109-2144">„Location“ ist jetzt ein Attribut eines Arbeitsbereichs.</span><span class="sxs-lookup"><span data-stu-id="fc109-2144">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="fc109-2145">[BREAKING CHANGE]`--location` wurde aus den Befehlen `job create`, `cluster create` und `file-server create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="fc109-2145">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="fc109-2146">[BREAKING CHANGE] Namen von Kurzoptionen wurden geändert, um die Schnittstelle konsistenter zu machen:</span><span class="sxs-lookup"><span data-stu-id="fc109-2146">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="fc109-2147">[`--config`, `-c`] in [`--config-file`, `-f`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="fc109-2147">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="fc109-2148">[`--cluster`, `-r`] in [`--cluster`, `-c`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="fc109-2148">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="fc109-2149">[`--cluster`, `-n`] in [`--cluster`, `-c`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="fc109-2149">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="fc109-2150">[`--job`, `-n`] in [`--job`, `-j`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="fc109-2150">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="fc109-2151">Karten</span><span class="sxs-lookup"><span data-stu-id="fc109-2151">Maps</span></span>

* <span data-ttu-id="fc109-2152">[BREAKING CHANGE]`maps account create` wurde so geändert, dass Nutzungsbedingungen entweder durch interaktive Eingabeaufforderung oder `--accept-tos`-Flag akzeptiert werden müssen.</span><span class="sxs-lookup"><span data-stu-id="fc109-2152">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="fc109-2153">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="fc109-2153">Network</span></span>

* <span data-ttu-id="fc109-2154">Unterstützung für `https` zu `network lb probe create` hinzugefügt [Nr. 6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="fc109-2154">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="fc109-2155">Problem behoben, aufgrund dessen die Groß-/Kleinschreibung von `--endpoint-status` berücksichtigt wurde.</span><span class="sxs-lookup"><span data-stu-id="fc109-2155">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="fc109-2156">#6502</span><span class="sxs-lookup"><span data-stu-id="fc109-2156">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="fc109-2157">Reservations</span><span class="sxs-lookup"><span data-stu-id="fc109-2157">Reservations</span></span>

* <span data-ttu-id="fc109-2158">[BREAKING CHANGE] Erforderlicher Parameter `ReservedResourceType` zu `reservations catalog show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2158">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="fc109-2159">Parameter `Location` zu `reservations catalog show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2159">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="fc109-2160">[BREAKING CHANGE]`kind` aus `ReservationProperties` entfernt</span><span class="sxs-lookup"><span data-stu-id="fc109-2160">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="fc109-2161">[BREAKING CHANGE]`capabilities` wurde in `Catalog` in `sku_properties` umbenannt</span><span class="sxs-lookup"><span data-stu-id="fc109-2161">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="fc109-2162">[BREAKING CHANGE] Eigenschaften `size` und `tier` aus `Catalog` entfernt</span><span class="sxs-lookup"><span data-stu-id="fc109-2162">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="fc109-2163">Parameter `InstanceFlexibility` zu `reservations reservation update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2163">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="fc109-2164">Role</span><span class="sxs-lookup"><span data-stu-id="fc109-2164">Role</span></span>

* <span data-ttu-id="fc109-2165">Fehlerbehandlung verbessert</span><span class="sxs-lookup"><span data-stu-id="fc109-2165">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="fc109-2166">SQL</span><span class="sxs-lookup"><span data-stu-id="fc109-2166">SQL</span></span>

* <span data-ttu-id="fc109-2167">Verwirrender Fehler behoben, der beim Ausführen von `az sql db list-editions` für einen Ort auftrat, der für Ihr Abonnement nicht verfügbar ist</span><span class="sxs-lookup"><span data-stu-id="fc109-2167">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="fc109-2168">Storage</span><span class="sxs-lookup"><span data-stu-id="fc109-2168">Storage</span></span>

* <span data-ttu-id="fc109-2169">Lesbarkeit der Tabellenausgabe für `storage blob download` verbessert</span><span class="sxs-lookup"><span data-stu-id="fc109-2169">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="fc109-2170">VM</span><span class="sxs-lookup"><span data-stu-id="fc109-2170">VM</span></span>

* <span data-ttu-id="fc109-2171">Verbesserte Einschränkung der VM-Größenüberprüfung für Unterstützung von beschleunigten Netzwerken in `vm create`</span><span class="sxs-lookup"><span data-stu-id="fc109-2171">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="fc109-2172">Warnung für `vmss create` hinzugefügt, dass die VM-Standardgröße von `Standard_D1_v2` auf `Standard_DS1_v2` umgestellt wird</span><span class="sxs-lookup"><span data-stu-id="fc109-2172">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="fc109-2173">`--force-update` zu `[vm|vmss] extension set` hinzugefügt, um die Erweiterung auch dann zu aktualisieren, wenn die Konfiguration nicht geändert wurde</span><span class="sxs-lookup"><span data-stu-id="fc109-2173">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="fc109-2174">13. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="fc109-2174">June 13, 2018</span></span>

<span data-ttu-id="fc109-2175">Version 2.0.37</span><span class="sxs-lookup"><span data-stu-id="fc109-2175">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="fc109-2176">Core</span><span class="sxs-lookup"><span data-stu-id="fc109-2176">Core</span></span>

* <span data-ttu-id="fc109-2177">Verbesserte interaktive Telemetrie</span><span class="sxs-lookup"><span data-stu-id="fc109-2177">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="fc109-2178">13. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="fc109-2178">June 13, 2018</span></span>

<span data-ttu-id="fc109-2179">Version 2.0.36</span><span class="sxs-lookup"><span data-stu-id="fc109-2179">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="fc109-2180">AKS</span><span class="sxs-lookup"><span data-stu-id="fc109-2180">AKS</span></span>

* <span data-ttu-id="fc109-2181">Zusätzliche erweiterte Netzwerkoptionen zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2181">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="fc109-2182">Argumente zu `aks create` zum Aktivieren der Überwachung und HTTP-Routing hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2182">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="fc109-2183">Argument `--no-ssh-key` zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2183">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="fc109-2184">Argument `--enable-rbac` zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2184">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="fc109-2185">[VORSCHAUVERSION] Unterstützung für Azure Active Directory-Authentifizierung zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2185">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="fc109-2186">AppService</span><span class="sxs-lookup"><span data-stu-id="fc109-2186">AppService</span></span>

* <span data-ttu-id="fc109-2187">Problem mit inkompatiblen urllib-Versionen behoben</span><span class="sxs-lookup"><span data-stu-id="fc109-2187">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="fc109-2188">5\. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="fc109-2188">June 5, 2018</span></span>

<span data-ttu-id="fc109-2189">Version 2.0.35</span><span class="sxs-lookup"><span data-stu-id="fc109-2189">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="fc109-2190">Interactive</span><span class="sxs-lookup"><span data-stu-id="fc109-2190">Interactive</span></span>

* <span data-ttu-id="fc109-2191">Grenzwerte für die Abhängigkeiten des interaktiven Modus hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2191">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="fc109-2192">5\. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="fc109-2192">June 5, 2018</span></span>

<span data-ttu-id="fc109-2193">Version 2.0.34</span><span class="sxs-lookup"><span data-stu-id="fc109-2193">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="fc109-2194">Core</span><span class="sxs-lookup"><span data-stu-id="fc109-2194">Core</span></span>

* <span data-ttu-id="fc109-2195">Unterstützung für mandantenübergreifende Ressourcenverweise hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2195">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="fc109-2196">Verbesserte Zuverlässigkeit bei Telemetrieuploads</span><span class="sxs-lookup"><span data-stu-id="fc109-2196">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="fc109-2197">ACR</span><span class="sxs-lookup"><span data-stu-id="fc109-2197">ACR</span></span>

* <span data-ttu-id="fc109-2198">Unterstützung für VSTS als Remotequellort hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2198">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="fc109-2199">Befehl `acr import` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2199">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="fc109-2200">AKS</span><span class="sxs-lookup"><span data-stu-id="fc109-2200">AKS</span></span>

* <span data-ttu-id="fc109-2201">`aks get-credentials` wurde geändert, um die Kube-Konfigurationsdatei mit sichereren Dateisystemberechtigungen zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="fc109-2201">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="fc109-2202">Batch</span><span class="sxs-lookup"><span data-stu-id="fc109-2202">Batch</span></span>

* <span data-ttu-id="fc109-2203">Fehler bei der Formatierung der Poollistentabelle behoben [[Problem 4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="fc109-2203">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="fc109-2204">IoT</span><span class="sxs-lookup"><span data-stu-id="fc109-2204">IOT</span></span>

* <span data-ttu-id="fc109-2205">Unterstützung für das Erstellen von IoT Hub-Instanzen im Tarif „Basic“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2205">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="fc109-2206">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="fc109-2206">Network</span></span>

* <span data-ttu-id="fc109-2207">`network vnet peering` wurde verbessert.</span><span class="sxs-lookup"><span data-stu-id="fc109-2207">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="fc109-2208">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="fc109-2208">Policy Insights</span></span>

* <span data-ttu-id="fc109-2209">Erstrelease</span><span class="sxs-lookup"><span data-stu-id="fc109-2209">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="fc109-2210">ARM</span><span class="sxs-lookup"><span data-stu-id="fc109-2210">ARM</span></span>

* <span data-ttu-id="fc109-2211">Befehle vom Typ `account management-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2211">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="fc109-2212">SQL</span><span class="sxs-lookup"><span data-stu-id="fc109-2212">SQL</span></span>

* <span data-ttu-id="fc109-2213">Neue Befehle für verwaltete Instanzen hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="fc109-2213">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="fc109-2214">Neue Befehle für verwaltete Datenbanken hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="fc109-2214">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="fc109-2215">Storage</span><span class="sxs-lookup"><span data-stu-id="fc109-2215">Storage</span></span>

* <span data-ttu-id="fc109-2216">Zusätzliche MimeTypes für JSON und JavaScript hinzugefügt (abzuleiten aus Dateierweiterungen)</span><span class="sxs-lookup"><span data-stu-id="fc109-2216">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="fc109-2217">VM</span><span class="sxs-lookup"><span data-stu-id="fc109-2217">VM</span></span>

* <span data-ttu-id="fc109-2218">`vm list-skus` wurde geändert, um feste Spalten zu verwenden und eine Warnung hinzuzufügen, dass `Tier` und `Size` entfernt werden.</span><span class="sxs-lookup"><span data-stu-id="fc109-2218">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="fc109-2219">Option `--accelerated-networking` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2219">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="fc109-2220">`--tags` zu `identity create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2220">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="fc109-2221">22. Mai 2018</span><span class="sxs-lookup"><span data-stu-id="fc109-2221">May 22, 2018</span></span>

<span data-ttu-id="fc109-2222">Version 2.0.33</span><span class="sxs-lookup"><span data-stu-id="fc109-2222">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="fc109-2223">Core</span><span class="sxs-lookup"><span data-stu-id="fc109-2223">Core</span></span>

* <span data-ttu-id="fc109-2224">Unterstützung für das Erweitern von `@` in Dateinamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2224">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="fc109-2225">ACS</span><span class="sxs-lookup"><span data-stu-id="fc109-2225">ACS</span></span>

* <span data-ttu-id="fc109-2226">Neue Dev Spaces-Befehle `aks use-dev-spaces` und `aks remove-dev-spaces` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2226">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="fc109-2227">Tippfehler in Hilfemeldung korrigiert</span><span class="sxs-lookup"><span data-stu-id="fc109-2227">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="fc109-2228">AppService</span><span class="sxs-lookup"><span data-stu-id="fc109-2228">AppService</span></span>

* <span data-ttu-id="fc109-2229">Verbesserte generische Aktualisierungsbefehle</span><span class="sxs-lookup"><span data-stu-id="fc109-2229">Improved generic update commands</span></span>
* <span data-ttu-id="fc109-2230">Asynchrone Unterstützung für `webapp deployment source config-zip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2230">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="fc109-2231">Container</span><span class="sxs-lookup"><span data-stu-id="fc109-2231">Container</span></span>

* <span data-ttu-id="fc109-2232">Unterstützung für das Exportieren einer Containergruppe im YAML-Format hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2232">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="fc109-2233">Unterstützung für die Verwendung einer YAML-Datei zum Erstellen/Aktualisieren einer Containergruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2233">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="fc109-2234">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="fc109-2234">Extension</span></span>

* <span data-ttu-id="fc109-2235">Verbesserte Entfernung von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="fc109-2235">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="fc109-2236">Interactive</span><span class="sxs-lookup"><span data-stu-id="fc109-2236">Interactive</span></span>

* <span data-ttu-id="fc109-2237">Protokollierung geändert, um Parser für Abschlüsse zu deaktivieren</span><span class="sxs-lookup"><span data-stu-id="fc109-2237">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="fc109-2238">Verbesserte Verarbeitung beschädigter Hilfscaches</span><span class="sxs-lookup"><span data-stu-id="fc109-2238">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="fc109-2239">KeyVault</span><span class="sxs-lookup"><span data-stu-id="fc109-2239">KeyVault</span></span>

* <span data-ttu-id="fc109-2240">keyvault-Befehle wurden korrigiert, damit sie in Cloud Shell oder auf virtuellen Computern mit Identität verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="fc109-2240">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="fc109-2241">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="fc109-2241">Network</span></span>

* <span data-ttu-id="fc109-2242">Problem behoben, aufgrund dessen `network watcher show-topology` nicht mit einem VNET und/oder Subnetznamen verwendet werden konnte ([#6326](https://github.com/Azure/azure-cli/issues/6326))</span><span class="sxs-lookup"><span data-stu-id="fc109-2242">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="fc109-2243">Problem behoben, aufgrund dessen einige `network watcher`-Befehle fälschlicherweise angaben, dass Network Watcher nicht für bestimmte Regionen aktiviert ist ([#6264](https://github.com/Azure/azure-cli/issues/6264))</span><span class="sxs-lookup"><span data-stu-id="fc109-2243">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="fc109-2244">SQL</span><span class="sxs-lookup"><span data-stu-id="fc109-2244">SQL</span></span>

* <span data-ttu-id="fc109-2245">[BREAKING CHANGE] Von den Befehlen `db` und `dw` zurückgegebene Antwortobjekte geändert:</span><span class="sxs-lookup"><span data-stu-id="fc109-2245">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="fc109-2246">Eigenschaft `serviceLevelObjective` in `currentServiceObjectiveName` umbenannt</span><span class="sxs-lookup"><span data-stu-id="fc109-2246">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="fc109-2247">Eigenschaften `currentServiceObjectiveId` und `requestedServiceObjectiveId` entfernt</span><span class="sxs-lookup"><span data-stu-id="fc109-2247">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="fc109-2248">Eigenschaft `maxSizeBytes` geändert (ist nun keine Zeichenfolge mehr, sondern ein Ganzzahlwert)</span><span class="sxs-lookup"><span data-stu-id="fc109-2248">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="fc109-2249">[BREAKING CHANGE] Die folgenden `db`- und `dw`-Eigenschaften wurden geändert und sind jetzt schreibgeschützt:</span><span class="sxs-lookup"><span data-stu-id="fc109-2249">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="fc109-2250">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="fc109-2250">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="fc109-2251">Verwenden Sie zum Aktualisieren den Parameter `--service-objective`, oder legen Sie die Eigenschaft `sku.name` fest.</span><span class="sxs-lookup"><span data-stu-id="fc109-2251">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="fc109-2252">`edition`.</span><span class="sxs-lookup"><span data-stu-id="fc109-2252">`edition`.</span></span> <span data-ttu-id="fc109-2253">Verwenden Sie zum Aktualisieren den Parameter `--edition`, oder legen Sie die Eigenschaft `sku.tier` fest.</span><span class="sxs-lookup"><span data-stu-id="fc109-2253">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="fc109-2254">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="fc109-2254">`elasticPoolName`.</span></span> <span data-ttu-id="fc109-2255">Verwenden Sie zum Aktualisieren den Parameter `--elastic-pool`, oder legen Sie die Eigenschaft `elasticPoolId` fest.</span><span class="sxs-lookup"><span data-stu-id="fc109-2255">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="fc109-2256">[BREAKING CHANGE] Die folgenden `elastic-pool`-Eigenschaften wurden geändert und sind jetzt schreibgeschützt:</span><span class="sxs-lookup"><span data-stu-id="fc109-2256">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="fc109-2257">`edition`.</span><span class="sxs-lookup"><span data-stu-id="fc109-2257">`edition`.</span></span> <span data-ttu-id="fc109-2258">Verwenden Sie zum Aktualisieren den Parameter `--edition`.</span><span class="sxs-lookup"><span data-stu-id="fc109-2258">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="fc109-2259">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="fc109-2259">`dtu`.</span></span> <span data-ttu-id="fc109-2260">Verwenden Sie zum Aktualisieren den Parameter `--capacity`.</span><span class="sxs-lookup"><span data-stu-id="fc109-2260">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="fc109-2261">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="fc109-2261">`databaseDtuMin`.</span></span> <span data-ttu-id="fc109-2262">Verwenden Sie zum Aktualisieren den Parameter `--db-min-capacity`.</span><span class="sxs-lookup"><span data-stu-id="fc109-2262">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="fc109-2263">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="fc109-2263">`databaseDtuMax`.</span></span> <span data-ttu-id="fc109-2264">Verwenden Sie zum Aktualisieren den Parameter `--db-max-capacity`.</span><span class="sxs-lookup"><span data-stu-id="fc109-2264">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="fc109-2265">Die Parameter `--family` und `--capacity` wurden zu den `db`-, `dw`- und `elastic-pool`-Befehlen hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-2265">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="fc109-2266">Den `db`-, `dw`- und `elastic-pool`-Befehlen wurden Tabellenformatierer hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-2266">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="fc109-2267">Storage</span><span class="sxs-lookup"><span data-stu-id="fc109-2267">Storage</span></span>

* <span data-ttu-id="fc109-2268">Vervollständigung für das Argument `--account-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2268">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="fc109-2269">Problem mit `storage entity query` behoben</span><span class="sxs-lookup"><span data-stu-id="fc109-2269">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="fc109-2270">VM</span><span class="sxs-lookup"><span data-stu-id="fc109-2270">VM</span></span>

* <span data-ttu-id="fc109-2271">[BREAKING CHANGE]`--write-accelerator` aus `vm create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="fc109-2271">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="fc109-2272">Die gleiche Unterstützung kann über `vm update` oder `vm disk attach` erzielt werden.</span><span class="sxs-lookup"><span data-stu-id="fc109-2272">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="fc109-2273">Erweiterungsimageabgleich in `[vm|vmss] extension` korrigiert</span><span class="sxs-lookup"><span data-stu-id="fc109-2273">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="fc109-2274">`--boot-diagnostics-storage` zu `vm create` zur Erfassung des Startprotokolls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2274">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="fc109-2275">`--license-type` zu `[vm|vmss] update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2275">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="fc109-2276">7\. Mai 2018</span><span class="sxs-lookup"><span data-stu-id="fc109-2276">May 7, 2018</span></span>

<span data-ttu-id="fc109-2277">Version 2.0.32</span><span class="sxs-lookup"><span data-stu-id="fc109-2277">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="fc109-2278">Core</span><span class="sxs-lookup"><span data-stu-id="fc109-2278">Core</span></span>

* <span data-ttu-id="fc109-2279">Ein Ausnahmefehler wurde behoben, der beim Abrufen von Geheimnissen aus einem Dienstprinzipalkonto mit Zertifikat auftrat.</span><span class="sxs-lookup"><span data-stu-id="fc109-2279">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="fc109-2280">Eingeschränkte Unterstützung für positionelle Argumente hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2280">Added limited support for positional arguments</span></span>
* <span data-ttu-id="fc109-2281">Problem behoben, aufgrund dessen `--query` nicht mit `--ids` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="fc109-2281">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="fc109-2282">#5591</span><span class="sxs-lookup"><span data-stu-id="fc109-2282">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="fc109-2283">Pipingszenarien von Befehlen bei Verwendung von `--ids` verbessert</span><span class="sxs-lookup"><span data-stu-id="fc109-2283">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="fc109-2284">Unterstützt `-o tsv` mit angegebener Abfrage bzw. `-o json` ohne angegeben Abfrage</span><span class="sxs-lookup"><span data-stu-id="fc109-2284">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="fc109-2285">Befehlsvorschläge bei Fehler hinzugefügt, wenn Befehle Tippfehler enthielten</span><span class="sxs-lookup"><span data-stu-id="fc109-2285">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="fc109-2286">Fehler bei der Eingabe von `az ''` behandelt</span><span class="sxs-lookup"><span data-stu-id="fc109-2286">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="fc109-2287">Unterstützung für benutzerdefinierte Ressourcentypen für Befehlsmodule und -erweiterungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2287">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="fc109-2288">ACR</span><span class="sxs-lookup"><span data-stu-id="fc109-2288">ACR</span></span>

* <span data-ttu-id="fc109-2289">ACR Build-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2289">Added ACR Build commands</span></span>
* <span data-ttu-id="fc109-2290">Fehlermeldungen vom Typ „Ressource nicht gefunden.“ verbessert</span><span class="sxs-lookup"><span data-stu-id="fc109-2290">Improved resource not found error messages</span></span>
* <span data-ttu-id="fc109-2291">Höhere Leistung bei der Ressourcenerstellung und optimierte Fehlerbehandlung</span><span class="sxs-lookup"><span data-stu-id="fc109-2291">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="fc109-2292">ACR-Anmeldung bei nicht standardmäßigen Konsolen und WSL optimiert</span><span class="sxs-lookup"><span data-stu-id="fc109-2292">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="fc109-2293">Fehlermeldungen zu Repositorybefehlen optimiert</span><span class="sxs-lookup"><span data-stu-id="fc109-2293">Improved repository commands error messages</span></span>
* <span data-ttu-id="fc109-2294">Tabellenspalten und -reihenfolge aktualisiert</span><span class="sxs-lookup"><span data-stu-id="fc109-2294">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="fc109-2295">ACS</span><span class="sxs-lookup"><span data-stu-id="fc109-2295">ACS</span></span>

* <span data-ttu-id="fc109-2296">Warnung hinzugefügt, dass `az aks` eine Vorschauversion des Diensts ist</span><span class="sxs-lookup"><span data-stu-id="fc109-2296">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="fc109-2297">Berechtigungsproblem in `aks install-connector` behoben, wenn `--aci-resource-group` nicht angegeben wird</span><span class="sxs-lookup"><span data-stu-id="fc109-2297">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="fc109-2298">AMS</span><span class="sxs-lookup"><span data-stu-id="fc109-2298">AMS</span></span>

* <span data-ttu-id="fc109-2299">Erste Version: Verwalten von Azure Media Services-Ressourcen</span><span class="sxs-lookup"><span data-stu-id="fc109-2299">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="fc109-2300">AppService</span><span class="sxs-lookup"><span data-stu-id="fc109-2300">Appservice</span></span>

* <span data-ttu-id="fc109-2301">Ein Problem in `webapp delete` wurde behoben, das bei Angabe von `--slot` auftrat.</span><span class="sxs-lookup"><span data-stu-id="fc109-2301">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="fc109-2302">`--runtime-version` aus `webapp auth update` entfernt</span><span class="sxs-lookup"><span data-stu-id="fc109-2302">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="fc109-2303">Unterstützung für „min\_tls\_version“ und „https2.0“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2303">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="fc109-2304">Unterstützung für mehrere Container hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2304">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="fc109-2305">Batch KI</span><span class="sxs-lookup"><span data-stu-id="fc109-2305">Batch AI</span></span>

* <span data-ttu-id="fc109-2306">`batchai create cluster` wurde geändert, um die in der Konfigurationsdatei des Clusters konfigurierte VM-Priorität zu berücksichtigen.</span><span class="sxs-lookup"><span data-stu-id="fc109-2306">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="fc109-2307">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="fc109-2307">Cognitive Services</span></span>

* <span data-ttu-id="fc109-2308">Tippfehler im Beispiel für `cognitiveservices account create` behoben [Nr. 5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="fc109-2308">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="fc109-2309">Nutzung</span><span class="sxs-lookup"><span data-stu-id="fc109-2309">Consumption</span></span>

* <span data-ttu-id="fc109-2310">Neue Befehle für Budget-API hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2310">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="fc109-2311">Container</span><span class="sxs-lookup"><span data-stu-id="fc109-2311">Container</span></span>

* <span data-ttu-id="fc109-2312">`--registry-server` muss nicht mehr für `container create` angegeben werden, wenn ein Registrierungsserver im Imagenamen enthalten ist.</span><span class="sxs-lookup"><span data-stu-id="fc109-2312">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="fc109-2313">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="fc109-2313">Cosmos DB</span></span>

* <span data-ttu-id="fc109-2314">VNET-Unterstützung für Azure CLI eingeführt: Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="fc109-2314">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="fc109-2315">DMS</span><span class="sxs-lookup"><span data-stu-id="fc109-2315">DMS</span></span>

* <span data-ttu-id="fc109-2316">Erste Version: Die Migration von SQL zu Azure SQL wird nun unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fc109-2316">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="fc109-2317">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="fc109-2317">Extension</span></span>

* <span data-ttu-id="fc109-2318">Fehler behoben, aufgrund dessen Erweiterungsmetadaten nicht mehr angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="fc109-2318">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="fc109-2319">Interactive</span><span class="sxs-lookup"><span data-stu-id="fc109-2319">Interactive</span></span>

* <span data-ttu-id="fc109-2320">Interaktive Vervollständigung funktioniert nun auch mit positionellen Argumenten.</span><span class="sxs-lookup"><span data-stu-id="fc109-2320">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="fc109-2321">Benutzerfreundlichere Ausgabe bei der Eingabe von '\'</span><span class="sxs-lookup"><span data-stu-id="fc109-2321">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="fc109-2322">Abschlüsse für Parameter ohne Hilfe korrigiert</span><span class="sxs-lookup"><span data-stu-id="fc109-2322">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="fc109-2323">Beschreibungen für Befehlsgruppen korrigiert</span><span class="sxs-lookup"><span data-stu-id="fc109-2323">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="fc109-2324">Labor</span><span class="sxs-lookup"><span data-stu-id="fc109-2324">Lab</span></span>

* <span data-ttu-id="fc109-2325">Regressionen aus Knack-Umwandlung korrigiert</span><span class="sxs-lookup"><span data-stu-id="fc109-2325">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="fc109-2326">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="fc109-2326">Network</span></span>

* <span data-ttu-id="fc109-2327">[BREAKING CHANGE] Parameter `--ids` entfernt für:</span><span class="sxs-lookup"><span data-stu-id="fc109-2327">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="fc109-2328">Profil</span><span class="sxs-lookup"><span data-stu-id="fc109-2328">Profile</span></span>

* <span data-ttu-id="fc109-2329">Quellerkennung für `disk create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="fc109-2329">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="fc109-2330">[BREAKING CHANGE]`--msi-port` und `--identity-port` entfernt, da sie nicht mehr verwendet werden</span><span class="sxs-lookup"><span data-stu-id="fc109-2330">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="fc109-2331">Tippfehler in kurzer Zusammenfassung für `account get-access-token` korrigiert</span><span class="sxs-lookup"><span data-stu-id="fc109-2331">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="fc109-2332">Redis</span><span class="sxs-lookup"><span data-stu-id="fc109-2332">Redis</span></span>

* <span data-ttu-id="fc109-2333">`redis patch-schedule patch-schedule show` wurde durch `redis patch-schedule show` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="fc109-2333">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="fc109-2334">`redis list-all` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="fc109-2334">Deprecated `redis list-all`.</span></span> <span data-ttu-id="fc109-2335">Diese Funktion wurde in `redis list` integriert.</span><span class="sxs-lookup"><span data-stu-id="fc109-2335">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="fc109-2336">`redis import-method` wurde durch `redis import` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="fc109-2336">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="fc109-2337">Unterstützung für `--ids` zu verschiedenen Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2337">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="fc109-2338">Role</span><span class="sxs-lookup"><span data-stu-id="fc109-2338">Role</span></span>

* <span data-ttu-id="fc109-2339">[BREAKING CHANGE] Veralteter Befehl `ad sp reset-credentials` entfernt</span><span class="sxs-lookup"><span data-stu-id="fc109-2339">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="fc109-2340">Storage</span><span class="sxs-lookup"><span data-stu-id="fc109-2340">Storage</span></span>

* <span data-ttu-id="fc109-2341">Zulassen, dass das Ziel-SAS-Token für die Blobkopie auf die Quelle angewendet wird, wenn Quell-SAS und Kontoschlüssel nicht angegeben werden</span><span class="sxs-lookup"><span data-stu-id="fc109-2341">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="fc109-2342">Verfügbar gemacht: Socket-Timeout für Blobuploads und -downloads</span><span class="sxs-lookup"><span data-stu-id="fc109-2342">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="fc109-2343">Blobnamen, die mit Pfadtrennzeichen beginnen, als relative Pfade behandeln</span><span class="sxs-lookup"><span data-stu-id="fc109-2343">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="fc109-2344">Zulassen, dass `storage blob copy --source-sas` mit dem Abfragezeichen „?“ beginnt</span><span class="sxs-lookup"><span data-stu-id="fc109-2344">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="fc109-2345">`storage entity query --marker` korrigiert, um Liste von Schlüsselwerten zu akzeptieren</span><span class="sxs-lookup"><span data-stu-id="fc109-2345">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="fc109-2346">VM</span><span class="sxs-lookup"><span data-stu-id="fc109-2346">VM</span></span>

* <span data-ttu-id="fc109-2347">Ungültige Erkennungslogik für nicht verwalteten Blob-URI korrigiert</span><span class="sxs-lookup"><span data-stu-id="fc109-2347">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="fc109-2348">Unterstützung für Datenträgerverschlüsselung ohne vom Benutzer bereitgestellte Dienstprinzipale hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2348">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="fc109-2349">[BREAKING CHANGE] Verwenden Sie nicht „ManagedIdentityExtension“ des virtuellen Computers für MSI-Unterstützung.</span><span class="sxs-lookup"><span data-stu-id="fc109-2349">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="fc109-2350">Unterstützung für Entfernungsrichtlinie zu `vmss` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2350">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="fc109-2351">[BREAKING CHANGE]`--ids` entfernt aus:</span><span class="sxs-lookup"><span data-stu-id="fc109-2351">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="fc109-2352">Unterstützung für Schreibbeschleunigung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2352">Added write accelerator support</span></span>
* <span data-ttu-id="fc109-2353">`vmss perform-maintenance` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2353">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="fc109-2354">`vm diagnostics set` korrigiert, um zuverlässig den Betriebssystemtyp des virtuellen Computers zu erkennen</span><span class="sxs-lookup"><span data-stu-id="fc109-2354">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="fc109-2355">`vm resize` geändert, um zu überprüfen, ob die angeforderte Größe von der derzeit festgelegten Größe abweicht, und nur bei einer Änderung eine Aktualisierung auszuführen</span><span class="sxs-lookup"><span data-stu-id="fc109-2355">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="fc109-2356">10. April 2018</span><span class="sxs-lookup"><span data-stu-id="fc109-2356">April 10, 2018</span></span>

<span data-ttu-id="fc109-2357">Version 2.0.31</span><span class="sxs-lookup"><span data-stu-id="fc109-2357">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="fc109-2358">ACR</span><span class="sxs-lookup"><span data-stu-id="fc109-2358">ACR</span></span>

* <span data-ttu-id="fc109-2359">Verbesserte Fehlerbehandlung für wincred-Fallback</span><span class="sxs-lookup"><span data-stu-id="fc109-2359">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="fc109-2360">ACS</span><span class="sxs-lookup"><span data-stu-id="fc109-2360">ACS</span></span>

* <span data-ttu-id="fc109-2361">Gültigkeit von per AKS erstellten SPNs in fünf Jahre geändert</span><span class="sxs-lookup"><span data-stu-id="fc109-2361">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="fc109-2362">AppService</span><span class="sxs-lookup"><span data-stu-id="fc109-2362">Appservice</span></span>

* [BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="fc109-2364">Nicht abgefangene Ausnahme für nicht vorhandene Web-App-Pläne behoben</span><span class="sxs-lookup"><span data-stu-id="fc109-2364">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="fc109-2365">Batch AI</span><span class="sxs-lookup"><span data-stu-id="fc109-2365">BatchAI</span></span>

* <span data-ttu-id="fc109-2366">Unterstützung für API 2018-03-01 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2366">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="fc109-2367">Bereitstellung auf Auftragsebene</span><span class="sxs-lookup"><span data-stu-id="fc109-2367">Job level mounting</span></span>
  - <span data-ttu-id="fc109-2368">Umgebungsvariablen mit Geheimniswerten</span><span class="sxs-lookup"><span data-stu-id="fc109-2368">Environment variables with secret values</span></span>
  - <span data-ttu-id="fc109-2369">Einstellungen von Leistungsindikatoren</span><span class="sxs-lookup"><span data-stu-id="fc109-2369">Performance counters settings</span></span>
  - <span data-ttu-id="fc109-2370">Berichtstellung für auftragsspezifisches Pfadsegment</span><span class="sxs-lookup"><span data-stu-id="fc109-2370">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="fc109-2371">Unterstützung für Unterordner in Listendateien-API</span><span class="sxs-lookup"><span data-stu-id="fc109-2371">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="fc109-2372">Berichterstellung zur Nutzung und zu Grenzwerten</span><span class="sxs-lookup"><span data-stu-id="fc109-2372">Usage and limits reporting</span></span>
  - <span data-ttu-id="fc109-2373">Zulassen der Angabe des Cachetyps für NFS-Server</span><span class="sxs-lookup"><span data-stu-id="fc109-2373">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="fc109-2374">Unterstützung für benutzerdefinierte Images</span><span class="sxs-lookup"><span data-stu-id="fc109-2374">Support for custom images</span></span>
  - <span data-ttu-id="fc109-2375">Unterstützung für pyTorch-Toolkit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2375">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="fc109-2376">Befehl `job wait` hinzugefügt, der das Warten auf die Auftragsfertigstellung ermöglicht und den Code für die Auftragsbeendigung meldet</span><span class="sxs-lookup"><span data-stu-id="fc109-2376">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="fc109-2377">Befehl `usage show` hinzugefügt, mit dem die aktuelle Nutzung von Batch KI-Ressourcen und die Grenzwerte für verschiedene Regionen aufgelistet werden</span><span class="sxs-lookup"><span data-stu-id="fc109-2377">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="fc109-2378">Nationale Clouds werden unterstützt</span><span class="sxs-lookup"><span data-stu-id="fc109-2378">National clouds are supported</span></span>
* <span data-ttu-id="fc109-2379">Befehlszeilenargumente für Aufträge hinzugefügt, um das Bereitstellen von Dateisystemen auf Auftragsebene zusätzlich zu Konfigurationsdateien zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="fc109-2379">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="fc109-2380">Weitere Optionen zum Anpassen von Clustern hinzugefügt – VM-Priorität, Subnetz, anfängliche Knotenanzahl für Cluster mit automatischer Skalierung, Angeben eines benutzerdefinierten Images</span><span class="sxs-lookup"><span data-stu-id="fc109-2380">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="fc109-2381">Befehlszeilenoption zum Angeben des Cachetyps für NFS mit Verwaltung per Batch KI hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2381">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="fc109-2382">Angeben der Bereitstellung von Dateisystemen in Konfigurationsdateien vereinfacht.</span><span class="sxs-lookup"><span data-stu-id="fc109-2382">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="fc109-2383">Weglassen von Anmeldeinformationen für Azure-Dateifreigaben und Azure-Blobcontainer ist jetzt möglich. Die CLI füllt fehlende Anmeldeinformationen auf, indem der Speicherkontoschlüssel verwendet wird, der über Befehlszeilenparameter oder per Umgebungsvariable angegeben wird, oder der Schlüssel wird über Azure Storage abgefragt (sofern das Speicherkonto zum aktuellen Abonnement gehört).</span><span class="sxs-lookup"><span data-stu-id="fc109-2383">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="fc109-2384">Der Befehl zum Streamen von Auftragsdateien wird jetzt automatisch abgeschlossen, nachdem der Auftrag beendet ist (Erfolg, Fehler, Beendigung oder Löschung)</span><span class="sxs-lookup"><span data-stu-id="fc109-2384">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="fc109-2385">Verbesserte `table`-Ausgabe für `show`-Vorgänge</span><span class="sxs-lookup"><span data-stu-id="fc109-2385">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="fc109-2386">Option `--use-auto-storage` für die Clustererstellung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-2386">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="fc109-2387">Diese Option erleichtert die Verwaltung von Speicherkonten und die Bereitstellung von Azure-Dateifreigaben und Azure-Blobcontainern in Clustern.</span><span class="sxs-lookup"><span data-stu-id="fc109-2387">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="fc109-2388">`--generate-ssh-keys` für `cluster create` und `file-server create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2388">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="fc109-2389">Möglichkeit zum Angeben der Knotensetupaufgabe über die Befehlszeile</span><span class="sxs-lookup"><span data-stu-id="fc109-2389">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="fc109-2390">[BREAKING CHANGE] Befehl `job stream-file` und `job list-files` in die Gruppe `job file` verschoben</span><span class="sxs-lookup"><span data-stu-id="fc109-2390">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="fc109-2391">[BREAKING CHANGE]`--admin-user-name` im Befehl `file-server create` in `--user-name` umbenannt, um Einheitlichkeit mit dem Befehl `cluster create` zu erzielen</span><span class="sxs-lookup"><span data-stu-id="fc109-2391">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="fc109-2392">Abrechnung</span><span class="sxs-lookup"><span data-stu-id="fc109-2392">Billing</span></span>

* <span data-ttu-id="fc109-2393">Registrierungskontobefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2393">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="fc109-2394">Nutzung</span><span class="sxs-lookup"><span data-stu-id="fc109-2394">Consumption</span></span>

* <span data-ttu-id="fc109-2395">Befehle vom Typ `marketplace` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2395">Added `marketplace` commands</span></span>
* <span data-ttu-id="fc109-2396">[BREAKING CHANGE]`reservations summaries` in `reservation summary` umbenannt</span><span class="sxs-lookup"><span data-stu-id="fc109-2396">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="fc109-2397">[BREAKING CHANGE]`reservations details` in `reservation detail` umbenannt</span><span class="sxs-lookup"><span data-stu-id="fc109-2397">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="fc109-2398">[BREAKING CHANGE] Kurzoptionen `--reservation-order-id` und `--reservation-id` für `reservation`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="fc109-2398">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="fc109-2399">[BREAKING CHANGE]`--grain`-Kurzoptionen für `reservation summary`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="fc109-2399">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="fc109-2400">[BREAKING CHANGE]`--include-meter-details`-Kurzoptionen für `pricesheet`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="fc109-2400">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="fc109-2401">Container</span><span class="sxs-lookup"><span data-stu-id="fc109-2401">Container</span></span>

* <span data-ttu-id="fc109-2402">Parameter für die Volumebereitstellung für das Git-Repository hinzugefügt: `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` und `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="fc109-2402">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="fc109-2403">[#5926](https://github.com/Azure/azure-cli/issues/5926) behoben: Fehler bei `az container exec`, wenn „--container-name“ angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="fc109-2403">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="fc109-2404">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="fc109-2404">Extension</span></span>

* <span data-ttu-id="fc109-2405">Meldung für Distributionsüberprüfung in Debugebene geändert</span><span class="sxs-lookup"><span data-stu-id="fc109-2405">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="fc109-2406">Interactive</span><span class="sxs-lookup"><span data-stu-id="fc109-2406">Interactive</span></span>

* <span data-ttu-id="fc109-2407">Geändert: Verhinderung des Abschlusses bei nicht erkannten Befehlen</span><span class="sxs-lookup"><span data-stu-id="fc109-2407">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="fc109-2408">Ereignishooks vor und nach der Erstellung der Teilstruktur von Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2408">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="fc109-2409">Abschluss für `--ids`-Parameter hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2409">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="fc109-2410">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="fc109-2410">Network</span></span>

* <span data-ttu-id="fc109-2411">[#5936](https://github.com/Azure/azure-cli/issues/5936) behoben: `application-gateway create`-Tags konnten nicht festgelegt werden</span><span class="sxs-lookup"><span data-stu-id="fc109-2411">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="fc109-2412">Argument `--auth-certs` zum Anfügen von Authentifizierungszertifikaten für `application-gateway http-settings [create|update]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-2412">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="fc109-2413">#4910</span><span class="sxs-lookup"><span data-stu-id="fc109-2413">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="fc109-2414">`ddos-protection`-Befehle zum Erstellen von DDoS-Schutzplänen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2414">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="fc109-2415">Unterstützung von `--ddos-protection-plan` für `vnet [create|update]` hinzugefügt, um das Zuordnen eines VNET zu einem DDoS-Schutzplan zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="fc109-2415">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="fc109-2416">Problem mit `--disable-bgp-route-propagation`-Flag in `network route-table [create|update]` behoben</span><span class="sxs-lookup"><span data-stu-id="fc109-2416">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="fc109-2417">Dummy-Argumente `--public-ip-address-type` und `--subnet-type` für `network lb [create|update]` entfernt</span><span class="sxs-lookup"><span data-stu-id="fc109-2417">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="fc109-2418">Unterstützung für TXT-Datensätze mit RFC 1035-Escapesequenzen für `network dns zone [import|export]` und `network dns record-set txt add-record` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2418">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="fc109-2419">Profil</span><span class="sxs-lookup"><span data-stu-id="fc109-2419">Profile</span></span>

* <span data-ttu-id="fc109-2420">Unterstützung für klassische Azure-Konten in `account list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2420">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="fc109-2421">[BREAKING CHANGE]`--msi` & `--msi-port`-Argumente entfernt</span><span class="sxs-lookup"><span data-stu-id="fc109-2421">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="fc109-2422">RDBMS</span><span class="sxs-lookup"><span data-stu-id="fc109-2422">RDBMS</span></span>

* <span data-ttu-id="fc109-2423">Befehl `georestore` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2423">Added `georestore` command</span></span>
* <span data-ttu-id="fc109-2424">Speichergrößenbeschränkung aus Befehl `create` entfernt</span><span class="sxs-lookup"><span data-stu-id="fc109-2424">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="fc109-2425">Resource</span><span class="sxs-lookup"><span data-stu-id="fc109-2425">Resource</span></span>

* <span data-ttu-id="fc109-2426">Unterstützung für `--metadata` zu `policy definition create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2426">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="fc109-2427">Unterstützung von `--metadata`, `--set`, `--add`, `--remove` für `policy definition update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2427">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="fc109-2428">SQL</span><span class="sxs-lookup"><span data-stu-id="fc109-2428">SQL</span></span>

* <span data-ttu-id="fc109-2429">`sql elastic-pool op list` und `sql elastic-pool op cancel` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2429">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="fc109-2430">Storage</span><span class="sxs-lookup"><span data-stu-id="fc109-2430">Storage</span></span>

* <span data-ttu-id="fc109-2431">Fehlermeldungen für falsch formatierte Verbindungszeichenfolgen verbessert</span><span class="sxs-lookup"><span data-stu-id="fc109-2431">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="fc109-2432">VM</span><span class="sxs-lookup"><span data-stu-id="fc109-2432">VM</span></span>

* <span data-ttu-id="fc109-2433">Unterstützung für die Konfiguration der Plattform-Fehlerdomänenanzahl für `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2433">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="fc109-2434">`vmss create` geändert, damit standardmäßig „Standard LB“ für zonales, großes oder per einzelner Platzierungsgruppe deaktiviertes Scale Set festgelegt wird</span><span class="sxs-lookup"><span data-stu-id="fc109-2434">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret`
* <span data-ttu-id="fc109-2436">Unterstützung für SKU mit öffentlicher IP für `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2436">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="fc109-2437">Argumente `--keyvault` und `--resource-group` für `vm secret format` hinzugefügt, um Szenarien zu unterstützen, bei denen der Befehl die Tresor-ID nicht auflösen kann.</span><span class="sxs-lookup"><span data-stu-id="fc109-2437">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="fc109-2438">#5718</span><span class="sxs-lookup"><span data-stu-id="fc109-2438">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="fc109-2439">Bessere Fehler für `[vm|vmss create]`, wenn der Standort einer Ressourcengruppe keine Zonenunterstützung aufweist</span><span class="sxs-lookup"><span data-stu-id="fc109-2439">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="fc109-2440">27. März 2018</span><span class="sxs-lookup"><span data-stu-id="fc109-2440">March 27, 2018</span></span>

<span data-ttu-id="fc109-2441">Version 2.0.30</span><span class="sxs-lookup"><span data-stu-id="fc109-2441">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="fc109-2442">Core</span><span class="sxs-lookup"><span data-stu-id="fc109-2442">Core</span></span>

* <span data-ttu-id="fc109-2443">Anzeigen einer Meldung für Erweiterungen, die in der Hilfe als Vorschauversion gekennzeichnet sind</span><span class="sxs-lookup"><span data-stu-id="fc109-2443">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="fc109-2444">ACS</span><span class="sxs-lookup"><span data-stu-id="fc109-2444">ACS</span></span>

* <span data-ttu-id="fc109-2445">Behebung eines Fehlers bei der SSL-Zertifikatprüfung für `aks install-cli` in Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="fc109-2445">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="fc109-2446">AppService</span><span class="sxs-lookup"><span data-stu-id="fc109-2446">Appservice</span></span>

* <span data-ttu-id="fc109-2447">Unterstützung nur von HTTPS zu `webapp update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2447">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="fc109-2448">Unterstützung für Slots zu `az webapp identity [assign|show]` und `az functionapp identity [assign|show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2448">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="fc109-2449">Backup</span><span class="sxs-lookup"><span data-stu-id="fc109-2449">Backup</span></span>

* <span data-ttu-id="fc109-2450">Neuer Befehl `az backup protection isenabled-for-vm` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-2450">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="fc109-2451">Mit diesem Befehl kann überprüft werden, ob ein virtueller Computer von einem beliebigen Tresor im Abonnement gesichert wird.</span><span class="sxs-lookup"><span data-stu-id="fc109-2451">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="fc109-2452">Azure-Objekt-IDs für Parameter `--resource-group` und `--vault-name` für die folgenden Befehle aktiviert:</span><span class="sxs-lookup"><span data-stu-id="fc109-2452">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="fc109-2453">`--name`-Parameter wurden geändert, um das Ausgabeformat von `backup ... show`-Befehlen zu akzeptieren.</span><span class="sxs-lookup"><span data-stu-id="fc109-2453">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="fc109-2454">Container</span><span class="sxs-lookup"><span data-stu-id="fc109-2454">Container</span></span>

* <span data-ttu-id="fc109-2455">Befehl `container exec` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-2455">Added `container exec` command.</span></span> <span data-ttu-id="fc109-2456">Ausführung von Befehlen in einem Container für eine ausgeführte Containergruppe</span><span class="sxs-lookup"><span data-stu-id="fc109-2456">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="fc109-2457">Zulassen der Tabellenausgabe zum Erstellen und Aktualisieren einer Containergruppe</span><span class="sxs-lookup"><span data-stu-id="fc109-2457">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="fc109-2458">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="fc109-2458">Extension</span></span>

* <span data-ttu-id="fc109-2459">Meldung für `extension add` hinzugefügt, wenn sich die Erweiterung in der Vorschauphase befindet</span><span class="sxs-lookup"><span data-stu-id="fc109-2459">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="fc109-2460">`extension list-available` geändert, um vollständige Erweiterungsdaten mit `--show-details` anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="fc109-2460">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="fc109-2461">[BREAKING CHANGE]`extension list-available` geändert, um standardmäßig vereinfachte Erweiterungsdaten anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="fc109-2461">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="fc109-2462">Interactive</span><span class="sxs-lookup"><span data-stu-id="fc109-2462">Interactive</span></span>

* <span data-ttu-id="fc109-2463">Vervollständigungen wurden geändert und werden jetzt aktiviert, sobald das Laden der Befehlstabelle abgeschlossen ist.</span><span class="sxs-lookup"><span data-stu-id="fc109-2463">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="fc109-2464">Fehler bei der Verwendung des Parameters `--style` behoben</span><span class="sxs-lookup"><span data-stu-id="fc109-2464">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="fc109-2465">Interaktiver Lexer nach Befehlstabellensicherung instanziiert (sofern nicht vorhanden)</span><span class="sxs-lookup"><span data-stu-id="fc109-2465">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="fc109-2466">Verbesserte Unterstützung der Vervollständigung</span><span class="sxs-lookup"><span data-stu-id="fc109-2466">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="fc109-2467">Labor</span><span class="sxs-lookup"><span data-stu-id="fc109-2467">Lab</span></span>

* <span data-ttu-id="fc109-2468">Probleme mit Befehl `create environment` behoben</span><span class="sxs-lookup"><span data-stu-id="fc109-2468">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="fc109-2469">Überwachen</span><span class="sxs-lookup"><span data-stu-id="fc109-2469">Monitor</span></span>

* <span data-ttu-id="fc109-2470">Unterstützung für `--top`, `--orderby` und `--namespace` zu `metrics list` hinzugefügt [Nr. 5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="fc109-2470">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="fc109-2471">[#4529](https://github.com/Azure/azure-cli/issues/5785) behoben: `metrics list` akzeptiert eine durch Leerzeichen getrennte Liste von abzurufenden Metriken</span><span class="sxs-lookup"><span data-stu-id="fc109-2471">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="fc109-2472">Unterstützung für `--namespace` zu `metrics list-definitions` hinzugefügt [Nr. 5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="fc109-2472">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="fc109-2473">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="fc109-2473">Network</span></span>

* <span data-ttu-id="fc109-2474">Unterstützung für private DNS-Zonen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2474">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="fc109-2475">Profil</span><span class="sxs-lookup"><span data-stu-id="fc109-2475">Profile</span></span>

* <span data-ttu-id="fc109-2476">Warnung für `--identity-port` und `--msi-port` zu `login` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2476">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="fc109-2477">RDBMS</span><span class="sxs-lookup"><span data-stu-id="fc109-2477">RDBMS</span></span>

* <span data-ttu-id="fc109-2478">GA-API-Version 2017-12-01 (Geschäftsmodell) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2478">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="fc109-2479">Resource</span><span class="sxs-lookup"><span data-stu-id="fc109-2479">Resource</span></span>

* [BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="fc109-2481">Role</span><span class="sxs-lookup"><span data-stu-id="fc109-2481">Role</span></span>

* <span data-ttu-id="fc109-2482">Unterstützung für erforderliche Zugriffskonfigurationen und native Clients zu `az ad app create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2482">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="fc109-2483">`rbac`-Befehle geändert, um maximal 1.000 IDs für Objektauflösung zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="fc109-2483">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="fc109-2484">Befehle zur Verwaltung von Anmeldeinformationen (`ad sp credential [reset|list|delete]`) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2484">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="fc109-2485">[BREAKING CHANGE] „properties“ aus `az role assignment [list|show]`-Ausgabe entfernt</span><span class="sxs-lookup"><span data-stu-id="fc109-2485">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="fc109-2486">Unterstützung für `dataActions`- und `notDataActions`-Berechtigungen zu `role definition` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2486">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="fc109-2487">Storage</span><span class="sxs-lookup"><span data-stu-id="fc109-2487">Storage</span></span>

* <span data-ttu-id="fc109-2488">Problem beim Hochladen von Dateien mit einer Größe von 195 GB bis 200 GB behoben</span><span class="sxs-lookup"><span data-stu-id="fc109-2488">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="fc109-2489">[#4049](https://github.com/Azure/azure-cli/issues/4049) behoben: Probleme bei Uploads von Anfügeblobs behoben, die ein Ignorieren der Bedingungsparameter verursacht haben</span><span class="sxs-lookup"><span data-stu-id="fc109-2489">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="fc109-2490">VM</span><span class="sxs-lookup"><span data-stu-id="fc109-2490">VM</span></span>

* <span data-ttu-id="fc109-2491">Warnung für anstehende BREAKING CHANGEen für Sätze mit mehr als 100 Instanzen zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2491">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="fc109-2492">Unterstützung der Zonenresilienz zu `vm [snapshot|image]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2492">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="fc109-2493">Datenträgerinstanzansicht geändert, um besseren Verschlüsselungsstatus zu melden</span><span class="sxs-lookup"><span data-stu-id="fc109-2493">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="fc109-2494">[BREAKING CHANGE]`vm extension delete` geändert, um keine Ausgabe mehr zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="fc109-2494">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="fc109-2495">13. März 2018</span><span class="sxs-lookup"><span data-stu-id="fc109-2495">March 13, 2018</span></span>

<span data-ttu-id="fc109-2496">Version 2.0.29</span><span class="sxs-lookup"><span data-stu-id="fc109-2496">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="fc109-2497">ACR</span><span class="sxs-lookup"><span data-stu-id="fc109-2497">ACR</span></span>

* <span data-ttu-id="fc109-2498">Unterstützung für den Parameter `--image` zu `repository delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2498">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="fc109-2499">Parameter `--manifest` und `--tag` des Befehls `repository delete` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="fc109-2499">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="fc109-2500">Befehl `repository untag` zum Entfernen eines Tags ohne das Löschen von Daten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2500">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="fc109-2501">ACS</span><span class="sxs-lookup"><span data-stu-id="fc109-2501">ACS</span></span>

* <span data-ttu-id="fc109-2502">Befehl `aks upgrade-connector` zum Aktualisieren eines vorhandenen Connectors hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2502">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="fc109-2503">`kubectl`-Konfigurationsdateien zur Verwendung von besser lesbarem YAML im Blockstil geändert</span><span class="sxs-lookup"><span data-stu-id="fc109-2503">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="fc109-2504">Advisor</span><span class="sxs-lookup"><span data-stu-id="fc109-2504">Advisor</span></span>

* <span data-ttu-id="fc109-2505">[BREAKING CHANGE]`advisor configuration get` in `advisor configuration list` umbenannt</span><span class="sxs-lookup"><span data-stu-id="fc109-2505">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="fc109-2506">[BREAKING CHANGE]`advisor configuration set` in `advisor configuration update` umbenannt</span><span class="sxs-lookup"><span data-stu-id="fc109-2506">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="fc109-2507">[BREAKING CHANGE]`advisor recommendation generate` entfernt</span><span class="sxs-lookup"><span data-stu-id="fc109-2507">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="fc109-2508">Parameter `--refresh` zu `advisor recommendation list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2508">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="fc109-2509">Befehl `advisor recommendation show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2509">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="fc109-2510">AppService</span><span class="sxs-lookup"><span data-stu-id="fc109-2510">Appservice</span></span>

* <span data-ttu-id="fc109-2511">`[webapp|functionapp] assign-identity` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="fc109-2511">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="fc109-2512">Befehle `webapp identity [assign|show]` und `functionapp identity [assign|show]` für verwaltete Identität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2512">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="fc109-2513">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="fc109-2513">Eventhubs</span></span>

* <span data-ttu-id="fc109-2514">Erste Veröffentlichung</span><span class="sxs-lookup"><span data-stu-id="fc109-2514">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="fc109-2515">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="fc109-2515">Extension</span></span>

* <span data-ttu-id="fc109-2516">Überprüfung zum Warnen von Benutzern hinzugefügt, wenn sich die verwendete Distribution von der in der Paketquelldatei gespeicherten Distribution unterscheidet, da dies Fehlern führen kann</span><span class="sxs-lookup"><span data-stu-id="fc109-2516">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="fc109-2517">Interactive</span><span class="sxs-lookup"><span data-stu-id="fc109-2517">Interactive</span></span>

* <span data-ttu-id="fc109-2518">[#5625](https://github.com/Azure/azure-cli/issues/5625) behoben: Verlauf über verschiedene Sitzungen hinweg beibehalten</span><span class="sxs-lookup"><span data-stu-id="fc109-2518">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="fc109-2519">[#3016](https://github.com/Azure/azure-cli/issues/3016) behoben: Verlauf nicht aufgezeichnet, obwohl er innerhalb des Bereichs liegt</span><span class="sxs-lookup"><span data-stu-id="fc109-2519">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="fc109-2520">[#5688](https://github.com/Azure/azure-cli/issues/5688) behoben: Abschlüsse wurden nicht angezeigt, wenn beim Laden der Befehlstabelle eine Ausnahme aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="fc109-2520">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="fc109-2521">Statusanzeige für lang ausgeführte Vorgänge korrigiert</span><span class="sxs-lookup"><span data-stu-id="fc109-2521">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="fc109-2522">Überwachen</span><span class="sxs-lookup"><span data-stu-id="fc109-2522">Monitor</span></span>

* <span data-ttu-id="fc109-2523">`monitor autoscale-settings`-Befehle als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="fc109-2523">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="fc109-2524">Befehle vom Typ `monitor autoscale` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2524">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="fc109-2525">Befehle vom Typ `monitor autoscale profile` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2525">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="fc109-2526">Befehle vom Typ `monitor autoscale rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2526">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="fc109-2527">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="fc109-2527">Network</span></span>

* <span data-ttu-id="fc109-2528">[BREAKING CHANGE] Parameter `--tags` aus `route-filter rule create` entfernt</span><span class="sxs-lookup"><span data-stu-id="fc109-2528">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="fc109-2529">Einige fehlerhafte Standardwerte für die folgenden Befehle entfernt:</span><span class="sxs-lookup"><span data-stu-id="fc109-2529">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="fc109-2530">`network watcher connection-monitor`-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2530">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="fc109-2531">Parameter `--vnet` und `--subnet` zu `network watcher show-topology` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2531">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="fc109-2532">Profil</span><span class="sxs-lookup"><span data-stu-id="fc109-2532">Profile</span></span>

* <span data-ttu-id="fc109-2533">Parameter `--msi` für `az login` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="fc109-2533">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="fc109-2534">Parameter `--identity` für `az login` als Ersatz vor `--msi` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2534">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="fc109-2535">RDBMS</span><span class="sxs-lookup"><span data-stu-id="fc109-2535">RDBMS</span></span>

* <span data-ttu-id="fc109-2536">[VORSCHAU] Geändert, sodass die API „2017-12-01-preview“ verwendet wird</span><span class="sxs-lookup"><span data-stu-id="fc109-2536">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="fc109-2537">Service Bus</span><span class="sxs-lookup"><span data-stu-id="fc109-2537">Service Bus</span></span>

* <span data-ttu-id="fc109-2538">Erste Veröffentlichung</span><span class="sxs-lookup"><span data-stu-id="fc109-2538">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="fc109-2539">Storage</span><span class="sxs-lookup"><span data-stu-id="fc109-2539">Storage</span></span>

* <span data-ttu-id="fc109-2540">[#4971](https://github.com/Azure/azure-cli/issues/4971) behoben: `storage blob copy` unterstützt jetzt andere Azure-Clouds.</span><span class="sxs-lookup"><span data-stu-id="fc109-2540">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="fc109-2541">[#5286](https://github.com/Azure/azure-cli/issues/5286) behoben: Batchbefehle `storage blob [delete-batch|download-batch|upload-batch]` lösen bei Vorbedingungsfehlern keinen Fehler mehr aus</span><span class="sxs-lookup"><span data-stu-id="fc109-2541">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="fc109-2542">VM</span><span class="sxs-lookup"><span data-stu-id="fc109-2542">VM</span></span>

* <span data-ttu-id="fc109-2543">`[vm|vmss] create` unterstützt jetzt das Anfügen nicht verwalteter Datenträger und das Konfigurieren der Zwischenspeicherung.</span><span class="sxs-lookup"><span data-stu-id="fc109-2543">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="fc109-2544">`[vm|vmss] assign-identity` und `[vm|vmss] remove-identity` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="fc109-2544">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="fc109-2545">Befehle `vm identity [assign|remove|show]` und `vmss identity [assign|remove|show]` als Ersatz für veraltete Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2545">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="fc109-2546">Standardpriorität in `vmss create` auf „Keine“ geändert</span><span class="sxs-lookup"><span data-stu-id="fc109-2546">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="fc109-2547">27. Februar 2018</span><span class="sxs-lookup"><span data-stu-id="fc109-2547">February 27, 2018</span></span>

<span data-ttu-id="fc109-2548">Version 2.0.28</span><span class="sxs-lookup"><span data-stu-id="fc109-2548">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="fc109-2549">Core</span><span class="sxs-lookup"><span data-stu-id="fc109-2549">Core</span></span>

* <span data-ttu-id="fc109-2550">[#5184](https://github.com/Azure/azure-cli/issues/5184) behoben: Problem beim Installieren von Homebrew</span><span class="sxs-lookup"><span data-stu-id="fc109-2550">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="fc109-2551">Unterstützung für Erweiterungstelemetrie mit benutzerdefinierten Schlüsseln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2551">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="fc109-2552">HTTP-Protokollierung zu `--debug` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2552">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="fc109-2553">ACS</span><span class="sxs-lookup"><span data-stu-id="fc109-2553">ACS</span></span>

* <span data-ttu-id="fc109-2554">Geändert, sodass für `aks install-connector` standardmäßig das Helm-Diagramm `virtual-kubelet-for-aks` verwendet wird</span><span class="sxs-lookup"><span data-stu-id="fc109-2554">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="fc109-2555">Problem behoben: Unzureichende Berechtigungen für Dienstprinzipale zum Erstellen einer ACI-Containergruppe</span><span class="sxs-lookup"><span data-stu-id="fc109-2555">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="fc109-2556">Parameter `--aci-container-group`, `--location` und `--image-tag` zu `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2556">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="fc109-2557">Veraltungshinweis aus `aks get-versions` entfernt</span><span class="sxs-lookup"><span data-stu-id="fc109-2557">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="fc109-2558">AppService</span><span class="sxs-lookup"><span data-stu-id="fc109-2558">Appservice</span></span>

* <span data-ttu-id="fc109-2559">Updates für die neue SDK-Version (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="fc109-2559">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="fc109-2560">[5538](https://github.com/Azure/azure-cli/issues/5538) behoben: `Free` wurde als ungültige SKU gemeldet.</span><span class="sxs-lookup"><span data-stu-id="fc109-2560">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="fc109-2561">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="fc109-2561">Cognitive Services</span></span>

* <span data-ttu-id="fc109-2562">Hinweis beim Erstellen eines neuen Cognitive Services-Kontos aktualisiert</span><span class="sxs-lookup"><span data-stu-id="fc109-2562">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="fc109-2563">Nutzung</span><span class="sxs-lookup"><span data-stu-id="fc109-2563">Consumption</span></span>

* <span data-ttu-id="fc109-2564">Neue Befehle für PriceSheet-API hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2564">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="fc109-2565">Vorhandene Formate für Nutzungsdetails und Reservierungsdetails aktualisiert</span><span class="sxs-lookup"><span data-stu-id="fc109-2565">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="fc109-2566">Container</span><span class="sxs-lookup"><span data-stu-id="fc109-2566">Container</span></span>

* <span data-ttu-id="fc109-2567">Argumente `--secrets` und `--secrets-mount-path` zu `container create` hinzugefügt, um Geheimnisse in ACI verwenden zu können</span><span class="sxs-lookup"><span data-stu-id="fc109-2567">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="fc109-2568">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="fc109-2568">Network</span></span>

* <span data-ttu-id="fc109-2569">[#5559](https://github.com/Azure/azure-cli/issues/5559) behoben: Fehlender Client in `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="fc109-2569">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="fc109-2570">Resource</span><span class="sxs-lookup"><span data-stu-id="fc109-2570">Resource</span></span>

* <span data-ttu-id="fc109-2571">`group deployment export` geändert, um eine partielle Vorlage und ggf. Fehler anzuzeigen, wenn der Vorgang nicht erfolgreich war</span><span class="sxs-lookup"><span data-stu-id="fc109-2571">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="fc109-2572">Role</span><span class="sxs-lookup"><span data-stu-id="fc109-2572">Role</span></span>

* <span data-ttu-id="fc109-2573">`role assignment list-changelogs` hinzugefügt, um die Überprüfung von Dienstprinzipalrollen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="fc109-2573">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="fc109-2574">SQL</span><span class="sxs-lookup"><span data-stu-id="fc109-2574">SQL</span></span>

* <span data-ttu-id="fc109-2575">Zonenredundanzunterstützung für Datenbanken und Pools für elastische Datenbanken hinzugefügt (bei Erstellung und Aktualisierung)</span><span class="sxs-lookup"><span data-stu-id="fc109-2575">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="fc109-2576">Storage</span><span class="sxs-lookup"><span data-stu-id="fc109-2576">Storage</span></span>

* <span data-ttu-id="fc109-2577">Angabe von Zielpfad/Präfix für `storage blob [upload-batch|download-batch]` ermöglicht</span><span class="sxs-lookup"><span data-stu-id="fc109-2577">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="fc109-2578">VM</span><span class="sxs-lookup"><span data-stu-id="fc109-2578">VM</span></span>

* <span data-ttu-id="fc109-2579">Unterstützung für das Anfügen/Trennen von Datenträgern für eine einzelne VMSS-Instanz hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2579">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="fc109-2580">13. Februar 2018</span><span class="sxs-lookup"><span data-stu-id="fc109-2580">February 13, 2018</span></span>

<span data-ttu-id="fc109-2581">Version 2.0.27</span><span class="sxs-lookup"><span data-stu-id="fc109-2581">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="fc109-2582">Core</span><span class="sxs-lookup"><span data-stu-id="fc109-2582">Core</span></span>

* <span data-ttu-id="fc109-2583">Authentifizierung für Abonnement-ID und Namen bei der MSI-Anmeldung in Authentifizierung mit Schlüssel geändert</span><span class="sxs-lookup"><span data-stu-id="fc109-2583">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="fc109-2584">ACS</span><span class="sxs-lookup"><span data-stu-id="fc109-2584">ACS</span></span>

* <span data-ttu-id="fc109-2585">[BREAKING CHANGE]`aks get-versions` aus Gründen der Genauigkeit in `aks get-upgrades` umbenannt</span><span class="sxs-lookup"><span data-stu-id="fc109-2585">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="fc109-2586">`aks get-versions` zur Anzeige der verfügbaren Kubernetes-Versionen für `aks create` geändert</span><span class="sxs-lookup"><span data-stu-id="fc109-2586">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="fc109-2587">Standardwerte von `aks create` in Auswahl der Kubernetes-Version durch den Server geändert</span><span class="sxs-lookup"><span data-stu-id="fc109-2587">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="fc109-2588">Hilfemeldungen zu dem von AKS generierten Dienstprinzipal aktualisiert</span><span class="sxs-lookup"><span data-stu-id="fc109-2588">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="fc109-2589">Standardknotengrößen für `aks create` von „Standard\_D1\_v2“ in „Standard\_DS1\_v2“ geändert</span><span class="sxs-lookup"><span data-stu-id="fc109-2589">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="fc109-2590">Zuverlässigkeit der Suche nach dem Dashboardpod für `az aks browse` verbessert</span><span class="sxs-lookup"><span data-stu-id="fc109-2590">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="fc109-2591">`aks get-credentials` korrigiert, um Unicode-Fehler beim Laden von Kubernetes-Konfigurationsdateien zu behandeln</span><span class="sxs-lookup"><span data-stu-id="fc109-2591">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="fc109-2592">Meldung zu `az aks install-cli` hinzugefügt, um das Abrufen von `kubectl` in `$PATH` zu erleichtern</span><span class="sxs-lookup"><span data-stu-id="fc109-2592">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="fc109-2593">AppService</span><span class="sxs-lookup"><span data-stu-id="fc109-2593">Appservice</span></span>

* <span data-ttu-id="fc109-2594">Problem behoben, das zu einem Fehler von `webapp [backup|restore]` aufgrund eines Nullverweises führte</span><span class="sxs-lookup"><span data-stu-id="fc109-2594">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="fc109-2595">Unterstützung für Standard-App Service-Pläne durch `az configure --defaults appserviceplan=my-asp` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2595">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="fc109-2596">CDN</span><span class="sxs-lookup"><span data-stu-id="fc109-2596">CDN</span></span>

* <span data-ttu-id="fc109-2597">Befehle vom Typ `cdn custom-domain [enable-https|disable-https]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2597">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="fc109-2598">Container</span><span class="sxs-lookup"><span data-stu-id="fc109-2598">Container</span></span>

* <span data-ttu-id="fc109-2599">Option `--follow` zu `az container logs` für Streamingprotokolle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2599">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="fc109-2600">Befehl `container attach` hinzugefügt, der die lokale Standardausgabe und Fehlerdatenströme an einen Container in einer Containergruppe angefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2600">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="fc109-2601">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="fc109-2601">CosmosDB</span></span>

* <span data-ttu-id="fc109-2602">Unterstützung für Einstellungsfunktionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2602">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="fc109-2603">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="fc109-2603">Extension</span></span>

* <span data-ttu-id="fc109-2604">Unterstützung für den Parameter `--pip-proxy` zu Befehlen vom Typ `az extension [add|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2604">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="fc109-2605">Unterstützung für das Argument `--pip-extra-index-urls` zu Befehlen vom Typ `az extension [add|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2605">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="fc109-2606">Feedback</span><span class="sxs-lookup"><span data-stu-id="fc109-2606">Feedback</span></span>

* <span data-ttu-id="fc109-2607">Erweiterungsinformationen zu Telemetriedaten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2607">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="fc109-2608">Interactive</span><span class="sxs-lookup"><span data-stu-id="fc109-2608">Interactive</span></span>

* <span data-ttu-id="fc109-2609">Problem behoben, aufgrund dessen der Benutzer bei Verwendung des interaktiven Modus in Cloud Shell zur Anmeldung aufgefordert wird</span><span class="sxs-lookup"><span data-stu-id="fc109-2609">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="fc109-2610">Regression mit fehlenden Parametervervollständigungen korrigiert</span><span class="sxs-lookup"><span data-stu-id="fc109-2610">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="fc109-2611">IoT</span><span class="sxs-lookup"><span data-stu-id="fc109-2611">IoT</span></span>

* <span data-ttu-id="fc109-2612">Problem behoben, aufgrund dessen `iot dps access policy [create|update]` bei erfolgreicher Ausführung einen Fehler „nicht gefunden“ zurückgibt</span><span class="sxs-lookup"><span data-stu-id="fc109-2612">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="fc109-2613">Problem behoben, aufgrund dessen `iot dps linked-hub [create|update]` bei erfolgreicher Ausführung einen Fehler „nicht gefunden“ zurückgibt</span><span class="sxs-lookup"><span data-stu-id="fc109-2613">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="fc109-2614">Unterstützung für `--no-wait` zu `iot dps access policy [create|update]` und `iot dps linked-hub [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2614">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="fc109-2615">`iot hub create` geändert, um die Angabe der Anzahl von Partitionen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="fc109-2615">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="fc109-2616">Überwachen</span><span class="sxs-lookup"><span data-stu-id="fc109-2616">Monitor</span></span>

* <span data-ttu-id="fc109-2617">Befehl `az monitor log-profiles create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="fc109-2617">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="fc109-2618">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="fc109-2618">Network</span></span>

* <span data-ttu-id="fc109-2619">Option `--tags` für folgende Befehle korrigiert:</span><span class="sxs-lookup"><span data-stu-id="fc109-2619">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="fc109-2620">Profil</span><span class="sxs-lookup"><span data-stu-id="fc109-2620">Profile</span></span>

* <span data-ttu-id="fc109-2621">`az login` im interaktiven Modus aktiviert</span><span class="sxs-lookup"><span data-stu-id="fc109-2621">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="fc109-2622">Resource</span><span class="sxs-lookup"><span data-stu-id="fc109-2622">Resource</span></span>

* <span data-ttu-id="fc109-2623">`feature show` wieder hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2623">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="fc109-2624">Role</span><span class="sxs-lookup"><span data-stu-id="fc109-2624">Role</span></span>

* <span data-ttu-id="fc109-2625">Argument `--available-to-other-tenants` zu `ad app update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2625">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="fc109-2626">SQL</span><span class="sxs-lookup"><span data-stu-id="fc109-2626">SQL</span></span>

* <span data-ttu-id="fc109-2627">Befehle vom Typ `sql server dns-alias` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2627">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="fc109-2628">`sql db rename` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2628">Added `sql db rename`</span></span>
* <span data-ttu-id="fc109-2629">Unterstützung für das Argument `--ids` für alle SQL-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2629">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="fc109-2630">Storage</span><span class="sxs-lookup"><span data-stu-id="fc109-2630">Storage</span></span>

* <span data-ttu-id="fc109-2631">Befehle `storage blob service-properties delete-policy` und `storage blob undelete` hinzugefügt, um vorläufiges Löschen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="fc109-2631">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="fc109-2632">VM</span><span class="sxs-lookup"><span data-stu-id="fc109-2632">VM</span></span>

* <span data-ttu-id="fc109-2633">Absturz bei unvollständiger Initialisierung der VM-Verschlüsselung behoben</span><span class="sxs-lookup"><span data-stu-id="fc109-2633">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="fc109-2634">Prinzipal-ID-Ausgabe beim Aktivieren von MSI hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2634">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="fc109-2635">`vm boot-diagnostics get-boot-log` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="fc109-2635">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="fc109-2636">31. Januar 2018</span><span class="sxs-lookup"><span data-stu-id="fc109-2636">January 31, 2018</span></span>

<span data-ttu-id="fc109-2637">Version 2.0.26</span><span class="sxs-lookup"><span data-stu-id="fc109-2637">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="fc109-2638">Core</span><span class="sxs-lookup"><span data-stu-id="fc109-2638">Core</span></span>

* <span data-ttu-id="fc109-2639">Unterstützung für das Abrufen von unformatierten Token im MSI-Kontext hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2639">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="fc109-2640">Abrufindikator-Zeichenfolge nach Fertigstellung von LRO für die Windows-Datei „cmd.exe“ entfernt</span><span class="sxs-lookup"><span data-stu-id="fc109-2640">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="fc109-2641">Warnung hinzugefügt, die angezeigt wird, wenn ein konfigurierter Standardwert in einen Eintrag auf INFO-Ebene geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="fc109-2641">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="fc109-2642">`--verbose` zum Anzeigen verwenden.</span><span class="sxs-lookup"><span data-stu-id="fc109-2642">Use `--verbose` to see</span></span>
* <span data-ttu-id="fc109-2643">Statusanzeige für Wait-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2643">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="fc109-2644">ACS</span><span class="sxs-lookup"><span data-stu-id="fc109-2644">ACS</span></span>

* <span data-ttu-id="fc109-2645">Argument `--disable-browser` erläutert</span><span class="sxs-lookup"><span data-stu-id="fc109-2645">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="fc109-2646">Vervollständigung mit der TAB-TASTE für Argumente vom Typ `--vm-size` verbessert</span><span class="sxs-lookup"><span data-stu-id="fc109-2646">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="fc109-2647">AppService</span><span class="sxs-lookup"><span data-stu-id="fc109-2647">Appservice</span></span>

* <span data-ttu-id="fc109-2648">`webapp log [tail|download]` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="fc109-2648">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="fc109-2649">Überprüfung `kind` für Web-Apps und Funktionen entfernt</span><span class="sxs-lookup"><span data-stu-id="fc109-2649">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="fc109-2650">CDN</span><span class="sxs-lookup"><span data-stu-id="fc109-2650">CDN</span></span>

* <span data-ttu-id="fc109-2651">Problem mit fehlendem Client für `cdn custom-domain create` behoben</span><span class="sxs-lookup"><span data-stu-id="fc109-2651">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="fc109-2652">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="fc109-2652">CosmosDB</span></span>

* <span data-ttu-id="fc109-2653">Parameterbeschreibung für Failoverrichtlinien korrigiert</span><span class="sxs-lookup"><span data-stu-id="fc109-2653">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="fc109-2654">Interactive</span><span class="sxs-lookup"><span data-stu-id="fc109-2654">Interactive</span></span>

* <span data-ttu-id="fc109-2655">Problem behoben, aufgrund dessen Vervollständigungen von Befehlsoptionen nicht mehr angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="fc109-2655">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="fc109-2656">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="fc109-2656">Network</span></span>

* <span data-ttu-id="fc109-2657">Schutz für `--cert-password` zu `application-gateway create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2657">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="fc109-2658">Problem mit `application-gateway update` behoben, aufgrund dessen `--sku` fälschlicherweise einen Standardwert anwendete</span><span class="sxs-lookup"><span data-stu-id="fc109-2658">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="fc109-2659">Schutz für `--shared-key` und `--authorization-key` zu `vpn-connection create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2659">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="fc109-2660">Problem mit fehlendem Client für `asg create` behoben</span><span class="sxs-lookup"><span data-stu-id="fc109-2660">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="fc109-2661">Parameter `--file-name / -f` für exportierte Namen zu `dns zone export` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2661">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="fc109-2662">Folgende Probleme mit `dns zone export` behoben:</span><span class="sxs-lookup"><span data-stu-id="fc109-2662">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="fc109-2663">Problem behoben, aufgrund dessen lange TXT-Einträge nicht korrekt exportiert wurden</span><span class="sxs-lookup"><span data-stu-id="fc109-2663">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="fc109-2664">Problem behoben, aufgrund dessen TXT-Einträge in Anführungszeichen fälschlich ohne Anführungszeichen in Escapezeichen exportiert wurden</span><span class="sxs-lookup"><span data-stu-id="fc109-2664">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="fc109-2665">Problem behoben, aufgrund dessen bestimmte Datensätze zweimal mit `dns zone import` importiert wurden</span><span class="sxs-lookup"><span data-stu-id="fc109-2665">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="fc109-2666">Befehle `vnet-gateway root-cert` und `vnet-gateway revoked-cert` wiederhergestellt</span><span class="sxs-lookup"><span data-stu-id="fc109-2666">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="fc109-2667">Profil</span><span class="sxs-lookup"><span data-stu-id="fc109-2667">Profile</span></span>

* <span data-ttu-id="fc109-2668">`get-access-token` zur Verwendung auf einer VM mit Identität korrigiert</span><span class="sxs-lookup"><span data-stu-id="fc109-2668">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="fc109-2669">Resource</span><span class="sxs-lookup"><span data-stu-id="fc109-2669">Resource</span></span>

* <span data-ttu-id="fc109-2670">Fehler mit `deployment [create|validate]` korrigiert, aufgrund dessen fälschlich eine Warnung angezeigt wurde, wenn ein Vorlagenfeld „Typ“ Werte in Großbuchstaben enthielt</span><span class="sxs-lookup"><span data-stu-id="fc109-2670">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="fc109-2671">Storage</span><span class="sxs-lookup"><span data-stu-id="fc109-2671">Storage</span></span>

* <span data-ttu-id="fc109-2672">Problem mit der Migration von Storage V1-Konten zu Storage V2 behoben</span><span class="sxs-lookup"><span data-stu-id="fc109-2672">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="fc109-2673">Statusberichterstellung für alle Upload-/Downloadbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2673">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="fc109-2674">Fehler korrigiert, der die Verwendung der arg-Option „-n“ mit `storage account check-name` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="fc109-2674">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="fc109-2675">Spalte „Momentaufnahme“ zur Tabellenausgabe für `blob [list|show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2675">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="fc109-2676">Fehler mit verschiedenen Parametern korrigiert, die als Int-Typen analysiert werden mussten</span><span class="sxs-lookup"><span data-stu-id="fc109-2676">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="fc109-2677">VM</span><span class="sxs-lookup"><span data-stu-id="fc109-2677">VM</span></span>

* <span data-ttu-id="fc109-2678">Befehl `vm image accept-terms` hinzugefügt, um die Erstellung von VMs aus Images mit zusätzlichen Gebühren zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="fc109-2678">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="fc109-2679">`[vm|vmss create]` korrigiert, um sicherzustellen, dass Befehle unter einem Proxy mit nicht signierten Zertifikaten ausgeführt werden können</span><span class="sxs-lookup"><span data-stu-id="fc109-2679">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="fc109-2680">[VORSCHAU] Unterstützung für „niedrige“ Priorität zu VMSS hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2680">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="fc109-2681">Schutz für `--admin-password` zu `[vm|vmss] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2681">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="fc109-2682">17. Januar 2018</span><span class="sxs-lookup"><span data-stu-id="fc109-2682">January 17, 2018</span></span>

<span data-ttu-id="fc109-2683">Version 2.0.25</span><span class="sxs-lookup"><span data-stu-id="fc109-2683">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="fc109-2684">ACR</span><span class="sxs-lookup"><span data-stu-id="fc109-2684">ACR</span></span>

* <span data-ttu-id="fc109-2685">Fallback auf ACR-Anmeldung bei Fehlern mit Windows-Anmeldeinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2685">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="fc109-2686">Registrierungsprotokolle aktiviert</span><span class="sxs-lookup"><span data-stu-id="fc109-2686">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="fc109-2687">ACS</span><span class="sxs-lookup"><span data-stu-id="fc109-2687">ACS</span></span>

* <span data-ttu-id="fc109-2688">Befehl `get-credentials` korrigiert</span><span class="sxs-lookup"><span data-stu-id="fc109-2688">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="fc109-2689">SPN-Rollenanforderung entfernt</span><span class="sxs-lookup"><span data-stu-id="fc109-2689">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="fc109-2690">AppService</span><span class="sxs-lookup"><span data-stu-id="fc109-2690">Appservice</span></span>

* <span data-ttu-id="fc109-2691">Fehler mit `config ssl upload` behoben, bei dem `hosting_environment_profile` NULL war</span><span class="sxs-lookup"><span data-stu-id="fc109-2691">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="fc109-2692">Unterstützung benutzerdefinierter URLs zu `browse` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2692">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="fc109-2693">Slotunterstützung für `log tail` korrigiert</span><span class="sxs-lookup"><span data-stu-id="fc109-2693">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="fc109-2694">Backup</span><span class="sxs-lookup"><span data-stu-id="fc109-2694">Backup</span></span>

* <span data-ttu-id="fc109-2695">Option `--container-name` von `backup item list` geändert (ist jetzt optional)</span><span class="sxs-lookup"><span data-stu-id="fc109-2695">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="fc109-2696">Speicherkontooptionen zu `backup restore restore-disks` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2696">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="fc109-2697">Standortüberprüfung in `backup protection enable-for-vm` korrigiert (Groß-/Kleinschreibung wird jetzt nicht mehr beachtet)</span><span class="sxs-lookup"><span data-stu-id="fc109-2697">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="fc109-2698">Problem behoben, durch das bei Befehlen mit ungültigem Containernamen ein Fehler auftrat</span><span class="sxs-lookup"><span data-stu-id="fc109-2698">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="fc109-2699">`backup item list` geändert (Integritätsstatus jetzt standardmäßig enthalten)</span><span class="sxs-lookup"><span data-stu-id="fc109-2699">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="fc109-2700">Batch</span><span class="sxs-lookup"><span data-stu-id="fc109-2700">Batch</span></span>

* <span data-ttu-id="fc109-2701">`batch login` geändert, um Authentifizierungsdetails zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="fc109-2701">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="fc109-2702">Cloud</span><span class="sxs-lookup"><span data-stu-id="fc109-2702">Cloud</span></span>

* <span data-ttu-id="fc109-2703">Beim Festlegen von `--profile` für eine Cloud werden nun keine Endpunkte mehr benötigt.</span><span class="sxs-lookup"><span data-stu-id="fc109-2703">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="fc109-2704">Nutzung</span><span class="sxs-lookup"><span data-stu-id="fc109-2704">Consumption</span></span>

* <span data-ttu-id="fc109-2705">Neue Befehle für Reservierungen hinzugefügt: `consumption reservations summaries` und `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="fc109-2705">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="fc109-2706">Event Grid</span><span class="sxs-lookup"><span data-stu-id="fc109-2706">Event Grid</span></span>

* <span data-ttu-id="fc109-2707">[BREAKING CHANGE] Die Befehle vom Typ `az eventgrid topic event-subscription` wurden in `eventgrid event-subscription` verschoben.</span><span class="sxs-lookup"><span data-stu-id="fc109-2707">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="fc109-2708">[BREAKING CHANGE] Die Befehle vom Typ `az eventgrid resource event-subscription` wurden in `eventgrid event-subscription` verschoben.</span><span class="sxs-lookup"><span data-stu-id="fc109-2708">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="fc109-2709">[BREAKING CHANGE] Der Befehl `eventgrid event-subscription show-endpoint-url` wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="fc109-2709">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="fc109-2710">Verwenden Sie stattdessen `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="fc109-2710">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="fc109-2711">Befehl `eventgrid topic update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2711">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="fc109-2712">Befehl `eventgrid event-subscription update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2712">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="fc109-2713">Parameter `--ids` für Befehle vom Typ `eventgrid topic` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2713">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="fc109-2714">Unterstützung der Vervollständigung mit der TAB-TASTE für Themennamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2714">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="fc109-2715">Interactive</span><span class="sxs-lookup"><span data-stu-id="fc109-2715">Interactive</span></span>

* <span data-ttu-id="fc109-2716">Problem behoben, das dazu führte, dass der interaktive Modus nicht mit Python 2.x verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="fc109-2716">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="fc109-2717">Fehler beim Start behoben</span><span class="sxs-lookup"><span data-stu-id="fc109-2717">Fixed errors on startup</span></span>
* <span data-ttu-id="fc109-2718">Problem behoben, das dazu führte, dass einige Befehle nicht im interaktiven Modus ausgeführt werden konnten</span><span class="sxs-lookup"><span data-stu-id="fc109-2718">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="fc109-2719">IoT</span><span class="sxs-lookup"><span data-stu-id="fc109-2719">IoT</span></span>

* <span data-ttu-id="fc109-2720">Unterstützung für Gerätebereitstellungsdienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2720">Added support for device provisioning service</span></span>
* <span data-ttu-id="fc109-2721">Benachrichtigungen zu veralteten Elementen in Befehlen und in der Befehlshilfe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2721">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="fc109-2722">IoT-Überprüfung hinzugefügt, um Benutzer über die IoT-Erweiterung zu informieren</span><span class="sxs-lookup"><span data-stu-id="fc109-2722">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="fc109-2723">Überwachen</span><span class="sxs-lookup"><span data-stu-id="fc109-2723">Monitor</span></span>

* <span data-ttu-id="fc109-2724">Unterstützung mehrerer Diagnoseeinstellung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-2724">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="fc109-2725">Der Parameter `--name` ist nun für `az monitor diagnostic-settings create` erforderlich.</span><span class="sxs-lookup"><span data-stu-id="fc109-2725">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="fc109-2726">Befehl `monitor diagnostic-settings categories` zum Abrufen der Diagnoseeinstellungskategorie hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2726">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="fc109-2727">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="fc109-2727">Network</span></span>

* <span data-ttu-id="fc109-2728">Problem behoben, das beim Ändern des aktiven Standbymodus mit `vnet-gateway update` auftrat</span><span class="sxs-lookup"><span data-stu-id="fc109-2728">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="fc109-2729">Unterstützung für HTTP2 zu `application-gateway [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2729">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="fc109-2730">Profil</span><span class="sxs-lookup"><span data-stu-id="fc109-2730">Profile</span></span>

* <span data-ttu-id="fc109-2731">Unterstützung für die Anmeldung mit durch Benutzer zugewiesenen Identitäten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2731">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="fc109-2732">Role</span><span class="sxs-lookup"><span data-stu-id="fc109-2732">Role</span></span>

* <span data-ttu-id="fc109-2733">Argument `--assignee-object-id` zu `role assignment create` hinzugefügt, um Graph-Abfrage zu umgehen</span><span class="sxs-lookup"><span data-stu-id="fc109-2733">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="fc109-2734">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="fc109-2734">Service Fabric</span></span>

* <span data-ttu-id="fc109-2735">Ausführliche Fehler zur Überprüfungsantwort bei der Clustererstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2735">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="fc109-2736">Problem mit fehlendem Client für verschiedene Befehle behoben</span><span class="sxs-lookup"><span data-stu-id="fc109-2736">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="fc109-2737">VM</span><span class="sxs-lookup"><span data-stu-id="fc109-2737">VM</span></span>

* <span data-ttu-id="fc109-2738">[VORSCHAUVERSION] Zonenübergreifende Unterstützung für `vmss`</span><span class="sxs-lookup"><span data-stu-id="fc109-2738">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="fc109-2739">[BREAKING CHANGE] Standard für Einzelzone (`vmss`) in Standardlastenausgleich geändert</span><span class="sxs-lookup"><span data-stu-id="fc109-2739">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="fc109-2740">[BREAKING CHANGE]`externalIdentities` in `userAssignedIdentities` geändert für EMSI</span><span class="sxs-lookup"><span data-stu-id="fc109-2740">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="fc109-2741">[VORSCHAUVERSION] Unterstützung für Austausch des Betriebssystemdatenträgers hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2741">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="fc109-2742">Unterstützung der Verwendung von VM-Images aus anderen Abonnements hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2742">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="fc109-2743">Argumente `--plan-name`, `--plan-product`, `--plan-promotion-code` und `--plan-publisher` zu `[vm|vmss] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2743">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="fc109-2744">Fehlerbedingte Probleme mit `[vm|vmss] create` behoben</span><span class="sxs-lookup"><span data-stu-id="fc109-2744">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="fc109-2745">Übermäßige Ressourcenverwendung durch `vm image list --all` behoben</span><span class="sxs-lookup"><span data-stu-id="fc109-2745">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="fc109-2746">19. Dezember 2017</span><span class="sxs-lookup"><span data-stu-id="fc109-2746">December 19, 2017</span></span>

<span data-ttu-id="fc109-2747">Version 2.0.23</span><span class="sxs-lookup"><span data-stu-id="fc109-2747">Version 2.0.23</span></span>

* <span data-ttu-id="fc109-2748">Unterstützung für die Anmeldung mit durch Benutzer zugewiesenen Identitäten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2748">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="fc109-2749">Container</span><span class="sxs-lookup"><span data-stu-id="fc109-2749">Container</span></span>

* <span data-ttu-id="fc109-2750">Falsche Reihenfolge der Parameter für Containerprotokolle behoben</span><span class="sxs-lookup"><span data-stu-id="fc109-2750">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="fc109-2751">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="fc109-2751">Network</span></span>

* <span data-ttu-id="fc109-2752">Argument `--disable-bgp-route-propagation` zu `route-table [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2752">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="fc109-2753">Argument `--ip-tags` zu `public-ip [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2753">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="fc109-2754">Storage</span><span class="sxs-lookup"><span data-stu-id="fc109-2754">Storage</span></span>

* <span data-ttu-id="fc109-2755">Unterstützung für Storage V2 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2755">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="fc109-2756">VM</span><span class="sxs-lookup"><span data-stu-id="fc109-2756">VM</span></span>

* <span data-ttu-id="fc109-2757">[VORSCHAUVERSION] Unterstützung für durch Benutzer zugewiesene Identitäten für virtuelle Computer und VMSSs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2757">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="fc109-2758">5\. Dezember 2017</span><span class="sxs-lookup"><span data-stu-id="fc109-2758">December 5, 2017</span></span>

<span data-ttu-id="fc109-2759">Version 2.0.22</span><span class="sxs-lookup"><span data-stu-id="fc109-2759">Version 2.0.22</span></span>

* <span data-ttu-id="fc109-2760">`az component`-Befehle wurden entfernt.</span><span class="sxs-lookup"><span data-stu-id="fc109-2760">Removed `az component` commands.</span></span> <span data-ttu-id="fc109-2761">Verwenden Sie stattdessen `az extension`.</span><span class="sxs-lookup"><span data-stu-id="fc109-2761">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="fc109-2762">Core</span><span class="sxs-lookup"><span data-stu-id="fc109-2762">Core</span></span>
* <span data-ttu-id="fc109-2763">Der `AZURE_US_GOV_CLOUD`-Autoritätsendpunkt von AAD wurde von „login.microsoftonline.com“ in „login.microsoftonline.us“ geändert.</span><span class="sxs-lookup"><span data-stu-id="fc109-2763">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="fc109-2764">Problem behoben, aufgrund dessen Telemetriedaten fortlaufend neu gesendet wurden</span><span class="sxs-lookup"><span data-stu-id="fc109-2764">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="fc109-2765">ACS</span><span class="sxs-lookup"><span data-stu-id="fc109-2765">ACS</span></span>

* <span data-ttu-id="fc109-2766">Die Befehle `aks install-connector` und `aks remove-connector` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-2766">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="fc109-2767">Verbesserte Fehlerberichterstellung für `acs create`</span><span class="sxs-lookup"><span data-stu-id="fc109-2767">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="fc109-2768">Feste Verwendung von `aks get-credentials -f` ohne vollqualifizierten Pfad</span><span class="sxs-lookup"><span data-stu-id="fc109-2768">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="fc109-2769">Advisor</span><span class="sxs-lookup"><span data-stu-id="fc109-2769">Advisor</span></span>

* <span data-ttu-id="fc109-2770">Erste Veröffentlichung</span><span class="sxs-lookup"><span data-stu-id="fc109-2770">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="fc109-2771">AppService</span><span class="sxs-lookup"><span data-stu-id="fc109-2771">Appservice</span></span>

* <span data-ttu-id="fc109-2772">Erstellung feststehender Zertifikatnamen mit `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="fc109-2772">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="fc109-2773">`webapp [list|show]` und `functionapp [list|show]` wurden verbessert, um die richtigen Apps anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="fc109-2773">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="fc109-2774">Standardwert für `WEBSITE_NODE_DEFAULT_VERSION` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2774">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="fc109-2775">Nutzung</span><span class="sxs-lookup"><span data-stu-id="fc109-2775">Consumption</span></span>

* <span data-ttu-id="fc109-2776">Unterstützung für API-Version 2017-11-30 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2776">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="fc109-2777">Container</span><span class="sxs-lookup"><span data-stu-id="fc109-2777">Container</span></span>

* <span data-ttu-id="fc109-2778">Feste Regression für Standardports</span><span class="sxs-lookup"><span data-stu-id="fc109-2778">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="fc109-2779">Überwachen</span><span class="sxs-lookup"><span data-stu-id="fc109-2779">Monitor</span></span>

* <span data-ttu-id="fc109-2780">Unterstützung mehrerer Dimensionen zu Metrikbefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2780">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="fc109-2781">Resource</span><span class="sxs-lookup"><span data-stu-id="fc109-2781">Resource</span></span>

* <span data-ttu-id="fc109-2782">Argument `--include-response-body` zu `resource show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2782">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="fc109-2783">Role</span><span class="sxs-lookup"><span data-stu-id="fc109-2783">Role</span></span>

* <span data-ttu-id="fc109-2784">Anzeige von Standardzuweisungen für „klassische“ Administratoren zu `role assignment list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2784">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="fc109-2785">Unterstützung für das Hinzufügen (anstelle der Überschreibung) von Anmeldeinformationen zu `ad sp reset-credentials` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2785">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="fc109-2786">Verbesserte Fehlerberichterstellung für `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="fc109-2786">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="fc109-2787">SQL</span><span class="sxs-lookup"><span data-stu-id="fc109-2787">SQL</span></span>

* <span data-ttu-id="fc109-2788">Die Befehle `sql db list-usages` und `sql db show-usage` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-2788">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="fc109-2789">Die Befehle `sql server conn-policy show` und `sql server conn-policy update` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-2789">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="fc109-2790">VM</span><span class="sxs-lookup"><span data-stu-id="fc109-2790">VM</span></span>

* <span data-ttu-id="fc109-2791">Zoneninformationen zu `az vm list-skus` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2791">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="fc109-2792">14. November 2017</span><span class="sxs-lookup"><span data-stu-id="fc109-2792">November 14, 2017</span></span>

<span data-ttu-id="fc109-2793">Version 2.0.21</span><span class="sxs-lookup"><span data-stu-id="fc109-2793">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="fc109-2794">ACR</span><span class="sxs-lookup"><span data-stu-id="fc109-2794">ACR</span></span>

* <span data-ttu-id="fc109-2795">Unterstützung für das Erstellen von Webhooks in Replikationsregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2795">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="fc109-2796">ACS</span><span class="sxs-lookup"><span data-stu-id="fc109-2796">ACS</span></span>

* <span data-ttu-id="fc109-2797">Formulierung in AKS von „Agent“ in „Knoten“ geändert</span><span class="sxs-lookup"><span data-stu-id="fc109-2797">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="fc109-2798">Option `--orchestrator-release` für `acs create` als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="fc109-2798">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="fc109-2799">VM-Standardgröße für AKS in `Standard_D1_v2` geändert</span><span class="sxs-lookup"><span data-stu-id="fc109-2799">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="fc109-2800">`az aks browse` für Windows korrigiert</span><span class="sxs-lookup"><span data-stu-id="fc109-2800">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="fc109-2801">`az aks get-credentials` für Windows korrigiert</span><span class="sxs-lookup"><span data-stu-id="fc109-2801">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="fc109-2802">AppService</span><span class="sxs-lookup"><span data-stu-id="fc109-2802">Appservice</span></span>

* <span data-ttu-id="fc109-2803">Bereitstellungsquelle `config-zip` für Web-Apps und Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2803">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="fc109-2804">Option `--docker-container-logging` zu `az webapp log config` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2804">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="fc109-2805">Option `storage` aus dem Parameter `--web-server-logging` von `az webapp log config` entfernt</span><span class="sxs-lookup"><span data-stu-id="fc109-2805">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="fc109-2806">Fehlermeldungen für `deployment user set` verbessert</span><span class="sxs-lookup"><span data-stu-id="fc109-2806">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="fc109-2807">Unterstützung für das Erstellen von Linux-Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2807">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="fc109-2808">`list-locations` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="fc109-2808">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="fc109-2809">Batch</span><span class="sxs-lookup"><span data-stu-id="fc109-2809">Batch</span></span>

* <span data-ttu-id="fc109-2810">Fehler im Poolerstellungsbefehl korrigiert, der bei Verwendung einer Ressourcen-ID mit dem Flag `--image` aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="fc109-2810">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="fc109-2811">BatchAI</span><span class="sxs-lookup"><span data-stu-id="fc109-2811">Batchai</span></span>

* <span data-ttu-id="fc109-2812">Kurzoption (`-s`) für `--vm-size` zur Angabe der VM-Größe im Befehl `file-server create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2812">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="fc109-2813">Argumente für Speicherkontoname und -schlüssel zum Parameter `cluster create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2813">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="fc109-2814">Dokumentation für `job list-files` und `job stream-file` korrigiert</span><span class="sxs-lookup"><span data-stu-id="fc109-2814">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="fc109-2815">Kurzoption (`-r`) für `--cluster-name` zur Angabe des Clusternamens im Befehl `job create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2815">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="fc109-2816">Cloud</span><span class="sxs-lookup"><span data-stu-id="fc109-2816">Cloud</span></span>

* <span data-ttu-id="fc109-2817">`cloud [register|update]` geändert, um die Registrierung von Clouds ohne erforderliche Endpunkte zu verhindern</span><span class="sxs-lookup"><span data-stu-id="fc109-2817">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="fc109-2818">Container</span><span class="sxs-lookup"><span data-stu-id="fc109-2818">Container</span></span>

* <span data-ttu-id="fc109-2819">Unterstützung für das Öffnen mehrerer Ports hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2819">Added support to open multiple ports</span></span>
* <span data-ttu-id="fc109-2820">Neustartrichtlinie für Containergruppen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2820">Added container group restart policy</span></span>
* <span data-ttu-id="fc109-2821">Unterstützung zum Einbinden einer Azure-Dateifreigabe als Volume hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2821">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="fc109-2822">Hilfedokumente aktualisiert</span><span class="sxs-lookup"><span data-stu-id="fc109-2822">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="fc109-2823">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="fc109-2823">Data Lake Analytics</span></span>

* <span data-ttu-id="fc109-2824">`[job|account] list` geändert, um präzisere Informationen zu erhalten</span><span class="sxs-lookup"><span data-stu-id="fc109-2824">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="fc109-2825">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="fc109-2825">Data Lake Store</span></span>

* <span data-ttu-id="fc109-2826">`account list` geändert, um präzisere Informationen zu erhalten</span><span class="sxs-lookup"><span data-stu-id="fc109-2826">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="fc109-2827">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="fc109-2827">Extension</span></span>

* <span data-ttu-id="fc109-2828">`extension list-available` hinzugefügt, um das Auflisten offizieller Microsoft-Erweiterungen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="fc109-2828">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="fc109-2829">`--name` zu `extension [add|update]` hinzugefügt, um das Installieren von Erweiterungen nach Name zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="fc109-2829">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="fc109-2830">IoT</span><span class="sxs-lookup"><span data-stu-id="fc109-2830">IoT</span></span>

* <span data-ttu-id="fc109-2831">Unterstützung für Zertifizierungsstellen (CAs) und Zertifikatketten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2831">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="fc109-2832">Überwachen</span><span class="sxs-lookup"><span data-stu-id="fc109-2832">Monitor</span></span>

* <span data-ttu-id="fc109-2833">Befehle vom Typ `activity-log alert` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2833">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="fc109-2834">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="fc109-2834">Network</span></span>

* <span data-ttu-id="fc109-2835">Unterstützung für CAA-DNS-Einträge hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2835">Added support for CAA DNS records</span></span>
* <span data-ttu-id="fc109-2836">Problem behoben, durch das Endpunkte nicht mit `traffic-manager profile update` aktualisiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="fc109-2836">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="fc109-2837">Problem behoben, durch das `vnet update --dns-servers` je nach VNet-Erstellungsmethode nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="fc109-2837">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="fc109-2838">Problem behoben, durch das relative DNS-Namen durch `dns zone import` nicht korrekt importiert wurden</span><span class="sxs-lookup"><span data-stu-id="fc109-2838">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="fc109-2839">Reservations</span><span class="sxs-lookup"><span data-stu-id="fc109-2839">Reservations</span></span>

* <span data-ttu-id="fc109-2840">Erste Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="fc109-2840">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="fc109-2841">Resource</span><span class="sxs-lookup"><span data-stu-id="fc109-2841">Resource</span></span>

* <span data-ttu-id="fc109-2842">Unterstützung für Ressourcen-IDs zum Parameter `--resource` und Sperren auf Ressourcenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2842">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="fc109-2843">SQL</span><span class="sxs-lookup"><span data-stu-id="fc109-2843">SQL</span></span>

* <span data-ttu-id="fc109-2844">Parameter `--ignore-missing-vnet-service-endpoint` zu `sql server vnet-rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2844">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="fc109-2845">Storage</span><span class="sxs-lookup"><span data-stu-id="fc109-2845">Storage</span></span>

* <span data-ttu-id="fc109-2846">`storage account create` geändert, sodass die SKU `Standard_RAGRS` als Standard verwendet wird</span><span class="sxs-lookup"><span data-stu-id="fc109-2846">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="fc109-2847">Fehler im Zusammenhang mit Datei-/Blobnamen korrigiert, die ASCII-fremde Zeichen enthalten</span><span class="sxs-lookup"><span data-stu-id="fc109-2847">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="fc109-2848">Fehler korrigiert, der die Verwendung von `--source-uri` mit `storage [blob|file] copy start-batch` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="fc109-2848">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="fc109-2849">Befehle zum Globalisieren und Löschen mehrerer Objekte mit `storage [blob|file] delete-batch` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2849">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="fc109-2850">Problem beim Aktivieren von Metriken mit `storage metrics update` behoben</span><span class="sxs-lookup"><span data-stu-id="fc109-2850">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="fc109-2851">Problem mit Dateien über 200 GB bei Verwendung von `storage blob upload-batch` behoben</span><span class="sxs-lookup"><span data-stu-id="fc109-2851">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="fc109-2852">Problem behoben, durch das `--bypass` und `--default-action` von `storage account [create|update]` ignoriert wurden</span><span class="sxs-lookup"><span data-stu-id="fc109-2852">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="fc109-2853">VM</span><span class="sxs-lookup"><span data-stu-id="fc109-2853">VM</span></span>

* <span data-ttu-id="fc109-2854">Fehler mit `vmss create` korrigiert, der die Verwendung der Größenebene `Basic` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="fc109-2854">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="fc109-2855">`--plan`-Argumente zu `[vm|vmss] create` für benutzerdefinierte Images mit Abrechnungsinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2855">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="fc109-2856">Befehle hinzugefügt: `vm secret `[add|remove|list]</span><span class="sxs-lookup"><span data-stu-id="fc109-2856">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="fc109-2857">`vm format-secret` in `vm secret format` umbenannt</span><span class="sxs-lookup"><span data-stu-id="fc109-2857">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="fc109-2858">Argument `--encrypt format` zu `vm encryption enable` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2858">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="fc109-2859">24. Oktober 2017</span><span class="sxs-lookup"><span data-stu-id="fc109-2859">October 24, 2017</span></span>

<span data-ttu-id="fc109-2860">Version 2.0.20</span><span class="sxs-lookup"><span data-stu-id="fc109-2860">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="fc109-2861">Core</span><span class="sxs-lookup"><span data-stu-id="fc109-2861">Core</span></span>

* <span data-ttu-id="fc109-2862">Aktualisierung von `2017-03-09-profile` zur Verwendung von Version `2016-01-01` der `MGMT_STORAGE`-API</span><span class="sxs-lookup"><span data-stu-id="fc109-2862">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="fc109-2863">ACR</span><span class="sxs-lookup"><span data-stu-id="fc109-2863">ACR</span></span>

* <span data-ttu-id="fc109-2864">Die Ressourcenverwaltung wurde aktualisiert und verweist nun auf die API-Version `2017-10-01`.</span><span class="sxs-lookup"><span data-stu-id="fc109-2864">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="fc109-2865">SKU „Bring Your Own Storage“ wurde in „Klassisch“ geändert.</span><span class="sxs-lookup"><span data-stu-id="fc109-2865">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="fc109-2866">Die Registrierungs-SKUs wurden in „Basic“, „Standard“ und „Premium“ umbenannt.</span><span class="sxs-lookup"><span data-stu-id="fc109-2866">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="fc109-2867">ACS</span><span class="sxs-lookup"><span data-stu-id="fc109-2867">ACS</span></span>

* <span data-ttu-id="fc109-2868">[VORSCHAUVERSION] Befehle vom Typ `az aks` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2868">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="fc109-2869">Problem mit `get-credentials` in Kubernetes behoben</span><span class="sxs-lookup"><span data-stu-id="fc109-2869">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="fc109-2870">AppService</span><span class="sxs-lookup"><span data-stu-id="fc109-2870">Appservice</span></span>

* <span data-ttu-id="fc109-2871">Problem behoben, aufgrund dessen heruntergeladene `webapp`-Protokolle unter Umständen ungültig waren</span><span class="sxs-lookup"><span data-stu-id="fc109-2871">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="fc109-2872">Komponente</span><span class="sxs-lookup"><span data-stu-id="fc109-2872">Component</span></span>

* <span data-ttu-id="fc109-2873">Deutlichere Meldung zur Einstellung für alle Installer und für Bestätigungsaufforderung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2873">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="fc109-2874">Überwachen</span><span class="sxs-lookup"><span data-stu-id="fc109-2874">Monitor</span></span>

* <span data-ttu-id="fc109-2875">Befehle vom Typ `action-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2875">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="fc109-2876">Resource</span><span class="sxs-lookup"><span data-stu-id="fc109-2876">Resource</span></span>

* <span data-ttu-id="fc109-2877">Inkompatibilität mit der aktuellen Version der msrest-Abhängigkeit in `group export` behoben</span><span class="sxs-lookup"><span data-stu-id="fc109-2877">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="fc109-2878">Problem mit `policy assignment create` behoben, sodass der Befehl mit integrierten Richtliniendefinitionen und Richtliniensatzdefinitionen verwendet werden kann</span><span class="sxs-lookup"><span data-stu-id="fc109-2878">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="fc109-2879">VM</span><span class="sxs-lookup"><span data-stu-id="fc109-2879">VM</span></span>

* <span data-ttu-id="fc109-2880">Argument `--accelerated-networking` zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2880">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="fc109-2881">9\. Oktober 2017</span><span class="sxs-lookup"><span data-stu-id="fc109-2881">October 9, 2017</span></span>

<span data-ttu-id="fc109-2882">Version 2.0.19</span><span class="sxs-lookup"><span data-stu-id="fc109-2882">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="fc109-2883">Core</span><span class="sxs-lookup"><span data-stu-id="fc109-2883">Core</span></span>

* <span data-ttu-id="fc109-2884">Verarbeitung von ADFS-Autoritäts-URLs wurde mit einem nachgestellten Schrägstrich zu Azure Stack hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-2884">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="fc109-2885">AppService</span><span class="sxs-lookup"><span data-stu-id="fc109-2885">Appservice</span></span>

* <span data-ttu-id="fc109-2886">Mit dem neuen Befehl `webapp update` wurde ein allgemeines Update hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-2886">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="fc109-2887">Batch</span><span class="sxs-lookup"><span data-stu-id="fc109-2887">Batch</span></span>

* <span data-ttu-id="fc109-2888">Aktualisierung auf Batch SDK 4.0.0</span><span class="sxs-lookup"><span data-stu-id="fc109-2888">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="fc109-2889">Die Option `--image` von „VirtualMachineConfiguration“ wurde aktualisiert, um zusätzlich zu „publish:offer:sku:version“ ARM-Imageverweise zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="fc109-2889">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="fc109-2890">Unterstützung für das neue CLI-Erweiterungsmodell für Batch-Erweiterungsbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2890">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="fc109-2891">Batch-Unterstützung aus dem Komponentenmodell entfernt</span><span class="sxs-lookup"><span data-stu-id="fc109-2891">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="fc109-2892">BatchAI</span><span class="sxs-lookup"><span data-stu-id="fc109-2892">Batchai</span></span>

* <span data-ttu-id="fc109-2893">Erste Version des Batch KI-Moduls</span><span class="sxs-lookup"><span data-stu-id="fc109-2893">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="fc109-2894">KeyVault</span><span class="sxs-lookup"><span data-stu-id="fc109-2894">Keyvault</span></span>

* <span data-ttu-id="fc109-2895">Key Vault-Authentifizierungsproblem behoben, das bei Verwendung von ADFS in Azure Stack auftrat.</span><span class="sxs-lookup"><span data-stu-id="fc109-2895">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="fc109-2896">(#4448)</span><span class="sxs-lookup"><span data-stu-id="fc109-2896">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="fc109-2897">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="fc109-2897">Network</span></span>

* <span data-ttu-id="fc109-2898">Das Argument `--server` von `application-gateway address-pool create` ist nun optional, sodass leere Adresspools zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="fc109-2898">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="fc109-2899">`traffic-manager` wurde aktualisiert, um aktuelle Features zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="fc109-2899">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="fc109-2900">Resource</span><span class="sxs-lookup"><span data-stu-id="fc109-2900">Resource</span></span>

* <span data-ttu-id="fc109-2901">Zusätzliche Unterstützung für `--resource-group/-g`-Optionen für Ressourcengruppennamen zu `group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2901">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="fc109-2902">Befehle für `account lock` hinzugefügt, um die Verwendung mit Sperren auf Abonnementebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="fc109-2902">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="fc109-2903">Befehle für `group lock` hinzugefügt, um die Verwendung mit Sperren auf Gruppenebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="fc109-2903">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="fc109-2904">Befehle für `resource lock` hinzugefügt, um die Verwendung mit Sperren auf Ressourcenebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="fc109-2904">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="fc109-2905">Sql</span><span class="sxs-lookup"><span data-stu-id="fc109-2905">Sql</span></span>

* <span data-ttu-id="fc109-2906">Unterstützung für SQL Transparent Data Encryption (TDE) und TDE für Bring Your Own Key-Szenarien hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2906">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="fc109-2907">Der Befehl `db list-deleted` und der Parameter `db restore --deleted-time` wurden hinzugefügt, um die Ermittlung und Wiederherstellung gelöschter Datenbanken zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="fc109-2907">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="fc109-2908">`db op list` und `db op cancel` wurden hinzugefügt, um das Auflisten und Abbrechen ausgeführter Vorgänge für eine Datenbank zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="fc109-2908">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="fc109-2909">Storage</span><span class="sxs-lookup"><span data-stu-id="fc109-2909">Storage</span></span>

* <span data-ttu-id="fc109-2910">Unterstützung für Momentaufnahme von Dateifreigaben hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2910">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="fc109-2911">VM</span><span class="sxs-lookup"><span data-stu-id="fc109-2911">Vm</span></span>

* <span data-ttu-id="fc109-2912">Korrektur eines Fehlers in `vm show`, bei dem die Verwendung von `-d` in Verbindung mit fehlenden privaten IP-Adressen einen Absturz verursachte</span><span class="sxs-lookup"><span data-stu-id="fc109-2912">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="fc109-2913">[VORSCHAUVERSION] Unterstützung für paralleles Upgrade zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2913">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="fc109-2914">Unterstützung für das Aktualisieren der Verschlüsselungseinstellungen mit `vm encryption enable` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2914">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="fc109-2915">Parameter `--os-disk-size-gb` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2915">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="fc109-2916">Parameter `--license-type` für Windows zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2916">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="fc109-2917">22. September 2017</span><span class="sxs-lookup"><span data-stu-id="fc109-2917">September 22, 2017</span></span>

<span data-ttu-id="fc109-2918">Version 2.0.18</span><span class="sxs-lookup"><span data-stu-id="fc109-2918">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="fc109-2919">Resource</span><span class="sxs-lookup"><span data-stu-id="fc109-2919">Resource</span></span>

* <span data-ttu-id="fc109-2920">Unterstützung für das Anzeigen integrierter Richtliniendefinitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2920">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="fc109-2921">Unterstützungsmodusparameter zum Erstellen von Richtliniendefinitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2921">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="fc109-2922">Unterstützung für UI-Definitionen und -Vorlagen zu `managedapp definition create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2922">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="fc109-2923">[BREAKING CHANGE] Der Ressourcentyp `managedapp` wurde von `appliances` in `applications` und von `applianceDefinitions` in `applicationDefinitions` geändert.</span><span class="sxs-lookup"><span data-stu-id="fc109-2923">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="fc109-2924">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="fc109-2924">Network</span></span>

* <span data-ttu-id="fc109-2925">Unterstützung für Verfügbarkeitszone zu Unterbefehlen `network lb` und `network public-ip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2925">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="fc109-2926">Unterstützung für IPv6-Microsoft-Peering zu `express-route` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2926">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="fc109-2927">Befehle für Anwendungssicherheitsgruppe `asg` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2927">Added `asg` application security group commands</span></span>
* <span data-ttu-id="fc109-2928">Argument `--application-security-groups` zu `nic [create|ip-config create|ip-config update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2928">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="fc109-2929">Argumente `--source-asgs` und `--destination-asgs` zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2929">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="fc109-2930">Argumente `--ddos-protection` und `--vm-protection` zu `vnet [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2930">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="fc109-2931">Befehle vom Typ `network [vnet-gateway|vpn-client|show-url]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2931">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="fc109-2932">Storage</span><span class="sxs-lookup"><span data-stu-id="fc109-2932">Storage</span></span>

* <span data-ttu-id="fc109-2933">Problem behoben, das nach der Aktualisierung des SDK unter Umständen einen Fehler der `storage account network-rule`-Befehle zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="fc109-2933">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="fc109-2934">Eventgrid</span><span class="sxs-lookup"><span data-stu-id="fc109-2934">Eventgrid</span></span>

* <span data-ttu-id="fc109-2935">Azure Event Grid Python SDK für die Verwendung der neueren API-Version „2017-09-15-preview“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="fc109-2935">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="fc109-2936">SQL</span><span class="sxs-lookup"><span data-stu-id="fc109-2936">SQL</span></span>

* <span data-ttu-id="fc109-2937">`sql server list`-Argument `--resource-group` geändert, sodass es nun optional ist.</span><span class="sxs-lookup"><span data-stu-id="fc109-2937">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="fc109-2938">Wird es nicht angegeben, werden alle SQL Server-Instanzen im Abonnement zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fc109-2938">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="fc109-2939">Parameter `--no-wait` zu `db [create|copy|restore|update|replica create|create|update]` und `dw [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2939">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="fc109-2940">KeyVault</span><span class="sxs-lookup"><span data-stu-id="fc109-2940">Keyvault</span></span>

* <span data-ttu-id="fc109-2941">Unterstützung für die Keyvault-Befehlsausführung hinter einem Proxy hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2941">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="fc109-2942">VM</span><span class="sxs-lookup"><span data-stu-id="fc109-2942">VM</span></span>

* <span data-ttu-id="fc109-2943">Unterstützung für Verfügbarkeitszone zu `[vm|vmss|disk] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2943">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="fc109-2944">Problem behoben, das bei Verwendung von `--app-gateway ID` mit `vmss create` einen Fehler zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="fc109-2944">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="fc109-2945">Argument `--asgs` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2945">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="fc109-2946">Unterstützung für die Ausführung von Befehlen auf virtuellen Computern mit `vm run-command` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2946">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="fc109-2947">[VORSCHAU] Unterstützung für VMSS-Datenträgerverschlüsselung mit `vmss encryption` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2947">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="fc109-2948">Unterstützung für die Durchführung der Wartung auf virtuellen Computern mit `vm perform-maintenance` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2948">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="fc109-2949">ACS</span><span class="sxs-lookup"><span data-stu-id="fc109-2949">ACS</span></span>

* <span data-ttu-id="fc109-2950">[VORSCHAU] Argument `--orchestrator-release` zu `acs create` für ACS-Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2950">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="fc109-2951">AppService</span><span class="sxs-lookup"><span data-stu-id="fc109-2951">Appservice</span></span>

* <span data-ttu-id="fc109-2952">Neue Möglichkeit zum Aktualisieren und Anzeigen der Authentifizierungseinstellungen mit `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="fc109-2952">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="fc109-2953">Backup</span><span class="sxs-lookup"><span data-stu-id="fc109-2953">Backup</span></span>

* <span data-ttu-id="fc109-2954">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="fc109-2954">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="fc109-2955">11. September 2017</span><span class="sxs-lookup"><span data-stu-id="fc109-2955">September 11, 2017</span></span>

<span data-ttu-id="fc109-2956">Version 2.0.17</span><span class="sxs-lookup"><span data-stu-id="fc109-2956">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="fc109-2957">Core</span><span class="sxs-lookup"><span data-stu-id="fc109-2957">Core</span></span>

* <span data-ttu-id="fc109-2958">Festlegung einer eigenen Korrelations-ID in Telemetrie durch das Befehlsmodul aktiviert</span><span class="sxs-lookup"><span data-stu-id="fc109-2958">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="fc109-2959">Ein Problem mit der JSON-Sicherungsdatei wurde behoben, das beim Festlegen des Diagnosemodus für Telemetrie auftrat</span><span class="sxs-lookup"><span data-stu-id="fc109-2959">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="fc109-2960">ACS</span><span class="sxs-lookup"><span data-stu-id="fc109-2960">Acs</span></span>

* <span data-ttu-id="fc109-2961">Befehl `acs list-locations` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2961">Added `acs list-locations` command</span></span>
* <span data-ttu-id="fc109-2962">`ssh-key-file` wird mit dem erwarteten Standardwert versehen.</span><span class="sxs-lookup"><span data-stu-id="fc109-2962">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="fc109-2963">AppService</span><span class="sxs-lookup"><span data-stu-id="fc109-2963">Appservice</span></span>

* <span data-ttu-id="fc109-2964">Neue Möglichkeit zum Erstellen einer Web-App in einer anderen Ressourcengruppe als der des aktiven Diensttarifs</span><span class="sxs-lookup"><span data-stu-id="fc109-2964">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="fc109-2965">CDN</span><span class="sxs-lookup"><span data-stu-id="fc109-2965">CDN</span></span>

* <span data-ttu-id="fc109-2966">Der Fehler bei `cdn custom-domain create`, dass „CustomDomain“ nicht wiederholbar ist, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="fc109-2966">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="fc109-2967">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="fc109-2967">Extension</span></span>

* <span data-ttu-id="fc109-2968">Erstrelease</span><span class="sxs-lookup"><span data-stu-id="fc109-2968">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="fc109-2969">KeyVault</span><span class="sxs-lookup"><span data-stu-id="fc109-2969">Keyvault</span></span>

* <span data-ttu-id="fc109-2970">Problem behoben, aufgrund dessen bei den Berechtigungen für `keyvault set-policy` die Groß-/Kleinschreibung beachtet werden musste</span><span class="sxs-lookup"><span data-stu-id="fc109-2970">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="fc109-2971">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="fc109-2971">Network</span></span>

* <span data-ttu-id="fc109-2972">`vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="fc109-2972">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="fc109-2973">Das Argument `--private-access-services` wurde für `vnet subnet create/update` in `--service-endpoints` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="fc109-2973">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="fc109-2974">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2974">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="fc109-2975">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2975">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="fc109-2976">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2976">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="fc109-2977">Resource</span><span class="sxs-lookup"><span data-stu-id="fc109-2977">Resource</span></span>

* <span data-ttu-id="fc109-2978">Übergabe von Parameterdefinitionen für Ressourcenrichtlinien in `policy definition create` und `policy definition update` zulassen</span><span class="sxs-lookup"><span data-stu-id="fc109-2978">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="fc109-2979">Übergabe von Parameterwerten für `policy assignment create` zulassen</span><span class="sxs-lookup"><span data-stu-id="fc109-2979">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="fc109-2980">Übergabe von JSON-Code oder einer Datei für alle Parameter zulassen</span><span class="sxs-lookup"><span data-stu-id="fc109-2980">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="fc109-2981">Inkrementierte API-Version</span><span class="sxs-lookup"><span data-stu-id="fc109-2981">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="fc109-2982">SQL</span><span class="sxs-lookup"><span data-stu-id="fc109-2982">SQL</span></span>

* <span data-ttu-id="fc109-2983">Befehle vom Typ `sql server vnet-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-2983">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="fc109-2984">VM</span><span class="sxs-lookup"><span data-stu-id="fc109-2984">VM</span></span>

* <span data-ttu-id="fc109-2985">Behoben: Zugriff nur zuweisen, wenn `--scope` angegeben wird</span><span class="sxs-lookup"><span data-stu-id="fc109-2985">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="fc109-2986">Behoben: Gleiche Erweiterungsbenennung wie Portal verwenden</span><span class="sxs-lookup"><span data-stu-id="fc109-2986">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="fc109-2987">`subscription` aus der Ausgabe von `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="fc109-2987">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="fc109-2988">Behoben: Speicher-SKU vom Typ `[vm|vmss] create` wird nicht auf Datenträger mit einem Image angewendet.</span><span class="sxs-lookup"><span data-stu-id="fc109-2988">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="fc109-2989">Behoben: `vm format-secret --secrets` akzeptierte keine durch neue Zeilen getrennte IDs.</span><span class="sxs-lookup"><span data-stu-id="fc109-2989">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="fc109-2990">31. August 2017</span><span class="sxs-lookup"><span data-stu-id="fc109-2990">August 31, 2017</span></span>

<span data-ttu-id="fc109-2991">Version 2.0.16</span><span class="sxs-lookup"><span data-stu-id="fc109-2991">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="fc109-2992">KeyVault</span><span class="sxs-lookup"><span data-stu-id="fc109-2992">Keyvault</span></span>

* <span data-ttu-id="fc109-2993">Fehler behoben, der beim Versuch auftrat, die Geheimniscodierung mit `secret download` automatisch aufzulösen</span><span class="sxs-lookup"><span data-stu-id="fc109-2993">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="fc109-2994">Sf</span><span class="sxs-lookup"><span data-stu-id="fc109-2994">Sf</span></span>

* <span data-ttu-id="fc109-2995">Alle Befehle wurden durch die Service Fabric-Befehlszeilenschnittstelle (sfctl) ersetzt.</span><span class="sxs-lookup"><span data-stu-id="fc109-2995">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="fc109-2996">Storage</span><span class="sxs-lookup"><span data-stu-id="fc109-2996">Storage</span></span>

* <span data-ttu-id="fc109-2997">Problem behoben, aufgrund dessen Speicherkonten nicht in Regionen erstellt werden konnten, die die NetworkACLs-Funktion nicht unterstützen</span><span class="sxs-lookup"><span data-stu-id="fc109-2997">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="fc109-2998">Festlegen des Inhaltstyps und der Inhaltscodierung während Blob- und Dateiuploads, wenn weder Inhaltstyp noch Inhaltscodierung angegeben sind</span><span class="sxs-lookup"><span data-stu-id="fc109-2998">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="fc109-2999">28. August 2017</span><span class="sxs-lookup"><span data-stu-id="fc109-2999">August 28, 2017</span></span>

<span data-ttu-id="fc109-3000">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="fc109-3000">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="fc109-3001">Befehlszeilenschnittstelle (CLI)</span><span class="sxs-lookup"><span data-stu-id="fc109-3001">CLI</span></span>

* <span data-ttu-id="fc109-3002">Rechtlichen Hinweis zu `--version` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-3002">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="fc109-3003">ACS</span><span class="sxs-lookup"><span data-stu-id="fc109-3003">ACS</span></span>

* <span data-ttu-id="fc109-3004">Vorschauregionen korrigiert</span><span class="sxs-lookup"><span data-stu-id="fc109-3004">Corrected preview regions</span></span>
* <span data-ttu-id="fc109-3005">Standardmäßiges DNS-Namenspräfix (`dns_name_prefix`) ordnungsgemäß formatiert</span><span class="sxs-lookup"><span data-stu-id="fc109-3005">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="fc109-3006">ACS-Befehlsausgabe optimiert</span><span class="sxs-lookup"><span data-stu-id="fc109-3006">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="fc109-3007">AppService</span><span class="sxs-lookup"><span data-stu-id="fc109-3007">Appservice</span></span>

* <span data-ttu-id="fc109-3008">[BREAKING CHANGE] Inkonsistenzen in der Ausgabe von `az webapp config appsettings [delete|set]` behoben</span><span class="sxs-lookup"><span data-stu-id="fc109-3008">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="fc109-3009">Neuen Alias (`-i`) für `az webapp config container set --docker-custom-image-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-3009">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="fc109-3010">`az webapp log show` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="fc109-3010">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="fc109-3011">Neue Argumente aus `az webapp delete` verfügbar gemacht, um App Service-Plan, Metriken oder DNS-Registrierung beizubehalten</span><span class="sxs-lookup"><span data-stu-id="fc109-3011">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="fc109-3012">Behoben: Korrekte Erkennung der Sloteinstellungen</span><span class="sxs-lookup"><span data-stu-id="fc109-3012">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="fc109-3013">IoT</span><span class="sxs-lookup"><span data-stu-id="fc109-3013">IoT</span></span>

* <span data-ttu-id="fc109-3014">#3934 behoben: Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="fc109-3014">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="fc109-3015">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="fc109-3015">Network</span></span>

* <span data-ttu-id="fc109-3016">[BREAKING CHANGE]`vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="fc109-3016">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="fc109-3017">[BREAKING CHANGE] Option `--private-access-services` für `--service-endpoints` in `vnet subnet [create|update]` umbenannt</span><span class="sxs-lookup"><span data-stu-id="fc109-3017">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="fc109-3018">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-3018">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="fc109-3019">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-3019">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="fc109-3020">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-3020">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="fc109-3021">Profil</span><span class="sxs-lookup"><span data-stu-id="fc109-3021">Profile</span></span>

* <span data-ttu-id="fc109-3022">`--msi` und `--msi-port` für die Anmeldung mit der Identität eines virtuellen Computers verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="fc109-3022">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="fc109-3023">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="fc109-3023">Service Fabric</span></span>

* <span data-ttu-id="fc109-3024">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="fc109-3024">Preview release</span></span>
* <span data-ttu-id="fc109-3025">Registrierungsbenutzer-/-kennwortregeln für Befehl vereinfacht</span><span class="sxs-lookup"><span data-stu-id="fc109-3025">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="fc109-3026">Kennwortanforderung für Benutzer trotz Parameterübergabe behoben</span><span class="sxs-lookup"><span data-stu-id="fc109-3026">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="fc109-3027">Unterstützung für leere Registrierungsanmeldeinformationen (`registry_cred`) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-3027">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="fc109-3028">Storage</span><span class="sxs-lookup"><span data-stu-id="fc109-3028">Storage</span></span>

* <span data-ttu-id="fc109-3029">Festlegen des Blobtarifs ermöglicht</span><span class="sxs-lookup"><span data-stu-id="fc109-3029">Enabled setting blob tier</span></span>
* <span data-ttu-id="fc109-3030">Argumente `--bypass` und `--default-action` zur Unterstützung von Diensttunneling zu `storage account [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-3030">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="fc109-3031">Befehle zum Hinzufügen von VNet-Regeln und IP-basierten Regeln zu `storage account network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-3031">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="fc109-3032">Dienstverschlüsselung durch vom Kunden verwalteten Schlüssel ermöglicht</span><span class="sxs-lookup"><span data-stu-id="fc109-3032">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="fc109-3033">[BREAKING CHANGE] Option `--encryption` für Befehl `az storage account create and az storage account update` in `--encryption-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="fc109-3033">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="fc109-3034">Behoben (4220): `az storage account update encryption` – Syntaxkonflikt</span><span class="sxs-lookup"><span data-stu-id="fc109-3034">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="fc109-3035">VM</span><span class="sxs-lookup"><span data-stu-id="fc109-3035">VM</span></span>

* <span data-ttu-id="fc109-3036">Problem behoben, aufgrund dessen bei Verwendung von `--instance-id *` zusätzliche, fehlerhafte Informationen für `vmss get-instance-view` angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="fc109-3036">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="fc109-3037">Unterstützung für `--lb-sku` zu `vmss create` hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="fc109-3037">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="fc109-3038">Menschliche Namen aus der Administratornamen-Blacklist für `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="fc109-3038">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="fc109-3039">Problem behoben, aufgrund dessen `[vm|vmss] create` einen Fehler ausgelöst hat, wenn aus einem Image keine Tarifinformationen extrahiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="fc109-3039">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="fc109-3040">Absturzproblem beim Erstellen einer VMMS-Skalierungsgruppe mit einem internen Lastenausgleich behoben</span><span class="sxs-lookup"><span data-stu-id="fc109-3040">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="fc109-3041">Problem behoben, aufgrund dessen das Argument `--no-wait` nicht mit `vm availability-set create` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="fc109-3041">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="fc109-3042">15. August 2017</span><span class="sxs-lookup"><span data-stu-id="fc109-3042">August 15, 2017</span></span>

<span data-ttu-id="fc109-3043">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="fc109-3043">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="fc109-3044">ACS</span><span class="sxs-lookup"><span data-stu-id="fc109-3044">ACS</span></span>

* <span data-ttu-id="fc109-3045">sshMaster0-Portnummer für Kubernetes korrigiert</span><span class="sxs-lookup"><span data-stu-id="fc109-3045">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="fc109-3046">AppService</span><span class="sxs-lookup"><span data-stu-id="fc109-3046">Appservice</span></span>

* <span data-ttu-id="fc109-3047">Ausnahme beim Erstellen einer neuen Git-basierten Linux-Web-App behoben</span><span class="sxs-lookup"><span data-stu-id="fc109-3047">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="fc109-3048">Event Grid</span><span class="sxs-lookup"><span data-stu-id="fc109-3048">Event Grid</span></span>

* <span data-ttu-id="fc109-3049">SDK-Abhängigkeiten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-3049">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="fc109-3050">11. August 2017</span><span class="sxs-lookup"><span data-stu-id="fc109-3050">August 11, 2017</span></span>

<span data-ttu-id="fc109-3051">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="fc109-3051">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="fc109-3052">ACS</span><span class="sxs-lookup"><span data-stu-id="fc109-3052">ACS</span></span>

* <span data-ttu-id="fc109-3053">Weitere Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-3053">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="fc109-3054">Batch</span><span class="sxs-lookup"><span data-stu-id="fc109-3054">Batch</span></span>

* <span data-ttu-id="fc109-3055">Auf Batch SDK 3.1.0 und Batch Management SDK 4.1.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="fc109-3055">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="fc109-3056">Neuen Befehl zum Anzeigen der Aufgabenanzahl eines Auftrags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-3056">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="fc109-3057">Fehler in der SAS-URL-Verarbeitung der Ressourcendatei behoben</span><span class="sxs-lookup"><span data-stu-id="fc109-3057">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="fc109-3058">Batch-Kontoendpunkt unterstützt nun optionales Präfix „https://“</span><span class="sxs-lookup"><span data-stu-id="fc109-3058">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="fc109-3059">Unterstützung für das Hinzufügen von Listen mit mehr als 100 Aufgaben zu einem Auftrag</span><span class="sxs-lookup"><span data-stu-id="fc109-3059">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="fc109-3060">Debugprotokollierung für das Laden des Erweiterungsbefehlsmoduls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-3060">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="fc109-3061">Komponente</span><span class="sxs-lookup"><span data-stu-id="fc109-3061">Component</span></span>

* <span data-ttu-id="fc109-3062">Warnung für veraltete Befehle vom Typ „az component“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-3062">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="fc109-3063">Container</span><span class="sxs-lookup"><span data-stu-id="fc109-3063">Container</span></span>

* <span data-ttu-id="fc109-3064">`create`: Problem behoben, aufgrund dessen das Gleichheitszeichen innerhalb einer Umgebungsvariablen nicht zulässig war</span><span class="sxs-lookup"><span data-stu-id="fc109-3064">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="fc109-3065">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="fc109-3065">Data Lake Store</span></span>

* <span data-ttu-id="fc109-3066">Fortschrittsüberwachung ermöglicht</span><span class="sxs-lookup"><span data-stu-id="fc109-3066">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="fc109-3067">Event Grid</span><span class="sxs-lookup"><span data-stu-id="fc109-3067">Event Grid</span></span>

* <span data-ttu-id="fc109-3068">Erste Veröffentlichung</span><span class="sxs-lookup"><span data-stu-id="fc109-3068">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="fc109-3069">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="fc109-3069">Network</span></span>

* <span data-ttu-id="fc109-3070">`lb`: Problem behoben, aufgrund dessen bestimmte Namen untergeordneter Ressourcen bei Auslassung nicht richtig aufgelöst wurden</span><span class="sxs-lookup"><span data-stu-id="fc109-3070">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="fc109-3071">`application-gateway {subresource} delete`: Problem behoben, aufgrund dessen `--no-wait` nicht berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="fc109-3071">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="fc109-3072">`application-gateway http-settings update`: Problem behoben, aufgrund dessen `--connection-draining-timeout` nicht deaktiviert werden konnte</span><span class="sxs-lookup"><span data-stu-id="fc109-3072">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="fc109-3073">Fehler behoben: Unerwartetes Schlüsselwortargument `sa_data_size_kilobyes` bei `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="fc109-3073">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="fc109-3074">Profil</span><span class="sxs-lookup"><span data-stu-id="fc109-3074">Profile</span></span>

* <span data-ttu-id="fc109-3075">`account list`: `--refresh` hinzugefügt, um die neuesten Abonnements vom Server zu synchronisieren</span><span class="sxs-lookup"><span data-stu-id="fc109-3075">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="fc109-3076">Storage</span><span class="sxs-lookup"><span data-stu-id="fc109-3076">Storage</span></span>

* <span data-ttu-id="fc109-3077">Aktualisieren des Speicherkontos mit vom System zugewiesener Identität ermöglicht</span><span class="sxs-lookup"><span data-stu-id="fc109-3077">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="fc109-3078">VM</span><span class="sxs-lookup"><span data-stu-id="fc109-3078">VM</span></span>

* <span data-ttu-id="fc109-3079">`availability-set`: Fehlerdomänenanzahl bei Konvertierung verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="fc109-3079">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="fc109-3080">Befehl `list-skus` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="fc109-3080">Exposed `list-skus` command</span></span>
* <span data-ttu-id="fc109-3081">Unterstützung der Identitätszuweisung ohne Erstellung von Rollenzuweisungen</span><span class="sxs-lookup"><span data-stu-id="fc109-3081">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="fc109-3082">Anwenden von Speicher-SKU beim Anfügen von Datenträgern</span><span class="sxs-lookup"><span data-stu-id="fc109-3082">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="fc109-3083">Standardmäßiger Betriebssystemdatenträger-Name und Speicher-SKU bei Verwendung verwalteter Datenträger entfernt</span><span class="sxs-lookup"><span data-stu-id="fc109-3083">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="fc109-3084">28. Juli 2017</span><span class="sxs-lookup"><span data-stu-id="fc109-3084">July 28, 2017</span></span>

<span data-ttu-id="fc109-3085">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="fc109-3085">Version 2.0.12</span></span>

* <span data-ttu-id="fc109-3086">Containerbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-3086">Added container commands</span></span>
* <span data-ttu-id="fc109-3087">Abrechnungs- und Nutzungsmodule hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-3087">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="fc109-3088">Core</span><span class="sxs-lookup"><span data-stu-id="fc109-3088">Core</span></span>

* <span data-ttu-id="fc109-3089">Ausgabe von SDK-Authentifizierungsinformationen für Dienstprinzipale mit Zertifikaten</span><span class="sxs-lookup"><span data-stu-id="fc109-3089">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="fc109-3090">Ausnahmen beim Bereitstellungsfortschritt behoben</span><span class="sxs-lookup"><span data-stu-id="fc109-3090">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="fc109-3091">Verwendung des ARM-Endpunkts aus der aktuellen Cloud für die Erstellung des Abonnementclients</span><span class="sxs-lookup"><span data-stu-id="fc109-3091">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="fc109-3092">Gleichzeitige Verarbeitung der Datei „clouds.config“ verbessert (3636)</span><span class="sxs-lookup"><span data-stu-id="fc109-3092">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="fc109-3093">Aktualisierung der Clientanforderungs-ID für jede Befehlsausführung</span><span class="sxs-lookup"><span data-stu-id="fc109-3093">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="fc109-3094">Erstellung von Abonnementclients mit richtigem SDK-Profil (3635)</span><span class="sxs-lookup"><span data-stu-id="fc109-3094">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="fc109-3095">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="fc109-3095">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="fc109-3096">Unterstützung für Auswahl von Tabellenausgabefeldern über jmespath Abfrage hinzugefügt (3581)</span><span class="sxs-lookup"><span data-stu-id="fc109-3096">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="fc109-3097">Stummschaltung von Analyseargumenten und Anfügeverlauf mit Gesten verbessert (3434)</span><span class="sxs-lookup"><span data-stu-id="fc109-3097">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="fc109-3098">Erstellung von Abonnementclients mit richtigem SDK-Profil</span><span class="sxs-lookup"><span data-stu-id="fc109-3098">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="fc109-3099">Verschiebung aller vorhandenen Erfassungsdateien in den neuesten Ordner</span><span class="sxs-lookup"><span data-stu-id="fc109-3099">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="fc109-3100">Idempotenz für VM-/VMSS-Erstellung behoben (3586)</span><span class="sxs-lookup"><span data-stu-id="fc109-3100">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="fc109-3101">Bei Befehlspfaden wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="fc109-3101">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="fc109-3102">Bei bestimmten booleschen Parametern wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="fc109-3102">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="fc109-3103">Unterstützung der Anmeldung bei lokalem AD FS-Server wie Azure Stack</span><span class="sxs-lookup"><span data-stu-id="fc109-3103">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="fc109-3104">Gleichzeitige Schreibvorgänge in „clouds.config“ behoben (3255)</span><span class="sxs-lookup"><span data-stu-id="fc109-3104">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="fc109-3105">ACR</span><span class="sxs-lookup"><span data-stu-id="fc109-3105">ACR</span></span>

* <span data-ttu-id="fc109-3106">Befehl `show-usage` für verwaltete Registrierungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-3106">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="fc109-3107">Unterstützung der SKU-Aktualisierung für verwaltete Registrierungen</span><span class="sxs-lookup"><span data-stu-id="fc109-3107">Support SKU update for managed registries</span></span>
* <span data-ttu-id="fc109-3108">Verwaltete Registrierungen mit verwalteter SKU hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-3108">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="fc109-3109">Webhooks für verwaltete Registrierungen mit ACR-Webhook-Befehlsmodul hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-3109">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="fc109-3110">AAD-Authentifizierung mit ACR-Anmeldebefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-3110">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="fc109-3111">Löschbefehl für Docker-Repositorys, Manifeste und Tags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-3111">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="fc109-3112">ACS</span><span class="sxs-lookup"><span data-stu-id="fc109-3112">ACS</span></span>

* <span data-ttu-id="fc109-3113">Unterstützung der API-Version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="fc109-3113">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="fc109-3114">AppService</span><span class="sxs-lookup"><span data-stu-id="fc109-3114">Appservice</span></span>

* <span data-ttu-id="fc109-3115">Fehler behoben, aufgrund dessen die Auflistung der Linux-Web-App keine Werte zurückgegeben hat</span><span class="sxs-lookup"><span data-stu-id="fc109-3115">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="fc109-3116">Unterstützung für das Abrufen von Anmeldeinformationen aus dem ACR</span><span class="sxs-lookup"><span data-stu-id="fc109-3116">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="fc109-3117">Entfernung aller Befehle unter `appservice web`</span><span class="sxs-lookup"><span data-stu-id="fc109-3117">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="fc109-3118">Maskierung von Docker-Registrierungskennwörtern aus der Befehlsausgabe (3656)</span><span class="sxs-lookup"><span data-stu-id="fc109-3118">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="fc109-3119">Gewährleistung der fehlerfreien Verwendung des Standardbrowsers unter macOS (3623)</span><span class="sxs-lookup"><span data-stu-id="fc109-3119">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="fc109-3120">Verbesserung des Nutzens von `webapp log tail` und `webapp log download` (3624)</span><span class="sxs-lookup"><span data-stu-id="fc109-3120">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="fc109-3121">Befehl `traffic-routing` zum Konfigurieren des statischen Routings verfügbar gemacht (3566)</span><span class="sxs-lookup"><span data-stu-id="fc109-3121">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="fc109-3122">Zuverlässigkeit beim Konfigurieren der Quellcodeverwaltung verbessert (3245)</span><span class="sxs-lookup"><span data-stu-id="fc109-3122">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="fc109-3123">Nicht unterstütztes Argument `--node-version` aus `webapp config update` für Windows-Web-Apps entfernt.</span><span class="sxs-lookup"><span data-stu-id="fc109-3123">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="fc109-3124">Verwenden Sie stattdessen `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="fc109-3124">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="fc109-3125">Batch</span><span class="sxs-lookup"><span data-stu-id="fc109-3125">Batch</span></span>

* <span data-ttu-id="fc109-3126">Auf Batch SDK 3.0.0 mit Unterstützung virtueller Computer mit niedriger Priorität in Pools aktualisiert</span><span class="sxs-lookup"><span data-stu-id="fc109-3126">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="fc109-3127">`pool create`-Option `--target-dedicated` in `--target-dedicated-nodes` umbenannt</span><span class="sxs-lookup"><span data-stu-id="fc109-3127">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="fc109-3128">`pool create`-Optionen `--target-low-priority-nodes` und `--application-licenses` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-3128">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="fc109-3129">CDN</span><span class="sxs-lookup"><span data-stu-id="fc109-3129">CDN</span></span>

* <span data-ttu-id="fc109-3130">Besser verständliche Fehlermeldung für `cdn endpoint list`, wenn das von `--profile-name` angegebene Profil nicht vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="fc109-3130">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="fc109-3131">Cloud</span><span class="sxs-lookup"><span data-stu-id="fc109-3131">Cloud</span></span>

* <span data-ttu-id="fc109-3132">API-Version des Cloudmetadaten-Endpunkts in das Format JJJJ-MM-TT umgewandelt</span><span class="sxs-lookup"><span data-stu-id="fc109-3132">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="fc109-3133">Katalogendpunkt nicht erforderlich</span><span class="sxs-lookup"><span data-stu-id="fc109-3133">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="fc109-3134">Unterstützung für die Cloudregistrierung nur mit ARM-Endpunkt</span><span class="sxs-lookup"><span data-stu-id="fc109-3134">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="fc109-3135">Option für `cloud set` bereitgestellt, um beim Auswählen der aktuellen Cloud das Profil auswählen zu können</span><span class="sxs-lookup"><span data-stu-id="fc109-3135">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="fc109-3136">`endpoint_vm_image_alias_doc` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="fc109-3136">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="fc109-3137">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="fc109-3137">CosmosDB</span></span>

* <span data-ttu-id="fc109-3138">Möglichkeit zum Erstellen einer Auflistung mit benutzerdefiniertem Partitionsschlüssel behoben</span><span class="sxs-lookup"><span data-stu-id="fc109-3138">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="fc109-3139">Unterstützung für Auflistungs-Standardgültigkeitsdauer hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-3139">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="fc109-3140">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="fc109-3140">Data Lake Analytics</span></span>

* <span data-ttu-id="fc109-3141">Zusätzliche Befehle für Compute-Richtlinienverwaltung unter der Überschrift `dla account compute-policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-3141">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="fc109-3142">`dla job pipeline show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-3142">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="fc109-3143">`dla job recurrence list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-3143">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="fc109-3144">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="fc109-3144">Data Lake Store</span></span>

* <span data-ttu-id="fc109-3145">Unterstützung für vom Benutzer verwaltete Schlüsseltresor-Schlüsselrotation in `dls account update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-3145">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="fc109-3146">Zugrunde liegende SDK-Version des Data Lake Store-Dateisystems aktualisiert, um ein Leistungsproblem zu behandeln</span><span class="sxs-lookup"><span data-stu-id="fc109-3146">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="fc109-3147">Befehl `dls enable-key-vault` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="fc109-3147">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="fc109-3148">Dieser Befehl versucht, eine vom Benutzer angegebene Key Vault-Instanz zur Verschlüsselung der Daten in einem Data Lake Store-Konto zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="fc109-3148">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="fc109-3149">Interactive</span><span class="sxs-lookup"><span data-stu-id="fc109-3149">Interactive</span></span>

* <span data-ttu-id="fc109-3150">Startzeit durch Verwendung zwischengespeicherter Befehle verbessert</span><span class="sxs-lookup"><span data-stu-id="fc109-3150">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="fc109-3151">Testabdeckung verbessert</span><span class="sxs-lookup"><span data-stu-id="fc109-3151">Increased test coverage</span></span>
* <span data-ttu-id="fc109-3152">?-Geste erweitert, sodass sie auch in den nächsten Befehl eingefügt wird</span><span class="sxs-lookup"><span data-stu-id="fc109-3152">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="fc109-3153">Interaktive Fehler mit dem Profil „2017-03-09-profile-preview“ behoben (3587)</span><span class="sxs-lookup"><span data-stu-id="fc109-3153">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="fc109-3154">`--version` als Parameter für den interaktiven Modus zugelassen (3645)</span><span class="sxs-lookup"><span data-stu-id="fc109-3154">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="fc109-3155">Beseitigung von Fehlern im interaktiven Modus beim Abschluss von Überprüfungen (3570)</span><span class="sxs-lookup"><span data-stu-id="fc109-3155">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="fc109-3156">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="fc109-3156">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="fc109-3157">Flag `--progress` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-3157">Added `--progress` flag</span></span>
* <span data-ttu-id="fc109-3158">`--debug` und `--verbose` aus Abschlüssen entfernt</span><span class="sxs-lookup"><span data-stu-id="fc109-3158">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="fc109-3159">`interactive` aus Abschlüssen entfernt (3324)</span><span class="sxs-lookup"><span data-stu-id="fc109-3159">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="fc109-3160">IoT</span><span class="sxs-lookup"><span data-stu-id="fc109-3160">IoT</span></span>

* <span data-ttu-id="fc109-3161">Behoben: Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="fc109-3161">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="fc109-3162">(3934)</span><span class="sxs-lookup"><span data-stu-id="fc109-3162">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="fc109-3163">Schlüsseltresor</span><span class="sxs-lookup"><span data-stu-id="fc109-3163">Key vault</span></span>

* <span data-ttu-id="fc109-3164">Befehle für Schlüsseltresor-Wiederherstellungsfeatures hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="fc109-3164">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="fc109-3165">`keyvault`-Unterbefehle: `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="fc109-3165">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="fc109-3166">`keyvault secret`-Unterbefehle: `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="fc109-3166">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="fc109-3167">`keyvault certificate`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="fc109-3167">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="fc109-3168">`keyvault key`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="fc109-3168">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="fc109-3169">Dienstprinzipal-Schlüsseltresorintegration hinzugefügt (3133)</span><span class="sxs-lookup"><span data-stu-id="fc109-3169">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="fc109-3170">Schlüsseltresor-Datenebene auf 0.3.2. aktualisiert</span><span class="sxs-lookup"><span data-stu-id="fc109-3170">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="fc109-3171">(3307)</span><span class="sxs-lookup"><span data-stu-id="fc109-3171">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="fc109-3172">Labor</span><span class="sxs-lookup"><span data-stu-id="fc109-3172">Lab</span></span>

* <span data-ttu-id="fc109-3173">Unterstützung für Übernahme eines beliebigen virtuellen Computers im Labor über `az lab vm claim` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-3173">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="fc109-3174">Tabellenausgabeformatierer für `az lab vm list` und `az lab vm show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-3174">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="fc109-3175">Überwachen</span><span class="sxs-lookup"><span data-stu-id="fc109-3175">Monitor</span></span>

* <span data-ttu-id="fc109-3176">Korrektur für Vorlagendatei mit Befehl `monitor autoscale-settings get-parameters-template` (3349)</span><span class="sxs-lookup"><span data-stu-id="fc109-3176">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="fc109-3177">`monitor alert-rule-incidents list` in `monitor alert list-incidents` umbenannt</span><span class="sxs-lookup"><span data-stu-id="fc109-3177">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="fc109-3178">`monitor alert-rule-incidents show` in `monitor alert show-incident` umbenannt</span><span class="sxs-lookup"><span data-stu-id="fc109-3178">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="fc109-3179">`monitor metric-defintions list` in `monitor metrics list-definitions` umbenannt</span><span class="sxs-lookup"><span data-stu-id="fc109-3179">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="fc109-3180">`monitor alert-rules` in `monitor alert` umbenannt</span><span class="sxs-lookup"><span data-stu-id="fc109-3180">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="fc109-3181">`monitor alert create` geändert:</span><span class="sxs-lookup"><span data-stu-id="fc109-3181">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="fc109-3182">Unterbefehle vom Typ `condition` und `action` akzeptieren keinen JSON-Code mehr.</span><span class="sxs-lookup"><span data-stu-id="fc109-3182">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="fc109-3183">Hinzufügung zahlreicher Parameter zur Vereinfachung der Regelerstellung</span><span class="sxs-lookup"><span data-stu-id="fc109-3183">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="fc109-3184">`location` nicht mehr erforderlich</span><span class="sxs-lookup"><span data-stu-id="fc109-3184">`location` no longer required</span></span>
  * <span data-ttu-id="fc109-3185">Hinzufügung von Namen- und ID-Unterstützung für Ziel</span><span class="sxs-lookup"><span data-stu-id="fc109-3185">Add name and ID support for target</span></span>
  * <span data-ttu-id="fc109-3186">Entfernung von `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="fc109-3186">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="fc109-3187">Umbenennung von `is-enabled` in `enabled` (nicht mehr erforderlich)</span><span class="sxs-lookup"><span data-stu-id="fc109-3187">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="fc109-3188">`description` wird nun abhängig von der angegebenen Bedingung auf einen Standardwert festgelegt.</span><span class="sxs-lookup"><span data-stu-id="fc109-3188">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="fc109-3189">Hinzufügung von Beispielen zur Verdeutlichung des neuen Formats</span><span class="sxs-lookup"><span data-stu-id="fc109-3189">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="fc109-3190">Unterstützung von Namen oder IDs für Befehle vom Typ `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="fc109-3190">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="fc109-3191">Komfortargumente und Beispiele zu `monitor alert rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-3191">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="fc109-3192">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="fc109-3192">Network</span></span>

* <span data-ttu-id="fc109-3193">Befehl `list-private-access-services` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-3193">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="fc109-3194">Argument `--private-access-services` zu `vnet subnet create` und `vnet subnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-3194">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="fc109-3195">Problem behoben, das einen Fehler für `application-gateway redirect-config create` zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="fc109-3195">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="fc109-3196">Problem behoben, aufgrund dessen `application-gateway redirect-config update` nicht mit `--no-wait` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="fc109-3196">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="fc109-3197">Fehler behoben, der bei der Verwendung des Arguments `--servers` mit `application-gateway address-pool create` und `application-gateway address-pool update` aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="fc109-3197">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="fc109-3198">Befehle vom Typ `application-gateway redirect-config` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-3198">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="fc109-3199">Befehle zu `application-gateway ssl-policy` hinzugefügt: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="fc109-3199">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="fc109-3200">Argumente zu `application-gateway ssl-policy set` hinzugefügt: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="fc109-3200">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="fc109-3201">Argumente zu `application-gateway http-settings create` und `application-gateway http-settings update` hinzugefügt: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="fc109-3201">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="fc109-3202">Argumente zu `application-gateway url-path-map create` und `application-gateway url-path-map update` hinzugefügt: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="fc109-3202">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="fc109-3203">Argument `--redirect-config` zu `application-gateway url-path-map rule create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-3203">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="fc109-3204">Unterstützung für `--no-wait` zu `application-gateway url-path-map rule delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-3204">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="fc109-3205">Argumente zu `application-gateway probe create` und `application-gateway probe update` hinzugefügt: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="fc109-3205">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="fc109-3206">Argument `--redirect-config` zu `application-gateway rule create` und `application-gateway rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-3206">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="fc109-3207">Unterstützung für `--accelerated-networking` zu `nic create` und `nic update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-3207">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="fc109-3208">Argument `--internal-dns-name-suffix` von `nic create` entfernt</span><span class="sxs-lookup"><span data-stu-id="fc109-3208">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="fc109-3209">Unterstützung für `--dns-servers` zu `nic update` und `nic create` hinzugefügt: Hinzufügung von Unterstützung für --dns-servers</span><span class="sxs-lookup"><span data-stu-id="fc109-3209">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="fc109-3210">Fehler korrigiert, aufgrund dessen `--local-address-prefixes` von `local-gateway create` ignoriert wurde</span><span class="sxs-lookup"><span data-stu-id="fc109-3210">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="fc109-3211">Unterstützung für `--dns-servers` zu `vnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-3211">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="fc109-3212">Fehler beim Erstellen eines Peerings ohne Routenfilterung mit `express-route peering create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="fc109-3212">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="fc109-3213">Fehler korrigiert, aufgrund dessen die Argumente `--provider` und `--bandwidth` nicht mit `express-route update` verwendet werden konnten</span><span class="sxs-lookup"><span data-stu-id="fc109-3213">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="fc109-3214">Fehler mit Standardlogik von `network watcher show-topology` korrigiert</span><span class="sxs-lookup"><span data-stu-id="fc109-3214">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="fc109-3215">Ausgabeformatierung für `network list-usages` verbessert</span><span class="sxs-lookup"><span data-stu-id="fc109-3215">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="fc109-3216">Verwendung der standardmäßigen Front-End-IP-Adresse für `application-gateway http-listener create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="fc109-3216">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="fc109-3217">Verwendung des Standardadresspools, der HTTP-Standardeinstellungen und des HTTP-Standardlisteners für `application-gateway rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="fc109-3217">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="fc109-3218">Verwendung der standardmäßigen Front-End-IP-Adresse und des standardmäßigen Back-End-Pools für `lb rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="fc109-3218">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="fc109-3219">Verwendung der standardmäßigen Front-End-IP-Adresse für `lb inbound-nat-rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="fc109-3219">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="fc109-3220">Profil</span><span class="sxs-lookup"><span data-stu-id="fc109-3220">Profile</span></span>

* <span data-ttu-id="fc109-3221">Unterstützung der Anmeldung innerhalb eines virtuellen Computers mit einer verwalteten Identität</span><span class="sxs-lookup"><span data-stu-id="fc109-3221">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="fc109-3222">Unterstützung der Ausgabe für `account show` im SDK-Authentifizierungsdateiformat</span><span class="sxs-lookup"><span data-stu-id="fc109-3222">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="fc109-3223">Anzeige von Warnungen für veraltete Befehle bei Verwendung von „--expanded-view“</span><span class="sxs-lookup"><span data-stu-id="fc109-3223">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="fc109-3224">Befehl `get-access-token` für die Bereitstellung eines unformatierten AAD-Tokens hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-3224">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="fc109-3225">Unterstützung der Anmeldung mit einem Benutzerkonto ohne zugeordnete Abonnements</span><span class="sxs-lookup"><span data-stu-id="fc109-3225">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="fc109-3226">RDBMS</span><span class="sxs-lookup"><span data-stu-id="fc109-3226">RDBMS</span></span>

* <span data-ttu-id="fc109-3227">Unterstützung der abonnementübergreifenden Auflistung von Servern (3417)</span><span class="sxs-lookup"><span data-stu-id="fc109-3227">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="fc109-3228">Behoben: `%s` wird aufgrund von fehlendem `% server_type` nicht verarbeitet (3393)</span><span class="sxs-lookup"><span data-stu-id="fc109-3228">Fixed `%s` not processed because of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="fc109-3229">Dokumentquellenzuordnung behoben und CI-Aufgabe zur Überprüfung hinzugefügt (3361)</span><span class="sxs-lookup"><span data-stu-id="fc109-3229">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="fc109-3230">MySQL- und PostgreSQL-Hilfe korrigiert (3369)</span><span class="sxs-lookup"><span data-stu-id="fc109-3230">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="fc109-3231">Resource</span><span class="sxs-lookup"><span data-stu-id="fc109-3231">Resource</span></span>

* <span data-ttu-id="fc109-3232">Eingabeaufforderungen bei fehlenden Parametern für `group deployment create` verbessert</span><span class="sxs-lookup"><span data-stu-id="fc109-3232">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="fc109-3233">Analyse der Syntax `--parameters KEY=VALUE` verbessert</span><span class="sxs-lookup"><span data-stu-id="fc109-3233">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="fc109-3234">Probleme behoben, durch die Parameterdateien von `group deployment create` bei Verwendung der Syntax `@<file>` nicht mehr erkannt wurden</span><span class="sxs-lookup"><span data-stu-id="fc109-3234">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="fc109-3235">Unterstützung des Arguments `--ids` für Befehle vom Typ `resource` und `managedapp`</span><span class="sxs-lookup"><span data-stu-id="fc109-3235">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="fc109-3236">Einige Analyse- und Fehlermeldungen korrigiert (3584)</span><span class="sxs-lookup"><span data-stu-id="fc109-3236">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="fc109-3237">Analyse vom Typ `--resource-type` für den Befehl `lock` korrigiert, sodass `<resource-namespace>` und `<resource-type>` akzeptiert werden</span><span class="sxs-lookup"><span data-stu-id="fc109-3237">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="fc109-3238">Parameterüberprüfung für Vorlagenlinkvorlagen hinzugefügt (3629)</span><span class="sxs-lookup"><span data-stu-id="fc109-3238">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="fc109-3239">Unterstützung für die Angabe von Bereitstellungsparametern mit der Syntax `KEY=VALUE` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-3239">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="fc109-3240">Role</span><span class="sxs-lookup"><span data-stu-id="fc109-3240">Role</span></span>

* <span data-ttu-id="fc109-3241">Unterstützung der Ausgabe im SDK-Authentifizierungsdateiformat für `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="fc109-3241">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="fc109-3242">Rollenzuweisungen und dazugehörige AAD-Anwendung beim Löschen eines Dienstprinzipals bereinigt (3610)</span><span class="sxs-lookup"><span data-stu-id="fc109-3242">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="fc109-3243">Einbeziehung des Zeitformats in Beschreibungen vom Typ `--start-date` und `--end-date` für `app create`-Argumente</span><span class="sxs-lookup"><span data-stu-id="fc109-3243">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="fc109-3244">Anzeige von Warnungen für veraltete Befehle bei Verwendung von `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="fc109-3244">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="fc109-3245">Schlüsseltresorintegration zu den Befehlen `create-for-rbac` und `reset-credentials` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-3245">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="fc109-3246">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="fc109-3246">Service Fabric</span></span>
* <span data-ttu-id="fc109-3247">Problem behoben, aufgrund dessen große Dateien in Anwendungen beim Hochladen gekürzt wurden (3666)</span><span class="sxs-lookup"><span data-stu-id="fc109-3247">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="fc109-3248">Tests für Service Fabric-Befehle hinzugefügt (3424)</span><span class="sxs-lookup"><span data-stu-id="fc109-3248">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="fc109-3249">Zahlreiche Service Fabric-Befehle korrigiert (3234)</span><span class="sxs-lookup"><span data-stu-id="fc109-3249">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="fc109-3250">SQL</span><span class="sxs-lookup"><span data-stu-id="fc109-3250">SQL</span></span>

* <span data-ttu-id="fc109-3251">Fehlerhafte1 Parameter `--identity` für `sql server create` entfernt</span><span class="sxs-lookup"><span data-stu-id="fc109-3251">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="fc109-3252">Kennwortwerte aus der Befehlsausgabe von `sql server create` und `sql server update` entfernt</span><span class="sxs-lookup"><span data-stu-id="fc109-3252">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="fc109-3253">Befehle `sql db list-editions` und `sql elastic-pool list-editions` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-3253">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="fc109-3254">Storage</span><span class="sxs-lookup"><span data-stu-id="fc109-3254">Storage</span></span>

* <span data-ttu-id="fc109-3255">Option `--marker` für die Befehle `storage blob list`, `storage container list` und `storage share list` entfernt (3745)</span><span class="sxs-lookup"><span data-stu-id="fc109-3255">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="fc109-3256">Erstellung eines reinen HTTPS-Speicherkontos ermöglicht</span><span class="sxs-lookup"><span data-stu-id="fc109-3256">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="fc109-3257">Speichermetriken, Protokollierung und CORS-Befehle aktualisiert (3495)</span><span class="sxs-lookup"><span data-stu-id="fc109-3257">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="fc109-3258">Ausnahmemeldung von „cors add“ umformuliert (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="fc109-3258">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="fc109-3259">Generator im Probelaufmodus des Downloadbatchbefehls in eine Liste konvertiert (3592)</span><span class="sxs-lookup"><span data-stu-id="fc109-3259">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="fc109-3260">Problem bei Probelauf des Blobdownloadbatchs behoben (3640) (3592)</span><span class="sxs-lookup"><span data-stu-id="fc109-3260">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="fc109-3261">VM</span><span class="sxs-lookup"><span data-stu-id="fc109-3261">VM</span></span>

* <span data-ttu-id="fc109-3262">Unterstützung der NSG-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="fc109-3262">Support configuring nsg</span></span>
* <span data-ttu-id="fc109-3263">Fehler behoben, aufgrund dessen der DNS-Server nicht ordnungsgemäß konfiguriert wurde</span><span class="sxs-lookup"><span data-stu-id="fc109-3263">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="fc109-3264">Unterstützung verwalteter Dienstidentitäten</span><span class="sxs-lookup"><span data-stu-id="fc109-3264">Support managed service identities</span></span>
* <span data-ttu-id="fc109-3265">Problem behoben, aufgrund dessen `cmss create` mit einem vorhandenen Lastenausgleich `--backend-pool-name` benötigte</span><span class="sxs-lookup"><span data-stu-id="fc109-3265">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="fc109-3266">Festlegung, dass die LUN von mit `vm image create` erstellten Datenträgern mit 0 beginnt</span><span class="sxs-lookup"><span data-stu-id="fc109-3266">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="fc109-3267">10. Mai 2017</span><span class="sxs-lookup"><span data-stu-id="fc109-3267">May 10, 2017</span></span>

<span data-ttu-id="fc109-3268">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="fc109-3268">Version 2.0.6</span></span>

* <span data-ttu-id="fc109-3269">Umbenennen von „documentdb“ in „cosmosdb“</span><span class="sxs-lookup"><span data-stu-id="fc109-3269">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="fc109-3270">Hinzufügen von rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="fc109-3270">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="fc109-3271">Einbeziehen der Data Lake Analytics- und Data Lake Store-Module</span><span class="sxs-lookup"><span data-stu-id="fc109-3271">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="fc109-3272">Einbeziehen des Cognitive Services-Moduls</span><span class="sxs-lookup"><span data-stu-id="fc109-3272">Include Cognitive Services module</span></span>
* <span data-ttu-id="fc109-3273">Einbeziehen des Service Fabric-Moduls</span><span class="sxs-lookup"><span data-stu-id="fc109-3273">Include Service Fabric module</span></span>
* <span data-ttu-id="fc109-3274">Einbeziehen des interaktiven Moduls (Umbenennen von „az-shell“)</span><span class="sxs-lookup"><span data-stu-id="fc109-3274">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="fc109-3275">Hinzufügen von Unterstützung für CDN-Befehle</span><span class="sxs-lookup"><span data-stu-id="fc109-3275">Add support for CDN commands</span></span>
* <span data-ttu-id="fc109-3276">Entfernen des Containermoduls</span><span class="sxs-lookup"><span data-stu-id="fc109-3276">Remove Container module</span></span>
* <span data-ttu-id="fc109-3277">Hinzufügen von „az -v“ als Verknüpfung für „az --version“ ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="fc109-3277">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="fc109-3278">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="fc109-3278">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="fc109-3279">Core</span><span class="sxs-lookup"><span data-stu-id="fc109-3279">Core</span></span>

* <span data-ttu-id="fc109-3280">Core: Erfassen von Ausnahmen, die durch einen nicht registrierten Anbieter verursacht werden, und automatische Registrierung</span><span class="sxs-lookup"><span data-stu-id="fc109-3280">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="fc109-3281">Leistung: Dauerhaftes Speichern des ADAL-Tokencaches im Arbeitsspeicher bis zum Prozessende ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="fc109-3281">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="fc109-3282">Korrigieren der vom hexadezimalen Fingerabdruck -o tsv zurückgegebenen Bytes ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="fc109-3282">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="fc109-3283">Verbessern des Downloads des Schlüsseltresorzertifikats und der AAD-SP-Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="fc109-3283">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="fc109-3284">Hinzufügen des Python-Speicherorts zu „az –version“ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="fc109-3284">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="fc109-3285">Anmeldung: Unterstützung der Anmeldung, wenn keine Abonnements vorhanden sind ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="fc109-3285">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="fc109-3286">Core: Beheben eines Fehlers bei zweimaliger Verwendung eines Dienstprinzipals bei der Anmeldung ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="fc109-3286">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="fc109-3287">Core: Ermöglichen der Konfiguration des Dateipfads von „accessTokens.json“ über eine Umgebungsvariable ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="fc109-3287">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="fc109-3288">Core: Zulassen der Anwendung konfigurierter Standardwerte auf optionale Argumente ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="fc109-3288">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="fc109-3289">Core: Verbesserte Leistung</span><span class="sxs-lookup"><span data-stu-id="fc109-3289">core: Improved performance</span></span>
* <span data-ttu-id="fc109-3290">Core: Zertifikate von benutzerdefinierter Zertifizierungsstelle – Unterstützung für das Festlegen der REQUESTS_CA_BUNDLE-Umgebungsvariablen</span><span class="sxs-lookup"><span data-stu-id="fc109-3290">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="fc109-3291">Core: Cloudkonfiguration – Verwenden des Endpunkts „resource manager“, wenn Endpunkt „management“ nicht festgelegt ist</span><span class="sxs-lookup"><span data-stu-id="fc109-3291">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="fc109-3292">ACS</span><span class="sxs-lookup"><span data-stu-id="fc109-3292">ACS</span></span>

* <span data-ttu-id="fc109-3293">Korrigieren der Master- und Agentanzahl als ganze Zahl statt Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fc109-3293">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="fc109-3294">Verfügbarmachen von „az acs create --no-wait“ und „az acs wait“ für die asynchrone Erstellung</span><span class="sxs-lookup"><span data-stu-id="fc109-3294">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="fc109-3295">Verfügbarmachen von „az acs create --validate“ für Probelaufüberprüfungen</span><span class="sxs-lookup"><span data-stu-id="fc109-3295">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="fc109-3296">Entfernen von Windows-Profil vor PUT-Aufruf für Skalierungsbefehl ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="fc109-3296">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="fc109-3297">AppService</span><span class="sxs-lookup"><span data-stu-id="fc109-3297">AppService</span></span>

* <span data-ttu-id="fc109-3298">functionapp: Hinzufügen der vollständigen functionapp-Unterstützung, einschließlich Erstellen, Anzeigen, Auflisten, Löschen, Hostname, SSL usw.</span><span class="sxs-lookup"><span data-stu-id="fc109-3298">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="fc109-3299">Hinzufügen von Team Services (vsts) als Continuous Delivery-Option zu „appservice web source-control config“</span><span class="sxs-lookup"><span data-stu-id="fc109-3299">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="fc109-3300">Erstellen von „az webapp“ als Ersatz für „az appservice web“ (für Abwärtskompatibilität bleibt „az appservice web“ für 2 weitere Releases erhalten)</span><span class="sxs-lookup"><span data-stu-id="fc109-3300">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="fc109-3301">Verfügbarmachen von Argumenten zum Konfigurieren von Bereitstellung und Laufzeitstapeln beim Erstellen von Web-Apps</span><span class="sxs-lookup"><span data-stu-id="fc109-3301">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="fc109-3302">Verfügbarmachen von „webapp list-runtimes“</span><span class="sxs-lookup"><span data-stu-id="fc109-3302">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="fc109-3303">Unterstützen der Konfiguration von Verbindungszeichenfolgen ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="fc109-3303">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="fc109-3304">Unterstützen des Slottauschs mit Vorschau</span><span class="sxs-lookup"><span data-stu-id="fc109-3304">support slot swap with preview</span></span>
* <span data-ttu-id="fc109-3305">Beheben von Fehlern in appservice-Befehlen ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="fc109-3305">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="fc109-3306">Verwenden der Ressourcengruppe des App Service-Plans für Zertifizierungsvorgänge ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="fc109-3306">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="fc109-3307">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="fc109-3307">CosmosDB</span></span>

* <span data-ttu-id="fc109-3308">Umbenennen des documentdb-Moduls in cosmosdb</span><span class="sxs-lookup"><span data-stu-id="fc109-3308">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="fc109-3309">Zusätzliche Unterstützung für documentdb-APIs auf Datenebene: Datenbank- und Sammlungsverwaltung</span><span class="sxs-lookup"><span data-stu-id="fc109-3309">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="fc109-3310">Zusätzliche Unterstützung für das Aktivieren des automatischen Failovers für Datenbankkonten</span><span class="sxs-lookup"><span data-stu-id="fc109-3310">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="fc109-3311">Zusätzliche Unterstützung für die neue ConsistentPrefix-Konsistenzrichtlinie</span><span class="sxs-lookup"><span data-stu-id="fc109-3311">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="fc109-3312">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="fc109-3312">Data Lake Analytics</span></span>

* <span data-ttu-id="fc109-3313">Beheben eines Fehlers, bei dem das Filtern von Auftragslisten nach Ergebnis und Status einen Fehler auslöst</span><span class="sxs-lookup"><span data-stu-id="fc109-3313">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="fc109-3314">Hinzufügen von Unterstützung für den neuen Katalogelementtyp „Paket“</span><span class="sxs-lookup"><span data-stu-id="fc109-3314">Add support for new catalog item type: package.</span></span> <span data-ttu-id="fc109-3315">Zugriff über: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="fc109-3315">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="fc109-3316">Ermöglichen der Auflistung folgender Katalogelemente innerhalb einer Datenbank (keine Schemaspezifikation erforderlich):</span><span class="sxs-lookup"><span data-stu-id="fc109-3316">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="fc109-3317">Tabelle</span><span class="sxs-lookup"><span data-stu-id="fc109-3317">Table</span></span>
  * <span data-ttu-id="fc109-3318">Tabellenwertfunktion</span><span class="sxs-lookup"><span data-stu-id="fc109-3318">Table valued function</span></span>
  * <span data-ttu-id="fc109-3319">Sicht</span><span class="sxs-lookup"><span data-stu-id="fc109-3319">View</span></span>
  * <span data-ttu-id="fc109-3320">Tabellenstatistiken.</span><span class="sxs-lookup"><span data-stu-id="fc109-3320">Table Statistics.</span></span> <span data-ttu-id="fc109-3321">Können auch mit einem Schema, jedoch ohne Angabe eines Tabellennamens aufgelistet werden.</span><span class="sxs-lookup"><span data-stu-id="fc109-3321">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="fc109-3322">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="fc109-3322">Data Lake Store</span></span>

* <span data-ttu-id="fc109-3323">Aktualisieren der Version des zugrunde liegenden Dateisystem-SDK, wodurch eine bessere Unterstützung für die Verarbeitung von Drosselungsszenarien auf Serverseite gewährt wird</span><span class="sxs-lookup"><span data-stu-id="fc109-3323">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="fc109-3324">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="fc109-3324">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="fc109-3325">Fehlende Hilfe für Zugriffsanzeige</span><span class="sxs-lookup"><span data-stu-id="fc109-3325">missed help for access show.</span></span> <span data-ttu-id="fc109-3326">hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="fc109-3326">adding it.</span></span> <span data-ttu-id="fc109-3327">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="fc109-3327">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="fc109-3328">Suchen</span><span class="sxs-lookup"><span data-stu-id="fc109-3328">Find</span></span>

* <span data-ttu-id="fc109-3329">Verbessern von Suchergebnissen und Ermöglichen der Versionsverwaltung des Suchindex</span><span class="sxs-lookup"><span data-stu-id="fc109-3329">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="fc109-3330">KeyVault</span><span class="sxs-lookup"><span data-stu-id="fc109-3330">KeyVault</span></span>

* <span data-ttu-id="fc109-3331">BC:`az keyvault certificate download` Ändern von „-e“ von Zeichenfolge oder Binärdatentyp in PEM oder DER zur besseren Darstellung der Optionen</span><span class="sxs-lookup"><span data-stu-id="fc109-3331">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="fc109-3332">BC: Entfernen von „--expires“ und „--not-before“ aus `keyvault certificate create`, da diese Parameter nicht vom Dienst unterstützt werden</span><span class="sxs-lookup"><span data-stu-id="fc109-3332">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="fc109-3333">Hinzufügen des Parameters „--validity“ zu `keyvault certificate create`, um gezielt den Wert in „--policy“ zu überschreiben</span><span class="sxs-lookup"><span data-stu-id="fc109-3333">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="fc109-3334">Beheben des Problems in `keyvault certificate get-default-policy`, bei dem „expires“ und „not_before“ verfügbar gemacht wurden, „validity_in_months“ hingegen nicht</span><span class="sxs-lookup"><span data-stu-id="fc109-3334">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="fc109-3335">Keyvault-Korrektur für den Import von PEM und PFX ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="fc109-3335">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="fc109-3336">Labor</span><span class="sxs-lookup"><span data-stu-id="fc109-3336">Lab</span></span>

* <span data-ttu-id="fc109-3337">Hinzufügen der Befehle „create“, „show“, „delete“ und „list“ für die Laborumgebung</span><span class="sxs-lookup"><span data-stu-id="fc109-3337">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="fc109-3338">Hinzufügen der Befehle „show“ und „list“ zur Anzeige von ARM-Vorlagen im Labor</span><span class="sxs-lookup"><span data-stu-id="fc109-3338">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="fc109-3339">Hinzufügen des Kennzeichens „--environment“ in `az lab vm list`, um virtuelle Computer nach Umgebung im Labor zu filtern</span><span class="sxs-lookup"><span data-stu-id="fc109-3339">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="fc109-3340">Hinzufügen des benutzerfreundlichen Befehls `az lab formula export-artifacts` zum Exportieren des Artefaktgerüsts innerhalb der Formel eines Labors</span><span class="sxs-lookup"><span data-stu-id="fc109-3340">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="fc109-3341">Hinzufügen von Befehlen zum Verwalten von Geheimnissen in einem Labor</span><span class="sxs-lookup"><span data-stu-id="fc109-3341">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="fc109-3342">Überwachen</span><span class="sxs-lookup"><span data-stu-id="fc109-3342">Monitor</span></span>

* <span data-ttu-id="fc109-3343">Fehlerbehebung: Modellieren von `--actions` von `az alert-rules create` zum Verarbeiten von JSON-Zeichenfolgen ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="fc109-3343">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="fc109-3344">Programmfehlerbehebung: Beim Erstellen von Diagnoseeinstellungen werden Protokolle/Metriken aus Anzeigebefehlen nicht akzeptiert ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="fc109-3344">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="fc109-3345">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="fc109-3345">Network</span></span>

* <span data-ttu-id="fc109-3346">Hinzufügen des `network watcher test-connectivity`-Befehls</span><span class="sxs-lookup"><span data-stu-id="fc109-3346">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="fc109-3347">Hinzufügen von Unterstützung für den `--filters`-Parameter für `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="fc109-3347">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="fc109-3348">Hinzufügen von Unterstützung für den Application Gateway-Verbindungsausgleich</span><span class="sxs-lookup"><span data-stu-id="fc109-3348">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="fc109-3349">Hinzufügen von Unterstützung für die Konfiguration von Application Gateway-WAF-Regelsätzen</span><span class="sxs-lookup"><span data-stu-id="fc109-3349">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="fc109-3350">Hinzufügen von Unterstützung für ExpressRoute-Routenfilter und -Regeln</span><span class="sxs-lookup"><span data-stu-id="fc109-3350">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="fc109-3351">Hinzufügen von Unterstützung für geografisches TrafficManager-Routing</span><span class="sxs-lookup"><span data-stu-id="fc109-3351">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="fc109-3352">Hinzufügen von Unterstützung für richtlinienbasierte Datenverkehrsselektoren für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="fc109-3352">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="fc109-3353">Hinzufügen von Unterstützung für IPSec-Richtlinien für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="fc109-3353">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="fc109-3354">Korrektur eines Fehlers bei `vpn-connection create` bei Verwendung der Parameter `--no-wait` oder `--validate`</span><span class="sxs-lookup"><span data-stu-id="fc109-3354">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="fc109-3355">Hinzufügen von Unterstützung für Aktiv/Aktiv-VNET-Gateways</span><span class="sxs-lookup"><span data-stu-id="fc109-3355">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="fc109-3356">Entfernen von NULL-Werten aus der Ausgabe von `network vpn-connection list/show`-Befehlen</span><span class="sxs-lookup"><span data-stu-id="fc109-3356">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="fc109-3357">BC: Korrektur eines Fehlers in der Ausgabe von `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="fc109-3357">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="fc109-3358">Korrektur eines Fehlers, bei dem das Argument „--key-length“ von „vpn-connection create“ nicht ordnungsgemäß analysiert wurde</span><span class="sxs-lookup"><span data-stu-id="fc109-3358">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="fc109-3359">Korrektur eines Fehlers in `dns zone import`, bei dem Datensätze nicht ordnungsgemäß importiert wurden</span><span class="sxs-lookup"><span data-stu-id="fc109-3359">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="fc109-3360">Korrektur eines Fehlers, bei dem `traffic-manager endpoint update` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="fc109-3360">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="fc109-3361">Hinzufügen von Network Watcher-Vorschaubefehlen</span><span class="sxs-lookup"><span data-stu-id="fc109-3361">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="fc109-3362">Profil</span><span class="sxs-lookup"><span data-stu-id="fc109-3362">Profile</span></span>

* <span data-ttu-id="fc109-3363">Unterstützung der Anmeldung, wenn keine Abonnements gefunden werden ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="fc109-3363">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="fc109-3364">Unterstützung für kurze Parameternamen in „az account set --subscription“ ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="fc109-3364">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="fc109-3365">Redis</span><span class="sxs-lookup"><span data-stu-id="fc109-3365">Redis</span></span>

* <span data-ttu-id="fc109-3366">Hinzufügen des Updatebefehls, durch den auch die Möglichkeit zum Skalieren für Redis Cache hinzugefügt wird</span><span class="sxs-lookup"><span data-stu-id="fc109-3366">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="fc109-3367">Verwerfen des Befehls „update-settings“</span><span class="sxs-lookup"><span data-stu-id="fc109-3367">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="fc109-3368">Resource</span><span class="sxs-lookup"><span data-stu-id="fc109-3368">Resource</span></span>

* <span data-ttu-id="fc109-3369">Hinzufügen der Befehle „managedapp“ und „managedapp definition“ ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="fc109-3369">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="fc109-3370">Unterstützung für die „provider operation“-Befehle ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="fc109-3370">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="fc109-3371">Unterstützung für die Erstellung generischer Ressourcen ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="fc109-3371">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="fc109-3372">Korrigieren der Ressourcenanalyse und der API-Versionssuche</span><span class="sxs-lookup"><span data-stu-id="fc109-3372">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="fc109-3373">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="fc109-3373">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="fc109-3374">Hinzufügen von Dokumenten für „az lock update“</span><span class="sxs-lookup"><span data-stu-id="fc109-3374">Add docs for az lock update.</span></span> <span data-ttu-id="fc109-3375">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="fc109-3375">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="fc109-3376">Beenden mit Fehler bei dem Versuch, Ressourcen für eine nicht vorhandene Gruppe aufzulisten</span><span class="sxs-lookup"><span data-stu-id="fc109-3376">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="fc109-3377">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="fc109-3377">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="fc109-3378">[Compute] Beheben von Problemen mit dem Update von VMSS- und VM-Verfügbarkeitsgruppen</span><span class="sxs-lookup"><span data-stu-id="fc109-3378">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="fc109-3379">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="fc109-3379">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="fc109-3380">Korrigieren des Erstellungs- und Löschvorgangs für Sperren, wenn „parent-resource-path“ auf „None“ festgelegt ist ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="fc109-3380">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="fc109-3381">Role</span><span class="sxs-lookup"><span data-stu-id="fc109-3381">Role</span></span>

* <span data-ttu-id="fc109-3382">create-for-rbac: Sicherstellen, dass das SP-Enddatum nicht das Ablaufdatum des Zertifikats überschreitet ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="fc109-3382">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="fc109-3383">RBAC: Hinzufügen vollständiger Unterstützung für „ad group“ ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="fc109-3383">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="fc109-3384">Rolle: Beheben von Probleme beim Rollendefinitionsupdate ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="fc109-3384">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="fc109-3385">create-for-rbac: Sicherstellen, dass das angegebene Benutzerkennwort übernommen wird</span><span class="sxs-lookup"><span data-stu-id="fc109-3385">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="fc109-3386">SQL</span><span class="sxs-lookup"><span data-stu-id="fc109-3386">SQL</span></span>

* <span data-ttu-id="fc109-3387">Hinzufügen der Befehle „az sql server list-usages“ und „az sql db list-usages“</span><span class="sxs-lookup"><span data-stu-id="fc109-3387">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="fc109-3388">SQL: Möglichkeit zur direkten Verbindung mit Ressourcenanbieter ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="fc109-3388">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="fc109-3389">Storage</span><span class="sxs-lookup"><span data-stu-id="fc109-3389">Storage</span></span>

* <span data-ttu-id="fc109-3390">Festlegen des Ressourcengruppenstandorts als Standardstandort für `storage account create`</span><span class="sxs-lookup"><span data-stu-id="fc109-3390">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="fc109-3391">Hinzufügen von Unterstützung für das inkrementelle Kopieren von Blobs</span><span class="sxs-lookup"><span data-stu-id="fc109-3391">Add support for incremental blob copy</span></span>
* <span data-ttu-id="fc109-3392">Hinzufügen von Unterstützung für den Upload umfangreicher Blockblobs</span><span class="sxs-lookup"><span data-stu-id="fc109-3392">Add support for large block blob upload</span></span>
* <span data-ttu-id="fc109-3393">Ändern der Blockgröße auf 100 MB, wenn die hochzuladende Datei größer als 200 GB ist</span><span class="sxs-lookup"><span data-stu-id="fc109-3393">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="fc109-3394">VM</span><span class="sxs-lookup"><span data-stu-id="fc109-3394">VM</span></span>

* <span data-ttu-id="fc109-3395">avail-set: Festlegen der UD- und FD-Domänenanzahl als optional</span><span class="sxs-lookup"><span data-stu-id="fc109-3395">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="fc109-3396">Hinweis: VM-Befehle in unabhängigen Clouds: Vermeiden Sie Features im Zusammenhang mit verwalteten Datenträgern, einschließlich der folgenden:</span><span class="sxs-lookup"><span data-stu-id="fc109-3396">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="fc109-3397">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="fc109-3397">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="fc109-3398">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="fc109-3398">az vm/vmss disk</span></span>
  3. <span data-ttu-id="fc109-3399">Verwenden Sie in „az vm/vmss create“ den Befehl „—use-unmanaged-disk“, um verwaltete Datenträger zu vermeiden. Andere Befehle sollten funktionieren.</span><span class="sxs-lookup"><span data-stu-id="fc109-3399">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="fc109-3400">vm/vmss: Verbessern des Warnungstexts beim Generieren von SSH-Schlüsselpaaren</span><span class="sxs-lookup"><span data-stu-id="fc109-3400">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="fc109-3401">vm/vmss: Unterstützen der Erstellung über ein Marketplace-Image, für das Planinformationen erforderlich sind ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="fc109-3401">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="fc109-3402">3\. April 2017</span><span class="sxs-lookup"><span data-stu-id="fc109-3402">April 3, 2017</span></span>

<span data-ttu-id="fc109-3403">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="fc109-3403">Version 2.0.2</span></span>

<span data-ttu-id="fc109-3404">In dieser Version wurden die Komponenten ACR, Batch, KeyVault und SQL eingeführt.</span><span class="sxs-lookup"><span data-stu-id="fc109-3404">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="fc109-3405">Core</span><span class="sxs-lookup"><span data-stu-id="fc109-3405">Core</span></span>

* <span data-ttu-id="fc109-3406">Hinzufügen der Module „acr“, „lab“, „monitor“ und „find“ zur Standardliste</span><span class="sxs-lookup"><span data-stu-id="fc109-3406">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="fc109-3407">Anmeldung: Überspringen des fehlerhaften Mandanten ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="fc109-3407">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="fc109-3408">Anmeldung: Festlegen des Standardabonnements auf ein Abonnement mit dem Status „Enabled“ ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="fc109-3408">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="fc109-3409">Hinzufügen von wait-Befehlen und Unterstützung von „--no-wait“ für mehr Befehle ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="fc109-3409">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="fc109-3410">Core: Unterstützen der Anmeldung per Dienstprinzipal mit einem Zertifikat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="fc109-3410">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="fc109-3411">Hinzufügen der Meldung zu fehlenden Vorlagenparametern</span><span class="sxs-lookup"><span data-stu-id="fc109-3411">Add prompting for missing template parameters.</span></span> <span data-ttu-id="fc109-3412">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="fc109-3412">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="fc109-3413">Unterstützen des Festlegens von Standardwerten für häufig verwendete Argumente, z.B. Standardressourcengruppe, Standardweb und Standard-VM</span><span class="sxs-lookup"><span data-stu-id="fc109-3413">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="fc109-3414">Unterstützen der Anmeldung an einem bestimmten Mandanten</span><span class="sxs-lookup"><span data-stu-id="fc109-3414">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="fc109-3415">ACS</span><span class="sxs-lookup"><span data-stu-id="fc109-3415">ACS</span></span>

* <span data-ttu-id="fc109-3416">[ACS] Hinzufügen von Unterstützung für die Konfiguration eines ACS-Standardclusters ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="fc109-3416">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="fc109-3417">Hinzufügen von Unterstützung der Aufforderung zur Kennworteingabe für SSH-Schlüssel</span><span class="sxs-lookup"><span data-stu-id="fc109-3417">Add support for ssh key password prompting.</span></span> <span data-ttu-id="fc109-3418">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="fc109-3418">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="fc109-3419">Hinzufügen von Unterstützung für Windows-Cluster</span><span class="sxs-lookup"><span data-stu-id="fc109-3419">Add support for windows clusters.</span></span> <span data-ttu-id="fc109-3420">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="fc109-3420">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="fc109-3421">Wechseln von der Rolle „Besitzer“ zur Rolle „Mitwirkender“</span><span class="sxs-lookup"><span data-stu-id="fc109-3421">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="fc109-3422">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="fc109-3422">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="fc109-3423">AppService</span><span class="sxs-lookup"><span data-stu-id="fc109-3423">AppService</span></span>

* <span data-ttu-id="fc109-3424">appservice: Unterstützung für das Abrufen der externen IP-Adresse für DNS A-Einträge ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="fc109-3424">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="fc109-3425">appservice: Unterstützung der Bindung von Platzhalterzertifikaten ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="fc109-3425">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="fc109-3426">appservice: Unterstützung von Veröffentlichungsprofilen für Listen ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="fc109-3426">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="fc109-3427">AppService: Auslösen der Synchronisierung der Quellcodeverwaltung nach der Konfiguration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="fc109-3427">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="fc109-3428">DataLake</span><span class="sxs-lookup"><span data-stu-id="fc109-3428">DataLake</span></span>

* <span data-ttu-id="fc109-3429">Erste Version des Data Lake Analytics-Moduls</span><span class="sxs-lookup"><span data-stu-id="fc109-3429">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="fc109-3430">Erste Version des Data Lake Store-Moduls</span><span class="sxs-lookup"><span data-stu-id="fc109-3430">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="fc109-3431">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="fc109-3431">DocuemntDB</span></span>

* <span data-ttu-id="fc109-3432">DocumentDB: Hinzufügen von Unterstützung für das Auflisten von Verbindungszeichenfolgen ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="fc109-3432">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="fc109-3433">VM</span><span class="sxs-lookup"><span data-stu-id="fc109-3433">VM</span></span>

* <span data-ttu-id="fc109-3434">[Compute] Hinzufügen von AppGateway-Unterstützung für Erstellung von VM-Skalierungsgruppen ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="fc109-3434">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="fc109-3435">[VM/VMSS] Verbesserte Unterstützung für die Datenträgerzwischenspeicherung ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="fc109-3435">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="fc109-3436">VM/VMSS: Einbinden der vom Portal verwendeten Logik zur Überprüfung von Anmeldeinformationen ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="fc109-3436">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="fc109-3437">Hinzufügen von wait-Befehlen und Unterstützung für „--no-wait“ ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="fc109-3437">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="fc109-3438">VM-Skalierungsgruppe: Unterstützung von „\*“ zum Auflisten der übergreifenden Instanzansicht für VMs ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="fc109-3438">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="fc109-3439">Hinzufügen – Geheimnisse für virtuellen Computer und VM-Skalierungsgruppe ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="fc109-3439">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="fc109-3440">Zulassen der VM-Erstellung mit spezialisierter VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="fc109-3440">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="fc109-3441">27. Februar 2017</span><span class="sxs-lookup"><span data-stu-id="fc109-3441">February 27, 2017</span></span>

<span data-ttu-id="fc109-3442">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="fc109-3442">Version 2.0.0</span></span>

<span data-ttu-id="fc109-3443">Diese Version der Azure CLI 2.0 ist die erste „allgemein verfügbare“ Version. Die allgemeine Verfügbarkeit gilt für die folgenden Befehlsmodule:</span><span class="sxs-lookup"><span data-stu-id="fc109-3443">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="fc109-3444">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="fc109-3444">Container Service (acs)</span></span>
- <span data-ttu-id="fc109-3445">Compute (einschließlich Resource Manager, VM, VM-Skalierungsgruppen, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="fc109-3445">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="fc109-3446">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="fc109-3446">Networking</span></span>
- <span data-ttu-id="fc109-3447">Storage</span><span class="sxs-lookup"><span data-stu-id="fc109-3447">Storage</span></span>

<span data-ttu-id="fc109-3448">Diese Befehlsmodule können in der Produktion verwendet werden und verfügen über Unterstützung durch eine Standard-SLA von Microsoft. Sie können Anfragen zu Problemen direkt beim Microsoft-Support oder in der [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/) öffnen. Sie haben die Möglichkeit, Fragen in [StackOverflow mit dem Tag „azure-cli“](http://stackoverflow.com/questions/tagged/azure-cli) zu stellen oder sich unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) an das Produktteam zu wenden. Außerdem können Sie über die Befehlszeile mit dem Befehl `az feedback` Feedback senden.</span><span class="sxs-lookup"><span data-stu-id="fc109-3448">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="fc109-3449">Die Befehle in diesen Modulen sind stabil, und es ist nicht zu erwarten, dass sich die Syntax in den anstehenden Veröffentlichungen dieser Version der Azure CLI ändern.</span><span class="sxs-lookup"><span data-stu-id="fc109-3449">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="fc109-3450">Verwenden Sie zum Überprüfen der Version der CLI den Befehl `az --version`. In der Ausgabe werden die Version der CLI selbst (für diese Veröffentlichung 2.0.0), die einzelnen Befehlsmodule und die von Ihnen genutzten Versionen von Python und GCC aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="fc109-3450">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="fc109-3451">Einige Befehlsmodule verfügen über das Postfix „b*n*“ oder „rc*n*“. Diese Befehlsmodule befinden sich noch in der Vorschauphase und werden später die allgemeine Verfügbarkeit erlangen.</span><span class="sxs-lookup"><span data-stu-id="fc109-3451">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="fc109-3452">Außerdem werden jeden Abend Vorschaubuilds der CLI bereitgestellt. Informationen hierzu finden Sie in der [Anleitung zum Abrufen der abendlichen Builds](https://github.com/Azure/azure-cli#nightly-builds) und im Abschnitt zum [Setup für Entwickler und Beitragen von Code](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="fc109-3452">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="fc109-3453">Sie können für die abendlichen Vorschaubuilds wie folgt Probleme melden:</span><span class="sxs-lookup"><span data-stu-id="fc109-3453">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="fc109-3454">Über die [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="fc109-3454">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="fc109-3455">Per Kontaktaufnahme mit dem Produktteam unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="fc109-3455">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="fc109-3456">Senden von Feedback über die Befehlszeile mit dem Befehl `az feedback`</span><span class="sxs-lookup"><span data-stu-id="fc109-3456">Provide feedback from the command line with the `az feedback` command</span></span>


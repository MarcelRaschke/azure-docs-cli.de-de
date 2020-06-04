---
title: Versionshinweise für die Azure CLI
description: Enthält Informationen zu den aktuellen Updates der Azure CLI.
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 06/02/2020
ms.topic: article
ms.service: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: be0db24ca312825aba03256119d1b5e43afbd902
ms.sourcegitcommit: 62355a77ca59addf7b19db6b95027676e52fd936
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/02/2020
ms.locfileid: "84275061"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="5f12f-103">Versionshinweise für die Azure CLI</span><span class="sxs-lookup"><span data-stu-id="5f12f-103">Azure CLI release notes</span></span>

## <a name="june-02-2020"></a><span data-ttu-id="5f12f-104">2\. Juni 2020</span><span class="sxs-lookup"><span data-stu-id="5f12f-104">June 02, 2020</span></span>

<span data-ttu-id="5f12f-105">Version 2.7.0</span><span class="sxs-lookup"><span data-stu-id="5f12f-105">Version 2.7.0</span></span>

### <a name="acr"></a><span data-ttu-id="5f12f-106">ACR</span><span class="sxs-lookup"><span data-stu-id="5f12f-106">ACR</span></span>

* <span data-ttu-id="5f12f-107">Tippfehler in einer Fehlermeldung der Tokenerstellung korrigiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-107">Fix a typo in an error message of token creation</span></span>

### <a name="aks"></a><span data-ttu-id="5f12f-108">AKS</span><span class="sxs-lookup"><span data-stu-id="5f12f-108">AKS</span></span>

* <span data-ttu-id="5f12f-109">Standard-VM-SKU in „Standard_D2s_v3“ geändert</span><span class="sxs-lookup"><span data-stu-id="5f12f-109">Change default vm sku to Standard_D2s_v3</span></span>
* <span data-ttu-id="5f12f-110">Erstellung der Rollenzuweisung für MSI-Cluster plus benutzerdefiniertes Subnetz korrigiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-110">Fix creating role assignment for MSI clsuter plus custom subnet</span></span>

### <a name="appservice"></a><span data-ttu-id="5f12f-111">AppService</span><span class="sxs-lookup"><span data-stu-id="5f12f-111">AppService</span></span>

* <span data-ttu-id="5f12f-112">Fehlerbehebung Nr. 12739: Von „az appservice list-locations“ werden einige ungültige Standorte zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5f12f-112">Fix #12739 az appservice list-locations returns some invalid locations</span></span>

### <a name="arm"></a><span data-ttu-id="5f12f-113">ARM</span><span class="sxs-lookup"><span data-stu-id="5f12f-113">ARM</span></span>

* <span data-ttu-id="5f12f-114">`az deployment`: Fehlerbehebung Nr. 13159 der fehlerhaften JSON-Meldung nach dem Entfernen von Kommentaren und nach dem Komprimieren</span><span class="sxs-lookup"><span data-stu-id="5f12f-114">`az deployment`: Fix issue #13159 of incorrect message of JSON after removing comments and compressing</span></span>
* <span data-ttu-id="5f12f-115">`az resource tag`: Fehlerbehebung Nr. 13255 für das Markieren von Ressourcen mit dem Ressourcentyp `Microsoft.ContainerRegistry/registries/webhooks`</span><span class="sxs-lookup"><span data-stu-id="5f12f-115">`az resource tag`: Fix issue #13255 of tagging resources with resource type `Microsoft.ContainerRegistry/registries/webhooks`</span></span>
* <span data-ttu-id="5f12f-116">Beispiele für das Ressourcenmodul verbessert</span><span class="sxs-lookup"><span data-stu-id="5f12f-116">Improve the examples for the resource module</span></span>

### <a name="aro"></a><span data-ttu-id="5f12f-117">ARO</span><span class="sxs-lookup"><span data-stu-id="5f12f-117">ARO</span></span>

* <span data-ttu-id="5f12f-118">CLIError in das richtige Flag für „--worker-vm-disk-size-gb“ geändert</span><span class="sxs-lookup"><span data-stu-id="5f12f-118">Change CLIError to correct flag for --worker-vm-disk-size-gb</span></span>

### <a name="eventhub"></a><span data-ttu-id="5f12f-119">EventHub</span><span class="sxs-lookup"><span data-stu-id="5f12f-119">EventHub</span></span>

* <span data-ttu-id="5f12f-120">Fehlerbehebung Nr. 12406: „intervalInSeconds“ wird von Argument „--capture-interval“ nicht aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="5f12f-120">Fix for issue #12406 Argument --capture-interval does not update the "intervalInSeconds"</span></span>

### <a name="hdinsight"></a><span data-ttu-id="5f12f-121">HDInsight</span><span class="sxs-lookup"><span data-stu-id="5f12f-121">HDInsight</span></span>

* <span data-ttu-id="5f12f-122">„get_json_object“ in „shell_safe_json_parse“ geändert</span><span class="sxs-lookup"><span data-stu-id="5f12f-122">Change get_json_object to shell_safe_json_parse</span></span>

### <a name="monitor"></a><span data-ttu-id="5f12f-123">Überwachen</span><span class="sxs-lookup"><span data-stu-id="5f12f-123">Monitor</span></span>

* <span data-ttu-id="5f12f-124">`az monitor metrics alert`: Verschiedene Hilfemeldungen optimiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-124">`az monitor metrics alert`: refine several help messages</span></span>
* <span data-ttu-id="5f12f-125">`az monitor diagnostic-settings create`: Unterstützung für das Argument „--export-to-resource-specific“</span><span class="sxs-lookup"><span data-stu-id="5f12f-125">`az monitor diagnostic-settings create`: support --export-to-resource-specific argument</span></span>
* <span data-ttu-id="5f12f-126">Unterstützung für die Wiederherstellung von LA-Arbeitsbereichen</span><span class="sxs-lookup"><span data-stu-id="5f12f-126">Support LA workspace recover</span></span>

### <a name="network"></a><span data-ttu-id="5f12f-127">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="5f12f-127">Network</span></span>

* <span data-ttu-id="5f12f-128">`az network dns zone`: Unterstützung des Bindestrichs (-)</span><span class="sxs-lookup"><span data-stu-id="5f12f-128">`az network dns zone`: support - character</span></span>
* <span data-ttu-id="5f12f-129">`az network vpn-connection ipsec-policy`: „--sa-lifetime“ und „--sa-max-size“ im Beispiel in höhere Werte geändert</span><span class="sxs-lookup"><span data-stu-id="5f12f-129">`az network vpn-connection ipsec-policy`: change the --sa-lifetime and --sa-max-size to larger values in example</span></span>
* <span data-ttu-id="5f12f-130">Netzwerk auf 2020-04-01 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-130">Bump network to 2020-04-01</span></span>
* <span data-ttu-id="5f12f-131">`az network private-endpoint-connection`: Unterstützung von Event Grid</span><span class="sxs-lookup"><span data-stu-id="5f12f-131">`az network private-endpoint-connection`: support event grid</span></span>
* <span data-ttu-id="5f12f-132">`az network express-route list-route-tables`: Fehler behoben, der dazu führte, dass Routen nicht als Tabelle aufgeführt werden konnten</span><span class="sxs-lookup"><span data-stu-id="5f12f-132">`az network express-route list-route-tables`: fix bug that cannot list routes as table</span></span>

### <a name="packaging"></a><span data-ttu-id="5f12f-133">Verpackung</span><span class="sxs-lookup"><span data-stu-id="5f12f-133">Packaging</span></span>

* <span data-ttu-id="5f12f-134">Ubuntu-Paket (Focal) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-134">Add Ubuntu Focal Package</span></span>

### <a name="rbac"></a><span data-ttu-id="5f12f-135">RBAC</span><span class="sxs-lookup"><span data-stu-id="5f12f-135">RBAC</span></span>

* <span data-ttu-id="5f12f-136">`az ad sp credential reset`: Erstellung von Anmeldeinformationen geändert, um problematische Sonderzeichen zu vermeiden</span><span class="sxs-lookup"><span data-stu-id="5f12f-136">`az ad sp credential reset`: modify credential generation to avoid troublesome special characters</span></span>

### <a name="redis"></a><span data-ttu-id="5f12f-137">Redis</span><span class="sxs-lookup"><span data-stu-id="5f12f-137">Redis</span></span>

* <span data-ttu-id="5f12f-138">Fehlerbehebung Nr. 13529: Dokumentation des Parameters „enable_non_ssl_port“ geändert</span><span class="sxs-lookup"><span data-stu-id="5f12f-138">Fix #13529: Change documentation of parameter enable_non_ssl_port</span></span>

### <a name="storage"></a><span data-ttu-id="5f12f-139">Storage</span><span class="sxs-lookup"><span data-stu-id="5f12f-139">Storage</span></span>

* <span data-ttu-id="5f12f-140">`az storage copy`: Parameter `--follow-symlinks` zur Unterstützung von symbolischen Verknüpfungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-140">`az storage copy`: Add parameter `--follow-symlinks` to support symlinks</span></span>
* <span data-ttu-id="5f12f-141">Lokaler Kontext für Speicherkonto aktiviert</span><span class="sxs-lookup"><span data-stu-id="5f12f-141">Enable local context for storage account</span></span>
* <span data-ttu-id="5f12f-142">`az storage logging`: Fehlerbehebung Nr. 11969: Fehlermeldung optimiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-142">`az storage logging`: Fix issue #11969 to refine error message</span></span>

## <a name="may-19-2020"></a><span data-ttu-id="5f12f-143">19. Mai 2020</span><span class="sxs-lookup"><span data-stu-id="5f12f-143">May 19, 2020</span></span>

<span data-ttu-id="5f12f-144">Version 2.6.0</span><span class="sxs-lookup"><span data-stu-id="5f12f-144">Version 2.6.0</span></span>

### <a name="acr"></a><span data-ttu-id="5f12f-145">ACR</span><span class="sxs-lookup"><span data-stu-id="5f12f-145">ACR</span></span>

* <span data-ttu-id="5f12f-146">Standardtimeout von fünf Minuten für jede an ACR gesendete Anforderung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-146">Add default timeout of 5 minutes for any requests to ACR</span></span>
* <span data-ttu-id="5f12f-147">Unterstützung für das Deaktivieren des Zugriffs auf das öffentliche Netzwerk</span><span class="sxs-lookup"><span data-stu-id="5f12f-147">Support disable public network access</span></span>
* <span data-ttu-id="5f12f-148">`az acr token create`: Argument „--days“ verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="5f12f-148">`az acr token create`: expose --days argument</span></span>
* <span data-ttu-id="5f12f-149">`az acr import`: Akzeptiert Werte für das Argument „--source“, bei denen der Servername einen Anmeldenamen enthält (mittels clientseitiger Korrektur)</span><span class="sxs-lookup"><span data-stu-id="5f12f-149">`az acr import`: accept --source argument values which contain login in server name through client end correction</span></span>

### <a name="acs"></a><span data-ttu-id="5f12f-150">ACS</span><span class="sxs-lookup"><span data-stu-id="5f12f-150">ACS</span></span>

* <span data-ttu-id="5f12f-151">Fehlerbehebung: Felderbereinigung für Felder entfernt, die nicht mehr vorhanden sind</span><span class="sxs-lookup"><span data-stu-id="5f12f-151">Bug fix: remove fields cleanup for fields that no longer exist</span></span>

### <a name="aks"></a><span data-ttu-id="5f12f-152">AKS</span><span class="sxs-lookup"><span data-stu-id="5f12f-152">AKS</span></span>

* <span data-ttu-id="5f12f-153">Hilfekontext des Befehls „uptime-sla“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-153">Update uptime-sla command help context</span></span>
* <span data-ttu-id="5f12f-154">Bereichsüberprüfung für die Aktualisierung der Mindestanzahl für die Autoskalierung entfernt</span><span class="sxs-lookup"><span data-stu-id="5f12f-154">Remove range check for updating min count for autoscaler</span></span>
* <span data-ttu-id="5f12f-155">Hotfix, der bewirkt, dass bei der CLI kein Fehler auftritt, wenn der Benutzer nur das Windows-Kennwort angibt</span><span class="sxs-lookup"><span data-stu-id="5f12f-155">Fix that cli doe not fail when user only specifies Windows password</span></span>

### <a name="ams"></a><span data-ttu-id="5f12f-156">AMS</span><span class="sxs-lookup"><span data-stu-id="5f12f-156">AMS</span></span>

* <span data-ttu-id="5f12f-157">`az ams transform create`: Funktion zum Erstellen einer Transformation mit einer FaceDetector-Voreinstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-157">`az ams transform create`: Add ability to create a transform with a FaceDetector preset</span></span>
* <span data-ttu-id="5f12f-158">`az ams content-key-policy create` : Funktion zum Erstellen einer FairPlay-Inhaltsschlüsselrichtlinie mit einer Konfiguration für die Offlinemiete hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-158">`az ams content-key-policy create` : Add ability to create a FairPlay content key policy with an offline rental configuration</span></span>

### <a name="appconfig"></a><span data-ttu-id="5f12f-159">AppConfig</span><span class="sxs-lookup"><span data-stu-id="5f12f-159">AppConfig</span></span>

* <span data-ttu-id="5f12f-160">Fehlerbehebung für die Schlüsselauflistungswerte mit Feldern</span><span class="sxs-lookup"><span data-stu-id="5f12f-160">Bug fix for list key values with fields</span></span>

### <a name="appservice"></a><span data-ttu-id="5f12f-161">AppService</span><span class="sxs-lookup"><span data-stu-id="5f12f-161">AppService</span></span>

* <span data-ttu-id="5f12f-162">`az functionapp create`: AzureWebJobsDashboard wird nur festgelegt, wenn AppInsights deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="5f12f-162">`az functionapp create`: AzureWebJobsDashboard will only be set if AppInsights is disabled</span></span>
* <span data-ttu-id="5f12f-163">Fehlerbehebung Nr. 10664: VNET-Integration – Standortüberprüfungsfehler und Fehlerbehebung Nr. 13257: Fehler bei „az webapp up“, wenn eine Ressourcengruppe erstellt werden muss</span><span class="sxs-lookup"><span data-stu-id="5f12f-163">Fix #10664- VNet Integration - Location Check Issue & fix #13257- az webapp up failing when RG needs to be created</span></span>
* <span data-ttu-id="5f12f-164">`az webapp|functionapp config ssl import`: Ressourcengruppenübergreifende Suche des Schlüsseltresors im Abonnement und verbesserte Hilfe und Beispiele</span><span class="sxs-lookup"><span data-stu-id="5f12f-164">`az webapp|functionapp config ssl import`: Lookup key vault across resources groups in subscription and improve help and examples.</span></span>
* <span data-ttu-id="5f12f-165">Lokaler Kontext für App Service integriert</span><span class="sxs-lookup"><span data-stu-id="5f12f-165">Onboard local context for app service</span></span>

### <a name="arm"></a><span data-ttu-id="5f12f-166">ARM</span><span class="sxs-lookup"><span data-stu-id="5f12f-166">ARM</span></span>

* <span data-ttu-id="5f12f-167">`az deployment`: Problem behoben, das dazu führte, dass templateLink beim Bereitstellen oder Überprüfen von „template-uri“ nicht zurückgegeben wurde</span><span class="sxs-lookup"><span data-stu-id="5f12f-167">`az deployment`: Fix the problem that the templateLink will not be returned when deploying or validating template-uri</span></span>
* <span data-ttu-id="5f12f-168">`az deployment`: Problem behoben, das dazu führte, dass speziell codierte Zeichen von der Bereitstellung/Überprüfung nicht unterstützt wurden</span><span class="sxs-lookup"><span data-stu-id="5f12f-168">`az deployment`: Fix the problem that deployment/validate does not support specially encoded character</span></span>
* <span data-ttu-id="5f12f-169">`az deployment sub/group what-if`: Arrayausrichtung und Fehlerbehandlung korrigiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-169">`az deployment sub/group what-if`: Fix array alignment and error handling</span></span>
* <span data-ttu-id="5f12f-170">`az deployment operation`: Veraltete Informationen angepasst</span><span class="sxs-lookup"><span data-stu-id="5f12f-170">`az deployment operation`: Modify the deprecate information</span></span>

### <a name="aro"></a><span data-ttu-id="5f12f-171">ARO</span><span class="sxs-lookup"><span data-stu-id="5f12f-171">ARO</span></span>

* <span data-ttu-id="5f12f-172">Beispiele zu folgenden Befehlen hinzugefügt: az aro create, list, list-credentials, show, delete</span><span class="sxs-lookup"><span data-stu-id="5f12f-172">Add examples to az aro create, list, list-credentials, show, delete</span></span>
* <span data-ttu-id="5f12f-173">Funktion „generate_random_id“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-173">Add generate_random_id function</span></span>

### <a name="backup"></a><span data-ttu-id="5f12f-174">Backup</span><span class="sxs-lookup"><span data-stu-id="5f12f-174">Backup</span></span>

* <span data-ttu-id="5f12f-175">FriendlyName im Befehl zum Aktivieren des Schutzes für AzureFileShare zulässig</span><span class="sxs-lookup"><span data-stu-id="5f12f-175">Allow FriendlyName in enable protection for AzureFileShare command</span></span>
* <span data-ttu-id="5f12f-176">Korrektur im IaasVM-Befehl „restore-disks“</span><span class="sxs-lookup"><span data-stu-id="5f12f-176">Fix in IaasVM restore-disks Command</span></span>
* <span data-ttu-id="5f12f-177">BackupManagementType „MAB“ zum Befehl zum Auflisten der Elemente hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-177">Add "MAB" BackupManagementType to item list command</span></span>
* <span data-ttu-id="5f12f-178">Unterstützung für die Wiederholung des Richtlinienupdates für fehlerhafte Elemente hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-178">Add support for retrying policy update for failed items.</span></span>
* <span data-ttu-id="5f12f-179">Funktion zum Fortsetzen des Schutzes für virtuelle Azure-Computer hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-179">Add Resume Protection functionality for Azure Virtual Machine</span></span>
* <span data-ttu-id="5f12f-180">Unterstützung zum Angeben der Ressourcengruppe zum Speichern von instantRP beim Erstellen oder Ändern der Richtlinie hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-180">Add support to specify ResourceGroup for storing instantRP during Create or Modify Policy</span></span>

### <a name="ci"></a><span data-ttu-id="5f12f-181">CI</span><span class="sxs-lookup"><span data-stu-id="5f12f-181">CI</span></span>

* <span data-ttu-id="5f12f-182">Unterstützung für flake8 3.8.0</span><span class="sxs-lookup"><span data-stu-id="5f12f-182">Support flake8 3.8.0</span></span>

### <a name="compute"></a><span data-ttu-id="5f12f-183">Compute</span><span class="sxs-lookup"><span data-stu-id="5f12f-183">Compute</span></span>

* <span data-ttu-id="5f12f-184">Neuer Befehl: az vm auto-shutdown</span><span class="sxs-lookup"><span data-stu-id="5f12f-184">New command az vm auto-shutdown</span></span>
* <span data-ttu-id="5f12f-185">`az vm list-skus`: Verhalten von „--zone“aktualisiert. Jetzt werden alle SKU-Typen zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5f12f-185">`az vm list-skus`: Update --zone behavior, return all type skus now</span></span>

### <a name="core"></a><span data-ttu-id="5f12f-186">Core</span><span class="sxs-lookup"><span data-stu-id="5f12f-186">Core</span></span>

* <span data-ttu-id="5f12f-187">Aktivierungsstatus aus dem lokalen Kontext für globale Benutzerebene aktualisiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-187">Update local context on/off status to global user level</span></span>

### <a name="extension"></a><span data-ttu-id="5f12f-188">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="5f12f-188">Extension</span></span>

* <span data-ttu-id="5f12f-189">`az extension add`: „--system“ hinzugefügt, um die Installation von Erweiterungen in einem Systempfad zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="5f12f-189">`az extension add`: Add --system to enable installing extensions in a system path</span></span>
* <span data-ttu-id="5f12f-190">Unterstützung für „.egg-info“ zum Speichern der Metadaten für die Radtyperweiterung</span><span class="sxs-lookup"><span data-stu-id="5f12f-190">Support .egg-info to store wheel type extension metadata</span></span>

### <a name="iot"></a><span data-ttu-id="5f12f-191">IoT</span><span class="sxs-lookup"><span data-stu-id="5f12f-191">IoT</span></span>

* <span data-ttu-id="5f12f-192">`az iot`: Nachricht des IoT-Befehlsmoduls mit dem Hinweis auf die Erweiterung für die erste Ausführung aktualisiert, sodass sie anstelle der veralteten ID die korrekte moderne ID (`azure-iot`) enthält</span><span class="sxs-lookup"><span data-stu-id="5f12f-192">`az iot`: Update the IoT command module first run extension awareness message to the accurate, non-deprecated modern Id `azure-iot`.</span></span>

### <a name="iot-hub"></a><span data-ttu-id="5f12f-193">IoT Hub</span><span class="sxs-lookup"><span data-stu-id="5f12f-193">IoT Hub</span></span>

* <span data-ttu-id="5f12f-194">Unterstützung für API- und Netzwerkisolationsbefehle für 2020-03-01</span><span class="sxs-lookup"><span data-stu-id="5f12f-194">Support for 2020-03-01 API and Network Isolation commands</span></span>

### <a name="netappfiles"></a><span data-ttu-id="5f12f-195">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="5f12f-195">NetAppFiles</span></span>

* <span data-ttu-id="5f12f-196">`az volume create`: „snapshot-id“ als Parameter zum Erstellen eines Volumes hinzugefügt. Ermöglicht Benutzern das Erstellen eines Volumes auf der Grundlage einer vorhandenen Momentaufnahme.</span><span class="sxs-lookup"><span data-stu-id="5f12f-196">`az volume create`: Adds snapshot-id as a parameter to create volume this will allow users to create a volume from existing snapshot.</span></span>

### <a name="network"></a><span data-ttu-id="5f12f-197">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="5f12f-197">Network</span></span>

* <span data-ttu-id="5f12f-198">TTL-Wert korrigiert, der für „dns add-record“ unbeabsichtigt geändert wurde</span><span class="sxs-lookup"><span data-stu-id="5f12f-198">Fix ttl value changed unintended for dns add-record</span></span>
* <span data-ttu-id="5f12f-199">`az network public-ip create`: Kunden über einen bevorstehenden Breaking Change informiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-199">`az network public-ip create`: Inform customers of a coming breaking change</span></span>
* <span data-ttu-id="5f12f-200">Unterstützung von generischen Befehlen für Private Link-Szenario</span><span class="sxs-lookup"><span data-stu-id="5f12f-200">Support generic commands for private link scenario</span></span>
* <span data-ttu-id="5f12f-201">`az network private-endpoint-connection`: Unterstützung für MySQL-, Postgre- und MariaDB-Typen</span><span class="sxs-lookup"><span data-stu-id="5f12f-201">`az network private-endpoint-connection`: Support mysql, postgre and mariadb types</span></span>
* <span data-ttu-id="5f12f-202">`az network private-endpoint-connection`: Unterstützung von CosmosDB-Typen</span><span class="sxs-lookup"><span data-stu-id="5f12f-202">`az network private-endpoint-connection`: Support cosmosdb types</span></span>
* <span data-ttu-id="5f12f-203">`az network private-endpoint`: „--group-ids“ und Umleitung an „--group-id“ als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="5f12f-203">`az network private-endpoint`: deprecate --group-ids and redirect to --group-id</span></span>

### <a name="output"></a><span data-ttu-id="5f12f-204">Output</span><span class="sxs-lookup"><span data-stu-id="5f12f-204">Output</span></span>

* <span data-ttu-id="5f12f-205">Anzeigen der Updateanweisung bei der Suche, beim Feedback und in „--help“</span><span class="sxs-lookup"><span data-stu-id="5f12f-205">Show update instruction in find, feedback and --help</span></span>

### <a name="packaging"></a><span data-ttu-id="5f12f-206">Verpackung</span><span class="sxs-lookup"><span data-stu-id="5f12f-206">Packaging</span></span>

* <span data-ttu-id="5f12f-207">Erstellen von MSI-/Homebrew-Paketen mit Abhängigkeiten, die aus „requirements.txt“ aufgelöst werden</span><span class="sxs-lookup"><span data-stu-id="5f12f-207">Build MSI/Homebrew packages with dependecies resolved from requirements.txt</span></span>

### <a name="rbac"></a><span data-ttu-id="5f12f-208">RBAC</span><span class="sxs-lookup"><span data-stu-id="5f12f-208">RBAC</span></span>

* <span data-ttu-id="5f12f-209">`az ad sp credential reset`: Erstellung unsicherer Anmeldeinformationen korrigiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-209">`az ad sp credential reset`: fix weak credential generation</span></span>

### <a name="storage"></a><span data-ttu-id="5f12f-210">Storage</span><span class="sxs-lookup"><span data-stu-id="5f12f-210">Storage</span></span>

* <span data-ttu-id="5f12f-211">`az storage account file-service-properties update/show`: Unterstützung für Dateieigenschaften für Speicherkonto hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-211">`az storage account file-service-properties update/show`: Add File Properties Support for Storage Account</span></span>
* <span data-ttu-id="5f12f-212">`az storage container create`: Fehlerbehebung Nr. 13373 durch Hinzufügen eines Validierungssteuerelements für öffentlichen Zugriff</span><span class="sxs-lookup"><span data-stu-id="5f12f-212">`az storage container create`: Fix #13373 by adding validator for public access</span></span>
* <span data-ttu-id="5f12f-213">Unterstützung für ADLS Gen2 (track2) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-213">Add ADLS Gen2 track2 support</span></span>
* <span data-ttu-id="5f12f-214">`az storage blob sync`: Unterstützung für `--connection-string`</span><span class="sxs-lookup"><span data-stu-id="5f12f-214">`az storage blob sync`: Support `--connection-string`</span></span>
* <span data-ttu-id="5f12f-215">`az storage blob sync`: Falsche Fehlermeldung korrigiert, die angezeigt wird, wenn der Installationsspeicherort von „azcopy“ nicht gefunden wird</span><span class="sxs-lookup"><span data-stu-id="5f12f-215">`az storage blob sync`: Fix the incorrect error message when azcopy cannot find the installation location</span></span>

## <a name="april-30-2020"></a><span data-ttu-id="5f12f-216">30. April 2020</span><span class="sxs-lookup"><span data-stu-id="5f12f-216">April 30, 2020</span></span>

<span data-ttu-id="5f12f-217">Version 2.5.1</span><span class="sxs-lookup"><span data-stu-id="5f12f-217">Version 2.5.1</span></span>

### <a name="acr"></a><span data-ttu-id="5f12f-218">ACR</span><span class="sxs-lookup"><span data-stu-id="5f12f-218">ACR</span></span>

* <span data-ttu-id="5f12f-219">`az acr check-health`: „DOCKER_PULL_ERROR“ unter Windows behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-219">`az acr check-health`: Fix "DOCKER_PULL_ERROR" on Windows</span></span>

### <a name="compute"></a><span data-ttu-id="5f12f-220">Compute</span><span class="sxs-lookup"><span data-stu-id="5f12f-220">Compute</span></span>

* <span data-ttu-id="5f12f-221">`az vm list-ip-addresses`: Fehlerbehandlung</span><span class="sxs-lookup"><span data-stu-id="5f12f-221">`az vm list-ip-addresses`: Error handling</span></span>
* <span data-ttu-id="5f12f-222">Fehler behoben, der bei der VM-Erstellung auftrat, wenn „endpoint_vm_image_alias_doc“ im Cloudprofil nicht festgelegt war</span><span class="sxs-lookup"><span data-stu-id="5f12f-222">Fix a bug of vm create if endpoint_vm_image_alias_doc is not set in cloud profile</span></span>
* <span data-ttu-id="5f12f-223">`az vmss create`: „--os-disk-size-gb“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-223">`az vmss create`: Add --os-disk-size-gb</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="5f12f-224">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="5f12f-224">Cosmos DB</span></span>

* <span data-ttu-id="5f12f-225">`az cosmosdb create/update`: Unterstützung für „--enable-public-network“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-225">`az cosmosdb create/update`: add --enable-public-network support</span></span>

### <a name="extension"></a><span data-ttu-id="5f12f-226">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="5f12f-226">Extension</span></span>

* <span data-ttu-id="5f12f-227">Laden der falschen Metadaten für die Radtyperweiterung korrigiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-227">Fix loading wrong metadata for wheel type extension</span></span>

### <a name="packaging"></a><span data-ttu-id="5f12f-228">Verpackung</span><span class="sxs-lookup"><span data-stu-id="5f12f-228">Packaging</span></span>

* <span data-ttu-id="5f12f-229">Az-Skript für Git Bash/Cygwin unter Windows hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-229">Add az script for Git Bash/Cygwin on Windows</span></span>

### <a name="sql"></a><span data-ttu-id="5f12f-230">SQL</span><span class="sxs-lookup"><span data-stu-id="5f12f-230">SQL</span></span>

* <span data-ttu-id="5f12f-231">`az sql instance-pool`: Befehlsgruppe für Instanzpools hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-231">`az sql instance-pool`: Add instance pools command group</span></span>

### <a name="storage"></a><span data-ttu-id="5f12f-232">Storage</span><span class="sxs-lookup"><span data-stu-id="5f12f-232">Storage</span></span>

* <span data-ttu-id="5f12f-233">Paket „azure-multiapi-storage“ auf 0.3.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-233">Upgrade package azure-multiapi-storage to 0.3.0</span></span>
* <span data-ttu-id="5f12f-234">Unterstützung von GZRS für Speicherkontoerstellung und -aktualisierung</span><span class="sxs-lookup"><span data-stu-id="5f12f-234">Support GZRS for storage account creation and update</span></span>
* <span data-ttu-id="5f12f-235">`az storage account failover`: Unterstützung für das Failover von GRS/GZRS-Speicherkonten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-235">`az storage account failover`: Add support for grs/gzrs storage account failover</span></span>
* <span data-ttu-id="5f12f-236">`az storage blob upload`: Parameter „--encryption-scope“ hinzugefügt, um die Angabe von Informationen zum Verschlüsselungsbereich zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="5f12f-236">`az storage blob upload`: Add --encryption-scope parameter to support specifying encryption scope information</span></span>

## <a name="april-28-2020"></a><span data-ttu-id="5f12f-237">28. April 2020</span><span class="sxs-lookup"><span data-stu-id="5f12f-237">April 28, 2020</span></span>

<span data-ttu-id="5f12f-238">Version 2.5.0</span><span class="sxs-lookup"><span data-stu-id="5f12f-238">Version 2.5.0</span></span>

### <a name="acs"></a><span data-ttu-id="5f12f-239">ACS</span><span class="sxs-lookup"><span data-stu-id="5f12f-239">ACS</span></span>

* <span data-ttu-id="5f12f-240">[BREAKING CHANGE] az openshift create: Parameter „--vnet-peer“ entfernt</span><span class="sxs-lookup"><span data-stu-id="5f12f-240">[BREAKING CHANGE] az openshift create: remove --vnet-peer parameter.</span></span>
* <span data-ttu-id="5f12f-241">`az openshift create`: Flags zur Unterstützung des privaten Clusters hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-241">`az openshift create`: add flags to support private cluster.</span></span>
* <span data-ttu-id="5f12f-242">`az openshift`: Upgrade auf API-Version `2019-10-27-preview`</span><span class="sxs-lookup"><span data-stu-id="5f12f-242">`az openshift`: upgrade to `2019-10-27-preview` API version.</span></span>
* <span data-ttu-id="5f12f-243">`az openshift`: Befehl `update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-243">`az openshift`: add `update` command.</span></span>

### <a name="aks"></a><span data-ttu-id="5f12f-244">AKS</span><span class="sxs-lookup"><span data-stu-id="5f12f-244">AKS</span></span>

* <span data-ttu-id="5f12f-245">`az aks create`: Unterstützung für Windows hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-245">`az aks create`: Add support for Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="5f12f-246">AppService</span><span class="sxs-lookup"><span data-stu-id="5f12f-246">AppService</span></span>

* <span data-ttu-id="5f12f-247">`az webapp deployment source config-zip`: Energiesparmodus nach „request.get()“ entfernt</span><span class="sxs-lookup"><span data-stu-id="5f12f-247">`az webapp deployment source config-zip`: remove sleep after request.get()</span></span>

### <a name="arm"></a><span data-ttu-id="5f12f-248">ARM</span><span class="sxs-lookup"><span data-stu-id="5f12f-248">ARM</span></span>

* <span data-ttu-id="5f12f-249">Was-wäre-wenn-Befehle für Vorlagenbereitstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-249">Add template deployment What-If commands</span></span>

### <a name="aro"></a><span data-ttu-id="5f12f-250">ARO</span><span class="sxs-lookup"><span data-stu-id="5f12f-250">ARO</span></span>

* <span data-ttu-id="5f12f-251">`az aro`: Tabellenausgabe korrigiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-251">`az aro`: Fix table output</span></span>

### <a name="ci"></a><span data-ttu-id="5f12f-252">CI</span><span class="sxs-lookup"><span data-stu-id="5f12f-252">CI</span></span>

* <span data-ttu-id="5f12f-253">pytest integriert und nose für Automatisierungstest als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="5f12f-253">Onboard pytest and deprecate nose for Automation Test</span></span>

### <a name="compute"></a><span data-ttu-id="5f12f-254">Compute</span><span class="sxs-lookup"><span data-stu-id="5f12f-254">Compute</span></span>

* <span data-ttu-id="5f12f-255">`az vmss disk detach`: Datenträgerfehler „NoneType“ behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-255">`az vmss disk detach`: fix data disk NoneType issue</span></span>
* <span data-ttu-id="5f12f-256">`az vm availability-set list`: Unterstützung zum Anzeigen der VM-Liste</span><span class="sxs-lookup"><span data-stu-id="5f12f-256">`az vm availability-set list`: Support showing VM list</span></span>
* <span data-ttu-id="5f12f-257">`az vm list-skus`: Anzeigeproblem des Tabellenformats behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-257">`az vm list-skus`: Fix display problem of table format</span></span>

### <a name="keyvault"></a><span data-ttu-id="5f12f-258">KeyVault</span><span class="sxs-lookup"><span data-stu-id="5f12f-258">KeyVault</span></span>

* <span data-ttu-id="5f12f-259">Neuer Parameter `--enable-rbac-authorization` bei Erstellung oder Aktualisierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-259">Add new parameter `--enable-rbac-authorization` during creating or updating</span></span>

### <a name="monitor"></a><span data-ttu-id="5f12f-260">Überwachen</span><span class="sxs-lookup"><span data-stu-id="5f12f-260">Monitor</span></span>

* <span data-ttu-id="5f12f-261">Unterstützung der CMK-Features für LA-Cluster</span><span class="sxs-lookup"><span data-stu-id="5f12f-261">Support LA cluster CMK features</span></span>
* <span data-ttu-id="5f12f-262">`az monitor log-analytics workspace linked-storage`: Unterstützung für BYOS-Features</span><span class="sxs-lookup"><span data-stu-id="5f12f-262">`az monitor log-analytics workspace linked-storage`: supports BYOS features</span></span>

### <a name="network"></a><span data-ttu-id="5f12f-263">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="5f12f-263">Network</span></span>

* <span data-ttu-id="5f12f-264">`az network security-partner`: Unterstützung des Sicherheitspartneranbieters</span><span class="sxs-lookup"><span data-stu-id="5f12f-264">`az network security-partner`: support security partner provider</span></span>

### <a name="privatedns"></a><span data-ttu-id="5f12f-265">PrivateDNS</span><span class="sxs-lookup"><span data-stu-id="5f12f-265">Privatedns</span></span>

* <span data-ttu-id="5f12f-266">Funktion in privater DNS-Zone zum Importieren der Exportzonendatei hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-266">Add feature in private DNS zone to import export zone file</span></span>

## <a name="april-21-2020"></a><span data-ttu-id="5f12f-267">21. April 2020</span><span class="sxs-lookup"><span data-stu-id="5f12f-267">April 21, 2020</span></span>

<span data-ttu-id="5f12f-268">Version 2.4.0</span><span class="sxs-lookup"><span data-stu-id="5f12f-268">Version 2.4.0</span></span>

### <a name="acr"></a><span data-ttu-id="5f12f-269">ACR</span><span class="sxs-lookup"><span data-stu-id="5f12f-269">ACR</span></span>

* <span data-ttu-id="5f12f-270">`az acr run --cmd`: Deaktivieren der Arbeitsverzeichnisaußerkraftsetzung</span><span class="sxs-lookup"><span data-stu-id="5f12f-270">`az acr run --cmd`: disable working directory override</span></span>
* <span data-ttu-id="5f12f-271">Unterstützung dedizierter Datenendpunkte</span><span class="sxs-lookup"><span data-stu-id="5f12f-271">Support dedicated data endpoint</span></span>

### <a name="aks"></a><span data-ttu-id="5f12f-272">AKS</span><span class="sxs-lookup"><span data-stu-id="5f12f-272">AKS</span></span>

* <span data-ttu-id="5f12f-273">`az aks list -o table` sollte „privateFqdn“ als FQDN für private Cluster anzeigen</span><span class="sxs-lookup"><span data-stu-id="5f12f-273">`az aks list -o table` should show privateFqdn as fqdn for private clusters</span></span>
* <span data-ttu-id="5f12f-274">„--uptime-sla“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-274">Add --uptime-sla</span></span>
* <span data-ttu-id="5f12f-275">containerservice-Paket aktualisiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-275">Update containerservice package</span></span>
* <span data-ttu-id="5f12f-276">Unterstützung für öffentliche IP-Adressen für Knoten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-276">Add node public IP support</span></span>
* <span data-ttu-id="5f12f-277">Tippfehler im help-Befehl korrigiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-277">Fix typo in the help command</span></span>

### <a name="appconfig"></a><span data-ttu-id="5f12f-278">AppConfig</span><span class="sxs-lookup"><span data-stu-id="5f12f-278">AppConfig</span></span>

* <span data-ttu-id="5f12f-279">Schlüsseltresorverweis für die Befehle „kv list“ und „kv export“ aufgelöst</span><span class="sxs-lookup"><span data-stu-id="5f12f-279">Resolve key vault reference for kv list and export commands</span></span>
* <span data-ttu-id="5f12f-280">Fehlerbehebung für die Werte für das Auflisten von Schlüsseln</span><span class="sxs-lookup"><span data-stu-id="5f12f-280">Bug fix for list key values</span></span>

### <a name="appservice"></a><span data-ttu-id="5f12f-281">AppService</span><span class="sxs-lookup"><span data-stu-id="5f12f-281">AppService</span></span>

* <span data-ttu-id="5f12f-282">`az functionapp create`: Vorgehensweise zum Festlegen von „linuxFxVersion“ für Linux-Funktions-Apps (.NET) geändert.</span><span class="sxs-lookup"><span data-stu-id="5f12f-282">`az functionapp create`: Changed the way linuxFxVersion was being set for dotnet linux function apps.</span></span> <span data-ttu-id="5f12f-283">Dadurch sollte der Fehler behoben sein, der die Erstellung von Linux-Verbrauchs-Apps (.NET) verhindert hat.</span><span class="sxs-lookup"><span data-stu-id="5f12f-283">This should fix a bug that was preventing dotnet linux consumption apps from being created</span></span>
* <span data-ttu-id="5f12f-284">[BREAKING CHANGE] `az webapp create`: Korrektur vorgenommen, um vorhandene App-Einstellungen (AppSettings) für „az webapp create“ beizubehalten</span><span class="sxs-lookup"><span data-stu-id="5f12f-284">[BREAKING CHANGE] `az webapp create`: fix to keep existing AppSettings with az webapp create</span></span>
* <span data-ttu-id="5f12f-285">[BREAKING CHANGE] `az webapp up`: Korrektur vorgenommen, um bei Verwendung des Flags „-g“ eine RG für den Befehl „az webapp up“ zu erstellen</span><span class="sxs-lookup"><span data-stu-id="5f12f-285">[BREAKING CHANGE] `az webapp up`: fix to create RG for az webapp up command when using -g flag</span></span>
* <span data-ttu-id="5f12f-286">[BREAKING CHANGE] `az webapp config`: Korrektur vorgenommen, um Werte für Nicht-JSON-Ausgaben mit „az webapp config connection-string list“ anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="5f12f-286">[BREAKING CHANGE] `az webapp config`: fix to show values for non-JSON output with az webapp config connection-string list</span></span>

### <a name="arm"></a><span data-ttu-id="5f12f-287">ARM</span><span class="sxs-lookup"><span data-stu-id="5f12f-287">ARM</span></span>

* <span data-ttu-id="5f12f-288">`az deployment create/validate`: Parameter `--no-prompt` hinzugefügt, um das Überspringen der Eingabeaufforderung für fehlende Parameter für die ARM-Vorlage zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="5f12f-288">`az deployment create/validate`: Add parameter `--no-prompt` to support skipping the prompt of missing parameters for ARM template</span></span>
* <span data-ttu-id="5f12f-289">`az deployment group/mg/sub/tenant validate`: Unterstützung von Kommentaren in der Bereitstellungsparameterdatei</span><span class="sxs-lookup"><span data-stu-id="5f12f-289">`az deployment group/mg/sub/tenant validate`: Support comments in deployment parameter file</span></span>
* <span data-ttu-id="5f12f-290">`az deployment`: `is_preview` für Parameter `--handle-extended-json-format` entfernt</span><span class="sxs-lookup"><span data-stu-id="5f12f-290">`az deployment`: Remove `is_preview` for parameter `--handle-extended-json-format`</span></span>
* <span data-ttu-id="5f12f-291">`az deployment group/mg/sub/tenant cancel`: Unterstützung für den Abbruch der Bereitstellung für ARM-Vorlagen</span><span class="sxs-lookup"><span data-stu-id="5f12f-291">`az deployment group/mg/sub/tenant cancel`: Support cancel deployment for ARM template</span></span>
* <span data-ttu-id="5f12f-292">`az deployment group/mg/sub/tenant validate`: Fehlermeldung bei einem Fehler der Bereitstellungsüberprüfung verbessert</span><span class="sxs-lookup"><span data-stu-id="5f12f-292">`az deployment group/mg/sub/tenant validate`: Improve the error message when deployment verification fails</span></span>
* <span data-ttu-id="5f12f-293">`az deployment-scripts`: Neue Befehle für DeploymentScripts hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-293">`az deployment-scripts`: Add new commands for DeploymentScripts</span></span>
* <span data-ttu-id="5f12f-294">`az resource tag`: Parameter `--is-incremental` hinzugefügt, um das inkrementelle Hinzufügen von Tags zur Ressource zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="5f12f-294">`az resource tag`: Add parameter `--is-incremental` to support adding tags to resource incrementally</span></span>

### <a name="aro"></a><span data-ttu-id="5f12f-295">ARO</span><span class="sxs-lookup"><span data-stu-id="5f12f-295">ARO</span></span>

* <span data-ttu-id="5f12f-296">`az aro`:  ARO-Befehlsmodul von Azure RedHat OpenShift V4 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-296">`az aro`:  Add Azure RedHat OpenShift V4 aro command module</span></span>

### <a name="batch"></a><span data-ttu-id="5f12f-297">Batch</span><span class="sxs-lookup"><span data-stu-id="5f12f-297">Batch</span></span>

* <span data-ttu-id="5f12f-298">Batch-API aktualisiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-298">Update Batch API</span></span>

### <a name="compute"></a><span data-ttu-id="5f12f-299">Compute</span><span class="sxs-lookup"><span data-stu-id="5f12f-299">Compute</span></span>

* <span data-ttu-id="5f12f-300">`az sig image-version create`: Speicherkontotyp „Premium_LRS“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-300">`az sig image-version create`: Add storage account type Premium_LRS</span></span>
* <span data-ttu-id="5f12f-301">`az vmss update`: Problem behoben, das beim Aktualisieren der Beendigungsbenachrichtigung auftrat</span><span class="sxs-lookup"><span data-stu-id="5f12f-301">`az vmss update`: Fix terminate notification update issue</span></span>
* <span data-ttu-id="5f12f-302">`az vm/vmss create`: Unterstützung für spezialisierte Imageversion hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-302">`az vm/vmss create`: Add support for specialized image version</span></span>
* <span data-ttu-id="5f12f-303">SIG-API-Version 2019-12-01</span><span class="sxs-lookup"><span data-stu-id="5f12f-303">SIG API Version 2019-12-01</span></span>
* <span data-ttu-id="5f12f-304">`az sig image-version create`: „--target-region-encryption“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-304">`az sig image-version create`: Add --target-region-encryption</span></span>
* <span data-ttu-id="5f12f-305">Fehler bei Serientestausführung behoben, der auf die Duplizierung des Schlüsseltresornamens im globalen In-Memory-Cache zurückzuführen war.</span><span class="sxs-lookup"><span data-stu-id="5f12f-305">Fix tests fail when running in serial due to keyvault name is duplicated in global in-momery cache</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="5f12f-306">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="5f12f-306">CosmosDB</span></span>

* <span data-ttu-id="5f12f-307">Unterstützung für `az cosmosdb private-link-resource/private-endpoint-connection`</span><span class="sxs-lookup"><span data-stu-id="5f12f-307">Support `az cosmosdb private-link-resource/private-endpoint-connection`</span></span>

### <a name="iot-central"></a><span data-ttu-id="5f12f-308">IoT Central</span><span class="sxs-lookup"><span data-stu-id="5f12f-308">IoT Central</span></span>

* <span data-ttu-id="5f12f-309">`az iotcentral` als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="5f12f-309">Deprecate `az iotcentral`</span></span>
* <span data-ttu-id="5f12f-310">Befehlsmodul `az iot central` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-310">Add `az iot central` command module</span></span>

### <a name="monitor"></a><span data-ttu-id="5f12f-311">Überwachen</span><span class="sxs-lookup"><span data-stu-id="5f12f-311">Monitor</span></span>

* <span data-ttu-id="5f12f-312">Unterstützung eines Private Link-Szenarios für die Überwachung</span><span class="sxs-lookup"><span data-stu-id="5f12f-312">Support private link scenario for monitor</span></span>
* <span data-ttu-id="5f12f-313">Falsche Simulationsmethode in „test_monitor_general_operations.py“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-313">Fix wrong mocking way in test_monitor_general_operations.py</span></span>

### <a name="network"></a><span data-ttu-id="5f12f-314">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="5f12f-314">Network</span></span>

* <span data-ttu-id="5f12f-315">SKU für den Befehl zur Aktualisierung der öffentlichen IP-Adresse als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="5f12f-315">Deprecate sku for public ip update command</span></span>
* <span data-ttu-id="5f12f-316">`az network private-endpoint`: Unterstützung für private DNS-Zonengruppe</span><span class="sxs-lookup"><span data-stu-id="5f12f-316">`az network private-endpoint`: Support private dns zone group</span></span>
* <span data-ttu-id="5f12f-317">Feature für lokalen Kontext für VNET-/Subnetzparameter aktiviert</span><span class="sxs-lookup"><span data-stu-id="5f12f-317">Enable local context feature for vnet/subnet parameter</span></span>
* <span data-ttu-id="5f12f-318">Falsches Verwendungsbeispiel in „test_nw_flow_log_delete“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-318">Fix wrong usage example in test_nw_flow_log_delete</span></span>

### <a name="packaging"></a><span data-ttu-id="5f12f-319">Verpackung</span><span class="sxs-lookup"><span data-stu-id="5f12f-319">Packaging</span></span>

* <span data-ttu-id="5f12f-320">Unterstützung für Ubuntu-/Disco-Paket eingestellt</span><span class="sxs-lookup"><span data-stu-id="5f12f-320">Drop support for Ubuntu/Disco package</span></span>

### <a name="rbac"></a><span data-ttu-id="5f12f-321">RBAC</span><span class="sxs-lookup"><span data-stu-id="5f12f-321">RBAC</span></span>

* <span data-ttu-id="5f12f-322">`az ad app create/update`: Unterstützung von „--optional-claims“ als Parameter</span><span class="sxs-lookup"><span data-stu-id="5f12f-322">`az ad app create/update`: support --optional-claims as a parameter</span></span>

### <a name="rdbms"></a><span data-ttu-id="5f12f-323">RDBMS</span><span class="sxs-lookup"><span data-stu-id="5f12f-323">RDBMS</span></span>

* <span data-ttu-id="5f12f-324">Azure Active Directory-Administratorbefehle für PostgreSQL und MySQL hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-324">Add Azure active directory administrator commands for PostgreSQL and MySQL</span></span>

### <a name="service-fabric"></a><span data-ttu-id="5f12f-325">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="5f12f-325">Service Fabric</span></span>

* <span data-ttu-id="5f12f-326">Fehlerbehebung Nr. 12891: `az sf application update --application-parameters` entfernt alte Parameter, die nicht in der Anforderung enthalten sind.</span><span class="sxs-lookup"><span data-stu-id="5f12f-326">Fix #12891: `az sf application update --application-parameters` removes old parameters that are not in the request</span></span>
* <span data-ttu-id="5f12f-327">Fehlerbehebung Nr. 12470: az sf create cluster: Fehler im Zusammenhang mit der Dauerhaftigkeit und Zuverlässigkeit von Updates sowie im Zusammenhang mit der codebasierten Suche der VMSS unter Angabe eines bestimmten Knotentypnamens behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-327">Fix #12470 az sf create cluster, fix bugs in update durability and reliability and find vmss correctly through the code given a node type name</span></span>

### <a name="sql"></a><span data-ttu-id="5f12f-328">SQL</span><span class="sxs-lookup"><span data-stu-id="5f12f-328">SQL</span></span>

* <span data-ttu-id="5f12f-329">`az sql mi op list`, `az sql mi op get`, `az sql mi op cancel` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-329">Add `az sql mi op list`, `az sql mi op get`, `az sql mi op cancel`</span></span>
* <span data-ttu-id="5f12f-330">`az sql midb`: Aktualisieren/Anzeigen der Richtlinie zur langfristigen Aufbewahrung, Anzeigen/Löschen von Sicherungen zur langfristigen Aufbewahrung, Wiederherstellen von Sicherungen zur langfristigen Aufbewahrung</span><span class="sxs-lookup"><span data-stu-id="5f12f-330">`az sql midb`: update/show long term retention policy,  show/delete long term retention backups, restore long term retention backup</span></span>

### <a name="storage"></a><span data-ttu-id="5f12f-331">Storage</span><span class="sxs-lookup"><span data-stu-id="5f12f-331">Storage</span></span>

* <span data-ttu-id="5f12f-332">„azure-mgmt-storage“ auf 9.0.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-332">Upgrade azure-mgmt-storage to 9.0.0</span></span>
* <span data-ttu-id="5f12f-333">`az storage logging off`: Unterstützung für das Ausschalten der Protokollierung für ein Speicherkonto</span><span class="sxs-lookup"><span data-stu-id="5f12f-333">`az storage logging off`: Support turning off logging for a storage account</span></span>
* <span data-ttu-id="5f12f-334">`az storage account update`: Automatische Rotation von Schlüsseln für CMK aktiviert</span><span class="sxs-lookup"><span data-stu-id="5f12f-334">`az storage account update`: Enable key auto-rotated for CMK</span></span>
* <span data-ttu-id="5f12f-335">`az storage account encryption-scope create/update/list/show`: Unterstützung zum Anpassen des Verschlüsselungsbereichs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-335">`az storage account encryption-scope create/update/list/show`: Add support to customize encryption scope</span></span>
* <span data-ttu-id="5f12f-336">`az storage container create`: „--default-encryption-scope“ und „--deny-encryption-scope-override“ hinzugefügt, um den Verschlüsselungsbereich für die Containerebene festzulegen</span><span class="sxs-lookup"><span data-stu-id="5f12f-336">`az storage container create`: Add --default-encryption-scope and --deny-encryption-scope-override to set encryption scope for container level</span></span>

### <a name="survey"></a><span data-ttu-id="5f12f-337">Umfrage</span><span class="sxs-lookup"><span data-stu-id="5f12f-337">Survey</span></span>

* <span data-ttu-id="5f12f-338">Switch zum Deaktivieren des Umfragelinks hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-338">Add switch to turn off survey link</span></span>

## <a name="april-01-2020"></a><span data-ttu-id="5f12f-339">01. April 2020</span><span class="sxs-lookup"><span data-stu-id="5f12f-339">April 01, 2020</span></span>

<span data-ttu-id="5f12f-340">Version 2.3.1</span><span class="sxs-lookup"><span data-stu-id="5f12f-340">Version 2.3.1</span></span>

### <a name="acr"></a><span data-ttu-id="5f12f-341">ACR</span><span class="sxs-lookup"><span data-stu-id="5f12f-341">ACR</span></span>

* <span data-ttu-id="5f12f-342">Falsche Version von „azure-mgmt-containerregistry“ für Linux korrigiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-342">Fix wrong version of azure-mgmt-containerregistry for Linux</span></span>

### <a name="profile"></a><span data-ttu-id="5f12f-343">Profil</span><span class="sxs-lookup"><span data-stu-id="5f12f-343">Profile</span></span>

* <span data-ttu-id="5f12f-344">az login: Anmeldefehler behoben, der auftrat, wenn nicht das Cloudprofil `latest` verwendet wurde</span><span class="sxs-lookup"><span data-stu-id="5f12f-344">az login: Fix login failure with cloud profiles other than `latest`</span></span>

## <a name="march-31-2020"></a><span data-ttu-id="5f12f-345">31. März 2020</span><span class="sxs-lookup"><span data-stu-id="5f12f-345">March 31, 2020</span></span>

<span data-ttu-id="5f12f-346">Version 2.3.0</span><span class="sxs-lookup"><span data-stu-id="5f12f-346">Version 2.3.0</span></span>

### <a name="acr"></a><span data-ttu-id="5f12f-347">ACR</span><span class="sxs-lookup"><span data-stu-id="5f12f-347">ACR</span></span>

* <span data-ttu-id="5f12f-348">„az acr task update“: NULL-Zeiger-Ausnahme</span><span class="sxs-lookup"><span data-stu-id="5f12f-348">'az acr task update': null pointer exception</span></span>
* <span data-ttu-id="5f12f-349">`az acr import`: Hilfe und Fehlermeldung geändert, um die Verwendung von „--source“ und „--registry“ zu verdeutlichen</span><span class="sxs-lookup"><span data-stu-id="5f12f-349">`az acr import`: Modify help and error message to clarify the usage of --source and --registry</span></span>
* <span data-ttu-id="5f12f-350">Überprüfung für das Argument „registry_name“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-350">Add a validator for argument 'registry_name'</span></span>
* <span data-ttu-id="5f12f-351">`az acr login`: Vorschauflag für „--expose-token“ entfernt</span><span class="sxs-lookup"><span data-stu-id="5f12f-351">`az acr login`:Remove the preview flag on '--expose-token'</span></span>
* <span data-ttu-id="5f12f-352">[BREAKING CHANGE] Branch-Parameter „az acr task create/update“ entfernt</span><span class="sxs-lookup"><span data-stu-id="5f12f-352">[BREAKING CHANGE] 'az acr task create/update' Branch parameter is removed</span></span>
* <span data-ttu-id="5f12f-353">„az acr task update“: Kunde kann nun Kontext, Git-Token und/oder Trigger einzeln aktualisieren</span><span class="sxs-lookup"><span data-stu-id="5f12f-353">'az acr task update' Customer now can update context, git-token, and or triggers individually</span></span>
* <span data-ttu-id="5f12f-354">„az acr agentpool“: Neues Feature</span><span class="sxs-lookup"><span data-stu-id="5f12f-354">'az acr agentpool': new feature</span></span>

### <a name="aks"></a><span data-ttu-id="5f12f-355">AKS</span><span class="sxs-lookup"><span data-stu-id="5f12f-355">AKS</span></span>

* <span data-ttu-id="5f12f-356">„apiServerAccessProfile“ bei der Aktualisierung von „--api-server-authorized-ip-ranges“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-356">Fix apiServerAccessProfile when updating --api-server-authorized-ip-ranges</span></span>
* <span data-ttu-id="5f12f-357">aks update: Überschreibung ausgehender IP-Adressen mit Eingabewerten bei der Aktualisierung</span><span class="sxs-lookup"><span data-stu-id="5f12f-357">aks update: Override outbound IPs with input values when update</span></span>
* <span data-ttu-id="5f12f-358">Keine SPN-Erstellung für MSI-Cluster sowie Unterstützung der Anfügung von ACR an MSI-Cluster</span><span class="sxs-lookup"><span data-stu-id="5f12f-358">Do not create SPN for MSI clusters and support attach acr to MSI clusters</span></span>

### <a name="ams"></a><span data-ttu-id="5f12f-359">AMS</span><span class="sxs-lookup"><span data-stu-id="5f12f-359">AMS</span></span>

* <span data-ttu-id="5f12f-360">Fix 12469: Hinzufügen von „content-key-policy“ für Fairplay aufgrund von Problemen mit dem Parameter „ask“ nicht erfolgreich</span><span class="sxs-lookup"><span data-stu-id="5f12f-360">Fix #12469: adding Fairplay content-key-policy fails due to problems with 'ask' parameter</span></span>

### <a name="appconfig"></a><span data-ttu-id="5f12f-361">AppConfig</span><span class="sxs-lookup"><span data-stu-id="5f12f-361">AppConfig</span></span>

* <span data-ttu-id="5f12f-362">„--skip-keyvault“ für „kv export“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-362">Add --skip-keyvault for kv export</span></span>

### <a name="appservice"></a><span data-ttu-id="5f12f-363">AppService</span><span class="sxs-lookup"><span data-stu-id="5f12f-363">AppService</span></span>

* <span data-ttu-id="5f12f-364">Fix 12509: Tag für „az webapp up“ standardmäßig entfernt</span><span class="sxs-lookup"><span data-stu-id="5f12f-364">Fix #12509: Remove the tag to az webapp up by default</span></span>
* <span data-ttu-id="5f12f-365">az functionapp create: Hilfemenü für „--runtime-version“ aktualisiert und Warnung hinzugefügt, wenn der Benutzer „--runtime-version“ für .NET angibt</span><span class="sxs-lookup"><span data-stu-id="5f12f-365">az functionapp create: Updated --runtime-version help menu and added warning when user specifies --runtime-version for dotnet</span></span>
* <span data-ttu-id="5f12f-366">az functionapp create: Methode zum Festlegen von „javaVersion“ für Windows-Funktions-Apps aktualisiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-366">az functionapp create: Updated the way javaVersion was being set for Windows function apps</span></span>

### <a name="arm"></a><span data-ttu-id="5f12f-367">ARM</span><span class="sxs-lookup"><span data-stu-id="5f12f-367">ARM</span></span>

* <span data-ttu-id="5f12f-368">az deployment create/validate: Standardmäßige Verwendung von „--handle-extended-json-format“</span><span class="sxs-lookup"><span data-stu-id="5f12f-368">az deployment create/validate: Use --handle-extended-json-format by default</span></span>
* <span data-ttu-id="5f12f-369">az lock create: Beispiele für die Erstellung einer Unterressource in der Hilfedokumentation hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-369">az lock create: Add examples of creating subresource in the help documentation</span></span>
* <span data-ttu-id="5f12f-370">az deployment {group/mg/sub/tenant} list: Unterstützung der provisioningState-Filterung</span><span class="sxs-lookup"><span data-stu-id="5f12f-370">az deployment {group/mg/sub/tenant} list: Support provisioningState filtering</span></span>
* <span data-ttu-id="5f12f-371">az deployment: Analysefehler für Kommentar unter letztem Argument behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-371">az deployment: Fix the parse bug for comment under the last argument</span></span>

### <a name="backup"></a><span data-ttu-id="5f12f-372">Backup</span><span class="sxs-lookup"><span data-stu-id="5f12f-372">Backup</span></span>

* <span data-ttu-id="5f12f-373">Mehrere Dateiwiederherstellungsfunktionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-373">Added multiple files restore capabilities</span></span>
* <span data-ttu-id="5f12f-374">Unterstützung der ausschließlichen Sicherung von Betriebssystemdatenträgern hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-374">Added support for Backing up OS Disks only</span></span>
* <span data-ttu-id="5f12f-375">Parameter „restore-as-unmanaged-disk“ für die Angabe einer nicht verwalteten Wiederherstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-375">Added restore-as-unmanaged-disk parameter to specify unmanaged restore</span></span>

### <a name="compute"></a><span data-ttu-id="5f12f-376">Compute</span><span class="sxs-lookup"><span data-stu-id="5f12f-376">Compute</span></span>

* <span data-ttu-id="5f12f-377">az vm create: Option „NONE“ von „--nsg-rule“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-377">az vm create: Add NONE option of --nsg-rule</span></span>
* <span data-ttu-id="5f12f-378">az vmss create/update: Vorschautag für automatische VMSS-Reparaturen entfernt</span><span class="sxs-lookup"><span data-stu-id="5f12f-378">az vmss create/update: remove vmss automatic repairs preview tag</span></span>
* <span data-ttu-id="5f12f-379">az vm update: Unterstützung von „--workspace“</span><span class="sxs-lookup"><span data-stu-id="5f12f-379">az vm update: Support --workspace</span></span>
* <span data-ttu-id="5f12f-380">Fehler im VirtualMachineScaleSetExtension-Initialisierungscode behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-380">Fix a bug in VirtualMachineScaleSetExtension initialization code</span></span>
* <span data-ttu-id="5f12f-381">Upgrade der VMAccessAgent-Version auf 2.4 durchgeführt</span><span class="sxs-lookup"><span data-stu-id="5f12f-381">Upgrade VMAccessAgent version to 2.4</span></span>
* <span data-ttu-id="5f12f-382">az vmss set-orchestration-service-state: Unterstützung zum Festlegen des Orchestrierungdienstzustands für VMSS</span><span class="sxs-lookup"><span data-stu-id="5f12f-382">az vmss set-orchestration-service-state: support vmss set orchestration service state</span></span>
* <span data-ttu-id="5f12f-383">Upgrade der Datenträger-API-Version auf 2019-11-01 durchgeführt</span><span class="sxs-lookup"><span data-stu-id="5f12f-383">Upgrade disk API version to 2019-11-01</span></span>
* <span data-ttu-id="5f12f-384">az disk create: add --disk-iops-read-only, --disk-mbps-read-only, --max-shares, --image-reference, --image-reference-lun, --gallery-image-reference, --gallery-image-reference-lun</span><span class="sxs-lookup"><span data-stu-id="5f12f-384">az disk create: add --disk-iops-read-only, --disk-mbps-read-only, --max-shares, --image-reference, --image-reference-lun, --gallery-image-reference, --gallery-image-reference-lun</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="5f12f-385">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="5f12f-385">Cosmos DB</span></span>

* <span data-ttu-id="5f12f-386">Fehlende Option „--type“ für Veraltungsumleitungen korrigiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-386">Fix missing --type option for deprecation redirections</span></span>

### <a name="docker"></a><span data-ttu-id="5f12f-387">Docker</span><span class="sxs-lookup"><span data-stu-id="5f12f-387">Docker</span></span>

* <span data-ttu-id="5f12f-388">Update auf Alpine 3.11 und Python 3.6.10 durchgeführt</span><span class="sxs-lookup"><span data-stu-id="5f12f-388">Update to Alpine 3.11 and Python 3.6.10</span></span>

### <a name="extension"></a><span data-ttu-id="5f12f-389">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="5f12f-389">Extension</span></span>

* <span data-ttu-id="5f12f-390">Laden von Erweiterungen im Systempfad mittels Paketen ermöglicht</span><span class="sxs-lookup"><span data-stu-id="5f12f-390">Allow to load extensions in the system path via packages</span></span>

### <a name="hdinsight"></a><span data-ttu-id="5f12f-391">HDInsight</span><span class="sxs-lookup"><span data-stu-id="5f12f-391">HDInsight</span></span>

* <span data-ttu-id="5f12f-392">(az hdinsight create:) Unterstützung der Angabe der unterstützten TLS-Mindestversion durch Kunden unter Verwendung des Parameters `--minimal-tls-version`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-392">(az hdinsight create:) Support customers specify minimal supported tls version by using parameter `--minimal-tls-version`.</span></span> <span data-ttu-id="5f12f-393">Zulässiger Wert: 1.0,1.1,1.2</span><span class="sxs-lookup"><span data-stu-id="5f12f-393">The allowed value is 1.0,1.1,1.2</span></span>

### <a name="iot"></a><span data-ttu-id="5f12f-394">IoT</span><span class="sxs-lookup"><span data-stu-id="5f12f-394">IoT</span></span>

* <span data-ttu-id="5f12f-395">Codebesitzer hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-395">Add codeowner</span></span>
* <span data-ttu-id="5f12f-396">az iot hub create: Standard-SKU von F1 in S1 geändert</span><span class="sxs-lookup"><span data-stu-id="5f12f-396">az iot hub create : Change default sku to S1 from F1</span></span>
* <span data-ttu-id="5f12f-397">iot hub: Unterstützung von „IotHub“ im Profil „2019-03-01-hybrid“</span><span class="sxs-lookup"><span data-stu-id="5f12f-397">iot hub: Support IotHub in the profile of 2019-03-01-hybrid</span></span>

### <a name="iotcentral"></a><span data-ttu-id="5f12f-398">IoTCentral</span><span class="sxs-lookup"><span data-stu-id="5f12f-398">IoTCentral</span></span>

* <span data-ttu-id="5f12f-399">Fehlerdetails sowie Standardanwendungsvorlage und Aufforderungsmeldung aktualisiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-399">Update error details, update default application template and prompt message</span></span>

### <a name="keyvault"></a><span data-ttu-id="5f12f-400">KeyVault</span><span class="sxs-lookup"><span data-stu-id="5f12f-400">KeyVault</span></span>

* <span data-ttu-id="5f12f-401">Unterstützung von Zertifikatsicherung/-wiederherstellung</span><span class="sxs-lookup"><span data-stu-id="5f12f-401">Support certificate backup/restore</span></span>
* <span data-ttu-id="5f12f-402">keyvault create/update: Unterstützung von „--retention-days“</span><span class="sxs-lookup"><span data-stu-id="5f12f-402">keyvault create/update: Support --retention-days</span></span>
* <span data-ttu-id="5f12f-403">Keine Anzeige von verwalteten Schlüsseln/Geheimnissen bei der Auflistung mehr</span><span class="sxs-lookup"><span data-stu-id="5f12f-403">No longer display managed keys/secrets while listing</span></span>
* <span data-ttu-id="5f12f-404">az keyvault create: Unterstützung von `--network-acls`, `--network-acls-ips` und `--network-acls-vnets` zur Angabe von Netzwerkregeln bei der Tresorerstellung</span><span class="sxs-lookup"><span data-stu-id="5f12f-404">az keyvault create: support `--network-acls`, `--network-acls-ips` and `--network-acls-vnets` for specifying network rules while creating vault</span></span>

### <a name="lock"></a><span data-ttu-id="5f12f-405">Sperre</span><span class="sxs-lookup"><span data-stu-id="5f12f-405">Lock</span></span>

* <span data-ttu-id="5f12f-406">Fehlerbehebung für „az lock delete“: „az lock delete“ funktioniert für „Microsoft.DocumentDB“ nicht.</span><span class="sxs-lookup"><span data-stu-id="5f12f-406">az lock delete fix bug: az lock delete does not work on Microsoft.DocumentDB</span></span>

### <a name="monitor"></a><span data-ttu-id="5f12f-407">Überwachen</span><span class="sxs-lookup"><span data-stu-id="5f12f-407">Monitor</span></span>

* <span data-ttu-id="5f12f-408">az monitor clone: Unterstützung des Klonens von Metrikregeln zwischen Ressourcen</span><span class="sxs-lookup"><span data-stu-id="5f12f-408">az monitor clone: support clone metric rules from one resource to another</span></span>
* <span data-ttu-id="5f12f-409">Fix IcM179210086: Erstellung einer benutzerdefinierten Metrikwarnung für die Application Insights-Metrik nicht möglich</span><span class="sxs-lookup"><span data-stu-id="5f12f-409">Fix IcM179210086: unable to create custom metric alert for their Application Insights metric</span></span>

### <a name="netappfiles"></a><span data-ttu-id="5f12f-410">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="5f12f-410">NetAppFiles</span></span>

* <span data-ttu-id="5f12f-411">az volume create: Datenschutzvolumes zum Hinzufügen von Replikationsvorgängen zugelassen: Genehmigen, Aussetzen, Fortsetzen, Status, Entfernen</span><span class="sxs-lookup"><span data-stu-id="5f12f-411">az volume create: Allow data protection volumes adding replication operations: approve, suspend, resume, status, remove</span></span>

### <a name="network"></a><span data-ttu-id="5f12f-412">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="5f12f-412">Network</span></span>

* <span data-ttu-id="5f12f-413">az network application-gateway waf-policy managed-rule rule-set add: Unterstützung von „ Microsoft_BotManagerRuleSet“</span><span class="sxs-lookup"><span data-stu-id="5f12f-413">az network application-gateway waf-policy managed-rule rule-set add: support Microsoft_BotManagerRuleSet</span></span>
* <span data-ttu-id="5f12f-414">network watcher flow-log show: Falsche Veraltungsinformationen behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-414">network watcher flow-log show: fix wrong deprecating info</span></span>
* <span data-ttu-id="5f12f-415">Unterstützung von Hostnamen im Application Gateway-Listener</span><span class="sxs-lookup"><span data-stu-id="5f12f-415">support host names in application gateway listener</span></span>
* <span data-ttu-id="5f12f-416">az network nat gateway: Unterstützung der Erstellung einer leeren Ressource ohne öffentliche IP-Adresse oder Präfix für öffentliche IP-Adressen</span><span class="sxs-lookup"><span data-stu-id="5f12f-416">az network nat gateway: support create empty resource without public ip or public ip prefix</span></span>
* <span data-ttu-id="5f12f-417">Unterstützung der VPN-Gateway-Generierung</span><span class="sxs-lookup"><span data-stu-id="5f12f-417">Support vpn gateway generation</span></span>
* <span data-ttu-id="5f12f-418">Unterstützung von `--if-none-match` in `az network dns record-set {} add-record`</span><span class="sxs-lookup"><span data-stu-id="5f12f-418">Support `--if-none-match` in `az network dns record-set {} add-record`</span></span>

### <a name="packaging"></a><span data-ttu-id="5f12f-419">Verpackung</span><span class="sxs-lookup"><span data-stu-id="5f12f-419">Packaging</span></span>

* <span data-ttu-id="5f12f-420">Unterstützung von Python 3.5 eingestellt</span><span class="sxs-lookup"><span data-stu-id="5f12f-420">Drop support for python 3.5</span></span>

### <a name="profile"></a><span data-ttu-id="5f12f-421">Profil</span><span class="sxs-lookup"><span data-stu-id="5f12f-421">Profile</span></span>

* <span data-ttu-id="5f12f-422">az login: Warnung für MFA-Fehler</span><span class="sxs-lookup"><span data-stu-id="5f12f-422">az login: Show warning for MFA error</span></span>

### <a name="rdbms"></a><span data-ttu-id="5f12f-423">RDBMS</span><span class="sxs-lookup"><span data-stu-id="5f12f-423">RDBMS</span></span>

* <span data-ttu-id="5f12f-424">Befehle zur Verwaltung von Verschlüsselungsschlüsseln für Serverdaten für PostgreSQL und MySQL hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-424">Add server data encryption key management commands for PostgreSQL and MySQL</span></span>

## <a name="march-10-2020"></a><span data-ttu-id="5f12f-425">10. März 2020</span><span class="sxs-lookup"><span data-stu-id="5f12f-425">March 10, 2020</span></span>

<span data-ttu-id="5f12f-426">Version 2.2.0</span><span class="sxs-lookup"><span data-stu-id="5f12f-426">Version 2.2.0</span></span>

### <a name="acr"></a><span data-ttu-id="5f12f-427">ACR</span><span class="sxs-lookup"><span data-stu-id="5f12f-427">ACR</span></span>

* <span data-ttu-id="5f12f-428">Fix: `az acr login` löst fälschlicherweise Fehler aus</span><span class="sxs-lookup"><span data-stu-id="5f12f-428">Fix: `az acr login` wrongly raise error</span></span>
* <span data-ttu-id="5f12f-429">Neuer Befehl `az acr helm install-cli` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-429">Add new command `az acr helm install-cli`</span></span>
* <span data-ttu-id="5f12f-430">Privater Link und CMK-Unterstützung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-430">Add private link and CMK support</span></span>
* <span data-ttu-id="5f12f-431">Befehl „private-link-resource list“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-431">add 'private-link-resource list' command</span></span>

### <a name="aks"></a><span data-ttu-id="5f12f-432">AKS</span><span class="sxs-lookup"><span data-stu-id="5f12f-432">AKS</span></span>

* <span data-ttu-id="5f12f-433">Durchsuchen von AKS in Cloud-Shell korrigiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-433">fix the aks browse in cloud shell</span></span>
* <span data-ttu-id="5f12f-434">az aks: NoneType-Fehler beim Überwachen von „addon“ und „agentpool“ behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-434">az aks: Fix monitoring addon and agentpool NoneType errors</span></span>
* <span data-ttu-id="5f12f-435">„--nodepool-tags“ zum Knotenpool beim Erstellen von Azure-Kubernetes-Clustern hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-435">Add --nodepool-tags to node pool when creating azure kubernetes cluster</span></span>
* <span data-ttu-id="5f12f-436">„--tags“ beim Hinzufügen oder Aktualisieren eines Knotenpool in einem Cluster hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-436">Add --tags when adding or updating a nodepool to cluster</span></span>
* <span data-ttu-id="5f12f-437">aks create: `--enable-private-cluster` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-437">aks create: add `--enable-private-cluster`</span></span>
* <span data-ttu-id="5f12f-438">„--nodepool-labels“ beim Erstellen von Azure-Kubernetes-Clustern hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-438">add --nodepool-labels when creating azure kubernetes cluster</span></span>
* <span data-ttu-id="5f12f-439">„--labels“ beim Hinzufügen eines neuen Knotenpools zu einem Azure-Kubernetes-Cluster hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-439">add --labels when adding a new nodepool to azure kubernetes cluster</span></span>
* <span data-ttu-id="5f12f-440">Fehlender Schrägstrich (/) in der Dashboard-URL hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-440">add missing / in the dashboard url</span></span>
* <span data-ttu-id="5f12f-441">Unterstützung der Erstellung von AKS-Clustern, sodass verwaltete Identitäten möglich sind</span><span class="sxs-lookup"><span data-stu-id="5f12f-441">Support create aks clusters enabling managed identity</span></span>
* <span data-ttu-id="5f12f-442">az aks: Überprüfen, ob das Netzwerk-Plug-In entweder „azure“ oder „kubenet“ ist</span><span class="sxs-lookup"><span data-stu-id="5f12f-442">az aks: Validate network plugin to be either "azure" or "kubenet"</span></span>
* <span data-ttu-id="5f12f-443">az aks: Unterstützung für AAD-Sitzungsschlüssel hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-443">az aks: Add aad session key support</span></span>
* <span data-ttu-id="5f12f-444">[BREAKING CHANGE] az aks: Unterstützung von MSI-Änderungen für GF und BF für omsagent (Containerüberwachung)(#1)</span><span class="sxs-lookup"><span data-stu-id="5f12f-444">[BREAKING CHANGE] az aks: support msi changes for GF and BF for omsagent (Container monitoring)(#1)</span></span>
* <span data-ttu-id="5f12f-445">az aks use-dev-spaces: Endpunkt-Typoption zum Befehl „use-dev-spaces“, hinzugefügt, um den auf einem Azure Dev Spaces-Controller erstellten Endpunkt anzupassen</span><span class="sxs-lookup"><span data-stu-id="5f12f-445">az aks use-dev-spaces: Adding endpoint type option to the use-dev-spaces command to customize the endpoint created on an Azure Dev Spaces controller</span></span>

### <a name="appconfig"></a><span data-ttu-id="5f12f-446">AppConfig</span><span class="sxs-lookup"><span data-stu-id="5f12f-446">AppConfig</span></span>

* <span data-ttu-id="5f12f-447">Verwendung von „kv set“ entsperrt, um Schlüsseltresorverweis und -funktion hinzuzufügen …</span><span class="sxs-lookup"><span data-stu-id="5f12f-447">Unblock using "kv set" to add keyvault reference and feature …</span></span>

### <a name="appservice"></a><span data-ttu-id="5f12f-448">AppService</span><span class="sxs-lookup"><span data-stu-id="5f12f-448">AppService</span></span>

* <span data-ttu-id="5f12f-449">az webapp create : Beheben eines Problems beim Ausführen des Befehls mit „--runtime“</span><span class="sxs-lookup"><span data-stu-id="5f12f-449">az webapp create : Fix issue when running the command with --runtime</span></span>
* <span data-ttu-id="5f12f-450">az functionapp deployment source config-zip: Fehlermeldung hinzugefügt, wenn der Ressourcengruppen- oder Funktionsname ungültig oder nicht vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="5f12f-450">az functionapp deployment source config-zip: Add an error message if resource group or function name are invalid/don't exist</span></span>
* <span data-ttu-id="5f12f-451">functionapp create: Warnmeldung korrigiert, die derzeit mit `functionapp create` angezeigt wird und ein `--functions_version`-Flag angibt, aber irrtümlich ein `_` anstelle eines `-` im Flagnamen verwendet</span><span class="sxs-lookup"><span data-stu-id="5f12f-451">functionapp create: Fix the warning message that appears with `functionapp create` today which cites a `--functions_version` flag but erroneously uses a `_` instead of a `-` in the flag name</span></span>
* <span data-ttu-id="5f12f-452">az functionapp create: Es wurde aktualisiert, wie linuxFxVersion und der Containerimagename für Linux-Funktions-Apps festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="5f12f-452">az functionapp create: Updated the way linuxFxVersion and container image name were being set for linux function apps</span></span>
* <span data-ttu-id="5f12f-453">az functionapp deployment source config-zip: Problems behoben, das durch die Racebedingung für die Änderung von App-Einstellungen während der ZIP-Bereitstellung verursacht wird und während der Bereitstellung 5xx-Fehler ausgibt</span><span class="sxs-lookup"><span data-stu-id="5f12f-453">az functionapp deployment source config-zip: Fix an issue caused by app settings change racing condition during zip deploy, giving 5xx errors during deployment</span></span>
* <span data-ttu-id="5f12f-454">Fix #5720946: „az webapp backup“ legt Namen nicht fest</span><span class="sxs-lookup"><span data-stu-id="5f12f-454">Fix #5720946: az webapp backup fails to set name</span></span>

### <a name="arm"></a><span data-ttu-id="5f12f-455">ARM</span><span class="sxs-lookup"><span data-stu-id="5f12f-455">ARM</span></span>

* <span data-ttu-id="5f12f-456">az resource: Beispiele für das Ressourcenmodul verbessert</span><span class="sxs-lookup"><span data-stu-id="5f12f-456">az resource: Improve the examples of the resource module</span></span>
* <span data-ttu-id="5f12f-457">az policy assignment list: Unterstützung für das Auflisten von Richtlinienzuweisungen im Verwaltungsgruppenbereich</span><span class="sxs-lookup"><span data-stu-id="5f12f-457">az policy assignment list: Support listing policy assignments at Management Group scope</span></span>
* <span data-ttu-id="5f12f-458">`az deployment group` und `az deployment operation group` für Vorlagenbereitstellung in Ressourcengruppen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-458">Add `az deployment group` and `az deployment operation group` for template deployment at resource groups.</span></span> <span data-ttu-id="5f12f-459">Dies ist ein Duplikat von `az group deployment` und `az group deployment operation`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-459">This is a duplicate of `az group deployment` and `az group deployment operation`</span></span>
* <span data-ttu-id="5f12f-460">`az deployment sub` und `az deployment operation sub` für Vorlagenbereitstellung im Abonnementbereich hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-460">Add `az deployment sub` and `az deployment operation sub` for template deployment at subscription scope.</span></span> <span data-ttu-id="5f12f-461">Dies ist ein Duplikat von `az deployment` und `az deployment operation`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-461">This is a duplicate of `az deployment` and `az deployment operation`</span></span>
* <span data-ttu-id="5f12f-462">`az deployment mg` und `az deployment operation mg` für Vorlagenbereitstellung in Verwaltungsgruppen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-462">Add `az deployment mg` and `az deployment operation mg` for template deployment at management groups</span></span>
* <span data-ttu-id="5f12f-463">`az deployment tenant` und `az deployment operation tenant` für Vorlagenbereitstellung im Mandantenbereich hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-463">Add `az deployment tenant` and `az deployment operation tenant` for template deployment at tenant scope</span></span>
* <span data-ttu-id="5f12f-464">az policy assignment create: Beschreibung zu Parameter `--location` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-464">az policy assignment create: Add a description to the `--location` parameter</span></span>
* <span data-ttu-id="5f12f-465">az group deployment create: Parameter `--aux-tenants` zur mandantenübergreifenden Unterstützung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-465">az group deployment create: Add parameter `--aux-tenants` to support cross tenants</span></span>

### <a name="cdn"></a><span data-ttu-id="5f12f-466">CDN</span><span class="sxs-lookup"><span data-stu-id="5f12f-466">CDN</span></span>

* <span data-ttu-id="5f12f-467">CDN-WAF-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-467">Add CDN WAF commands</span></span>

### <a name="compute"></a><span data-ttu-id="5f12f-468">Compute</span><span class="sxs-lookup"><span data-stu-id="5f12f-468">Compute</span></span>

* <span data-ttu-id="5f12f-469">az sig image-version: „--data-snapshot-luns“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-469">az sig image-version: add --data-snapshot-luns</span></span>
* <span data-ttu-id="5f12f-470">az ppg show: „--colocation-status“ hinzugefügt, um das Abrufen des Zusammenstellungsstatus aller Ressourcen in der Näherungsplatzierungsgruppe zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="5f12f-470">az ppg show: add --colocation-status to enable fetching the colocation status of all the resources in the proximity placement group</span></span>
* <span data-ttu-id="5f12f-471">az vmss create/update: Unterstützung automatischer Reparaturen</span><span class="sxs-lookup"><span data-stu-id="5f12f-471">az vmss create/update: support automatic repairs</span></span>
* <span data-ttu-id="5f12f-472">[BREAKING CHANGE] az image template: „template“ in „builder“ umbenannt</span><span class="sxs-lookup"><span data-stu-id="5f12f-472">[BREAKING CHANGE] az image template: rename template to builder</span></span>
* <span data-ttu-id="5f12f-473">az image builder create: „--image-template“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-473">az image builder create: add --image-template</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="5f12f-474">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="5f12f-474">Cosmos DB</span></span>

* <span data-ttu-id="5f12f-475">Gespeicherte Prozedur „Add Sql“, udf- und trigger-Cmdlets hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-475">Add Sql stored procedure, udf and trigger cmdlets</span></span>
* <span data-ttu-id="5f12f-476">az cosmosdb create: „--key-uri“ hinzugefügt, um das Hinzufügen von Schlüsseltresor-Verschlüsselungsinformationen zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="5f12f-476">az cosmosdb create: add --key-uri to support adding key vault encryption information</span></span>

### <a name="keyvault"></a><span data-ttu-id="5f12f-477">KeyVault</span><span class="sxs-lookup"><span data-stu-id="5f12f-477">KeyVault</span></span>

* <span data-ttu-id="5f12f-478">keyvault create: „soft-delete“ standardmäßig aktiviert</span><span class="sxs-lookup"><span data-stu-id="5f12f-478">keyvault create: enable soft-delete by default</span></span>

### <a name="monitor"></a><span data-ttu-id="5f12f-479">Überwachen</span><span class="sxs-lookup"><span data-stu-id="5f12f-479">Monitor</span></span>

* <span data-ttu-id="5f12f-480">az monitor metrics alert create: Unterstützung von `~` in `--condition`</span><span class="sxs-lookup"><span data-stu-id="5f12f-480">az monitor metrics alert create: support `~` in `--condition`</span></span>

### <a name="network"></a><span data-ttu-id="5f12f-481">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="5f12f-481">Network</span></span>

* <span data-ttu-id="5f12f-482">az network application-gateway rewrite-rule create: Unterstützung der URL-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="5f12f-482">az network application-gateway rewrite-rule create: support url configuration</span></span>
* <span data-ttu-id="5f12f-483">az network dns zone import: Bei „--zone-name“ wird die Groß-/Kleinschreibung künftig nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="5f12f-483">az network dns zone import: --zone-name will be case insensitive in the future</span></span>
* <span data-ttu-id="5f12f-484">az network private-endpoint/private-link-service: Vorschaubezeichnung entfernt</span><span class="sxs-lookup"><span data-stu-id="5f12f-484">az network private-endpoint/private-link-service: remove preview label</span></span>
* <span data-ttu-id="5f12f-485">az network bastion: Unterstützung von „bastion“</span><span class="sxs-lookup"><span data-stu-id="5f12f-485">az network bastion: support bastion</span></span>
* <span data-ttu-id="5f12f-486">az network vnet list-available-ips: Unterstützung für das Auflisten verfügbarer IPs in einem VNET</span><span class="sxs-lookup"><span data-stu-id="5f12f-486">az network vnet list-available-ips: support list available ips in a vnet</span></span>
* <span data-ttu-id="5f12f-487">az network watcher flow-log create/list/delete/update: neue Befehle hinzugefügt, um Watcher-Datenflussprotokolle zu verwalten und „--location“ zur expliziten Identifizierung von Watcher verfügbar zu machen</span><span class="sxs-lookup"><span data-stu-id="5f12f-487">az network watcher flow-log create/list/delete/update: add new commands to manage watcher flow log and exposing --location to identify watcher explicitly</span></span>
* <span data-ttu-id="5f12f-488">az network watcher flow-log configure: veraltet</span><span class="sxs-lookup"><span data-stu-id="5f12f-488">az network watcher flow-log configure: deprecated</span></span>
* <span data-ttu-id="5f12f-489">az network watcher flow-log show: Unterstützung von „--location“ und „--name“, um ein ARM-formatiertes Ergebnis zu erhalten; alte formatierte Ausgabe als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-489">az network watcher flow-log show: support --location and --name to get ARM-formatted result, deprecated old formatted output</span></span>

### <a name="policy"></a><span data-ttu-id="5f12f-490">Richtlinie</span><span class="sxs-lookup"><span data-stu-id="5f12f-490">Policy</span></span>

* <span data-ttu-id="5f12f-491">az policy assignment create: Fehler behoben, dass automatisch generierter Name der Richtlinienzuweisung den Grenzwert überschreitet</span><span class="sxs-lookup"><span data-stu-id="5f12f-491">az policy assignment create: Fix the bug that automatically generated name of policy assignment exceeds the limit</span></span>

### <a name="rbac"></a><span data-ttu-id="5f12f-492">RBAC</span><span class="sxs-lookup"><span data-stu-id="5f12f-492">RBAC</span></span>

* <span data-ttu-id="5f12f-493">az ad group show: Problem behoben, dass „--group“-Wert als regulärer Ausdruck behandelt wurde</span><span class="sxs-lookup"><span data-stu-id="5f12f-493">az ad group show: fix --group value treated as regex problem</span></span>

### <a name="rdbms"></a><span data-ttu-id="5f12f-494">RDBMS</span><span class="sxs-lookup"><span data-stu-id="5f12f-494">RDBMS</span></span>

* <span data-ttu-id="5f12f-495">SDK-Version von „azure-mgmt-rdbms“ auf 2.0.0 festgelegt</span><span class="sxs-lookup"><span data-stu-id="5f12f-495">Bump the azure-mgmt-rdbms SDK version to 2.0.0</span></span>
* <span data-ttu-id="5f12f-496">az postgres private-endpoint-connection: Verwalten von Verbindungen mit privatem Postgres-Endpunkt</span><span class="sxs-lookup"><span data-stu-id="5f12f-496">az postgres private-endpoint-connection: manage postgres private endpoint connections</span></span>
* <span data-ttu-id="5f12f-497">az postgres private-link-resource: Verwalten von privaten Postgres-Linkressourcen</span><span class="sxs-lookup"><span data-stu-id="5f12f-497">az postgres private-link-resource: manage postgres private link resources</span></span>
* <span data-ttu-id="5f12f-498">az mysql private-endpoint-connection: Verwalten von Verbindungen mit privatem MySQL-Endpunkt</span><span class="sxs-lookup"><span data-stu-id="5f12f-498">az mysql private-endpoint-connection: manage mysql private endpoint connections</span></span>
* <span data-ttu-id="5f12f-499">az mysql private-link-resource: Verwalten von privaten MySQL-Linkressourcen</span><span class="sxs-lookup"><span data-stu-id="5f12f-499">az mysql private-link-resource: manage mysql private link resources</span></span>
* <span data-ttu-id="5f12f-500">az mariadb private-endpoint-connection: Verwalten von Verbindungen mit privatem MariaDB-Endpunkt</span><span class="sxs-lookup"><span data-stu-id="5f12f-500">az mariadb private-endpoint-connection: manage mariadb private endpoint connections</span></span>
* <span data-ttu-id="5f12f-501">az mariadb private-link-resource: Verwalten von privaten MariaDB-Linkressourcen</span><span class="sxs-lookup"><span data-stu-id="5f12f-501">az mariadb private-link-resource: manage mariadb private link resources</span></span>
* <span data-ttu-id="5f12f-502">Aktualisieren von Tests von privaten RDBMS-Endpunkten</span><span class="sxs-lookup"><span data-stu-id="5f12f-502">Updating RDBMS Private Endpoint Tests</span></span>

### <a name="sql"></a><span data-ttu-id="5f12f-503">SQL</span><span class="sxs-lookup"><span data-stu-id="5f12f-503">SQL</span></span>

* <span data-ttu-id="5f12f-504">Sql midb: list-deleted, show-deleted, update-retention, show-retention hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-504">Sql midb Add: list-deleted, show-deleted, update-retention, show-retention</span></span>
* <span data-ttu-id="5f12f-505">(sql server create:) Optionales Flag „Enable“/„Disable“ für public-network-access zu „sql server create“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-505">(sql server create:) Add optional public-network-access 'Enable'/'Disable' flag to sql server create</span></span>
* <span data-ttu-id="5f12f-506">(sql server update): kundenorientierte Änderung vorgenommen</span><span class="sxs-lookup"><span data-stu-id="5f12f-506">(sql server update:) make some customer-facing change</span></span>
* <span data-ttu-id="5f12f-507">Eigenschaft „minimal_tls_version“ für MI und SQL-Datenbank hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-507">Add minimal_tls_version property for MI and SQL DB</span></span>

### <a name="storage"></a><span data-ttu-id="5f12f-508">Storage</span><span class="sxs-lookup"><span data-stu-id="5f12f-508">Storage</span></span>

* <span data-ttu-id="5f12f-509">az storage blob delete-batch: Flag `--dryrun` mit Fehlverhalten</span><span class="sxs-lookup"><span data-stu-id="5f12f-509">az storage blob delete-batch: Misbehaving `--dryrun` flag</span></span>
* <span data-ttu-id="5f12f-510">az storage account network-rule hinzugefügt (Fehlerbehebung): Hinzufügen von Vorgängen muss idempotent sein</span><span class="sxs-lookup"><span data-stu-id="5f12f-510">az storage account network-rule add (bug fix): add operation should be idempotent</span></span>
* <span data-ttu-id="5f12f-511">az storage account create/update: Unterstützung für Routingpräferenz hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-511">az storage account create/update: Add Routing Preference support</span></span>
* <span data-ttu-id="5f12f-512">„azure-mgmt-storage“ auf Version 8.0.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-512">Upgrade azure-mgmt-storage version to 8.0.0</span></span>
* <span data-ttu-id="5f12f-513">az storage container immutability create: Parameter „--allow-protected-append-write“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-513">az storage container immutability create: add --allow-protected-append-write parameter</span></span>
* <span data-ttu-id="5f12f-514">az storage account private-link-resource list: Unterstützung zum Auflisten privater Linkressourcen für Speicherkonto hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-514">az storage account private-link-resource list: Add support to list private link resources for storage account</span></span>
* <span data-ttu-id="5f12f-515">az storage account private-endpoint-connection approve/reject/show/delete: Unterstützung der Verwaltung von Verbindungen mit privaten Endpunkten</span><span class="sxs-lookup"><span data-stu-id="5f12f-515">az storage account private-endpoint-connection approve/reject/show/delete: Support to manage private endpoint connections</span></span>
* <span data-ttu-id="5f12f-516">az storage account blob-service-properties update: „--enable-restore-policy“ und „--restore-days“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-516">az storage account blob-service-properties update: add --enable-restore-policy and --restore-days</span></span>
* <span data-ttu-id="5f12f-517">az storage blob restore: Unterstützung für die Wiederherstellung von Blobbereichen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-517">az storage blob restore: Add support to restore blob ranges</span></span>

## <a name="february-18-2020"></a><span data-ttu-id="5f12f-518">18. Februar 2020</span><span class="sxs-lookup"><span data-stu-id="5f12f-518">February 18, 2020</span></span>

<span data-ttu-id="5f12f-519">Version 2.1.0</span><span class="sxs-lookup"><span data-stu-id="5f12f-519">Version 2.1.0</span></span>

### <a name="acr"></a><span data-ttu-id="5f12f-520">ACR</span><span class="sxs-lookup"><span data-stu-id="5f12f-520">ACR</span></span>

* <span data-ttu-id="5f12f-521">Neues Argument `--expose-token` für `az acr login` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-521">Add a new argument `--expose-token` for `az acr login`</span></span>
* <span data-ttu-id="5f12f-522">Falsche Ausgabe für `az acr task identity show -n Name -r Registry -o table` korrigiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-522">Fix the incorrect output of `az acr task identity show -n Name -r Registry -o table`</span></span>
* <span data-ttu-id="5f12f-523">az acr login: Auslösen von „CLIError“, wenn vom Docker-Befehl Fehler zurückgegeben werden</span><span class="sxs-lookup"><span data-stu-id="5f12f-523">az acr login: Throw a CLIError if there are errors returned by docker command</span></span>

### <a name="acs"></a><span data-ttu-id="5f12f-524">ACS</span><span class="sxs-lookup"><span data-stu-id="5f12f-524">ACS</span></span>

* <span data-ttu-id="5f12f-525">aks create/update: Validierung für `--vnet-subnet-id` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-525">aks create/update: add `--vnet-subnet-id` validation</span></span>

### <a name="aladdin"></a><span data-ttu-id="5f12f-526">Aladdin</span><span class="sxs-lookup"><span data-stu-id="5f12f-526">Aladdin</span></span>

* <span data-ttu-id="5f12f-527">Analysieren der generierten Beispiele in „_help.py“ der Befehle</span><span class="sxs-lookup"><span data-stu-id="5f12f-527">Parse generated examples into commands' _help.py</span></span>

### <a name="ams"></a><span data-ttu-id="5f12f-528">AMS</span><span class="sxs-lookup"><span data-stu-id="5f12f-528">AMS</span></span>

* <span data-ttu-id="5f12f-529">az ams ist jetzt allgemein verfügbar.</span><span class="sxs-lookup"><span data-stu-id="5f12f-529">az ams is GA now</span></span>

### <a name="appconfig"></a><span data-ttu-id="5f12f-530">AppConfig</span><span class="sxs-lookup"><span data-stu-id="5f12f-530">AppConfig</span></span>

* <span data-ttu-id="5f12f-531">Hilfenachricht überarbeitet, um nicht unterstützte Schlüssel-/Bezeichnungsfilter auszuschließen</span><span class="sxs-lookup"><span data-stu-id="5f12f-531">Revise help message to exclude unsupported key/label filter</span></span>
* <span data-ttu-id="5f12f-532">Vorschautag für die meisten Befehle entfernt (mit Ausnahme der Flags für verwaltete Identitäten und Features)</span><span class="sxs-lookup"><span data-stu-id="5f12f-532">Remove preview tag for most commands excluding managed identity and feature flags</span></span>
* <span data-ttu-id="5f12f-533">Kundenseitig verwalteter Schlüssel beim Aktualisieren der Speicher hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-533">Add customer managed key when updating stores</span></span>

### <a name="appservice"></a><span data-ttu-id="5f12f-534">AppService</span><span class="sxs-lookup"><span data-stu-id="5f12f-534">AppService</span></span>

* <span data-ttu-id="5f12f-535">az webapp list-runtimes: Fehler bei „list-runtimes“ behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-535">az webapp list-runtimes: Fix the bug for list-runtimes</span></span>
* <span data-ttu-id="5f12f-536">„az webapp|functionapp config ssl create“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-536">Add az webapp|functionapp config ssl create</span></span>
* <span data-ttu-id="5f12f-537">Unterstützung für v3-Funktions-Apps und Node 12</span><span class="sxs-lookup"><span data-stu-id="5f12f-537">Add support for v3 function apps and node 12</span></span>

### <a name="arm"></a><span data-ttu-id="5f12f-538">ARM</span><span class="sxs-lookup"><span data-stu-id="5f12f-538">ARM</span></span>

* <span data-ttu-id="5f12f-539">az policy assignment create: Fehlermeldung korrigiert, die angezeigt wird, wenn der Parameter `--policy` ungültig ist</span><span class="sxs-lookup"><span data-stu-id="5f12f-539">az policy assignment create: Fix the error message when the `--policy` parameter is invalid</span></span>
* <span data-ttu-id="5f12f-540">az group deployment create: Fehler „stat: path too long for Windows" korrigiert, der angezeigt wird, wenn eine zu große Datei vom Typ „parameters.json“ verwendet wird</span><span class="sxs-lookup"><span data-stu-id="5f12f-540">az group deployment create: Fix "stat: path too long for Windows" error when using large parameters.json file</span></span>

### <a name="backup"></a><span data-ttu-id="5f12f-541">Backup</span><span class="sxs-lookup"><span data-stu-id="5f12f-541">Backup</span></span>

* <span data-ttu-id="5f12f-542">Korrektur des Wiederherstellungsflows auf Elementebene am ursprünglichen Speicherort</span><span class="sxs-lookup"><span data-stu-id="5f12f-542">Fix for item level recovery flow in OLR</span></span>
* <span data-ttu-id="5f12f-543">Unterstützung von „Als Dateien wiederherstellen“ für SQL- und SAP-Datenbanken hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-543">Add restore as files support for SQL and SAP Databases</span></span>

### <a name="compute"></a><span data-ttu-id="5f12f-544">Compute</span><span class="sxs-lookup"><span data-stu-id="5f12f-544">Compute</span></span>

* <span data-ttu-id="5f12f-545">vm/vmss/availability-set update: „--ppg“ hinzugefügt, um die Aktualisierung von „ProximityPlacementGroup“ zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="5f12f-545">vm/vmss/availability-set update: add --ppg to allowing updating ProximityPlacementGroup</span></span>
* <span data-ttu-id="5f12f-546">vmss create: „--data-disk-iops“ und „--data-disk-mbps“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-546">vmss create: add --data-disk-iops and --data-disk-mbps</span></span>
* <span data-ttu-id="5f12f-547">az vm host: Vorschautag für `vm host` und `vm host group` entfernt</span><span class="sxs-lookup"><span data-stu-id="5f12f-547">az vm host: remove preview tag for `vm host` and `vm host group`</span></span>
* <span data-ttu-id="5f12f-548">[BREAKING CHANGE] Behebung Nr. 10728: `az vm create`: Automatisches Erstellen des Subnetzes, wenn das VNET angegeben wird und das Subnetz nicht vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="5f12f-548">[BREAKING CHANGE] Fix #10728: `az vm create`: create subnet automatically if vnet is specified and subnet not exists</span></span>
* <span data-ttu-id="5f12f-549">Erhöhen der Stabilität von „vm image list“</span><span class="sxs-lookup"><span data-stu-id="5f12f-549">Increase robustness of vm image list</span></span>

### <a name="eventhub"></a><span data-ttu-id="5f12f-550">Eventhub</span><span class="sxs-lookup"><span data-stu-id="5f12f-550">Eventhub</span></span>

* <span data-ttu-id="5f12f-551">Azure Stack-Unterstützung für Profil „2019-03-01-hybrid“</span><span class="sxs-lookup"><span data-stu-id="5f12f-551">Azure Stack support for 2019-03-01-hybrid profile</span></span>

### <a name="keyvault"></a><span data-ttu-id="5f12f-552">KeyVault</span><span class="sxs-lookup"><span data-stu-id="5f12f-552">KeyVault</span></span>

* <span data-ttu-id="5f12f-553">az keyvault key create: neuer Wert `import` für Parameter `--ops` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-553">az keyvault key create: add a new value `import` for parameter `--ops`</span></span>
* <span data-ttu-id="5f12f-554">az keyvault key list-versions: Unterstützung des Parameters `--id` für die Angabe von Schlüsseln</span><span class="sxs-lookup"><span data-stu-id="5f12f-554">az keyvault key list-versions: support parameter `--id` for specifying keys</span></span>
* <span data-ttu-id="5f12f-555">Unterstützung für Verbindungen mit privaten Endpunkten</span><span class="sxs-lookup"><span data-stu-id="5f12f-555">Support private endpoint connections</span></span>

### <a name="network"></a><span data-ttu-id="5f12f-556">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="5f12f-556">Network</span></span>

* <span data-ttu-id="5f12f-557">Geändert in „azure-mgmt-network 9.0.0“</span><span class="sxs-lookup"><span data-stu-id="5f12f-557">Bump to azure-mgmt-network 9.0.0</span></span>
* <span data-ttu-id="5f12f-558">az network private-link-service update/create: Unterstützung von „--enable-proxy-protocol“</span><span class="sxs-lookup"><span data-stu-id="5f12f-558">az network private-link-service update/create: support --enable-proxy-protocol</span></span>
* <span data-ttu-id="5f12f-559">Feature für Version 2 von Verbindungsmonitor hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-559">Add connection Monitor V2 feature</span></span>

### <a name="packaging"></a><span data-ttu-id="5f12f-560">Verpackung</span><span class="sxs-lookup"><span data-stu-id="5f12f-560">Packaging</span></span>

* <span data-ttu-id="5f12f-561">[BREAKING CHANGE] Unterstützung für Python 2.7 eingestellt</span><span class="sxs-lookup"><span data-stu-id="5f12f-561">[BREAKING CHANGE] Drop support for Python 2.7</span></span>

### <a name="profile"></a><span data-ttu-id="5f12f-562">Profil</span><span class="sxs-lookup"><span data-stu-id="5f12f-562">Profile</span></span>

* <span data-ttu-id="5f12f-563">Vorschau: Neue Attribute `homeTenantId` und `managedByTenants` zu Abonnementkonten hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-563">Preview: Add new attributes `homeTenantId` and `managedByTenants` to subscription accounts.</span></span> <span data-ttu-id="5f12f-564">Führen Sie `az login` erneut aus, damit die Änderungen wirksam werden.</span><span class="sxs-lookup"><span data-stu-id="5f12f-564">Please re-run `az login` for the changes to take effect</span></span>
* <span data-ttu-id="5f12f-565">az login: Eine Warnung wird angezeigt, wenn ein Abonnement von mehren Mandanten aufgeführt wird und der erste als Standard festgelegt wird.</span><span class="sxs-lookup"><span data-stu-id="5f12f-565">az login: Show a warning when a subscription is listed from more than one tenants and default to the first one.</span></span> <span data-ttu-id="5f12f-566">Fügen Sie `--tenant` in `az login` ein, um beim Zugreifen auf dieses Abonnement einen bestimmten Mandanten auszuwählen.</span><span class="sxs-lookup"><span data-stu-id="5f12f-566">To select a specific tenant when accessing this subscription, please include `--tenant` in `az login`</span></span>

### <a name="role"></a><span data-ttu-id="5f12f-567">Role</span><span class="sxs-lookup"><span data-stu-id="5f12f-567">Role</span></span>

* <span data-ttu-id="5f12f-568">az role assignment create: Problem behoben, das beim Zuweisen einer Rolle zu einem Dienstprinzipal nach Anzeigename einen Fehler vom Typ „HTTP 400“ verursachte</span><span class="sxs-lookup"><span data-stu-id="5f12f-568">az role assignment create: Fix the error that assigning a role to a service principal by display name yields a HTTP 400</span></span>

### <a name="sql"></a><span data-ttu-id="5f12f-569">SQL</span><span class="sxs-lookup"><span data-stu-id="5f12f-569">SQL</span></span>

* <span data-ttu-id="5f12f-570">Cmdlet `az sql mi update` der verwalteten SQL-Instanz mit zwei neuen Parametern aktualisiert: tier und family</span><span class="sxs-lookup"><span data-stu-id="5f12f-570">Update SQL Managed Instance cmdlet `az sql mi update` with two new parameters: tier and family</span></span>

### <a name="storage"></a><span data-ttu-id="5f12f-571">Storage</span><span class="sxs-lookup"><span data-stu-id="5f12f-571">Storage</span></span>

* <span data-ttu-id="5f12f-572">[BREAKING CHANGE] `az storage account create`: Art des Standardspeicherkontos in StorageV2 geändert</span><span class="sxs-lookup"><span data-stu-id="5f12f-572">[BREAKING CHANGE] `az storage account create`: Change default storage account kind to StorageV2</span></span>

## <a name="february-04-2020"></a><span data-ttu-id="5f12f-573">04. Februar 2020</span><span class="sxs-lookup"><span data-stu-id="5f12f-573">February 04, 2020</span></span>

<span data-ttu-id="5f12f-574">Version 2.0.81</span><span class="sxs-lookup"><span data-stu-id="5f12f-574">Version 2.0.81</span></span>

### <a name="acs"></a><span data-ttu-id="5f12f-575">ACS</span><span class="sxs-lookup"><span data-stu-id="5f12f-575">ACS</span></span>

* <span data-ttu-id="5f12f-576">Unterstützung für das Festlegen zugeordneter Ausgangsports und Leerlauftimeouts für Load Balancer Standard hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-576">Add support to set outbound allocated ports and idle timeouts on standard load balancer</span></span>
* <span data-ttu-id="5f12f-577">Aktualisierung auf API-Version 2019-11-01</span><span class="sxs-lookup"><span data-stu-id="5f12f-577">Update to API Version 2019-11-01</span></span>

### <a name="acr"></a><span data-ttu-id="5f12f-578">ACR</span><span class="sxs-lookup"><span data-stu-id="5f12f-578">ACR</span></span>

* <span data-ttu-id="5f12f-579">[BREAKING CHANGE] `az acr delete` löst eine Eingabeaufforderung aus.</span><span class="sxs-lookup"><span data-stu-id="5f12f-579">[BREAKING CHANGE] `az acr delete` will prompt</span></span>
* <span data-ttu-id="5f12f-580">[BREAKING CHANGE] „az acr task delete“ löst eine Eingabeaufforderung aus.</span><span class="sxs-lookup"><span data-stu-id="5f12f-580">[BREAKING CHANGE] 'az acr task delete' will prompt</span></span>
* <span data-ttu-id="5f12f-581">Neue Befehlsgruppe „az acr taskrun show/list/delete“ für die Aufgabenausführungsverwaltung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-581">Add a new command group 'az acr taskrun show/list/delete' for taskrun management</span></span>

### <a name="aks"></a><span data-ttu-id="5f12f-582">AKS</span><span class="sxs-lookup"><span data-stu-id="5f12f-582">AKS</span></span>

* <span data-ttu-id="5f12f-583">Jeder Cluster erhält einen separaten Dienstprinzipal zur Verbesserung der Isolation.</span><span class="sxs-lookup"><span data-stu-id="5f12f-583">Each cluster gets a separate service principal to improve isolation</span></span>

### <a name="appconfig"></a><span data-ttu-id="5f12f-584">AppConfig</span><span class="sxs-lookup"><span data-stu-id="5f12f-584">AppConfig</span></span>

* <span data-ttu-id="5f12f-585">Unterstützung für den Import/Export von KeyVault-Verweisen in/aus AppService</span><span class="sxs-lookup"><span data-stu-id="5f12f-585">Support import/export of keyvault references from/to appservice</span></span>
* <span data-ttu-id="5f12f-586">Unterstützung für den Import/Export aller Bezeichnungen in appconfig und aus appconfig</span><span class="sxs-lookup"><span data-stu-id="5f12f-586">Support import/export of all labels from appconfig to appconfig</span></span>
* <span data-ttu-id="5f12f-587">Überprüfen der Schlüssel- und Featurenamen vor dem Festlegen und Importieren</span><span class="sxs-lookup"><span data-stu-id="5f12f-587">Validate key and feature names before setting and importing</span></span>
* <span data-ttu-id="5f12f-588">Verfügbarmachen der SKU-Änderung für den Konfigurationsspeicher</span><span class="sxs-lookup"><span data-stu-id="5f12f-588">Expose sku modification for configuration store.</span></span>
* <span data-ttu-id="5f12f-589">Befehlsgruppe für die verwaltete Identität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-589">Add command group for managed identity.</span></span>

### <a name="appservice"></a><span data-ttu-id="5f12f-590">AppService</span><span class="sxs-lookup"><span data-stu-id="5f12f-590">AppService</span></span>

* <span data-ttu-id="5f12f-591">Azure Stack: Oberflächenbefehle im Profil „2019-03-01-hybrid“</span><span class="sxs-lookup"><span data-stu-id="5f12f-591">Azure Stack: surface commands under the profile of 2019-03-01-hybrid</span></span>
* <span data-ttu-id="5f12f-592">functionapp: Funktion zum Erstellen von Java-Funktions-Apps in Linux hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-592">functionapp: Add ability to create Java function apps in Linux</span></span>

### <a name="arm"></a><span data-ttu-id="5f12f-593">ARM</span><span class="sxs-lookup"><span data-stu-id="5f12f-593">ARM</span></span>

* <span data-ttu-id="5f12f-594">Behebung von Problem Nr. 10246: `az resource tag` stürzt ab, wenn der übergebene Parameter `--ids` der Ressourcengruppen-ID entspricht.</span><span class="sxs-lookup"><span data-stu-id="5f12f-594">Fix issue #10246: `az resource tag` crashes when the parameter `--ids` passed in is resource group ID</span></span>
* <span data-ttu-id="5f12f-595">Behebung von Problem Nr. 11658: Der Befehl `az group export` unterstützt die Parameter `--query` und `--output` nicht.</span><span class="sxs-lookup"><span data-stu-id="5f12f-595">Fix issue #11658: `az group export` command does not support `--query` and `--output` parameters</span></span>
* <span data-ttu-id="5f12f-596">Behebung von Problem Nr. 10279: Der Exitcode von `az group deployment validate` ist 0, wenn bei der Überprüfung ein Fehler auftritt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-596">Fix issue #10279: The exit code of `az group deployment validate` is 0 when the verification fails</span></span>
* <span data-ttu-id="5f12f-597">Behebung von Problem Nr. 9916: Fehlermeldung des Konflikts zwischen Tag und anderen Filterbedingungen für Befehl `az resource list` verbessert</span><span class="sxs-lookup"><span data-stu-id="5f12f-597">Fix issue #9916: Improve the error message of the conflict between tag and other filter conditions for `az resource list` command</span></span>
* <span data-ttu-id="5f12f-598">Neuer Parameter `--managed-by` hinzugefügt, um das Hinzufügen der Informationen vom Typ „managedBy“ für Befehl `az group create` zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="5f12f-598">Add new parameter `--managed-by` to support adding managedBy information for command `az group create`</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="5f12f-599">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="5f12f-599">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="5f12f-600">Untergruppe `monitor` hinzugefügt, um Log Analytics-Überwachung im Azure Red Hat OpenShift-Cluster zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="5f12f-600">Add `monitor` subgroup to manage Log Analytics monitoring in Azure Red Hat OpensShift cluster</span></span>

### <a name="botservice"></a><span data-ttu-id="5f12f-601">BotService</span><span class="sxs-lookup"><span data-stu-id="5f12f-601">BotService</span></span>

* <span data-ttu-id="5f12f-602">Behebung von Problem Nr. 11697: `az bot create` ist nicht idempotent.</span><span class="sxs-lookup"><span data-stu-id="5f12f-602">Fix issue #11697: `az bot create` is not idempotent</span></span>
* <span data-ttu-id="5f12f-603">Tests zur Namenskorrektur geändert, sodass sie nur im Livemodus ausgeführt werden</span><span class="sxs-lookup"><span data-stu-id="5f12f-603">Change name-correcting tests to run in Live-mode only</span></span>

### <a name="cdn"></a><span data-ttu-id="5f12f-604">CDN</span><span class="sxs-lookup"><span data-stu-id="5f12f-604">CDN</span></span>

* <span data-ttu-id="5f12f-605">Unterstützung für das rulesEngine-Feature hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-605">Add support for rulesEngine feature</span></span>
* <span data-ttu-id="5f12f-606">Neue Befehlsgruppe „cdn endpoint rule“ zum Verwalten von Regeln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-606">Add new commands group 'cdn endpoint rule' to manage rules</span></span>
* <span data-ttu-id="5f12f-607">azure-mgmt-cdn-Version auf 4.0.0 aktualisiert, um API-Version 2019-04-15 zu verwenden</span><span class="sxs-lookup"><span data-stu-id="5f12f-607">Update azure-mgmt-cdn version to 4.0.0 to use api version 2019-04-15</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="5f12f-608">Bereitstellungs-Manager</span><span class="sxs-lookup"><span data-stu-id="5f12f-608">Deployment Manager</span></span>

* <span data-ttu-id="5f12f-609">Auflistungsvorgang für alle Ressourcen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-609">Add list operation for all resources.</span></span>
* <span data-ttu-id="5f12f-610">Schrittressource für neuen Schritttyp optimiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-610">Enhance step resource for new step type.</span></span>
* <span data-ttu-id="5f12f-611">Paket „azure-mgmt-deploymentmanager“ zur Verwendung von Version 0.2.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-611">Update azure-mgmt-deploymentmanager package to use version 0.2.0.</span></span>

### <a name="iot"></a><span data-ttu-id="5f12f-612">IoT</span><span class="sxs-lookup"><span data-stu-id="5f12f-612">IoT</span></span>

* <span data-ttu-id="5f12f-613">Befehle vom Typ „IoT hub Job“ als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="5f12f-613">Deprecate 'IoT hub Job' commands.</span></span>

### <a name="iot-central"></a><span data-ttu-id="5f12f-614">IoT Central</span><span class="sxs-lookup"><span data-stu-id="5f12f-614">IoT Central</span></span>

* <span data-ttu-id="5f12f-615">Unterstützung der App-Erstellung/-Aktualisierung mit neuem SKU-Namen ST0, ST1, ST2</span><span class="sxs-lookup"><span data-stu-id="5f12f-615">Support app creation/update with the new sku name ST0, ST1, ST2.</span></span>

### <a name="key-vault"></a><span data-ttu-id="5f12f-616">Key Vault</span><span class="sxs-lookup"><span data-stu-id="5f12f-616">Key Vault</span></span>

* <span data-ttu-id="5f12f-617">Neuer Befehl `az keyvault key download` zum Herunterladen von Schlüsseln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-617">Add a new command `az keyvault key download` for downloading keys.</span></span>

### <a name="misc"></a><span data-ttu-id="5f12f-618">Sonstiges</span><span class="sxs-lookup"><span data-stu-id="5f12f-618">Misc</span></span>

* <span data-ttu-id="5f12f-619">Behebung Nr. 6371: Unterstützung für die Vervollständigung von Dateinamen und Umgebungsvariablen in Bash</span><span class="sxs-lookup"><span data-stu-id="5f12f-619">Fix #6371: Support filename and environment variable completion in Bash</span></span>

### <a name="network"></a><span data-ttu-id="5f12f-620">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="5f12f-620">Network</span></span>

* <span data-ttu-id="5f12f-621">Behebung Nr. 2092: az network dns record-set add/remove: Warnung hinzugefügt, wenn Datensatzgruppe nicht gefunden wurde.</span><span class="sxs-lookup"><span data-stu-id="5f12f-621">Fix #2092: az network dns record-set add/remove: add warning when record-set is not found.</span></span> <span data-ttu-id="5f12f-622">In Zukunft wird ein zusätzliches Argument unterstützt, um diese automatische Erstellung zu bestätigen.</span><span class="sxs-lookup"><span data-stu-id="5f12f-622">In the future, an extra argument will be supported to confirm this auto creation.</span></span>

### <a name="policy"></a><span data-ttu-id="5f12f-623">Richtlinie</span><span class="sxs-lookup"><span data-stu-id="5f12f-623">Policy</span></span>

* <span data-ttu-id="5f12f-624">Neuer Befehl `az policy metadata` hinzugefügt, um umfangreiche Richtlinienmetadatenressourcen abzurufen</span><span class="sxs-lookup"><span data-stu-id="5f12f-624">Add new command `az policy metadata` to retrieve rich policy metadata resources</span></span>
* <span data-ttu-id="5f12f-625">`az policy remediation create`: Geben Sie mit dem Parameter `--resource-discovery-mode` an, ob die Konformität vor der Wartung neu bewertet werden soll.</span><span class="sxs-lookup"><span data-stu-id="5f12f-625">`az policy remediation create`: Specify whether compliance should be re-evaluated prior to remediation with the `--resource-discovery-mode` parameter</span></span>

### <a name="profile"></a><span data-ttu-id="5f12f-626">Profil</span><span class="sxs-lookup"><span data-stu-id="5f12f-626">Profile</span></span>

* <span data-ttu-id="5f12f-627">`az account get-access-token`: Parameter `--tenant` hinzugefügt, um das Token für den Mandanten direkt abzurufen. Es muss kein Abonnement angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="5f12f-627">`az account get-access-token`: Add `--tenant` parameter to acquire token for the tenant directly, needless to specify a subscription</span></span>

### <a name="rbac"></a><span data-ttu-id="5f12f-628">RBAC</span><span class="sxs-lookup"><span data-stu-id="5f12f-628">RBAC</span></span>

* <span data-ttu-id="5f12f-629">[BREAKING CHANGE] Behebung Nr. 11883: `az role assignment create`: Bei leerem Bereich wird ein Fehler ausgegeben.</span><span class="sxs-lookup"><span data-stu-id="5f12f-629">[BREAKING CHANGE] Fix #11883: `az role assignment create`: empty scope will prompt error</span></span>

### <a name="security"></a><span data-ttu-id="5f12f-630">Sicherheit</span><span class="sxs-lookup"><span data-stu-id="5f12f-630">Security</span></span>

* <span data-ttu-id="5f12f-631">Neue Befehle `az atp show` und `az atp update` hinzugefügt, um erweiterte Einstellungen für den Bedrohungsschutz für Speicherkonten anzuzeigen und zu verwalten</span><span class="sxs-lookup"><span data-stu-id="5f12f-631">Add new commands `az atp show` and `az atp update` to view and manage advanced threat protection settings for storage accounts.</span></span>

### <a name="sql"></a><span data-ttu-id="5f12f-632">SQL</span><span class="sxs-lookup"><span data-stu-id="5f12f-632">SQL</span></span>

* <span data-ttu-id="5f12f-633">`sql dw create`: Parameter `--zone-redundant` und `--read-replica-count` als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="5f12f-633">`sql dw create`: deprecate `--zone-redundant` and `--read-replica-count` parameters.</span></span> <span data-ttu-id="5f12f-634">Diese Parameter gelten nicht für Datawarehouse.</span><span class="sxs-lookup"><span data-stu-id="5f12f-634">These parameters do not apply to DataWarehouse.</span></span>
* <span data-ttu-id="5f12f-635">[BREAKING CHANGE] `az sql db create`: „WideWorldImportersStd“ und „WideWorldImportersFull“ als dokumentierte zulässige Werte für „az sql db create --sample-name“ entfernt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-635">[BREAKING CHANGE] `az sql db create`: Remove "WideWorldImportersStd" and "WideWorldImportersFull" as documented allowed values for "az sql db create --sample-name".</span></span> <span data-ttu-id="5f12f-636">Diese Beispieldatenbanken führen immer zu einem Fehler bei der Erstellung.</span><span class="sxs-lookup"><span data-stu-id="5f12f-636">These sample databases would always cause creation to fail.</span></span>
* <span data-ttu-id="5f12f-637">Neue Befehle `sql db classification show/list/update/delete` und `sql db classification recommendation list/enable/disable` zur Verwaltung von Vertraulichkeitsklassifizierungen für SQL-Datenbanken hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-637">Add New commands `sql db classification show/list/update/delete` and `sql db classification recommendation list/enable/disable` to manage sensitivity classifications for SQL databases.</span></span>
* <span data-ttu-id="5f12f-638">`az sql db audit-policy`: Behebung für leere Überwachungsaktionen und -gruppen</span><span class="sxs-lookup"><span data-stu-id="5f12f-638">`az sql db audit-policy`: Fix for empty audit actions and groups</span></span>

### <a name="storage"></a><span data-ttu-id="5f12f-639">Storage</span><span class="sxs-lookup"><span data-stu-id="5f12f-639">Storage</span></span>

* <span data-ttu-id="5f12f-640">Neue Befehlsgruppe `az storage share-rm` hinzugefügt, um den Ressourcenanbieter „Microsoft.Storage“ für Verwaltungsvorgänge der Azure-Dateifreigabe zu verwenden</span><span class="sxs-lookup"><span data-stu-id="5f12f-640">Add a new command group `az storage share-rm` to use the Microsoft.Storage resource provider for Azure file share management operations.</span></span>
* <span data-ttu-id="5f12f-641">Behebung für Problem Nr. 11415: Berechtigungsfehler für `az storage blob update`</span><span class="sxs-lookup"><span data-stu-id="5f12f-641">Fix issue #11415: permission error for `az storage blob update`</span></span>
* <span data-ttu-id="5f12f-642">Integration von Azcopy 10.3.3 und Unterstützung von Win32</span><span class="sxs-lookup"><span data-stu-id="5f12f-642">Integrate Azcopy 10.3.3 and support Win32.</span></span>
* <span data-ttu-id="5f12f-643">`az storage copy`: Parameter `--include-path`, `--include-pattern`, `--exclude-path` und`--exclude-pattern` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-643">`az storage copy`: Add `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="5f12f-644">`az storage remove`: Parameter `--inlcude` und `--exclude` in Parameter `--include-path`, `--include-pattern`, `--exclude-path` und`--exclude-pattern` geändert</span><span class="sxs-lookup"><span data-stu-id="5f12f-644">`az storage remove`: Change `--inlcude` and `--exclude` parameters to `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="5f12f-645">`az storage sync`: Parameter `--include-pattern`, `--exclude-path` und`--exclude-pattern` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-645">`az storage sync`: Add `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>

### <a name="servicefabric"></a><span data-ttu-id="5f12f-646">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="5f12f-646">ServiceFabric</span></span>

* <span data-ttu-id="5f12f-647">Neue Befehle zum Verwalten von Anwendung und Diensten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-647">Add new commands to manage appliaction and services.</span></span>

## <a name="january-13-2020"></a><span data-ttu-id="5f12f-648">13. Januar 2020</span><span class="sxs-lookup"><span data-stu-id="5f12f-648">January 13, 2020</span></span>

<span data-ttu-id="5f12f-649">Version 2.0.80</span><span class="sxs-lookup"><span data-stu-id="5f12f-649">Version 2.0.80</span></span>

### <a name="compute"></a><span data-ttu-id="5f12f-650">Compute</span><span class="sxs-lookup"><span data-stu-id="5f12f-650">Compute</span></span>

* <span data-ttu-id="5f12f-651">Datenträgeraktualisierung: „--disk-encryption-set“ und „--encryption-type“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-651">disk update: Add --disk-encryption-set and --encryption-type</span></span>
* <span data-ttu-id="5f12f-652">Momentaufnahmeerstellung/-aktualisierung: „--disk-encryption-set“ und „--encryption-type“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-652">snapshot create/update: Add --disk-encryption-set and --encryption-type</span></span>

### <a name="storage"></a><span data-ttu-id="5f12f-653">Storage</span><span class="sxs-lookup"><span data-stu-id="5f12f-653">Storage</span></span>

* <span data-ttu-id="5f12f-654">„azure-mgmt-storage“ auf Version 7.1.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-654">Upgrade azure-mgmt-storage version to 7.1.0</span></span>
* <span data-ttu-id="5f12f-655">`az storage account create`: `--encryption-key-type-for-table` und `--encryption-key-type-for-queue` zur Unterstützung des Tabellen- und Warteschlangenverschlüsselungsdiensts hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-655">`az storage account create`: Add `--encryption-key-type-for-table` and `--encryption-key-type-for-queue` to support Table and Queue Encryption Service</span></span>

## <a name="january-07-2020"></a><span data-ttu-id="5f12f-656">7\. Januar 2020</span><span class="sxs-lookup"><span data-stu-id="5f12f-656">January 07, 2020</span></span>

<span data-ttu-id="5f12f-657">Version 2.0.79</span><span class="sxs-lookup"><span data-stu-id="5f12f-657">Version 2.0.79</span></span>

### <a name="acr"></a><span data-ttu-id="5f12f-658">ACR</span><span class="sxs-lookup"><span data-stu-id="5f12f-658">ACR</span></span>

* <span data-ttu-id="5f12f-659">[BREAKING CHANGE] Parameter „--os“ für „acr build“, „acr task create/update“, „acr run“ und „acr pack“ wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-659">[BREAKING CHANGE] Remove '--os' parameter for 'acr build', 'acr task create/update', 'acr run', and 'acr pack'.</span></span> <span data-ttu-id="5f12f-660">Verwenden Sie stattdessen „--platform“.</span><span class="sxs-lookup"><span data-stu-id="5f12f-660">Use '--platform' instead.</span></span>

### <a name="appconfig"></a><span data-ttu-id="5f12f-661">AppConfig</span><span class="sxs-lookup"><span data-stu-id="5f12f-661">AppConfig</span></span>

* <span data-ttu-id="5f12f-662">Unterstützung für das Importieren/Exportieren von Featureflags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-662">Add support for importing/exporting feature flags</span></span>
* <span data-ttu-id="5f12f-663">Neuer Befehl „az appconfig kv set-keyvault“ für das Erstellen einer KeyVault-Referenz hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-663">Add new command 'az appconfig kv set-keyvault' for creating keyvault reference</span></span>
* <span data-ttu-id="5f12f-664">Unterstützung verschiedener Benennungskonventionen beim Exportieren von Featureflags in eine Datei</span><span class="sxs-lookup"><span data-stu-id="5f12f-664">Support various naming conventions when exporting feature flags to file</span></span>

### <a name="appservice"></a><span data-ttu-id="5f12f-665">AppService</span><span class="sxs-lookup"><span data-stu-id="5f12f-665">AppService</span></span>

* <span data-ttu-id="5f12f-666">Behebung von Problem Nr. 7154: Aktualisierung der Dokumentation für Befehl „<>“, sodass Backticks anstelle von einfachen Anführungszeichen verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="5f12f-666">Fix issue #7154: Updating documentation for command <> to use back ticks instead of single quotes</span></span>
* <span data-ttu-id="5f12f-667">Behebung von Problem Nr. 11287: „webapp up“: Für die mit „up“ erstellte App muss standardmäßig SSL aktiviert sein.</span><span class="sxs-lookup"><span data-stu-id="5f12f-667">Fix issue #11287: webapp up: By default make the app created using up 'should be 'SSL enabled'</span></span>
* <span data-ttu-id="5f12f-668">Behebung von Problem Nr. 11592: Flag „az webapp up“ für statische HTML-Websites hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-668">Fix issue #11592: Add az webapp up flag for html static sites</span></span>

### <a name="arm"></a><span data-ttu-id="5f12f-669">ARM</span><span class="sxs-lookup"><span data-stu-id="5f12f-669">ARM</span></span>

* <span data-ttu-id="5f12f-670">Behebung `az resource tag`: Recovery Services-Tresor-Tags können nicht aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="5f12f-670">Fix `az resource tag`: Recovery Services Vault tags cannot be updated</span></span>

### <a name="backup"></a><span data-ttu-id="5f12f-671">Backup</span><span class="sxs-lookup"><span data-stu-id="5f12f-671">Backup</span></span>

* <span data-ttu-id="5f12f-672">Neuer Befehl „backup protection undelete“ hinzugefügt, um die Funktion zum vorläufigen Löschen für IaasVM-Workloads zu aktivieren</span><span class="sxs-lookup"><span data-stu-id="5f12f-672">Added new command 'backup protection undelete' to enable soft-delete feature for IaasVM workload</span></span>
* <span data-ttu-id="5f12f-673">Neuer Parameter „--soft-delete-feature-state“ hinzugefügt, um den Befehl „backup-properties“ festzulegen</span><span class="sxs-lookup"><span data-stu-id="5f12f-673">Added new parameter '--soft-delete-feature-state' to set backup-properties command</span></span>
* <span data-ttu-id="5f12f-674">Unterstützung für den Ausschluss von Datenträgern für IaasVM-Workload hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-674">Added disk exclusion support for IaasVM workload</span></span>

### <a name="compute"></a><span data-ttu-id="5f12f-675">Compute</span><span class="sxs-lookup"><span data-stu-id="5f12f-675">Compute</span></span>

* <span data-ttu-id="5f12f-676">Fehler `vm create` in Azure Stack-Profil behoben.</span><span class="sxs-lookup"><span data-stu-id="5f12f-676">Fix `vm create` failure in Azure Stack profile.</span></span>
* <span data-ttu-id="5f12f-677">vm monitor metrics tail/list-definitions: Unterstützung einer Abfragemetrik und von Listendefinitionen für eine VM.</span><span class="sxs-lookup"><span data-stu-id="5f12f-677">vm monitor metrics tail/list-definitions: support query metric and list definitions for a vm.</span></span>
* <span data-ttu-id="5f12f-678">Neue Aktion des Befehls zum erneuten Anwenden für „az vm“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-678">Add new reapply command action for az vm</span></span>

### <a name="hdinsight"></a><span data-ttu-id="5f12f-679">HDInsight</span><span class="sxs-lookup"><span data-stu-id="5f12f-679">HDInsight</span></span>

* <span data-ttu-id="5f12f-680">Unterstützung für das Erstellen eines Kafka-Clusters mit Kafka-REST-Proxy</span><span class="sxs-lookup"><span data-stu-id="5f12f-680">Support for creating a Kafka cluster with Kafka Rest Proxy</span></span>
* <span data-ttu-id="5f12f-681">„azure-mgmt-hdinsight“ auf 1.3.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-681">Upgrade azure-mgmt-hdinsight to 1.3.0</span></span>

### <a name="misc"></a><span data-ttu-id="5f12f-682">Verschiedenes:</span><span class="sxs-lookup"><span data-stu-id="5f12f-682">Misc.</span></span>

* <span data-ttu-id="5f12f-683">Vorschaubefehl `az version show` hinzugefügt, um die Versionen der Azure CLI-Module und Erweiterungen standardmäßig im JSON-Format oder im mit „--output“ konfigurierten Format anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="5f12f-683">Add preview command `az version show` to show the versions of Azure CLI modules and extensions in JSON format by default or format configured by --output</span></span>

### <a name="event-hubs"></a><span data-ttu-id="5f12f-684">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="5f12f-684">Event Hubs</span></span>

* <span data-ttu-id="5f12f-685">[BREAKING CHANGE] Statusoption „ReceiveDisabled“ aus „az eventhubs eventhub update“ und „az eventhubs eventhub create“ entfernt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-685">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az eventhubs eventhub update' and 'az eventhubs eventhub create'.</span></span> <span data-ttu-id="5f12f-686">Diese Option ist für Event Hub-Entitäten nicht gültig.</span><span class="sxs-lookup"><span data-stu-id="5f12f-686">This option is not valid for Event Hub entities.</span></span>

### <a name="service-bus"></a><span data-ttu-id="5f12f-687">Service Bus</span><span class="sxs-lookup"><span data-stu-id="5f12f-687">Service Bus</span></span>

* <span data-ttu-id="5f12f-688">[BREAKING CHANGE] Statusoption „ReceiveDisabled“ aus Befehlen „az servicebus topic create“, „az servicebus topic update“, „az servicebus queue create“ und „az servicebus queue update“ entfernt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-688">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az servicebus topic create', 'az servicebus topic update', 'az servicebus queue create', and 'az servicebus queue update'.</span></span> <span data-ttu-id="5f12f-689">Diese Option ist für Service Bus-Themen und -Warteschlangen nicht gültig.</span><span class="sxs-lookup"><span data-stu-id="5f12f-689">This option is not valid for Service Bus topics and queues.</span></span>

### <a name="rbac"></a><span data-ttu-id="5f12f-690">RBAC</span><span class="sxs-lookup"><span data-stu-id="5f12f-690">RBAC</span></span>

* <span data-ttu-id="5f12f-691">Behebung Nr. 11712: `az ad app/sp show` gibt nicht den Exitcode 3 zurück, wenn die Anwendung oder der Dienstprinzipal nicht vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="5f12f-691">Fix #11712: `az ad app/sp show` does not return exit code 3 when the application or service principal does not exist</span></span>

### <a name="storage"></a><span data-ttu-id="5f12f-692">Storage</span><span class="sxs-lookup"><span data-stu-id="5f12f-692">Storage</span></span>

* <span data-ttu-id="5f12f-693">`az storage account create`: Vorschaukennzeichnung für Parameter „--enable-hierarchical-namespace“ entfernt</span><span class="sxs-lookup"><span data-stu-id="5f12f-693">`az storage account create`: Remove preview flag for --enable-hierarchical-namespace parameter</span></span>
* <span data-ttu-id="5f12f-694">azure-mgmt-storage-Version auf 7.0.0 aktualisiert, um API-Version 2019-06-01 zu verwenden</span><span class="sxs-lookup"><span data-stu-id="5f12f-694">Update azure-mgmt-storage version to 7.0.0 to use api version 2019-06-01</span></span>
* <span data-ttu-id="5f12f-695">Neue Parameter `--enable-delete-retention` und `--delete-retention-days` hinzugefügt, um die Verwaltung der Aufbewahrungsrichtlinie für Löschen für „blob-service-properties“ von Speicherkonten zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="5f12f-695">Add new parameters `--enable-delete-retention` and `--delete-retention-days` to support managing delete retention policy for storage account blob-service-properties.</span></span>

## <a name="december-17-2019"></a><span data-ttu-id="5f12f-696">17. Dezember 2019</span><span class="sxs-lookup"><span data-stu-id="5f12f-696">December 17, 2019</span></span>

<span data-ttu-id="5f12f-697">2.0.78</span><span class="sxs-lookup"><span data-stu-id="5f12f-697">2.0.78</span></span>

### <a name="acr"></a><span data-ttu-id="5f12f-698">ACR</span><span class="sxs-lookup"><span data-stu-id="5f12f-698">ACR</span></span>

* <span data-ttu-id="5f12f-699">Unterstützung für lokalen Kontext in „acr task run“</span><span class="sxs-lookup"><span data-stu-id="5f12f-699">Added support Local context in acr task run</span></span>

### <a name="acs"></a><span data-ttu-id="5f12f-700">ACS</span><span class="sxs-lookup"><span data-stu-id="5f12f-700">ACS</span></span>

* <span data-ttu-id="5f12f-701">[BREAKING CHANGE] az openshift create: `--workspace-resource-id` in `--workspace-id` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-701">[BREAKING CHANGE]az openshift create: rename `--workspace-resource-id` to `--workspace-id`.</span></span>

### <a name="ams"></a><span data-ttu-id="5f12f-702">AMS</span><span class="sxs-lookup"><span data-stu-id="5f12f-702">AMS</span></span>

* <span data-ttu-id="5f12f-703">Befehle zum Anzeigen aktualisiert, sodass 3 zurückgegeben wird, wenn die Ressource nicht gefunden wurde</span><span class="sxs-lookup"><span data-stu-id="5f12f-703">Updated show commands to return 3 when resource not found</span></span>

### <a name="appconfig"></a><span data-ttu-id="5f12f-704">AppConfig</span><span class="sxs-lookup"><span data-stu-id="5f12f-704">AppConfig</span></span>

* <span data-ttu-id="5f12f-705">Fehler beim Anhängen der API-Version an die Anforderungs-URL korrigiert.</span><span class="sxs-lookup"><span data-stu-id="5f12f-705">Fixed bug when appending api-version to request url.</span></span> <span data-ttu-id="5f12f-706">Die vorhandene Lösung funktioniert nicht mit Paginierung.</span><span class="sxs-lookup"><span data-stu-id="5f12f-706">The existing solution doesn't work with pagination.</span></span>
* <span data-ttu-id="5f12f-707">Unterstützung für die Anzeige von weiteren Sprachen neben Englisch hinzugefügt, da der Back-End-Dienst Unicode für die Globalisierung unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-707">Added support for showing languages besides English as our backend service support unicode for globalization.</span></span>

### <a name="appservice"></a><span data-ttu-id="5f12f-708">AppService</span><span class="sxs-lookup"><span data-stu-id="5f12f-708">AppService</span></span>

* <span data-ttu-id="5f12f-709">Problem Nr. 11217 behoben: Web-App: „az webapp config ssl upload“ muss Slot-Parameter unterstützen.</span><span class="sxs-lookup"><span data-stu-id="5f12f-709">Fixed issue #11217: webapp: az webapp config ssl upload should support slot parameter</span></span>
* <span data-ttu-id="5f12f-710">Problem Nr. 10965 behoben: Error: Der Name darf nicht leer sein.</span><span class="sxs-lookup"><span data-stu-id="5f12f-710">Fixed issue #10965: Error: Name cannot be empty.</span></span> <span data-ttu-id="5f12f-711">Entfernen anhand von „ip_address“ und „subnet“ zulassen</span><span class="sxs-lookup"><span data-stu-id="5f12f-711">Allow remove by ip_address and subnet</span></span>
* <span data-ttu-id="5f12f-712">Unterstützung des Imports von Zertifikaten aus Key Vault hinzugefügt `az webapp config ssl import`</span><span class="sxs-lookup"><span data-stu-id="5f12f-712">Added support for importing certificates from Key Vault `az webapp config ssl import`</span></span>

### <a name="arm"></a><span data-ttu-id="5f12f-713">ARM</span><span class="sxs-lookup"><span data-stu-id="5f12f-713">ARM</span></span>

* <span data-ttu-id="5f12f-714">Paket „azure-mgmt-resource“ auf die Verwendung von 6.0.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-714">Updated azure-mgmt-resource package to use 6.0.0</span></span>
* <span data-ttu-id="5f12f-715">Mandantenübergreifende Unterstützung für Befehl `az group deployment create` durch Hinzufügen des neuen Parameters `--aux-subs`</span><span class="sxs-lookup"><span data-stu-id="5f12f-715">Cross Tenant Support for `az group deployment create` command by adding new parameter `--aux-subs`</span></span>
* <span data-ttu-id="5f12f-716">Neuer Parameter `--metadata` hinzugefügt, um das Hinzufügen von Metadateninformationen für Richtliniensatzdefinitionen zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="5f12f-716">Added new parameter `--metadata` to support adding metadata information for policy set definitions.</span></span>

### <a name="backup"></a><span data-ttu-id="5f12f-717">Backup</span><span class="sxs-lookup"><span data-stu-id="5f12f-717">Backup</span></span>

* <span data-ttu-id="5f12f-718">Unterstützung der Sicherung für SQL- und SAP Hana-Workloads hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-718">Added Backup support for SQL and SAP Hana workload.</span></span>

### <a name="botservice"></a><span data-ttu-id="5f12f-719">BotService</span><span class="sxs-lookup"><span data-stu-id="5f12f-719">BotService</span></span>

* <span data-ttu-id="5f12f-720">[Breaking Change] Flag „--version“ aus Vorschaubefehl „az bot create“ entfernt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-720">[Breaking change] Remove '--version' flag from preview command 'az bot create'.</span></span> <span data-ttu-id="5f12f-721">Nur v4-SDK-Bots werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-721">Only v4 SDK bots are supported.</span></span>
* <span data-ttu-id="5f12f-722">Überprüfung der Namensverfügbarkeit für „az bot create“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-722">Added name availability check for 'az bot create'.</span></span>
* <span data-ttu-id="5f12f-723">Unterstützung für das Aktualisieren der Symbol-URL für einen Bot über „az bot update“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-723">Added support for updating the icon URL for a bot via 'az bot update'.</span></span>
* <span data-ttu-id="5f12f-724">Unterstützung für das Aktualisieren eines Direct Line-Kanals über „az bot directline update“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-724">Added support for updating a Direct Line channel via 'az bot directline update'.</span></span>
* <span data-ttu-id="5f12f-725">Unterstützung für Flag „--enable-enhanced-auth“ zu „az bot directline create“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-725">Added '--enable-enhanced-auth' flag support to 'az bot directline create'.</span></span>
* <span data-ttu-id="5f12f-726">Die folgenden Befehlsgruppen sind allgemein verfügbar und befinden sich nicht in der Vorschau: „az bot authsetting“.</span><span class="sxs-lookup"><span data-stu-id="5f12f-726">The following command groups are GA and not in preview: 'az bot authsetting'.</span></span>
* <span data-ttu-id="5f12f-727">Die folgenden Befehle in „az bot“ sind allgemein verfügbar und befinden sich nicht in der Vorschau: „create“, „prepare-deploy“, „show“, „delete“, „update“.</span><span class="sxs-lookup"><span data-stu-id="5f12f-727">The following commands in 'az bot' are GA and not in preview: 'create', 'prepare-deploy', 'show', 'delete', 'update'.</span></span>
* <span data-ttu-id="5f12f-728">„az bot prepare-deploy“ korrigiert, indem der Wert voon „--proj-file-path“ in Kleinschreibung geändert wurde (z. B. „Test.csproj“ in „test.csproj“).</span><span class="sxs-lookup"><span data-stu-id="5f12f-728">Fixed 'az bot prepare-deploy' changing '--proj-file-path' value to lower case (e.g. "Test.csproj" to "test.csproj").</span></span>

### <a name="compute"></a><span data-ttu-id="5f12f-729">Compute</span><span class="sxs-lookup"><span data-stu-id="5f12f-729">Compute</span></span>

* <span data-ttu-id="5f12f-730">vmss create/update: „--scale-in-policy“ hinzugefügt, womit entschieden wird, welche virtuellen Computer beim horizontalen Herunterskalieren einer VM-Skalierungsgruppe zum Entfernen ausgewählt werden.</span><span class="sxs-lookup"><span data-stu-id="5f12f-730">vmss create/update: Added --scale-in-policy, which decides which virtual machines are chosen for removal when a VMSS is scaled-in.</span></span>
* <span data-ttu-id="5f12f-731">vm/vmss update: „--priority“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-731">vm/vmss update: Added --priority.</span></span>
* <span data-ttu-id="5f12f-732">vm/vmss update: „--max-price“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-732">vm/vmss update: Added --max-price.</span></span>
* <span data-ttu-id="5f12f-733">Befehlsgruppe „disk-encryption-set“ hinzugefügt (create, show, update, delete, list).</span><span class="sxs-lookup"><span data-stu-id="5f12f-733">Added disk-encryption-set command group (create, show, update, delete, list).</span></span>
* <span data-ttu-id="5f12f-734">disk create: „--encryption-type“ und „--disk-encryption-set“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-734">disk create: Added --encryption-type and --disk-encryption-set.</span></span>
* <span data-ttu-id="5f12f-735">vm/vmss create: „--os-disk-encryption-set“ und „--data-disk-encryption-sets“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-735">vm/vmss create: Added --os-disk-encryption-set and --data-disk-encryption-sets.</span></span>

### <a name="core"></a><span data-ttu-id="5f12f-736">Core</span><span class="sxs-lookup"><span data-stu-id="5f12f-736">Core</span></span>

* <span data-ttu-id="5f12f-737">Unterstützung für Python 3.4 entfernt</span><span class="sxs-lookup"><span data-stu-id="5f12f-737">Removed support for Python 3.4</span></span>
* <span data-ttu-id="5f12f-738">Plug-In für HaTS-Umfrage in mehreren Befehlen</span><span class="sxs-lookup"><span data-stu-id="5f12f-738">Plug in HaTS survey in multiple commands</span></span>

### <a name="dls"></a><span data-ttu-id="5f12f-739">DLS</span><span class="sxs-lookup"><span data-stu-id="5f12f-739">DLS</span></span>

* <span data-ttu-id="5f12f-740">ADLS-SDK-Version aktualisiert (0.0.48).</span><span class="sxs-lookup"><span data-stu-id="5f12f-740">Updated ADLS sdk version (0.0.48).</span></span>

### <a name="install"></a><span data-ttu-id="5f12f-741">Installieren</span><span class="sxs-lookup"><span data-stu-id="5f12f-741">Install</span></span>

* <span data-ttu-id="5f12f-742">Installationsskript unterstützt Python 3.8</span><span class="sxs-lookup"><span data-stu-id="5f12f-742">Install script support python 3.8</span></span>

### <a name="iot"></a><span data-ttu-id="5f12f-743">IoT</span><span class="sxs-lookup"><span data-stu-id="5f12f-743">IOT</span></span>

* <span data-ttu-id="5f12f-744">[BREAKING CHANGE] Parameter „--failover-region“ aus „manual-failover“ entfernt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-744">[BREAKING CHANGE] Removed --failover-region parameter from manual-failover.</span></span> <span data-ttu-id="5f12f-745">Das Failover erfolgt jetzt in eine zugewiesene, geografisch gekoppelte sekundäre Region.</span><span class="sxs-lookup"><span data-stu-id="5f12f-745">Now it will failover to assigned geo-paired secondary region.</span></span>

### <a name="key-vault"></a><span data-ttu-id="5f12f-746">Key Vault</span><span class="sxs-lookup"><span data-stu-id="5f12f-746">Key Vault</span></span>

* <span data-ttu-id="5f12f-747">Nr. 8095 behoben: `az keyvault storage remove`: Hilfemeldung verbessert</span><span class="sxs-lookup"><span data-stu-id="5f12f-747">Fixed #8095: `az keyvault storage remove`: improve the help message</span></span>
* <span data-ttu-id="5f12f-748">Nr. 8921 behoben: `az keyvault key/secret/certificate list/list-deleted/list-versions`: Validierungsfehler in Parameter `--maxresults` behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-748">Fixed #8921: `az keyvault key/secret/certificate list/list-deleted/list-versions`: fix the validation bug on parameter `--maxresults`</span></span>
* <span data-ttu-id="5f12f-749">Nr. 10512 behoben: `az keyvault set-policy`: Fehlermeldung verbessert, wenn weder `--object-id`, `--spn` noch `--upn` angegeben ist</span><span class="sxs-lookup"><span data-stu-id="5f12f-749">Fixed #10512: `az keyvault set-policy`: improve the error message when none of `--object-id`, `--spn` or `--upn` is specified</span></span>
* <span data-ttu-id="5f12f-750">Nr. 10846 behoben: `az keyvault secret show-deleted`: Wenn `--id` angegeben ist, ist `--name/-n` nicht erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5f12f-750">Fixed #10846: `az keyvault secret show-deleted`: when `--id` is specified, `--name/-n` is not required</span></span>
* <span data-ttu-id="5f12f-751">Nr. 11084 behoben: `az keyvault secret download`: Hilfemeldung von Parameter `--encoding` verbessert</span><span class="sxs-lookup"><span data-stu-id="5f12f-751">Fixed #11084: `az keyvault secret download`: improve the help message of parameter `--encoding`</span></span>

### <a name="network"></a><span data-ttu-id="5f12f-752">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="5f12f-752">Network</span></span>

* <span data-ttu-id="5f12f-753">az network application-gateway probe: Unterstützung für Option „--port“ hinzugefügt, um einen Port zum Prüfen von Back-End-Servern beim Erstellen und Aktualisieren anzugeben</span><span class="sxs-lookup"><span data-stu-id="5f12f-753">az network application-gateway probe: Added support --port option to specify a port for probing backend servers when create and update</span></span>
* <span data-ttu-id="5f12f-754">az network application-gateway url-path-map create/update: Fehlerbehebung für `--waf-policy`</span><span class="sxs-lookup"><span data-stu-id="5f12f-754">az network application-gateway url-path-map create/update: bug fix for `--waf-policy`</span></span>
* <span data-ttu-id="5f12f-755">az network application-gateway: Unterstützung für `--rewrite-rule-set` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-755">az network application-gateway: Added support `--rewrite-rule-set`</span></span>
* <span data-ttu-id="5f12f-756">az network list-service-aliases: Unterstützung für Listendienstaliase hinzugefügt, die für Dienstendpunktrichtlinien verwendet werden können</span><span class="sxs-lookup"><span data-stu-id="5f12f-756">az network list-service-aliases: Added support list service aliases which can be used for Service Endpoint Policies</span></span>
* <span data-ttu-id="5f12f-757">az network dns zone import: Unterstützung für „.@“ in Datensatzname hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-757">az network dns zone import: Added support .@ in record name</span></span>

### <a name="packaging"></a><span data-ttu-id="5f12f-758">Verpackung</span><span class="sxs-lookup"><span data-stu-id="5f12f-758">Packaging</span></span>

* <span data-ttu-id="5f12f-759">Back-Edge-Builds für PIP-Installation hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-759">Added back edge builds for pip install</span></span>
* <span data-ttu-id="5f12f-760">Ubuntu-Eoan-Paket hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-760">Added Ubuntu eoan package</span></span>

### <a name="policy"></a><span data-ttu-id="5f12f-761">Richtlinie</span><span class="sxs-lookup"><span data-stu-id="5f12f-761">Policy</span></span>

* <span data-ttu-id="5f12f-762">Unterstützung für Version 2019-09-01 der Richtlinien-API hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-762">Added support for Policy API version 2019-09-01.</span></span>
* <span data-ttu-id="5f12f-763">az policy set-definition: Unterstützung der Gruppierung innerhalb von Richtliniensatzdefinitionen mit `--definition-groups`-Parameter hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-763">az policy set-definition: Added support grouping within policy set definitions with `--definition-groups` parameter</span></span>

### <a name="redis"></a><span data-ttu-id="5f12f-764">Redis</span><span class="sxs-lookup"><span data-stu-id="5f12f-764">Redis</span></span>

* <span data-ttu-id="5f12f-765">Vorschauparameter `--replicas-per-master` zu Befehl `az redis create`hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-765">Added preview param `--replicas-per-master` to `az redis create` command</span></span>
* <span data-ttu-id="5f12f-766">„azure-mgmt-redis“ von 6.0.0 auf 7.0.0rc1 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-766">Updated azure-mgmt-redis from 6.0.0 to 7.0.0rc1</span></span>

### <a name="servicefabric"></a><span data-ttu-id="5f12f-767">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="5f12f-767">ServiceFabric</span></span>

* <span data-ttu-id="5f12f-768">Hinzufügen von Logik in Knotentyp korrigiert, einschließlich Nr. 10963: Beim Hinzufügen eines neuen Knotentyps mit Dauerhaftigkeitsstufe „Gold“ wird immer ein CLI-Fehler ausgegeben.</span><span class="sxs-lookup"><span data-stu-id="5f12f-768">Fixed in node-type add logic including #10963: Adding new node type with durability level Gold will always throw CLI error</span></span>
* <span data-ttu-id="5f12f-769">ServiceFabricNodeVmExt-Version in Erstellungsvorlage auf 1.1 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-769">Updated ServiceFabricNodeVmExt version to 1.1 in creation template</span></span>

### <a name="sql"></a><span data-ttu-id="5f12f-770">SQL</span><span class="sxs-lookup"><span data-stu-id="5f12f-770">SQL</span></span>

* <span data-ttu-id="5f12f-771">Parameter „--read-scale“ und „--read-replicas“ zu Befehlen „sql db create“ und „sql db update“ hinzugefügt, um Leseskalierungsverwaltung zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="5f12f-771">Added "--read-scale" and "--read-replicas" parameters to sql db create and update commands, to support read scale management.</span></span>

### <a name="storage"></a><span data-ttu-id="5f12f-772">Storage</span><span class="sxs-lookup"><span data-stu-id="5f12f-772">Storage</span></span>

* <span data-ttu-id="5f12f-773">Allgemein verfügbares Release – Eigenschaft „Large File Shares“ für Befehle „storage account create“ und „storage account update“</span><span class="sxs-lookup"><span data-stu-id="5f12f-773">GA Release Large File Shares property for storage account create and update command</span></span>
* <span data-ttu-id="5f12f-774">Allgemein verfügbares Release – Unterstützung von SAS-Token für die Benutzerdelegierung</span><span class="sxs-lookup"><span data-stu-id="5f12f-774">GA Release User Delegation SAS token Support</span></span>
* <span data-ttu-id="5f12f-775">Neue Befehle `az storage account blob-service-properties show` und `az storage account blob-service-properties update --enable-change-feed` hinzugefügt, um Blob-Diensteigenschaften für das Speicherkonto zu verwalten.</span><span class="sxs-lookup"><span data-stu-id="5f12f-775">Added new commands `az storage account blob-service-properties show` and `az storage account blob-service-properties update --enable-change-feed` to manage blob service properties for storage account.</span></span>
* <span data-ttu-id="5f12f-776">[BEVORSTEHENDER BREAKING CHANGE] `az storage copy`: Das Zeichen `*` wird nicht mehr als Platzhalter in der URL, es werden jedoch die neuen Parameter „--include-pattern“ und „--exclude-pattern“ mit Unterstützung des Platzhalters `*` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-776">[COMING BREAKING CHANGE] `az storage copy`: `*` character is no longer supported as a wildcard in URL, but new parameters --include-pattern and --exclude-pattern will be added with `*` wildcard support.</span></span>
* <span data-ttu-id="5f12f-777">Problem Nr. 11043 behoben: Unterstützung für das Entfernen des gesamten Containers/der gesamten Freigabe in `az storage remove` Befehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-777">Fixed issue #11043: Added support to remove whole container/share in `az storage remove` command</span></span>

## <a name="november-26-2019"></a><span data-ttu-id="5f12f-778">26. November 2019</span><span class="sxs-lookup"><span data-stu-id="5f12f-778">November 26, 2019</span></span>

<span data-ttu-id="5f12f-779">Version 2.0.77</span><span class="sxs-lookup"><span data-stu-id="5f12f-779">Version 2.0.77</span></span>

### <a name="acr"></a><span data-ttu-id="5f12f-780">ACR</span><span class="sxs-lookup"><span data-stu-id="5f12f-780">ACR</span></span>

* <span data-ttu-id="5f12f-781">Parameter `--branch` in „acr task create/update“ als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-781">Deprecated parameter `--branch` from acr task create/update</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="5f12f-782">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="5f12f-782">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="5f12f-783">`--workspace-resource-id`-Flag hinzugefügt, um die Erstellung eines Azure Red Hat OpenShift-Clusters mit Überwachung zuzulassen</span><span class="sxs-lookup"><span data-stu-id="5f12f-783">Added `--workspace-resource-id` flag to allow creation of Azure Red Hat Openshift cluster with monitoring</span></span>
* <span data-ttu-id="5f12f-784">`monitor_profile`-Flag hinzugefügt, um einen Azure Red Hat OpenShift-Clusters mit Überwachung zu erstellen</span><span class="sxs-lookup"><span data-stu-id="5f12f-784">Added `monitor_profile` to create Azure Red Hat OpenShift cluster with monitoring</span></span>

### <a name="aks"></a><span data-ttu-id="5f12f-785">AKS</span><span class="sxs-lookup"><span data-stu-id="5f12f-785">AKS</span></span>

* <span data-ttu-id="5f12f-786">Unterstützung des Rotationsvorgangs für Clusterzertifikate mithilfe von für Cluster Zertifikat Rotation mit „az aks rotate-certs“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-786">Added support cluster certificate rotation operation using "az aks rotate-certs".</span></span>

### <a name="appconfig"></a><span data-ttu-id="5f12f-787">AppConfig</span><span class="sxs-lookup"><span data-stu-id="5f12f-787">AppConfig</span></span>

* <span data-ttu-id="5f12f-788">Unterstützung für die Verwendung von „:“ für `as az appconfig kv import`-Trennzeichen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-788">Added support for using ":" for `as az appconfig kv import` separator</span></span>
* <span data-ttu-id="5f12f-789">Problem beim Auflisten von Schlüsselwerten mit mehreren Bezeichnungen, einschließlich NULL-Bezeichnung, behoben.</span><span class="sxs-lookup"><span data-stu-id="5f12f-789">Fixed issue for listing key values with multiple labels including null label.</span></span> 
* <span data-ttu-id="5f12f-790">Verwaltungsebenen-SDK, „azure-mgmt-appconfiguration“, auf Version 0.3.0 aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="5f12f-790">Updated management plane sdk, azure-mgmt-appconfiguration, to version 0.3.0.</span></span> 

### <a name="appservice"></a><span data-ttu-id="5f12f-791">AppService</span><span class="sxs-lookup"><span data-stu-id="5f12f-791">AppService</span></span>

* <span data-ttu-id="5f12f-792">Problem Nr. 11100 behoben AttributeError für „az webapp up“ beim Erstellen eines Dienstplans</span><span class="sxs-lookup"><span data-stu-id="5f12f-792">Fixed issue #11100: AttributeError for az webapp up when create service plan</span></span>
* <span data-ttu-id="5f12f-793">az webapp up: Erzwingen der Erstellung oder Bereitstellung auf einer Website für unterstützte Sprachen, es werden keine Standardeinstellungen verwendet.</span><span class="sxs-lookup"><span data-stu-id="5f12f-793">az webapp up: Forcing the creation or deployment to a site for supported languages, no defaults used.</span></span>
* <span data-ttu-id="5f12f-794">Unterstützung für App Service-Umgebung hinzugefügt: az appservice ase show | list | list-addresses | list-plans | create | update | delete</span><span class="sxs-lookup"><span data-stu-id="5f12f-794">Added support for App Service Environment: az appservice ase show | list | list-addresses | list-plans | create | update | delete</span></span>

### <a name="backup"></a><span data-ttu-id="5f12f-795">Backup</span><span class="sxs-lookup"><span data-stu-id="5f12f-795">Backup</span></span>

* <span data-ttu-id="5f12f-796">Problem in Az-Sicherungsrichtlinie „list-associated-items“ behoben.</span><span class="sxs-lookup"><span data-stu-id="5f12f-796">Fixed issue in az backup policy list-associated-items.</span></span> <span data-ttu-id="5f12f-797">Optionaler Parameter „BackupManagementType“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-797">Added optional BackupManagementType parameter.</span></span>

### <a name="compute"></a><span data-ttu-id="5f12f-798">Compute</span><span class="sxs-lookup"><span data-stu-id="5f12f-798">Compute</span></span>

* <span data-ttu-id="5f12f-799">API-Version von Compute, Datenträger, Momentaufnahmen auf 2019-07-01 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-799">Upgraded API version of compute, disks, snapshots to 2019-07-01</span></span>
* <span data-ttu-id="5f12f-800">vmss create: Verbesserung für – Orchestrierungsmodus</span><span class="sxs-lookup"><span data-stu-id="5f12f-800">vmss create: Improvement for --orchestration-mode</span></span>
* <span data-ttu-id="5f12f-801">sig image-definition create: „--os-state“ hinzugefügt, um die Angabe zu ermöglichen, ob die unter diesem Image erstellten virtuellen Computer „generalisiert“ oder „spezialisiert“ sind</span><span class="sxs-lookup"><span data-stu-id="5f12f-801">sig image-definition create: Added --os-state to allow specifying whether the virtual machines created under this image are 'Generalized' or 'Specialized'</span></span>
* <span data-ttu-id="5f12f-802">sig image-definition create: „--hyper-v-generation“ hinzugefügt, um die Angabe der Hypervisorgeneration zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="5f12f-802">sig image-definition create: Added --hyper-v-generation to allow specifying the hypervisor generation</span></span>
* <span data-ttu-id="5f12f-803">sig image-version create: Unterstützung für „--os-snapshot“ und „--data-snapshots“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-803">sig image-version create: Added support --os-snapshot and --data-snapshots</span></span>
* <span data-ttu-id="5f12f-804">image create: „--data-disk-caching“ hinzugefügt, um die Angabe der Zwischenspeicherungseinstellung von Datenträger zu ermöflichen</span><span class="sxs-lookup"><span data-stu-id="5f12f-804">image create: Added --data-disk-caching to allow specifying caching setting of data disks</span></span>
* <span data-ttu-id="5f12f-805">Upgrade des Python-Compute-SDK auf 10.0.0</span><span class="sxs-lookup"><span data-stu-id="5f12f-805">Upgraded Python Compute SDK to 10.0.0</span></span>
* <span data-ttu-id="5f12f-806">vm/vmss create: „Spot“ zu Aufzählungseigenschaft „Priority“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-806">vm/vmss create: Added 'Spot' to 'Priority' enum property</span></span>
* <span data-ttu-id="5f12f-807">[Breaking Change] Parameter „--max-billing“ für sowohl VM als auch VMSS in „--max-price“ umbenannt, um die Konsistenz mit Swagger- und PowerShell-Cmdlets sicherzustellen</span><span class="sxs-lookup"><span data-stu-id="5f12f-807">[Breaking change] Renamed '--max-billing' parameter to '--max-price', for both VM and VMSS, to be consistent with Swagger and Powershell cmdlets</span></span>
* <span data-ttu-id="5f12f-808">vm monitor log show: Unterstützung für das Abfragen von Protokollen über verknüpften Protokollanalyse-Arbeitsbereich hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-808">vm monitor log show: Added support for querying log over linked log analytics workspace.</span></span>

### <a name="iot"></a><span data-ttu-id="5f12f-809">IoT</span><span class="sxs-lookup"><span data-stu-id="5f12f-809">IOT</span></span>

* <span data-ttu-id="5f12f-810">Behebung Nr. 2531: Argumente für Benutzerfreundlichkeit für Hub-Update hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-810">Fix #2531: Added convenience arguments for hub update.</span></span>
* <span data-ttu-id="5f12f-811">Behebung Nr. 8323: Fehlende Parameter zum Erstellen eines benutzerdefinierten Speicherendpunkts hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-811">Fix #8323: Added missing parameters to create storage custom endpoint.</span></span>
* <span data-ttu-id="5f12f-812">Regressionsfehler behoben: Die Änderungen wurden rückgängig gemacht, sodass der standardmäßige Speicherendpunkt überschrieben wurde.</span><span class="sxs-lookup"><span data-stu-id="5f12f-812">Fix regression bug: Reverted the changes which overrides the default storage endpoint.</span></span>

### <a name="key-vault"></a><span data-ttu-id="5f12f-813">Key Vault</span><span class="sxs-lookup"><span data-stu-id="5f12f-813">Key Vault</span></span>

* <span data-ttu-id="5f12f-814">Nr. 11121 behoben: Bei der Verwendung von `az keyvault certificate list` erfordert die Übergabe von `--include-pending` jetzt nicht mehr den Wert `true` oder `false`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-814">Fixed #11121: When using `az keyvault certificate list`, passing `--include-pending` now doesn't require a value of `true` or `false`</span></span>

### <a name="netappfiles"></a><span data-ttu-id="5f12f-815">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="5f12f-815">NetAppFiles</span></span>

* <span data-ttu-id="5f12f-816">Upgrade von „azure-mgmt-netapp“ auf Version 0.7.0, die einige zusätzliche Volumeeigenschaften enthält, die bevorstehenden Replikationsvorgängen zugeordnet sind</span><span class="sxs-lookup"><span data-stu-id="5f12f-816">Upgraded azure-mgmt-netapp to 0.7.0 which includes some additional volume properties associated with upcoming replication operations</span></span>

### <a name="network"></a><span data-ttu-id="5f12f-817">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="5f12f-817">Network</span></span>

* <span data-ttu-id="5f12f-818">application-gateway waf-config: veraltet</span><span class="sxs-lookup"><span data-stu-id="5f12f-818">application-gateway waf-config: deprecated</span></span>
* <span data-ttu-id="5f12f-819">application-gateway waf-policy: Untergruppe „managed-rules“ zur Verwaltung von verwalteten Regelsätzen und Ausschlussregeln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-819">application-gateway waf-policy: Added subgroup managed-rules to manage managed rule sets and exclusion rules</span></span>
* <span data-ttu-id="5f12f-820">application-gateway waf-policy: Untergruppe „policy-setting“ zur Verwaltung der globalen Konfiguration von „waf-policy“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-820">application-gateway waf-policy: Added subgroup policy-setting to manage global configuration of a waf-policy</span></span>
* <span data-ttu-id="5f12f-821">[BREAKING CHANGE] application-gateway waf-policy: Untergruppenregel in „custom-rule“ umbenannt</span><span class="sxs-lookup"><span data-stu-id="5f12f-821">[BREAKING CHANGE] application-gateway waf-policy: Renamed subgroup rule to custom-rule</span></span>
* <span data-ttu-id="5f12f-822">application-gateway http-listener: „--firewall-policy“ beim Erstellen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-822">application-gateway http-listener: Added --firewall-policy when create</span></span>
* <span data-ttu-id="5f12f-823">application-gateway url-path-map rule: „--firewall-policy“ beim Erstellen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-823">application-gateway url-path-map rule: Added --firewall-policy when create</span></span>

### <a name="packaging"></a><span data-ttu-id="5f12f-824">Verpackung</span><span class="sxs-lookup"><span data-stu-id="5f12f-824">Packaging</span></span>

* <span data-ttu-id="5f12f-825">Az-Wrapper in Python neu geschrieben</span><span class="sxs-lookup"><span data-stu-id="5f12f-825">Rewrote the az wrapper in Python</span></span>
* <span data-ttu-id="5f12f-826">Unterstützung für Python 3.8 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-826">Added support for Python 3.8</span></span>
* <span data-ttu-id="5f12f-827">Für RPM-Paket in Python 3 geändert</span><span class="sxs-lookup"><span data-stu-id="5f12f-827">Changed to Python 3 for RPM package</span></span>

### <a name="profile"></a><span data-ttu-id="5f12f-828">Profil</span><span class="sxs-lookup"><span data-stu-id="5f12f-828">Profile</span></span>

* <span data-ttu-id="5f12f-829">Fehler beim Ausführen von `az login -u {} -p {}` mit Microsoft-Konto entfernt</span><span class="sxs-lookup"><span data-stu-id="5f12f-829">Polished error when running `az login -u {} -p {}` with Microsoft account</span></span>
* <span data-ttu-id="5f12f-830">`SSLError` beim Ausführen von `az login` hinter einem Proxy mit einem selbstsignierten Stammzertifikat entfernt</span><span class="sxs-lookup"><span data-stu-id="5f12f-830">Polished `SSLError` when running `az login` behind a proxy with self-signed root certificate</span></span>
* <span data-ttu-id="5f12f-831">Nr. 10578 behoben: `az login` hängt, wenn mehrere Instanzen gleichzeitig unter Windows oder WSL gestartet werden.</span><span class="sxs-lookup"><span data-stu-id="5f12f-831">Fixed #10578: `az login` hangs when more than one instances are launched at the same time on Windows or WSL</span></span>
* <span data-ttu-id="5f12f-832">Nr. 11059 behoben: `az login --allow-no-subscriptions` schlägt fehl, wenn Abonnements im Mandanten vorhanden sind.</span><span class="sxs-lookup"><span data-stu-id="5f12f-832">Fixed #11059: `az login --allow-no-subscriptions` fails if there are subscriptions in the tenant</span></span>
* <span data-ttu-id="5f12f-833">Nr. 11238 behoben: Nach dem Umbenennen eines Abonnements führt die Anmeldung mit MSI dazu, dass das gleiche Abonnement zweimal angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="5f12f-833">Fixed #11238: After renaming a subscription, logging in with MSI will result in the same subscription appearing twice</span></span>

### <a name="rbac"></a><span data-ttu-id="5f12f-834">RBAC</span><span class="sxs-lookup"><span data-stu-id="5f12f-834">RBAC</span></span>

* <span data-ttu-id="5f12f-835">Nr. 10996 behoben: Fehler für `--force-change-password-next-login` in `az ad user update` entfernt, wenn `--password` nicht angegeben ist</span><span class="sxs-lookup"><span data-stu-id="5f12f-835">Fixed #10996: Polish error for `--force-change-password-next-login` in `az ad user update` when `--password` is not specified</span></span>

### <a name="redis"></a><span data-ttu-id="5f12f-836">Redis</span><span class="sxs-lookup"><span data-stu-id="5f12f-836">Redis</span></span>

* <span data-ttu-id="5f12f-837">Nr. 2902 behoben: Festlegen von Speicherkonfigurationen beim Aktualisieren des Basic-SKU-Cache vermeiden</span><span class="sxs-lookup"><span data-stu-id="5f12f-837">Fixed #2902: Avoid setting memory configs while updating Basic SKU cache</span></span>

### <a name="reservations"></a><span data-ttu-id="5f12f-838">Reservations</span><span class="sxs-lookup"><span data-stu-id="5f12f-838">Reservations</span></span>

* <span data-ttu-id="5f12f-839">SDK-Version auf 0.6.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-839">Upgraded SDK Version to 0.6.0</span></span>
* <span data-ttu-id="5f12f-840">Abrechnungsplandetails nach dem Aufrufen von „Get-Gatalogs“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-840">Added billingplan details info after calling Get-Gatalogs</span></span>
* <span data-ttu-id="5f12f-841">Neuer Befehl `az reservations reservation-order calculate` zum Berechnen des Preises für eine Reservierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-841">Added new command `az reservations reservation-order calculate` to calculate the price for a reservation</span></span>
* <span data-ttu-id="5f12f-842">Neuer Befehl `az reservations reservation-order purchase` zum Erwerb einer neuen Reservierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-842">Added new command `az reservations reservation-order purchase` to purchase a new reservation</span></span>

### <a name="rest"></a><span data-ttu-id="5f12f-843">REST</span><span class="sxs-lookup"><span data-stu-id="5f12f-843">Rest</span></span>
* <span data-ttu-id="5f12f-844">`az rest` in allgemeine Verfügbarkeit geändert</span><span class="sxs-lookup"><span data-stu-id="5f12f-844">Changed `az rest` to GA</span></span>

### <a name="sql"></a><span data-ttu-id="5f12f-845">SQL</span><span class="sxs-lookup"><span data-stu-id="5f12f-845">SQL</span></span>

* <span data-ttu-id="5f12f-846">„azure-mgmt-sql“ auf Version 0.15.0 aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="5f12f-846">Updated azure-mgmt-sql to version 0.15.0.</span></span>

### <a name="storage"></a><span data-ttu-id="5f12f-847">Storage</span><span class="sxs-lookup"><span data-stu-id="5f12f-847">Storage</span></span>

* <span data-ttu-id="5f12f-848">storage account create: „--enable-hierarchical-namespace“ hinzugefügt, um Dateisystemsemantik in Blobdienst zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="5f12f-848">storage account create: Added --enable-hierarchical-namespace to support filesystem semantics in blob service.</span></span>
* <span data-ttu-id="5f12f-849">Ausnahme ohne Zusammenhang aus Fehlermeldung entfernt</span><span class="sxs-lookup"><span data-stu-id="5f12f-849">Removed unrelated exception from error message</span></span>
* <span data-ttu-id="5f12f-850">Probleme mit falscher Fehlermeldung „Sie verfügen nicht über die erforderlichen Berechtigungen zum Ausführen dieses Vorgangs“ behoben.</span><span class="sxs-lookup"><span data-stu-id="5f12f-850">Fixed issues with incorrect error message "You do not have the required permissions needed to perform this operation."</span></span> <span data-ttu-id="5f12f-851">bei Blockierung durch Netzwerkregeln oder bei „AuthenticationFailed“.</span><span class="sxs-lookup"><span data-stu-id="5f12f-851">when blocked by network rules or AuthenticationFailed.</span></span>

## <a name="november-4-2019"></a><span data-ttu-id="5f12f-852">4\. November 2019</span><span class="sxs-lookup"><span data-stu-id="5f12f-852">November 4, 2019</span></span>

<span data-ttu-id="5f12f-853">Version 2.0.76</span><span class="sxs-lookup"><span data-stu-id="5f12f-853">Version 2.0.76</span></span>

### <a name="acr"></a><span data-ttu-id="5f12f-854">ACR</span><span class="sxs-lookup"><span data-stu-id="5f12f-854">ACR</span></span>

* <span data-ttu-id="5f12f-855">Vorschauparameter `--pack-image-tag` wurde dem Befehl `az acr pack build` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-855">Added a preview parameter `--pack-image-tag` to command `az acr pack build`.</span></span>
* <span data-ttu-id="5f12f-856">Unterstützung der Aktivierung der Überwachung beim Erstellen einer Registrierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-856">Added support for enabling auditing on creating a registry</span></span>
* <span data-ttu-id="5f12f-857">Unterstützung von RBAC mit Repositoryumfang hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-857">Added support for Repository-scoped RBAC</span></span>

### <a name="aks"></a><span data-ttu-id="5f12f-858">AKS</span><span class="sxs-lookup"><span data-stu-id="5f12f-858">AKS</span></span>

* <span data-ttu-id="5f12f-859">`--enable-cluster-autoscaler`, `--min-count` und `--max-count` wurden dem Befehl `az aks create` hinzugefügt, sodass die automatische Clusterskalierung für den Knotenpool aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="5f12f-859">Added `--enable-cluster-autoscaler`, `--min-count` and `--max-count` to the `az aks create` command, which enables cluster autoscaler for the node pool.</span></span>
* <span data-ttu-id="5f12f-860">Die obigen Flags sowie `--update-cluster-autoscaler` und `--disable-cluster-autoscaler` wurden dem Befehl `az aks update` hinzugefügt, sodass Updates der automatischen Clusterskalierung zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="5f12f-860">Added the above flags as well as `--update-cluster-autoscaler` and `--disable-cluster-autoscaler` to the `az aks update` command, allowing updates to cluster autoscaler.</span></span>

### <a name="appconfig"></a><span data-ttu-id="5f12f-861">AppConfig</span><span class="sxs-lookup"><span data-stu-id="5f12f-861">AppConfig</span></span>

* <span data-ttu-id="5f12f-862">Befehlsgruppe der AppConfig-Funktion zum Verwalten von in einer App Configuration-Instanz gespeicherten Featureflags wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-862">Added appconfig feature command group to manage feature flags stored in an App Configuration.</span></span>
* <span data-ttu-id="5f12f-863">Geringfügiger Programmfehler für Befehl „appconfig kv export to file“ wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="5f12f-863">Fixed minor bug for appconfig kv export to file command.</span></span> <span data-ttu-id="5f12f-864">Das Lesen der Zieldateiinhalte wird während des Exports angehalten.</span><span class="sxs-lookup"><span data-stu-id="5f12f-864">Stop reading dest file contents during export.</span></span>

### <a name="appservice"></a><span data-ttu-id="5f12f-865">AppService</span><span class="sxs-lookup"><span data-stu-id="5f12f-865">AppService</span></span>

* <span data-ttu-id="5f12f-866">`az appservice plan create`: Unterstützung für das Festlegen von „persitescalung“ beim Erstellen eines App-Serviceplans wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-866">`az appservice plan create`: Added support to set 'persitescaling' on appservice plan create.</span></span>
* <span data-ttu-id="5f12f-867">Ein Problem wurde behoben, aufgrund dessen der Vorgang „webapp config ssl bind“ vorhandene Tags aus der Ressource entfernt hat.</span><span class="sxs-lookup"><span data-stu-id="5f12f-867">Fixed an issue where webapp config ssl bind operation was removing existing tags from the resource</span></span>
* <span data-ttu-id="5f12f-868">Flag `--build-remote` wurde für `az functionapp deployment source config-zip` hinzugefügt, um die Remotebuildaktion während der Funktions-App-Bereitstellung zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="5f12f-868">Added `--build-remote` flag for `az functionapp deployment source config-zip` to support remote build action during function app deployment.</span></span>
* <span data-ttu-id="5f12f-869">Die Standardknotenversion in Funktions-Apps wurde für Windows in ~ 10 geändert.</span><span class="sxs-lookup"><span data-stu-id="5f12f-869">Changed default node version on function apps to ~10 for Windows</span></span>
* <span data-ttu-id="5f12f-870">`--runtime-version`-Eigenschaft zu `az functionapp create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-870">Added `--runtime-version` property to `az functionapp create`</span></span>

### <a name="arm"></a><span data-ttu-id="5f12f-871">ARM</span><span class="sxs-lookup"><span data-stu-id="5f12f-871">ARM</span></span>

* <span data-ttu-id="5f12f-872">`az deployment/group deployment validate`: Parameter `--handle-extended-json-format` wurde hinzugefügt, um bei der Bereitstellung mehrere Zeilen und Kommentare in der JSON-Vorlage zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="5f12f-872">`az deployment/group deployment validate`: Added `--handle-extended-json-format` parameter to support multiline and comments in json template when deployment.</span></span>
* <span data-ttu-id="5f12f-873">„azure-mgmt-resource“ auf „2019-07-01“ festgelegt</span><span class="sxs-lookup"><span data-stu-id="5f12f-873">Bumped azure-mgmt-resource to 2019-07-01</span></span>

### <a name="backup"></a><span data-ttu-id="5f12f-874">Backup</span><span class="sxs-lookup"><span data-stu-id="5f12f-874">Backup</span></span>

* <span data-ttu-id="5f12f-875">Unterstützung für AzureFiles-Sicherung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-875">Added AzureFiles backup support</span></span>

### <a name="compute"></a><span data-ttu-id="5f12f-876">Compute</span><span class="sxs-lookup"><span data-stu-id="5f12f-876">Compute</span></span>

* <span data-ttu-id="5f12f-877">`az vm create`: Beim gleichzeitigen Festlegen von beschleunigtem Netzwerkbetrieb und einer vorhandenen NIC wurde eine Warnung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-877">`az vm create`: Added warning when specifying accelerated networking and an existing NIC together.</span></span>
* <span data-ttu-id="5f12f-878">`az vm create`: `--vmss` hinzugefügt, um eine vorhandene VM-Skalierungsgruppe anzugeben, welcher der virtuelle Computer zugewiesen werden soll.</span><span class="sxs-lookup"><span data-stu-id="5f12f-878">`az vm create`: Added `--vmss` to specify an existing virtual machine scale set that the virtual machine should be assigned to.</span></span>
* <span data-ttu-id="5f12f-879">`az vm/vmss create`: Eine lokale Kopie der Imagealiasdatei wurde hinzugefügt, sodass in einer eingeschränkten Netzwerkumgebung darauf zugegriffen werden kann.</span><span class="sxs-lookup"><span data-stu-id="5f12f-879">`az vm/vmss create`: Added a local copy of image alias file so that it can be accessed in a restricted network environment.</span></span>
* <span data-ttu-id="5f12f-880">`az vmss create`: `--orchestration-mode` hinzugefügt, um anzugeben, wie virtuelle Computer von der Skalierungsgruppe verwaltet werden.</span><span class="sxs-lookup"><span data-stu-id="5f12f-880">`az vmss create`: Added `--orchestration-mode` to specify how virtual machines are managed by the scale set.</span></span>
* <span data-ttu-id="5f12f-881">`az vm/vmss update`: `--ultra-ssd-enabled` hinzugefügt, um das Aktualisieren der SSD-Einstellung zuzulassen.</span><span class="sxs-lookup"><span data-stu-id="5f12f-881">`az vm/vmss update`: Added `--ultra-ssd-enabled` to allow updating ultra SSD setting.</span></span>
* <span data-ttu-id="5f12f-882">[BREAKING CHANGE] `az vm extension set`: Ein Fehler wurde behoben, aufgrund dessen Benutzer mit `--ids` keine Erweiterung auf einem virtuellen Computer festlegen konnten.</span><span class="sxs-lookup"><span data-stu-id="5f12f-882">[BREAKING CHANGE] `az vm extension set`: Fixed bug where users could not set an extension on a VM with `--ids`.</span></span>
* <span data-ttu-id="5f12f-883">Neue Befehle wurden zu `az vm image terms accept/cancel/show` hinzugefügt , um Azure Marketplace-Imagebedingungen zu verwalten.</span><span class="sxs-lookup"><span data-stu-id="5f12f-883">Added new commands `az vm image terms accept/cancel/show` to manage Azure Marketplace image terms.</span></span>
* <span data-ttu-id="5f12f-884">VMAccessForLinux auf Version 1.5 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-884">Updated VMAccessForLinux to version 1.5</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="5f12f-885">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="5f12f-885">CosmosDB</span></span>

* <span data-ttu-id="5f12f-886">[BREAKING CHANGE] `az sql container create`: `--partition-key-path` in erforderlichen Parameter geändert</span><span class="sxs-lookup"><span data-stu-id="5f12f-886">[BREAKING CHANGE] `az sql container create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="5f12f-887">[BREAKING CHANGE] `az gremlin graph create`: `--partition-key-path` in erforderlichen Parameter geändert</span><span class="sxs-lookup"><span data-stu-id="5f12f-887">[BREAKING CHANGE] `az gremlin graph create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="5f12f-888">`az sql container create`: `--unique-key-policy` und `--conflict-resolution-policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-888">`az sql container create`: Added `--unique-key-policy` and `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="5f12f-889">`az sql container create/update`: Aktualisierung des `--idx`-Standardschemas</span><span class="sxs-lookup"><span data-stu-id="5f12f-889">`az sql container create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="5f12f-890">`gremlin graph create`: `--conflict-resolution-policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-890">`gremlin graph create`: Added `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="5f12f-891">`gremlin graph create/update`: Aktualisierung des `--idx`-Standardschemas</span><span class="sxs-lookup"><span data-stu-id="5f12f-891">`gremlin graph create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="5f12f-892">Tippfehler in Hilfemeldung korrigiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-892">Fixed typo in help message</span></span>
* <span data-ttu-id="5f12f-893">Datenbank: Informationen zur eingestellten Unterstützung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-893">database: Added deprecation information</span></span>
* <span data-ttu-id="5f12f-894">Auflistung: Informationen zur eingestellten Unterstützung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-894">collection: Added deprecation information</span></span>

### <a name="iot"></a><span data-ttu-id="5f12f-895">IoT</span><span class="sxs-lookup"><span data-stu-id="5f12f-895">IoT</span></span>

* <span data-ttu-id="5f12f-896">Neuer Routingquelltyp hinzugefügt: DigitalTwinChangeEvents</span><span class="sxs-lookup"><span data-stu-id="5f12f-896">Added new routing source type: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="5f12f-897">Fehlende Features in `az iot hub create` behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-897">Fixed missing features in `az iot hub create`</span></span>

### <a name="key-vault"></a><span data-ttu-id="5f12f-898">Key Vault</span><span class="sxs-lookup"><span data-stu-id="5f12f-898">Key Vault</span></span>

* <span data-ttu-id="5f12f-899">Ein unerwarteter Fehler wurde behoben, bei dem keine Zertifikatdatei vorhanden war.</span><span class="sxs-lookup"><span data-stu-id="5f12f-899">Fixed an unexpected error when certificate file does not exist</span></span>
* <span data-ttu-id="5f12f-900">Funktionsunfähigkeit von `az keyvault recover/purge` behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-900">Fixed `az keyvault recover/purge` not working</span></span>

### <a name="netappfiles"></a><span data-ttu-id="5f12f-901">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="5f12f-901">NetAppFiles</span></span>

* <span data-ttu-id="5f12f-902">„azure-mgmt-netapp“ wurde auf 0.6.0 aktualisiert, um API-Version 2019-07-01 zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="5f12f-902">Upgraded azure-mgmt-netapp to 0.6.0 to use API version 2019-07-01.</span></span> <span data-ttu-id="5f12f-903">Diese neue API-Version umfasst:</span><span class="sxs-lookup"><span data-stu-id="5f12f-903">This new API version includes:</span></span>

    - <span data-ttu-id="5f12f-904">Volumeerstellung `--protocol-types` akzeptiert jetzt „NFSv4.1“ anstelle von „NFSv4“.</span><span class="sxs-lookup"><span data-stu-id="5f12f-904">Volume creation `--protocol-types` accepts now "NFSv4.1" not "NFSv4"</span></span>
    - <span data-ttu-id="5f12f-905">Die Richtlinie der Volumeexportrichtlinie heißt jetzt „nfsv41“ anstelle von „nfsv4“.</span><span class="sxs-lookup"><span data-stu-id="5f12f-905">Volume export policy property now named 'nfsv41' not 'nfsv4'</span></span>
    - <span data-ttu-id="5f12f-906">Volume `--creation-token` wurde in `--file-path` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-906">Volume `--creation-token` renamed to `--file-path`</span></span>
    - <span data-ttu-id="5f12f-907">Das Erstellungsdatum einer Momentaufnahme heißt jetzt einfach „erstellt“.</span><span class="sxs-lookup"><span data-stu-id="5f12f-907">Snapshot creation date now named just 'created'</span></span>

### <a name="network"></a><span data-ttu-id="5f12f-908">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="5f12f-908">Network</span></span>

* <span data-ttu-id="5f12f-909">`az network private-dns link vnet create/update`: Unterstützung für mandantenübergreifende Verknüpfung virtueller Netzwerke.</span><span class="sxs-lookup"><span data-stu-id="5f12f-909">`az network private-dns link vnet create/update`: Support cross-tenant virtual network linking.</span></span>
* <span data-ttu-id="5f12f-910">[BREAKING CHANGE] `az network vnet subnet list`: `--resource-group` und `--vnet-name` wurden geändert und sind jetzt erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5f12f-910">[BREAKING CHANGE] `az network vnet subnet list`: Changed `--resource-group` and `--vnet-name` to be required now.</span></span>
* <span data-ttu-id="5f12f-911">`az network public-ip prefix create`: Unterstützung der Angabe der IP-Adressversion (IPv4, IPv6) bei der Erstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-911">`az network public-ip prefix create`: Added support to specify IP address version (IPv4, IPv6) when creation</span></span>
* <span data-ttu-id="5f12f-912">„azure-mgmt-network“ auf 7.0.0 und „api-version“ auf 2019-09-01 festgelegt</span><span class="sxs-lookup"><span data-stu-id="5f12f-912">Bumped azure-mgmt-network to 7.0.0 and api-version to 2019-09-01</span></span>
* <span data-ttu-id="5f12f-913">`az network vrouter`: Unterstützung für neuen virtuellen Dienstrouter und virtuelles Routerpeering hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-913">`az network vrouter`: Added support for new service virtual router and virtual router peering</span></span>
* <span data-ttu-id="5f12f-914">`az network express-route gateway connection`: Unterstützung für `--internet-security` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-914">`az network express-route gateway connection`: Added support for `--internet-security`</span></span>

### <a name="profile"></a><span data-ttu-id="5f12f-915">Profil</span><span class="sxs-lookup"><span data-stu-id="5f12f-915">Profile</span></span>

* <span data-ttu-id="5f12f-916">Funktionsunfähigkeit von `az account get-access-token --resource-type ms-graph` behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-916">Fixed `az account get-access-token --resource-type ms-graph` not working</span></span>
* <span data-ttu-id="5f12f-917">Warnung aus `az login` entfernt</span><span class="sxs-lookup"><span data-stu-id="5f12f-917">Removed warning from `az login`</span></span>

### <a name="rbac"></a><span data-ttu-id="5f12f-918">RBAC</span><span class="sxs-lookup"><span data-stu-id="5f12f-918">RBAC</span></span>

* <span data-ttu-id="5f12f-919">Funktionsunfähigkeit von `az ad app update --id {} --display-name {}` behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-919">Fixed `az ad app update --id {} --display-name {}` doesn't work</span></span>

### <a name="servicefabric"></a><span data-ttu-id="5f12f-920">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="5f12f-920">ServiceFabric</span></span>

* <span data-ttu-id="5f12f-921">`az sf cluster create`: Ein Problem wurde behoben, indem die Compute-VMSS von „template.json“ für Service Fabric unter Linux und Windows von Standarddatenträgern auf verwaltete Datenträger umgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="5f12f-921">`az sf cluster create`: Fixed an issue by modifying service fabric linux and windows template.json compute vmss from standard to managed disks</span></span>

### <a name="sql"></a><span data-ttu-id="5f12f-922">SQL</span><span class="sxs-lookup"><span data-stu-id="5f12f-922">SQL</span></span>

* <span data-ttu-id="5f12f-923">Die Parameter `--compute-model`, `--auto-pause-delay` und `--min-capacity` wurden hinzugefügt, um CRUD-Vorgänge für das neue SQL-Datenbank-Angebot zu unterstützen: Serverloses Computemodell.</span><span class="sxs-lookup"><span data-stu-id="5f12f-923">Added `--compute-model`, `--auto-pause-delay`, and `--min-capacity` parameters to support CRUD operations for new SQL Database offering: Serverless compute model.</span></span>

### <a name="storage"></a><span data-ttu-id="5f12f-924">Storage</span><span class="sxs-lookup"><span data-stu-id="5f12f-924">Storage</span></span>

* <span data-ttu-id="5f12f-925">`az storage account create/update`: Parameter „--enable-files-adds“ und Azure Active Directory-Eigenschaftenargumentgruppe hinzugefügt, um Active Directory Domain-Dienstauthentifizierung für Azure Files zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="5f12f-925">`az storage account create/update`: Added --enable-files-adds parameter and Azure Active Directory Properties Argument group to support Azure Files Active Directory Domain Service Authentication</span></span>
* <span data-ttu-id="5f12f-926">`az storage account keys list/renew` wurde erweitert, um die Auflistung oder erneute Generierung von Kerberos-Schlüsseln des Speicherkontos zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="5f12f-926">Expanded `az storage account keys list/renew` to support listing or regenerating Kerberos keys of storage account.</span></span>

## <a name="october-15-2019"></a><span data-ttu-id="5f12f-927">15. Oktober 2019</span><span class="sxs-lookup"><span data-stu-id="5f12f-927">October 15, 2019</span></span>

<span data-ttu-id="5f12f-928">Version 2.0.75</span><span class="sxs-lookup"><span data-stu-id="5f12f-928">Version 2.0.75</span></span>

### <a name="aks"></a><span data-ttu-id="5f12f-929">AKS</span><span class="sxs-lookup"><span data-stu-id="5f12f-929">AKS</span></span>

* <span data-ttu-id="5f12f-930">Standardwert `--load-balancer-sku` in `standard` geändert, sofern von der Kubernetes-Version unterstützt</span><span class="sxs-lookup"><span data-stu-id="5f12f-930">Changed `--load-balancer-sku` default value to `standard` if supported by the kubernetes version</span></span>
* <span data-ttu-id="5f12f-931">Standardwert `--vm-set-type` in `virtualmachinescalesets` geändert, sofern von der Kubernetes-Version unterstützt</span><span class="sxs-lookup"><span data-stu-id="5f12f-931">Changed `--vm-set-type` default value to `virtualmachinescalesets` if supported by the kubernetes version</span></span>

### <a name="ams"></a><span data-ttu-id="5f12f-932">AMS</span><span class="sxs-lookup"><span data-stu-id="5f12f-932">AMS</span></span>

* <span data-ttu-id="5f12f-933">[BREAKING CHANGE] Name von `job start` in `job create` geändert</span><span class="sxs-lookup"><span data-stu-id="5f12f-933">[BREAKING CHANGE] Changed the name of `job start` to `job create`</span></span>
* <span data-ttu-id="5f12f-934">[BREAKING CHANGE] Parameter `--ask` von `content-key-policy create` geändert, sodass eine hexadezimale Zeichenfolge mit 32 Zeichen anstelle von UTF8 verwendet wird</span><span class="sxs-lookup"><span data-stu-id="5f12f-934">[BREAKING CHANGE] Changed the `--ask` parameter of `content-key-policy create` to use a 32-character hex string instead of UTF8</span></span>

### <a name="appservice"></a><span data-ttu-id="5f12f-935">AppService</span><span class="sxs-lookup"><span data-stu-id="5f12f-935">AppService</span></span>

* <span data-ttu-id="5f12f-936">Befehle vom Typ `webapp config access-restriction show|set|add|remove` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-936">Added commands `webapp config access-restriction show|set|add|remove`</span></span>
* <span data-ttu-id="5f12f-937">Bessere Fehlerbehandlung zu `webapp up` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-937">Added better error handling to `webapp up`</span></span>
* <span data-ttu-id="5f12f-938">Unterstützung für SKU `Isolated` zu `appservice plan update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-938">Added support for `Isolated` SKU to `appservice plan update`</span></span>

### <a name="arm"></a><span data-ttu-id="5f12f-939">ARM</span><span class="sxs-lookup"><span data-stu-id="5f12f-939">ARM</span></span>

* <span data-ttu-id="5f12f-940">Parameter `--handle-extended-json-format` zu `deployment create` hinzugefügt, um mehrere Zeilen und Kommentare in der JSON-Vorlage zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="5f12f-940">Added `--handle-extended-json-format` parameter `deployment create` to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="5f12f-941">Compute</span><span class="sxs-lookup"><span data-stu-id="5f12f-941">Compute</span></span>

* <span data-ttu-id="5f12f-942">Parameter `--enable-agent` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-942">Added `--enable-agent` parameter to `vm create`</span></span>
* <span data-ttu-id="5f12f-943">`vm create` geändert, um bei der Verwendung von Zonen die SKU „Standard“ für die öffentliche IP-Adresse zu verwenden</span><span class="sxs-lookup"><span data-stu-id="5f12f-943">Changed `vm create` to use standard public IP SKU automatically when using zones</span></span>
* <span data-ttu-id="5f12f-944">`vm create` geändert, um automatisch einen gültigen Computernamen für eine VM zu erstellen, falls keiner angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="5f12f-944">Changed `vm create` to automatically create a valid computer name for a VM if none is provided</span></span>
* <span data-ttu-id="5f12f-945">Parameter `--computer-name-prefix` zu `vmss create` hinzugefügt, um das benutzerdefinierte Computernamenspräfix virtueller Computer in VMSS zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="5f12f-945">Added `--computer-name-prefix` parameter to `vmss create` to support custom computer name prefix of virtual machines in the VMSS</span></span>
* <span data-ttu-id="5f12f-946">Parameter `--workspace` zu `vm create` hinzugefügt, um automatisch einen Log Analytics-Arbeitsbereich zu aktivieren</span><span class="sxs-lookup"><span data-stu-id="5f12f-946">Add `--workspace` parameter to `vm create` to enable log analytics workspace automatically</span></span>
* <span data-ttu-id="5f12f-947">API-Version für Kataloge auf 2019-07-01 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-947">Updated galleries API version to 2019-07-01</span></span>

### <a name="core"></a><span data-ttu-id="5f12f-948">Core</span><span class="sxs-lookup"><span data-stu-id="5f12f-948">Core</span></span>

* <span data-ttu-id="5f12f-949">Syntaxprüfung für Parameter `--set` im generischen Updatebefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-949">Added syntax check for `--set` parameter in generic update command</span></span>

### <a name="iot"></a><span data-ttu-id="5f12f-950">IoT</span><span class="sxs-lookup"><span data-stu-id="5f12f-950">IoT</span></span>

* <span data-ttu-id="5f12f-951">Problem behoben, bei dem für `iot hub show` der Fehler „Ressource nicht gefunden.“ zurückgegeben wurde</span><span class="sxs-lookup"><span data-stu-id="5f12f-951">Fixed an issue where `iot hub show` would incorrectly error with "resource not found"</span></span>

### <a name="monitor"></a><span data-ttu-id="5f12f-952">Überwachen</span><span class="sxs-lookup"><span data-stu-id="5f12f-952">Monitor</span></span>

* <span data-ttu-id="5f12f-953">Unterstützung für CRUD zu `monitor log-analytics workspace` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-953">Added support for CRUD to `monitor log-analytics workspace`</span></span>

### <a name="network"></a><span data-ttu-id="5f12f-954">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="5f12f-954">Network</span></span>

* <span data-ttu-id="5f12f-955">Unterstützung für mandantenübergreifende virtuelle Verbindung zu `network private-dns link vnet [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-955">Added support for cross-tenant virtual linking to `network private-dns link vnet [create|update]`</span></span>
* <span data-ttu-id="5f12f-956">[BREAKING CHANGE]`network vnet subnet list` geändert, um Parameter `--resource-group` und `--vnet-name` vorauszusetzen</span><span class="sxs-lookup"><span data-stu-id="5f12f-956">[BREAKING CHANGE] Changed `network vnet subnet list` to require `--resource-group` and `--vnet-name` parameters</span></span>

### <a name="sql"></a><span data-ttu-id="5f12f-957">SQL</span><span class="sxs-lookup"><span data-stu-id="5f12f-957">SQL</span></span>

* <span data-ttu-id="5f12f-958">Befehle zu `sql mi ad-admin` hinzugefügt, die das Festlegen eines AAD-Administrators für verwaltete Instanzen unterstützen</span><span class="sxs-lookup"><span data-stu-id="5f12f-958">Added commands to `sql mi ad-admin` that support setting an AAD administrator on managed instances</span></span>

### <a name="storage"></a><span data-ttu-id="5f12f-959">Storage</span><span class="sxs-lookup"><span data-stu-id="5f12f-959">Storage</span></span>

* <span data-ttu-id="5f12f-960">Parameter `--preserve-s2s-access-tier` zu `storage copy` hinzugefügt, um die Zugriffsebene beim Kopieren von Dienst zu Dienst beizubehalten</span><span class="sxs-lookup"><span data-stu-id="5f12f-960">Added `--preserve-s2s-access-tier` parameter `storage copy` to preserve access tier during service to service copy</span></span>
* <span data-ttu-id="5f12f-961">Parameter `--enable-large-file-share` zu `storage account [create|update]` hinzugefügt, um große Dateifreigaben für ein Speicherkonto zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="5f12f-961">Added `--enable-large-file-share` parameter to `storage account [create|update]` to support large file shares for storage account</span></span>

## <a name="september-24-2019"></a><span data-ttu-id="5f12f-962">24. September 2019</span><span class="sxs-lookup"><span data-stu-id="5f12f-962">September 24, 2019</span></span>

<span data-ttu-id="5f12f-963">Version 2.0.74</span><span class="sxs-lookup"><span data-stu-id="5f12f-963">Version 2.0.74</span></span>

### <a name="acr"></a><span data-ttu-id="5f12f-964">ACR</span><span class="sxs-lookup"><span data-stu-id="5f12f-964">ACR</span></span>

* <span data-ttu-id="5f12f-965">Erforderlicher Parameter `--type` zu `acr config retention update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-965">Added a required `--type` parameter to `acr config retention update`</span></span>
* <span data-ttu-id="5f12f-966">[BREAKING CHANGE] Umbenannter Parameter `--name -n` in `--registry -r ` für Befehlsgruppe `acr config` geändert</span><span class="sxs-lookup"><span data-stu-id="5f12f-966">[BREAKING CHANGE] Renamed parameter `--name -n` changed to `--registry -r ` for `acr config` command group</span></span>

### <a name="aks"></a><span data-ttu-id="5f12f-967">AKS</span><span class="sxs-lookup"><span data-stu-id="5f12f-967">AKS</span></span>

* <span data-ttu-id="5f12f-968">Parameter `--load-balancer-sku` zum Befehl `aks create` hinzugefügt, um die Erstellung von AKS-Clustern mit SLB zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="5f12f-968">Added `--load-balancer-sku` parameter to `aks create` command, which allows for creating AKS cluster with SLB</span></span>
* <span data-ttu-id="5f12f-969">Parameter `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` und `--load-balancer-outbound-ip-prefixes` zu den Befehlen `aks [create|update]` hinzugefügt,um die Aktualisierung des Lastenausgleichsprofils eines AKS-Clusters mit SLB zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="5f12f-969">Added `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` and `--load-balancer-outbound-ip-prefixes` parameters to `aks [create|update]` commands, which allow for updating load balancer profile of an AKS cluster with SLB</span></span>
* <span data-ttu-id="5f12f-970">Parameter `--vm-set-type` zum Befehl `aks create` hinzugefügt, um die Angabe von VM-Typen eines AKS-Clusters (vmas oder vmss) zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="5f12f-970">Added `--vm-set-type` parameter to `aks create` command, which allows to specify vm types of an AKS Cluster (vmas or vmss)</span></span>

### <a name="arm"></a><span data-ttu-id="5f12f-971">ARM</span><span class="sxs-lookup"><span data-stu-id="5f12f-971">ARM</span></span>

* <span data-ttu-id="5f12f-972">Parameter `--handle-extended-json-format` zum Befehl `group deployment create` hinzugefügt, um mehrere Zeilen und Kommentare in der JSON-Vorlage zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="5f12f-972">Added `--handle-extended-json-format` parameter to `group deployment create` command to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="5f12f-973">Compute</span><span class="sxs-lookup"><span data-stu-id="5f12f-973">Compute</span></span>

* <span data-ttu-id="5f12f-974">Parameter `--terminate-notification-time` zu den Befehlen `vmss [create|update]` hinzugefügt, um die Konfigurierbarkeit der Beendigung geplanter Ereignisse zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="5f12f-974">Added `--terminate-notification-time` parameter to `vmss [create|update]` commands to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="5f12f-975">Parameter `--enable-terminate-notification` zu den Befehlen `vmss update` hinzugefügt, um die Konfigurierbarkeit der Beendigung geplanter Ereignisse zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="5f12f-975">Added `--enable-terminate-notification` parameter to `vmss update` command to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="5f12f-976">Parameter `--priority,` `--eviction-policy,` `--max-billing` zu `[vm|vmss] create`-Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-976">Added `--priority,` `--eviction-policy,` `--max-billing` parameters to `[vm|vmss] create` commands</span></span>
* <span data-ttu-id="5f12f-977">`disk create` geändert, um die Angabe der genauen Größe des Datenträgeruploads zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="5f12f-977">Changed `disk create` to allow specifying the exact size of the disk upload</span></span>
* <span data-ttu-id="5f12f-978">Unterstützung für inkrementelle Momentaufnahmen für verwaltete Datenträger zu `snapshot create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-978">Added support for incremental snapshots for managed disks to `snapshot create`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="5f12f-979">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="5f12f-979">Cosmos DB</span></span>

* <span data-ttu-id="5f12f-980">Parameter `--type <key-type>` zum Befehl `cosmosdb keys list` hinzugefügt, um Schlüssel, schreibgeschützte Schlüssel oder Verbindungszeichenfolgen anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="5f12f-980">Added `--type <key-type>` parameter to `cosmosdb keys list` command to show key, read only keys or connection strings</span></span>
* <span data-ttu-id="5f12f-981">Befehl `cosmosdb keys regenerate` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-981">Added `cosmosdb keys regenerate` command</span></span>
* <span data-ttu-id="5f12f-982">[VERALTET] Befehle `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` und `cosmosdb list-read-only-keys` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-982">[DEPRECATED] Deprecated `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` and `cosmosdb list-read-only-keys` commands</span></span>

### <a name="eventgrid"></a><span data-ttu-id="5f12f-983">EventGrid</span><span class="sxs-lookup"><span data-stu-id="5f12f-983">EventGrid</span></span>

* <span data-ttu-id="5f12f-984">Endpunkthilfetext korrigiert, um auf den richtigen Parameter zu verweisen</span><span class="sxs-lookup"><span data-stu-id="5f12f-984">Fixed the endpoint help text to refer to the right parameter</span></span>

### <a name="key-vault"></a><span data-ttu-id="5f12f-985">Key Vault</span><span class="sxs-lookup"><span data-stu-id="5f12f-985">Key Vault</span></span>

* <span data-ttu-id="5f12f-986">Problem behoben, aufgrund dessen die Anmeldung mit einem Mandanten (`login -t`) unter Umständen zu einem Fehler von `keyvault create` führte</span><span class="sxs-lookup"><span data-stu-id="5f12f-986">Fixed issue where logging in with a tenant (`login -t`) could cause `keyvault create` to fail</span></span>

### <a name="monitor"></a><span data-ttu-id="5f12f-987">Überwachen</span><span class="sxs-lookup"><span data-stu-id="5f12f-987">Monitor</span></span>

* <span data-ttu-id="5f12f-988">Problem behoben, aufgrund dessen das Zeichen `:` in `--condition` für `monitor metrics alert create` nicht zulässig war</span><span class="sxs-lookup"><span data-stu-id="5f12f-988">Fixed issue where `:` character was not allowed in `--condition` argument to `monitor metrics alert create`</span></span>

### <a name="policy"></a><span data-ttu-id="5f12f-989">Richtlinie</span><span class="sxs-lookup"><span data-stu-id="5f12f-989">Policy</span></span>

* <span data-ttu-id="5f12f-990">Unterstützung für Policy-API-Version 2019-06-01 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-990">Added support for Policy API version 2019-06-01</span></span>
* <span data-ttu-id="5f12f-991">Parameter `--enforcement-mode` zum Befehl `policy assignment create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-991">Added `--enforcement-mode` parameter to `policy assignment create` command</span></span>

### <a name="storage"></a><span data-ttu-id="5f12f-992">Storage</span><span class="sxs-lookup"><span data-stu-id="5f12f-992">Storage</span></span>

* <span data-ttu-id="5f12f-993">Parameter `--blob-type` zum Befehl `az storage copy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-993">Added `--blob-type` parameter to `az storage copy` command</span></span>

## <a name="september-10-2019"></a><span data-ttu-id="5f12f-994">10. September 2019</span><span class="sxs-lookup"><span data-stu-id="5f12f-994">September 10, 2019</span></span>

### <a name="acr"></a><span data-ttu-id="5f12f-995">ACR</span><span class="sxs-lookup"><span data-stu-id="5f12f-995">ACR</span></span>

* <span data-ttu-id="5f12f-996">Befehlsgruppe `acr config retention` zum Konfigurieren der Aufbewahrungsrichtlinie hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-996">Added command group `acr config retention` to configure retention policy</span></span>

### <a name="aks"></a><span data-ttu-id="5f12f-997">AKS</span><span class="sxs-lookup"><span data-stu-id="5f12f-997">AKS</span></span>

* <span data-ttu-id="5f12f-998">Unterstützung für die ACR-Integration mit den folgenden Befehlen hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="5f12f-998">Added support for ACR integration with the following commands:</span></span>
  * <span data-ttu-id="5f12f-999">Parameter `--attach-acr` zu `aks [create|update]` hinzugefügt, um einen ACR an einen AKS-Cluster anzufügen</span><span class="sxs-lookup"><span data-stu-id="5f12f-999">Added `--attach-acr` parameter to `aks [create|update]` to attach an ACR to an AKS cluster</span></span>
  * <span data-ttu-id="5f12f-1000">Parameter `--detach-acr` zu `aks update` hinzugefügt, um den ACR von einem AKS-Cluster zu trennen</span><span class="sxs-lookup"><span data-stu-id="5f12f-1000">Added `--detach-acr` parameter to `aks update` to detach the ACR from an AKS cluster</span></span>

### <a name="arm"></a><span data-ttu-id="5f12f-1001">ARM</span><span class="sxs-lookup"><span data-stu-id="5f12f-1001">ARM</span></span>

* <span data-ttu-id="5f12f-1002">Zur Verwendung der API-Version 2019-05-10 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-1002">Updated to use API version 2019-05-10</span></span>

### <a name="batch"></a><span data-ttu-id="5f12f-1003">Batch</span><span class="sxs-lookup"><span data-stu-id="5f12f-1003">Batch</span></span>

* <span data-ttu-id="5f12f-1004">Neue JSON-Konfigurationseinstellungen für `batch pool create` zu `--json-file` hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="5f12f-1004">Added new JSON configuration settings to `--json-file` for `batch pool create`:</span></span>
  * <span data-ttu-id="5f12f-1005">`MountConfigurations` für Dateisystemeinbindungen hinzugefügt (Details siehe https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body )</span><span class="sxs-lookup"><span data-stu-id="5f12f-1005">Added `MountConfigurations` for file system mounts (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
  * <span data-ttu-id="5f12f-1006">Optionale Eigenschaft `publicIPs` in `NetworkConfiguration` für öffentliche IP-Adressen für Pools hinzugefügt (Details siehe https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body )</span><span class="sxs-lookup"><span data-stu-id="5f12f-1006">Added optional property `publicIPs` on `NetworkConfiguration` for public IPs on pools (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
* <span data-ttu-id="5f12f-1007">Unterstützung für Kataloge mit freigegebenen Images zu `--image` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1007">Added support for shared image galleries to `--image`</span></span>
* <span data-ttu-id="5f12f-1008">[BREAKING CHANGE] Standardwert von `--start-task-wait-for-success` für `batch pool create` in `true` geändert</span><span class="sxs-lookup"><span data-stu-id="5f12f-1008">[BREAKING CHANGE] Changed default value of `--start-task-wait-for-success` on `batch pool create` to be `true`</span></span>
* <span data-ttu-id="5f12f-1009">[BREAKING CHANGE] Standardwert von `Scope` für `AutoUserSpecification` geändert, damit immer „Pool“ verwendet wird (vormals `Task` für Windows-Knoten bzw. `Pool` für Linux-Knoten)</span><span class="sxs-lookup"><span data-stu-id="5f12f-1009">[BREAKING CHANGE] Changed default value for `Scope` on `AutoUserSpecification` to always be Pool (was `Task` on Windows nodes, `Pool` on Linux nodes)</span></span>
  * <span data-ttu-id="5f12f-1010">Dieses Argument kann nur über eine JSON-Konfiguration mit `--json-file` festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1010">This argument can only be set from a JSON configuration with `--json-file`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="5f12f-1011">HDInsight</span><span class="sxs-lookup"><span data-stu-id="5f12f-1011">HDInsight</span></span>

* <span data-ttu-id="5f12f-1012">Allgemein verfügbares Release</span><span class="sxs-lookup"><span data-stu-id="5f12f-1012">GA release</span></span>
* <span data-ttu-id="5f12f-1013">[BREAKING CHANGE] Parameter `--workernode-count/-c` von `az hdinsight resize` in erforderlich geändert</span><span class="sxs-lookup"><span data-stu-id="5f12f-1013">[BREAKING CHANGE] Changed parameter `--workernode-count/-c` of `az hdinsight resize` to be required.</span></span>

### <a name="key-vault"></a><span data-ttu-id="5f12f-1014">Key Vault</span><span class="sxs-lookup"><span data-stu-id="5f12f-1014">Key Vault</span></span>

* <span data-ttu-id="5f12f-1015">Problem behoben, aufgrund dessen Subnetze nicht aus Netzwerkregeln gelöscht werden konnten</span><span class="sxs-lookup"><span data-stu-id="5f12f-1015">Fixed issue where subnets couldn't be deleted from network rules</span></span>
* <span data-ttu-id="5f12f-1016">Problem behoben, aufgrund dessen doppelte Subnetze und IP-Adressen zu Netzwerkregeln hinzugefügt werden konnten</span><span class="sxs-lookup"><span data-stu-id="5f12f-1016">Fixed issue where duplicated subnets and IP addresses could be added to network rules</span></span>

### <a name="network"></a><span data-ttu-id="5f12f-1017">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="5f12f-1017">Network</span></span>

* <span data-ttu-id="5f12f-1018">Parameter `--interval` zu `network watcher flow-log` hinzugefügt, um den Wert für das Intervall der Datenverkehrsanalyse festzulegen</span><span class="sxs-lookup"><span data-stu-id="5f12f-1018">Added `--interval` parameter to `network watcher flow-log` to set traffic analysis interval value</span></span>
* <span data-ttu-id="5f12f-1019">`network application-gateway identity` zum Verwalten der Gatewayidentität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1019">Added `network application-gateway identity` to manage gateway identity</span></span>
* <span data-ttu-id="5f12f-1020">Unterstützung zum Festlegen der Key Vault-ID zu `network application-gateway ssl-cert` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1020">Added support for setting Key Vault ID to `network application-gateway ssl-cert`</span></span>
* <span data-ttu-id="5f12f-1021">`network express-route peering peer-connection [show|list]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1021">Added `network express-route peering peer-connection [show|list]`</span></span>

### <a name="policy"></a><span data-ttu-id="5f12f-1022">Richtlinie</span><span class="sxs-lookup"><span data-stu-id="5f12f-1022">Policy</span></span>

* <span data-ttu-id="5f12f-1023">Zur Verwendung der API-Version 2019-01-01 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-1023">Updated to use API version 2019-01-01</span></span>

## <a name="august-27-2019"></a><span data-ttu-id="5f12f-1024">27. August 2019</span><span class="sxs-lookup"><span data-stu-id="5f12f-1024">August 27, 2019</span></span>

<span data-ttu-id="5f12f-1025">Version 2.0.72</span><span class="sxs-lookup"><span data-stu-id="5f12f-1025">Version 2.0.72</span></span>

### <a name="acr"></a><span data-ttu-id="5f12f-1026">ACR</span><span class="sxs-lookup"><span data-stu-id="5f12f-1026">ACR</span></span>

* <span data-ttu-id="5f12f-1027">[BREAKING CHANGE] Unterstützung für SKU `classic` entfernt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1027">[BREAKING CHANGE] Removed support for the `classic` SKU</span></span>

### <a name="api-management"></a><span data-ttu-id="5f12f-1028">API Management</span><span class="sxs-lookup"><span data-stu-id="5f12f-1028">API Management</span></span>

* <span data-ttu-id="5f12f-1029">[VORSCHAU] Befehlsgruppe `apim` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1029">[PREVIEW] Added `apim` command group</span></span>

### <a name="appservice"></a><span data-ttu-id="5f12f-1030">AppService</span><span class="sxs-lookup"><span data-stu-id="5f12f-1030">AppService</span></span>

* <span data-ttu-id="5f12f-1031">Problem mit dem Befehl `webapp webjob continuous start` bei Angabe eines Slots behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-1031">Fixed issue with `webapp webjob continuous start` command when specifying a slot</span></span>
* <span data-ttu-id="5f12f-1032">`webapp up` geändert, um den Ordner `env` zu erkennen und aus der für die Bereitstellung verwendeten Datei zu entfernen</span><span class="sxs-lookup"><span data-stu-id="5f12f-1032">Changed `webapp up` to detect `env` folder and remove it from the file used for deployment</span></span>

### <a name="keyvault"></a><span data-ttu-id="5f12f-1033">KeyVault</span><span class="sxs-lookup"><span data-stu-id="5f12f-1033">Keyvault</span></span>

* <span data-ttu-id="5f12f-1034">Fehler in `keyvault secret set` behoben, aufgrund dessen das Argument `--expires` ignoriert wurde</span><span class="sxs-lookup"><span data-stu-id="5f12f-1034">Fixed a bug in `keyvault secret set` that igored the `--expires` argument</span></span>

### <a name="network"></a><span data-ttu-id="5f12f-1035">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="5f12f-1035">Network</span></span>

* <span data-ttu-id="5f12f-1036">Unterstützung für IPv6-Adressen zu Argumenten vom Typ `--private-ip-address-version` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1036">Added support for IPv6 addresses to `--private-ip-address-version` arguments</span></span>
* <span data-ttu-id="5f12f-1037">Neue Befehle vom Typ `network private-endpoint [create|update|list-types]` für die Verwaltung privater Endpunkte hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1037">Added new commands `network private-endpoint [create|update|list-types]` for private endpoint management</span></span>
* <span data-ttu-id="5f12f-1038">Befehlsgruppe `network private-link-service` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1038">Added command group `network private-link-service`</span></span>
* <span data-ttu-id="5f12f-1039">Argumente `--private-endpoint-network-policies` und `--private-link-service-network-policies` zu `network vnet subnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1039">Added `--private-endpoint-network-policies` and `--private-link-service-network-policies` arguments to `network vnet subnet update`</span></span>

### <a name="rbac"></a><span data-ttu-id="5f12f-1040">RBAC</span><span class="sxs-lookup"><span data-stu-id="5f12f-1040">RBAC</span></span>

* <span data-ttu-id="5f12f-1041">Problem mit `ad app update --homepage` behoben, aufgrund dessen die Startseite nicht aktualisiert wurde</span><span class="sxs-lookup"><span data-stu-id="5f12f-1041">Fixed issue with `ad app update --homepage` where homepage would not be updated</span></span>

### <a name="servicefabric"></a><span data-ttu-id="5f12f-1042">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="5f12f-1042">ServiceFabric</span></span>

* <span data-ttu-id="5f12f-1043">Unterstützung für Key Vault-Namen mit Groß- und Kleinschreibung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1043">Added support for mixed-case Key Vault names</span></span>
* <span data-ttu-id="5f12f-1044">Problem bei der Verwendung von Zertifikaten in Key Vault behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-1044">Fixed issue when using certificates in Key Vault</span></span>
* <span data-ttu-id="5f12f-1045">Problem bei der Verwendung von PFX-Zertifikatdateien behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-1045">Fixed issue with using PFX certificate files</span></span>
* <span data-ttu-id="5f12f-1046">Problem mit `sf cluster certificate add` behoben, wenn keine Key Vault-Ressourcengruppe angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="5f12f-1046">Fixed issue with `sf cluster certificate add` when Key Vault resource group wasn't specified</span></span>
* <span data-ttu-id="5f12f-1047">Problem behoben, aufgrund dessen `sf cluster set` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="5f12f-1047">Fixed issue with `sf cluster set` not working</span></span>

### <a name="signalr"></a><span data-ttu-id="5f12f-1048">SignalR</span><span class="sxs-lookup"><span data-stu-id="5f12f-1048">SignalR</span></span>

* <span data-ttu-id="5f12f-1049">Neue Befehle hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="5f12f-1049">Added new commands:</span></span>
  * <span data-ttu-id="5f12f-1050">`signalr cors`: Verwalten von CORS für SignalR</span><span class="sxs-lookup"><span data-stu-id="5f12f-1050">`signalr cors`: Manage SignalR CORS</span></span>
  * <span data-ttu-id="5f12f-1051">`signalr restart`: Starten eines SignalR-Diensts</span><span class="sxs-lookup"><span data-stu-id="5f12f-1051">`signalr restart`: Restart a SignalR service</span></span>
  * <span data-ttu-id="5f12f-1052">`signalr update`: Aktualisieren eines SignalR-Diensts</span><span class="sxs-lookup"><span data-stu-id="5f12f-1052">`signalr update`: Update a SignalR service</span></span>
* <span data-ttu-id="5f12f-1053">Argument `--service-mode` zu `signalr create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1053">Added `--service-mode` argument to `signalr create`</span></span>

### <a name="storage"></a><span data-ttu-id="5f12f-1054">Storage</span><span class="sxs-lookup"><span data-stu-id="5f12f-1054">Storage</span></span>

* <span data-ttu-id="5f12f-1055">Befehl `storage account revoke-delegation-keys` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1055">Added `storage account revoke-delegation-keys` command</span></span>

## <a name="august-13-2019"></a><span data-ttu-id="5f12f-1056">13. August 2019</span><span class="sxs-lookup"><span data-stu-id="5f12f-1056">August 13, 2019</span></span>

<span data-ttu-id="5f12f-1057">Version 2.0.71</span><span class="sxs-lookup"><span data-stu-id="5f12f-1057">Version 2.0.71</span></span>

### <a name="appservice"></a><span data-ttu-id="5f12f-1058">AppService</span><span class="sxs-lookup"><span data-stu-id="5f12f-1058">AppService</span></span>

* <span data-ttu-id="5f12f-1059">Problem behoben, aufgrund dessen bei Befehlen vom Typ `webapp webjob continuous` für Slots Fehler auftraten</span><span class="sxs-lookup"><span data-stu-id="5f12f-1059">Fixed issue where `webapp webjob continuous` commands were failing for slots</span></span>

### <a name="botservice"></a><span data-ttu-id="5f12f-1060">BotService</span><span class="sxs-lookup"><span data-stu-id="5f12f-1060">BotService</span></span>

* <span data-ttu-id="5f12f-1061">[BREAKING CHANGE] Unterstützung für die Erstellung von Bots der Version 3 entfernt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1061">[BREAKING CHANGE] Removed support for creating v3 SDK bots</span></span>

### <a name="cognitiveservices"></a><span data-ttu-id="5f12f-1062">CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="5f12f-1062">CognitiveServices</span></span>

* <span data-ttu-id="5f12f-1063">Befehle vom Typ `cognitiveservices account network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1063">Added `cognitiveservices account network-rule` commands</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="5f12f-1064">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="5f12f-1064">Cosmos DB</span></span>

* <span data-ttu-id="5f12f-1065">Beim Aktualisieren mehrerer Schreibstandorte wurde eine Warnung entfernt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1065">Removed warning when updating multiple write locations</span></span>
* <span data-ttu-id="5f12f-1066">CRUD-Befehle für CosmosDB SQL-, MongoDB-, Cassandra-, Gremlin- und Tabellenressourcen sowie den Ressourcendurchsatz hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1066">Added CRUD commands for CosmosDB SQL, MongoDB, Cassandra, Gremlin and Table resources and resource's throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="5f12f-1067">HDInsight</span><span class="sxs-lookup"><span data-stu-id="5f12f-1067">HDInsight</span></span>

<span data-ttu-id="5f12f-1068">Dieses Release enthält zahlreiche wichtige Änderungen.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1068">This release contains a large number of breaking changes.</span></span>

* <span data-ttu-id="5f12f-1069">[BREAKING CHANGE] Parameter für `hdinsight create` umbenannt:</span><span class="sxs-lookup"><span data-stu-id="5f12f-1069">[BREAKING CHANGE] Renamed parameters for `hdinsight create`:</span></span>
  * <span data-ttu-id="5f12f-1070">`--storage-default-container` in `--storage-container` umbenannt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1070">Renamed `--storage-default-container` to `--storage-container`</span></span>
  * <span data-ttu-id="5f12f-1071">`--storage-default-filesystem` in `--storage-filesystem` umbenannt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1071">Renamed `--storage-default-filesystem` to `--storage-filesystem`</span></span>
* <span data-ttu-id="5f12f-1072">[BREAKING CHANGE] Das Argument `--name` von `application create` wurde so geändert, dass es den Anwendungsnamen anstelle des Clusternamens darstellt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1072">[BREAKING CHANGE] Changed the `--name` argument of `application create` to represent the application name instead of the cluster name</span></span>
* <span data-ttu-id="5f12f-1073">Argument `--cluster-name` zu `application create` hinzugefügt, um die alte Funktion `--name` zu ersetzen</span><span class="sxs-lookup"><span data-stu-id="5f12f-1073">Added `--cluster-name` argument to `application create` to replace old `--name` functionality</span></span>
* <span data-ttu-id="5f12f-1074">[BREAKING CHANGE] Parameter für `application create` umbenannt:</span><span class="sxs-lookup"><span data-stu-id="5f12f-1074">[BREAKING CHANGE] Renamed parameters for `application create`:</span></span>
  * <span data-ttu-id="5f12f-1075">`--application-type` in `--type` umbenannt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1075">Renamed `--application-type` to `--type`</span></span>
  * <span data-ttu-id="5f12f-1076">`--marketplace-identifier` in `--marketplace-id` umbenannt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1076">Renamed `--marketplace-identifier` to `--marketplace-id`</span></span>
  * <span data-ttu-id="5f12f-1077">`--https-endpoint-access-mode` in `--access-mode` umbenannt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1077">Renamed `--https-endpoint-access-mode` to `--access-mode`</span></span>
  * <span data-ttu-id="5f12f-1078">`--https-endpoint-destination-port` in `--destination-port` umbenannt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1078">Renamed  `--https-endpoint-destination-port` to `--destination-port`</span></span>
* <span data-ttu-id="5f12f-1079">[BREAKING CHANGE] Parameter für `application create` entfernt:</span><span class="sxs-lookup"><span data-stu-id="5f12f-1079">[BREAKING CHANGE] Removed parameters for `application create`:</span></span>
  * `--https-endpoint-location`
  * `--https-endpoint-public-port`
  * `--ssh-endpoint-destination-port`
  * `--ssh-endpoint-location`
  * `--ssh-endpoint-public-port`
* <span data-ttu-id="5f12f-1080">[WICHTIGE ÄNDERUNG] `--target-instance-count` für `hdinsight resize` in `--workernode-count` umbenannt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1080">[BREAKING CHNAGE] Renamed `--target-instance-count` to `--workernode-count` for `hdinsight resize`</span></span>
* <span data-ttu-id="5f12f-1081">[BREAKING CHANGE] Alle Befehle in der Gruppe `hdinsight script-action` wurden so geändert, dass sie den Parameter `--name` als Namen der Skriptaktion verwenden.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1081">[BREAKING CHANGE] Changed all commands in the `hdinsight script-action` group to use the `--name` parameter as the name of the script action.</span></span>
* <span data-ttu-id="5f12f-1082">Argument `--cluster-name` zu allen Befehlen vom Typ `hdinsight script-action` hinzugefügt, um die alte Funktion `--name` zu ersetzen</span><span class="sxs-lookup"><span data-stu-id="5f12f-1082">Added `--cluster-name` argument to all `hdinsight script-action` commands to replace old `--name` functionality</span></span>
* <span data-ttu-id="5f12f-1083">[BREAKING CHANGE]`--script-execution-id` für alle Befehle vom Typ `hdinsight script-action` in `--execution-id` umbenannt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1083">[BREAKING CHANGE] Renamed `--script-execution-id` to `--execution-id` for all `hdinsight script-action` commands</span></span>
* <span data-ttu-id="5f12f-1084">[BREAKING CHANGE]`hdinsight script-action show` in `hdinsight script-action show-execution-details` umbenannt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1084">[BREAKING CHANGE] Renamed `hdinsight script-action show` to `hdinsight script-action show-execution-details`</span></span>
* <span data-ttu-id="5f12f-1085">[WICHTIGE ÄNDERUNG] Parameter in `hdinsight script-action execute --roles` geändert, sodass sie durch Leerzeichen anstelle von Kommas getrennt sind</span><span class="sxs-lookup"><span data-stu-id="5f12f-1085">[BREAKING CHNAGE] Changed parameters to `hdinsight script-action execute --roles` to be space-separated instead of comma-separated</span></span>
* <span data-ttu-id="5f12f-1086">[BREAKING CHANGE] Parameter `--persisted` für `hdinsight script-action list` entfernt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1086">[BREAKING CHANGE] Removed the `--persisted` parameter of `hdinsight script-action list`</span></span>
* <span data-ttu-id="5f12f-1087">Der Parameter `hdinsight create --cluster-configurations` wurde so geändert, dass er einen Pfad zu einer lokalen JSON-Datei oder JSON-Zeichenfolge akzeptiert.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1087">Changed the `hdinsight create --cluster-configurations` parameter to accept a path to a local JSON file or a JSON string</span></span>
* <span data-ttu-id="5f12f-1088">Befehl `hdinsight script-action list-execution-history` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1088">Added command `hdinsight script-action list-execution-history`</span></span>
* <span data-ttu-id="5f12f-1089">`hdinsight monitor enable --workspace` geändert, um die ID oder den Namen eines Log Analytics-Arbeitsbereichs zu akzeptieren</span><span class="sxs-lookup"><span data-stu-id="5f12f-1089">Changed `hdinsight monitor enable --workspace` to accept a Log Analytics workspace ID or workspace name</span></span>
* <span data-ttu-id="5f12f-1090">Argument `hdinsight monitor enable --primary-key` hinzugefügt. Dieses Argument wird benötigt, wenn eine Arbeitsbereichs-ID als Parameter angegeben wird.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1090">Added the `hdinsight monitor enable --primary-key` argument, which is needed if a workspace ID is provided as the parameter</span></span>
* <span data-ttu-id="5f12f-1091">Weitere Beispiele und aktualisierte Beschreibungen für Hilfemeldungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1091">Added more examples and updated descriptions for help messages</span></span>

### <a name="interactive"></a><span data-ttu-id="5f12f-1092">Interactive</span><span class="sxs-lookup"><span data-stu-id="5f12f-1092">Interactive</span></span>

* <span data-ttu-id="5f12f-1093">Ladefehler behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-1093">Fixed a loading error</span></span>

### <a name="kubernetes"></a><span data-ttu-id="5f12f-1094">Kubernetes</span><span class="sxs-lookup"><span data-stu-id="5f12f-1094">Kubernetes</span></span>

* <span data-ttu-id="5f12f-1095">Änderung, um `https` zu verwenden, wenn der Dashboardcontainerport `https` verwendet</span><span class="sxs-lookup"><span data-stu-id="5f12f-1095">Changed to use `https` if dashboard container port is using `https`</span></span>

### <a name="network"></a><span data-ttu-id="5f12f-1096">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="5f12f-1096">Network</span></span>

* <span data-ttu-id="5f12f-1097">Argument `--yes` hinzugefügt zu `network dns record-set cname delete`</span><span class="sxs-lookup"><span data-stu-id="5f12f-1097">Added `--yes` argument `network dns record-set cname delete`</span></span>

### <a name="profile"></a><span data-ttu-id="5f12f-1098">Profil</span><span class="sxs-lookup"><span data-stu-id="5f12f-1098">Profile</span></span>

* <span data-ttu-id="5f12f-1099">Argument `--resource-type` zu `account get-access-token` zum Abrufen von Ressourcenzugriffstoken hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1099">Added `--resource-type` argument to `account get-access-token` to get resource access tokens</span></span>

### <a name="servicefabric"></a><span data-ttu-id="5f12f-1100">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="5f12f-1100">ServiceFabric</span></span>

* <span data-ttu-id="5f12f-1101">Alle unterstützten Betriebssystemversionen für „sf cluster create“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1101">Added all supported os version for sf cluster create</span></span>
* <span data-ttu-id="5f12f-1102">Fehler beim Überprüfen des primären Zertifikats behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-1102">Fixed primary certificate validation bug</span></span>

### <a name="storage"></a><span data-ttu-id="5f12f-1103">Storage</span><span class="sxs-lookup"><span data-stu-id="5f12f-1103">Storage</span></span>

* <span data-ttu-id="5f12f-1104">Befehl `storage copy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1104">Added command `storage copy`</span></span>

## <a name="july-30-2019"></a><span data-ttu-id="5f12f-1105">30. Juli 2019</span><span class="sxs-lookup"><span data-stu-id="5f12f-1105">July 30, 2019</span></span>

<span data-ttu-id="5f12f-1106">Version 2.0.70</span><span class="sxs-lookup"><span data-stu-id="5f12f-1106">Version 2.0.70</span></span>

### <a name="acr"></a><span data-ttu-id="5f12f-1107">ACR</span><span class="sxs-lookup"><span data-stu-id="5f12f-1107">ACR</span></span>

* <span data-ttu-id="5f12f-1108">Problem #9952 behoben (Regression im Befehl `acr pack build`)</span><span class="sxs-lookup"><span data-stu-id="5f12f-1108">Fixed issue #9952 (a regression in the `acr pack build` command)</span></span>
* <span data-ttu-id="5f12f-1109">Standardname des Generatorimages in `acr pack build` entfernt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1109">Removed the default builder image name in `acr pack build`</span></span>

### <a name="appservice"></a><span data-ttu-id="5f12f-1110">AppService</span><span class="sxs-lookup"><span data-stu-id="5f12f-1110">Appservice</span></span>

* <span data-ttu-id="5f12f-1111">`webapp config ssl` geändert, um eine Meldung anzuzeigen, wenn eine Ressource nicht gefunden wurde</span><span class="sxs-lookup"><span data-stu-id="5f12f-1111">Changed `webapp config ssl` to show a message if a resource is not found</span></span>
* <span data-ttu-id="5f12f-1112">Problem behoben, aufgrund dessen `functionapp create` den Speicherkontotypen `Standard_RAGRS` nicht akzeptiert hat</span><span class="sxs-lookup"><span data-stu-id="5f12f-1112">Fixed issue where `functionapp create` does not accept `Standard_RAGRS` storage account type</span></span>
* <span data-ttu-id="5f12f-1113">Problem behoben, aufgrund dessen für `webapp up` ein Fehler auftrat, wenn für die Ausführung ältere Python-Versionen verwendet wurden</span><span class="sxs-lookup"><span data-stu-id="5f12f-1113">Fixed an issue where `webapp up` would fail if run using older versions of python</span></span>

### <a name="network"></a><span data-ttu-id="5f12f-1114">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="5f12f-1114">Network</span></span>

* <span data-ttu-id="5f12f-1115">Ungültiger Parameter `--ids` aus `network nic ip-config add` entfernt (Fehlerbehebungen #9861)</span><span class="sxs-lookup"><span data-stu-id="5f12f-1115">Removed invalid parameter `--ids` from `network nic ip-config add` (fixes #9861)</span></span>
* <span data-ttu-id="5f12f-1116">Fehlerbehebungen #9604.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1116">Fixes #9604.</span></span> <span data-ttu-id="5f12f-1117">Parameter `--root-certs` zu `network application-gateway http-settings [create|update]` hinzugefügt, um vom Benutzer zugewiesene vertrauenswürdige Stammzertifikate zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1117">Added `--root-certs` parameter to `network application-gateway http-settings [create|update]` to support user associate trusted root certificates.</span></span>
* <span data-ttu-id="5f12f-1118">Argument `--subscription` für `network dns record-set ns create` korrigiert (#9965)</span><span class="sxs-lookup"><span data-stu-id="5f12f-1118">Fixed arguent `--subscription` for `network dns record-set ns create` (#9965)</span></span>

### <a name="rbac"></a><span data-ttu-id="5f12f-1119">RBAC</span><span class="sxs-lookup"><span data-stu-id="5f12f-1119">RBAC</span></span>

* <span data-ttu-id="5f12f-1120">Befehl `user update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1120">Added `user update` command</span></span>
* <span data-ttu-id="5f12f-1121">[VERALTET]`--upn-or-object-id` in benutzerbezogenen Befehlen als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-1121">[DEPRECATED] Deprecated `--upn-or-object-id` from user-related commands</span></span>
    * <span data-ttu-id="5f12f-1122">Verwenden Sie das Ersatzargument `--id`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1122">Use replacement argument `--id`</span></span>
* <span data-ttu-id="5f12f-1123">Argument `--id` zu benutzerbezogenen Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1123">Added `--id` argument to user-related commands</span></span>

### <a name="sql"></a><span data-ttu-id="5f12f-1124">SQL</span><span class="sxs-lookup"><span data-stu-id="5f12f-1124">SQL</span></span>

* <span data-ttu-id="5f12f-1125">Verwaltungsbefehle für Schlüssel verwalteter Instanzen und TDE-Schutzvorrichtung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1125">Added management commands for managed instance keys and TDE protector</span></span>

### <a name="storage"></a><span data-ttu-id="5f12f-1126">Storage</span><span class="sxs-lookup"><span data-stu-id="5f12f-1126">Storage</span></span>

* <span data-ttu-id="5f12f-1127">Befehl `storage remove` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1127">Added `storage remove` command</span></span>
* <span data-ttu-id="5f12f-1128">Problem mit `storage blob update` behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-1128">Fixed an issue with `storage blob update`</span></span>

### <a name="vm"></a><span data-ttu-id="5f12f-1129">VM</span><span class="sxs-lookup"><span data-stu-id="5f12f-1129">VM</span></span>

* <span data-ttu-id="5f12f-1130">`list-skus` wurde geändert, um eine neuere API-Version für die Ausgabe von Zonendetails zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1130">Changed `list-skus` to use newer api-version to output zone details</span></span>
* <span data-ttu-id="5f12f-1131">Standardwert `--single-placement-group` für `vmss create` in `false` geändert</span><span class="sxs-lookup"><span data-stu-id="5f12f-1131">Changed default of `--single-placement-group` to `false` for `vmss create`</span></span>
* <span data-ttu-id="5f12f-1132">Möglichkeit zum Auswählen von ZRS-Speicher-SKUs für `[snapshot|disk] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1132">Added ability to select ZRS storage SKUs for `[snapshot|disk] create`</span></span>
* <span data-ttu-id="5f12f-1133">Neue Befehlsgruppe `vm host` zur Unterstützung dedizierter Hosts hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1133">Added new command group `vm host` to support dedicated hosts</span></span>
* <span data-ttu-id="5f12f-1134">Parameter `--host` und `--host-group` für `vm create` hinzugefügt, um den dedizierten VM-Host festzulegen</span><span class="sxs-lookup"><span data-stu-id="5f12f-1134">Added parameters `--host` and `--host-group` on `vm create` to set VM dedicated host</span></span>

## <a name="july-16-2019"></a><span data-ttu-id="5f12f-1135">16. Juli 2019</span><span class="sxs-lookup"><span data-stu-id="5f12f-1135">July 16, 2019</span></span>

<span data-ttu-id="5f12f-1136">Version 2.0.69</span><span class="sxs-lookup"><span data-stu-id="5f12f-1136">Version 2.0.69</span></span>

### <a name="appservice"></a><span data-ttu-id="5f12f-1137">AppService</span><span class="sxs-lookup"><span data-stu-id="5f12f-1137">Appservice</span></span>

* <span data-ttu-id="5f12f-1138">`webapp identity`-Befehle geändert, um eine korrekte Fehlermeldung zurückzugeben, wenn „ResourceGroupName“ oder der App-Name ungültig sind</span><span class="sxs-lookup"><span data-stu-id="5f12f-1138">Changed `webapp identity` commands to return a proper error message if ResourceGroupName or App name are invalid</span></span>
* <span data-ttu-id="5f12f-1139">`webapp list` korrigiert, sodass der korrekte Wert für „numberOfSites“ zurückgegeben wird, wenn „ResourceGroup“ nicht angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="5f12f-1139">Fixed `webapp list` to return the correct value for numberOfSites if no ResourceGroup was provided</span></span>
* <span data-ttu-id="5f12f-1140">Nebeneffekte von `appservice plan create` und `webapp create` behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-1140">Fixed side-effects of `appservice plan create` and `webapp create`</span></span>

### <a name="core"></a><span data-ttu-id="5f12f-1141">Core</span><span class="sxs-lookup"><span data-stu-id="5f12f-1141">Core</span></span>

* <span data-ttu-id="5f12f-1142">Problem behoben, aufgrund dessen `--subscription` angezeigt wurde, obwohl nicht anwendbar</span><span class="sxs-lookup"><span data-stu-id="5f12f-1142">Fixed issue where `--subscription` would appear despite being not applicable</span></span>

### <a name="batch"></a><span data-ttu-id="5f12f-1143">Batch</span><span class="sxs-lookup"><span data-stu-id="5f12f-1143">Batch</span></span>

* <span data-ttu-id="5f12f-1144">[BREAKING CHANGE]`batch pool node-agent-skus list` durch `batch pool supported-images list` ersetzt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1144">[BREAKING CHANGE] Replaced `batch pool node-agent-skus list` with `batch pool supported-images list`</span></span>
* <span data-ttu-id="5f12f-1145">Unterstützung für Sicherheitsregeln hinzugefügt, die den Netzwerkzugriff auf einen Pool basierend auf dem Quellport des Datenverkehrs blockieren, wenn die Option `--json-file` von `batch pool create network` verwendet wird</span><span class="sxs-lookup"><span data-stu-id="5f12f-1145">Added support for security rules blocking network access to a pool based on the source port of the traffic when using the `--json-file` option of `batch pool create network`</span></span>
* <span data-ttu-id="5f12f-1146">Unterstützung für die Ausführung der Aufgabe im Arbeitsverzeichnis des Containers oder der Batch-Aufgabe hinzugefügt, wenn die Option `--json-file` von `batch task create` verwendet wird</span><span class="sxs-lookup"><span data-stu-id="5f12f-1146">Added support for executing the task in the container working directory or in the Batch task working directory when using the `--json-file` option of `batch task create`</span></span>
* <span data-ttu-id="5f12f-1147">Fehler in Option `--application-package-references` von `batch pool create` behoben, aufgrund dessen nur Standardeinstellungen möglich waren</span><span class="sxs-lookup"><span data-stu-id="5f12f-1147">Fixed error in `--application-package-references` option of `batch pool create` where it would only work with defaults</span></span>

### <a name="eventhubs"></a><span data-ttu-id="5f12f-1148">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="5f12f-1148">Eventhubs</span></span>

* <span data-ttu-id="5f12f-1149">Validierung für Parameter `--rights` von `authorizationrule`-Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1149">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="rdbms"></a><span data-ttu-id="5f12f-1150">RDBMS</span><span class="sxs-lookup"><span data-stu-id="5f12f-1150">RDBMS</span></span>

* <span data-ttu-id="5f12f-1151">Optionaler Parameter zum Angeben der Replikat-SKU für den Befehl zum Erstellen von Replikaten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1151">Added optional parameter to specify replica SKU for create replica command</span></span>
* <span data-ttu-id="5f12f-1152">Problem mit CI-Testfehler bei der Erstellung von MySQL-Replikaten behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-1152">Fixed the issue with CI test failure with creating MySQL replica</span></span>

### <a name="relay"></a><span data-ttu-id="5f12f-1153">Relay</span><span class="sxs-lookup"><span data-stu-id="5f12f-1153">Relay</span></span>

* <span data-ttu-id="5f12f-1154">Problem mit Hybridverbindung behoben, wenn die Client-Autorisierung deaktiviert ist [#8775](https://github.com/azure/azure-cli/issues/8775)</span><span class="sxs-lookup"><span data-stu-id="5f12f-1154">Fixed issue with hybrid connection when client authroization disabled [#8775](https://github.com/azure/azure-cli/issues/8775)</span></span>
* <span data-ttu-id="5f12f-1155">Parameter `--requires-transport-security` zu `relay wcfrelay create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1155">Added parameter `--requires-transport-security` to `relay wcfrelay create`</span></span>

### <a name="servicebus"></a><span data-ttu-id="5f12f-1156">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="5f12f-1156">Servicebus</span></span>

* <span data-ttu-id="5f12f-1157">Validierung für Parameter `--rights` von `authorizationrule`-Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1157">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="storage"></a><span data-ttu-id="5f12f-1158">Storage</span><span class="sxs-lookup"><span data-stu-id="5f12f-1158">Storage</span></span>

* <span data-ttu-id="5f12f-1159">AADDS für Files für Speicherkontoaktualisierung aktiviert</span><span class="sxs-lookup"><span data-stu-id="5f12f-1159">Enable Files AADDS for storage account update</span></span>
* <span data-ttu-id="5f12f-1160">Problem `storage blob service-properties update --set` behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-1160">Fixed issue `storage blob service-properties update --set`</span></span>

## <a name="july-2-2019"></a><span data-ttu-id="5f12f-1161">2\. Juli 2019</span><span class="sxs-lookup"><span data-stu-id="5f12f-1161">July 2, 2019</span></span>

<span data-ttu-id="5f12f-1162">Version 2.0.68</span><span class="sxs-lookup"><span data-stu-id="5f12f-1162">Version 2.0.68</span></span>

### <a name="core"></a><span data-ttu-id="5f12f-1163">Core</span><span class="sxs-lookup"><span data-stu-id="5f12f-1163">Core</span></span>

* <span data-ttu-id="5f12f-1164">Befehlsmodule sind jetzt in einer einzelnen verteilbaren Python-Komponente zusammengefasst.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1164">Command modules are now consolidated into a single Python distributable.</span></span> <span data-ttu-id="5f12f-1165">Die direkte Verwendung zahlreicher Pakete vom Typ `azure-cli-` in PyPI ist daher veraltet.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1165">This deprecates direct use of many `azure-cli-` packages on PyPI.</span></span>
  <span data-ttu-id="5f12f-1166">Dadurch sollte sich die Installationsgröße reduzieren. Darüber hinaus sollte es nur Benutzer betreffen, die eine direkte Installation über `pip` ausgeführt haben.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1166">This should reduce install size and only affect users who have directly installed via `pip`.</span></span>

### <a name="acr"></a><span data-ttu-id="5f12f-1167">ACR</span><span class="sxs-lookup"><span data-stu-id="5f12f-1167">ACR</span></span>

* <span data-ttu-id="5f12f-1168">Unterstützung für Trigger mit Timer zu Aufgabe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1168">Added support for Timer Triggers to Task</span></span>

### <a name="appservice"></a><span data-ttu-id="5f12f-1169">AppService</span><span class="sxs-lookup"><span data-stu-id="5f12f-1169">Appservice</span></span>

* <span data-ttu-id="5f12f-1170">`functionapp create` wurde so geändert, das Application Insights standardmäßig aktiviert wird.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1170">Changed `functionapp create` to enable application insights by default</span></span>
* <span data-ttu-id="5f12f-1171">[BREAKING CHANGE] Veralteter Befehl `functionapp devops-build` entfernt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1171">[BREAKING CHANGE] Removed deprecated `functionapp devops-build` command.</span></span>
  *  <span data-ttu-id="5f12f-1172">Verwenden Sie stattdessen den neuen Befehl `az functionapp devops-pipeline`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1172">Use the new command `az functionapp devops-pipeline` instead</span></span>
* <span data-ttu-id="5f12f-1173">Unterstützung des Funktions-App-Plans für Linux-Verbrauch zu `functionapp deployment config-zip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1173">Added Linux Consumption function app plan support to `functionapp deployment config-zip`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="5f12f-1174">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="5f12f-1174">Cosmos DB</span></span>

* <span data-ttu-id="5f12f-1175">Unterstützung für das Deaktivieren von TTL hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1175">Added support for disabling TTL</span></span>

### <a name="dls"></a><span data-ttu-id="5f12f-1176">DLS</span><span class="sxs-lookup"><span data-stu-id="5f12f-1176">DLS</span></span>

* <span data-ttu-id="5f12f-1177">Aktualisierte ADLS-Version (0.0.45)</span><span class="sxs-lookup"><span data-stu-id="5f12f-1177">Updated ADLS version (0.0.45)</span></span>

### <a name="feedback"></a><span data-ttu-id="5f12f-1178">Feedback</span><span class="sxs-lookup"><span data-stu-id="5f12f-1178">Feedback</span></span>

* <span data-ttu-id="5f12f-1179">Wird ein fehlgeschlagener Erweiterungsbefehl gemeldet, versucht `az feedback` nun, über den Index die Projekt-/Repository-URL der Erweiterung im Browser zu öffnen.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1179">When reporting a failed extension command, `az feedback` now attempts to open the browser to the project/repo url of the extension from the index</span></span>

### <a name="hdinsight"></a><span data-ttu-id="5f12f-1180">HDInsight</span><span class="sxs-lookup"><span data-stu-id="5f12f-1180">HDInsight</span></span>

* <span data-ttu-id="5f12f-1181">[BREAKING CHANGE] Der Befehlsgruppenname `oms` wurde in `monitor` geändert.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1181">[BREAKING CHANGE] Changed `oms` command group name to `monitor`</span></span>
* <span data-ttu-id="5f12f-1182">[BREAKING CHANGE]`--http-password/-p` als erforderlicher Parameter festgelegt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1182">[BREAKING CHANGE] Made `--http-password/-p` a required parameter</span></span> 
* <span data-ttu-id="5f12f-1183">Vervollständigungen für `--cluster-admin-account` und `cluster-users-group-dns` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1183">Added completers for `--cluster-admin-account` and `cluster-users-group-dns` parameters completer</span></span> 
* <span data-ttu-id="5f12f-1184">Parameter `cluster-users-group-dns` so geändert, dass er erforderlich ist, wenn `—esp` vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="5f12f-1184">Changed `cluster-users-group-dns` parameter to be required when `—esp` is present</span></span>
* <span data-ttu-id="5f12f-1185">Timeout für alle vorhandenen automatischen Argumentvervollständigungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1185">Added a timeout for all existing argument auto-completers</span></span>
* <span data-ttu-id="5f12f-1186">Timeout für das Transformieren des Ressourcennamens in eine Ressourcen-ID hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1186">Added a timeout for transforming resource name to resource id</span></span>
* <span data-ttu-id="5f12f-1187">Die automatischen Vervollständigungen wurden so geändert, dass Ressourcen aus einer beliebigen Ressourcengruppe ausgewählt werden.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1187">Changed Auto-completers to select resources from any resource group.</span></span> <span data-ttu-id="5f12f-1188">Dabei kann es sich um eine andere Ressourcengruppe als die mit `-g` angegebene Gruppe handeln.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1188">It can be a different resource group than the one specified with `-g`</span></span>
* <span data-ttu-id="5f12f-1189">Unterstützung für die Parameter `--sub-domain-suffix` und `--disable_gateway_auth` im Befehl `hdinsight application create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1189">Added support for `--sub-domain-suffix` and `--disable_gateway_auth` parameters in the `hdinsight application create` command</span></span>

### <a name="managed-services"></a><span data-ttu-id="5f12f-1190">Verwaltete Dienste</span><span class="sxs-lookup"><span data-stu-id="5f12f-1190">Managed Services</span></span>

* <span data-ttu-id="5f12f-1191">Befehlsmodul für verwaltete Dienste als Vorschau eingeführt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1191">Introducing managed service command module in preview</span></span>

### <a name="profile"></a><span data-ttu-id="5f12f-1192">Profil</span><span class="sxs-lookup"><span data-stu-id="5f12f-1192">Profile</span></span>
* <span data-ttu-id="5f12f-1193">Argument `--subscription` für Abmeldebefehl unterdrückt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1193">Suppress `--subscription` argument for logout command</span></span>

### <a name="rbac"></a><span data-ttu-id="5f12f-1194">RBAC</span><span class="sxs-lookup"><span data-stu-id="5f12f-1194">RBAC</span></span>

* <span data-ttu-id="5f12f-1195">[BREAKING CHANGE] Argument `--password` für `create-for-rbac` entfernt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1195">[BREAKING CHANGE] Removed `--password` argument for `create-for-rbac`</span></span>
* <span data-ttu-id="5f12f-1196">Parameter `--assignee-principal-type` zum Befehl `create` hinzugefügt, um zeitweilige Fehler zu vermeiden, die durch die Replikationswartezeit des AAD-Graph-Servers verursacht werden</span><span class="sxs-lookup"><span data-stu-id="5f12f-1196">Added `--assignee-principal-type` parameter to `create` command to avoid intermittent failures caused by AAD graph server replication latency</span></span>
* <span data-ttu-id="5f12f-1197">Absturz in `ad signed-in-user` beim Auflisten von in Besitz befindlichen Objekten behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-1197">Fixed a crash in `ad signed-in-user` when listing owned objects</span></span>
* <span data-ttu-id="5f12f-1198">Problem behoben, aufgrund dessen `ad sp` nicht die richtige Anwendung über einen Dienstprinzipal fand</span><span class="sxs-lookup"><span data-stu-id="5f12f-1198">Fixed issue where `ad sp` would not find the right application from a service principal</span></span>

### <a name="rdbms"></a><span data-ttu-id="5f12f-1199">RDBMS</span><span class="sxs-lookup"><span data-stu-id="5f12f-1199">RDBMS</span></span>

* <span data-ttu-id="5f12f-1200">Unterstützung für die Replikation für MariaDB hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1200">Added support for replication for MariaDB</span></span>

### <a name="sql"></a><span data-ttu-id="5f12f-1201">SQL</span><span class="sxs-lookup"><span data-stu-id="5f12f-1201">SQL</span></span>

* <span data-ttu-id="5f12f-1202">Zulässige Werte für `sql db create --sample-name` dokumentiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-1202">Documented allowed values for `sql db create --sample-name`</span></span>

### <a name="storage"></a><span data-ttu-id="5f12f-1203">Storage</span><span class="sxs-lookup"><span data-stu-id="5f12f-1203">Storage</span></span>

* <span data-ttu-id="5f12f-1204">Unterstützung von SAS-Token für die Benutzerdelegierung mit `--as-user` zu `storage blob generate-sas` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1204">Added user delegation SAS token support with `--as-user` to `storage blob generate-sas`</span></span> 
* <span data-ttu-id="5f12f-1205">Unterstützung von SAS-Token für die Benutzerdelegierung mit `--as-user` zu `storage container generate-sas` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1205">Added user delegation SAS token support with `--as-user` to `storage container generate-sas`</span></span> 

### <a name="vm"></a><span data-ttu-id="5f12f-1206">VM</span><span class="sxs-lookup"><span data-stu-id="5f12f-1206">VM</span></span>

* <span data-ttu-id="5f12f-1207">Fehler behoben, aufgrund dessen `vmss create` bei der Ausführung mit `--no-wait` eine Fehlermeldung zurückgab</span><span class="sxs-lookup"><span data-stu-id="5f12f-1207">Fixed bug where `vmss create` returns an error message when run with `--no-wait`</span></span>
* <span data-ttu-id="5f12f-1208">Die clientseitige Validierung für `vmss create --single-placement-group` wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1208">Removed client-side validation for `vmss create --single-placement-group`.</span></span> <span data-ttu-id="5f12f-1209">Es tritt kein Fehler auf, wenn `--single-placement-group` auf `true` und für `--instance-count` ein größerer Wert als 100 festgelegt wird oder wenn Verfügbarkeitszonen angegeben werden. Diese Validierung wird jedoch dem Computedienst überlassen.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1209">Does not fail if `--single-placement-group` is set to `true` and`--instance-count` is greater than 100 or availability zones are specified, but leaves this validation to the compute service</span></span>
* <span data-ttu-id="5f12f-1210">Problem behoben, aufgrund dessen bei der Verwendung von `--latest` für `[vm|vmss] extension image list` ein Fehler auftrat</span><span class="sxs-lookup"><span data-stu-id="5f12f-1210">Fixed bug where `[vm|vmss] extension image list` fails when used with `--latest`</span></span>


## <a name="june-18-2019"></a><span data-ttu-id="5f12f-1211">18. Juni 2019</span><span class="sxs-lookup"><span data-stu-id="5f12f-1211">June 18, 2019</span></span>

<span data-ttu-id="5f12f-1212">Version 2.0.67</span><span class="sxs-lookup"><span data-stu-id="5f12f-1212">Version 2.0.67</span></span>

### <a name="core"></a><span data-ttu-id="5f12f-1213">Core</span><span class="sxs-lookup"><span data-stu-id="5f12f-1213">Core</span></span>

<span data-ttu-id="5f12f-1214">In diesem Release wird das neue [Preview]-Tag eingeführt, um Kunden gegenüber deutlich zu machen, dass sich eine Befehlsgruppe, ein Befehl oder ein Argument in der Vorschauphase befindet.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1214">This release introduces a new [Preview] tag to more clearly communicate to customers when a command group, command or argument is in preview status.</span></span> <span data-ttu-id="5f12f-1215">Diese Information war zuvor im Hilfetext oder implizit durch die Versionsnummer des Befehlsmoduls angegeben.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1215">This was previously called out in help text or communicated implicitly by the command module version number.</span></span>
<span data-ttu-id="5f12f-1216">Die Befehlszeilenschnittstelle wird künftig Versionsnummern für einzelne Pakete entfernen.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1216">The CLI will be removing version numbers for individual packages in the future.</span></span> <span data-ttu-id="5f12f-1217">Wenn sich ein Befehl in der Vorschauphase befindet, gilt dies auch für alle seine Argumente.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1217">If a command is in preview, all of its arguments are as well.</span></span> <span data-ttu-id="5f12f-1218">Wenn eine Befehlsgruppe als Vorschau gekennzeichnet ist, befinden sich auch alle Befehle und Argumente in der Vorschauphase.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1218">If a command group is labeled as being in preview, then all commands and arguments are considered to be in preview as well.</span></span>

<span data-ttu-id="5f12f-1219">Infolge dieser Änderung befinden sich in diesem Release verschiedene Befehlsgruppen anscheinend „plötzlich“ in der Vorschauphase.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1219">As a result of this change, several command groups may seem to "suddenly" appear to be in a preview status with this release.</span></span> <span data-ttu-id="5f12f-1220">Tatsächlich ist es jedoch so, dass sich die meisten Pakete in der Vorschauphase befanden, in diesem Release jedoch als allgemein verfügbar gelten.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1220">What actually happened is that most packages were in a preview status, but are being deemed GA with this release</span></span>

### <a name="acr"></a><span data-ttu-id="5f12f-1221">ACR</span><span class="sxs-lookup"><span data-stu-id="5f12f-1221">ACR</span></span>
* <span data-ttu-id="5f12f-1222">Befehl „acr check-health“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1222">Added 'acr check-health' command</span></span>
* <span data-ttu-id="5f12f-1223">Verbesserte Fehlerbehandlung für AAD-Token und für das Abrufen externer Befehle</span><span class="sxs-lookup"><span data-stu-id="5f12f-1223">Improved error handling for AAD tokens and for retrieving external commands</span></span>

### <a name="acs"></a><span data-ttu-id="5f12f-1224">ACS</span><span class="sxs-lookup"><span data-stu-id="5f12f-1224">ACS</span></span>
* <span data-ttu-id="5f12f-1225">Veraltete ACS-Befehle werden jetzt in der Hilfeansicht ausgeblendet.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1225">Deprecated ACS commands are now hidden from help view</span></span>

### <a name="ams"></a><span data-ttu-id="5f12f-1226">AMS</span><span class="sxs-lookup"><span data-stu-id="5f12f-1226">AMS</span></span>
* <span data-ttu-id="5f12f-1227">[BREAKING CHANGE] Änderung, damit ISO 8601-Zeitzeichenfolgen für „archive-window-length“ und „key-frame-interval-duration“ zurückgegeben werden</span><span class="sxs-lookup"><span data-stu-id="5f12f-1227">[BREAKING CHANGE] Changed to return ISO 8601 time strings for archive-window-length and key-frame-interval-duration</span></span>

### <a name="appservice"></a><span data-ttu-id="5f12f-1228">AppService</span><span class="sxs-lookup"><span data-stu-id="5f12f-1228">AppService</span></span>
* <span data-ttu-id="5f12f-1229">Standortbasiertes Routing für `webapp deleted list` und `webapp deleted restore` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1229">Added location based routing for `webapp deleted list` and `webapp deleted restore`</span></span>
* <span data-ttu-id="5f12f-1230">Problem behoben, aufgrund dessen in Azure Cloud Shell nicht auf die von einer Web-App protokollierte Ziel-URL („Sie können die App starten unter...“) geklickt werden konnte</span><span class="sxs-lookup"><span data-stu-id="5f12f-1230">Fixed issue where webapp up logged target URL ("You can launch the app at...") was not clickable in Azure Cloud Shell</span></span>
* <span data-ttu-id="5f12f-1231">Problem behoben, aufgrund dessen beim Erstellen von Apps bei einigen SKUs ein AlwaysOn-Fehler auftrat</span><span class="sxs-lookup"><span data-stu-id="5f12f-1231">Fixed an issue where creating apps with the some SKUs was failing with an AlwaysOn error</span></span>
* <span data-ttu-id="5f12f-1232">Vorabüberprüfung zu `[appservice|webapp] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1232">Added pre-validation to `[appservice|webapp] create`</span></span>
* <span data-ttu-id="5f12f-1233">`[webapp|functionapp] traffic-routing` korrigiert, damit der richtige actionHostName-Wert verwendet wird</span><span class="sxs-lookup"><span data-stu-id="5f12f-1233">Fixed `[webapp|functionapp] traffic-routing` to use the correct actionHostName</span></span>
* <span data-ttu-id="5f12f-1234">Slotunterstützung zu `functionapp`-Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1234">Added slot support to `functionapp` commands</span></span>

### <a name="batch"></a><span data-ttu-id="5f12f-1235">Batch</span><span class="sxs-lookup"><span data-stu-id="5f12f-1235">Batch</span></span>
* <span data-ttu-id="5f12f-1236">AAD-Authentifizierungsregression korrigiert, die von übermäßiger Berichterstellung für Authentifizierung mit gemeinsam verwendetem Schlüssel verursacht wurde</span><span class="sxs-lookup"><span data-stu-id="5f12f-1236">Fixed AAD auth regression caused by over-aggressive error reporting for Shared Key Auth</span></span>

### <a name="batchai"></a><span data-ttu-id="5f12f-1237">Batch AI</span><span class="sxs-lookup"><span data-stu-id="5f12f-1237">BatchAI</span></span>
* <span data-ttu-id="5f12f-1238">BatchAI-Befehle sind jetzt veraltet und ausgeblendet.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1238">BatchAI commands are now deprecated and hidden</span></span>

### <a name="botservice"></a><span data-ttu-id="5f12f-1239">BotService</span><span class="sxs-lookup"><span data-stu-id="5f12f-1239">BotService</span></span>
* <span data-ttu-id="5f12f-1240">Für Befehle, die Version 3 des SDK unterstützen, wurden die Warnmeldungen „Support eingestellt“/„Wartungsmodus“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1240">Added "discontinued support"/"maintenance mode" warning messages for commands that support the v3 SDK</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="5f12f-1241">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="5f12f-1241">CosmosDB</span></span>
* <span data-ttu-id="5f12f-1242">[VERALTET] Der Befehl `cosmosdb list-keys` wurde als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1242">[DEPRECATED] Deprecated the `cosmosdb list-keys` command</span></span>
* <span data-ttu-id="5f12f-1243">Befehl `cosmosdb keys list` hinzugefügt, er ersetzt `cosmosdb list-keys`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1243">Added the `cosmosdb keys list` command - replaces `cosmosdb list-keys`</span></span>
* <span data-ttu-id="5f12f-1244">`cosmsodb create/update`: Neues Format für „--location“ hinzugefügt, um das Festlegen der Eigenschaft „isZoneRedundant“ zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="5f12f-1244">`cosmsodb create/update`: Added new format for --location to allow setting "isZoneRedundant" property.</span></span> <span data-ttu-id="5f12f-1245">Das alte Format wurde als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1245">Deprecated old format</span></span>

### <a name="eventgrid"></a><span data-ttu-id="5f12f-1246">EventGrid</span><span class="sxs-lookup"><span data-stu-id="5f12f-1246">EventGrid</span></span>
* <span data-ttu-id="5f12f-1247">`eventgrid domain`-Befehle für CRUD-Vorgänge für Domänen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1247">Added `eventgrid domain` commands for domain CRUD operations</span></span>
* <span data-ttu-id="5f12f-1248">`eventgrid domain topic`-Befehle für CRUD-Vorgänge für Domänenthemen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1248">Added `eventgrid domain topic` commands for domain topics CRUD operations</span></span>
* <span data-ttu-id="5f12f-1249">Argument `--odata-query` zu `eventgrid [topic|event-subscription] list` zum Filtern der Ergebnisse mithilfe von OData-Syntax hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1249">Added `--odata-query` argument to `eventgrid [topic|event-subscription] list` for filtering results using OData syntax</span></span>
* <span data-ttu-id="5f12f-1250">`event-subscription create/update`: „servicebusqueue“ als neue Werte für den Parameter `--endpoint-type` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1250">`event-subscription create/update`: Added servicebusqueue as new values for the `--endpoint-type` parameter</span></span>
* <span data-ttu-id="5f12f-1251">[BREAKING CHANGE] Unterstützung für `--included-event-types All` mit `eventgrid event-subscription [create|update]` entfernt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1251">[BREAKING CHANGE] Removed support for `--included-event-types All` with `eventgrid event-subscription [create|update]`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="5f12f-1252">HDInsight</span><span class="sxs-lookup"><span data-stu-id="5f12f-1252">HDInsight</span></span>
* <span data-ttu-id="5f12f-1253">Unterstützung für den Parameter `--ssh-public-key` im Befehl vom Typ `hdinsight create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1253">Added support for `--ssh-public-key` parameter in `hdinsight create` command</span></span>

### <a name="iot"></a><span data-ttu-id="5f12f-1254">IoT</span><span class="sxs-lookup"><span data-stu-id="5f12f-1254">IoT</span></span>
* <span data-ttu-id="5f12f-1255">Unterstützung für das erneute Generieren von Autorisierungsrichtlinienschlüsseln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1255">Added support to regenerate authorization policy keys</span></span>
* <span data-ttu-id="5f12f-1256">SDK und Unterstützung für den Bereitstellungsdienst des DigitalTwin-Repositorys hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1256">Added SDK and support for DigitalTwin Repository Provisioning Service</span></span>

### <a name="network"></a><span data-ttu-id="5f12f-1257">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="5f12f-1257">Network</span></span>
* <span data-ttu-id="5f12f-1258">Zonenunterstützung für NAT Gateway hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1258">Added Zone support for Nat Gateway</span></span>
* <span data-ttu-id="5f12f-1259">Befehl `network list-service-tags` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1259">Added command `network list-service-tags`</span></span>
* <span data-ttu-id="5f12f-1260">Problem mit `dns zone import` behoben, aufgrund dessen Benutzer keine A-Platzhaltereinträge importieren konnten</span><span class="sxs-lookup"><span data-stu-id="5f12f-1260">Fixed issue with `dns zone import` where users could not import wildcard A records</span></span>
* <span data-ttu-id="5f12f-1261">Problem mit `watcher flow-log configure` behoben, aufgrund dessen die Flowprotokollierung in bestimmten Regionen nicht aktiviert werden konnte</span><span class="sxs-lookup"><span data-stu-id="5f12f-1261">Fixed issue with `watcher flow-log configure` where flow logging could not be enabled in certain regions</span></span>

### <a name="resource"></a><span data-ttu-id="5f12f-1262">Resource</span><span class="sxs-lookup"><span data-stu-id="5f12f-1262">Resource</span></span>
* <span data-ttu-id="5f12f-1263">Befehl `az rest` zum Ausführen von REST-Aufrufen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1263">Added `az rest` command for making REST calls</span></span>
* <span data-ttu-id="5f12f-1264">Fehler behoben, der bei Verwendung von `policy assignment list` mit `--scope` auf Ressourcengruppen- oder Abonnementebene auftrat</span><span class="sxs-lookup"><span data-stu-id="5f12f-1264">Fixed error when using `policy assignment list` with a resource group or subscription level `--scope`</span></span>

### <a name="servicebus"></a><span data-ttu-id="5f12f-1265">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="5f12f-1265">ServiceBus</span></span>
* <span data-ttu-id="5f12f-1266">Problem mit `servicebus topic create --max-size` behoben [Nr. 9319](https://github.com/azure/azure-cli/issues/9319)</span><span class="sxs-lookup"><span data-stu-id="5f12f-1266">Fixed issue with `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span></span>

### <a name="sql"></a><span data-ttu-id="5f12f-1267">SQL</span><span class="sxs-lookup"><span data-stu-id="5f12f-1267">SQL</span></span>
* <span data-ttu-id="5f12f-1268">`--location` wurde geändert und ist nun für `sql [server|mi] create` optional. Ohne Angabe wird der Ressourcengruppenstandort verwendet.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1268">Changed `--location` to be optional for `sql [server|mi] create` - uses resource group location if not specified</span></span>
* <span data-ttu-id="5f12f-1269">Der Fehler, dass das Objekt „NoneType“ nicht wiederholbar ist, wurde für `sql db list-editions --available` behoben.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1269">Fixed "'NoneType' object is not iterable" error for `sql db list-editions --available`</span></span>

### <a name="sqlvm"></a><span data-ttu-id="5f12f-1270">SQLVm</span><span class="sxs-lookup"><span data-stu-id="5f12f-1270">SQLVm</span></span>
* <span data-ttu-id="5f12f-1271">[WICHTIGE ÄNDERUNG] `sql vm create` wurde geändert und erfordert nun den Parameter `--license-type`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1271">[BREAKING CHNAGE] Changed `sql vm create` to require `--license-type` parameter</span></span>
* <span data-ttu-id="5f12f-1272">Änderung, um beim Erstellen oder Aktualisieren einer SQL-VM das Festlegen der SQL-Image-SKU zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="5f12f-1272">Changed to allow setting SQL image SKU when creating or updating a sql vm</span></span>

### <a name="storage"></a><span data-ttu-id="5f12f-1273">Storage</span><span class="sxs-lookup"><span data-stu-id="5f12f-1273">Storage</span></span>
* <span data-ttu-id="5f12f-1274">Problem mit fehlendem Kontoschlüssel für `storage container generate-sas` behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-1274">Fixed issue with missing account key for `storage container generate-sas`</span></span>
* <span data-ttu-id="5f12f-1275">Problem mit `storage blob sync` unter Linux behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-1275">Fixed issue with `storage blob sync` on Linux</span></span>

### <a name="vm"></a><span data-ttu-id="5f12f-1276">VM</span><span class="sxs-lookup"><span data-stu-id="5f12f-1276">VM</span></span>
* <span data-ttu-id="5f12f-1277">[VORSCHAU] Befehle vom Typ `vm image template` zum Erstellen von VM-Images hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1277">[PREVIEW] Added `vm image template` commands to build VM images</span></span>

## <a name="june-4-2019"></a><span data-ttu-id="5f12f-1278">4\. Juni 2019</span><span class="sxs-lookup"><span data-stu-id="5f12f-1278">June 4, 2019</span></span>

<span data-ttu-id="5f12f-1279">Version 2.0.66</span><span class="sxs-lookup"><span data-stu-id="5f12f-1279">Version 2.0.66</span></span>

### <a name="core"></a><span data-ttu-id="5f12f-1280">Core</span><span class="sxs-lookup"><span data-stu-id="5f12f-1280">Core</span></span>
* <span data-ttu-id="5f12f-1281">Fehler behoben, aufgrund dessen bei Befehlen ein Fehler auftrat, wenn `--output yaml` mit `--query` verwendet wurde</span><span class="sxs-lookup"><span data-stu-id="5f12f-1281">Fixed bug where commands fail if `--output yaml` is used with `--query`</span></span>

### <a name="acr"></a><span data-ttu-id="5f12f-1282">ACR</span><span class="sxs-lookup"><span data-stu-id="5f12f-1282">ACR</span></span>
* <span data-ttu-id="5f12f-1283">Befehlsgruppe „acr pack“ zum Erstellen von Aufgaben zur Schnellerstellung mit Buildpacks hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1283">Added 'acr pack' command group for creating quick build Tasks using Buildpacks.</span></span>

### <a name="acs"></a><span data-ttu-id="5f12f-1284">ACS</span><span class="sxs-lookup"><span data-stu-id="5f12f-1284">ACS</span></span>
* <span data-ttu-id="5f12f-1285">Zulassen der Aktivierung/Deaktivierung des AKS-Add-Ons für das Kube-Dashboard</span><span class="sxs-lookup"><span data-stu-id="5f12f-1285">Allow enabling/disabling AKS kube-dashboard addon</span></span>
* <span data-ttu-id="5f12f-1286">Ausgeben einer benutzerfreundlichen Nachricht, wenn das Abonnement nicht in der Whitelist zur Verwendung von Azure Red Hat OpenShift enthalten ist</span><span class="sxs-lookup"><span data-stu-id="5f12f-1286">Print a friendly message when the subscription is not whitelisted to use Azure Red Hat OpenShift</span></span>

### <a name="batch"></a><span data-ttu-id="5f12f-1287">Batch</span><span class="sxs-lookup"><span data-stu-id="5f12f-1287">Batch</span></span>
* <span data-ttu-id="5f12f-1288">Bessere Fehlerbehandlung, wenn der Benutzer nicht bei einem Konto angemeldet ist \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span><span class="sxs-lookup"><span data-stu-id="5f12f-1288">Improved error handling when not logged in to an account \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span></span>

### <a name="iot"></a><span data-ttu-id="5f12f-1289">IoT</span><span class="sxs-lookup"><span data-stu-id="5f12f-1289">IoT</span></span>
* <span data-ttu-id="5f12f-1290">Unterstützung für manuelles Failover hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1290">Added support for manual failover</span></span>

### <a name="network"></a><span data-ttu-id="5f12f-1291">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="5f12f-1291">Network</span></span>
* <span data-ttu-id="5f12f-1292">Befehle vom Typ `network application-gateway waf-policy` hinzugefügt, um benutzerdefinierte WAF-Regeln zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="5f12f-1292">Added `network application-gateway waf-policy` commands to support custom WAF rules.</span></span>
* <span data-ttu-id="5f12f-1293">Argumente `--waf-policy` und `--max-capacity` zu `network application-gateway [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1293">Added `--waf-policy` and `--max-capacity` arguments to `network application-gateway [create|update]`</span></span> 

### <a name="resource"></a><span data-ttu-id="5f12f-1294">Resource</span><span class="sxs-lookup"><span data-stu-id="5f12f-1294">Resource</span></span>
* <span data-ttu-id="5f12f-1295">Verbesserte Fehlermeldungen aus `deployment create`, wenn TTY nicht verfügbar ist</span><span class="sxs-lookup"><span data-stu-id="5f12f-1295">Improved error message from `deployment create` when there is no TTY available</span></span>

### <a name="role"></a><span data-ttu-id="5f12f-1296">Role</span><span class="sxs-lookup"><span data-stu-id="5f12f-1296">Role</span></span>
* <span data-ttu-id="5f12f-1297">Hilfetext aktualisiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-1297">Updated help text.</span></span>

### <a name="compute"></a><span data-ttu-id="5f12f-1298">Compute</span><span class="sxs-lookup"><span data-stu-id="5f12f-1298">Compute</span></span>
* <span data-ttu-id="5f12f-1299">Unterstützung zu `vm create` für virtuelle Computer aus einem verwalteten Image mit Datenträger-LUNs hinzugefügt, die nicht bei 0 beginnen oder die Nummern überspringen</span><span class="sxs-lookup"><span data-stu-id="5f12f-1299">Added support to `vm create` for VMs from a managed image with data-disk luns that do not start from 0 or that skip numbers</span></span>

## <a name="may-21-2019"></a><span data-ttu-id="5f12f-1300">21. Mai 2019</span><span class="sxs-lookup"><span data-stu-id="5f12f-1300">May 21, 2019</span></span>

<span data-ttu-id="5f12f-1301">Version 2.0.65</span><span class="sxs-lookup"><span data-stu-id="5f12f-1301">Version 2.0.65</span></span>

### <a name="core"></a><span data-ttu-id="5f12f-1302">Core</span><span class="sxs-lookup"><span data-stu-id="5f12f-1302">Core</span></span>
* <span data-ttu-id="5f12f-1303">Besseres Feedback für Authentifizierungsfehler hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1303">Added better feedback for authentication errors</span></span>
* <span data-ttu-id="5f12f-1304">Problem behoben, aufgrund dessen die CLI Erweiterungen lädt, die nicht mit der Core-Version kompatibel waren</span><span class="sxs-lookup"><span data-stu-id="5f12f-1304">Fixed issue where the CLI would load extensions that were not compatible with its core version</span></span>
* <span data-ttu-id="5f12f-1305">Problem beim Starten behoben, wenn `clouds.config` beschädigt ist</span><span class="sxs-lookup"><span data-stu-id="5f12f-1305">Fixed issue with launching when `clouds.config` is corrupted</span></span>

### <a name="acr"></a><span data-ttu-id="5f12f-1306">ACR</span><span class="sxs-lookup"><span data-stu-id="5f12f-1306">ACR</span></span>
* <span data-ttu-id="5f12f-1307">Unterstützung für verwaltete Identitäten zu Aufgaben hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1307">Added support for Managed Identities to Tasks</span></span>

### <a name="acs"></a><span data-ttu-id="5f12f-1308">ACS</span><span class="sxs-lookup"><span data-stu-id="5f12f-1308">ACS</span></span>
* <span data-ttu-id="5f12f-1309">`openshift create`-Befehl bei der Verwendung mit dem AAD-Kundenclient korrigiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-1309">Fixed `openshift create` command when used with customer AAD client</span></span>

### <a name="appservice"></a><span data-ttu-id="5f12f-1310">AppService</span><span class="sxs-lookup"><span data-stu-id="5f12f-1310">AppService</span></span>
* <span data-ttu-id="5f12f-1311">[VERALTET] Befehl `functionapp devops-build` als veraltet gekennzeichnet – wird in der nächsten Version entfernt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1311">[DEPRECATED] Deprecated `functionapp devops-build` command - will be removed in next release</span></span>
* <span data-ttu-id="5f12f-1312">`functionapp devops-pipeline` geändert, um das Buildprotokoll von Azure DevOps im ausführlichen Modus abzurufen</span><span class="sxs-lookup"><span data-stu-id="5f12f-1312">Changed `functionapp devops-pipeline` to fetch build log from Azure DevOps in verbose mode</span></span>
* <span data-ttu-id="5f12f-1313">[BREAKING CHANGE] Flag `--use_local_settings` aus dem Befehl `functionapp devops-pipeline` entfernt – kein Vorgang wurde ausgeführt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1313">[BREAKING CHANGE] Removed `--use_local_settings` flag from `functionapp devops-pipeline` command - was a no-op</span></span>
* <span data-ttu-id="5f12f-1314">`webapp up` geändert, sodass die JSON-Ausgabe zurückgegeben wird, wenn `--logs` nicht verwendet wird</span><span class="sxs-lookup"><span data-stu-id="5f12f-1314">Changed `webapp up` to return JSON output if `--logs` is not used</span></span>
* <span data-ttu-id="5f12f-1315">Unterstützung hinzugefügt zum Schreiben von Standardressourcen in die lokale Konfiguration für `webapp up`</span><span class="sxs-lookup"><span data-stu-id="5f12f-1315">Added support for writing default resources to local config for `webapp up`</span></span>
* <span data-ttu-id="5f12f-1316">Unterstützung zu `webapp up` hinzugefügt für die erneute Bereitstellung einer App ohne Verwendung des `--location`-Arguments</span><span class="sxs-lookup"><span data-stu-id="5f12f-1316">Added support to `webapp up` for redeploying an app without using the `--location` argument</span></span>
* <span data-ttu-id="5f12f-1317">Problem behoben, bei dem für die ASP-Erstellung der Linux-SKU „Free“ der SKU-Wert „Free“ nicht funktioniert hat</span><span class="sxs-lookup"><span data-stu-id="5f12f-1317">Fixed an issue where for Linux Free SKU ASP creation use Free as SKU value was not working</span></span>

### <a name="botservice"></a><span data-ttu-id="5f12f-1318">BotService</span><span class="sxs-lookup"><span data-stu-id="5f12f-1318">BotService</span></span>
* <span data-ttu-id="5f12f-1319">Geändert, sodass Groß-/Kleinschreibung für `--lang`-Parameter für Befehle zulässig ist</span><span class="sxs-lookup"><span data-stu-id="5f12f-1319">Changed to allow all casing for `--lang` parameters for commands</span></span>
* <span data-ttu-id="5f12f-1320">Beschreibung für das Befehlsmodul aktualisiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-1320">Updated description for command module</span></span>

### <a name="consumption"></a><span data-ttu-id="5f12f-1321">Nutzung</span><span class="sxs-lookup"><span data-stu-id="5f12f-1321">Consumption</span></span>
* <span data-ttu-id="5f12f-1322">Fehlende erforderliche Parameter bei der Ausführung von `consumption usage list --billing-period-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1322">Added missing required parameter when running `consumption usage list --billing-period-name`</span></span>

### <a name="iot"></a><span data-ttu-id="5f12f-1323">IoT</span><span class="sxs-lookup"><span data-stu-id="5f12f-1323">IoT</span></span>
* <span data-ttu-id="5f12f-1324">Unterstützung für das Auflisten aller Schlüssel hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1324">Added support to list all keys</span></span>

### <a name="network"></a><span data-ttu-id="5f12f-1325">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="5f12f-1325">Network</span></span>
* [BREAKING CHANGE]: Removed `network interface-endpoints` command group - use `network private-endpoints` 
* <span data-ttu-id="5f12f-1327">`--nat-gateway`-Argument zu `network vnet subnet [create|update]` für das Anfügen an ein NAT-Gateway hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1327">Added `--nat-gateway` argument to `network vnet subnet [create|update]` for attaching to a NAT gateway</span></span>
* <span data-ttu-id="5f12f-1328">Problem mit `dns zone import` behoben, aufgrund dessen Eintragsnamen keinem Datensatztyp entsprochen haben</span><span class="sxs-lookup"><span data-stu-id="5f12f-1328">Fixed issue with `dns zone import` where record names could not match a record type</span></span>

### <a name="rdbms"></a><span data-ttu-id="5f12f-1329">RDBMS</span><span class="sxs-lookup"><span data-stu-id="5f12f-1329">RDBMS</span></span>
* <span data-ttu-id="5f12f-1330">Postgres- und MySLQ-Unterstützung für die Georeplikation hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1330">Added postgres and mysql support for geo replication</span></span>

### <a name="rbac"></a><span data-ttu-id="5f12f-1331">RBAC</span><span class="sxs-lookup"><span data-stu-id="5f12f-1331">RBAC</span></span>
* <span data-ttu-id="5f12f-1332">Unterstützung für den Verwaltungsgruppenumfang zu `role assignment` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1332">Added support for management group scope to `role assignment`</span></span>

### <a name="storage"></a><span data-ttu-id="5f12f-1333">Storage</span><span class="sxs-lookup"><span data-stu-id="5f12f-1333">Storage</span></span>
* <span data-ttu-id="5f12f-1334">`storage blob sync`: Synchronisierungsbefehl für Speicherblob hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1334">`storage blob sync`: add sync command for storage blob</span></span>

### <a name="compute"></a><span data-ttu-id="5f12f-1335">Compute</span><span class="sxs-lookup"><span data-stu-id="5f12f-1335">Compute</span></span>
* <span data-ttu-id="5f12f-1336">`--computer-name` zu `vm create` zum Festlegen des Computernamens eines virtuellen Computers hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1336">Added `--computer-name` to `vm create` for setting a VM's computer name</span></span>
* <span data-ttu-id="5f12f-1337">`--ssh-key-value` umbenannt in `--ssh-key-values` für `[vm|vmss] create`: Jetzt können mehrere öffentliche SSH-Schlüsselwerte oder -pfade akzeptiert werden.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1337">Renamed `--ssh-key-value` renamed to `--ssh-key-values` for `[vm|vmss] create` - can now accept multiple ssh public key values or paths</span></span>
  * <span data-ttu-id="5f12f-1338">__Hinweis__: Dies ist **kein** Breaking Change: `--ssh-key-value` wird korrekt analysiert, da nur eine Übereinstimmung mit `--ssh-key-values` besteht.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1338">__Note__: This is **not** a breaking change - `--ssh-key-value` will be parsed correctly as it matches only `--ssh-key-values`</span></span>
* <span data-ttu-id="5f12f-1339">`--type`-Argument von `ppg create` in optionales Argument geändert</span><span class="sxs-lookup"><span data-stu-id="5f12f-1339">Changed the `--type` argument of `ppg create` to be optional</span></span>

## <a name="may-6-2019"></a><span data-ttu-id="5f12f-1340">6\. Mai 2019</span><span class="sxs-lookup"><span data-stu-id="5f12f-1340">May 6, 2019</span></span>

<span data-ttu-id="5f12f-1341">Version 2.0.64</span><span class="sxs-lookup"><span data-stu-id="5f12f-1341">Version 2.0.64</span></span>

### <a name="acs"></a><span data-ttu-id="5f12f-1342">ACS</span><span class="sxs-lookup"><span data-stu-id="5f12f-1342">ACS</span></span>
* <span data-ttu-id="5f12f-1343">[BREAKING CHANGE] Flag `--fqdn` aus den `openshift`-Befehlen entfernt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1343">[BREAKING CHANGE] Removed `--fqdn` flag on `openshift` commands</span></span>
* <span data-ttu-id="5f12f-1344">Geändert, sodass die allgemein verfügbare Azure Red Hat Openshift-API-Version verwendet wird</span><span class="sxs-lookup"><span data-stu-id="5f12f-1344">Changed to use Azure Red Hat Openshift GA API Version</span></span>
* <span data-ttu-id="5f12f-1345">Flag `customer-admin-group-id` wurde zu `openshift create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1345">Added `customer-admin-group-id` flag to `openshift create`</span></span>
* <span data-ttu-id="5f12f-1346">[ALLGEMEIN VERFÜGBAR] `(PREVIEW)` aus der `aks create`-Option `--network-policy` entfernt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1346">[GA] Removed `(PREVIEW)` from `aks create` option `--network-policy`</span></span>

### <a name="appservice"></a><span data-ttu-id="5f12f-1347">AppService</span><span class="sxs-lookup"><span data-stu-id="5f12f-1347">Appservice</span></span>
* <span data-ttu-id="5f12f-1348">[VERALTET] Befehl `functionapp devops-build` als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="5f12f-1348">[DEPRECATED] Deprecated `functionapp devops-build` command</span></span>
  * <span data-ttu-id="5f12f-1349">Umbenannt in `functionapp devops-pipeline`</span><span class="sxs-lookup"><span data-stu-id="5f12f-1349">Renamed to `functionapp devops-pipeline`</span></span>
* <span data-ttu-id="5f12f-1350">Fehler beim Abrufen des richtigen Benutzernamens für Cloud Shell behoben, der einen Fehler von `webapp up` verursachte</span><span class="sxs-lookup"><span data-stu-id="5f12f-1350">Fixed getting the correct username for cloudshell which was causing `webapp up` to fail</span></span>
* <span data-ttu-id="5f12f-1351">Dokumentation von `appservice plan --sku` mit den unterstützten App Service-Plänen aktualisiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-1351">Updated `appservice plan --sku` documentation updated to reflect the supported appserviceplans</span></span>
* <span data-ttu-id="5f12f-1352">Optionale Argumente für Ressourcengruppe und Plan zu `webapp up` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1352">Added optional arguments for resource group and plan to `webapp up`</span></span>
* <span data-ttu-id="5f12f-1353">Unterstützung zur Berücksichtigung der Umgebungsvariablen `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` zu `webapp ssh` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1353">Added support to `webapp ssh` to respect `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>
* <span data-ttu-id="5f12f-1354">Unterstützung für `appserviceplan create` für die kostenlose Linux-SKU hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1354">Added `appserviceplan create` support for Linux Free SKU</span></span>
* <span data-ttu-id="5f12f-1355">`webapp up` geändert, um nach dem Festlegen der App-Einstellung `SCM_DO_BUILD_DURING_DEPLOYMENT=true` zum Verarbeiten des Kudu-Kaltstarts für 30 Sekunden in den Energiesparmodus zu wechseln</span><span class="sxs-lookup"><span data-stu-id="5f12f-1355">Changed `webapp up` to have a 30s sleep after setting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` appsetting to handle kudu cold start</span></span>
* <span data-ttu-id="5f12f-1356">Unterstützung für die `powershell`-Runtime zu `functionapp create` unter Windows hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1356">Added support for `powershell` runtime to `functionapp create` on Windows</span></span>
* <span data-ttu-id="5f12f-1357">Befehl `create-remote-connection` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1357">Added `create-remote-connection` command</span></span>

### <a name="batch"></a><span data-ttu-id="5f12f-1358">Batch</span><span class="sxs-lookup"><span data-stu-id="5f12f-1358">Batch</span></span>
* <span data-ttu-id="5f12f-1359">Fehler im Validierungssteuerelement für `--application-package-references`-Optionen korrigiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-1359">Fixed bug in validator for `--application-package-references` options</span></span>

### <a name="botservice"></a><span data-ttu-id="5f12f-1360">Botservice</span><span class="sxs-lookup"><span data-stu-id="5f12f-1360">Botservice</span></span>
* <span data-ttu-id="5f12f-1361">[BREAKING CHANGE]`bot create -v v4 -k webapp` geändert, sodass standardmäßig eine leerer Web-App-Bot erstellt wird (d. h. kein Bot wird in App Service bereitgestellt)</span><span class="sxs-lookup"><span data-stu-id="5f12f-1361">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to create an empty Web App Bot by default (i.e. no bot is deployed to the App Service)</span></span>
* <span data-ttu-id="5f12f-1362">`--echo`-Flag zu `bot create` hinzugefügt, sodass das alte Verhalten mit `-v v4` verwendet wird</span><span class="sxs-lookup"><span data-stu-id="5f12f-1362">Added `--echo` flag to `bot create` to use the old behavior with `-v v4`</span></span>
* <span data-ttu-id="5f12f-1363">[BREAKING CHANGE] Standardwert von `--version` in `v4` geändert</span><span class="sxs-lookup"><span data-stu-id="5f12f-1363">[BREAKING CHANGE] Changed the default value of  `--version` to `v4`</span></span>
  * <span data-ttu-id="5f12f-1364">__HINWEIS:__ `bot prepare-publish` verwendet weiterhin den alten Standard.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1364">__NOTE:__ `bot prepare-publish` still uses the its old default</span></span>
* <span data-ttu-id="5f12f-1365">[BREAKING CHANGE]`--lang` geändert, sodass der Standard nicht mehr `Csharp` ist.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1365">[BREAKING CHANGE] Changed `--lang` to no longer default to `Csharp`.</span></span> <span data-ttu-id="5f12f-1366">Wenn der Befehl `--lang` erfordert und dies nicht angegeben ist, wird der Befehl nun mit Fehler beendet.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1366">If the command requires `--lang` and it is not provided, the command will now error out</span></span>
* <span data-ttu-id="5f12f-1367">[BREAKING CHANGE]`--appid`- und `--password`-Argumente für `bot create` in erforderlich geändert, sie können jetzt über `ad app create` erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1367">[BREAKING CHANGE] Changed the `--appid` and `--password` args for `bot create` to be required and can now be created via `ad app create`</span></span>
* <span data-ttu-id="5f12f-1368">`--appid`- und `--password`-Validierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1368">Added `--appid` and `--password` validation</span></span>
* <span data-ttu-id="5f12f-1369">[BREAKING CHANGE]`bot create -v v4` geändert, sodass kein Speicherkonto bzw. keine Application Insights-Instanz erstellt oder verwendet wird</span><span class="sxs-lookup"><span data-stu-id="5f12f-1369">[BREAKING CHANGE] Changed `bot create -v v4` to not create or use a Storage Account or Application Insights</span></span>
* <span data-ttu-id="5f12f-1370">[BREAKING CHANGE]`bot create -v v3` geändert, sodass eine Region erforderlich ist, in der Application Insights verfügbar ist</span><span class="sxs-lookup"><span data-stu-id="5f12f-1370">[BREAKING CHANGE] Changed `bot create -v v3` to require a region where Application Insights is available</span></span>
* <span data-ttu-id="5f12f-1371">[BREAKING CHANGE]`bot update` geändert, sodass es sich jetzt nur auf spezifische Eigenschaften eines Bots auswirkt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1371">[BREAKING CHANGE] Changed `bot update` to now affect only specific properties of a bot</span></span>
* <span data-ttu-id="5f12f-1372">[BREAKING CHANGE]`--lang`-Flags geändert, sodass `Javascript` anstelle von `Node` akzeptiert wird</span><span class="sxs-lookup"><span data-stu-id="5f12f-1372">[BREAKING CHANGE] Changed `--lang` flags to accept `Javascript` instead of `Node`</span></span>
* <span data-ttu-id="5f12f-1373">[BREAKING CHANGE]`Node` als zulässiger `--lang`-Wert entfernt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1373">[BREAKING CHANGE] Removed `Node` as an allowed `--lang` value</span></span>
* <span data-ttu-id="5f12f-1374">[BREAKING CHANGE]`bot create -v v4 -k webapp` geändert, sodass `SCM_DO_BUILD_DURING_DEPLOYMENT` nicht mehr auf TRUE festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1374">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to no longer set `SCM_DO_BUILD_DURING_DEPLOYMENT` to true.</span></span> <span data-ttu-id="5f12f-1375">Alle Bereitstellungen über Kudu fungieren ihrem Standardverhalten entsprechend.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1375">All deployments through Kudu will act according to their default behavior</span></span>
* <span data-ttu-id="5f12f-1376">`bot download` für Bots ohne `.bot`-Dateien geändert, sodass die sprachspezifische Konfigurationsdatei mit Werten aus den Anwendungseinstellungen für den Bot erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1376">Changed `bot download` for bots without `.bot` files to create the language-specific configuration file with values from the Application Settings for the bot</span></span>
* <span data-ttu-id="5f12f-1377">Unterstützung für `Typescript` zu `bot prepare-deploy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1377">Added `Typescript` support to `bot prepare-deploy`</span></span>
* <span data-ttu-id="5f12f-1378">Warnmeldung zu `bot prepare-deploy` für `Javascript`- und `Typescript`-Bots hinzugefügt, wenn `package.json` in `--code-dir` nicht enthalten ist</span><span class="sxs-lookup"><span data-stu-id="5f12f-1378">Added warning message to `bot prepare-deploy` for `Javascript` and `Typescript` bots for when `--code-dir` does not contain `package.json`</span></span>
* <span data-ttu-id="5f12f-1379">`bot prepare-deploy` geändert, sodass bei Erfolg `true` zurückgegeben wird</span><span class="sxs-lookup"><span data-stu-id="5f12f-1379">Changed `bot prepare-deploy` to return `true` if successful</span></span>
* <span data-ttu-id="5f12f-1380">Ausführliche Protokollierung zu `bot prepare-deploy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1380">Added verbose logging to `bot prepare-deploy`</span></span>
* <span data-ttu-id="5f12f-1381">Mehr verfügbare Application Insights-Regionen zu `az bot create -v v3` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1381">Added more available Application Insights regions to `az bot create -v v3`</span></span>

### <a name="configure"></a><span data-ttu-id="5f12f-1382">Konfigurieren</span><span class="sxs-lookup"><span data-stu-id="5f12f-1382">Configure</span></span>
* <span data-ttu-id="5f12f-1383">Unterstützung für die ordnerbasierte Argument-Standardwertkonfigurationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1383">Added support for folder based argument default value configurations</span></span>

### <a name="eventhubs"></a><span data-ttu-id="5f12f-1384">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="5f12f-1384">Eventhubs</span></span>
* <span data-ttu-id="5f12f-1385">Befehle vom Typ `namespace network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1385">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="5f12f-1386">`--default-action`-Argument für Netzwerkregeln zu `namespace [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1386">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="5f12f-1387">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="5f12f-1387">Network</span></span>
* <span data-ttu-id="5f12f-1388">[BREAKING CHANGE]`--cache`-Argument mit `--defer` für `vnet [create|update]` ersetzt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1388">[BREAKING CHANGE] Replaced `--cache` arugment with `--defer` for `vnet [create|update]`</span></span> 

### <a name="policy-insights"></a><span data-ttu-id="5f12f-1389">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="5f12f-1389">Policy Insights</span></span>
* <span data-ttu-id="5f12f-1390">Unterstützung für `--expand PolicyEvaluationDetails` hinzugefügt, sodass Richtlinienauswertungsdetails von der Ressource abgefragt werden</span><span class="sxs-lookup"><span data-stu-id="5f12f-1390">Added support for `--expand PolicyEvaluationDetails` to query policy evaluation details on the resource</span></span>

### <a name="role"></a><span data-ttu-id="5f12f-1391">Role</span><span class="sxs-lookup"><span data-stu-id="5f12f-1391">Role</span></span>
* <span data-ttu-id="5f12f-1392">[VERALTET]: Ausblenden des „--password"-Arguments von `create-for-rbac` geändert; Unterstützung wird im Mai 2019 entfernt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1392">[DEPRECATED] Changed `create-for-rbac` hide '--password' argument - support will be removed in May 2019</span></span>

### <a name="service-bus"></a><span data-ttu-id="5f12f-1393">Service Bus</span><span class="sxs-lookup"><span data-stu-id="5f12f-1393">Service Bus</span></span>
* <span data-ttu-id="5f12f-1394">Befehle vom Typ `namespace network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1394">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="5f12f-1395">`--default-action`-Argument für Netzwerkregeln zu `namespace [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1395">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>
* <span data-ttu-id="5f12f-1396">`topic [create|update]` korrigiert, sodass `--max-size`-Unterstützung für 10-, 20-, 40- und 80-GB-Werte mit Premium-SKU zulässig ist</span><span class="sxs-lookup"><span data-stu-id="5f12f-1396">Fixed `topic [create|update]` to allow `--max-size` support for 10, 20, 40 and 80GB values with premium SKU</span></span>

### <a name="sql"></a><span data-ttu-id="5f12f-1397">SQL</span><span class="sxs-lookup"><span data-stu-id="5f12f-1397">SQL</span></span>
* <span data-ttu-id="5f12f-1398">Befehle vom Typ `sql virtual-cluster [list|show|delete]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1398">Added `sql virtual-cluster [list|show|delete]` commands</span></span>

### <a name="vm"></a><span data-ttu-id="5f12f-1399">VM</span><span class="sxs-lookup"><span data-stu-id="5f12f-1399">VM</span></span>
* <span data-ttu-id="5f12f-1400">`--protect-from-scale-in` und `--protect-from-scale-set-actions` zu `vmss update` hinzugefügt, sodass Aktualisierungen der Schutzrichtlinie von VMSS-VM-Instanzen aktiviert sind</span><span class="sxs-lookup"><span data-stu-id="5f12f-1400">Added `--protect-from-scale-in` and `--protect-from-scale-set-actions` to `vmss update` to enable updates to the protection policy of VMSS VM instances</span></span>
* <span data-ttu-id="5f12f-1401">`--instance-id` zu `vmss update` hinzugefügt, sodass allgemeine Aktualisierungen von VMSS-VM-Instanzen aktiviert sind</span><span class="sxs-lookup"><span data-stu-id="5f12f-1401">Added `--instance-id` to `vmss update` to enable generic update of VMSS VM instances</span></span>
* <span data-ttu-id="5f12f-1402">`--instance-id` zu `vmss wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1402">Added `--instance-id` to `vmss wait`</span></span>
* <span data-ttu-id="5f12f-1403">Neue `ppg`-Befehlsgruppe für die Verwaltung von Näherungsplatzierungsgruppen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1403">Added new `ppg` command group for managing Proximity Placement Groups</span></span>
* <span data-ttu-id="5f12f-1404">`--ppg` zu `[vm|vmss] create` und `vm availability-set create` für die Verwaltung von PPGs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1404">Added `--ppg` to `[vm|vmss] create` and `vm availability-set create` for managing PPGs</span></span>
* <span data-ttu-id="5f12f-1405">Parameter `--hyper-v-generation` zu `image create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1405">Added `--hyper-v-generation` parameter to `image create`</span></span>

## <a name="april-23-2019"></a><span data-ttu-id="5f12f-1406">23. April 2019</span><span class="sxs-lookup"><span data-stu-id="5f12f-1406">April 23, 2019</span></span>

<span data-ttu-id="5f12f-1407">Version 2.0.63</span><span class="sxs-lookup"><span data-stu-id="5f12f-1407">Version 2.0.63</span></span>

### <a name="acs"></a><span data-ttu-id="5f12f-1408">ACS</span><span class="sxs-lookup"><span data-stu-id="5f12f-1408">ACS</span></span>
* <span data-ttu-id="5f12f-1409">`aks get-credentials` zur Anzeige einer Eingabeaufforderung zum Überschreiben doppelter Werte geändert</span><span class="sxs-lookup"><span data-stu-id="5f12f-1409">Changed `aks get-credentials` to prompt to overwrite duplicated values</span></span>
* <span data-ttu-id="5f12f-1410">`(PREVIEW)` aus Dev Spaces-Befehlen „aks use-dev-spaces“ und „aks remove-dev-spaces“ entfernt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1410">Removed `(PREVIEW)` from Dev Spaces commands "aks use-dev-spaces" and "aks remove-dev-spaces"</span></span>

### <a name="ams"></a><span data-ttu-id="5f12f-1411">AMS</span><span class="sxs-lookup"><span data-stu-id="5f12f-1411">AMS</span></span>
* <span data-ttu-id="5f12f-1412">Fehler bei der Objekt- und Kontofilteraktualisierung behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-1412">Fixed bug with asset and account filters update</span></span>

### <a name="appservice"></a><span data-ttu-id="5f12f-1413">AppService</span><span class="sxs-lookup"><span data-stu-id="5f12f-1413">AppService</span></span>
* <span data-ttu-id="5f12f-1414">Unterstützung für die App Service-Umgebung (App Service Environment, ASE) und Zeitlimit zu `webapp ssh` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1414">Added support for ASE and timeout to `webapp ssh`</span></span>
* <span data-ttu-id="5f12f-1415">Unterstützung für die Einrichtung von CI/CD für eine Azure DevOps-Pipeline aus einem GitHub-Repository zu Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1415">Added support for establishing CI CD to an Azure DevOps pipeline from a Github repository to Function apps</span></span>
* <span data-ttu-id="5f12f-1416">`--github-pat`-Argument zu `functionapp devops-build create` hinzugefügt, um persönliche GitHub-Zugriffstoken zu akzeptieren</span><span class="sxs-lookup"><span data-stu-id="5f12f-1416">Added `--github-pat` argument to `functionapp devops-build create` to accept Github personal access token</span></span>
* <span data-ttu-id="5f12f-1417">`--github-repository`-Argument zu `functionapp devops-build create` hinzugefügt, um das GitHub-Repository mit dem Quellcode einer Funktions-App zu akzeptieren</span><span class="sxs-lookup"><span data-stu-id="5f12f-1417">Added `--github-repository` argument to `functionapp devops-build create` to accept Github repository that contains a functionapp source code</span></span>
* <span data-ttu-id="5f12f-1418">Problem behoben, aufgrund dessen bei `az webapp up --logs` ein Fehler auftrat und die .NET Core-Standardversion auf 2.1 aktualisiert wurde</span><span class="sxs-lookup"><span data-stu-id="5f12f-1418">Fixed issue where `az webapp up --logs` was failing with a error and updating default .NETCORE version to 2.1</span></span>
* <span data-ttu-id="5f12f-1419">Unnötige Funktions-App-Einstellungen beim Erstellen einer Funktions-App mit Verbrauchsplan entfernt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1419">Removed unnecessary functionapp settings when creating a function app with consumption plan</span></span>
* <span data-ttu-id="5f12f-1420">`webapp up` geändert, sodass die ASP-Standardzeichenfolge jetzt eine Zahl am Ende anfügt, um einen neuen ASP basierend auf SKU-Optionen zu erstellen</span><span class="sxs-lookup"><span data-stu-id="5f12f-1420">Changed `webapp up` so the default asp string now appends number at the end to create a new ASP based on SKU options</span></span>
* <span data-ttu-id="5f12f-1421">`-b` als Option für `webapp up` hinzugefügt, um die App im Browser zu starten</span><span class="sxs-lookup"><span data-stu-id="5f12f-1421">Added `-b` as an option to `webapp up` to launch the app in the browser</span></span>
* <span data-ttu-id="5f12f-1422">`webapp deployment source config zip` geändert, um die `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`-Umgebungsvariable zu behandeln</span><span class="sxs-lookup"><span data-stu-id="5f12f-1422">Changed `webapp deployment source config zip` to handle `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="5f12f-1423">Bereitstellungs-Manager</span><span class="sxs-lookup"><span data-stu-id="5f12f-1423">Deployment Manager</span></span>
* <span data-ttu-id="5f12f-1424">[VORSCHAUVERSIPN] Erstellen und Verwalten von Artefakten, die Rollouts unterstützen</span><span class="sxs-lookup"><span data-stu-id="5f12f-1424">[PREVIEW] Create and manage artifacts that support rollouts</span></span>

### <a name="lab"></a><span data-ttu-id="5f12f-1425">Labor</span><span class="sxs-lookup"><span data-stu-id="5f12f-1425">Lab</span></span>
* <span data-ttu-id="5f12f-1426">Fehler behoben, der zu einer vorzeitigen Beendigung führen würde</span><span class="sxs-lookup"><span data-stu-id="5f12f-1426">Fixed bug which would cause an early exit</span></span>

### <a name="network"></a><span data-ttu-id="5f12f-1427">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="5f12f-1427">Network</span></span>
* <span data-ttu-id="5f12f-1428">Automatische Delegierung des Namenservers im übergeordneten Element während der Erstellung der untergeordneten Zone zu `dns zone create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1428">Added auto name server delegation to `dns zone create` in parent during child zone creation</span></span>

### <a name="resource"></a><span data-ttu-id="5f12f-1429">Resource</span><span class="sxs-lookup"><span data-stu-id="5f12f-1429">Resource</span></span>
* <span data-ttu-id="5f12f-1430">[VERALTET]: Argumente `--link-id`, `--target-id` und `--filter-string` von `resource link` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-1430">[DEPRECATED] Deprecated `--link-id`, `--target-id` and `--filter-string` arguments of `resource link`</span></span>
  * <span data-ttu-id="5f12f-1431">Verwenden Sie stattdessen die Argumente `--link`, `--target` und `--filter`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1431">Use the arguments `--link`, `--target`, and `--filter` instead</span></span>
* <span data-ttu-id="5f12f-1432">Problem behoben, aufgrund dessen `resource link [create|update]`-Befehle nicht verwendet werden konnten</span><span class="sxs-lookup"><span data-stu-id="5f12f-1432">Fixed issue where `resource link [create|update]` commands would not work</span></span>
* <span data-ttu-id="5f12f-1433">Problem behoben, aufgrund dessen das Löschen anhand einer Ressourcen-ID bei einem Fehler zu einem Absturz führen konnte</span><span class="sxs-lookup"><span data-stu-id="5f12f-1433">Fixed an issue where deleting using a resource ID could crash on error</span></span>

### <a name="sql"></a><span data-ttu-id="5f12f-1434">SQL</span><span class="sxs-lookup"><span data-stu-id="5f12f-1434">SQL</span></span>
* <span data-ttu-id="5f12f-1435">Unterstützung für benutzerdefinierte Zeitzonen auf verwalteten Instanzen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1435">Added support for custom time zone on managed instances</span></span>
* <span data-ttu-id="5f12f-1436">Geändert, um die Verwendung des Namens eines Pools für elastische Datenbanken mit `sql db update` zuzulassen</span><span class="sxs-lookup"><span data-stu-id="5f12f-1436">Changed to allow elastic pool name to be used with `sql db update`</span></span>
* <span data-ttu-id="5f12f-1437">Unterstützung für `--no-wait` zu `sql server [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1437">Added `--no-wait` support to `sql server [create|update]`</span></span>
* <span data-ttu-id="5f12f-1438">Befehl `sql server wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1438">Added command `sql server wait`</span></span>

### <a name="storage"></a><span data-ttu-id="5f12f-1439">Storage</span><span class="sxs-lookup"><span data-stu-id="5f12f-1439">Storage</span></span>
* <span data-ttu-id="5f12f-1440">Problem mit doppelt codierten SAS-Token in `storage blob generate-sas` behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-1440">Fixed issue with double-encoded SAS tokens in `storage blob generate-sas`</span></span>

### <a name="vm"></a><span data-ttu-id="5f12f-1441">VM</span><span class="sxs-lookup"><span data-stu-id="5f12f-1441">VM</span></span>
* <span data-ttu-id="5f12f-1442">`--skip-shutdown`-Flag zum Ausschalten von VMs ohne Herunterfahren zu `vm|vmss stop` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1442">Added `--skip-shutdown` flag to `vm|vmss stop` to power-off VMs without shutdown</span></span>
* <span data-ttu-id="5f12f-1443">`--storage-account-type`-Argument zum Festlegen des Kontotyps des Veröffentlichungsprofils zu `sig image-version create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1443">Added `--storage-account-type` argument to `sig image-version create` to set the publishing profile's account type</span></span>
* <span data-ttu-id="5f12f-1444">`--target-regions`-Argument zu `sig image-version create` hinzugefügt, um das Festlegen von regionsspezifischen Speicherkontotypen zuzulassen</span><span class="sxs-lookup"><span data-stu-id="5f12f-1444">Added `--target-regions` argument to `sig image-version create` to allow setting region-specific storage account types</span></span>

## <a name="april-9-2019"></a><span data-ttu-id="5f12f-1445">9\. April 2019</span><span class="sxs-lookup"><span data-stu-id="5f12f-1445">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="5f12f-1446">Core</span><span class="sxs-lookup"><span data-stu-id="5f12f-1446">Core</span></span>
* <span data-ttu-id="5f12f-1447">Problem behoben, aufgrund dessen einige Erweiterungen mit der Version `Unknown` angezeigt wurden und nicht aktualisiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="5f12f-1447">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="5f12f-1448">ACR</span><span class="sxs-lookup"><span data-stu-id="5f12f-1448">ACR</span></span>
* <span data-ttu-id="5f12f-1449">Unterstützung für die kontextlose Ausführung eines Images hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1449">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="5f12f-1450">AMS</span><span class="sxs-lookup"><span data-stu-id="5f12f-1450">AMS</span></span>
* [VERALTET]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
[DEPRECATED]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [BREAKING CHANGE]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="5f12f-1453">Unterstützung für neue Verschlüsselungsparameter in `ams streaming-policy create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1453">Added new encryption parameters support in `ams streaming-policy create`</span></span>
* <span data-ttu-id="5f12f-1454">Neuer Parameter `--filters` zu `ams streaming-locator create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1454">Added new paramter `--filters` to `ams streaming-locator create`</span></span>

### <a name="appservice"></a><span data-ttu-id="5f12f-1455">AppService</span><span class="sxs-lookup"><span data-stu-id="5f12f-1455">AppService</span></span>
* <span data-ttu-id="5f12f-1456">Unterstützung für `--logs` zu `webapp up` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1456">Added `--logs` support to `webapp up`</span></span>
* <span data-ttu-id="5f12f-1457">Probleme bei der Generierung von `azure-pipelines.yml` beim Befehl `functionapp devops-build create` behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-1457">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="5f12f-1458">Fehlerbehandlung und Indikatoren für `unctionapp devops-build create` verbessert</span><span class="sxs-lookup"><span data-stu-id="5f12f-1458">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="5f12f-1459">[BREAKING CHANGE] Flag `--local-git` für den Befehl `devops-build` entfernt; lokale Git-Erkennung und -Verarbeitung sind zum Erstellen von Azure DevOps-Pipelines obligatorisch</span><span class="sxs-lookup"><span data-stu-id="5f12f-1459">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="5f12f-1460">Unterstützung für das Erstellen von Linux-Functions-Plänen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1460">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="5f12f-1461">Möglichkeit zum Wechseln eines Plans unter einer Funktions-App mit `functionapp update --plan` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1461">Added ability to switch a plan underneath a function app using `functionapp update --plan`</span></span>
* <span data-ttu-id="5f12f-1462">Unterstützung für Einstellungen zum Aufskalieren für den Azure Functions-Premium-Plan hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1462">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="5f12f-1463">CDN</span><span class="sxs-lookup"><span data-stu-id="5f12f-1463">CDN</span></span>
* <span data-ttu-id="5f12f-1464">Unterstützung hinzugefügt für `Microsoft_Standard` und `Standard_ChinaCdn`</span><span class="sxs-lookup"><span data-stu-id="5f12f-1464">Added support for `Microsoft_Standard` and `Standard_ChinaCdn`</span></span>

### <a name="feedback"></a><span data-ttu-id="5f12f-1465">Feedback</span><span class="sxs-lookup"><span data-stu-id="5f12f-1465">Feedback</span></span>
* <span data-ttu-id="5f12f-1466">`feedback` zur Anzeige von Metadaten zu den zuletzt ausgeführten Befehlen geändert</span><span class="sxs-lookup"><span data-stu-id="5f12f-1466">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="5f12f-1467">`feedback` geändert, um den Benutzer zur Unterstützung beim Issueerstellungsprozess aufzufordern (durch Öffnen eines Browsers und Verwenden einer Issuevorlage)</span><span class="sxs-lookup"><span data-stu-id="5f12f-1467">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="5f12f-1468">`feedback` geändert, um den Issuetext bei der Ausführung mit „--verbose“ auszugeben</span><span class="sxs-lookup"><span data-stu-id="5f12f-1468">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="5f12f-1469">Überwachen</span><span class="sxs-lookup"><span data-stu-id="5f12f-1469">Monitor</span></span>
* <span data-ttu-id="5f12f-1470">Problem behoben, aufgrund dessen „Count“ kein zulässiger Wert für `metrics alert [create|update]` war</span><span class="sxs-lookup"><span data-stu-id="5f12f-1470">Fixed issue where "count" was not a permitted value with `metrics alert [create|update]`</span></span> 

### <a name="network"></a><span data-ttu-id="5f12f-1471">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="5f12f-1471">Network</span></span>
* <span data-ttu-id="5f12f-1472">Problem behoben, aufgrund dessen das Tabellenformat mit `vnet-gateway list-bgp-peer-status` nicht angezeigt wurde</span><span class="sxs-lookup"><span data-stu-id="5f12f-1472">Fixed table format not displaying with `vnet-gateway list-bgp-peer-status`</span></span>
* <span data-ttu-id="5f12f-1473">Befehle `list-request-headers` und `list-response-headers` zu `application-gateway rewrite-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1473">Added `list-request-headers` and `list-response-headers` commands to `application-gateway rewrite-rule`</span></span>
* <span data-ttu-id="5f12f-1474">Befehl `list-server-variables` zu `application-gateway rewrite-rule condition` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1474">Added `list-server-variables` command to `application-gateway rewrite-rule condition`</span></span>
* <span data-ttu-id="5f12f-1475">Problem behoben, aufgrund dessen durch das Aktualisieren des Linkstatus für einen ExpressRoute-Port eine Ausnahme vom Typ „unbekanntes Attribut“ ausgelöst wurde: `express-route port update`</span><span class="sxs-lookup"><span data-stu-id="5f12f-1475">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception `express-route port update`</span></span>

### <a name="privatedns"></a><span data-ttu-id="5f12f-1476">PrivateDNS</span><span class="sxs-lookup"><span data-stu-id="5f12f-1476">PrivateDNS</span></span>
* <span data-ttu-id="5f12f-1477">`network private-dns` für private DNS-Zonen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1477">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="5f12f-1478">Resource</span><span class="sxs-lookup"><span data-stu-id="5f12f-1478">Resource</span></span>
* <span data-ttu-id="5f12f-1479">Problem mit `deployment create` und `group deployment create` behoben, aufgrund dessen eine Parameterdatei mit leerem Parametersatz nicht verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="5f12f-1479">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="5f12f-1480">Role</span><span class="sxs-lookup"><span data-stu-id="5f12f-1480">Role</span></span>
* <span data-ttu-id="5f12f-1481">`create-for-rbac` korrigiert, um `--years` korrekt zu verarbeiten</span><span class="sxs-lookup"><span data-stu-id="5f12f-1481">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="5f12f-1482">[BREAKING CHANGE]`role assignment delete` geändert, um eine Eingabeaufforderung anzuzeigen, wenn alle Zuweisungen im Abonnement ohne Bedingungen gelöscht werden</span><span class="sxs-lookup"><span data-stu-id="5f12f-1482">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="5f12f-1483">SQL</span><span class="sxs-lookup"><span data-stu-id="5f12f-1483">SQL</span></span>
* <span data-ttu-id="5f12f-1484">`sql mi [create|update]` mit den Eigenschaften „proxyOverride“ und „publicDataEndpointEnabled“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-1484">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="5f12f-1485">Storage</span><span class="sxs-lookup"><span data-stu-id="5f12f-1485">Storage</span></span>
* <span data-ttu-id="5f12f-1486">[BREAKING CHANGE] Ergebnis von `storage blob delete` entfernt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1486">[BREAKING CHANGE] Removed result of `storage blob delete`</span></span>
* <span data-ttu-id="5f12f-1487">`--full-uri` zu `storage blob generate-sas` hinzugefügt, um den vollständigen URI für das Blob mit SAS zu erstellen</span><span class="sxs-lookup"><span data-stu-id="5f12f-1487">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="5f12f-1488">`--file-snapshot` zu `storage file copy start` hinzugefügt, um die Datei aus der Momentaufnahme zu kopieren</span><span class="sxs-lookup"><span data-stu-id="5f12f-1488">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="5f12f-1489">`storage blob copy cancel` geändert, um anstelle der Ausnahme für „NoPendingCopyOperation“ nur den Fehler anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="5f12f-1489">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="5f12f-1490">26. März 2019</span><span class="sxs-lookup"><span data-stu-id="5f12f-1490">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="5f12f-1491">Core</span><span class="sxs-lookup"><span data-stu-id="5f12f-1491">Core</span></span>
* <span data-ttu-id="5f12f-1492">Probleme mit der Inkompatibilität der Entwicklungserweiterung behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-1492">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="5f12f-1493">Die Fehlerbehandlung verweist Kunden jetzt auf die Problemseite.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1493">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="5f12f-1494">Cloud</span><span class="sxs-lookup"><span data-stu-id="5f12f-1494">Cloud</span></span>
* <span data-ttu-id="5f12f-1495">Fehler „Abonnement nicht gefunden“ in `cloud set` behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-1495">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="5f12f-1496">ACR</span><span class="sxs-lookup"><span data-stu-id="5f12f-1496">ACR</span></span>
* <span data-ttu-id="5f12f-1497">Redundante Quellen im Imageimport korrigiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-1497">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="5f12f-1498">`--auth-mode` wurde den Befehlen `acr build`, `acr run`, `acr task create` und `acr task update` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1498">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="5f12f-1499">Befehlsgruppe „acr task credential“ zum Verwalten von Anmeldeinformationen für eine Aufgabe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1499">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="5f12f-1500">„--no-wait“ zum Befehl `acr build` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1500">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="5f12f-1501">AppService</span><span class="sxs-lookup"><span data-stu-id="5f12f-1501">AppService</span></span>
* <span data-ttu-id="5f12f-1502">Problem behoben, das dazu führte, dass die Ausführung aus einem leeren Verzeichnis oder ein Szenario mit unbekannten Code von `webapp up` nicht korrekt behandelt wurde</span><span class="sxs-lookup"><span data-stu-id="5f12f-1502">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="5f12f-1503">Problem behoben, aufgrund dessen Slots für `[webapp|functionapp] config ssl bind` nicht verwendet werden konnten</span><span class="sxs-lookup"><span data-stu-id="5f12f-1503">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="5f12f-1504">Bot Service</span><span class="sxs-lookup"><span data-stu-id="5f12f-1504">BOT Service</span></span>
* <span data-ttu-id="5f12f-1505">`bot prepare-deploy` hinzugefügt, um die Bereitstellung von Bots über `webapp` vorzubereiten</span><span class="sxs-lookup"><span data-stu-id="5f12f-1505">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="5f12f-1506">`bot create --kind registration` geändert, um das Kennwort anzuzeigen, falls kein Kennwort angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="5f12f-1506">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="5f12f-1507">[BREAKING CHANGE]`--endpoint` wurde in `bot create --kind registration` geändert, sodass nun standardmäßig eine leere Zeichenfolge verwendet wird, anstatt eine Angabe zu erfordern.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1507">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="5f12f-1508">`SCM_DO_BUILD_DURING_DEPLOYMENT` zu den Anwendungseinstellungen der ARM-Vorlage für Web-App-Bot (v4) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1508">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="5f12f-1509">CDN</span><span class="sxs-lookup"><span data-stu-id="5f12f-1509">CDN</span></span>
* <span data-ttu-id="5f12f-1510">Unterstützung für `--no-wait` zu `cdn endpoint [create|update|start|stop|delete|load|purge]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1510">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* <span data-ttu-id="5f12f-1511">[BREAKING CHANGE] Das standardmäßige Zwischenspeicherverhalten für Abfragezeichenfolgen von `cdn endpoint create` wurde geändert.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1511">[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour.</span></span> <span data-ttu-id="5f12f-1512">Es wird nicht mehr standardmäßig „IgnoreQueryString“ festgelegt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1512">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="5f12f-1513">Er wird jetzt vom Dienst festgelegt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1513">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="5f12f-1514">Cosmosdb</span><span class="sxs-lookup"><span data-stu-id="5f12f-1514">Cosmosdb</span></span>
* <span data-ttu-id="5f12f-1515">Unterstützung für `--enable-multiple-write-locations` bei Kontoaktualisierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1515">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="5f12f-1516">Untergruppe `network-rule` mit Befehlen `add`, `remove` und `list` zum Verwalten von VNET-Regeln eines Cosmos DB-Kontos hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1516">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="5f12f-1517">Interactive</span><span class="sxs-lookup"><span data-stu-id="5f12f-1517">Interactive</span></span>
* <span data-ttu-id="5f12f-1518">Inkompatibilität mit der über azdev installierten interaktiven Erweiterung korrigiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-1518">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="5f12f-1519">Überwachen</span><span class="sxs-lookup"><span data-stu-id="5f12f-1519">Monitor</span></span>
* <span data-ttu-id="5f12f-1520">Geändert, sodass der Dimensionswert `*` für `monitor metrics alert [create|update]` zulässig ist</span><span class="sxs-lookup"><span data-stu-id="5f12f-1520">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="5f12f-1521">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="5f12f-1521">Network</span></span>
* <span data-ttu-id="5f12f-1522">Befehlsgruppe `rewrite-rule` zu `application-gateway` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1522">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="5f12f-1523">Profil</span><span class="sxs-lookup"><span data-stu-id="5f12f-1523">Profile</span></span>
* <span data-ttu-id="5f12f-1524">Kontounterstützung auf Mandantenebene für verwaltete Dienstidentität zu `login` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1524">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="5f12f-1525">Postgres</span><span class="sxs-lookup"><span data-stu-id="5f12f-1525">Postgres</span></span> 
* <span data-ttu-id="5f12f-1526">postgresql-Befehle vom Typ `replica` und Befehl `restart server` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1526">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="5f12f-1527">Änderungen vorgenommen, um den Standardspeicherort aus der Ressourcengruppe abzurufen, wenn er für die Erstellung von Servern nicht angegeben wurde, und um eine Überprüfung für die Aufbewahrungstage hinzuzufügen</span><span class="sxs-lookup"><span data-stu-id="5f12f-1527">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="5f12f-1528">Resource</span><span class="sxs-lookup"><span data-stu-id="5f12f-1528">Resource</span></span>
* <span data-ttu-id="5f12f-1529">Verbesserte Tabellenausgabe für `deployment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="5f12f-1529">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="5f12f-1530">Problem mit `deployment [create|validate]` behoben, aufgrund dessen der Typ „secureObject“ nicht erkannt wurde</span><span class="sxs-lookup"><span data-stu-id="5f12f-1530">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="5f12f-1531">Graph</span><span class="sxs-lookup"><span data-stu-id="5f12f-1531">Graph</span></span>
* <span data-ttu-id="5f12f-1532">Unterstützung für `--end-date` zu `ad [app|sp] credential reset` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1532">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="5f12f-1533">Unterstützung für das Hinzufügen von Berechtigungen mit `ad app permission add` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1533">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="5f12f-1534">Fehler mit `ad app permission list` behoben, wenn keine Berechtigungen vorlagen</span><span class="sxs-lookup"><span data-stu-id="5f12f-1534">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="5f12f-1535">Änderung an `ad sp delete` vorgenommen, um das Entfernen einer Rollenzuweisung zu überspringen, wenn das aktuelle Konto kein Abonnement enthält</span><span class="sxs-lookup"><span data-stu-id="5f12f-1535">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="5f12f-1536">`ad app create` geändert, sodass ohne Angabe für `--identifier-uris` standardmäßig eine leere Liste verwendet wird</span><span class="sxs-lookup"><span data-stu-id="5f12f-1536">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="5f12f-1537">storage</span><span class="sxs-lookup"><span data-stu-id="5f12f-1537">storage</span></span>
* <span data-ttu-id="5f12f-1538">`--snapshot` zu `storage file download-batch` für den Download von einer Freigabemomentaufnahme hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1538">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="5f12f-1539">Statusanzeige für `storage blob [download-batch|upload-batch]` geändert, damit sie weniger ausführlich dargestellt wird und das aktuelle Blob angibt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1539">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="5f12f-1540">Problem mit `storage account update` behoben, das beim Aktualisieren von Verschlüsselungsparametern auftrat</span><span class="sxs-lookup"><span data-stu-id="5f12f-1540">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="5f12f-1541">Problem behoben, bei dem für `storage blob show` ein Fehler auftrat, wenn oauth (`--auth-mode=login`) verwendet wurde</span><span class="sxs-lookup"><span data-stu-id="5f12f-1541">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="5f12f-1542">VM</span><span class="sxs-lookup"><span data-stu-id="5f12f-1542">VM</span></span>
* <span data-ttu-id="5f12f-1543">Befehl `image update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1543">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="5f12f-1544">12. März 2019</span><span class="sxs-lookup"><span data-stu-id="5f12f-1544">March 12, 2019</span></span>

<span data-ttu-id="5f12f-1545">Version 2.0.60</span><span class="sxs-lookup"><span data-stu-id="5f12f-1545">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="5f12f-1546">Core</span><span class="sxs-lookup"><span data-stu-id="5f12f-1546">Core</span></span>

* <span data-ttu-id="5f12f-1547">Falsche Fehlermeldung in `cloud set` zu nicht gefundenem Abonnement korrigiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-1547">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="5f12f-1548">ACR</span><span class="sxs-lookup"><span data-stu-id="5f12f-1548">ACR</span></span>

* <span data-ttu-id="5f12f-1549">Redundante Quellen im Imageimport korrigiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-1549">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="5f12f-1550">ACS</span><span class="sxs-lookup"><span data-stu-id="5f12f-1550">ACS</span></span>

* <span data-ttu-id="5f12f-1551">Änderung vorgenommen, um den Parameter `--listen-address` für `aks browse` zu ignorieren, wenn er nicht von kubectl unterstützt wird</span><span class="sxs-lookup"><span data-stu-id="5f12f-1551">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="5f12f-1552">AppService</span><span class="sxs-lookup"><span data-stu-id="5f12f-1552">AppService</span></span>

* <span data-ttu-id="5f12f-1553">`[webapp|functionapp] deployment list-publishing-credentials` hinzugefügt, um die Kudu-Veröffentlichungs-URL und die entsprechenden Anmeldeinformationen abzurufen</span><span class="sxs-lookup"><span data-stu-id="5f12f-1553">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="5f12f-1554">Fehlerhafte Ausgabeanweisung für `webapp auth update` entfernt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1554">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="5f12f-1555">`functionapp` korrigiert, um das korrekte Image für die Runtime in App Service-Plänen unter Linux festzulegen</span><span class="sxs-lookup"><span data-stu-id="5f12f-1555">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="5f12f-1556">Vorschau-Tag für `webapp up` entfernt und Verbesserungen am Befehl implementiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-1556">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="5f12f-1557">Botservice</span><span class="sxs-lookup"><span data-stu-id="5f12f-1557">Botservice</span></span>

* <span data-ttu-id="5f12f-1558">`SCM_DO_BUILD_DURING_DEPLOYMENT` zu den Anwendungseinstellungen der ARM-Vorlage für Web-App-Bot (v4) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1558">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="5f12f-1559">`Microsoft-BotFramework-AppId` und `Microsoft-BotFramework-AppPassword` zu den Anwendungseinstellungen der ARM-Vorlage für Web-App-Bot (v4) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1559">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="5f12f-1560">Einfache Anführungszeichen aus der Befehlsausgabe von `bot publish` am Ende von `bot create` entfernt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1560">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="5f12f-1561">`bot publish` wurde geändert und ist jetzt asynchron.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1561">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="5f12f-1562">Container</span><span class="sxs-lookup"><span data-stu-id="5f12f-1562">Container</span></span>

* <span data-ttu-id="5f12f-1563">Argument `--no-wait` zu `container [start|restart]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1563">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="5f12f-1564">EventHub</span><span class="sxs-lookup"><span data-stu-id="5f12f-1564">EventHub</span></span>

* <span data-ttu-id="5f12f-1565">Flag `--skip-empty-archives` zu `eventhub create|update` hinzugefügt, um leere Archive in der Aufzeichnung zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="5f12f-1565">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="5f12f-1566">Suchen</span><span class="sxs-lookup"><span data-stu-id="5f12f-1566">Find</span></span>

* <span data-ttu-id="5f12f-1567">Umfangreiches Funktionsupdate</span><span class="sxs-lookup"><span data-stu-id="5f12f-1567">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="5f12f-1568">HDInsight</span><span class="sxs-lookup"><span data-stu-id="5f12f-1568">HDInsight</span></span>

* <span data-ttu-id="5f12f-1569">Parameter `--storage-account-managed-identity` zu `hdinsight create` hinzugefügt, um MSI in ADLS Gen2 zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="5f12f-1569">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="5f12f-1570">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="5f12f-1570">Network</span></span>

* <span data-ttu-id="5f12f-1571">Problem mit `vpn-connection update` behoben, aufgrund dessen die Aktualisierung einer VPN-Verbindung zwischen Gateways in verschiedenen Abonnements fehlschlug</span><span class="sxs-lookup"><span data-stu-id="5f12f-1571">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="5f12f-1572">Rdbms</span><span class="sxs-lookup"><span data-stu-id="5f12f-1572">Rdbms</span></span>

* <span data-ttu-id="5f12f-1573">Kleinere Korrekturen, um den Standardspeicherort aus der Ressourcengruppe abzurufen, wenn er für die Erstellung von Servern nicht angegeben wurde, und um eine Überprüfung für die Aufbewahrungstage hinzuzufügen</span><span class="sxs-lookup"><span data-stu-id="5f12f-1573">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="5f12f-1574">Role</span><span class="sxs-lookup"><span data-stu-id="5f12f-1574">Role</span></span>

* <span data-ttu-id="5f12f-1575">`role definition update` wurde korrigiert und nutzt nun die ID, um die Definition korrekt aufzulösen.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1575">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="5f12f-1576">`ad app credential reset` geändert, um die Annahme zu entfernen, dass der Dienstprinzipal der App stets vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="5f12f-1576">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="5f12f-1577">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="5f12f-1577">Service Fabric</span></span>

* <span data-ttu-id="5f12f-1578">Das Problem, dass `sf cluster list` nicht wiederholbar war, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1578">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="5f12f-1579">26. Februar 2019</span><span class="sxs-lookup"><span data-stu-id="5f12f-1579">February 26, 2019</span></span>

<span data-ttu-id="5f12f-1580">Version 2.0.59</span><span class="sxs-lookup"><span data-stu-id="5f12f-1580">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="5f12f-1581">Core</span><span class="sxs-lookup"><span data-stu-id="5f12f-1581">Core</span></span>

* <span data-ttu-id="5f12f-1582">Problem behoben, aufgrund dessen die Verwendung von `--subscription NAME` in einigen Instanzen eine Ausnahme ausgelöst hat</span><span class="sxs-lookup"><span data-stu-id="5f12f-1582">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="5f12f-1583">ACR</span><span class="sxs-lookup"><span data-stu-id="5f12f-1583">ACR</span></span>

* <span data-ttu-id="5f12f-1584">Parameter `--target` für die Befehle `acr build`, `acr task create` und `acr task update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1584">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="5f12f-1585">Verbesserte Fehlerbehandlung für Runtimebefehle, wenn keine Anmeldung bei Azure besteht</span><span class="sxs-lookup"><span data-stu-id="5f12f-1585">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="5f12f-1586">ACS</span><span class="sxs-lookup"><span data-stu-id="5f12f-1586">ACS</span></span>

* <span data-ttu-id="5f12f-1587">Option `--listen-address` zu `aks port-forward` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1587">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="5f12f-1588">AppService</span><span class="sxs-lookup"><span data-stu-id="5f12f-1588">AppService</span></span>

* <span data-ttu-id="5f12f-1589">Befehl `functionapp devops-build` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1589">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="5f12f-1590">Batch</span><span class="sxs-lookup"><span data-stu-id="5f12f-1590">Batch</span></span>
* <span data-ttu-id="5f12f-1591">[BREAKING CHANGE] Befehl `batch pool upgrade os` entfernt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1591">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="5f12f-1592">[BREAKING CHANGE]`Pacakges`-Eigenschaft aus `Application`-Antworten entfernt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1592">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="5f12f-1593">Befehl `batch application package list` zum Auflisten von Paketen einer Anwendung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1593">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="5f12f-1594">[BREAKING CHANGE]`--application-id` in allen `batch application`-Befehlen in `--application-name` geändert</span><span class="sxs-lookup"><span data-stu-id="5f12f-1594">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="5f12f-1595">Argument `--json-file` für Befehle zum Anfordern der unformatierten API-Antwort hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1595">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="5f12f-1596">Validierung aktualisiert, sodass das `https://`-Element automatisch in alle Endpunkte aufgenommen wird, wenn es fehlt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1596">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="5f12f-1597">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="5f12f-1597">CosmosDB</span></span>

* <span data-ttu-id="5f12f-1598">Untergruppe `network-rule` mit Befehlen `add`, `remove` und `list` zum Verwalten von VNET-Regeln eines Cosmos DB-Kontos hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1598">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="5f12f-1599">Kusto</span><span class="sxs-lookup"><span data-stu-id="5f12f-1599">Kusto</span></span>

* <span data-ttu-id="5f12f-1600">[BREAKING CHANGE] Typen `hot_cache_period` und `soft_delete_period` für Datenbank in Format der Zeitspanne nach ISO8601 geändert</span><span class="sxs-lookup"><span data-stu-id="5f12f-1600">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="5f12f-1601">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="5f12f-1601">Network</span></span>

* <span data-ttu-id="5f12f-1602">Argument `--express-route-gateway-bypass` zu `vpn-connection [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1602">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="5f12f-1603">Befehlsgruppen aus `express-route`-Erweiterungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1603">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="5f12f-1604">Befehlsgruppen `express-route gateway` und `express-route port` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1604">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="5f12f-1605">Argument `--legacy-mode` zu `express-route peering [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1605">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="5f12f-1606">Argumente `--allow-classic-operations` und `--express-route-port` zu `express-route [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1606">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="5f12f-1607">Argument `--gateway-default-site` zu `vnet-gateway [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1607">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="5f12f-1608">Befehle vom Typ `ipsec-policy` zu `vnet-gateway` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1608">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="5f12f-1609">Resource</span><span class="sxs-lookup"><span data-stu-id="5f12f-1609">Resource</span></span>

* <span data-ttu-id="5f12f-1610">Problem mit `deployment create` behoben, aufgrund dessen beim Feld „Typ“ die Groß-/Kleinschreibung beachtet wurde</span><span class="sxs-lookup"><span data-stu-id="5f12f-1610">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="5f12f-1611">Unterstützung für URI-basierte Parameterdatei zu `policy assignment create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1611">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="5f12f-1612">Unterstützung für URI-basierte Parameter und Definitionen zu `policy set-definition update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1612">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="5f12f-1613">Verarbeitung von Parametern und Regeln für `policy definition update` korrigiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-1613">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="5f12f-1614">Problem mit `resource show/update/delete/tag/invoke-action` behoben, aufgrund dessen bei abonnementübergreifenden IDs die Abonnement-ID nicht ordnungsgemäß berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="5f12f-1614">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="5f12f-1615">Role</span><span class="sxs-lookup"><span data-stu-id="5f12f-1615">Role</span></span>

* <span data-ttu-id="5f12f-1616">Unterstützung für App-Rollen zu `ad app [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1616">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="5f12f-1617">VM</span><span class="sxs-lookup"><span data-stu-id="5f12f-1617">VM</span></span>

* <span data-ttu-id="5f12f-1618">Problem mit `vm create where ` behoben, aufgrund dessen der beschleunigte Netzwerkbetrieb für Ubuntu 18.0 nicht standardmäßig aktiviert war</span><span class="sxs-lookup"><span data-stu-id="5f12f-1618">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="5f12f-1619">12. Februar 2019</span><span class="sxs-lookup"><span data-stu-id="5f12f-1619">February 12, 2019</span></span>

<span data-ttu-id="5f12f-1620">Version 2.0.58</span><span class="sxs-lookup"><span data-stu-id="5f12f-1620">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="5f12f-1621">Core</span><span class="sxs-lookup"><span data-stu-id="5f12f-1621">Core</span></span>

* <span data-ttu-id="5f12f-1622">`az --version` zeigt jetzt eine Benachrichtigung an, wenn Sie Pakete haben, für die ein Update verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1622">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="5f12f-1623">Die Regression, dass `--ids` nicht mehr mit JSON-Ausgaben verwendet werden konnte, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1623">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="5f12f-1624">ACR</span><span class="sxs-lookup"><span data-stu-id="5f12f-1624">ACR</span></span>
* <span data-ttu-id="5f12f-1625">[BREAKING CHANGE] Die Befehlsgruppe `acr build-task` wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1625">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="5f12f-1626">[BREAKING CHANGE] Die Optionen `--tag` und `--manifest` wurden aus `acr repository delete` entfernt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1626">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="5f12f-1627">ACS</span><span class="sxs-lookup"><span data-stu-id="5f12f-1627">ACS</span></span>
* <span data-ttu-id="5f12f-1628">Unterstützung für Namen ohne Berücksichtigung von Groß-/Kleinschreibung wurde zu `aks [enable-addons|disable-addons]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1628">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="5f12f-1629">Unterstützung für Azure Active Directory-Aktualisierungsvorgang mithilfe von `aks update-credentials --reset-aad` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1629">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="5f12f-1630">Die Information, dass `--output` für `aks get-credentials` ignoriert wird, wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1630">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="5f12f-1631">AMS</span><span class="sxs-lookup"><span data-stu-id="5f12f-1631">AMS</span></span>
* <span data-ttu-id="5f12f-1632">Befehle vom Typ `ams streaming-endpoint [start | stop | create | update] wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1632">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="5f12f-1633">Befehle vom Typ `ams live-event [create | start | stop | reset] wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1633">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="5f12f-1634">AppService</span><span class="sxs-lookup"><span data-stu-id="5f12f-1634">Appservice</span></span>
* <span data-ttu-id="5f12f-1635">Die Möglichkeit zum Erstellen und Konfigurieren von Funktionen mithilfe von ACR-Containern wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1635">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="5f12f-1636">Unterstützung für das Aktualisieren von Web-App-Konfigurationen über JSON wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1636">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="5f12f-1637">Die Hilfe für `appservice-plan-update` wurde verbessert.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1637">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="5f12f-1638">Unterstützung für App-Erkenntnisse beim Erstellen von Funktions-Apps wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1638">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="5f12f-1639">Probleme mit der Web-App SSH wurden behoben.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1639">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="5f12f-1640">Botservice</span><span class="sxs-lookup"><span data-stu-id="5f12f-1640">Botservice</span></span>
* <span data-ttu-id="5f12f-1641">Die Benutzeroberfläche für `bot publish` wurde verbessert.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1641">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="5f12f-1642">Eine Warnung für Zeitlimit bei der Ausführung von `npm install` während `az bot publish` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1642">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="5f12f-1643">Ungültiges char-Element wurde `.` aus `--name` in `az bot create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1643">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="5f12f-1644">Eine Änderung wurde vorgenommen, um die zufällige Zuordnung von Ressourcennamen beim Erstellen von Azure Storage-Instanzen, App Service-Plänen, Funktions-/Web-Apps und Application Insights-Instanzen zu verhindern.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1644">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="5f12f-1645">[VERALTET] Argument `--proj-name` zugunsten von `--proj-file-path` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-1645">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="5f12f-1646">`az bot publish` wurde geändert, um abgerufene IIS-Bereitstellungsdateien vom Typ „Node.js“ zu entfernen, wenn sie nicht bereits vorhanden waren.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1646">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="5f12f-1647">Das `--keep-node-modules` Argument wurde zu `az bot publish` hinzugefügt, damit der Ordner `node_modules` in App Service nicht gelöscht wird.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1647">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="5f12f-1648">Das Schlüssel-Wert-Paar `"publishCommand"` wurde der Ausgabe von `az bot create` beim Erstellen einer Funktions-App oder eines Web-App-Bots hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1648">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="5f12f-1649">Der Wert von `"publishCommand"` ist ein `az bot publish`-Befehl, der bereits die erforderlichen Parameter zum Veröffentlichen des neu erstellten Bots enthält.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1649">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="5f12f-1650">`"WEBSITE_NODE_DEFAULT_VERSION"` in der ARM-Vorlage wurde so aktualisiert, dass v4-SDK-Bots 10.14.1 anstelle von 8.9.4 verwenden.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1650">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="5f12f-1651">Key Vault</span><span class="sxs-lookup"><span data-stu-id="5f12f-1651">Key Vault</span></span>
* <span data-ttu-id="5f12f-1652">Ein Problem mit `keyvault secret backup` wurde behoben, aufgrund dessen einige Benutzer bei Verwendung von `--id` einen `unexpected_keyword`-Fehler erhielten.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1652">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="5f12f-1653">Überwachen</span><span class="sxs-lookup"><span data-stu-id="5f12f-1653">Monitor</span></span>
* <span data-ttu-id="5f12f-1654">`monitor metrics alert [create|update]` wurde so geändert, dass der Dimensionswert `*` zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1654">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="5f12f-1655">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="5f12f-1655">Network</span></span>
* <span data-ttu-id="5f12f-1656">`dns zone export` wurde geändert, um sicherzustellen, dass es sich bei exportierten CNAMEs um FQDNs handelt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1656">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="5f12f-1657">Parameter `--gateway-name` wurde zu `nic ip-config address-pool [add|remove]` hinzugefügt, um Back-End-Adresspools von Anwendungsgateways zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1657">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="5f12f-1658">Argumente `--traffic-analytics` und `--workspace` wurden zu `network watcher flow-log configure` hinzugefügt, um Datenverkehrsanalysen über einen Log Analytics-Arbeitsbereich zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1658">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="5f12f-1659">`--idle-timeout` und `--floating-ip` wurden zu `lb inbound-nat-pool [create|update]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1659">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="5f12f-1660">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="5f12f-1660">Policy Insights</span></span>
* <span data-ttu-id="5f12f-1661">`policy remediation`-Befehle wurden hinzugefügt, um Korrekturfunktionen der Ressourcenrichtlinie zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1661">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="5f12f-1662">RDBMS</span><span class="sxs-lookup"><span data-stu-id="5f12f-1662">RDBMS</span></span>
* <span data-ttu-id="5f12f-1663">Hilfemeldung und Befehlsparameter wurden verbessert.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1663">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="5f12f-1664">Redis</span><span class="sxs-lookup"><span data-stu-id="5f12f-1664">Redis</span></span>
* <span data-ttu-id="5f12f-1665">Befehle zum Verwalten von „firewall-rules“ (erstellen, aktualisieren, löschen, anzeigen, auflisten) wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1665">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="5f12f-1666">Befehle zum Verwalten von „server-link“ (erstellen, aktualisieren, löschen, anzeigen, auflisten) wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1666">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="5f12f-1667">Befehle zum Verwalten von „patch-schedule“ (erstellen, aktualisieren, löschen, anzeigen, auflisten) wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1667">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="5f12f-1668">Unterstützung für Verfügbarkeitszonen und TLS-Mindestversion wurden zu „redis create“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1668">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="5f12f-1669">[BREAKING CHANGE] Befehle `redis update-settings` und `redis list-all` wurden entfernt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1669">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="5f12f-1670">[BREAKING CHANGE] Parameter für `redis create`: „Mandanteneinstellungen“ werden im Format „Schlüssel[=Wert] nicht akzeptiert.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1670">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="5f12f-1671">[VERALTET] Warnmeldung zur Markierung des Befehls `redis import-method` als veraltet hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1671">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="5f12f-1672">Role</span><span class="sxs-lookup"><span data-stu-id="5f12f-1672">Role</span></span>
* <span data-ttu-id="5f12f-1673">[BREAKING CHANGE] Befehl `az identity` wurde aus den `vm`-Befehlen hierher verschoben.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1673">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="5f12f-1674">SQL-VM</span><span class="sxs-lookup"><span data-stu-id="5f12f-1674">SQL VM</span></span>
* <span data-ttu-id="5f12f-1675">[VERALTET] Argument `--boostrap-acc-pwd` aufgrund eines Tippfehlers als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-1675">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="5f12f-1676">VM</span><span class="sxs-lookup"><span data-stu-id="5f12f-1676">VM</span></span>
* <span data-ttu-id="5f12f-1677">`vm list-skus` wurde so geändert, dass `--all` anstelle von `--all true` verwendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1677">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="5f12f-1678">`vmss run-command [invoke | list | show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1678">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="5f12f-1679">Ein Fehler wurde behoben, aufgrund dessen bei der Ausführung von `vmss encryption enable` bisher ein Fehler auftrat.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1679">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="5f12f-1680">[BREAKING CHANGE] Die Befehle vom Typ `az identity` wurden zu `role`-Befehlen verschoben.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1680">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="5f12f-1681">31. Januar 2019</span><span class="sxs-lookup"><span data-stu-id="5f12f-1681">January 31, 2019</span></span>

<span data-ttu-id="5f12f-1682">Version 2.0.57</span><span class="sxs-lookup"><span data-stu-id="5f12f-1682">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="5f12f-1683">Core</span><span class="sxs-lookup"><span data-stu-id="5f12f-1683">Core</span></span>

* <span data-ttu-id="5f12f-1684">Hotfix für [Problem 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="5f12f-1684">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="5f12f-1685">28. Januar 2019</span><span class="sxs-lookup"><span data-stu-id="5f12f-1685">January 28, 2019</span></span>

<span data-ttu-id="5f12f-1686">Version 2.0.56</span><span class="sxs-lookup"><span data-stu-id="5f12f-1686">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="5f12f-1687">ACR</span><span class="sxs-lookup"><span data-stu-id="5f12f-1687">ACR</span></span>
* <span data-ttu-id="5f12f-1688">Unterstützung für VNet/IP-Regeln wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1688">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="5f12f-1689">ACS</span><span class="sxs-lookup"><span data-stu-id="5f12f-1689">ACS</span></span>
* <span data-ttu-id="5f12f-1690">Virtuelle Knoten (Vorschau) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1690">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="5f12f-1691">Verwaltete OpenShift-Befehle wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1691">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="5f12f-1692">Unterstützung für den Dienstprinzipal-Updatevorgang mit `aks update-credentials -reset-service-principal` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1692">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="5f12f-1693">AMS</span><span class="sxs-lookup"><span data-stu-id="5f12f-1693">AMS</span></span>
* <span data-ttu-id="5f12f-1694">[BREAKING CHANGE]`ams asset get-streaming-locators` in `ams asset list-streaming-locators` umbenannt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1694">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="5f12f-1695">[BREAKING CHANGE]`ams streaming-locator get-content-keys` in `ams streaming-locator list-content-keys` umbenannt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1695">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="5f12f-1696">AppService</span><span class="sxs-lookup"><span data-stu-id="5f12f-1696">Appservice</span></span>
* <span data-ttu-id="5f12f-1697">Unterstützung für App-Erkenntnisse in `functionapp create` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1697">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="5f12f-1698">Unterstützung für die Erstellung von App Service-Plänen (einschließlich Elastic Premium) wurde zu Funktions-Apps hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1698">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="5f12f-1699">Probleme bei einer App-Einstellung mit Elastic Premium-Plänen wurden behoben.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1699">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="5f12f-1700">Container</span><span class="sxs-lookup"><span data-stu-id="5f12f-1700">Container</span></span>
* <span data-ttu-id="5f12f-1701">Befehl `container start` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1701">Added `container start` command</span></span>
* <span data-ttu-id="5f12f-1702">Eine Änderung wurde vorgenommen, um bei der Containererstellung die Verwendung von Dezimalwerten für die CPU zuzulassen.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1702">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="5f12f-1703">EventGrid</span><span class="sxs-lookup"><span data-stu-id="5f12f-1703">EventGrid</span></span>
* <span data-ttu-id="5f12f-1704">Parameter `--deadletter-endpoint` zu `event-subscription [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1704">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="5f12f-1705">„storagequeue“ und „hybridconnection“ wurden als neue Werte für „event-subscription [create|update] --endpoint-type“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1705">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="5f12f-1706">Parameter `--max-delivery-attempts` und `--event-ttl` wurden zu `event-subscription create` hinzugefügt, um die Wiederholungsrichtlinie für Ereignisse anzugeben.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1706">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="5f12f-1707">Eine Warnmeldung wurde zu `event-subscription [create|update]` hinzugefügt, wenn Webhook als Ziel für ein Ereignisabonnement verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1707">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="5f12f-1708">Parameter „source-resource-id“ wurde für alle Befehle im Zusammenhang mit Ereignisabonnements hinzugefügt, und alle anderen Parameter im Zusammenhang mit Quellressourcen wurden als veraltet markiert.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1708">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="5f12f-1709">HDInsight</span><span class="sxs-lookup"><span data-stu-id="5f12f-1709">HDInsight</span></span>
* <span data-ttu-id="5f12f-1710">[BREAKING CHANGE] Die Parameter `--virtual-network` und `--subnet-name` wurden aus `hdinsight [application] create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1710">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="5f12f-1711">[BREAKING CHANGE]`hdinsight create --storage-account` wurde so geändert, dass der Name oder die ID eines Speicherkontos anstellen von Blobendpunkten akzeptiert wird.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1711">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="5f12f-1712">Parameter `--vnet-name` und `--subnet-name` zu `hdinsight create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1712">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="5f12f-1713">Unterstützung für das Enterprise-Sicherheitspaket und Datenträgerverschlüsselung wurde zu `hdinsight create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1713">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="5f12f-1714">Befehl `hdinsight rotate-disk-encryption-key` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1714">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="5f12f-1715">Befehl `hdinsight update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1715">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="5f12f-1716">IoT</span><span class="sxs-lookup"><span data-stu-id="5f12f-1716">IoT</span></span>
* <span data-ttu-id="5f12f-1717">Codierungsformat wurde zu Befehl „routing-endpoint“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1717">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="5f12f-1718">Kusto</span><span class="sxs-lookup"><span data-stu-id="5f12f-1718">Kusto</span></span>
* <span data-ttu-id="5f12f-1719">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="5f12f-1719">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="5f12f-1720">Überwachen</span><span class="sxs-lookup"><span data-stu-id="5f12f-1720">Monitor</span></span>
* <span data-ttu-id="5f12f-1721">ID-Vergleich wurde so geändert, dass Groß-/Kleinschreibung nicht mehr beachtet wird.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1721">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="5f12f-1722">Profil</span><span class="sxs-lookup"><span data-stu-id="5f12f-1722">Profile</span></span>
* <span data-ttu-id="5f12f-1723">Konto auf Mandantenebene für verwaltete Dienstidentität für `login` wird aktiviert.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1723">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="5f12f-1724">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="5f12f-1724">Network</span></span>
* <span data-ttu-id="5f12f-1725">Ein Problem mit `express-route update` wurde behoben, aufgrund dessen das Argument `--bandwidth` ignoriert wurde.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1725">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="5f12f-1726">Ein Problem mit `ddos-protection update` wurde behoben, aufgrund dessen das festgelegte Verständnis zu einer Stapelüberwachung führte.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1726">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="5f12f-1727">Resource</span><span class="sxs-lookup"><span data-stu-id="5f12f-1727">Resource</span></span>
* <span data-ttu-id="5f12f-1728">Unterstützung für die URI-Parameterdatei wurde zu `group deployment create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1728">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="5f12f-1729">Unterstützung für verwaltete Identitäten wurde zu `policy assignment [create|list|show]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1729">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="5f12f-1730">Virtueller SQL-Computer</span><span class="sxs-lookup"><span data-stu-id="5f12f-1730">SQL Virtual Machine</span></span>
* <span data-ttu-id="5f12f-1731">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="5f12f-1731">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="5f12f-1732">Storage</span><span class="sxs-lookup"><span data-stu-id="5f12f-1732">Storage</span></span>
* <span data-ttu-id="5f12f-1733">Eine Lösung wurde so geändert, dass nur Eigenschaften aktualisiert werden, die im selben Objekt geändert werden.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1733">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="5f12f-1734">Nr. 8021 wurde korrigiert, Binärdaten werden bei der Rückgabe in Base64 codiert.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1734">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="5f12f-1735">VM</span><span class="sxs-lookup"><span data-stu-id="5f12f-1735">VM</span></span>
* <span data-ttu-id="5f12f-1736">`vm encryption enable` wurde geändert, um den Schlüsseltresor für die Datenträgerverschlüsselung zu überprüfen und sicherzustellen, dass der Schlüsseltresor für die Schlüsselverschlüsselung vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1736">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="5f12f-1737">Flag `--force` wurde zu `vm encryption enable` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1737">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="5f12f-1738">15. Januar 2019</span><span class="sxs-lookup"><span data-stu-id="5f12f-1738">January 15, 2019</span></span>

<span data-ttu-id="5f12f-1739">Version 2.0.55</span><span class="sxs-lookup"><span data-stu-id="5f12f-1739">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="5f12f-1740">ACR</span><span class="sxs-lookup"><span data-stu-id="5f12f-1740">ACR</span></span>
* <span data-ttu-id="5f12f-1741">Wurde geändert, um den Push eines nicht vorhandenen Helm-Diagramms zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1741">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="5f12f-1742">Wurde geändert, um Laufzeitvorgänge ohne ARM-Anforderungen zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1742">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="5f12f-1743">[VERALTET] Parameter `--resource-group` in folgenden Befehlen als veraltet markiert:</span><span class="sxs-lookup"><span data-stu-id="5f12f-1743">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="5f12f-1744">ACS</span><span class="sxs-lookup"><span data-stu-id="5f12f-1744">ACS</span></span>
* <span data-ttu-id="5f12f-1745">Unterstützung für neue ACI-Regionen wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1745">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="5f12f-1746">AppService</span><span class="sxs-lookup"><span data-stu-id="5f12f-1746">Appservice</span></span>
* <span data-ttu-id="5f12f-1747">Ein Problem beim Hochladen von Zertifikaten für in einer ASE gehostete Apps wurde behoben, aufgrund dessen die AS-RG und die App-RG nicht übereinstimmten.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1747">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="5f12f-1748">`webapp up` wurde geändert, sodass SKU P1V1 als Standard für Linux verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1748">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="5f12f-1749">`[webapp|functionapp] deployment source config-zip` wurde korrigiert, sodass beim Fehlschlagen einer Bereitstellung die richtige Fehlermeldung angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1749">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="5f12f-1750">Befehl `webapp ssh` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1750">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="5f12f-1751">Botservice</span><span class="sxs-lookup"><span data-stu-id="5f12f-1751">Botservice</span></span>
* <span data-ttu-id="5f12f-1752">Aktualisierungen des Bereitstellungsstatus wurden zu `bot create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1752">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="5f12f-1753">Konfigurieren</span><span class="sxs-lookup"><span data-stu-id="5f12f-1753">Configure</span></span>
* <span data-ttu-id="5f12f-1754">`none` wurde als konfigurierbares Ausgabeformat hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1754">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="5f12f-1755">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="5f12f-1755">CosmosDB</span></span>
* <span data-ttu-id="5f12f-1756">Unterstützung für das Erstellen einer Datenbank mit gemeinsam genutztem Durchsatz wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1756">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="5f12f-1757">HDInsight</span><span class="sxs-lookup"><span data-stu-id="5f12f-1757">HDInsight</span></span>
* <span data-ttu-id="5f12f-1758">Befehle zum Verwalten von Anwendungen wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1758">Added commands for managing applications</span></span>
* <span data-ttu-id="5f12f-1759">Befehle zum Verwalten von Skriptaktionen wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1759">Added commands for managing script actions</span></span>
* <span data-ttu-id="5f12f-1760">Befehle zum Verwalten von der Operations Management Suite (OMS) wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1760">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="5f12f-1761">Unterstützung zum Auflisten der regionalen Nutzung wurde zu `hdinsight list-usage` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1761">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="5f12f-1762">[BREAKING CHANGE] Standardclustertyp wurde aus `hdinsight create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1762">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="5f12f-1763">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="5f12f-1763">Network</span></span>
* <span data-ttu-id="5f12f-1764">Argumente `--custom-headers` und `--status-code-ranges` zu `traffic-manager profile [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1764">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="5f12f-1765">Neue Routingtypen wurden hinzugefügt: Subnetz und MultiValue</span><span class="sxs-lookup"><span data-stu-id="5f12f-1765">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="5f12f-1766">Argumente `--custom-headers` und `--subnets` zu `traffic-manager endpoint [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1766">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="5f12f-1767">Eine Problem wurde behoben, aufgrund dessen die Angabe von `--vnets ""` für `ddos-protection update` einen Fehler verursacht hat.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1767">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="5f12f-1768">Role</span><span class="sxs-lookup"><span data-stu-id="5f12f-1768">Role</span></span>
* <span data-ttu-id="5f12f-1769">[VERALTET] Argument `--password` als veraltet markiert für `create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1769">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="5f12f-1770">Verwenden Sie stattdessen sichere, von der CLI generierte Kennwörter.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1770">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="5f12f-1771">Sicherheit</span><span class="sxs-lookup"><span data-stu-id="5f12f-1771">Security</span></span>
* <span data-ttu-id="5f12f-1772">Erstrelease</span><span class="sxs-lookup"><span data-stu-id="5f12f-1772">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="5f12f-1773">Storage</span><span class="sxs-lookup"><span data-stu-id="5f12f-1773">Storage</span></span>
* <span data-ttu-id="5f12f-1774">[BREAKING CHANGE] Die Standardanzahl von Ergebnissen wurde für `storage [blob|file|container|share] list` in 5.000 geändert.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1774">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="5f12f-1775">Verwenden Sie `--num-results *` für das ursprüngliche Verhalten, alle Ergebnisse zurückzugeben.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1775">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="5f12f-1776">Parameter `--marker` zu `storage [blob|file|container|share] list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1776">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="5f12f-1777">Ein Protokollmarker für die nächste Seite wurde zur STDERR für `storage [blob|file|container|share] list` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1777">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="5f12f-1778">Der Befehl `storage blob service-properties update` mit Unterstützung für statische Websites wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1778">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="5f12f-1779">VM</span><span class="sxs-lookup"><span data-stu-id="5f12f-1779">VM</span></span>
* <span data-ttu-id="5f12f-1780">`vm [disk|unmanaged-disk]` und `vmss disk` wurden geändert, sodass sie konsistentere Parameter enthalten.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1780">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="5f12f-1781">Unterstützung für mandantenübergreifende Imageverweise wurden zu `[vm|vmss] create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1781">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="5f12f-1782">Fehler bei Standardkonfiguration in `vm diagnostics get-default-config --windows-os` wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1782">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="5f12f-1783">Argument `--provision-after-extensions` wurde zu `vmss extension set` hinzugefügt, um zu definieren, welche Erweiterungen vor dem Festlegen der Erweiterung bereitgestellt werden müssen.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1783">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="5f12f-1784">Argument `--replica-count` wurde zu `sig image-version update` hinzugefügt, um die Standardanzahl für die Replikation festzulegen.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1784">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="5f12f-1785">Fehler bei `image create --source` wurde behoben, aufgrund dessen, der Quellbetriebssystem-Datenträger für einen virtuellen Computer mit dem gleichen Namen gehalten wurde, selbst wenn die vollständige Ressourcen-ID angegeben war.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1785">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="5f12f-1786">20. Dezember 2018</span><span class="sxs-lookup"><span data-stu-id="5f12f-1786">December 20, 2018</span></span>

<span data-ttu-id="5f12f-1787">Version 2.0.54</span><span class="sxs-lookup"><span data-stu-id="5f12f-1787">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="5f12f-1788">AppService</span><span class="sxs-lookup"><span data-stu-id="5f12f-1788">Appservice</span></span>
* <span data-ttu-id="5f12f-1789">Problem behoben, bei dem `webapp up` nicht erneut bereitgestellt werden konnte</span><span class="sxs-lookup"><span data-stu-id="5f12f-1789">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="5f12f-1790">Unterstützung für das Auflisten und Wiederherstellen von Web-App-Momentaufnahmen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1790">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="5f12f-1791">Unterstützung für das Flag `--runtime` zu Windows-Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1791">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="5f12f-1792">IoTCentral</span><span class="sxs-lookup"><span data-stu-id="5f12f-1792">IoTCentral</span></span>
* <span data-ttu-id="5f12f-1793">Fehler bei API-Aufruf für update-Befehl behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-1793">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="5f12f-1794">Role</span><span class="sxs-lookup"><span data-stu-id="5f12f-1794">Role</span></span>
* <span data-ttu-id="5f12f-1795">[BREAKING CHANGE]`ad [app|sp] list` geändert, damit standardmäßig nur die ersten 100 Objekte aufgelistet werden</span><span class="sxs-lookup"><span data-stu-id="5f12f-1795">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="5f12f-1796">SQL</span><span class="sxs-lookup"><span data-stu-id="5f12f-1796">SQL</span></span>
* <span data-ttu-id="5f12f-1797">Unterstützung für die benutzerdefinierte Sortierung auf verwalteten Instanzen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1797">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="5f12f-1798">VM</span><span class="sxs-lookup"><span data-stu-id="5f12f-1798">VM</span></span>
* <span data-ttu-id="5f12f-1799">Parameter `---os-type` zu `disk create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1799">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="5f12f-1800">18. Dezember 2018</span><span class="sxs-lookup"><span data-stu-id="5f12f-1800">December 18, 2018</span></span>

<span data-ttu-id="5f12f-1801">Version 2.0.53</span><span class="sxs-lookup"><span data-stu-id="5f12f-1801">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="5f12f-1802">ACR</span><span class="sxs-lookup"><span data-stu-id="5f12f-1802">ACR</span></span>
* <span data-ttu-id="5f12f-1803">Unterstützung für Imageimport aus externen Containerregistrierungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1803">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="5f12f-1804">Tabellenlayout für Aufgabenliste komprimiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-1804">Condensed the table layout for task list</span></span>
* <span data-ttu-id="5f12f-1805">Unterstützung für Azure DevOps-URLs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1805">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="5f12f-1806">ACS</span><span class="sxs-lookup"><span data-stu-id="5f12f-1806">ACS</span></span>
* <span data-ttu-id="5f12f-1807">Virtuelle Knoten (Vorschau) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1807">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="5f12f-1808">„(PREVIEW)“ aus AAD-Argumenten für `aks create` entfernt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1808">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="5f12f-1809">[VERALTET]`az acs`-Befehle als veraltet markiert.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1809">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="5f12f-1810">ACS wird am 31. Januar 2020 eingestellt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1810">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="5f12f-1811">Unterstützung für Netzwerkrichtlinie bei der Erstellung neuer AKS-Cluster hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1811">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="5f12f-1812">Anforderung des Arguments `--nodepool-name` bei nur einem Knotenpool für `aks scale` entfernt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1812">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="5f12f-1813">AppService</span><span class="sxs-lookup"><span data-stu-id="5f12f-1813">Appservice</span></span>
* <span data-ttu-id="5f12f-1814">Problem behoben, bei dem für `webapp config container` der Parameter `--slot` nicht berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="5f12f-1814">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="5f12f-1815">Botservice</span><span class="sxs-lookup"><span data-stu-id="5f12f-1815">Botservice</span></span>
* <span data-ttu-id="5f12f-1816">Unterstützung für Analyse von `.bot`-Dateien beim Aufrufen von `bot show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1816">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="5f12f-1817">Fehler bei der AppInsights-Bereitstellung behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-1817">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="5f12f-1818">Leerzeichenfehler bei Dateipfaden behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-1818">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="5f12f-1819">Kudu-Netzwerkaufrufe reduziert</span><span class="sxs-lookup"><span data-stu-id="5f12f-1819">Reduced Kudu network calls</span></span>
* <span data-ttu-id="5f12f-1820">Allgemeine Verbesserungen bei Befehlen der Benutzeroberfläche durchgeführt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1820">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="5f12f-1821">Nutzung</span><span class="sxs-lookup"><span data-stu-id="5f12f-1821">Consumption</span></span>
* <span data-ttu-id="5f12f-1822">Fehler für Budget-API zum Anzeigen von Benachrichtigungen behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-1822">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="5f12f-1823">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="5f12f-1823">CosmosDB</span></span>
* <span data-ttu-id="5f12f-1824">Unterstützung für die Aktualisierung des Kontos von „Singlemaster“ auf „Multimaster“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1824">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="5f12f-1825">Karten</span><span class="sxs-lookup"><span data-stu-id="5f12f-1825">Maps</span></span>
* <span data-ttu-id="5f12f-1826">Unterstützung für SKU „S1“ für `maps account [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1826">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="5f12f-1827">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="5f12f-1827">Network</span></span>
* <span data-ttu-id="5f12f-1828">Unterstützung für `--format` und `--log-version` für `watcher flow-log configure` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1828">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="5f12f-1829">Problem mit `dns zone update` behoben, bei dem die Verwendung von "" zum Löschen von Auflösungs- und Registrierungs-VNETs nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="5f12f-1829">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="5f12f-1830">Resource</span><span class="sxs-lookup"><span data-stu-id="5f12f-1830">Resource</span></span>
* <span data-ttu-id="5f12f-1831">Verarbeitung des Bereichsparameters für Verwaltungsgruppen in `policy assignment [create|list|delete|show|update]` behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-1831">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="5f12f-1832">Neuen Befehl `resource wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1832">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="5f12f-1833">Storage</span><span class="sxs-lookup"><span data-stu-id="5f12f-1833">Storage</span></span>
*  <span data-ttu-id="5f12f-1834">Möglichkeit zum Aktualisieren der Protokollschemaversion für Speicherdienste in `storage logging update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1834">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="5f12f-1835">VM</span><span class="sxs-lookup"><span data-stu-id="5f12f-1835">VM</span></span>
* <span data-ttu-id="5f12f-1836">Absturz in `vm identity remove` behoben, der aufgetreten ist, wenn der angegebenen VM keine verwalteten Dienstidentitäten zugewiesen waren</span><span class="sxs-lookup"><span data-stu-id="5f12f-1836">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="5f12f-1837">4\. Dezember 2018</span><span class="sxs-lookup"><span data-stu-id="5f12f-1837">December 4, 2018</span></span>

<span data-ttu-id="5f12f-1838">Version 2.0.52</span><span class="sxs-lookup"><span data-stu-id="5f12f-1838">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="5f12f-1839">Core</span><span class="sxs-lookup"><span data-stu-id="5f12f-1839">Core</span></span>
* <span data-ttu-id="5f12f-1840">Unterstützung für mandantenübergreifende Ressourcenbereitstellung für mehrinstanzenfähigen Dienstprinzipal hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1840">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="5f12f-1841">Behebung eines Fehlers, aufgrund dessen IDs, die von einem Befehl mit Ausgabe im TSV-Format weitergeleitet wurden, nicht ordnungsgemäß analysiert wurden</span><span class="sxs-lookup"><span data-stu-id="5f12f-1841">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="5f12f-1842">AppService</span><span class="sxs-lookup"><span data-stu-id="5f12f-1842">Appservice</span></span>
* <span data-ttu-id="5f12f-1843">[VORSCHAU] Befehl `webapp up` hinzugefügt, der Benutzer beim Erstellen und Bereitstellen von Inhalten in Apps unterstützt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1843">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="5f12f-1844">Behebung eines Fehlers in einer containerbasierten Windows-App, der aufgrund einer Back-End-Änderung auftrat</span><span class="sxs-lookup"><span data-stu-id="5f12f-1844">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="5f12f-1845">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="5f12f-1845">Network</span></span>
* <span data-ttu-id="5f12f-1846">Argument `--exclusion` zu `application-gateway waf-config set` hinzugefügt, um WAF-Ausschlüsse zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="5f12f-1846">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="5f12f-1847">Role</span><span class="sxs-lookup"><span data-stu-id="5f12f-1847">Role</span></span>
* <span data-ttu-id="5f12f-1848">Unterstützung für benutzerdefinierte Bezeichner für Kennwortanmeldeinformation hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1848">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="5f12f-1849">VM</span><span class="sxs-lookup"><span data-stu-id="5f12f-1849">VM</span></span>
* <span data-ttu-id="5f12f-1850">[VERALTET] Parameter `vm extension [show|wait] --expand` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-1850">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="5f12f-1851">Parameter `--force` zu `vm restart` hinzugefügt, um nicht reagierende virtuelle Computer erneut bereitzustellen</span><span class="sxs-lookup"><span data-stu-id="5f12f-1851">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="5f12f-1852">`[vm|vmss] create --authentication-type` geändert, um „all“ zu akzeptieren und einen virtuellen Computer mit Kennwort- und SSH-Authentifizierung zu erstellen</span><span class="sxs-lookup"><span data-stu-id="5f12f-1852">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="5f12f-1853">Parameter `image create --os-disk-caching` hinzugefügt, um die Zwischenspeicherung von Betriebssystemdatenträgern für ein Image festzulegen</span><span class="sxs-lookup"><span data-stu-id="5f12f-1853">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="5f12f-1854">20. November 2018</span><span class="sxs-lookup"><span data-stu-id="5f12f-1854">November 20, 2018</span></span>

<span data-ttu-id="5f12f-1855">Version 2.0.51</span><span class="sxs-lookup"><span data-stu-id="5f12f-1855">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="5f12f-1856">Core</span><span class="sxs-lookup"><span data-stu-id="5f12f-1856">Core</span></span>
* <span data-ttu-id="5f12f-1857">MSI-Anmeldung geändert, sodass der Abonnementname nicht in der Identität wiederverwendet wird</span><span class="sxs-lookup"><span data-stu-id="5f12f-1857">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="5f12f-1858">ACR</span><span class="sxs-lookup"><span data-stu-id="5f12f-1858">ACR</span></span>
* <span data-ttu-id="5f12f-1859">Kontexttoken zum Aufgabenschritt hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1859">Added context token to task step</span></span>
* <span data-ttu-id="5f12f-1860">Unterstützung für das Festlegen von Geheimnissen in „acr run“ zum Spiegeln der ACR-Aufgabe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1860">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="5f12f-1861">Unterstützung für `--top` und `--orderby` für die Befehle `show-tags` und `show-manifests` verbessert</span><span class="sxs-lookup"><span data-stu-id="5f12f-1861">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="5f12f-1862">AppService</span><span class="sxs-lookup"><span data-stu-id="5f12f-1862">Appservice</span></span>
* <span data-ttu-id="5f12f-1863">Standardtimeout der ZIP-Bereitstellung für das Abrufen des Status auf fünf Minuten erhöht und Timeout-Eigenschaft zum Anpassen dieses Werts hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1863">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="5f12f-1864">Aktualisierung der standardmäßigen `node_version`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1864">Updated the default `node_version`.</span></span> <span data-ttu-id="5f12f-1865">Während eines Austauschvorgangs mit zwei Phasen werden bei der Austauschaktion zum Zurücksetzen des Slots alle App-Einstellungen und Verbindungszeichenfolgen beibehalten.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1865">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="5f12f-1866">Clientseitige SKU-Überprüfung für die Erstellung eines Linux-App Service-Plans entfernt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1866">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="5f12f-1867">Behebung eines Fehlers beim Abrufen des ZipDeploy-Status</span><span class="sxs-lookup"><span data-stu-id="5f12f-1867">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="5f12f-1868">IotCentral</span><span class="sxs-lookup"><span data-stu-id="5f12f-1868">IotCentral</span></span>
* <span data-ttu-id="5f12f-1869">Verfügbarkeitsprüfung für Unterdomänen beim Erstellen einer IoT Central-Anwendung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1869">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="5f12f-1870">KeyVault</span><span class="sxs-lookup"><span data-stu-id="5f12f-1870">KeyVault</span></span>
* <span data-ttu-id="5f12f-1871">Behebung eines Fehlers, aufgrund dessen Fehler mitunter ignoriert wurden</span><span class="sxs-lookup"><span data-stu-id="5f12f-1871">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="5f12f-1872">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="5f12f-1872">Network</span></span>
* <span data-ttu-id="5f12f-1873">`root-cert`-Unterbefehle zum Behandeln von vertrauenswürdigen Stammzertifikaten zu `application-gateway` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1873">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="5f12f-1874">Optionen `--min-capacity` und `--custom-error-pages` zu `application-gateway [create|update]` hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="5f12f-1874">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="5f12f-1875">`--zones` zur Unterstützung von Verfügbarkeitszonen zu `application-gateway create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1875">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="5f12f-1876">Argumente `--file-upload-limit`, `--max-request-body-size` und `--request-body-check` zu `application-gateway waf-config set` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1876">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="5f12f-1877">Rdbms</span><span class="sxs-lookup"><span data-stu-id="5f12f-1877">Rdbms</span></span>
* <span data-ttu-id="5f12f-1878">MariaDB-VNET-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1878">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="5f12f-1879">RBAC</span><span class="sxs-lookup"><span data-stu-id="5f12f-1879">Rbac</span></span>
* <span data-ttu-id="5f12f-1880">Problem beim Aktualisieren unveränderlicher Anmeldeinformationen in `ad app update` behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-1880">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="5f12f-1881">Ausgabewarnungen zur Ankündigung bevorstehender Breaking Changes für `ad [app|sp] list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1881">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="5f12f-1882">Storage</span><span class="sxs-lookup"><span data-stu-id="5f12f-1882">Storage</span></span>
* <span data-ttu-id="5f12f-1883">Behandlung von Ausnahmefällen für Speicherkopierbefehle verbessert</span><span class="sxs-lookup"><span data-stu-id="5f12f-1883">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="5f12f-1884">Problem behoben, aufgrund dessen `storage blob copy start-batch` bei identischen Ziel- und Quellkonten keine Anmeldeinformationen verwendete</span><span class="sxs-lookup"><span data-stu-id="5f12f-1884">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="5f12f-1885">Fehler bei `storage [blob|file] url` behoben, aufgrund dessen `sas_token` nicht in die URL eingebunden wurde</span><span class="sxs-lookup"><span data-stu-id="5f12f-1885">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="5f12f-1886">Breaking Change-Warnung zu `[blob|container] list` hinzugefügt: In Kürze werden standardmäßig nur die ersten 5.000 Ergebnisse ausgegeben.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1886">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="5f12f-1887">VM</span><span class="sxs-lookup"><span data-stu-id="5f12f-1887">VM</span></span>
* <span data-ttu-id="5f12f-1888">Unterstützung für die separate Angabe einer Speicherkonto-SKU für verwaltete Betriebssystemdatenträger und Datenträger zu `[vm|vmss] create --storage-sku` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1888">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="5f12f-1889">Parameter für den Versionsnamen von `sig image-version` in `--image-version -e` geändert</span><span class="sxs-lookup"><span data-stu-id="5f12f-1889">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="5f12f-1890">`sig image-version`-Argument `--image-version-name` als veraltet markiert und durch `--image-version` ersetzt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1890">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="5f12f-1891">Unterstützung für die Verwendung des lokalen Betriebssystemdatenträgers für `[vm|vmss] create --ephemeral-os-disk` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1891">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="5f12f-1892">Unterstützung für `--no-wait` zu `snapshot create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1892">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="5f12f-1893">Befehl `snapshot wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1893">Added `snapshot wait` command</span></span>
* <span data-ttu-id="5f12f-1894">Unterstützung für die Verwendung von Instanznamen mit `[vm|vmss] extension set --extension-instance-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1894">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="5f12f-1895">6\. November 2018</span><span class="sxs-lookup"><span data-stu-id="5f12f-1895">November 6, 2018</span></span>

<span data-ttu-id="5f12f-1896">Version 2.0.50</span><span class="sxs-lookup"><span data-stu-id="5f12f-1896">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="5f12f-1897">Core</span><span class="sxs-lookup"><span data-stu-id="5f12f-1897">Core</span></span>
* <span data-ttu-id="5f12f-1898">Unterstützung für die Dienstprinzipalauthentifizierung (SN und Aussteller) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1898">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="5f12f-1899">ACR</span><span class="sxs-lookup"><span data-stu-id="5f12f-1899">ACR</span></span>
* <span data-ttu-id="5f12f-1900">Unterstützung für Commit- und Pull Request-Git-Ereignisse für Aufgabenquellentrigger hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1900">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="5f12f-1901">Auf Verwendung des Standard-Dockerfiles umgestellt, falls im Erstellungsbefehl kein Dockerfile angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="5f12f-1901">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="5f12f-1902">ACS</span><span class="sxs-lookup"><span data-stu-id="5f12f-1902">ACS</span></span>
* <span data-ttu-id="5f12f-1903">[BREAKING CHANGE]`enable_cloud_console_aks_browse` entfernt, um standardmäßig „az aks browse“ zu aktivieren</span><span class="sxs-lookup"><span data-stu-id="5f12f-1903">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="5f12f-1904">Advisor</span><span class="sxs-lookup"><span data-stu-id="5f12f-1904">Advisor</span></span>
* <span data-ttu-id="5f12f-1905">Allgemein verfügbares Release</span><span class="sxs-lookup"><span data-stu-id="5f12f-1905">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="5f12f-1906">AMS</span><span class="sxs-lookup"><span data-stu-id="5f12f-1906">AMS</span></span>
* <span data-ttu-id="5f12f-1907">Neue Befehlsgruppen hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="5f12f-1907">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="5f12f-1908">Neue Befehle hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="5f12f-1908">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="5f12f-1909">Unterstützung von Verschlüsselungsparametern für `ams streaming-policy create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1909">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="5f12f-1910">Für `ams transform output remove` kann jetzt der zu entfernende Ausgabeindex angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1910">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="5f12f-1911">Argumente `--correlation-data` und `--label` zur Befehlsgruppe `ams job` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1911">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="5f12f-1912">Argumente `--storage-account` und `--container` zur Befehlsgruppe `ams asset` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1912">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="5f12f-1913">Standardwerte für Ablaufzeit (aktueller Zeitpunkt + 23 Std.) und Berechtigungen (Lesen) im Befehl `ams asset get-sas-url` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1913">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="5f12f-1914">[BREAKING CHANGE] Befehl `ams streaming locator` durch `ams streaming-locator` ersetzt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1914">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="5f12f-1915">[BREAKING CHANGE] Argument `--content-keys` von `ams streaming locator` aktualisiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-1915">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="5f12f-1916">[BREAKING CHANGE]`--content-policy-name` im Befehl `ams streaming locator` in `--content-key-policy-name` umbenannt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1916">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="5f12f-1917">[BREAKING CHANGE] Befehl `ams streaming policy` durch `ams streaming-policy` ersetzt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1917">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="5f12f-1918">[BREAKING CHANGE] Das Argument `--preset-names` wurde in der Befehlsgruppe `--preset` durch `ams transform` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1918">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="5f12f-1919">Ab sofort kann nur noch eine einzelne Ausgabe/Voreinstellung festgelegt werden. (Wenn Sie weitere hinzufügen möchten, müssen Sie `ams transform output add` ausführen.)</span><span class="sxs-lookup"><span data-stu-id="5f12f-1919">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="5f12f-1920">Darüber hinaus können Sie eine benutzerdefinierte Voreinstellung für den Standard-Encoder (StandardEncoderPreset) festlegen, indem Sie den Pfad an Ihr benutzerdefiniertes JSON-Objekt übergeben.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1920">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="5f12f-1921">[BREAKING CHANGE]`--output-asset-names ` wurde im Befehl `ams job start` in `--output-assets` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1921">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="5f12f-1922">Ab sofort wird eine durch Leerzeichen getrennte Ressourcenliste im Format „assetName=Bezeichnung“ akzeptiert.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1922">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="5f12f-1923">Ressourcen ohne Bezeichnung können wie folgt gesendet werden: „assetName=“.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1923">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="5f12f-1924">AppService</span><span class="sxs-lookup"><span data-stu-id="5f12f-1924">AppService</span></span>
* <span data-ttu-id="5f12f-1925">Fehler in `az webapp config backup update` behoben, der dazu führte, dass kein Sicherungszeitplan festgelegt werden konnte, wenn noch keiner festgelegt war</span><span class="sxs-lookup"><span data-stu-id="5f12f-1925">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="5f12f-1926">Konfigurieren</span><span class="sxs-lookup"><span data-stu-id="5f12f-1926">Configure</span></span>
* <span data-ttu-id="5f12f-1927">YAML zu Ausgabeformatoptionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1927">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="5f12f-1928">Container</span><span class="sxs-lookup"><span data-stu-id="5f12f-1928">Container</span></span>
* <span data-ttu-id="5f12f-1929">Auf Anzeige der Identität umgestellt, wenn eine Containergruppe nach YAML exportiert wird</span><span class="sxs-lookup"><span data-stu-id="5f12f-1929">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="5f12f-1930">EventHub</span><span class="sxs-lookup"><span data-stu-id="5f12f-1930">EventHub</span></span>
* <span data-ttu-id="5f12f-1931">Flag `--enable-kafka` hinzugefügt, um Kafka in `eventhub namespace [create|update]` zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="5f12f-1931">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="5f12f-1932">Interactive</span><span class="sxs-lookup"><span data-stu-id="5f12f-1932">Interactive</span></span>
* <span data-ttu-id="5f12f-1933">Interactive installiert nun die Erweiterung `interactive`, um schnellere Updates und schnelleren Support zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="5f12f-1933">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="5f12f-1934">Überwachen</span><span class="sxs-lookup"><span data-stu-id="5f12f-1934">Monitor</span></span>
* <span data-ttu-id="5f12f-1935">Unterstützung für Metriknamen mit Schrägstrichen und Punkten zu `--condition` in `monitor metrics alert [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1935">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="5f12f-1936">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="5f12f-1936">Network</span></span>
* <span data-ttu-id="5f12f-1937">Befehlsnamen vom Typ `network interface-endpoint` zugunsten von `network private-endpoint` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-1937">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="5f12f-1938">Problem behoben, das dazu führte, dass das Argument `--peer-circuit` in `express-route peering connection create` keine ID akzeptiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-1938">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="5f12f-1939">Problem behoben, das dazu führte, dass `--ip-tags` mit `public-ip create` nicht ordnungsgemäß funktioniert</span><span class="sxs-lookup"><span data-stu-id="5f12f-1939">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="5f12f-1940">Profil</span><span class="sxs-lookup"><span data-stu-id="5f12f-1940">Profile</span></span>
* <span data-ttu-id="5f12f-1941">`--use-cert-sn-issuer` zu `az login` hinzugefügt, um Dienstprinzipalanmeldungen mit automatischem Zertifikatrollover zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="5f12f-1941">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="5f12f-1942">RDBMS</span><span class="sxs-lookup"><span data-stu-id="5f12f-1942">RDBMS</span></span>
* <span data-ttu-id="5f12f-1943">MySQL-Replikatbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1943">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="5f12f-1944">Resource</span><span class="sxs-lookup"><span data-stu-id="5f12f-1944">Resource</span></span>
* <span data-ttu-id="5f12f-1945">Unterstützung für Verwaltungsgruppen und Abonnements zu Befehlen vom Typ `policy definition|set-definition` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1945">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="5f12f-1946">Role</span><span class="sxs-lookup"><span data-stu-id="5f12f-1946">Role</span></span>
* <span data-ttu-id="5f12f-1947">Unterstützung für die API-Berechtigungsverwaltung, den angemeldeten Benutzer und die Verwaltung von Anwendungskennwörtern und Zertifikatanmeldeinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1947">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="5f12f-1948">`ad sp create-for-rbac` geändert, um „displayName“ und Dienstprinzipalname besser unterscheiden zu können</span><span class="sxs-lookup"><span data-stu-id="5f12f-1948">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="5f12f-1949">Unterstützung der Gewährung von Berechtigungen für AAD-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1949">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="5f12f-1950">Storage</span><span class="sxs-lookup"><span data-stu-id="5f12f-1950">Storage</span></span>
* <span data-ttu-id="5f12f-1951">Möglichkeit hinzugefügt, allein mit SAS und Endpunkten (ohne Kontoname oder Schlüssel) eine Verbindung mit Speicherdiensten herzustellen, wie unter `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>` beschrieben</span><span class="sxs-lookup"><span data-stu-id="5f12f-1951">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="5f12f-1952">VM</span><span class="sxs-lookup"><span data-stu-id="5f12f-1952">VM</span></span>
* <span data-ttu-id="5f12f-1953">Argument `storage-sku` zu `image create` hinzugefügt, um das Festlegen des standardmäßigen Speicherkontotyps für das Image zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="5f12f-1953">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="5f12f-1954">Fehler für `vm resize` behoben, durch den die Option `--no-wait` einen Absturz des Befehls verursachte</span><span class="sxs-lookup"><span data-stu-id="5f12f-1954">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="5f12f-1955">Tabellenausgabeformat für `vm encryption show` geändert, um den Status anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="5f12f-1955">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="5f12f-1956">`vm secret format` geändert, um JSON/JSONC-Ausgabe erforderlich zu machen.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1956">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="5f12f-1957">Der Benutzer wird gewarnt, und es wird standardmäßig die JSON-Ausgabe verwendet, wenn ein unzulässiges Ausgabeformat ausgewählt wird.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1957">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="5f12f-1958">Argumentüberprüfung für `vm create --image` verbessert</span><span class="sxs-lookup"><span data-stu-id="5f12f-1958">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="5f12f-1959">23. Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="5f12f-1959">October 23, 2018</span></span>

<span data-ttu-id="5f12f-1960">Version 2.0.49</span><span class="sxs-lookup"><span data-stu-id="5f12f-1960">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="5f12f-1961">Core</span><span class="sxs-lookup"><span data-stu-id="5f12f-1961">Core</span></span>
* <span data-ttu-id="5f12f-1962">Problem mit `--ids` behoben, aufgrund dessen `--subscription` Vorrang vor dem Abonnement in `--ids` hatte</span><span class="sxs-lookup"><span data-stu-id="5f12f-1962">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="5f12f-1963">Ausdrückliche Warnungen hinzugefügt, wenn Parameter durch die Verwendung von `--ids` ignoriert würden</span><span class="sxs-lookup"><span data-stu-id="5f12f-1963">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="5f12f-1964">ACR</span><span class="sxs-lookup"><span data-stu-id="5f12f-1964">ACR</span></span>
* <span data-ttu-id="5f12f-1965">Problem mit der ACR Build-Codierung in Python2 behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-1965">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="5f12f-1966">CDN</span><span class="sxs-lookup"><span data-stu-id="5f12f-1966">CDN</span></span>
* <span data-ttu-id="5f12f-1967">[BREAKING CHANGE] Standardverhalten beim Zwischenspeichern der Abfragezeichenfolge von `cdn endpoint create` so geändert, dass der Standardwert nicht mehr „IgnoreQueryString“ ist.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1967">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="5f12f-1968">Er wird jetzt vom Dienst festgelegt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1968">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="5f12f-1969">Container</span><span class="sxs-lookup"><span data-stu-id="5f12f-1969">Container</span></span>
* <span data-ttu-id="5f12f-1970">`Private` als gültiger Typ für die Übergabe an „--ip-address“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1970">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="5f12f-1971">Geändert, sodass nur eine Subnetz-ID für das Einrichten eines virtuellen Netzwerks für die Containergruppe zulässig ist</span><span class="sxs-lookup"><span data-stu-id="5f12f-1971">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="5f12f-1972">Geändert, sodass das Verwenden eines VNET-Namens oder einer Ressourcen-ID zulässig ist, um die Verwendung von VNETs aus verschiedenen Ressourcengruppen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="5f12f-1972">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="5f12f-1973">`--assign-identity` hinzugefügt, um einer Containergruppe eine MSI-Identität hinzuzufügen</span><span class="sxs-lookup"><span data-stu-id="5f12f-1973">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="5f12f-1974">`--scope` hinzugefügt, um eine Rollenzuweisung für die vom System zugewiesene MSI-Identität zu erstellen</span><span class="sxs-lookup"><span data-stu-id="5f12f-1974">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="5f12f-1975">Warnung hinzugefügt, wenn eine Containergruppe mit einem Image ohne Prozess mit langer Ausführungszeit erstellt wird</span><span class="sxs-lookup"><span data-stu-id="5f12f-1975">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="5f12f-1976">Probleme mit der Tabellenausgabe für Befehle `list` und `show` behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-1976">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="5f12f-1977">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="5f12f-1977">CosmosDB</span></span>
* <span data-ttu-id="5f12f-1978">Unterstützung für `--enable-multiple-write-locations` zu `cosmosdb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1978">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="5f12f-1979">Interactive</span><span class="sxs-lookup"><span data-stu-id="5f12f-1979">Interactive</span></span>
* <span data-ttu-id="5f12f-1980">Geändert, um sicherzustellen, dass der Parameter für globales Abonnement in Parametern angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="5f12f-1980">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="5f12f-1981">IoT Central</span><span class="sxs-lookup"><span data-stu-id="5f12f-1981">IoT Central</span></span>
* <span data-ttu-id="5f12f-1982">Optionen für Vorlagen und Anzeigenamen für die Erstellung von IoT Central-Anwendungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1982">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="5f12f-1983">[BREAKING CHANGE] Unterstützung für F1-SKU entfernt; stattdessen ist die S1-SKU zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="5f12f-1983">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="5f12f-1984">Überwachen</span><span class="sxs-lookup"><span data-stu-id="5f12f-1984">Monitor</span></span>
* <span data-ttu-id="5f12f-1985">Änderungen an `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="5f12f-1985">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="5f12f-1986">Unterstützung für das Auflisten aller Ereignisse auf Abonnementebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1986">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="5f12f-1987">`--offset`-Parameter für das einfachere Erstellen von Zeitabfragen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1987">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="5f12f-1988">Validierung für `--start-time` und `--end-time` verbessert, um die Verwendung von mehr ISO8601-Formate und benutzerfreundlicheren datetime-Formaten zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="5f12f-1988">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="5f12f-1989">`--namespace` als Alias für veraltete Option `--resource-provider` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1989">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="5f12f-1990">`--filters` als veraltet markiert, da vom Dienst ausschließlich Werte mit stark typisierten Optionen unterstützt werden</span><span class="sxs-lookup"><span data-stu-id="5f12f-1990">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="5f12f-1991">Änderungen an `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="5f12f-1991">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="5f12f-1992">`--offset`-Parameter für das einfachere Erstellen von Zeitabfragen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-1992">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="5f12f-1993">Validierung für `--start-time` und `--end-time` verbessert, um die Verwendung von mehr ISO8601-Formate und benutzerfreundlicheren datetime-Formaten zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="5f12f-1993">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="5f12f-1994">Validierung für `--event-hub`- und `--event-hub-rule`-Argumente an `monitor diagnostic-settings create` verbessert</span><span class="sxs-lookup"><span data-stu-id="5f12f-1994">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="5f12f-1995">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="5f12f-1995">Network</span></span>
* <span data-ttu-id="5f12f-1996">`--app-gateway-address-pools`- und `--gateway-name`-Argumente zu `nic create` hinzugefügt, um das Hinzufügen von Back-End-Adresspools für Anwendungsgateways zu einer NIC zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="5f12f-1996">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="5f12f-1997">`--app-gateway-address-pools`- und `--gateway-name`-Argumente zu `nic ip-config create/update` hinzugefügt, um das Hinzufügen von Back-End-Adresspools für Anwendungsgateways zu einer NIC zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="5f12f-1997">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="5f12f-1998">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="5f12f-1998">ServiceBus</span></span>
* <span data-ttu-id="5f12f-1999">Schreibgeschütztes `migration_state`-Element zu „MigrationConfigProperties“ hinzugefügt, um den aktuellen Status der Migration von Service Bus Standard- zu Premium-Namespace anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="5f12f-1999">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="5f12f-2000">SQL</span><span class="sxs-lookup"><span data-stu-id="5f12f-2000">SQL</span></span>
* <span data-ttu-id="5f12f-2001">`sql failover-group create` und `sql failover-group update` korrigiert, damit die Verwendung einer Richtlinie für manuelles Failover möglich ist</span><span class="sxs-lookup"><span data-stu-id="5f12f-2001">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="5f12f-2002">Storage</span><span class="sxs-lookup"><span data-stu-id="5f12f-2002">Storage</span></span>
* <span data-ttu-id="5f12f-2003">Formatierung der `az storage cors list`-Ausgabe korrigiert, sodass alle Elemente den richtigen Dienstschlüssel anzeigen</span><span class="sxs-lookup"><span data-stu-id="5f12f-2003">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="5f12f-2004">`--bypass-immutability-policy`-Parameter für das Löschen von durch Unveränderlichkeitsrichtlinien blockierten Containern hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2004">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="5f12f-2005">VM</span><span class="sxs-lookup"><span data-stu-id="5f12f-2005">VM</span></span>
* <span data-ttu-id="5f12f-2006">Datenträger-Zwischenspeicherungsmodus `None` für Lv/Lv2-Computerserine in `[vm|vmss] create` erzwungen</span><span class="sxs-lookup"><span data-stu-id="5f12f-2006">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="5f12f-2007">Liste der unterstützten Größen für unterstützenden Netzwerkbeschleuniger für `vm create` aktualisiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-2007">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="5f12f-2008">Stark typisierte Argumente für UltraSSD-IOPS und MBit/s-Konfigurationen für `disk create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2008">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="5f12f-2009">16. Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="5f12f-2009">October 16, 2018</span></span>

<span data-ttu-id="5f12f-2010">Version 2.0.48</span><span class="sxs-lookup"><span data-stu-id="5f12f-2010">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="5f12f-2011">VM</span><span class="sxs-lookup"><span data-stu-id="5f12f-2011">VM</span></span>
* <span data-ttu-id="5f12f-2012">SDK-Problem behoben, das ein Fehlschlagen der Homebrew-Installation verursacht hat</span><span class="sxs-lookup"><span data-stu-id="5f12f-2012">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="5f12f-2013">9\. Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="5f12f-2013">October 9, 2018</span></span>

<span data-ttu-id="5f12f-2014">Version 2.0.47</span><span class="sxs-lookup"><span data-stu-id="5f12f-2014">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="5f12f-2015">Core</span><span class="sxs-lookup"><span data-stu-id="5f12f-2015">Core</span></span>
* <span data-ttu-id="5f12f-2016">Verbesserte Fehlerbehandlung für Fehler vom Typ „Ungültige Anforderung“</span><span class="sxs-lookup"><span data-stu-id="5f12f-2016">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="5f12f-2017">ACR</span><span class="sxs-lookup"><span data-stu-id="5f12f-2017">ACR</span></span>
* <span data-ttu-id="5f12f-2018">Unterstützung für ähnliches Tabellenformat wie Helm-Client hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2018">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="5f12f-2019">ACS</span><span class="sxs-lookup"><span data-stu-id="5f12f-2019">ACS</span></span>
* <span data-ttu-id="5f12f-2020">`aks [create|scale] --nodepool-name` zum Konfigurieren des Knotenpoolnamens hinzugefügt, auf 12 Zeichen gekürzt, Standard: nodepool1</span><span class="sxs-lookup"><span data-stu-id="5f12f-2020">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="5f12f-2021">Korrektur, bei der auf „scp“ zurückgegriffen wird, wenn Parimiko nicht funktioniert</span><span class="sxs-lookup"><span data-stu-id="5f12f-2021">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="5f12f-2022">`aks create` geändert, sodass `--aad-tenant-id` nicht mehr erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="5f12f-2022">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="5f12f-2023">Verbesserte Zusammenführung von Kubernetes-Anmeldeinformationen, wenn doppelte Einträge vorhanden sind</span><span class="sxs-lookup"><span data-stu-id="5f12f-2023">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="5f12f-2024">Container</span><span class="sxs-lookup"><span data-stu-id="5f12f-2024">Container</span></span>
* <span data-ttu-id="5f12f-2025">`functionapp create` geändert, sodass das Erstellen eines Linux-Nutzungsplans mit einer bestimmten Runtime unterstützt wird</span><span class="sxs-lookup"><span data-stu-id="5f12f-2025">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="5f12f-2026">[VORSCHAUVERSION] Unterstützung für das Hosten von Web-Apps in Windows-Containern hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2026">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="5f12f-2027">Event Hub</span><span class="sxs-lookup"><span data-stu-id="5f12f-2027">Event Hub</span></span>
* <span data-ttu-id="5f12f-2028">Befehl `eventhub update` korrigiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-2028">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="5f12f-2029">[BREAKING CHANGE]`list`-Befehle geändert, sodass Fehler von Typ „NotFound(404)“ für Ressourcen mit der typische Vorgehensweise behandelt werden, anstatt eine leere Liste anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="5f12f-2029">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="5f12f-2030">Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="5f12f-2030">Extensions</span></span>
* <span data-ttu-id="5f12f-2031">Problem beim Hinzufügen einer Erweiterung behoben, die bereits installiert ist</span><span class="sxs-lookup"><span data-stu-id="5f12f-2031">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="5f12f-2032">HDInsight</span><span class="sxs-lookup"><span data-stu-id="5f12f-2032">HDInsight</span></span>
* <span data-ttu-id="5f12f-2033">Erste Veröffentlichung</span><span class="sxs-lookup"><span data-stu-id="5f12f-2033">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="5f12f-2034">IoT</span><span class="sxs-lookup"><span data-stu-id="5f12f-2034">IoT</span></span>
* <span data-ttu-id="5f12f-2035">Befehl zur Erweiterungsinstallation zu Banner bei der ersten Ausführung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2035">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="5f12f-2036">KeyVault</span><span class="sxs-lookup"><span data-stu-id="5f12f-2036">KeyVault</span></span>
* <span data-ttu-id="5f12f-2037">Geändert, sodass Key Vault-Speicherbefehle auf das aktuelle API-Profil beschränkt sind</span><span class="sxs-lookup"><span data-stu-id="5f12f-2037">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="5f12f-2038">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="5f12f-2038">Network</span></span>
* <span data-ttu-id="5f12f-2039">`network dns zone create` korrigiert: Befehl ist auch erfolgreich, wenn der Benutzer einen Standardspeicherort konfiguriert hat.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2039">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="5f12f-2040">Siehe Nr. 6052</span><span class="sxs-lookup"><span data-stu-id="5f12f-2040">See #6052</span></span>
* <span data-ttu-id="5f12f-2041">`--remote-vnet-id` für `network vnet peering create` eingestellt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2041">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="5f12f-2042">`--remote-vnet` zum `network vnet peering create`-Element hinzugefügt, das einen Namen oder eine ID akzeptiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-2042">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="5f12f-2043">Unterstützung für mehrere Subnetzpräfixe zu `network vnet create` in `--subnet-prefixes` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2043">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="5f12f-2044">Unterstützung für mehrere Subnetzpräfixe zu `network vnet subnet [create|update]` in `--address-prefixes` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2044">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="5f12f-2045">Problem mit `network application-gateway create` behoben, das die Erstellung von Gateways mit der SKU `WAF_v2` oder `Standard_v2` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="5f12f-2045">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="5f12f-2046">`--service-endpoint-policy`-Argument für Benutzerfreundlichkeit zu `network vnet subnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2046">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="5f12f-2047">Role</span><span class="sxs-lookup"><span data-stu-id="5f12f-2047">Role</span></span>
* <span data-ttu-id="5f12f-2048">Unterstützung für das Auflisten von Azure AD-App-Besitzern in `ad app owner` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2048">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="5f12f-2049">Unterstützung für das Auflisten von Azure AD-Dienstprinzipalbesitzern in `ad sp owner` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2049">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="5f12f-2050">Geändert, um sicherzustellen, dass die Erstellungs- und Aktualisierungsbefehle für die Rollendefinition Konfigurationen mit mehreren Berechtigungen akzeptieren</span><span class="sxs-lookup"><span data-stu-id="5f12f-2050">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="5f12f-2051">`ad sp create-for-rbac` geändert, um sicherzustellen, dass der Homepage-URI immer „https“ ist</span><span class="sxs-lookup"><span data-stu-id="5f12f-2051">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="5f12f-2052">Service Bus</span><span class="sxs-lookup"><span data-stu-id="5f12f-2052">Service Bus</span></span>
* <span data-ttu-id="5f12f-2053">[BREAKING CHANGE]`list`-Befehle geändert, sodass Fehler von Typ „NotFound(404)“ für Ressourcen mit der typische Vorgehensweise behandelt werden, anstatt eine leere Liste anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="5f12f-2053">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="5f12f-2054">VM</span><span class="sxs-lookup"><span data-stu-id="5f12f-2054">VM</span></span>
* <span data-ttu-id="5f12f-2055">Leeres `accessSas`-Feld in `disk grant-access` korrigiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-2055">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="5f12f-2056">`vmss create` geändert, sodass ein ausreichend großer Front-End-Portbereich zur Verarbeitung von Überbereitstellung reserviert ist</span><span class="sxs-lookup"><span data-stu-id="5f12f-2056">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="5f12f-2057">Aktualisierungsbefehle für `sig` korrigiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-2057">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="5f12f-2058">`--no-wait`-Unterstützung für die Verwaltung von Imageversionen in `sig` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2058">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="5f12f-2059">`vm list-ip-addresses` geändert, sodass die Verfügbarkeitszone von öffentlichen IP-Adressen angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="5f12f-2059">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="5f12f-2060">`[vm|vmss] disk attach` geändert, sodass die Standard-LUN eines Datenträgers standardmäßig auf die erste verfügbare Stelle festgelegt wird</span><span class="sxs-lookup"><span data-stu-id="5f12f-2060">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="5f12f-2061">21. September 2018</span><span class="sxs-lookup"><span data-stu-id="5f12f-2061">September 21, 2018</span></span>

<span data-ttu-id="5f12f-2062">Version 2.0.46</span><span class="sxs-lookup"><span data-stu-id="5f12f-2062">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="5f12f-2063">ACR</span><span class="sxs-lookup"><span data-stu-id="5f12f-2063">ACR</span></span>
* <span data-ttu-id="5f12f-2064">ACR-Aufgabenbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2064">Added ACR Task commands</span></span>
* <span data-ttu-id="5f12f-2065">Befehl für die Schnellausführung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2065">Added quick run command</span></span>
* <span data-ttu-id="5f12f-2066">`build-task`-Befehlsgruppe als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-2066">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="5f12f-2067">`helm`-Befehlsgruppe hinzugefügt, um die Verwaltung von Helm-Diagrammen mit ACR zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="5f12f-2067">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="5f12f-2068">Unterstützung für idempotentes Erstellen für die verwaltete Registrierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2068">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="5f12f-2069">Formatfreies Flag für die Anzeige von Buildprotokollen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2069">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="5f12f-2070">ACS</span><span class="sxs-lookup"><span data-stu-id="5f12f-2070">ACS</span></span>
* <span data-ttu-id="5f12f-2071">Befehl `install-connector` zum Festlegen des AKS-Master-FQDN geändert</span><span class="sxs-lookup"><span data-stu-id="5f12f-2071">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="5f12f-2072">Erstellen der Rollenzuweisung für „vnet-subnet-id“ (wenn kein Dienstprinzipal angegeben wurde) und „skip-role-assignment“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-2072">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="5f12f-2073">AppService</span><span class="sxs-lookup"><span data-stu-id="5f12f-2073">AppService</span></span>

* <span data-ttu-id="5f12f-2074">Unterstützung für WebJobs-Vorgangsverwaltung hinzugefügt (kontinuierlich/ausgelöst)</span><span class="sxs-lookup"><span data-stu-id="5f12f-2074">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="5f12f-2075">„az webapp config set“ unterstützt die Eigenschaft „--fts-state“; Unterstützung für „az functionapp config set/show“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2075">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="5f12f-2076">Unterstützung für Bring Your Own Storage für Web-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2076">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="5f12f-2077">Unterstützung für das Auflisten und Wiederherstellen gelöschter Web-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2077">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="5f12f-2078">Batch</span><span class="sxs-lookup"><span data-stu-id="5f12f-2078">Batch</span></span>
* <span data-ttu-id="5f12f-2079">Hinzufügen von Aufgaben über `--json-file` geändert, um die AddTaskCollectionParameter-Syntax zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="5f12f-2079">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="5f12f-2080">Dokumentation akzeptierter `--json-file`-Formate aktualisiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-2080">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="5f12f-2081">`--max-tasks-per-node-option` zu `batch pool create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2081">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="5f12f-2082">Verhalten von `batch account` geändert, um das aktuell angemeldete Konto anzuzeigen, wenn keine Optionen angegeben wurden</span><span class="sxs-lookup"><span data-stu-id="5f12f-2082">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="5f12f-2083">Batch KI</span><span class="sxs-lookup"><span data-stu-id="5f12f-2083">Batch AI</span></span> 
* <span data-ttu-id="5f12f-2084">Fehler bei der automatischen Speicherkontoerstellung im Befehl `batchai cluster create` behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-2084">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="5f12f-2085">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="5f12f-2085">Cognitive Services</span></span>
* <span data-ttu-id="5f12f-2086">Vervollständigung für die Argumente `--sku`, `--kind` und `--location` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2086">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="5f12f-2087">Befehl `cognitiveservices account list-usage` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2087">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="5f12f-2088">Befehl `cognitiveservices account list-kinds` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2088">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="5f12f-2089">Befehl `cognitiveservices account list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2089">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="5f12f-2090">`cognitiveservices list` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-2090">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="5f12f-2091">`--name` geändert (ist jetzt optional für `cognitiveservices account list-skus`)</span><span class="sxs-lookup"><span data-stu-id="5f12f-2091">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="5f12f-2092">Container</span><span class="sxs-lookup"><span data-stu-id="5f12f-2092">Container</span></span>
* <span data-ttu-id="5f12f-2093">Möglichkeit zum Neustarten und Beenden einer ausgeführten Containergruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2093">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="5f12f-2094">`--network-profile` zum Übergeben eines Netzwerkprofils hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2094">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="5f12f-2095">`--subnet` und `--vnet_name` hinzugefügt, um das Erstellen von Containergruppen in einem VNET zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="5f12f-2095">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="5f12f-2096">Tabellenausgabe geändert, sodass der Status der Containergruppe angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="5f12f-2096">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="5f12f-2097">Data Lake</span><span class="sxs-lookup"><span data-stu-id="5f12f-2097">Datalake</span></span>
* <span data-ttu-id="5f12f-2098">Befehle für VNET-Regeln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2098">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="5f12f-2099">Interaktive Shell</span><span class="sxs-lookup"><span data-stu-id="5f12f-2099">Interactive Shell</span></span>
* <span data-ttu-id="5f12f-2100">Fehler in Windows behoben, durch den Befehle nicht ordnungsgemäß ausgeführt wurden</span><span class="sxs-lookup"><span data-stu-id="5f12f-2100">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="5f12f-2101">Durch veraltete Objekte verursachtes Problem beim Laden von Befehlen im interaktiven Modus behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-2101">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="5f12f-2102">IoT</span><span class="sxs-lookup"><span data-stu-id="5f12f-2102">IoT</span></span>
* <span data-ttu-id="5f12f-2103">Routingunterstützung für IoT Hubs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2103">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="5f12f-2104">Key Vault</span><span class="sxs-lookup"><span data-stu-id="5f12f-2104">Key Vault</span></span>
* <span data-ttu-id="5f12f-2105">Key Vault-Schlüsselimport für RSA-Schlüssel korrigiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-2105">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="5f12f-2106">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="5f12f-2106">Network</span></span>
* <span data-ttu-id="5f12f-2107">Befehle vom Typ `network public-ip prefix` hinzugefügt, um Präfixe von öffentlichen IP-Adressen zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="5f12f-2107">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="5f12f-2108">Befehle vom Typ `network service-endpoint` hinzugefügt, um Dienstendpunktrichtlinien-Features zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="5f12f-2108">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="5f12f-2109">Befehle vom Typ `network lb outbound-rule` hinzugefügt, um die Erstellung von Ausgangsregeln für Load Balancer Standard zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="5f12f-2109">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="5f12f-2110">`--public-ip-prefix` zu `network lb frontend-ip create/update` hinzugefügt, um Front-End-IP-Konfigurationen mit Präfixen von öffentlichen IP-Adressen zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="5f12f-2110">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="5f12f-2111">`--enable-tcp-reset` zu `network lb rule/inbound-nat-rule/inbound-nat-pool create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2111">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="5f12f-2112">`--disable-outbound-snat` zu `network lb rule create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2112">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="5f12f-2113">Verwendung von `network watcher flow-log show/configure` mit klassischen NSGs ermöglicht</span><span class="sxs-lookup"><span data-stu-id="5f12f-2113">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="5f12f-2114">Hinzufügen des `network watcher run-configuration-diagnostic`-Befehls</span><span class="sxs-lookup"><span data-stu-id="5f12f-2114">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="5f12f-2115">Befehl `network watcher test-connectivity` korrigiert und Eigenschaften `--method`, `--valid-status-codes` und `--headers` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2115">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="5f12f-2116">`network express-route create/update`: Flag `--allow-global-reach` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2116">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="5f12f-2117">`network vnet subnet create/update`: Unterstützung für `--delegation` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2117">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="5f12f-2118">Befehl `network vnet subnet list-available-delegations` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2118">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="5f12f-2119">`network traffic-manager profile create/update`: Unterstützung für `--interval`, `--timeout` und `--max-failures` für die Überwachungskonfiguration hinzugefügt; Optionen `--monitor-path`, `--monitor-port` und `--monitor-protocol` zugunsten von `--path`, `--port` und `--protocol` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-2119">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="5f12f-2120">`network lb frontend-ip create/update`: Logik für das Festlegen der Zuweisungsmethode für private IP-Adressen korrigiert. Bei Angabe einer privaten IP-Adresse ist die Zuweisung statisch. Wird keine private IP-Adresse (oder eine leere Zeichenfolge für die private IP-Adresse) angegeben, erfolgt eine dynamische Zuweisung.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2120">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="5f12f-2121">`dns record-set * create/update`: Unterstützung für `--target-resource` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2121">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="5f12f-2122">Befehle vom Typ `network interface-endpoint` hinzugefügt, um Schnittstellenendpunkt-Objekte abzufragen</span><span class="sxs-lookup"><span data-stu-id="5f12f-2122">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="5f12f-2123">`network profile show/list/delete` für die partielle Verwaltung von Netzwerkprofilen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2123">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="5f12f-2124">Befehle vom Typ `network express-route peering connection` für die Verwaltung von Peeringverbindungen zwischen ExpressRoute-Instanzen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2124">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="5f12f-2125">RDBMS</span><span class="sxs-lookup"><span data-stu-id="5f12f-2125">RDBMS</span></span>
* <span data-ttu-id="5f12f-2126">Unterstützung für den MariaDB-Dienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2126">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="5f12f-2127">Reservierung</span><span class="sxs-lookup"><span data-stu-id="5f12f-2127">Reservation</span></span>
* <span data-ttu-id="5f12f-2128">Cosmos DB im Enumerationstyp für reservierte Ressourcen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2128">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="5f12f-2129">Namenseigenschaft im Patchmodell hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2129">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="5f12f-2130">App-Verwaltung</span><span class="sxs-lookup"><span data-stu-id="5f12f-2130">Manage App</span></span>
* <span data-ttu-id="5f12f-2131">Fehler in `managedapp create --kind MarketPlace` korrigiert, der zum Absturz der Instanzerstellung einer verwalteten Marketplace-App führte</span><span class="sxs-lookup"><span data-stu-id="5f12f-2131">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="5f12f-2132">Befehle vom Typ `feature` geändert, um sie auf unterstützte Profile zu beschränken</span><span class="sxs-lookup"><span data-stu-id="5f12f-2132">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="5f12f-2133">Role</span><span class="sxs-lookup"><span data-stu-id="5f12f-2133">Role</span></span>
* <span data-ttu-id="5f12f-2134">Unterstützung für das Auflisten der Gruppenmitgliedschaften des Benutzers hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2134">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="5f12f-2135">SignalR</span><span class="sxs-lookup"><span data-stu-id="5f12f-2135">SignalR</span></span>
* <span data-ttu-id="5f12f-2136">Erste Version</span><span class="sxs-lookup"><span data-stu-id="5f12f-2136">First release</span></span>

### <a name="storage"></a><span data-ttu-id="5f12f-2137">Storage</span><span class="sxs-lookup"><span data-stu-id="5f12f-2137">Storage</span></span>
* <span data-ttu-id="5f12f-2138">Parameter `--auth-mode login` für die Verwendung der Anmeldeinformationen des Benutzers für die Blob- und Warteschlangenautorisierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2138">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="5f12f-2139">`storage container immutability-policy/legal-hold` für die Verwaltung von unveränderlichem Speicher hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2139">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="5f12f-2140">VM</span><span class="sxs-lookup"><span data-stu-id="5f12f-2140">VM</span></span>
* <span data-ttu-id="5f12f-2141">Problem behoben, das dazu führte, dass die Datei mit dem privaten Schlüssel durch `vm create --generate-ssh-keys` überschrieben wird, wenn die Datei mit dem privaten Schlüssel fehlt (Nr. 4725, 6780)</span><span class="sxs-lookup"><span data-stu-id="5f12f-2141">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="5f12f-2142">Unterstützung für den gemeinsamen Image-Katalog über `az sig` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2142">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="5f12f-2143">28. August 2018</span><span class="sxs-lookup"><span data-stu-id="5f12f-2143">August 28, 2018</span></span>

<span data-ttu-id="5f12f-2144">Version 2.0.45</span><span class="sxs-lookup"><span data-stu-id="5f12f-2144">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="5f12f-2145">Core</span><span class="sxs-lookup"><span data-stu-id="5f12f-2145">Core</span></span>

* <span data-ttu-id="5f12f-2146">Das Problem, aufgrund dessen eine leere Konfigurationsdatei geladen wurde, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2146">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="5f12f-2147">Unterstützung für Profil `2018-03-01-hybrid` für Azure Stack hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2147">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="5f12f-2148">ACR</span><span class="sxs-lookup"><span data-stu-id="5f12f-2148">ACR</span></span>

* <span data-ttu-id="5f12f-2149">Problemumgehung für Laufzeitvorgänge ohne ARM-Anforderungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2149">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="5f12f-2150">Änderung vorgenommen, um im Befehl `build` Versionskontrolldateien (etwa „.git“ und „.gitignore“) standardmäßig aus der TAR-Datei auszuschließen</span><span class="sxs-lookup"><span data-stu-id="5f12f-2150">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="5f12f-2151">ACS</span><span class="sxs-lookup"><span data-stu-id="5f12f-2151">ACS</span></span>

* <span data-ttu-id="5f12f-2152">`aks create` geändert, dass standardmäßig virtuelle Computer vom Typ `Standard_DS2_v2` erstellt werden</span><span class="sxs-lookup"><span data-stu-id="5f12f-2152">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="5f12f-2153">`aks get-credentials` geändert, um nun neue APIs zum Abrufen der Clusteranmeldeinformationen aufzurufen</span><span class="sxs-lookup"><span data-stu-id="5f12f-2153">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="5f12f-2154">AppService</span><span class="sxs-lookup"><span data-stu-id="5f12f-2154">AppService</span></span>

* <span data-ttu-id="5f12f-2155">Unterstützung für CORS in „functionapp“ und „webapp“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2155">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="5f12f-2156">ARM-Tagunterstützung in Erstellungsbefehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2156">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="5f12f-2157">`[webapp|functionapp] identity show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="5f12f-2157">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="5f12f-2158">Backup</span><span class="sxs-lookup"><span data-stu-id="5f12f-2158">Backup</span></span>

* <span data-ttu-id="5f12f-2159">`backup vault backup-properties show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="5f12f-2159">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="5f12f-2160">Botdienst</span><span class="sxs-lookup"><span data-stu-id="5f12f-2160">Bot Service</span></span>

* <span data-ttu-id="5f12f-2161">Anfängliches Release der Botdienst-CLI</span><span class="sxs-lookup"><span data-stu-id="5f12f-2161">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="5f12f-2162">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="5f12f-2162">Cognitive Services</span></span>

* <span data-ttu-id="5f12f-2163">Neuer Parameter `--api-properties,` hinzugefügt, der zum Erstellen einiger Dienste erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="5f12f-2163">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="5f12f-2164">IoT</span><span class="sxs-lookup"><span data-stu-id="5f12f-2164">IoT</span></span>

* <span data-ttu-id="5f12f-2165">Problem mit dem Zuweisen verknüpfter Hubs behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-2165">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="5f12f-2166">Überwachen</span><span class="sxs-lookup"><span data-stu-id="5f12f-2166">Monitor</span></span>

* <span data-ttu-id="5f12f-2167">`monitor metrics alert`-Befehle für Metrikwarnungen nahezu in Echtzeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2167">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="5f12f-2168">`monitor alert`-Befehle als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-2168">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="5f12f-2169">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="5f12f-2169">Network</span></span>

* <span data-ttu-id="5f12f-2170">`network application-gateway ssl-policy predefined show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="5f12f-2170">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="5f12f-2171">Resource</span><span class="sxs-lookup"><span data-stu-id="5f12f-2171">Resource</span></span>

* <span data-ttu-id="5f12f-2172">`provider operation show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="5f12f-2172">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="5f12f-2173">Storage</span><span class="sxs-lookup"><span data-stu-id="5f12f-2173">Storage</span></span>

* <span data-ttu-id="5f12f-2174">`storage share policy show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="5f12f-2174">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="5f12f-2175">VM</span><span class="sxs-lookup"><span data-stu-id="5f12f-2175">VM</span></span>

* <span data-ttu-id="5f12f-2176">`vm/vmss identity show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="5f12f-2176">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="5f12f-2177">`--storage-caching` für `vm create` eingestellt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2177">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="5f12f-2178">14. August 2018</span><span class="sxs-lookup"><span data-stu-id="5f12f-2178">Auguest 14, 2018</span></span>

<span data-ttu-id="5f12f-2179">Version 2.0.44</span><span class="sxs-lookup"><span data-stu-id="5f12f-2179">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="5f12f-2180">Core</span><span class="sxs-lookup"><span data-stu-id="5f12f-2180">Core</span></span>

* <span data-ttu-id="5f12f-2181">Numerische Anzeige in `table`-Ausgabe korrigiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-2181">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="5f12f-2182">YAML-Ausgabeformat hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2182">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="5f12f-2183">Telemetrie</span><span class="sxs-lookup"><span data-stu-id="5f12f-2183">Telemetry</span></span>

* <span data-ttu-id="5f12f-2184">Verbesserte Berichterstellung für Telemetriedaten</span><span class="sxs-lookup"><span data-stu-id="5f12f-2184">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="5f12f-2185">ACR</span><span class="sxs-lookup"><span data-stu-id="5f12f-2185">ACR</span></span>

* <span data-ttu-id="5f12f-2186">Befehle vom Typ `content-trust policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2186">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="5f12f-2187">Problem behoben, aufgrund dessen `.dockerignore` nicht richtig verarbeitet wurde</span><span class="sxs-lookup"><span data-stu-id="5f12f-2187">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="5f12f-2188">ACS</span><span class="sxs-lookup"><span data-stu-id="5f12f-2188">ACS</span></span>

* <span data-ttu-id="5f12f-2189">`az acs/aks install-cli` für die Installation in `%USERPROFILE%\.azure-kubectl` unter Windows geändert</span><span class="sxs-lookup"><span data-stu-id="5f12f-2189">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="5f12f-2190">`az aks install-connector` geändert, um zu ermitteln, ob der Cluster über RBAC verfügt, und um den ACI-Connector entsprechend zu konfigurieren</span><span class="sxs-lookup"><span data-stu-id="5f12f-2190">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="5f12f-2191">Geändert in Rollenzuweisung zum Subnetz bei entsprechender Angabe</span><span class="sxs-lookup"><span data-stu-id="5f12f-2191">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="5f12f-2192">Neue Option zum Überspringen der Rollenzuweisung für Subnetz hinzugefügt, wenn dieses angegeben ist</span><span class="sxs-lookup"><span data-stu-id="5f12f-2192">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="5f12f-2193">Geändert, um Rollenzuweisung zum Subnetz zu überspringen, wenn bereits eine Zuweisung vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="5f12f-2193">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="5f12f-2194">AppService</span><span class="sxs-lookup"><span data-stu-id="5f12f-2194">AppService</span></span>

* <span data-ttu-id="5f12f-2195">Fehler behoben, der das Erstellen einer Funktions-App mithilfe von Speicherkonten in externen Ressourcengruppen verhinderte</span><span class="sxs-lookup"><span data-stu-id="5f12f-2195">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="5f12f-2196">Absturz bei ZIP-Bereitstellung behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-2196">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="5f12f-2197">Batch AI</span><span class="sxs-lookup"><span data-stu-id="5f12f-2197">BatchAI</span></span>

* <span data-ttu-id="5f12f-2198">Protokollierungsausgabe für die automatische Speicherkontoerstellung geändert, sodass nun „Ressourcen*gruppe*“ angegeben wird</span><span class="sxs-lookup"><span data-stu-id="5f12f-2198">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="5f12f-2199">Container</span><span class="sxs-lookup"><span data-stu-id="5f12f-2199">Container</span></span>

* <span data-ttu-id="5f12f-2200">`--secure-environment-variables` zum Übergeben sicherer Umgebungsvariablen an einen Container hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2200">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="5f12f-2201">IoT</span><span class="sxs-lookup"><span data-stu-id="5f12f-2201">IoT</span></span>

* <span data-ttu-id="5f12f-2202">[BREAKING CHANGE] Veraltete Befehle entfernt, die in die IoT-Erweiterung verschoben wurden</span><span class="sxs-lookup"><span data-stu-id="5f12f-2202">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="5f12f-2203">Elemente aktualisiert, um nicht die Domäne `azure-devices.net` anzunehmen</span><span class="sxs-lookup"><span data-stu-id="5f12f-2203">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="5f12f-2204">Iot Central</span><span class="sxs-lookup"><span data-stu-id="5f12f-2204">Iot Central</span></span>

* <span data-ttu-id="5f12f-2205">Erstes Release des IoT Central-Moduls</span><span class="sxs-lookup"><span data-stu-id="5f12f-2205">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="5f12f-2206">KeyVault</span><span class="sxs-lookup"><span data-stu-id="5f12f-2206">KeyVault</span></span>


* <span data-ttu-id="5f12f-2207">Befehle zum Verwalten von Speicherkonten und SAS-Definitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2207">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="5f12f-2208">Befehle für Netzwerkregeln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2208">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="5f12f-2209">Parameter `--id` zu Geheimnis-, Schlüssel- und Zertifikatvorgängen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2209">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="5f12f-2210">Unterstützung für Version mit mehreren APIs zur Schlüsseltresorverwaltung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2210">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="5f12f-2211">Unterstützung für Version mit mehreren APIs zur Schlüsseltresordatenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2211">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="5f12f-2212">Relay</span><span class="sxs-lookup"><span data-stu-id="5f12f-2212">Relay</span></span>

* <span data-ttu-id="5f12f-2213">Erste Veröffentlichung</span><span class="sxs-lookup"><span data-stu-id="5f12f-2213">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="5f12f-2214">Sql</span><span class="sxs-lookup"><span data-stu-id="5f12f-2214">Sql</span></span>

* <span data-ttu-id="5f12f-2215">Befehle vom Typ `sql failover-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2215">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="5f12f-2216">Storage</span><span class="sxs-lookup"><span data-stu-id="5f12f-2216">Storage</span></span>

* <span data-ttu-id="5f12f-2217">[BREAKING CHANGE]`storage account show-usage` geändert, um Parameter `--location` erforderlich zu machen. Auflistung nach Region</span><span class="sxs-lookup"><span data-stu-id="5f12f-2217">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="5f12f-2218">Parameter `--resource-group` geändert, sodass er für `storage account`-Befehle optional ist</span><span class="sxs-lookup"><span data-stu-id="5f12f-2218">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="5f12f-2219">Warnungen vom Typ „Fehler bei Vorbedingung“ für einzelne Fehler in Batch-Befehlen für eine aggregiert Nachricht entfernt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2219">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="5f12f-2220">`[blob|file] delete-batch`-Befehle geändert, sodass kein Array mit Null-Werten mehr ausgegeben wird</span><span class="sxs-lookup"><span data-stu-id="5f12f-2220">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="5f12f-2221">`blob [download|upload|delete-batch]`-Befehle geändert, um SAS-Token aus Container-URL zu lesen</span><span class="sxs-lookup"><span data-stu-id="5f12f-2221">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="5f12f-2222">VM</span><span class="sxs-lookup"><span data-stu-id="5f12f-2222">VM</span></span>

* <span data-ttu-id="5f12f-2223">Allgemeine Filter zu `vm list-skus` für höhere Benutzerfreundlichkeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2223">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="5f12f-2224">31. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="5f12f-2224">July 31, 2018</span></span>

<span data-ttu-id="5f12f-2225">Version 2.0.43</span><span class="sxs-lookup"><span data-stu-id="5f12f-2225">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="5f12f-2226">ACR</span><span class="sxs-lookup"><span data-stu-id="5f12f-2226">ACR</span></span>

* <span data-ttu-id="5f12f-2227">Flag `--with-secure-properties` zum Befehl `acr build-task show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2227">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="5f12f-2228">Befehl `acr build-task update-build` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2228">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="5f12f-2229">ACS</span><span class="sxs-lookup"><span data-stu-id="5f12f-2229">ACS</span></span>

* <span data-ttu-id="5f12f-2230">Änderung, um 0 (Erfolg) zurückzugeben, wenn `az aks browse` durch Drücken von [STRG+C] beendet wird</span><span class="sxs-lookup"><span data-stu-id="5f12f-2230">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="5f12f-2231">Batch</span><span class="sxs-lookup"><span data-stu-id="5f12f-2231">Batch</span></span>

* <span data-ttu-id="5f12f-2232">Korrektur eines Fehlers bei der Anzeige des AAD-Tokens in Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="5f12f-2232">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="5f12f-2233">Container</span><span class="sxs-lookup"><span data-stu-id="5f12f-2233">Container</span></span>

* <span data-ttu-id="5f12f-2234">Voraussetzung von `--log-analytics-workspace-key` für Name oder ID im festgelegten Abonnement entfernt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2234">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="5f12f-2235">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="5f12f-2235">Network</span></span>

* <span data-ttu-id="5f12f-2236">DNS-Unterstützung zu „2017-03-09-profile“ für Azure Stack hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2236">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="5f12f-2237">Resource</span><span class="sxs-lookup"><span data-stu-id="5f12f-2237">Resource</span></span>

* <span data-ttu-id="5f12f-2238">`--rollback-on-error` zu `group deployment create` hinzugefügt, um bei einem Fehler eine als funktionierend bekannte Bereitstellung auszuführen</span><span class="sxs-lookup"><span data-stu-id="5f12f-2238">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="5f12f-2239">Problem behoben, aufgrund dessen `--parameters {}` mit `group deployment create` zu einem Fehler führte</span><span class="sxs-lookup"><span data-stu-id="5f12f-2239">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="5f12f-2240">Role</span><span class="sxs-lookup"><span data-stu-id="5f12f-2240">Role</span></span>

* <span data-ttu-id="5f12f-2241">Unterstützung für das Stack-Profil „2017-03-09-profile“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2241">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="5f12f-2242">Problem behoben, aufgrund dessen das generische Update von Parametern auf `app update` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="5f12f-2242">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="5f12f-2243">Suchen,</span><span class="sxs-lookup"><span data-stu-id="5f12f-2243">Search</span></span>

* <span data-ttu-id="5f12f-2244">Befehle für Azure Search-Dienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2244">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="5f12f-2245">Service Bus</span><span class="sxs-lookup"><span data-stu-id="5f12f-2245">Service Bus</span></span>

* <span data-ttu-id="5f12f-2246">Migrationsbefehlsgruppe hinzugefügt, um einen Namespace von Service Bus Standard zu Premium zu migrieren</span><span class="sxs-lookup"><span data-stu-id="5f12f-2246">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="5f12f-2247">Neue optionale Eigenschaften zu Service Bus-Warteschlange und -Abonnement hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2247">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="5f12f-2248">`--enable-batched-operations` und `--enable-dead-lettering-on-message-expiration` in `queue`</span><span class="sxs-lookup"><span data-stu-id="5f12f-2248">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="5f12f-2249">`--dead-letter-on-filter-exceptions` in `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="5f12f-2249">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="5f12f-2250">Storage</span><span class="sxs-lookup"><span data-stu-id="5f12f-2250">Storage</span></span>

* <span data-ttu-id="5f12f-2251">Unterstützung für den Download großer Dateien über eine einzelne Verbindung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2251">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="5f12f-2252">`show`-Befehle konvertiert, bei denen im Falle einer fehlenden Ressource kein Fehler mit dem Exitcode 3 ausgelöst wurde</span><span class="sxs-lookup"><span data-stu-id="5f12f-2252">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="5f12f-2253">VM</span><span class="sxs-lookup"><span data-stu-id="5f12f-2253">VM</span></span>

* <span data-ttu-id="5f12f-2254">Unterstützung zum Auflisten von Verfügbarkeitsgruppen nach Abonnement hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2254">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="5f12f-2255">Unterstützung für `StandardSSD_LRS` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2255">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="5f12f-2256">Unterstützung für Anwendungssicherheitsgruppe beim Erstellen einer VM-Skalierungsgruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2256">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="5f12f-2257">[BREAKING CHANGE]`[vm|vmss] create`, `[vm|vmss] identity assign` und `[vm|vmss] identity remove` wurden geändert, um vom Benutzer zugewiesene Identitäten im Wörterbuchformat auszugeben.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2257">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="5f12f-2258">18. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="5f12f-2258">July 18, 2018</span></span>

<span data-ttu-id="5f12f-2259">Version 2.0.42</span><span class="sxs-lookup"><span data-stu-id="5f12f-2259">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="5f12f-2260">Core</span><span class="sxs-lookup"><span data-stu-id="5f12f-2260">Core</span></span>

* <span data-ttu-id="5f12f-2261">Unterstützung für browserbasierte Anmeldung WSL-Bash-Fenster hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2261">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="5f12f-2262">`--force-string`-Flag für alle generischen Updatebefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2262">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="5f12f-2263">[BREAKING CHANGE] Befehle vom Typ „show“ so geändert, dass die Fehlermeldung protokolliert wird und der Vorgang bei einer fehlenden Ressource mit dem Exitcode 3 fehlschlägt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2263">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="5f12f-2264">ACR</span><span class="sxs-lookup"><span data-stu-id="5f12f-2264">ACR</span></span>

* <span data-ttu-id="5f12f-2265">[BREAKING CHANGE] „--no-push“ in Befehl „acr build“ in reines Flag geändert</span><span class="sxs-lookup"><span data-stu-id="5f12f-2265">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="5f12f-2266">Befehle `show` und `update` unter Gruppe `acr repository` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2266">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="5f12f-2267">`--detail`-Flag für `show-manifests` und `show-tags` hinzugefügt, um ausführlichere Informationen anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="5f12f-2267">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="5f12f-2268">Parameter `--image` zur Unterstützung des Abrufs von Builddetails oder Protokollen anhand eines Images hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2268">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="5f12f-2269">ACS</span><span class="sxs-lookup"><span data-stu-id="5f12f-2269">ACS</span></span>

* <span data-ttu-id="5f12f-2270">`az aks create` so geändert, dass mit Fehler beendet wird, wenn `--max-pods` kleiner als 5 ist</span><span class="sxs-lookup"><span data-stu-id="5f12f-2270">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="5f12f-2271">AppService</span><span class="sxs-lookup"><span data-stu-id="5f12f-2271">AppService</span></span>

* <span data-ttu-id="5f12f-2272">Unterstützung für PremiumV2-SKUs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2272">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="5f12f-2273">Batch</span><span class="sxs-lookup"><span data-stu-id="5f12f-2273">Batch</span></span>

* <span data-ttu-id="5f12f-2274">Korrektur eines Fehlers bei der Verwendung von Anmeldeinformationen im Cloud Shell-Modus</span><span class="sxs-lookup"><span data-stu-id="5f12f-2274">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="5f12f-2275">JSON-Eingabe so geändert, dass Groß-/Kleinschreibung nicht beachtet wird</span><span class="sxs-lookup"><span data-stu-id="5f12f-2275">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="5f12f-2276">Batch KI</span><span class="sxs-lookup"><span data-stu-id="5f12f-2276">Batch AI</span></span>

* <span data-ttu-id="5f12f-2277">Befehl `az batchai job exec` korrigiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-2277">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="5f12f-2278">Container</span><span class="sxs-lookup"><span data-stu-id="5f12f-2278">Container</span></span>

* <span data-ttu-id="5f12f-2279">Anforderung von Benutzername und Kennwort für Nicht-DockerHub-Registrierungen entfernt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2279">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="5f12f-2280">Fehler beim Erstellen von Containergruppen aus YAML-Datei behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-2280">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="5f12f-2281">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="5f12f-2281">Network</span></span>

* <span data-ttu-id="5f12f-2282">Unterstützung für `--no-wait` zu `network nic [create|update|delete]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2282">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="5f12f-2283">`network nic wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2283">Added `network nic wait`</span></span>
* <span data-ttu-id="5f12f-2284">`--ids`-Argument für `network vnet [subnet|peering] list` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-2284">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="5f12f-2285">`--include-default`-Flag hinzugefügt, um Standardsicherheitsregeln in die Ausgabe von `network nsg rule list` aufzunehmen</span><span class="sxs-lookup"><span data-stu-id="5f12f-2285">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="5f12f-2286">Resource</span><span class="sxs-lookup"><span data-stu-id="5f12f-2286">Resource</span></span>

* <span data-ttu-id="5f12f-2287">Unterstützung für `--no-wait` zu `group deployment delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2287">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="5f12f-2288">Unterstützung für `--no-wait` zu `deployment delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2288">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="5f12f-2289">Befehl `deployment wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2289">Added `deployment wait` command</span></span>
* <span data-ttu-id="5f12f-2290">Problem behoben, aufgrund dessen die `az deployment`-Befehle auf Abonnementebene fälschlicherweise für Profil „2017-03-09-profile“ angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="5f12f-2290">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="5f12f-2291">SQL</span><span class="sxs-lookup"><span data-stu-id="5f12f-2291">SQL</span></span>

* <span data-ttu-id="5f12f-2292">Fehler „Der angegebene Ressourcengruppenname ... entsprach nicht dem Namen in der URL“ beim Angeben des Namens des Pools für elastische Datenbanken für `sql db copy`-und `sql db replica create`-Befehle behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-2292">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="5f12f-2293">Konfigurieren des Standard-SQL Servers durch Ausführen von `az configure --defaults sql-server=<name>` zulässig</span><span class="sxs-lookup"><span data-stu-id="5f12f-2293">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="5f12f-2294">Tabellenformatierer für Befehle `sql server`, `sql server firewall-rule`, `sql list-usages` und `sql show-usage` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2294">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="5f12f-2295">Storage</span><span class="sxs-lookup"><span data-stu-id="5f12f-2295">Storage</span></span>

* <span data-ttu-id="5f12f-2296">`pageRanges`-Eigenschaft zu `storage blob show`-Ausgabe hinzugefügt, die für Seitenblobs ausgefüllt wird</span><span class="sxs-lookup"><span data-stu-id="5f12f-2296">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="5f12f-2297">VM</span><span class="sxs-lookup"><span data-stu-id="5f12f-2297">VM</span></span>

* <span data-ttu-id="5f12f-2298">[BREAKING CHANGE]`vmss create` so geändert, dass `Standard_DS1_v2` als standardmäßige Instanzgröße verwendet wird</span><span class="sxs-lookup"><span data-stu-id="5f12f-2298">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="5f12f-2299">Unterstützung für `--no-wait` zu `vm extension [set|delete]` und `vmss extension [set|delete]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2299">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="5f12f-2300">`vm extension wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2300">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="5f12f-2301">3\. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="5f12f-2301">July 3, 2018</span></span>

<span data-ttu-id="5f12f-2302">Version 2.0.41</span><span class="sxs-lookup"><span data-stu-id="5f12f-2302">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="5f12f-2303">AKS</span><span class="sxs-lookup"><span data-stu-id="5f12f-2303">AKS</span></span>

* <span data-ttu-id="5f12f-2304">Überwachung geändert, sodass Abonnement-ID verwendet wird</span><span class="sxs-lookup"><span data-stu-id="5f12f-2304">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="5f12f-2305">3\. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="5f12f-2305">July 3, 2018</span></span>

<span data-ttu-id="5f12f-2306">Version 2.0.40</span><span class="sxs-lookup"><span data-stu-id="5f12f-2306">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="5f12f-2307">Core</span><span class="sxs-lookup"><span data-stu-id="5f12f-2307">Core</span></span>

* <span data-ttu-id="5f12f-2308">Neuer Autorisierungscode-Flow für interaktive Anmeldung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2308">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="5f12f-2309">ACR</span><span class="sxs-lookup"><span data-stu-id="5f12f-2309">ACR</span></span>

* <span data-ttu-id="5f12f-2310">Abruf-Buildstatus hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2310">Added polling build status</span></span>
* <span data-ttu-id="5f12f-2311">Unterstützung für Enumerationswerte ohne Berücksichtigung von Groß-/Kleinschreibung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2311">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="5f12f-2312">Parameter `--top` und `--orderby` für `show-manifests` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2312">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="5f12f-2313">ACS</span><span class="sxs-lookup"><span data-stu-id="5f12f-2313">ACS</span></span>

* <span data-ttu-id="5f12f-2314">[BREAKING CHANGE] Standardmäßiges Aktivieren der rollenbasierten Zugriffssteuerung für Kubernetes</span><span class="sxs-lookup"><span data-stu-id="5f12f-2314">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="5f12f-2315">Argument `--disable-rbac` hinzugefügt und `--enable-rbac` als veraltet festgelegt, da es nun der Standard ist</span><span class="sxs-lookup"><span data-stu-id="5f12f-2315">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="5f12f-2316">Optionen für Befehl `aks browse` wurden aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2316">Updated options for `aks browse` command.</span></span> <span data-ttu-id="5f12f-2317">Unterstützung für `--listen-port` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2317">Added `--listen-port` support</span></span>
* <span data-ttu-id="5f12f-2318">Standardmäßiges Helm-Diagrammpaket für Befehl `aks install-connector` wurde aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2318">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="5f12f-2319">Verwenden von „virtual-kubelet-for-aks-latest.tgz“</span><span class="sxs-lookup"><span data-stu-id="5f12f-2319">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="5f12f-2320">Befehle `aks enable-addons` und `aks disable-addons` zum Aktualisieren eines vorhandenen Clusters hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2320">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="5f12f-2321">AppService</span><span class="sxs-lookup"><span data-stu-id="5f12f-2321">AppService</span></span>

* <span data-ttu-id="5f12f-2322">Unterstützung für das Deaktivieren der Identität über `webapp identity remove` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2322">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="5f12f-2323">`preview`-Tag für Identitätsfunktion entfernt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2323">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="5f12f-2324">Backup</span><span class="sxs-lookup"><span data-stu-id="5f12f-2324">Backup</span></span>

* <span data-ttu-id="5f12f-2325">Moduldefinition aktualisiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-2325">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="5f12f-2326">Batch AI</span><span class="sxs-lookup"><span data-stu-id="5f12f-2326">BatchAI</span></span>

* <span data-ttu-id="5f12f-2327">Tabellenausgabe für Befehle `batchai cluster node list` und `batchai job node list` korrigiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-2327">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="5f12f-2328">Cloud</span><span class="sxs-lookup"><span data-stu-id="5f12f-2328">Cloud</span></span>

* <span data-ttu-id="5f12f-2329">Serversuffix `acr login` zu Cloudkonfiguration hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2329">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="5f12f-2330">Container</span><span class="sxs-lookup"><span data-stu-id="5f12f-2330">Container</span></span>

* <span data-ttu-id="5f12f-2331">`container create` zu Standard für Vorgang mit langer Ausführungsdauer geändert</span><span class="sxs-lookup"><span data-stu-id="5f12f-2331">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="5f12f-2332">Log Analytics-Parameter `--log-analytics-workspace` und `--log-analytics-workspace-key` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2332">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="5f12f-2333">Parameter `--protocol` zum Festlegen des zu verwendenden Netzwerkprotokolls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2333">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="5f12f-2334">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="5f12f-2334">Extension</span></span>

* <span data-ttu-id="5f12f-2335">`extension list-available` geändert, sodass nur mit der CLI-Version kompatible Erweiterungen angezeigt werden</span><span class="sxs-lookup"><span data-stu-id="5f12f-2335">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="5f12f-2336">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="5f12f-2336">Network</span></span>

* <span data-ttu-id="5f12f-2337">Problem behoben, aufgrund dessen bei Datensatztypen die Groß-/Kleinschreibung beachtet werden musste ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="5f12f-2337">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="5f12f-2338">Rdbms</span><span class="sxs-lookup"><span data-stu-id="5f12f-2338">Rdbms</span></span>

* <span data-ttu-id="5f12f-2339">Befehle vom Typ `[postgres|myql] server vnet-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2339">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="5f12f-2340">Resource</span><span class="sxs-lookup"><span data-stu-id="5f12f-2340">Resource</span></span>

* <span data-ttu-id="5f12f-2341">Neue Vorgangsgruppe `deployment` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2341">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="5f12f-2342">VM</span><span class="sxs-lookup"><span data-stu-id="5f12f-2342">VM</span></span>

* <span data-ttu-id="5f12f-2343">Unterstützung für das Entfernen der vom System zugewiesenen Identität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2343">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="5f12f-2344">25. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="5f12f-2344">June 25, 2018</span></span>

<span data-ttu-id="5f12f-2345">Version 2.0.39</span><span class="sxs-lookup"><span data-stu-id="5f12f-2345">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="5f12f-2346">Befehlszeilenschnittstelle (CLI)</span><span class="sxs-lookup"><span data-stu-id="5f12f-2346">CLI</span></span>

* <span data-ttu-id="5f12f-2347">Dateieinschränkung in MSI-Installer aktualisiert, um Problem mit der Erweiterungsinstallation zu beheben</span><span class="sxs-lookup"><span data-stu-id="5f12f-2347">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="5f12f-2348">19. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="5f12f-2348">June 19, 2018</span></span>

<span data-ttu-id="5f12f-2349">Version 2.0.38</span><span class="sxs-lookup"><span data-stu-id="5f12f-2349">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="5f12f-2350">Core</span><span class="sxs-lookup"><span data-stu-id="5f12f-2350">Core</span></span>

* <span data-ttu-id="5f12f-2351">Globale Unterstützung für `--subscription` zu den meisten Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2351">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="5f12f-2352">ACR</span><span class="sxs-lookup"><span data-stu-id="5f12f-2352">ACR</span></span>

* <span data-ttu-id="5f12f-2353">`azure-storage-blob` als Abhängigkeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2353">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="5f12f-2354">CPU-Standardkonfiguration für `acr build-task create` geändert, sodass zwei Kerne verwendet werden</span><span class="sxs-lookup"><span data-stu-id="5f12f-2354">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="5f12f-2355">ACS</span><span class="sxs-lookup"><span data-stu-id="5f12f-2355">ACS</span></span>

* <span data-ttu-id="5f12f-2356">Optionen des Befehls `aks use-dev-spaces` wurden aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2356">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="5f12f-2357">Unterstützung für `--update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2357">Added `--update` support</span></span>
* <span data-ttu-id="5f12f-2358">`aks get-credentials --admin` geändert, sodass der Benutzerkontext in `$HOME/.kube/config` ersetzt wird</span><span class="sxs-lookup"><span data-stu-id="5f12f-2358">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="5f12f-2359">Schreibgeschützte `nodeResourceGroup`-Eigenschaft in verwalteten Clustern verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="5f12f-2359">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="5f12f-2360">Befehlsfehler `acs browse` korrigiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-2360">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="5f12f-2361">`--connector-name` für `aks install-connector`, `aks upgrade-connector` und `aks remove-connector` als optional festgelegt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2361">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="5f12f-2362">Neue Azure Container Instances-Regionen für `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2362">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="5f12f-2363">Normalisierter Speicherort im Helm-Versionsnamen und Knotenname zu `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2363">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="5f12f-2364">AppService</span><span class="sxs-lookup"><span data-stu-id="5f12f-2364">AppService</span></span>

* <span data-ttu-id="5f12f-2365">Unterstützung für neuere Versionen von „urllib“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2365">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="5f12f-2366">Unterstützung der Verwendung eines App Service-Plans aus externen Ressourcengruppen zu `functionapp create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2366">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="5f12f-2367">Batch</span><span class="sxs-lookup"><span data-stu-id="5f12f-2367">Batch</span></span>

* <span data-ttu-id="5f12f-2368">`azure-batch-extensions`-Abhängigkeit entfernt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2368">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="5f12f-2369">Batch KI</span><span class="sxs-lookup"><span data-stu-id="5f12f-2369">Batch AI</span></span>

* <span data-ttu-id="5f12f-2370">Unterstützung für Arbeitsbereiche wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2370">Added support for workspaces.</span></span> <span data-ttu-id="5f12f-2371">Arbeitsbereiche ermöglichen das Zusammenfassen von Clustern, Dateiservern und Experimenten in Gruppen ohne Beschränkung der Anzahl von Ressourcen, die erstellt werden können.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2371">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="5f12f-2372">Unterstützung für Experimente wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2372">Added support for experiments.</span></span> <span data-ttu-id="5f12f-2373">Experimente ermöglichen das Zusammenfassen von Aufträgen in Sammlungen ohne Beschränkung der Anzahl von erstellten Aufträgen.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2373">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="5f12f-2374">Unterstützung für das Konfigurieren von `/dev/shm` für Aufträge hinzugefügt, die in einem Docker-Container ausgeführt werden</span><span class="sxs-lookup"><span data-stu-id="5f12f-2374">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="5f12f-2375">Die Befehle `batchai cluster node exec` und `batchai job node exec` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2375">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="5f12f-2376">Diese Befehle ermöglichen die Ausführung aller Befehle direkt auf Knoten und bieten Funktionen zur Portweiterleitung.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2376">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="5f12f-2377">Unterstützung für `--ids` zu `batchai`-Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2377">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="5f12f-2378">[BREAKING CHANGE] Alle Cluster und Dateiserver müssen unter Arbeitsbereichen erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2378">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="5f12f-2379">[BREAKING CHANGE] Aufträge müssen unter Experimenten erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2379">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="5f12f-2380">[BREAKING CHANGE]`--nfs-resource-group` wurde aus den Befehlen `cluster create` und `job create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2380">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="5f12f-2381">Geben Sie zum Bereitstellen eines NFS, das einem anderen Arbeitsbereich/einer anderen Ressourcengruppe angehört, die ARM-ID des Dateiservers über die Option `--nfs` an.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2381">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="5f12f-2382">[BREAKING CHANGE]`--cluster-resource-group` wurde aus dem Befehl `job create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2382">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="5f12f-2383">Geben Sie zum Übermitteln eines Auftrags, der einem anderen Arbeitsbereich/einer anderen Ressourcengruppe angehört, die ARM-ID des Clusters über die Option `--cluster` an.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2383">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="5f12f-2384">[BREAKING CHANGE] Attribut `location` wurde aus Aufträgen, Clustern und Dateiservern entfernt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2384">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="5f12f-2385">„Location“ ist jetzt ein Attribut eines Arbeitsbereichs.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2385">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="5f12f-2386">[BREAKING CHANGE]`--location` wurde aus den Befehlen `job create`, `cluster create` und `file-server create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2386">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="5f12f-2387">[BREAKING CHANGE] Namen von Kurzoptionen wurden geändert, um die Schnittstelle konsistenter zu machen:</span><span class="sxs-lookup"><span data-stu-id="5f12f-2387">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="5f12f-2388">[`--config`, `-c`] in [`--config-file`, `-f`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2388">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="5f12f-2389">[`--cluster`, `-r`] in [`--cluster`, `-c`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2389">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="5f12f-2390">[`--cluster`, `-n`] in [`--cluster`, `-c`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2390">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="5f12f-2391">[`--job`, `-n`] in [`--job`, `-j`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2391">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="5f12f-2392">Karten</span><span class="sxs-lookup"><span data-stu-id="5f12f-2392">Maps</span></span>

* <span data-ttu-id="5f12f-2393">[BREAKING CHANGE]`maps account create` wurde so geändert, dass Nutzungsbedingungen entweder durch interaktive Eingabeaufforderung oder `--accept-tos`-Flag akzeptiert werden müssen.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2393">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="5f12f-2394">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="5f12f-2394">Network</span></span>

* <span data-ttu-id="5f12f-2395">Unterstützung für `https` zu `network lb probe create` hinzugefügt [Nr. 6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="5f12f-2395">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="5f12f-2396">Problem behoben, aufgrund dessen die Groß-/Kleinschreibung von `--endpoint-status` berücksichtigt wurde.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2396">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="5f12f-2397">#6502</span><span class="sxs-lookup"><span data-stu-id="5f12f-2397">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="5f12f-2398">Reservations</span><span class="sxs-lookup"><span data-stu-id="5f12f-2398">Reservations</span></span>

* <span data-ttu-id="5f12f-2399">[BREAKING CHANGE] Erforderlicher Parameter `ReservedResourceType` zu `reservations catalog show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2399">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="5f12f-2400">Parameter `Location` zu `reservations catalog show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2400">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="5f12f-2401">[BREAKING CHANGE]`kind` aus `ReservationProperties` entfernt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2401">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="5f12f-2402">[BREAKING CHANGE]`capabilities` wurde in `Catalog` in `sku_properties` umbenannt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2402">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="5f12f-2403">[BREAKING CHANGE] Eigenschaften `size` und `tier` aus `Catalog` entfernt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2403">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="5f12f-2404">Parameter `InstanceFlexibility` zu `reservations reservation update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2404">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="5f12f-2405">Role</span><span class="sxs-lookup"><span data-stu-id="5f12f-2405">Role</span></span>

* <span data-ttu-id="5f12f-2406">Fehlerbehandlung verbessert</span><span class="sxs-lookup"><span data-stu-id="5f12f-2406">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="5f12f-2407">SQL</span><span class="sxs-lookup"><span data-stu-id="5f12f-2407">SQL</span></span>

* <span data-ttu-id="5f12f-2408">Verwirrender Fehler behoben, der beim Ausführen von `az sql db list-editions` für einen Ort auftrat, der für Ihr Abonnement nicht verfügbar ist</span><span class="sxs-lookup"><span data-stu-id="5f12f-2408">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="5f12f-2409">Storage</span><span class="sxs-lookup"><span data-stu-id="5f12f-2409">Storage</span></span>

* <span data-ttu-id="5f12f-2410">Lesbarkeit der Tabellenausgabe für `storage blob download` verbessert</span><span class="sxs-lookup"><span data-stu-id="5f12f-2410">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="5f12f-2411">VM</span><span class="sxs-lookup"><span data-stu-id="5f12f-2411">VM</span></span>

* <span data-ttu-id="5f12f-2412">Verbesserte Einschränkung der VM-Größenüberprüfung für Unterstützung von beschleunigten Netzwerken in `vm create`</span><span class="sxs-lookup"><span data-stu-id="5f12f-2412">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="5f12f-2413">Warnung für `vmss create` hinzugefügt, dass die VM-Standardgröße von `Standard_D1_v2` auf `Standard_DS1_v2` umgestellt wird</span><span class="sxs-lookup"><span data-stu-id="5f12f-2413">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="5f12f-2414">`--force-update` zu `[vm|vmss] extension set` hinzugefügt, um die Erweiterung auch dann zu aktualisieren, wenn die Konfiguration nicht geändert wurde</span><span class="sxs-lookup"><span data-stu-id="5f12f-2414">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="5f12f-2415">13. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="5f12f-2415">June 13, 2018</span></span>

<span data-ttu-id="5f12f-2416">Version 2.0.37</span><span class="sxs-lookup"><span data-stu-id="5f12f-2416">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="5f12f-2417">Core</span><span class="sxs-lookup"><span data-stu-id="5f12f-2417">Core</span></span>

* <span data-ttu-id="5f12f-2418">Verbesserte interaktive Telemetrie</span><span class="sxs-lookup"><span data-stu-id="5f12f-2418">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="5f12f-2419">13. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="5f12f-2419">June 13, 2018</span></span>

<span data-ttu-id="5f12f-2420">Version 2.0.36</span><span class="sxs-lookup"><span data-stu-id="5f12f-2420">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="5f12f-2421">AKS</span><span class="sxs-lookup"><span data-stu-id="5f12f-2421">AKS</span></span>

* <span data-ttu-id="5f12f-2422">Zusätzliche erweiterte Netzwerkoptionen zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2422">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="5f12f-2423">Argumente zu `aks create` zum Aktivieren der Überwachung und HTTP-Routing hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2423">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="5f12f-2424">Argument `--no-ssh-key` zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2424">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="5f12f-2425">Argument `--enable-rbac` zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2425">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="5f12f-2426">[VORSCHAUVERSION] Unterstützung für Azure Active Directory-Authentifizierung zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2426">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="5f12f-2427">AppService</span><span class="sxs-lookup"><span data-stu-id="5f12f-2427">AppService</span></span>

* <span data-ttu-id="5f12f-2428">Problem mit inkompatiblen urllib-Versionen behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-2428">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="5f12f-2429">5\. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="5f12f-2429">June 5, 2018</span></span>

<span data-ttu-id="5f12f-2430">Version 2.0.35</span><span class="sxs-lookup"><span data-stu-id="5f12f-2430">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="5f12f-2431">Interactive</span><span class="sxs-lookup"><span data-stu-id="5f12f-2431">Interactive</span></span>

* <span data-ttu-id="5f12f-2432">Grenzwerte für die Abhängigkeiten des interaktiven Modus hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2432">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="5f12f-2433">5\. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="5f12f-2433">June 5, 2018</span></span>

<span data-ttu-id="5f12f-2434">Version 2.0.34</span><span class="sxs-lookup"><span data-stu-id="5f12f-2434">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="5f12f-2435">Core</span><span class="sxs-lookup"><span data-stu-id="5f12f-2435">Core</span></span>

* <span data-ttu-id="5f12f-2436">Unterstützung für mandantenübergreifende Ressourcenverweise hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2436">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="5f12f-2437">Verbesserte Zuverlässigkeit bei Telemetrieuploads</span><span class="sxs-lookup"><span data-stu-id="5f12f-2437">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="5f12f-2438">ACR</span><span class="sxs-lookup"><span data-stu-id="5f12f-2438">ACR</span></span>

* <span data-ttu-id="5f12f-2439">Unterstützung für VSTS als Remotequellort hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2439">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="5f12f-2440">Befehl `acr import` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2440">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="5f12f-2441">AKS</span><span class="sxs-lookup"><span data-stu-id="5f12f-2441">AKS</span></span>

* <span data-ttu-id="5f12f-2442">`aks get-credentials` wurde geändert, um die Kube-Konfigurationsdatei mit sichereren Dateisystemberechtigungen zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2442">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="5f12f-2443">Batch</span><span class="sxs-lookup"><span data-stu-id="5f12f-2443">Batch</span></span>

* <span data-ttu-id="5f12f-2444">Fehler bei der Formatierung der Poollistentabelle behoben [[Problem 4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="5f12f-2444">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="5f12f-2445">IoT</span><span class="sxs-lookup"><span data-stu-id="5f12f-2445">IOT</span></span>

* <span data-ttu-id="5f12f-2446">Unterstützung für das Erstellen von IoT Hub-Instanzen im Tarif „Basic“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2446">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="5f12f-2447">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="5f12f-2447">Network</span></span>

* <span data-ttu-id="5f12f-2448">`network vnet peering` wurde verbessert.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2448">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="5f12f-2449">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="5f12f-2449">Policy Insights</span></span>

* <span data-ttu-id="5f12f-2450">Erstrelease</span><span class="sxs-lookup"><span data-stu-id="5f12f-2450">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="5f12f-2451">ARM</span><span class="sxs-lookup"><span data-stu-id="5f12f-2451">ARM</span></span>

* <span data-ttu-id="5f12f-2452">Befehle vom Typ `account management-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2452">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="5f12f-2453">SQL</span><span class="sxs-lookup"><span data-stu-id="5f12f-2453">SQL</span></span>

* <span data-ttu-id="5f12f-2454">Neue Befehle für verwaltete Instanzen hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="5f12f-2454">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="5f12f-2455">Neue Befehle für verwaltete Datenbanken hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="5f12f-2455">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="5f12f-2456">Storage</span><span class="sxs-lookup"><span data-stu-id="5f12f-2456">Storage</span></span>

* <span data-ttu-id="5f12f-2457">Zusätzliche MimeTypes für JSON und JavaScript hinzugefügt (abzuleiten aus Dateierweiterungen)</span><span class="sxs-lookup"><span data-stu-id="5f12f-2457">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="5f12f-2458">VM</span><span class="sxs-lookup"><span data-stu-id="5f12f-2458">VM</span></span>

* <span data-ttu-id="5f12f-2459">`vm list-skus` wurde geändert, um feste Spalten zu verwenden und eine Warnung hinzuzufügen, dass `Tier` und `Size` entfernt werden.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2459">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="5f12f-2460">Option `--accelerated-networking` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2460">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="5f12f-2461">`--tags` zu `identity create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2461">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="5f12f-2462">22. Mai 2018</span><span class="sxs-lookup"><span data-stu-id="5f12f-2462">May 22, 2018</span></span>

<span data-ttu-id="5f12f-2463">Version 2.0.33</span><span class="sxs-lookup"><span data-stu-id="5f12f-2463">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="5f12f-2464">Core</span><span class="sxs-lookup"><span data-stu-id="5f12f-2464">Core</span></span>

* <span data-ttu-id="5f12f-2465">Unterstützung für das Erweitern von `@` in Dateinamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2465">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="5f12f-2466">ACS</span><span class="sxs-lookup"><span data-stu-id="5f12f-2466">ACS</span></span>

* <span data-ttu-id="5f12f-2467">Neue Dev Spaces-Befehle `aks use-dev-spaces` und `aks remove-dev-spaces` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2467">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="5f12f-2468">Tippfehler in Hilfemeldung korrigiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-2468">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="5f12f-2469">AppService</span><span class="sxs-lookup"><span data-stu-id="5f12f-2469">AppService</span></span>

* <span data-ttu-id="5f12f-2470">Verbesserte generische Aktualisierungsbefehle</span><span class="sxs-lookup"><span data-stu-id="5f12f-2470">Improved generic update commands</span></span>
* <span data-ttu-id="5f12f-2471">Asynchrone Unterstützung für `webapp deployment source config-zip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2471">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="5f12f-2472">Container</span><span class="sxs-lookup"><span data-stu-id="5f12f-2472">Container</span></span>

* <span data-ttu-id="5f12f-2473">Unterstützung für das Exportieren einer Containergruppe im YAML-Format hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2473">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="5f12f-2474">Unterstützung für die Verwendung einer YAML-Datei zum Erstellen/Aktualisieren einer Containergruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2474">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="5f12f-2475">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="5f12f-2475">Extension</span></span>

* <span data-ttu-id="5f12f-2476">Verbesserte Entfernung von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="5f12f-2476">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="5f12f-2477">Interactive</span><span class="sxs-lookup"><span data-stu-id="5f12f-2477">Interactive</span></span>

* <span data-ttu-id="5f12f-2478">Protokollierung geändert, um Parser für Abschlüsse zu deaktivieren</span><span class="sxs-lookup"><span data-stu-id="5f12f-2478">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="5f12f-2479">Verbesserte Verarbeitung beschädigter Hilfscaches</span><span class="sxs-lookup"><span data-stu-id="5f12f-2479">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="5f12f-2480">KeyVault</span><span class="sxs-lookup"><span data-stu-id="5f12f-2480">KeyVault</span></span>

* <span data-ttu-id="5f12f-2481">keyvault-Befehle wurden korrigiert, damit sie in Cloud Shell oder auf virtuellen Computern mit Identität verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2481">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="5f12f-2482">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="5f12f-2482">Network</span></span>

* <span data-ttu-id="5f12f-2483">Problem behoben, aufgrund dessen `network watcher show-topology` nicht mit einem VNET und/oder Subnetznamen verwendet werden konnte ([#6326](https://github.com/Azure/azure-cli/issues/6326))</span><span class="sxs-lookup"><span data-stu-id="5f12f-2483">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="5f12f-2484">Problem behoben, aufgrund dessen einige `network watcher`-Befehle fälschlicherweise angaben, dass Network Watcher nicht für bestimmte Regionen aktiviert ist ([#6264](https://github.com/Azure/azure-cli/issues/6264))</span><span class="sxs-lookup"><span data-stu-id="5f12f-2484">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="5f12f-2485">SQL</span><span class="sxs-lookup"><span data-stu-id="5f12f-2485">SQL</span></span>

* <span data-ttu-id="5f12f-2486">[BREAKING CHANGE] Von den Befehlen `db` und `dw` zurückgegebene Antwortobjekte geändert:</span><span class="sxs-lookup"><span data-stu-id="5f12f-2486">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="5f12f-2487">Eigenschaft `serviceLevelObjective` in `currentServiceObjectiveName` umbenannt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2487">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="5f12f-2488">Eigenschaften `currentServiceObjectiveId` und `requestedServiceObjectiveId` entfernt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2488">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="5f12f-2489">Eigenschaft `maxSizeBytes` geändert (ist nun keine Zeichenfolge mehr, sondern ein Ganzzahlwert)</span><span class="sxs-lookup"><span data-stu-id="5f12f-2489">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="5f12f-2490">[BREAKING CHANGE] Die folgenden `db`- und `dw`-Eigenschaften wurden geändert und sind jetzt schreibgeschützt:</span><span class="sxs-lookup"><span data-stu-id="5f12f-2490">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="5f12f-2491">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2491">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="5f12f-2492">Verwenden Sie zum Aktualisieren den Parameter `--service-objective`, oder legen Sie die Eigenschaft `sku.name` fest.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2492">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="5f12f-2493">`edition`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2493">`edition`.</span></span> <span data-ttu-id="5f12f-2494">Verwenden Sie zum Aktualisieren den Parameter `--edition`, oder legen Sie die Eigenschaft `sku.tier` fest.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2494">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="5f12f-2495">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2495">`elasticPoolName`.</span></span> <span data-ttu-id="5f12f-2496">Verwenden Sie zum Aktualisieren den Parameter `--elastic-pool`, oder legen Sie die Eigenschaft `elasticPoolId` fest.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2496">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="5f12f-2497">[BREAKING CHANGE] Die folgenden `elastic-pool`-Eigenschaften wurden geändert und sind jetzt schreibgeschützt:</span><span class="sxs-lookup"><span data-stu-id="5f12f-2497">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="5f12f-2498">`edition`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2498">`edition`.</span></span> <span data-ttu-id="5f12f-2499">Verwenden Sie zum Aktualisieren den Parameter `--edition`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2499">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="5f12f-2500">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2500">`dtu`.</span></span> <span data-ttu-id="5f12f-2501">Verwenden Sie zum Aktualisieren den Parameter `--capacity`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2501">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="5f12f-2502">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2502">`databaseDtuMin`.</span></span> <span data-ttu-id="5f12f-2503">Verwenden Sie zum Aktualisieren den Parameter `--db-min-capacity`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2503">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="5f12f-2504">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2504">`databaseDtuMax`.</span></span> <span data-ttu-id="5f12f-2505">Verwenden Sie zum Aktualisieren den Parameter `--db-max-capacity`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2505">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="5f12f-2506">Die Parameter `--family` und `--capacity` wurden zu den `db`-, `dw`- und `elastic-pool`-Befehlen hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2506">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="5f12f-2507">Den `db`-, `dw`- und `elastic-pool`-Befehlen wurden Tabellenformatierer hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2507">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="5f12f-2508">Storage</span><span class="sxs-lookup"><span data-stu-id="5f12f-2508">Storage</span></span>

* <span data-ttu-id="5f12f-2509">Vervollständigung für das Argument `--account-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2509">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="5f12f-2510">Problem mit `storage entity query` behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-2510">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="5f12f-2511">VM</span><span class="sxs-lookup"><span data-stu-id="5f12f-2511">VM</span></span>

* <span data-ttu-id="5f12f-2512">[BREAKING CHANGE]`--write-accelerator` aus `vm create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2512">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="5f12f-2513">Die gleiche Unterstützung kann über `vm update` oder `vm disk attach` erzielt werden.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2513">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="5f12f-2514">Erweiterungsimageabgleich in `[vm|vmss] extension` korrigiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-2514">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="5f12f-2515">`--boot-diagnostics-storage` zu `vm create` zur Erfassung des Startprotokolls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2515">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="5f12f-2516">`--license-type` zu `[vm|vmss] update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2516">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="5f12f-2517">7\. Mai 2018</span><span class="sxs-lookup"><span data-stu-id="5f12f-2517">May 7, 2018</span></span>

<span data-ttu-id="5f12f-2518">Version 2.0.32</span><span class="sxs-lookup"><span data-stu-id="5f12f-2518">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="5f12f-2519">Core</span><span class="sxs-lookup"><span data-stu-id="5f12f-2519">Core</span></span>

* <span data-ttu-id="5f12f-2520">Ein Ausnahmefehler wurde behoben, der beim Abrufen von Geheimnissen aus einem Dienstprinzipalkonto mit Zertifikat auftrat.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2520">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="5f12f-2521">Eingeschränkte Unterstützung für positionelle Argumente hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2521">Added limited support for positional arguments</span></span>
* <span data-ttu-id="5f12f-2522">Problem behoben, aufgrund dessen `--query` nicht mit `--ids` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="5f12f-2522">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="5f12f-2523">#5591</span><span class="sxs-lookup"><span data-stu-id="5f12f-2523">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="5f12f-2524">Pipingszenarien von Befehlen bei Verwendung von `--ids` verbessert</span><span class="sxs-lookup"><span data-stu-id="5f12f-2524">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="5f12f-2525">Unterstützt `-o tsv` mit angegebener Abfrage bzw. `-o json` ohne angegeben Abfrage</span><span class="sxs-lookup"><span data-stu-id="5f12f-2525">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="5f12f-2526">Befehlsvorschläge bei Fehler hinzugefügt, wenn Befehle Tippfehler enthielten</span><span class="sxs-lookup"><span data-stu-id="5f12f-2526">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="5f12f-2527">Fehler bei der Eingabe von `az ''` behandelt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2527">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="5f12f-2528">Unterstützung für benutzerdefinierte Ressourcentypen für Befehlsmodule und -erweiterungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2528">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="5f12f-2529">ACR</span><span class="sxs-lookup"><span data-stu-id="5f12f-2529">ACR</span></span>

* <span data-ttu-id="5f12f-2530">ACR Build-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2530">Added ACR Build commands</span></span>
* <span data-ttu-id="5f12f-2531">Fehlermeldungen vom Typ „Ressource nicht gefunden.“ verbessert</span><span class="sxs-lookup"><span data-stu-id="5f12f-2531">Improved resource not found error messages</span></span>
* <span data-ttu-id="5f12f-2532">Höhere Leistung bei der Ressourcenerstellung und optimierte Fehlerbehandlung</span><span class="sxs-lookup"><span data-stu-id="5f12f-2532">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="5f12f-2533">ACR-Anmeldung bei nicht standardmäßigen Konsolen und WSL optimiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-2533">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="5f12f-2534">Fehlermeldungen zu Repositorybefehlen optimiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-2534">Improved repository commands error messages</span></span>
* <span data-ttu-id="5f12f-2535">Tabellenspalten und -reihenfolge aktualisiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-2535">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="5f12f-2536">ACS</span><span class="sxs-lookup"><span data-stu-id="5f12f-2536">ACS</span></span>

* <span data-ttu-id="5f12f-2537">Warnung hinzugefügt, dass `az aks` eine Vorschauversion des Diensts ist</span><span class="sxs-lookup"><span data-stu-id="5f12f-2537">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="5f12f-2538">Berechtigungsproblem in `aks install-connector` behoben, wenn `--aci-resource-group` nicht angegeben wird</span><span class="sxs-lookup"><span data-stu-id="5f12f-2538">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="5f12f-2539">AMS</span><span class="sxs-lookup"><span data-stu-id="5f12f-2539">AMS</span></span>

* <span data-ttu-id="5f12f-2540">Erste Version: Verwalten von Azure Media Services-Ressourcen</span><span class="sxs-lookup"><span data-stu-id="5f12f-2540">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="5f12f-2541">AppService</span><span class="sxs-lookup"><span data-stu-id="5f12f-2541">Appservice</span></span>

* <span data-ttu-id="5f12f-2542">Ein Problem in `webapp delete` wurde behoben, das bei Angabe von `--slot` auftrat.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2542">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="5f12f-2543">`--runtime-version` aus `webapp auth update` entfernt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2543">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="5f12f-2544">Unterstützung für „min\_tls\_version“ und „https2.0“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2544">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="5f12f-2545">Unterstützung für mehrere Container hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2545">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="5f12f-2546">Batch KI</span><span class="sxs-lookup"><span data-stu-id="5f12f-2546">Batch AI</span></span>

* <span data-ttu-id="5f12f-2547">`batchai create cluster` wurde geändert, um die in der Konfigurationsdatei des Clusters konfigurierte VM-Priorität zu berücksichtigen.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2547">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="5f12f-2548">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="5f12f-2548">Cognitive Services</span></span>

* <span data-ttu-id="5f12f-2549">Tippfehler im Beispiel für `cognitiveservices account create` behoben [Nr. 5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="5f12f-2549">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="5f12f-2550">Nutzung</span><span class="sxs-lookup"><span data-stu-id="5f12f-2550">Consumption</span></span>

* <span data-ttu-id="5f12f-2551">Neue Befehle für Budget-API hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2551">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="5f12f-2552">Container</span><span class="sxs-lookup"><span data-stu-id="5f12f-2552">Container</span></span>

* <span data-ttu-id="5f12f-2553">`--registry-server` muss nicht mehr für `container create` angegeben werden, wenn ein Registrierungsserver im Imagenamen enthalten ist.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2553">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="5f12f-2554">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="5f12f-2554">Cosmos DB</span></span>

* <span data-ttu-id="5f12f-2555">VNET-Unterstützung für Azure CLI eingeführt: Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="5f12f-2555">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="5f12f-2556">DMS</span><span class="sxs-lookup"><span data-stu-id="5f12f-2556">DMS</span></span>

* <span data-ttu-id="5f12f-2557">Erste Version: Die Migration von SQL zu Azure SQL wird nun unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2557">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="5f12f-2558">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="5f12f-2558">Extension</span></span>

* <span data-ttu-id="5f12f-2559">Fehler behoben, aufgrund dessen Erweiterungsmetadaten nicht mehr angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="5f12f-2559">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="5f12f-2560">Interactive</span><span class="sxs-lookup"><span data-stu-id="5f12f-2560">Interactive</span></span>

* <span data-ttu-id="5f12f-2561">Interaktive Vervollständigung funktioniert nun auch mit positionellen Argumenten.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2561">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="5f12f-2562">Benutzerfreundlichere Ausgabe bei der Eingabe von '\'</span><span class="sxs-lookup"><span data-stu-id="5f12f-2562">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="5f12f-2563">Abschlüsse für Parameter ohne Hilfe korrigiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-2563">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="5f12f-2564">Beschreibungen für Befehlsgruppen korrigiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-2564">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="5f12f-2565">Labor</span><span class="sxs-lookup"><span data-stu-id="5f12f-2565">Lab</span></span>

* <span data-ttu-id="5f12f-2566">Regressionen aus Knack-Umwandlung korrigiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-2566">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="5f12f-2567">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="5f12f-2567">Network</span></span>

* <span data-ttu-id="5f12f-2568">[BREAKING CHANGE] Parameter `--ids` entfernt für:</span><span class="sxs-lookup"><span data-stu-id="5f12f-2568">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="5f12f-2569">Profil</span><span class="sxs-lookup"><span data-stu-id="5f12f-2569">Profile</span></span>

* <span data-ttu-id="5f12f-2570">Quellerkennung für `disk create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-2570">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="5f12f-2571">[BREAKING CHANGE]`--msi-port` und `--identity-port` entfernt, da sie nicht mehr verwendet werden</span><span class="sxs-lookup"><span data-stu-id="5f12f-2571">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="5f12f-2572">Tippfehler in kurzer Zusammenfassung für `account get-access-token` korrigiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-2572">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="5f12f-2573">Redis</span><span class="sxs-lookup"><span data-stu-id="5f12f-2573">Redis</span></span>

* <span data-ttu-id="5f12f-2574">`redis patch-schedule patch-schedule show` wurde durch `redis patch-schedule show` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2574">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="5f12f-2575">`redis list-all` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-2575">Deprecated `redis list-all`.</span></span> <span data-ttu-id="5f12f-2576">Diese Funktion wurde in `redis list` integriert.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2576">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="5f12f-2577">`redis import-method` wurde durch `redis import` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2577">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="5f12f-2578">Unterstützung für `--ids` zu verschiedenen Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2578">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="5f12f-2579">Role</span><span class="sxs-lookup"><span data-stu-id="5f12f-2579">Role</span></span>

* <span data-ttu-id="5f12f-2580">[BREAKING CHANGE] Veralteter Befehl `ad sp reset-credentials` entfernt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2580">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="5f12f-2581">Storage</span><span class="sxs-lookup"><span data-stu-id="5f12f-2581">Storage</span></span>

* <span data-ttu-id="5f12f-2582">Zulassen, dass das Ziel-SAS-Token für die Blobkopie auf die Quelle angewendet wird, wenn Quell-SAS und Kontoschlüssel nicht angegeben werden</span><span class="sxs-lookup"><span data-stu-id="5f12f-2582">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="5f12f-2583">Verfügbar gemacht: Socket-Timeout für Blobuploads und -downloads</span><span class="sxs-lookup"><span data-stu-id="5f12f-2583">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="5f12f-2584">Blobnamen, die mit Pfadtrennzeichen beginnen, als relative Pfade behandeln</span><span class="sxs-lookup"><span data-stu-id="5f12f-2584">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="5f12f-2585">Zulassen, dass `storage blob copy --source-sas` mit dem Abfragezeichen „?“ beginnt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2585">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="5f12f-2586">`storage entity query --marker` korrigiert, um Liste von Schlüsselwerten zu akzeptieren</span><span class="sxs-lookup"><span data-stu-id="5f12f-2586">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="5f12f-2587">VM</span><span class="sxs-lookup"><span data-stu-id="5f12f-2587">VM</span></span>

* <span data-ttu-id="5f12f-2588">Ungültige Erkennungslogik für nicht verwalteten Blob-URI korrigiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-2588">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="5f12f-2589">Unterstützung für Datenträgerverschlüsselung ohne vom Benutzer bereitgestellte Dienstprinzipale hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2589">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="5f12f-2590">[BREAKING CHANGE] Verwenden Sie nicht „ManagedIdentityExtension“ des virtuellen Computers für MSI-Unterstützung.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2590">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="5f12f-2591">Unterstützung für Entfernungsrichtlinie zu `vmss` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2591">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="5f12f-2592">[BREAKING CHANGE]`--ids` entfernt aus:</span><span class="sxs-lookup"><span data-stu-id="5f12f-2592">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="5f12f-2593">Unterstützung für Schreibbeschleunigung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2593">Added write accelerator support</span></span>
* <span data-ttu-id="5f12f-2594">`vmss perform-maintenance` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2594">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="5f12f-2595">`vm diagnostics set` korrigiert, um zuverlässig den Betriebssystemtyp des virtuellen Computers zu erkennen</span><span class="sxs-lookup"><span data-stu-id="5f12f-2595">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="5f12f-2596">`vm resize` geändert, um zu überprüfen, ob die angeforderte Größe von der derzeit festgelegten Größe abweicht, und nur bei einer Änderung eine Aktualisierung auszuführen</span><span class="sxs-lookup"><span data-stu-id="5f12f-2596">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="5f12f-2597">10. April 2018</span><span class="sxs-lookup"><span data-stu-id="5f12f-2597">April 10, 2018</span></span>

<span data-ttu-id="5f12f-2598">Version 2.0.31</span><span class="sxs-lookup"><span data-stu-id="5f12f-2598">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="5f12f-2599">ACR</span><span class="sxs-lookup"><span data-stu-id="5f12f-2599">ACR</span></span>

* <span data-ttu-id="5f12f-2600">Verbesserte Fehlerbehandlung für wincred-Fallback</span><span class="sxs-lookup"><span data-stu-id="5f12f-2600">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="5f12f-2601">ACS</span><span class="sxs-lookup"><span data-stu-id="5f12f-2601">ACS</span></span>

* <span data-ttu-id="5f12f-2602">Gültigkeit von per AKS erstellten SPNs in fünf Jahre geändert</span><span class="sxs-lookup"><span data-stu-id="5f12f-2602">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="5f12f-2603">AppService</span><span class="sxs-lookup"><span data-stu-id="5f12f-2603">Appservice</span></span>

* [BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="5f12f-2605">Nicht abgefangene Ausnahme für nicht vorhandene Web-App-Pläne behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-2605">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="5f12f-2606">Batch AI</span><span class="sxs-lookup"><span data-stu-id="5f12f-2606">BatchAI</span></span>

* <span data-ttu-id="5f12f-2607">Unterstützung für API 2018-03-01 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2607">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="5f12f-2608">Bereitstellung auf Auftragsebene</span><span class="sxs-lookup"><span data-stu-id="5f12f-2608">Job level mounting</span></span>
  - <span data-ttu-id="5f12f-2609">Umgebungsvariablen mit Geheimniswerten</span><span class="sxs-lookup"><span data-stu-id="5f12f-2609">Environment variables with secret values</span></span>
  - <span data-ttu-id="5f12f-2610">Einstellungen von Leistungsindikatoren</span><span class="sxs-lookup"><span data-stu-id="5f12f-2610">Performance counters settings</span></span>
  - <span data-ttu-id="5f12f-2611">Berichtstellung für auftragsspezifisches Pfadsegment</span><span class="sxs-lookup"><span data-stu-id="5f12f-2611">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="5f12f-2612">Unterstützung für Unterordner in Listendateien-API</span><span class="sxs-lookup"><span data-stu-id="5f12f-2612">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="5f12f-2613">Berichterstellung zur Nutzung und zu Grenzwerten</span><span class="sxs-lookup"><span data-stu-id="5f12f-2613">Usage and limits reporting</span></span>
  - <span data-ttu-id="5f12f-2614">Zulassen der Angabe des Cachetyps für NFS-Server</span><span class="sxs-lookup"><span data-stu-id="5f12f-2614">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="5f12f-2615">Unterstützung für benutzerdefinierte Images</span><span class="sxs-lookup"><span data-stu-id="5f12f-2615">Support for custom images</span></span>
  - <span data-ttu-id="5f12f-2616">Unterstützung für pyTorch-Toolkit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2616">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="5f12f-2617">Befehl `job wait` hinzugefügt, der das Warten auf die Auftragsfertigstellung ermöglicht und den Code für die Auftragsbeendigung meldet</span><span class="sxs-lookup"><span data-stu-id="5f12f-2617">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="5f12f-2618">Befehl `usage show` hinzugefügt, mit dem die aktuelle Nutzung von Batch KI-Ressourcen und die Grenzwerte für verschiedene Regionen aufgelistet werden</span><span class="sxs-lookup"><span data-stu-id="5f12f-2618">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="5f12f-2619">Nationale Clouds werden unterstützt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2619">National clouds are supported</span></span>
* <span data-ttu-id="5f12f-2620">Befehlszeilenargumente für Aufträge hinzugefügt, um das Bereitstellen von Dateisystemen auf Auftragsebene zusätzlich zu Konfigurationsdateien zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="5f12f-2620">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="5f12f-2621">Weitere Optionen zum Anpassen von Clustern hinzugefügt – VM-Priorität, Subnetz, anfängliche Knotenanzahl für Cluster mit automatischer Skalierung, Angeben eines benutzerdefinierten Images</span><span class="sxs-lookup"><span data-stu-id="5f12f-2621">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="5f12f-2622">Befehlszeilenoption zum Angeben des Cachetyps für NFS mit Verwaltung per Batch KI hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2622">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="5f12f-2623">Angeben der Bereitstellung von Dateisystemen in Konfigurationsdateien vereinfacht.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2623">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="5f12f-2624">Weglassen von Anmeldeinformationen für Azure-Dateifreigaben und Azure-Blobcontainer ist jetzt möglich. Die CLI füllt fehlende Anmeldeinformationen auf, indem der Speicherkontoschlüssel verwendet wird, der über Befehlszeilenparameter oder per Umgebungsvariable angegeben wird, oder der Schlüssel wird über Azure Storage abgefragt (sofern das Speicherkonto zum aktuellen Abonnement gehört).</span><span class="sxs-lookup"><span data-stu-id="5f12f-2624">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="5f12f-2625">Der Befehl zum Streamen von Auftragsdateien wird jetzt automatisch abgeschlossen, nachdem der Auftrag beendet ist (Erfolg, Fehler, Beendigung oder Löschung)</span><span class="sxs-lookup"><span data-stu-id="5f12f-2625">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="5f12f-2626">Verbesserte `table`-Ausgabe für `show`-Vorgänge</span><span class="sxs-lookup"><span data-stu-id="5f12f-2626">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="5f12f-2627">Option `--use-auto-storage` für die Clustererstellung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2627">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="5f12f-2628">Diese Option erleichtert die Verwaltung von Speicherkonten und die Bereitstellung von Azure-Dateifreigaben und Azure-Blobcontainern in Clustern.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2628">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="5f12f-2629">`--generate-ssh-keys` für `cluster create` und `file-server create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2629">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="5f12f-2630">Möglichkeit zum Angeben der Knotensetupaufgabe über die Befehlszeile</span><span class="sxs-lookup"><span data-stu-id="5f12f-2630">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="5f12f-2631">[BREAKING CHANGE] Befehl `job stream-file` und `job list-files` in die Gruppe `job file` verschoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-2631">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="5f12f-2632">[BREAKING CHANGE]`--admin-user-name` im Befehl `file-server create` in `--user-name` umbenannt, um Einheitlichkeit mit dem Befehl `cluster create` zu erzielen</span><span class="sxs-lookup"><span data-stu-id="5f12f-2632">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="5f12f-2633">Abrechnung</span><span class="sxs-lookup"><span data-stu-id="5f12f-2633">Billing</span></span>

* <span data-ttu-id="5f12f-2634">Registrierungskontobefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2634">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="5f12f-2635">Nutzung</span><span class="sxs-lookup"><span data-stu-id="5f12f-2635">Consumption</span></span>

* <span data-ttu-id="5f12f-2636">Befehle vom Typ `marketplace` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2636">Added `marketplace` commands</span></span>
* <span data-ttu-id="5f12f-2637">[BREAKING CHANGE]`reservations summaries` in `reservation summary` umbenannt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2637">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="5f12f-2638">[BREAKING CHANGE]`reservations details` in `reservation detail` umbenannt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2638">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="5f12f-2639">[BREAKING CHANGE] Kurzoptionen `--reservation-order-id` und `--reservation-id` für `reservation`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2639">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="5f12f-2640">[BREAKING CHANGE]`--grain`-Kurzoptionen für `reservation summary`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2640">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="5f12f-2641">[BREAKING CHANGE]`--include-meter-details`-Kurzoptionen für `pricesheet`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2641">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="5f12f-2642">Container</span><span class="sxs-lookup"><span data-stu-id="5f12f-2642">Container</span></span>

* <span data-ttu-id="5f12f-2643">Parameter für die Volumebereitstellung für das Git-Repository hinzugefügt: `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` und `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="5f12f-2643">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="5f12f-2644">[#5926](https://github.com/Azure/azure-cli/issues/5926) behoben: Fehler bei `az container exec`, wenn „--container-name“ angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="5f12f-2644">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="5f12f-2645">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="5f12f-2645">Extension</span></span>

* <span data-ttu-id="5f12f-2646">Meldung für Distributionsüberprüfung in Debugebene geändert</span><span class="sxs-lookup"><span data-stu-id="5f12f-2646">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="5f12f-2647">Interactive</span><span class="sxs-lookup"><span data-stu-id="5f12f-2647">Interactive</span></span>

* <span data-ttu-id="5f12f-2648">Geändert: Verhinderung des Abschlusses bei nicht erkannten Befehlen</span><span class="sxs-lookup"><span data-stu-id="5f12f-2648">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="5f12f-2649">Ereignishooks vor und nach der Erstellung der Teilstruktur von Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2649">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="5f12f-2650">Abschluss für `--ids`-Parameter hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2650">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="5f12f-2651">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="5f12f-2651">Network</span></span>

* <span data-ttu-id="5f12f-2652">[#5936](https://github.com/Azure/azure-cli/issues/5936) behoben: `application-gateway create`-Tags konnten nicht festgelegt werden</span><span class="sxs-lookup"><span data-stu-id="5f12f-2652">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="5f12f-2653">Argument `--auth-certs` zum Anfügen von Authentifizierungszertifikaten für `application-gateway http-settings [create|update]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2653">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="5f12f-2654">#4910</span><span class="sxs-lookup"><span data-stu-id="5f12f-2654">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="5f12f-2655">`ddos-protection`-Befehle zum Erstellen von DDoS-Schutzplänen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2655">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="5f12f-2656">Unterstützung von `--ddos-protection-plan` für `vnet [create|update]` hinzugefügt, um das Zuordnen eines VNET zu einem DDoS-Schutzplan zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="5f12f-2656">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="5f12f-2657">Problem mit `--disable-bgp-route-propagation`-Flag in `network route-table [create|update]` behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-2657">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="5f12f-2658">Dummy-Argumente `--public-ip-address-type` und `--subnet-type` für `network lb [create|update]` entfernt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2658">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="5f12f-2659">Unterstützung für TXT-Datensätze mit RFC 1035-Escapesequenzen für `network dns zone [import|export]` und `network dns record-set txt add-record` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2659">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="5f12f-2660">Profil</span><span class="sxs-lookup"><span data-stu-id="5f12f-2660">Profile</span></span>

* <span data-ttu-id="5f12f-2661">Unterstützung für klassische Azure-Konten in `account list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2661">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="5f12f-2662">[BREAKING CHANGE]`--msi` & `--msi-port`-Argumente entfernt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2662">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="5f12f-2663">RDBMS</span><span class="sxs-lookup"><span data-stu-id="5f12f-2663">RDBMS</span></span>

* <span data-ttu-id="5f12f-2664">Befehl `georestore` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2664">Added `georestore` command</span></span>
* <span data-ttu-id="5f12f-2665">Speichergrößenbeschränkung aus Befehl `create` entfernt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2665">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="5f12f-2666">Resource</span><span class="sxs-lookup"><span data-stu-id="5f12f-2666">Resource</span></span>

* <span data-ttu-id="5f12f-2667">Unterstützung für `--metadata` zu `policy definition create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2667">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="5f12f-2668">Unterstützung von `--metadata`, `--set`, `--add`, `--remove` für `policy definition update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2668">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="5f12f-2669">SQL</span><span class="sxs-lookup"><span data-stu-id="5f12f-2669">SQL</span></span>

* <span data-ttu-id="5f12f-2670">`sql elastic-pool op list` und `sql elastic-pool op cancel` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2670">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="5f12f-2671">Storage</span><span class="sxs-lookup"><span data-stu-id="5f12f-2671">Storage</span></span>

* <span data-ttu-id="5f12f-2672">Fehlermeldungen für falsch formatierte Verbindungszeichenfolgen verbessert</span><span class="sxs-lookup"><span data-stu-id="5f12f-2672">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="5f12f-2673">VM</span><span class="sxs-lookup"><span data-stu-id="5f12f-2673">VM</span></span>

* <span data-ttu-id="5f12f-2674">Unterstützung für die Konfiguration der Plattform-Fehlerdomänenanzahl für `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2674">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="5f12f-2675">`vmss create` geändert, damit standardmäßig „Standard LB“ für zonales, großes oder per einzelner Platzierungsgruppe deaktiviertes Scale Set festgelegt wird</span><span class="sxs-lookup"><span data-stu-id="5f12f-2675">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret`
* <span data-ttu-id="5f12f-2677">Unterstützung für SKU mit öffentlicher IP für `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2677">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="5f12f-2678">Argumente `--keyvault` und `--resource-group` für `vm secret format` hinzugefügt, um Szenarien zu unterstützen, bei denen der Befehl die Tresor-ID nicht auflösen kann.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2678">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="5f12f-2679">#5718</span><span class="sxs-lookup"><span data-stu-id="5f12f-2679">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="5f12f-2680">Bessere Fehler für `[vm|vmss create]`, wenn der Standort einer Ressourcengruppe keine Zonenunterstützung aufweist</span><span class="sxs-lookup"><span data-stu-id="5f12f-2680">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="5f12f-2681">27. März 2018</span><span class="sxs-lookup"><span data-stu-id="5f12f-2681">March 27, 2018</span></span>

<span data-ttu-id="5f12f-2682">Version 2.0.30</span><span class="sxs-lookup"><span data-stu-id="5f12f-2682">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="5f12f-2683">Core</span><span class="sxs-lookup"><span data-stu-id="5f12f-2683">Core</span></span>

* <span data-ttu-id="5f12f-2684">Anzeigen einer Meldung für Erweiterungen, die in der Hilfe als Vorschauversion gekennzeichnet sind</span><span class="sxs-lookup"><span data-stu-id="5f12f-2684">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="5f12f-2685">ACS</span><span class="sxs-lookup"><span data-stu-id="5f12f-2685">ACS</span></span>

* <span data-ttu-id="5f12f-2686">Behebung eines Fehlers bei der SSL-Zertifikatprüfung für `aks install-cli` in Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="5f12f-2686">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="5f12f-2687">AppService</span><span class="sxs-lookup"><span data-stu-id="5f12f-2687">Appservice</span></span>

* <span data-ttu-id="5f12f-2688">Unterstützung nur von HTTPS zu `webapp update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2688">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="5f12f-2689">Unterstützung für Slots zu `az webapp identity [assign|show]` und `az functionapp identity [assign|show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2689">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="5f12f-2690">Backup</span><span class="sxs-lookup"><span data-stu-id="5f12f-2690">Backup</span></span>

* <span data-ttu-id="5f12f-2691">Neuer Befehl `az backup protection isenabled-for-vm` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2691">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="5f12f-2692">Mit diesem Befehl kann überprüft werden, ob ein virtueller Computer von einem beliebigen Tresor im Abonnement gesichert wird.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2692">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="5f12f-2693">Azure-Objekt-IDs für Parameter `--resource-group` und `--vault-name` für die folgenden Befehle aktiviert:</span><span class="sxs-lookup"><span data-stu-id="5f12f-2693">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="5f12f-2694">`--name`-Parameter wurden geändert, um das Ausgabeformat von `backup ... show`-Befehlen zu akzeptieren.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2694">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="5f12f-2695">Container</span><span class="sxs-lookup"><span data-stu-id="5f12f-2695">Container</span></span>

* <span data-ttu-id="5f12f-2696">Befehl `container exec` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2696">Added `container exec` command.</span></span> <span data-ttu-id="5f12f-2697">Ausführung von Befehlen in einem Container für eine ausgeführte Containergruppe</span><span class="sxs-lookup"><span data-stu-id="5f12f-2697">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="5f12f-2698">Zulassen der Tabellenausgabe zum Erstellen und Aktualisieren einer Containergruppe</span><span class="sxs-lookup"><span data-stu-id="5f12f-2698">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="5f12f-2699">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="5f12f-2699">Extension</span></span>

* <span data-ttu-id="5f12f-2700">Meldung für `extension add` hinzugefügt, wenn sich die Erweiterung in der Vorschauphase befindet</span><span class="sxs-lookup"><span data-stu-id="5f12f-2700">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="5f12f-2701">`extension list-available` geändert, um vollständige Erweiterungsdaten mit `--show-details` anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="5f12f-2701">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="5f12f-2702">[BREAKING CHANGE]`extension list-available` geändert, um standardmäßig vereinfachte Erweiterungsdaten anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="5f12f-2702">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="5f12f-2703">Interactive</span><span class="sxs-lookup"><span data-stu-id="5f12f-2703">Interactive</span></span>

* <span data-ttu-id="5f12f-2704">Vervollständigungen wurden geändert und werden jetzt aktiviert, sobald das Laden der Befehlstabelle abgeschlossen ist.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2704">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="5f12f-2705">Fehler bei der Verwendung des Parameters `--style` behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-2705">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="5f12f-2706">Interaktiver Lexer nach Befehlstabellensicherung instanziiert (sofern nicht vorhanden)</span><span class="sxs-lookup"><span data-stu-id="5f12f-2706">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="5f12f-2707">Verbesserte Unterstützung der Vervollständigung</span><span class="sxs-lookup"><span data-stu-id="5f12f-2707">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="5f12f-2708">Labor</span><span class="sxs-lookup"><span data-stu-id="5f12f-2708">Lab</span></span>

* <span data-ttu-id="5f12f-2709">Probleme mit Befehl `create environment` behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-2709">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="5f12f-2710">Überwachen</span><span class="sxs-lookup"><span data-stu-id="5f12f-2710">Monitor</span></span>

* <span data-ttu-id="5f12f-2711">Unterstützung für `--top`, `--orderby` und `--namespace` zu `metrics list` hinzugefügt [Nr. 5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="5f12f-2711">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="5f12f-2712">[#4529](https://github.com/Azure/azure-cli/issues/5785) behoben: `metrics list` akzeptiert eine durch Leerzeichen getrennte Liste von abzurufenden Metriken</span><span class="sxs-lookup"><span data-stu-id="5f12f-2712">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="5f12f-2713">Unterstützung für `--namespace` zu `metrics list-definitions` hinzugefügt [Nr. 5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="5f12f-2713">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="5f12f-2714">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="5f12f-2714">Network</span></span>

* <span data-ttu-id="5f12f-2715">Unterstützung für private DNS-Zonen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2715">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="5f12f-2716">Profil</span><span class="sxs-lookup"><span data-stu-id="5f12f-2716">Profile</span></span>

* <span data-ttu-id="5f12f-2717">Warnung für `--identity-port` und `--msi-port` zu `login` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2717">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="5f12f-2718">RDBMS</span><span class="sxs-lookup"><span data-stu-id="5f12f-2718">RDBMS</span></span>

* <span data-ttu-id="5f12f-2719">GA-API-Version 2017-12-01 (Geschäftsmodell) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2719">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="5f12f-2720">Resource</span><span class="sxs-lookup"><span data-stu-id="5f12f-2720">Resource</span></span>

* [BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="5f12f-2722">Role</span><span class="sxs-lookup"><span data-stu-id="5f12f-2722">Role</span></span>

* <span data-ttu-id="5f12f-2723">Unterstützung für erforderliche Zugriffskonfigurationen und native Clients zu `az ad app create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2723">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="5f12f-2724">`rbac`-Befehle geändert, um maximal 1.000 IDs für Objektauflösung zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="5f12f-2724">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="5f12f-2725">Befehle zur Verwaltung von Anmeldeinformationen (`ad sp credential [reset|list|delete]`) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2725">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="5f12f-2726">[BREAKING CHANGE] „properties“ aus `az role assignment [list|show]`-Ausgabe entfernt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2726">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="5f12f-2727">Unterstützung für `dataActions`- und `notDataActions`-Berechtigungen zu `role definition` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2727">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="5f12f-2728">Storage</span><span class="sxs-lookup"><span data-stu-id="5f12f-2728">Storage</span></span>

* <span data-ttu-id="5f12f-2729">Problem beim Hochladen von Dateien mit einer Größe von 195 GB bis 200 GB behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-2729">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="5f12f-2730">[#4049](https://github.com/Azure/azure-cli/issues/4049) behoben: Probleme bei Uploads von Anfügeblobs behoben, die ein Ignorieren der Bedingungsparameter verursacht haben</span><span class="sxs-lookup"><span data-stu-id="5f12f-2730">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="5f12f-2731">VM</span><span class="sxs-lookup"><span data-stu-id="5f12f-2731">VM</span></span>

* <span data-ttu-id="5f12f-2732">Warnung für anstehende BREAKING CHANGEen für Sätze mit mehr als 100 Instanzen zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2732">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="5f12f-2733">Unterstützung der Zonenresilienz zu `vm [snapshot|image]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2733">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="5f12f-2734">Datenträgerinstanzansicht geändert, um besseren Verschlüsselungsstatus zu melden</span><span class="sxs-lookup"><span data-stu-id="5f12f-2734">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="5f12f-2735">[BREAKING CHANGE]`vm extension delete` geändert, um keine Ausgabe mehr zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="5f12f-2735">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="5f12f-2736">13. März 2018</span><span class="sxs-lookup"><span data-stu-id="5f12f-2736">March 13, 2018</span></span>

<span data-ttu-id="5f12f-2737">Version 2.0.29</span><span class="sxs-lookup"><span data-stu-id="5f12f-2737">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="5f12f-2738">ACR</span><span class="sxs-lookup"><span data-stu-id="5f12f-2738">ACR</span></span>

* <span data-ttu-id="5f12f-2739">Unterstützung für den Parameter `--image` zu `repository delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2739">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="5f12f-2740">Parameter `--manifest` und `--tag` des Befehls `repository delete` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-2740">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="5f12f-2741">Befehl `repository untag` zum Entfernen eines Tags ohne das Löschen von Daten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2741">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="5f12f-2742">ACS</span><span class="sxs-lookup"><span data-stu-id="5f12f-2742">ACS</span></span>

* <span data-ttu-id="5f12f-2743">Befehl `aks upgrade-connector` zum Aktualisieren eines vorhandenen Connectors hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2743">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="5f12f-2744">`kubectl`-Konfigurationsdateien zur Verwendung von besser lesbarem YAML im Blockstil geändert</span><span class="sxs-lookup"><span data-stu-id="5f12f-2744">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="5f12f-2745">Advisor</span><span class="sxs-lookup"><span data-stu-id="5f12f-2745">Advisor</span></span>

* <span data-ttu-id="5f12f-2746">[BREAKING CHANGE]`advisor configuration get` in `advisor configuration list` umbenannt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2746">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="5f12f-2747">[BREAKING CHANGE]`advisor configuration set` in `advisor configuration update` umbenannt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2747">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="5f12f-2748">[BREAKING CHANGE]`advisor recommendation generate` entfernt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2748">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="5f12f-2749">Parameter `--refresh` zu `advisor recommendation list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2749">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="5f12f-2750">Befehl `advisor recommendation show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2750">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="5f12f-2751">AppService</span><span class="sxs-lookup"><span data-stu-id="5f12f-2751">Appservice</span></span>

* <span data-ttu-id="5f12f-2752">`[webapp|functionapp] assign-identity` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-2752">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="5f12f-2753">Befehle `webapp identity [assign|show]` und `functionapp identity [assign|show]` für verwaltete Identität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2753">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="5f12f-2754">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="5f12f-2754">Eventhubs</span></span>

* <span data-ttu-id="5f12f-2755">Erste Veröffentlichung</span><span class="sxs-lookup"><span data-stu-id="5f12f-2755">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="5f12f-2756">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="5f12f-2756">Extension</span></span>

* <span data-ttu-id="5f12f-2757">Überprüfung zum Warnen von Benutzern hinzugefügt, wenn sich die verwendete Distribution von der in der Paketquelldatei gespeicherten Distribution unterscheidet, da dies Fehlern führen kann</span><span class="sxs-lookup"><span data-stu-id="5f12f-2757">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="5f12f-2758">Interactive</span><span class="sxs-lookup"><span data-stu-id="5f12f-2758">Interactive</span></span>

* <span data-ttu-id="5f12f-2759">[#5625](https://github.com/Azure/azure-cli/issues/5625) behoben: Verlauf über verschiedene Sitzungen hinweg beibehalten</span><span class="sxs-lookup"><span data-stu-id="5f12f-2759">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="5f12f-2760">[#3016](https://github.com/Azure/azure-cli/issues/3016) behoben: Verlauf nicht aufgezeichnet, obwohl er innerhalb des Bereichs liegt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2760">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="5f12f-2761">[#5688](https://github.com/Azure/azure-cli/issues/5688) behoben: Abschlüsse wurden nicht angezeigt, wenn beim Laden der Befehlstabelle eine Ausnahme aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="5f12f-2761">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="5f12f-2762">Statusanzeige für lang ausgeführte Vorgänge korrigiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-2762">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="5f12f-2763">Überwachen</span><span class="sxs-lookup"><span data-stu-id="5f12f-2763">Monitor</span></span>

* <span data-ttu-id="5f12f-2764">`monitor autoscale-settings`-Befehle als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-2764">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="5f12f-2765">Befehle vom Typ `monitor autoscale` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2765">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="5f12f-2766">Befehle vom Typ `monitor autoscale profile` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2766">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="5f12f-2767">Befehle vom Typ `monitor autoscale rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2767">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="5f12f-2768">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="5f12f-2768">Network</span></span>

* <span data-ttu-id="5f12f-2769">[BREAKING CHANGE] Parameter `--tags` aus `route-filter rule create` entfernt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2769">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="5f12f-2770">Einige fehlerhafte Standardwerte für die folgenden Befehle entfernt:</span><span class="sxs-lookup"><span data-stu-id="5f12f-2770">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="5f12f-2771">`network watcher connection-monitor`-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2771">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="5f12f-2772">Parameter `--vnet` und `--subnet` zu `network watcher show-topology` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2772">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="5f12f-2773">Profil</span><span class="sxs-lookup"><span data-stu-id="5f12f-2773">Profile</span></span>

* <span data-ttu-id="5f12f-2774">Parameter `--msi` für `az login` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-2774">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="5f12f-2775">Parameter `--identity` für `az login` als Ersatz vor `--msi` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2775">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="5f12f-2776">RDBMS</span><span class="sxs-lookup"><span data-stu-id="5f12f-2776">RDBMS</span></span>

* <span data-ttu-id="5f12f-2777">[VORSCHAU] Geändert, sodass die API „2017-12-01-preview“ verwendet wird</span><span class="sxs-lookup"><span data-stu-id="5f12f-2777">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="5f12f-2778">Service Bus</span><span class="sxs-lookup"><span data-stu-id="5f12f-2778">Service Bus</span></span>

* <span data-ttu-id="5f12f-2779">Erste Veröffentlichung</span><span class="sxs-lookup"><span data-stu-id="5f12f-2779">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="5f12f-2780">Storage</span><span class="sxs-lookup"><span data-stu-id="5f12f-2780">Storage</span></span>

* <span data-ttu-id="5f12f-2781">[#4971](https://github.com/Azure/azure-cli/issues/4971) behoben: `storage blob copy` unterstützt jetzt andere Azure-Clouds.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2781">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="5f12f-2782">[#5286](https://github.com/Azure/azure-cli/issues/5286) behoben: Batchbefehle `storage blob [delete-batch|download-batch|upload-batch]` lösen bei Vorbedingungsfehlern keinen Fehler mehr aus</span><span class="sxs-lookup"><span data-stu-id="5f12f-2782">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="5f12f-2783">VM</span><span class="sxs-lookup"><span data-stu-id="5f12f-2783">VM</span></span>

* <span data-ttu-id="5f12f-2784">`[vm|vmss] create` unterstützt jetzt das Anfügen nicht verwalteter Datenträger und das Konfigurieren der Zwischenspeicherung.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2784">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="5f12f-2785">`[vm|vmss] assign-identity` und `[vm|vmss] remove-identity` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-2785">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="5f12f-2786">Befehle `vm identity [assign|remove|show]` und `vmss identity [assign|remove|show]` als Ersatz für veraltete Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2786">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="5f12f-2787">Standardpriorität in `vmss create` auf „Keine“ geändert</span><span class="sxs-lookup"><span data-stu-id="5f12f-2787">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="5f12f-2788">27. Februar 2018</span><span class="sxs-lookup"><span data-stu-id="5f12f-2788">February 27, 2018</span></span>

<span data-ttu-id="5f12f-2789">Version 2.0.28</span><span class="sxs-lookup"><span data-stu-id="5f12f-2789">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="5f12f-2790">Core</span><span class="sxs-lookup"><span data-stu-id="5f12f-2790">Core</span></span>

* <span data-ttu-id="5f12f-2791">[#5184](https://github.com/Azure/azure-cli/issues/5184) behoben: Problem beim Installieren von Homebrew</span><span class="sxs-lookup"><span data-stu-id="5f12f-2791">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="5f12f-2792">Unterstützung für Erweiterungstelemetrie mit benutzerdefinierten Schlüsseln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2792">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="5f12f-2793">HTTP-Protokollierung zu `--debug` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2793">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="5f12f-2794">ACS</span><span class="sxs-lookup"><span data-stu-id="5f12f-2794">ACS</span></span>

* <span data-ttu-id="5f12f-2795">Geändert, sodass für `aks install-connector` standardmäßig das Helm-Diagramm `virtual-kubelet-for-aks` verwendet wird</span><span class="sxs-lookup"><span data-stu-id="5f12f-2795">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="5f12f-2796">Problem behoben: Unzureichende Berechtigungen für Dienstprinzipale zum Erstellen einer ACI-Containergruppe</span><span class="sxs-lookup"><span data-stu-id="5f12f-2796">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="5f12f-2797">Parameter `--aci-container-group`, `--location` und `--image-tag` zu `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2797">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="5f12f-2798">Veraltungshinweis aus `aks get-versions` entfernt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2798">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="5f12f-2799">AppService</span><span class="sxs-lookup"><span data-stu-id="5f12f-2799">Appservice</span></span>

* <span data-ttu-id="5f12f-2800">Updates für die neue SDK-Version (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="5f12f-2800">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="5f12f-2801">[5538](https://github.com/Azure/azure-cli/issues/5538) behoben: `Free` wurde als ungültige SKU gemeldet.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2801">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="5f12f-2802">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="5f12f-2802">Cognitive Services</span></span>

* <span data-ttu-id="5f12f-2803">Hinweis beim Erstellen eines neuen Cognitive Services-Kontos aktualisiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-2803">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="5f12f-2804">Nutzung</span><span class="sxs-lookup"><span data-stu-id="5f12f-2804">Consumption</span></span>

* <span data-ttu-id="5f12f-2805">Neue Befehle für PriceSheet-API hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2805">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="5f12f-2806">Vorhandene Formate für Nutzungsdetails und Reservierungsdetails aktualisiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-2806">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="5f12f-2807">Container</span><span class="sxs-lookup"><span data-stu-id="5f12f-2807">Container</span></span>

* <span data-ttu-id="5f12f-2808">Argumente `--secrets` und `--secrets-mount-path` zu `container create` hinzugefügt, um Geheimnisse in ACI verwenden zu können</span><span class="sxs-lookup"><span data-stu-id="5f12f-2808">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="5f12f-2809">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="5f12f-2809">Network</span></span>

* <span data-ttu-id="5f12f-2810">[#5559](https://github.com/Azure/azure-cli/issues/5559) behoben: Fehlender Client in `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="5f12f-2810">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="5f12f-2811">Resource</span><span class="sxs-lookup"><span data-stu-id="5f12f-2811">Resource</span></span>

* <span data-ttu-id="5f12f-2812">`group deployment export` geändert, um eine partielle Vorlage und ggf. Fehler anzuzeigen, wenn der Vorgang nicht erfolgreich war</span><span class="sxs-lookup"><span data-stu-id="5f12f-2812">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="5f12f-2813">Role</span><span class="sxs-lookup"><span data-stu-id="5f12f-2813">Role</span></span>

* <span data-ttu-id="5f12f-2814">`role assignment list-changelogs` hinzugefügt, um die Überprüfung von Dienstprinzipalrollen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="5f12f-2814">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="5f12f-2815">SQL</span><span class="sxs-lookup"><span data-stu-id="5f12f-2815">SQL</span></span>

* <span data-ttu-id="5f12f-2816">Zonenredundanzunterstützung für Datenbanken und Pools für elastische Datenbanken hinzugefügt (bei Erstellung und Aktualisierung)</span><span class="sxs-lookup"><span data-stu-id="5f12f-2816">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="5f12f-2817">Storage</span><span class="sxs-lookup"><span data-stu-id="5f12f-2817">Storage</span></span>

* <span data-ttu-id="5f12f-2818">Angabe von Zielpfad/Präfix für `storage blob [upload-batch|download-batch]` ermöglicht</span><span class="sxs-lookup"><span data-stu-id="5f12f-2818">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="5f12f-2819">VM</span><span class="sxs-lookup"><span data-stu-id="5f12f-2819">VM</span></span>

* <span data-ttu-id="5f12f-2820">Unterstützung für das Anfügen/Trennen von Datenträgern für eine einzelne VMSS-Instanz hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2820">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="5f12f-2821">13. Februar 2018</span><span class="sxs-lookup"><span data-stu-id="5f12f-2821">February 13, 2018</span></span>

<span data-ttu-id="5f12f-2822">Version 2.0.27</span><span class="sxs-lookup"><span data-stu-id="5f12f-2822">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="5f12f-2823">Core</span><span class="sxs-lookup"><span data-stu-id="5f12f-2823">Core</span></span>

* <span data-ttu-id="5f12f-2824">Authentifizierung für Abonnement-ID und Namen bei der MSI-Anmeldung in Authentifizierung mit Schlüssel geändert</span><span class="sxs-lookup"><span data-stu-id="5f12f-2824">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="5f12f-2825">ACS</span><span class="sxs-lookup"><span data-stu-id="5f12f-2825">ACS</span></span>

* <span data-ttu-id="5f12f-2826">[BREAKING CHANGE]`aks get-versions` aus Gründen der Genauigkeit in `aks get-upgrades` umbenannt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2826">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="5f12f-2827">`aks get-versions` zur Anzeige der verfügbaren Kubernetes-Versionen für `aks create` geändert</span><span class="sxs-lookup"><span data-stu-id="5f12f-2827">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="5f12f-2828">Standardwerte von `aks create` in Auswahl der Kubernetes-Version durch den Server geändert</span><span class="sxs-lookup"><span data-stu-id="5f12f-2828">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="5f12f-2829">Hilfemeldungen zu dem von AKS generierten Dienstprinzipal aktualisiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-2829">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="5f12f-2830">Standardknotengrößen für `aks create` von „Standard\_D1\_v2“ in „Standard\_DS1\_v2“ geändert</span><span class="sxs-lookup"><span data-stu-id="5f12f-2830">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="5f12f-2831">Zuverlässigkeit der Suche nach dem Dashboardpod für `az aks browse` verbessert</span><span class="sxs-lookup"><span data-stu-id="5f12f-2831">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="5f12f-2832">`aks get-credentials` korrigiert, um Unicode-Fehler beim Laden von Kubernetes-Konfigurationsdateien zu behandeln</span><span class="sxs-lookup"><span data-stu-id="5f12f-2832">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="5f12f-2833">Meldung zu `az aks install-cli` hinzugefügt, um das Abrufen von `kubectl` in `$PATH` zu erleichtern</span><span class="sxs-lookup"><span data-stu-id="5f12f-2833">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="5f12f-2834">AppService</span><span class="sxs-lookup"><span data-stu-id="5f12f-2834">Appservice</span></span>

* <span data-ttu-id="5f12f-2835">Problem behoben, das zu einem Fehler von `webapp [backup|restore]` aufgrund eines Nullverweises führte</span><span class="sxs-lookup"><span data-stu-id="5f12f-2835">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="5f12f-2836">Unterstützung für Standard-App Service-Pläne durch `az configure --defaults appserviceplan=my-asp` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2836">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="5f12f-2837">CDN</span><span class="sxs-lookup"><span data-stu-id="5f12f-2837">CDN</span></span>

* <span data-ttu-id="5f12f-2838">Befehle vom Typ `cdn custom-domain [enable-https|disable-https]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2838">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="5f12f-2839">Container</span><span class="sxs-lookup"><span data-stu-id="5f12f-2839">Container</span></span>

* <span data-ttu-id="5f12f-2840">Option `--follow` zu `az container logs` für Streamingprotokolle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2840">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="5f12f-2841">Befehl `container attach` hinzugefügt, der die lokale Standardausgabe und Fehlerdatenströme an einen Container in einer Containergruppe angefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2841">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="5f12f-2842">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="5f12f-2842">CosmosDB</span></span>

* <span data-ttu-id="5f12f-2843">Unterstützung für Einstellungsfunktionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2843">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="5f12f-2844">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="5f12f-2844">Extension</span></span>

* <span data-ttu-id="5f12f-2845">Unterstützung für den Parameter `--pip-proxy` zu Befehlen vom Typ `az extension [add|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2845">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="5f12f-2846">Unterstützung für das Argument `--pip-extra-index-urls` zu Befehlen vom Typ `az extension [add|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2846">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="5f12f-2847">Feedback</span><span class="sxs-lookup"><span data-stu-id="5f12f-2847">Feedback</span></span>

* <span data-ttu-id="5f12f-2848">Erweiterungsinformationen zu Telemetriedaten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2848">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="5f12f-2849">Interactive</span><span class="sxs-lookup"><span data-stu-id="5f12f-2849">Interactive</span></span>

* <span data-ttu-id="5f12f-2850">Problem behoben, aufgrund dessen der Benutzer bei Verwendung des interaktiven Modus in Cloud Shell zur Anmeldung aufgefordert wird</span><span class="sxs-lookup"><span data-stu-id="5f12f-2850">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="5f12f-2851">Regression mit fehlenden Parametervervollständigungen korrigiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-2851">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="5f12f-2852">IoT</span><span class="sxs-lookup"><span data-stu-id="5f12f-2852">IoT</span></span>

* <span data-ttu-id="5f12f-2853">Problem behoben, aufgrund dessen `iot dps access policy [create|update]` bei erfolgreicher Ausführung einen Fehler „nicht gefunden“ zurückgibt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2853">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="5f12f-2854">Problem behoben, aufgrund dessen `iot dps linked-hub [create|update]` bei erfolgreicher Ausführung einen Fehler „nicht gefunden“ zurückgibt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2854">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="5f12f-2855">Unterstützung für `--no-wait` zu `iot dps access policy [create|update]` und `iot dps linked-hub [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2855">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="5f12f-2856">`iot hub create` geändert, um die Angabe der Anzahl von Partitionen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="5f12f-2856">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="5f12f-2857">Überwachen</span><span class="sxs-lookup"><span data-stu-id="5f12f-2857">Monitor</span></span>

* <span data-ttu-id="5f12f-2858">Befehl `az monitor log-profiles create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-2858">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="5f12f-2859">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="5f12f-2859">Network</span></span>

* <span data-ttu-id="5f12f-2860">Option `--tags` für folgende Befehle korrigiert:</span><span class="sxs-lookup"><span data-stu-id="5f12f-2860">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="5f12f-2861">Profil</span><span class="sxs-lookup"><span data-stu-id="5f12f-2861">Profile</span></span>

* <span data-ttu-id="5f12f-2862">`az login` im interaktiven Modus aktiviert</span><span class="sxs-lookup"><span data-stu-id="5f12f-2862">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="5f12f-2863">Resource</span><span class="sxs-lookup"><span data-stu-id="5f12f-2863">Resource</span></span>

* <span data-ttu-id="5f12f-2864">`feature show` wieder hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2864">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="5f12f-2865">Role</span><span class="sxs-lookup"><span data-stu-id="5f12f-2865">Role</span></span>

* <span data-ttu-id="5f12f-2866">Argument `--available-to-other-tenants` zu `ad app update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2866">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="5f12f-2867">SQL</span><span class="sxs-lookup"><span data-stu-id="5f12f-2867">SQL</span></span>

* <span data-ttu-id="5f12f-2868">Befehle vom Typ `sql server dns-alias` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2868">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="5f12f-2869">`sql db rename` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2869">Added `sql db rename`</span></span>
* <span data-ttu-id="5f12f-2870">Unterstützung für das Argument `--ids` für alle SQL-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2870">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="5f12f-2871">Storage</span><span class="sxs-lookup"><span data-stu-id="5f12f-2871">Storage</span></span>

* <span data-ttu-id="5f12f-2872">Befehle `storage blob service-properties delete-policy` und `storage blob undelete` hinzugefügt, um vorläufiges Löschen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="5f12f-2872">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="5f12f-2873">VM</span><span class="sxs-lookup"><span data-stu-id="5f12f-2873">VM</span></span>

* <span data-ttu-id="5f12f-2874">Absturz bei unvollständiger Initialisierung der VM-Verschlüsselung behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-2874">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="5f12f-2875">Prinzipal-ID-Ausgabe beim Aktivieren von MSI hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2875">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="5f12f-2876">`vm boot-diagnostics get-boot-log` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="5f12f-2876">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="5f12f-2877">31. Januar 2018</span><span class="sxs-lookup"><span data-stu-id="5f12f-2877">January 31, 2018</span></span>

<span data-ttu-id="5f12f-2878">Version 2.0.26</span><span class="sxs-lookup"><span data-stu-id="5f12f-2878">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="5f12f-2879">Core</span><span class="sxs-lookup"><span data-stu-id="5f12f-2879">Core</span></span>

* <span data-ttu-id="5f12f-2880">Unterstützung für das Abrufen von unformatierten Token im MSI-Kontext hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2880">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="5f12f-2881">Abrufindikator-Zeichenfolge nach Fertigstellung von LRO für die Windows-Datei „cmd.exe“ entfernt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2881">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="5f12f-2882">Warnung hinzugefügt, die angezeigt wird, wenn ein konfigurierter Standardwert in einen Eintrag auf INFO-Ebene geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2882">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="5f12f-2883">`--verbose` zum Anzeigen verwenden.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2883">Use `--verbose` to see</span></span>
* <span data-ttu-id="5f12f-2884">Statusanzeige für Wait-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2884">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="5f12f-2885">ACS</span><span class="sxs-lookup"><span data-stu-id="5f12f-2885">ACS</span></span>

* <span data-ttu-id="5f12f-2886">Argument `--disable-browser` erläutert</span><span class="sxs-lookup"><span data-stu-id="5f12f-2886">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="5f12f-2887">Vervollständigung mit der TAB-TASTE für Argumente vom Typ `--vm-size` verbessert</span><span class="sxs-lookup"><span data-stu-id="5f12f-2887">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="5f12f-2888">AppService</span><span class="sxs-lookup"><span data-stu-id="5f12f-2888">Appservice</span></span>

* <span data-ttu-id="5f12f-2889">`webapp log [tail|download]` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="5f12f-2889">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="5f12f-2890">Überprüfung `kind` für Web-Apps und Funktionen entfernt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2890">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="5f12f-2891">CDN</span><span class="sxs-lookup"><span data-stu-id="5f12f-2891">CDN</span></span>

* <span data-ttu-id="5f12f-2892">Problem mit fehlendem Client für `cdn custom-domain create` behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-2892">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="5f12f-2893">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="5f12f-2893">CosmosDB</span></span>

* <span data-ttu-id="5f12f-2894">Parameterbeschreibung für Failoverrichtlinien korrigiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-2894">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="5f12f-2895">Interactive</span><span class="sxs-lookup"><span data-stu-id="5f12f-2895">Interactive</span></span>

* <span data-ttu-id="5f12f-2896">Problem behoben, aufgrund dessen Vervollständigungen von Befehlsoptionen nicht mehr angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="5f12f-2896">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="5f12f-2897">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="5f12f-2897">Network</span></span>

* <span data-ttu-id="5f12f-2898">Schutz für `--cert-password` zu `application-gateway create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2898">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="5f12f-2899">Problem mit `application-gateway update` behoben, aufgrund dessen `--sku` fälschlicherweise einen Standardwert anwendete</span><span class="sxs-lookup"><span data-stu-id="5f12f-2899">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="5f12f-2900">Schutz für `--shared-key` und `--authorization-key` zu `vpn-connection create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2900">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="5f12f-2901">Problem mit fehlendem Client für `asg create` behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-2901">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="5f12f-2902">Parameter `--file-name / -f` für exportierte Namen zu `dns zone export` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2902">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="5f12f-2903">Folgende Probleme mit `dns zone export` behoben:</span><span class="sxs-lookup"><span data-stu-id="5f12f-2903">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="5f12f-2904">Problem behoben, aufgrund dessen lange TXT-Einträge nicht korrekt exportiert wurden</span><span class="sxs-lookup"><span data-stu-id="5f12f-2904">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="5f12f-2905">Problem behoben, aufgrund dessen TXT-Einträge in Anführungszeichen fälschlich ohne Anführungszeichen in Escapezeichen exportiert wurden</span><span class="sxs-lookup"><span data-stu-id="5f12f-2905">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="5f12f-2906">Problem behoben, aufgrund dessen bestimmte Datensätze zweimal mit `dns zone import` importiert wurden</span><span class="sxs-lookup"><span data-stu-id="5f12f-2906">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="5f12f-2907">Befehle `vnet-gateway root-cert` und `vnet-gateway revoked-cert` wiederhergestellt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2907">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="5f12f-2908">Profil</span><span class="sxs-lookup"><span data-stu-id="5f12f-2908">Profile</span></span>

* <span data-ttu-id="5f12f-2909">`get-access-token` zur Verwendung auf einer VM mit Identität korrigiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-2909">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="5f12f-2910">Resource</span><span class="sxs-lookup"><span data-stu-id="5f12f-2910">Resource</span></span>

* <span data-ttu-id="5f12f-2911">Fehler mit `deployment [create|validate]` korrigiert, aufgrund dessen fälschlich eine Warnung angezeigt wurde, wenn ein Vorlagenfeld „Typ“ Werte in Großbuchstaben enthielt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2911">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="5f12f-2912">Storage</span><span class="sxs-lookup"><span data-stu-id="5f12f-2912">Storage</span></span>

* <span data-ttu-id="5f12f-2913">Problem mit der Migration von Storage V1-Konten zu Storage V2 behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-2913">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="5f12f-2914">Statusberichterstellung für alle Upload-/Downloadbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2914">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="5f12f-2915">Fehler korrigiert, der die Verwendung der arg-Option „-n“ mit `storage account check-name` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="5f12f-2915">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="5f12f-2916">Spalte „Momentaufnahme“ zur Tabellenausgabe für `blob [list|show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2916">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="5f12f-2917">Fehler mit verschiedenen Parametern korrigiert, die als Int-Typen analysiert werden mussten</span><span class="sxs-lookup"><span data-stu-id="5f12f-2917">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="5f12f-2918">VM</span><span class="sxs-lookup"><span data-stu-id="5f12f-2918">VM</span></span>

* <span data-ttu-id="5f12f-2919">Befehl `vm image accept-terms` hinzugefügt, um die Erstellung von VMs aus Images mit zusätzlichen Gebühren zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="5f12f-2919">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="5f12f-2920">`[vm|vmss create]` korrigiert, um sicherzustellen, dass Befehle unter einem Proxy mit nicht signierten Zertifikaten ausgeführt werden können</span><span class="sxs-lookup"><span data-stu-id="5f12f-2920">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="5f12f-2921">[VORSCHAU] Unterstützung für „niedrige“ Priorität zu VMSS hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2921">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="5f12f-2922">Schutz für `--admin-password` zu `[vm|vmss] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2922">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="5f12f-2923">17. Januar 2018</span><span class="sxs-lookup"><span data-stu-id="5f12f-2923">January 17, 2018</span></span>

<span data-ttu-id="5f12f-2924">Version 2.0.25</span><span class="sxs-lookup"><span data-stu-id="5f12f-2924">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="5f12f-2925">ACR</span><span class="sxs-lookup"><span data-stu-id="5f12f-2925">ACR</span></span>

* <span data-ttu-id="5f12f-2926">Fallback auf ACR-Anmeldung bei Fehlern mit Windows-Anmeldeinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2926">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="5f12f-2927">Registrierungsprotokolle aktiviert</span><span class="sxs-lookup"><span data-stu-id="5f12f-2927">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="5f12f-2928">ACS</span><span class="sxs-lookup"><span data-stu-id="5f12f-2928">ACS</span></span>

* <span data-ttu-id="5f12f-2929">Befehl `get-credentials` korrigiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-2929">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="5f12f-2930">SPN-Rollenanforderung entfernt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2930">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="5f12f-2931">AppService</span><span class="sxs-lookup"><span data-stu-id="5f12f-2931">Appservice</span></span>

* <span data-ttu-id="5f12f-2932">Fehler mit `config ssl upload` behoben, bei dem `hosting_environment_profile` NULL war</span><span class="sxs-lookup"><span data-stu-id="5f12f-2932">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="5f12f-2933">Unterstützung benutzerdefinierter URLs zu `browse` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2933">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="5f12f-2934">Slotunterstützung für `log tail` korrigiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-2934">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="5f12f-2935">Backup</span><span class="sxs-lookup"><span data-stu-id="5f12f-2935">Backup</span></span>

* <span data-ttu-id="5f12f-2936">Option `--container-name` von `backup item list` geändert (ist jetzt optional)</span><span class="sxs-lookup"><span data-stu-id="5f12f-2936">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="5f12f-2937">Speicherkontooptionen zu `backup restore restore-disks` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2937">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="5f12f-2938">Standortüberprüfung in `backup protection enable-for-vm` korrigiert (Groß-/Kleinschreibung wird jetzt nicht mehr beachtet)</span><span class="sxs-lookup"><span data-stu-id="5f12f-2938">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="5f12f-2939">Problem behoben, durch das bei Befehlen mit ungültigem Containernamen ein Fehler auftrat</span><span class="sxs-lookup"><span data-stu-id="5f12f-2939">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="5f12f-2940">`backup item list` geändert (Integritätsstatus jetzt standardmäßig enthalten)</span><span class="sxs-lookup"><span data-stu-id="5f12f-2940">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="5f12f-2941">Batch</span><span class="sxs-lookup"><span data-stu-id="5f12f-2941">Batch</span></span>

* <span data-ttu-id="5f12f-2942">`batch login` geändert, um Authentifizierungsdetails zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="5f12f-2942">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="5f12f-2943">Cloud</span><span class="sxs-lookup"><span data-stu-id="5f12f-2943">Cloud</span></span>

* <span data-ttu-id="5f12f-2944">Beim Festlegen von `--profile` für eine Cloud werden nun keine Endpunkte mehr benötigt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2944">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="5f12f-2945">Nutzung</span><span class="sxs-lookup"><span data-stu-id="5f12f-2945">Consumption</span></span>

* <span data-ttu-id="5f12f-2946">Neue Befehle für Reservierungen hinzugefügt: `consumption reservations summaries` und `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="5f12f-2946">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="5f12f-2947">Event Grid</span><span class="sxs-lookup"><span data-stu-id="5f12f-2947">Event Grid</span></span>

* <span data-ttu-id="5f12f-2948">[BREAKING CHANGE] Die Befehle vom Typ `az eventgrid topic event-subscription` wurden in `eventgrid event-subscription` verschoben.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2948">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="5f12f-2949">[BREAKING CHANGE] Die Befehle vom Typ `az eventgrid resource event-subscription` wurden in `eventgrid event-subscription` verschoben.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2949">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="5f12f-2950">[BREAKING CHANGE] Der Befehl `eventgrid event-subscription show-endpoint-url` wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2950">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="5f12f-2951">Verwenden Sie stattdessen `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2951">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="5f12f-2952">Befehl `eventgrid topic update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2952">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="5f12f-2953">Befehl `eventgrid event-subscription update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2953">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="5f12f-2954">Parameter `--ids` für Befehle vom Typ `eventgrid topic` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2954">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="5f12f-2955">Unterstützung der Vervollständigung mit der TAB-TASTE für Themennamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2955">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="5f12f-2956">Interactive</span><span class="sxs-lookup"><span data-stu-id="5f12f-2956">Interactive</span></span>

* <span data-ttu-id="5f12f-2957">Problem behoben, das dazu führte, dass der interaktive Modus nicht mit Python 2.x verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="5f12f-2957">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="5f12f-2958">Fehler beim Start behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-2958">Fixed errors on startup</span></span>
* <span data-ttu-id="5f12f-2959">Problem behoben, das dazu führte, dass einige Befehle nicht im interaktiven Modus ausgeführt werden konnten</span><span class="sxs-lookup"><span data-stu-id="5f12f-2959">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="5f12f-2960">IoT</span><span class="sxs-lookup"><span data-stu-id="5f12f-2960">IoT</span></span>

* <span data-ttu-id="5f12f-2961">Unterstützung für Gerätebereitstellungsdienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2961">Added support for device provisioning service</span></span>
* <span data-ttu-id="5f12f-2962">Benachrichtigungen zu veralteten Elementen in Befehlen und in der Befehlshilfe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2962">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="5f12f-2963">IoT-Überprüfung hinzugefügt, um Benutzer über die IoT-Erweiterung zu informieren</span><span class="sxs-lookup"><span data-stu-id="5f12f-2963">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="5f12f-2964">Überwachen</span><span class="sxs-lookup"><span data-stu-id="5f12f-2964">Monitor</span></span>

* <span data-ttu-id="5f12f-2965">Unterstützung mehrerer Diagnoseeinstellung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2965">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="5f12f-2966">Der Parameter `--name` ist nun für `az monitor diagnostic-settings create` erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5f12f-2966">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="5f12f-2967">Befehl `monitor diagnostic-settings categories` zum Abrufen der Diagnoseeinstellungskategorie hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2967">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="5f12f-2968">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="5f12f-2968">Network</span></span>

* <span data-ttu-id="5f12f-2969">Problem behoben, das beim Ändern des aktiven Standbymodus mit `vnet-gateway update` auftrat</span><span class="sxs-lookup"><span data-stu-id="5f12f-2969">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="5f12f-2970">Unterstützung für HTTP2 zu `application-gateway [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2970">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="5f12f-2971">Profil</span><span class="sxs-lookup"><span data-stu-id="5f12f-2971">Profile</span></span>

* <span data-ttu-id="5f12f-2972">Unterstützung für die Anmeldung mit durch Benutzer zugewiesenen Identitäten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2972">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="5f12f-2973">Role</span><span class="sxs-lookup"><span data-stu-id="5f12f-2973">Role</span></span>

* <span data-ttu-id="5f12f-2974">Argument `--assignee-object-id` zu `role assignment create` hinzugefügt, um Graph-Abfrage zu umgehen</span><span class="sxs-lookup"><span data-stu-id="5f12f-2974">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="5f12f-2975">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="5f12f-2975">Service Fabric</span></span>

* <span data-ttu-id="5f12f-2976">Ausführliche Fehler zur Überprüfungsantwort bei der Clustererstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2976">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="5f12f-2977">Problem mit fehlendem Client für verschiedene Befehle behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-2977">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="5f12f-2978">VM</span><span class="sxs-lookup"><span data-stu-id="5f12f-2978">VM</span></span>

* <span data-ttu-id="5f12f-2979">[VORSCHAUVERSION] Zonenübergreifende Unterstützung für `vmss`</span><span class="sxs-lookup"><span data-stu-id="5f12f-2979">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="5f12f-2980">[BREAKING CHANGE] Standard für Einzelzone (`vmss`) in Standardlastenausgleich geändert</span><span class="sxs-lookup"><span data-stu-id="5f12f-2980">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="5f12f-2981">[BREAKING CHANGE]`externalIdentities` in `userAssignedIdentities` geändert für EMSI</span><span class="sxs-lookup"><span data-stu-id="5f12f-2981">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="5f12f-2982">[VORSCHAUVERSION] Unterstützung für Austausch des Betriebssystemdatenträgers hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2982">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="5f12f-2983">Unterstützung der Verwendung von VM-Images aus anderen Abonnements hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2983">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="5f12f-2984">Argumente `--plan-name`, `--plan-product`, `--plan-promotion-code` und `--plan-publisher` zu `[vm|vmss] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2984">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="5f12f-2985">Fehlerbedingte Probleme mit `[vm|vmss] create` behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-2985">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="5f12f-2986">Übermäßige Ressourcenverwendung durch `vm image list --all` behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-2986">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="5f12f-2987">19. Dezember 2017</span><span class="sxs-lookup"><span data-stu-id="5f12f-2987">December 19, 2017</span></span>

<span data-ttu-id="5f12f-2988">Version 2.0.23</span><span class="sxs-lookup"><span data-stu-id="5f12f-2988">Version 2.0.23</span></span>

* <span data-ttu-id="5f12f-2989">Unterstützung für die Anmeldung mit durch Benutzer zugewiesenen Identitäten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2989">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="5f12f-2990">Container</span><span class="sxs-lookup"><span data-stu-id="5f12f-2990">Container</span></span>

* <span data-ttu-id="5f12f-2991">Falsche Reihenfolge der Parameter für Containerprotokolle behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-2991">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="5f12f-2992">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="5f12f-2992">Network</span></span>

* <span data-ttu-id="5f12f-2993">Argument `--disable-bgp-route-propagation` zu `route-table [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2993">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="5f12f-2994">Argument `--ip-tags` zu `public-ip [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2994">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="5f12f-2995">Storage</span><span class="sxs-lookup"><span data-stu-id="5f12f-2995">Storage</span></span>

* <span data-ttu-id="5f12f-2996">Unterstützung für Storage V2 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2996">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="5f12f-2997">VM</span><span class="sxs-lookup"><span data-stu-id="5f12f-2997">VM</span></span>

* <span data-ttu-id="5f12f-2998">[VORSCHAUVERSION] Unterstützung für durch Benutzer zugewiesene Identitäten für virtuelle Computer und VMSSs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-2998">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="5f12f-2999">5\. Dezember 2017</span><span class="sxs-lookup"><span data-stu-id="5f12f-2999">December 5, 2017</span></span>

<span data-ttu-id="5f12f-3000">Version 2.0.22</span><span class="sxs-lookup"><span data-stu-id="5f12f-3000">Version 2.0.22</span></span>

* <span data-ttu-id="5f12f-3001">`az component`-Befehle wurden entfernt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-3001">Removed `az component` commands.</span></span> <span data-ttu-id="5f12f-3002">Verwenden Sie stattdessen `az extension`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-3002">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="5f12f-3003">Core</span><span class="sxs-lookup"><span data-stu-id="5f12f-3003">Core</span></span>
* <span data-ttu-id="5f12f-3004">Der `AZURE_US_GOV_CLOUD`-Autoritätsendpunkt von AAD wurde von „login.microsoftonline.com“ in „login.microsoftonline.us“ geändert.</span><span class="sxs-lookup"><span data-stu-id="5f12f-3004">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="5f12f-3005">Problem behoben, aufgrund dessen Telemetriedaten fortlaufend neu gesendet wurden</span><span class="sxs-lookup"><span data-stu-id="5f12f-3005">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="5f12f-3006">ACS</span><span class="sxs-lookup"><span data-stu-id="5f12f-3006">ACS</span></span>

* <span data-ttu-id="5f12f-3007">Die Befehle `aks install-connector` und `aks remove-connector` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-3007">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="5f12f-3008">Verbesserte Fehlerberichterstellung für `acs create`</span><span class="sxs-lookup"><span data-stu-id="5f12f-3008">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="5f12f-3009">Feste Verwendung von `aks get-credentials -f` ohne vollqualifizierten Pfad</span><span class="sxs-lookup"><span data-stu-id="5f12f-3009">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="5f12f-3010">Advisor</span><span class="sxs-lookup"><span data-stu-id="5f12f-3010">Advisor</span></span>

* <span data-ttu-id="5f12f-3011">Erste Veröffentlichung</span><span class="sxs-lookup"><span data-stu-id="5f12f-3011">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="5f12f-3012">AppService</span><span class="sxs-lookup"><span data-stu-id="5f12f-3012">Appservice</span></span>

* <span data-ttu-id="5f12f-3013">Erstellung feststehender Zertifikatnamen mit `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="5f12f-3013">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="5f12f-3014">`webapp [list|show]` und `functionapp [list|show]` wurden verbessert, um die richtigen Apps anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="5f12f-3014">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="5f12f-3015">Standardwert für `WEBSITE_NODE_DEFAULT_VERSION` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3015">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="5f12f-3016">Nutzung</span><span class="sxs-lookup"><span data-stu-id="5f12f-3016">Consumption</span></span>

* <span data-ttu-id="5f12f-3017">Unterstützung für API-Version 2017-11-30 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3017">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="5f12f-3018">Container</span><span class="sxs-lookup"><span data-stu-id="5f12f-3018">Container</span></span>

* <span data-ttu-id="5f12f-3019">Feste Regression für Standardports</span><span class="sxs-lookup"><span data-stu-id="5f12f-3019">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="5f12f-3020">Überwachen</span><span class="sxs-lookup"><span data-stu-id="5f12f-3020">Monitor</span></span>

* <span data-ttu-id="5f12f-3021">Unterstützung mehrerer Dimensionen zu Metrikbefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3021">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="5f12f-3022">Resource</span><span class="sxs-lookup"><span data-stu-id="5f12f-3022">Resource</span></span>

* <span data-ttu-id="5f12f-3023">Argument `--include-response-body` zu `resource show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3023">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="5f12f-3024">Role</span><span class="sxs-lookup"><span data-stu-id="5f12f-3024">Role</span></span>

* <span data-ttu-id="5f12f-3025">Anzeige von Standardzuweisungen für „klassische“ Administratoren zu `role assignment list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3025">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="5f12f-3026">Unterstützung für das Hinzufügen (anstelle der Überschreibung) von Anmeldeinformationen zu `ad sp reset-credentials` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3026">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="5f12f-3027">Verbesserte Fehlerberichterstellung für `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="5f12f-3027">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="5f12f-3028">SQL</span><span class="sxs-lookup"><span data-stu-id="5f12f-3028">SQL</span></span>

* <span data-ttu-id="5f12f-3029">Die Befehle `sql db list-usages` und `sql db show-usage` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-3029">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="5f12f-3030">Die Befehle `sql server conn-policy show` und `sql server conn-policy update` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-3030">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="5f12f-3031">VM</span><span class="sxs-lookup"><span data-stu-id="5f12f-3031">VM</span></span>

* <span data-ttu-id="5f12f-3032">Zoneninformationen zu `az vm list-skus` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3032">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="5f12f-3033">14. November 2017</span><span class="sxs-lookup"><span data-stu-id="5f12f-3033">November 14, 2017</span></span>

<span data-ttu-id="5f12f-3034">Version 2.0.21</span><span class="sxs-lookup"><span data-stu-id="5f12f-3034">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="5f12f-3035">ACR</span><span class="sxs-lookup"><span data-stu-id="5f12f-3035">ACR</span></span>

* <span data-ttu-id="5f12f-3036">Unterstützung für das Erstellen von Webhooks in Replikationsregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3036">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="5f12f-3037">ACS</span><span class="sxs-lookup"><span data-stu-id="5f12f-3037">ACS</span></span>

* <span data-ttu-id="5f12f-3038">Formulierung in AKS von „Agent“ in „Knoten“ geändert</span><span class="sxs-lookup"><span data-stu-id="5f12f-3038">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="5f12f-3039">Option `--orchestrator-release` für `acs create` als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="5f12f-3039">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="5f12f-3040">VM-Standardgröße für AKS in `Standard_D1_v2` geändert</span><span class="sxs-lookup"><span data-stu-id="5f12f-3040">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="5f12f-3041">`az aks browse` für Windows korrigiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-3041">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="5f12f-3042">`az aks get-credentials` für Windows korrigiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-3042">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="5f12f-3043">AppService</span><span class="sxs-lookup"><span data-stu-id="5f12f-3043">Appservice</span></span>

* <span data-ttu-id="5f12f-3044">Bereitstellungsquelle `config-zip` für Web-Apps und Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3044">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="5f12f-3045">Option `--docker-container-logging` zu `az webapp log config` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3045">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="5f12f-3046">Option `storage` aus dem Parameter `--web-server-logging` von `az webapp log config` entfernt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3046">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="5f12f-3047">Fehlermeldungen für `deployment user set` verbessert</span><span class="sxs-lookup"><span data-stu-id="5f12f-3047">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="5f12f-3048">Unterstützung für das Erstellen von Linux-Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3048">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="5f12f-3049">`list-locations` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="5f12f-3049">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="5f12f-3050">Batch</span><span class="sxs-lookup"><span data-stu-id="5f12f-3050">Batch</span></span>

* <span data-ttu-id="5f12f-3051">Fehler im Poolerstellungsbefehl korrigiert, der bei Verwendung einer Ressourcen-ID mit dem Flag `--image` aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="5f12f-3051">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="5f12f-3052">BatchAI</span><span class="sxs-lookup"><span data-stu-id="5f12f-3052">Batchai</span></span>

* <span data-ttu-id="5f12f-3053">Kurzoption (`-s`) für `--vm-size` zur Angabe der VM-Größe im Befehl `file-server create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3053">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="5f12f-3054">Argumente für Speicherkontoname und -schlüssel zum Parameter `cluster create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3054">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="5f12f-3055">Dokumentation für `job list-files` und `job stream-file` korrigiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-3055">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="5f12f-3056">Kurzoption (`-r`) für `--cluster-name` zur Angabe des Clusternamens im Befehl `job create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3056">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="5f12f-3057">Cloud</span><span class="sxs-lookup"><span data-stu-id="5f12f-3057">Cloud</span></span>

* <span data-ttu-id="5f12f-3058">`cloud [register|update]` geändert, um die Registrierung von Clouds ohne erforderliche Endpunkte zu verhindern</span><span class="sxs-lookup"><span data-stu-id="5f12f-3058">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="5f12f-3059">Container</span><span class="sxs-lookup"><span data-stu-id="5f12f-3059">Container</span></span>

* <span data-ttu-id="5f12f-3060">Unterstützung für das Öffnen mehrerer Ports hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3060">Added support to open multiple ports</span></span>
* <span data-ttu-id="5f12f-3061">Neustartrichtlinie für Containergruppen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3061">Added container group restart policy</span></span>
* <span data-ttu-id="5f12f-3062">Unterstützung zum Einbinden einer Azure-Dateifreigabe als Volume hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3062">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="5f12f-3063">Hilfedokumente aktualisiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-3063">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="5f12f-3064">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="5f12f-3064">Data Lake Analytics</span></span>

* <span data-ttu-id="5f12f-3065">`[job|account] list` geändert, um präzisere Informationen zu erhalten</span><span class="sxs-lookup"><span data-stu-id="5f12f-3065">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="5f12f-3066">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="5f12f-3066">Data Lake Store</span></span>

* <span data-ttu-id="5f12f-3067">`account list` geändert, um präzisere Informationen zu erhalten</span><span class="sxs-lookup"><span data-stu-id="5f12f-3067">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="5f12f-3068">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="5f12f-3068">Extension</span></span>

* <span data-ttu-id="5f12f-3069">`extension list-available` hinzugefügt, um das Auflisten offizieller Microsoft-Erweiterungen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="5f12f-3069">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="5f12f-3070">`--name` zu `extension [add|update]` hinzugefügt, um das Installieren von Erweiterungen nach Name zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="5f12f-3070">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="5f12f-3071">IoT</span><span class="sxs-lookup"><span data-stu-id="5f12f-3071">IoT</span></span>

* <span data-ttu-id="5f12f-3072">Unterstützung für Zertifizierungsstellen (CAs) und Zertifikatketten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3072">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="5f12f-3073">Überwachen</span><span class="sxs-lookup"><span data-stu-id="5f12f-3073">Monitor</span></span>

* <span data-ttu-id="5f12f-3074">Befehle vom Typ `activity-log alert` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3074">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="5f12f-3075">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="5f12f-3075">Network</span></span>

* <span data-ttu-id="5f12f-3076">Unterstützung für CAA-DNS-Einträge hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3076">Added support for CAA DNS records</span></span>
* <span data-ttu-id="5f12f-3077">Problem behoben, durch das Endpunkte nicht mit `traffic-manager profile update` aktualisiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="5f12f-3077">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="5f12f-3078">Problem behoben, durch das `vnet update --dns-servers` je nach VNet-Erstellungsmethode nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="5f12f-3078">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="5f12f-3079">Problem behoben, durch das relative DNS-Namen durch `dns zone import` nicht korrekt importiert wurden</span><span class="sxs-lookup"><span data-stu-id="5f12f-3079">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="5f12f-3080">Reservations</span><span class="sxs-lookup"><span data-stu-id="5f12f-3080">Reservations</span></span>

* <span data-ttu-id="5f12f-3081">Erste Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="5f12f-3081">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="5f12f-3082">Resource</span><span class="sxs-lookup"><span data-stu-id="5f12f-3082">Resource</span></span>

* <span data-ttu-id="5f12f-3083">Unterstützung für Ressourcen-IDs zum Parameter `--resource` und Sperren auf Ressourcenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3083">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="5f12f-3084">SQL</span><span class="sxs-lookup"><span data-stu-id="5f12f-3084">SQL</span></span>

* <span data-ttu-id="5f12f-3085">Parameter `--ignore-missing-vnet-service-endpoint` zu `sql server vnet-rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3085">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="5f12f-3086">Storage</span><span class="sxs-lookup"><span data-stu-id="5f12f-3086">Storage</span></span>

* <span data-ttu-id="5f12f-3087">`storage account create` geändert, sodass die SKU `Standard_RAGRS` als Standard verwendet wird</span><span class="sxs-lookup"><span data-stu-id="5f12f-3087">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="5f12f-3088">Fehler im Zusammenhang mit Datei-/Blobnamen korrigiert, die ASCII-fremde Zeichen enthalten</span><span class="sxs-lookup"><span data-stu-id="5f12f-3088">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="5f12f-3089">Fehler korrigiert, der die Verwendung von `--source-uri` mit `storage [blob|file] copy start-batch` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="5f12f-3089">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="5f12f-3090">Befehle zum Globalisieren und Löschen mehrerer Objekte mit `storage [blob|file] delete-batch` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3090">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="5f12f-3091">Problem beim Aktivieren von Metriken mit `storage metrics update` behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-3091">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="5f12f-3092">Problem mit Dateien über 200 GB bei Verwendung von `storage blob upload-batch` behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-3092">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="5f12f-3093">Problem behoben, durch das `--bypass` und `--default-action` von `storage account [create|update]` ignoriert wurden</span><span class="sxs-lookup"><span data-stu-id="5f12f-3093">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="5f12f-3094">VM</span><span class="sxs-lookup"><span data-stu-id="5f12f-3094">VM</span></span>

* <span data-ttu-id="5f12f-3095">Fehler mit `vmss create` korrigiert, der die Verwendung der Größenebene `Basic` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="5f12f-3095">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="5f12f-3096">`--plan`-Argumente zu `[vm|vmss] create` für benutzerdefinierte Images mit Abrechnungsinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3096">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="5f12f-3097">Befehle hinzugefügt: `vm secret `[add|remove|list]</span><span class="sxs-lookup"><span data-stu-id="5f12f-3097">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="5f12f-3098">`vm format-secret` in `vm secret format` umbenannt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3098">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="5f12f-3099">Argument `--encrypt format` zu `vm encryption enable` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3099">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="5f12f-3100">24. Oktober 2017</span><span class="sxs-lookup"><span data-stu-id="5f12f-3100">October 24, 2017</span></span>

<span data-ttu-id="5f12f-3101">Version 2.0.20</span><span class="sxs-lookup"><span data-stu-id="5f12f-3101">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="5f12f-3102">Core</span><span class="sxs-lookup"><span data-stu-id="5f12f-3102">Core</span></span>

* <span data-ttu-id="5f12f-3103">Aktualisierung von `2017-03-09-profile` zur Verwendung von Version `2016-01-01` der `MGMT_STORAGE`-API</span><span class="sxs-lookup"><span data-stu-id="5f12f-3103">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="5f12f-3104">ACR</span><span class="sxs-lookup"><span data-stu-id="5f12f-3104">ACR</span></span>

* <span data-ttu-id="5f12f-3105">Die Ressourcenverwaltung wurde aktualisiert und verweist nun auf die API-Version `2017-10-01`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-3105">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="5f12f-3106">SKU „Bring Your Own Storage“ wurde in „Klassisch“ geändert.</span><span class="sxs-lookup"><span data-stu-id="5f12f-3106">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="5f12f-3107">Die Registrierungs-SKUs wurden in „Basic“, „Standard“ und „Premium“ umbenannt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-3107">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="5f12f-3108">ACS</span><span class="sxs-lookup"><span data-stu-id="5f12f-3108">ACS</span></span>

* <span data-ttu-id="5f12f-3109">[VORSCHAUVERSION] Befehle vom Typ `az aks` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3109">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="5f12f-3110">Problem mit `get-credentials` in Kubernetes behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-3110">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="5f12f-3111">AppService</span><span class="sxs-lookup"><span data-stu-id="5f12f-3111">Appservice</span></span>

* <span data-ttu-id="5f12f-3112">Problem behoben, aufgrund dessen heruntergeladene `webapp`-Protokolle unter Umständen ungültig waren</span><span class="sxs-lookup"><span data-stu-id="5f12f-3112">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="5f12f-3113">Komponente</span><span class="sxs-lookup"><span data-stu-id="5f12f-3113">Component</span></span>

* <span data-ttu-id="5f12f-3114">Deutlichere Meldung zur Einstellung für alle Installer und für Bestätigungsaufforderung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3114">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="5f12f-3115">Überwachen</span><span class="sxs-lookup"><span data-stu-id="5f12f-3115">Monitor</span></span>

* <span data-ttu-id="5f12f-3116">Befehle vom Typ `action-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3116">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="5f12f-3117">Resource</span><span class="sxs-lookup"><span data-stu-id="5f12f-3117">Resource</span></span>

* <span data-ttu-id="5f12f-3118">Inkompatibilität mit der aktuellen Version der msrest-Abhängigkeit in `group export` behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-3118">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="5f12f-3119">Problem mit `policy assignment create` behoben, sodass der Befehl mit integrierten Richtliniendefinitionen und Richtliniensatzdefinitionen verwendet werden kann</span><span class="sxs-lookup"><span data-stu-id="5f12f-3119">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="5f12f-3120">VM</span><span class="sxs-lookup"><span data-stu-id="5f12f-3120">VM</span></span>

* <span data-ttu-id="5f12f-3121">Argument `--accelerated-networking` zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3121">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="5f12f-3122">9\. Oktober 2017</span><span class="sxs-lookup"><span data-stu-id="5f12f-3122">October 9, 2017</span></span>

<span data-ttu-id="5f12f-3123">Version 2.0.19</span><span class="sxs-lookup"><span data-stu-id="5f12f-3123">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="5f12f-3124">Core</span><span class="sxs-lookup"><span data-stu-id="5f12f-3124">Core</span></span>

* <span data-ttu-id="5f12f-3125">Verarbeitung von ADFS-Autoritäts-URLs wurde mit einem nachgestellten Schrägstrich zu Azure Stack hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-3125">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="5f12f-3126">AppService</span><span class="sxs-lookup"><span data-stu-id="5f12f-3126">Appservice</span></span>

* <span data-ttu-id="5f12f-3127">Mit dem neuen Befehl `webapp update` wurde ein allgemeines Update hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-3127">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="5f12f-3128">Batch</span><span class="sxs-lookup"><span data-stu-id="5f12f-3128">Batch</span></span>

* <span data-ttu-id="5f12f-3129">Aktualisierung auf Batch SDK 4.0.0</span><span class="sxs-lookup"><span data-stu-id="5f12f-3129">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="5f12f-3130">Die Option `--image` von „VirtualMachineConfiguration“ wurde aktualisiert, um zusätzlich zu „publish:offer:sku:version“ ARM-Imageverweise zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="5f12f-3130">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="5f12f-3131">Unterstützung für das neue CLI-Erweiterungsmodell für Batch-Erweiterungsbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3131">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="5f12f-3132">Batch-Unterstützung aus dem Komponentenmodell entfernt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3132">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="5f12f-3133">BatchAI</span><span class="sxs-lookup"><span data-stu-id="5f12f-3133">Batchai</span></span>

* <span data-ttu-id="5f12f-3134">Erste Version des Batch KI-Moduls</span><span class="sxs-lookup"><span data-stu-id="5f12f-3134">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="5f12f-3135">KeyVault</span><span class="sxs-lookup"><span data-stu-id="5f12f-3135">Keyvault</span></span>

* <span data-ttu-id="5f12f-3136">Key Vault-Authentifizierungsproblem behoben, das bei Verwendung von ADFS in Azure Stack auftrat.</span><span class="sxs-lookup"><span data-stu-id="5f12f-3136">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="5f12f-3137">(#4448)</span><span class="sxs-lookup"><span data-stu-id="5f12f-3137">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="5f12f-3138">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="5f12f-3138">Network</span></span>

* <span data-ttu-id="5f12f-3139">Das Argument `--server` von `application-gateway address-pool create` ist nun optional, sodass leere Adresspools zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="5f12f-3139">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="5f12f-3140">`traffic-manager` wurde aktualisiert, um aktuelle Features zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="5f12f-3140">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="5f12f-3141">Resource</span><span class="sxs-lookup"><span data-stu-id="5f12f-3141">Resource</span></span>

* <span data-ttu-id="5f12f-3142">Zusätzliche Unterstützung für `--resource-group/-g`-Optionen für Ressourcengruppennamen zu `group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3142">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="5f12f-3143">Befehle für `account lock` hinzugefügt, um die Verwendung mit Sperren auf Abonnementebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="5f12f-3143">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="5f12f-3144">Befehle für `group lock` hinzugefügt, um die Verwendung mit Sperren auf Gruppenebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="5f12f-3144">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="5f12f-3145">Befehle für `resource lock` hinzugefügt, um die Verwendung mit Sperren auf Ressourcenebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="5f12f-3145">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="5f12f-3146">Sql</span><span class="sxs-lookup"><span data-stu-id="5f12f-3146">Sql</span></span>

* <span data-ttu-id="5f12f-3147">Unterstützung für SQL Transparent Data Encryption (TDE) und TDE für Bring Your Own Key-Szenarien hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3147">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="5f12f-3148">Der Befehl `db list-deleted` und der Parameter `db restore --deleted-time` wurden hinzugefügt, um die Ermittlung und Wiederherstellung gelöschter Datenbanken zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="5f12f-3148">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="5f12f-3149">`db op list` und `db op cancel` wurden hinzugefügt, um das Auflisten und Abbrechen ausgeführter Vorgänge für eine Datenbank zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="5f12f-3149">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="5f12f-3150">Storage</span><span class="sxs-lookup"><span data-stu-id="5f12f-3150">Storage</span></span>

* <span data-ttu-id="5f12f-3151">Unterstützung für Momentaufnahme von Dateifreigaben hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3151">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="5f12f-3152">VM</span><span class="sxs-lookup"><span data-stu-id="5f12f-3152">Vm</span></span>

* <span data-ttu-id="5f12f-3153">Korrektur eines Fehlers in `vm show`, bei dem die Verwendung von `-d` in Verbindung mit fehlenden privaten IP-Adressen einen Absturz verursachte</span><span class="sxs-lookup"><span data-stu-id="5f12f-3153">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="5f12f-3154">[VORSCHAUVERSION] Unterstützung für paralleles Upgrade zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3154">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="5f12f-3155">Unterstützung für das Aktualisieren der Verschlüsselungseinstellungen mit `vm encryption enable` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3155">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="5f12f-3156">Parameter `--os-disk-size-gb` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3156">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="5f12f-3157">Parameter `--license-type` für Windows zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3157">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="5f12f-3158">22. September 2017</span><span class="sxs-lookup"><span data-stu-id="5f12f-3158">September 22, 2017</span></span>

<span data-ttu-id="5f12f-3159">Version 2.0.18</span><span class="sxs-lookup"><span data-stu-id="5f12f-3159">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="5f12f-3160">Resource</span><span class="sxs-lookup"><span data-stu-id="5f12f-3160">Resource</span></span>

* <span data-ttu-id="5f12f-3161">Unterstützung für das Anzeigen integrierter Richtliniendefinitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3161">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="5f12f-3162">Unterstützungsmodusparameter zum Erstellen von Richtliniendefinitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3162">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="5f12f-3163">Unterstützung für UI-Definitionen und -Vorlagen zu `managedapp definition create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3163">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="5f12f-3164">[BREAKING CHANGE] Der Ressourcentyp `managedapp` wurde von `appliances` in `applications` und von `applianceDefinitions` in `applicationDefinitions` geändert.</span><span class="sxs-lookup"><span data-stu-id="5f12f-3164">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="5f12f-3165">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="5f12f-3165">Network</span></span>

* <span data-ttu-id="5f12f-3166">Unterstützung für Verfügbarkeitszone zu Unterbefehlen `network lb` und `network public-ip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3166">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="5f12f-3167">Unterstützung für IPv6-Microsoft-Peering zu `express-route` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3167">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="5f12f-3168">Befehle für Anwendungssicherheitsgruppe `asg` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3168">Added `asg` application security group commands</span></span>
* <span data-ttu-id="5f12f-3169">Argument `--application-security-groups` zu `nic [create|ip-config create|ip-config update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3169">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="5f12f-3170">Argumente `--source-asgs` und `--destination-asgs` zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3170">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="5f12f-3171">Argumente `--ddos-protection` und `--vm-protection` zu `vnet [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3171">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="5f12f-3172">Befehle vom Typ `network [vnet-gateway|vpn-client|show-url]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3172">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="5f12f-3173">Storage</span><span class="sxs-lookup"><span data-stu-id="5f12f-3173">Storage</span></span>

* <span data-ttu-id="5f12f-3174">Problem behoben, das nach der Aktualisierung des SDK unter Umständen einen Fehler der `storage account network-rule`-Befehle zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="5f12f-3174">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="5f12f-3175">Eventgrid</span><span class="sxs-lookup"><span data-stu-id="5f12f-3175">Eventgrid</span></span>

* <span data-ttu-id="5f12f-3176">Azure Event Grid Python SDK für die Verwendung der neueren API-Version „2017-09-15-preview“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-3176">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="5f12f-3177">SQL</span><span class="sxs-lookup"><span data-stu-id="5f12f-3177">SQL</span></span>

* <span data-ttu-id="5f12f-3178">`sql server list`-Argument `--resource-group` geändert, sodass es nun optional ist.</span><span class="sxs-lookup"><span data-stu-id="5f12f-3178">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="5f12f-3179">Wird es nicht angegeben, werden alle SQL Server-Instanzen im Abonnement zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5f12f-3179">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="5f12f-3180">Parameter `--no-wait` zu `db [create|copy|restore|update|replica create|create|update]` und `dw [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3180">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="5f12f-3181">KeyVault</span><span class="sxs-lookup"><span data-stu-id="5f12f-3181">Keyvault</span></span>

* <span data-ttu-id="5f12f-3182">Unterstützung für die Keyvault-Befehlsausführung hinter einem Proxy hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3182">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="5f12f-3183">VM</span><span class="sxs-lookup"><span data-stu-id="5f12f-3183">VM</span></span>

* <span data-ttu-id="5f12f-3184">Unterstützung für Verfügbarkeitszone zu `[vm|vmss|disk] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3184">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="5f12f-3185">Problem behoben, das bei Verwendung von `--app-gateway ID` mit `vmss create` einen Fehler zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="5f12f-3185">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="5f12f-3186">Argument `--asgs` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3186">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="5f12f-3187">Unterstützung für die Ausführung von Befehlen auf virtuellen Computern mit `vm run-command` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3187">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="5f12f-3188">[VORSCHAU] Unterstützung für VMSS-Datenträgerverschlüsselung mit `vmss encryption` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3188">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="5f12f-3189">Unterstützung für die Durchführung der Wartung auf virtuellen Computern mit `vm perform-maintenance` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3189">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="5f12f-3190">ACS</span><span class="sxs-lookup"><span data-stu-id="5f12f-3190">ACS</span></span>

* <span data-ttu-id="5f12f-3191">[VORSCHAU] Argument `--orchestrator-release` zu `acs create` für ACS-Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3191">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="5f12f-3192">AppService</span><span class="sxs-lookup"><span data-stu-id="5f12f-3192">Appservice</span></span>

* <span data-ttu-id="5f12f-3193">Neue Möglichkeit zum Aktualisieren und Anzeigen der Authentifizierungseinstellungen mit `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="5f12f-3193">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="5f12f-3194">Backup</span><span class="sxs-lookup"><span data-stu-id="5f12f-3194">Backup</span></span>

* <span data-ttu-id="5f12f-3195">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="5f12f-3195">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="5f12f-3196">11. September 2017</span><span class="sxs-lookup"><span data-stu-id="5f12f-3196">September 11, 2017</span></span>

<span data-ttu-id="5f12f-3197">Version 2.0.17</span><span class="sxs-lookup"><span data-stu-id="5f12f-3197">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="5f12f-3198">Core</span><span class="sxs-lookup"><span data-stu-id="5f12f-3198">Core</span></span>

* <span data-ttu-id="5f12f-3199">Festlegung einer eigenen Korrelations-ID in Telemetrie durch das Befehlsmodul aktiviert</span><span class="sxs-lookup"><span data-stu-id="5f12f-3199">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="5f12f-3200">Ein Problem mit der JSON-Sicherungsdatei wurde behoben, das beim Festlegen des Diagnosemodus für Telemetrie auftrat</span><span class="sxs-lookup"><span data-stu-id="5f12f-3200">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="5f12f-3201">ACS</span><span class="sxs-lookup"><span data-stu-id="5f12f-3201">Acs</span></span>

* <span data-ttu-id="5f12f-3202">Befehl `acs list-locations` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3202">Added `acs list-locations` command</span></span>
* <span data-ttu-id="5f12f-3203">`ssh-key-file` wird mit dem erwarteten Standardwert versehen.</span><span class="sxs-lookup"><span data-stu-id="5f12f-3203">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="5f12f-3204">AppService</span><span class="sxs-lookup"><span data-stu-id="5f12f-3204">Appservice</span></span>

* <span data-ttu-id="5f12f-3205">Neue Möglichkeit zum Erstellen einer Web-App in einer anderen Ressourcengruppe als der des aktiven Diensttarifs</span><span class="sxs-lookup"><span data-stu-id="5f12f-3205">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="5f12f-3206">CDN</span><span class="sxs-lookup"><span data-stu-id="5f12f-3206">CDN</span></span>

* <span data-ttu-id="5f12f-3207">Der Fehler bei `cdn custom-domain create`, dass „CustomDomain“ nicht wiederholbar ist, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="5f12f-3207">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="5f12f-3208">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="5f12f-3208">Extension</span></span>

* <span data-ttu-id="5f12f-3209">Erstrelease</span><span class="sxs-lookup"><span data-stu-id="5f12f-3209">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="5f12f-3210">KeyVault</span><span class="sxs-lookup"><span data-stu-id="5f12f-3210">Keyvault</span></span>

* <span data-ttu-id="5f12f-3211">Problem behoben, aufgrund dessen bei den Berechtigungen für `keyvault set-policy` die Groß-/Kleinschreibung beachtet werden musste</span><span class="sxs-lookup"><span data-stu-id="5f12f-3211">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="5f12f-3212">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="5f12f-3212">Network</span></span>

* <span data-ttu-id="5f12f-3213">`vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3213">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="5f12f-3214">Das Argument `--private-access-services` wurde für `vnet subnet create/update` in `--service-endpoints` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-3214">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="5f12f-3215">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3215">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="5f12f-3216">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3216">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="5f12f-3217">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3217">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="5f12f-3218">Resource</span><span class="sxs-lookup"><span data-stu-id="5f12f-3218">Resource</span></span>

* <span data-ttu-id="5f12f-3219">Übergabe von Parameterdefinitionen für Ressourcenrichtlinien in `policy definition create` und `policy definition update` zulassen</span><span class="sxs-lookup"><span data-stu-id="5f12f-3219">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="5f12f-3220">Übergabe von Parameterwerten für `policy assignment create` zulassen</span><span class="sxs-lookup"><span data-stu-id="5f12f-3220">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="5f12f-3221">Übergabe von JSON-Code oder einer Datei für alle Parameter zulassen</span><span class="sxs-lookup"><span data-stu-id="5f12f-3221">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="5f12f-3222">Inkrementierte API-Version</span><span class="sxs-lookup"><span data-stu-id="5f12f-3222">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="5f12f-3223">SQL</span><span class="sxs-lookup"><span data-stu-id="5f12f-3223">SQL</span></span>

* <span data-ttu-id="5f12f-3224">Befehle vom Typ `sql server vnet-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3224">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="5f12f-3225">VM</span><span class="sxs-lookup"><span data-stu-id="5f12f-3225">VM</span></span>

* <span data-ttu-id="5f12f-3226">Behoben: Zugriff nur zuweisen, wenn `--scope` angegeben wird</span><span class="sxs-lookup"><span data-stu-id="5f12f-3226">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="5f12f-3227">Behoben: Gleiche Erweiterungsbenennung wie Portal verwenden</span><span class="sxs-lookup"><span data-stu-id="5f12f-3227">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="5f12f-3228">`subscription` aus der Ausgabe von `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3228">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="5f12f-3229">Behoben: Speicher-SKU vom Typ `[vm|vmss] create` wird nicht auf Datenträger mit einem Image angewendet.</span><span class="sxs-lookup"><span data-stu-id="5f12f-3229">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="5f12f-3230">Behoben: `vm format-secret --secrets` akzeptierte keine durch neue Zeilen getrennte IDs.</span><span class="sxs-lookup"><span data-stu-id="5f12f-3230">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="5f12f-3231">31. August 2017</span><span class="sxs-lookup"><span data-stu-id="5f12f-3231">August 31, 2017</span></span>

<span data-ttu-id="5f12f-3232">Version 2.0.16</span><span class="sxs-lookup"><span data-stu-id="5f12f-3232">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="5f12f-3233">KeyVault</span><span class="sxs-lookup"><span data-stu-id="5f12f-3233">Keyvault</span></span>

* <span data-ttu-id="5f12f-3234">Fehler behoben, der beim Versuch auftrat, die Geheimniscodierung mit `secret download` automatisch aufzulösen</span><span class="sxs-lookup"><span data-stu-id="5f12f-3234">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="5f12f-3235">Sf</span><span class="sxs-lookup"><span data-stu-id="5f12f-3235">Sf</span></span>

* <span data-ttu-id="5f12f-3236">Alle Befehle wurden durch die Service Fabric-Befehlszeilenschnittstelle (sfctl) ersetzt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-3236">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="5f12f-3237">Storage</span><span class="sxs-lookup"><span data-stu-id="5f12f-3237">Storage</span></span>

* <span data-ttu-id="5f12f-3238">Problem behoben, aufgrund dessen Speicherkonten nicht in Regionen erstellt werden konnten, die die NetworkACLs-Funktion nicht unterstützen</span><span class="sxs-lookup"><span data-stu-id="5f12f-3238">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="5f12f-3239">Festlegen des Inhaltstyps und der Inhaltscodierung während Blob- und Dateiuploads, wenn weder Inhaltstyp noch Inhaltscodierung angegeben sind</span><span class="sxs-lookup"><span data-stu-id="5f12f-3239">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="5f12f-3240">28. August 2017</span><span class="sxs-lookup"><span data-stu-id="5f12f-3240">August 28, 2017</span></span>

<span data-ttu-id="5f12f-3241">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="5f12f-3241">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="5f12f-3242">Befehlszeilenschnittstelle (CLI)</span><span class="sxs-lookup"><span data-stu-id="5f12f-3242">CLI</span></span>

* <span data-ttu-id="5f12f-3243">Rechtlichen Hinweis zu `--version` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3243">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="5f12f-3244">ACS</span><span class="sxs-lookup"><span data-stu-id="5f12f-3244">ACS</span></span>

* <span data-ttu-id="5f12f-3245">Vorschauregionen korrigiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-3245">Corrected preview regions</span></span>
* <span data-ttu-id="5f12f-3246">Standardmäßiges DNS-Namenspräfix (`dns_name_prefix`) ordnungsgemäß formatiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-3246">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="5f12f-3247">ACS-Befehlsausgabe optimiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-3247">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="5f12f-3248">AppService</span><span class="sxs-lookup"><span data-stu-id="5f12f-3248">Appservice</span></span>

* <span data-ttu-id="5f12f-3249">[BREAKING CHANGE] Inkonsistenzen in der Ausgabe von `az webapp config appsettings [delete|set]` behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-3249">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="5f12f-3250">Neuen Alias (`-i`) für `az webapp config container set --docker-custom-image-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3250">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="5f12f-3251">`az webapp log show` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="5f12f-3251">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="5f12f-3252">Neue Argumente aus `az webapp delete` verfügbar gemacht, um App Service-Plan, Metriken oder DNS-Registrierung beizubehalten</span><span class="sxs-lookup"><span data-stu-id="5f12f-3252">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="5f12f-3253">Behoben: Korrekte Erkennung der Sloteinstellungen</span><span class="sxs-lookup"><span data-stu-id="5f12f-3253">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="5f12f-3254">IoT</span><span class="sxs-lookup"><span data-stu-id="5f12f-3254">IoT</span></span>

* <span data-ttu-id="5f12f-3255">#3934 behoben: Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="5f12f-3255">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="5f12f-3256">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="5f12f-3256">Network</span></span>

* <span data-ttu-id="5f12f-3257">[BREAKING CHANGE]`vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3257">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="5f12f-3258">[BREAKING CHANGE] Option `--private-access-services` für `--service-endpoints` in `vnet subnet [create|update]` umbenannt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3258">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="5f12f-3259">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3259">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="5f12f-3260">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3260">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="5f12f-3261">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3261">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="5f12f-3262">Profil</span><span class="sxs-lookup"><span data-stu-id="5f12f-3262">Profile</span></span>

* <span data-ttu-id="5f12f-3263">`--msi` und `--msi-port` für die Anmeldung mit der Identität eines virtuellen Computers verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="5f12f-3263">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="5f12f-3264">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="5f12f-3264">Service Fabric</span></span>

* <span data-ttu-id="5f12f-3265">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="5f12f-3265">Preview release</span></span>
* <span data-ttu-id="5f12f-3266">Registrierungsbenutzer-/-kennwortregeln für Befehl vereinfacht</span><span class="sxs-lookup"><span data-stu-id="5f12f-3266">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="5f12f-3267">Kennwortanforderung für Benutzer trotz Parameterübergabe behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-3267">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="5f12f-3268">Unterstützung für leere Registrierungsanmeldeinformationen (`registry_cred`) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3268">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="5f12f-3269">Storage</span><span class="sxs-lookup"><span data-stu-id="5f12f-3269">Storage</span></span>

* <span data-ttu-id="5f12f-3270">Festlegen des Blobtarifs ermöglicht</span><span class="sxs-lookup"><span data-stu-id="5f12f-3270">Enabled setting blob tier</span></span>
* <span data-ttu-id="5f12f-3271">Argumente `--bypass` und `--default-action` zur Unterstützung von Diensttunneling zu `storage account [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3271">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="5f12f-3272">Befehle zum Hinzufügen von VNet-Regeln und IP-basierten Regeln zu `storage account network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3272">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="5f12f-3273">Dienstverschlüsselung durch vom Kunden verwalteten Schlüssel ermöglicht</span><span class="sxs-lookup"><span data-stu-id="5f12f-3273">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="5f12f-3274">[BREAKING CHANGE] Option `--encryption` für Befehl `az storage account create and az storage account update` in `--encryption-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3274">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="5f12f-3275">Behoben (4220): `az storage account update encryption` – Syntaxkonflikt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3275">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="5f12f-3276">VM</span><span class="sxs-lookup"><span data-stu-id="5f12f-3276">VM</span></span>

* <span data-ttu-id="5f12f-3277">Problem behoben, aufgrund dessen bei Verwendung von `--instance-id *` zusätzliche, fehlerhafte Informationen für `vmss get-instance-view` angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="5f12f-3277">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="5f12f-3278">Unterstützung für `--lb-sku` zu `vmss create` hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="5f12f-3278">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="5f12f-3279">Menschliche Namen aus der Administratornamen-Blacklist für `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3279">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="5f12f-3280">Problem behoben, aufgrund dessen `[vm|vmss] create` einen Fehler ausgelöst hat, wenn aus einem Image keine Tarifinformationen extrahiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="5f12f-3280">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="5f12f-3281">Absturzproblem beim Erstellen einer VMMS-Skalierungsgruppe mit einem internen Lastenausgleich behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-3281">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="5f12f-3282">Problem behoben, aufgrund dessen das Argument `--no-wait` nicht mit `vm availability-set create` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="5f12f-3282">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="5f12f-3283">15. August 2017</span><span class="sxs-lookup"><span data-stu-id="5f12f-3283">August 15, 2017</span></span>

<span data-ttu-id="5f12f-3284">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="5f12f-3284">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="5f12f-3285">ACS</span><span class="sxs-lookup"><span data-stu-id="5f12f-3285">ACS</span></span>

* <span data-ttu-id="5f12f-3286">sshMaster0-Portnummer für Kubernetes korrigiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-3286">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="5f12f-3287">AppService</span><span class="sxs-lookup"><span data-stu-id="5f12f-3287">Appservice</span></span>

* <span data-ttu-id="5f12f-3288">Ausnahme beim Erstellen einer neuen Git-basierten Linux-Web-App behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-3288">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="5f12f-3289">Event Grid</span><span class="sxs-lookup"><span data-stu-id="5f12f-3289">Event Grid</span></span>

* <span data-ttu-id="5f12f-3290">SDK-Abhängigkeiten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3290">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="5f12f-3291">11. August 2017</span><span class="sxs-lookup"><span data-stu-id="5f12f-3291">August 11, 2017</span></span>

<span data-ttu-id="5f12f-3292">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="5f12f-3292">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="5f12f-3293">ACS</span><span class="sxs-lookup"><span data-stu-id="5f12f-3293">ACS</span></span>

* <span data-ttu-id="5f12f-3294">Weitere Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3294">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="5f12f-3295">Batch</span><span class="sxs-lookup"><span data-stu-id="5f12f-3295">Batch</span></span>

* <span data-ttu-id="5f12f-3296">Auf Batch SDK 3.1.0 und Batch Management SDK 4.1.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-3296">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="5f12f-3297">Neuen Befehl zum Anzeigen der Aufgabenanzahl eines Auftrags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3297">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="5f12f-3298">Fehler in der SAS-URL-Verarbeitung der Ressourcendatei behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-3298">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="5f12f-3299">Batch-Kontoendpunkt unterstützt nun optionales Präfix „https://“</span><span class="sxs-lookup"><span data-stu-id="5f12f-3299">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="5f12f-3300">Unterstützung für das Hinzufügen von Listen mit mehr als 100 Aufgaben zu einem Auftrag</span><span class="sxs-lookup"><span data-stu-id="5f12f-3300">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="5f12f-3301">Debugprotokollierung für das Laden des Erweiterungsbefehlsmoduls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3301">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="5f12f-3302">Komponente</span><span class="sxs-lookup"><span data-stu-id="5f12f-3302">Component</span></span>

* <span data-ttu-id="5f12f-3303">Warnung für veraltete Befehle vom Typ „az component“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3303">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="5f12f-3304">Container</span><span class="sxs-lookup"><span data-stu-id="5f12f-3304">Container</span></span>

* <span data-ttu-id="5f12f-3305">`create`: Problem behoben, aufgrund dessen das Gleichheitszeichen innerhalb einer Umgebungsvariablen nicht zulässig war</span><span class="sxs-lookup"><span data-stu-id="5f12f-3305">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="5f12f-3306">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="5f12f-3306">Data Lake Store</span></span>

* <span data-ttu-id="5f12f-3307">Fortschrittsüberwachung ermöglicht</span><span class="sxs-lookup"><span data-stu-id="5f12f-3307">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="5f12f-3308">Event Grid</span><span class="sxs-lookup"><span data-stu-id="5f12f-3308">Event Grid</span></span>

* <span data-ttu-id="5f12f-3309">Erste Veröffentlichung</span><span class="sxs-lookup"><span data-stu-id="5f12f-3309">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="5f12f-3310">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="5f12f-3310">Network</span></span>

* <span data-ttu-id="5f12f-3311">`lb`: Problem behoben, aufgrund dessen bestimmte Namen untergeordneter Ressourcen bei Auslassung nicht richtig aufgelöst wurden</span><span class="sxs-lookup"><span data-stu-id="5f12f-3311">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="5f12f-3312">`application-gateway {subresource} delete`: Problem behoben, aufgrund dessen `--no-wait` nicht berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="5f12f-3312">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="5f12f-3313">`application-gateway http-settings update`: Problem behoben, aufgrund dessen `--connection-draining-timeout` nicht deaktiviert werden konnte</span><span class="sxs-lookup"><span data-stu-id="5f12f-3313">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="5f12f-3314">Fehler behoben: Unerwartetes Schlüsselwortargument `sa_data_size_kilobyes` bei `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="5f12f-3314">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="5f12f-3315">Profil</span><span class="sxs-lookup"><span data-stu-id="5f12f-3315">Profile</span></span>

* <span data-ttu-id="5f12f-3316">`account list`: `--refresh` hinzugefügt, um die neuesten Abonnements vom Server zu synchronisieren</span><span class="sxs-lookup"><span data-stu-id="5f12f-3316">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="5f12f-3317">Storage</span><span class="sxs-lookup"><span data-stu-id="5f12f-3317">Storage</span></span>

* <span data-ttu-id="5f12f-3318">Aktualisieren des Speicherkontos mit vom System zugewiesener Identität ermöglicht</span><span class="sxs-lookup"><span data-stu-id="5f12f-3318">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="5f12f-3319">VM</span><span class="sxs-lookup"><span data-stu-id="5f12f-3319">VM</span></span>

* <span data-ttu-id="5f12f-3320">`availability-set`: Fehlerdomänenanzahl bei Konvertierung verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="5f12f-3320">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="5f12f-3321">Befehl `list-skus` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="5f12f-3321">Exposed `list-skus` command</span></span>
* <span data-ttu-id="5f12f-3322">Unterstützung der Identitätszuweisung ohne Erstellung von Rollenzuweisungen</span><span class="sxs-lookup"><span data-stu-id="5f12f-3322">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="5f12f-3323">Anwenden von Speicher-SKU beim Anfügen von Datenträgern</span><span class="sxs-lookup"><span data-stu-id="5f12f-3323">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="5f12f-3324">Standardmäßiger Betriebssystemdatenträger-Name und Speicher-SKU bei Verwendung verwalteter Datenträger entfernt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3324">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="5f12f-3325">28. Juli 2017</span><span class="sxs-lookup"><span data-stu-id="5f12f-3325">July 28, 2017</span></span>

<span data-ttu-id="5f12f-3326">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="5f12f-3326">Version 2.0.12</span></span>

* <span data-ttu-id="5f12f-3327">Containerbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3327">Added container commands</span></span>
* <span data-ttu-id="5f12f-3328">Abrechnungs- und Nutzungsmodule hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3328">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="5f12f-3329">Core</span><span class="sxs-lookup"><span data-stu-id="5f12f-3329">Core</span></span>

* <span data-ttu-id="5f12f-3330">Ausgabe von SDK-Authentifizierungsinformationen für Dienstprinzipale mit Zertifikaten</span><span class="sxs-lookup"><span data-stu-id="5f12f-3330">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="5f12f-3331">Ausnahmen beim Bereitstellungsfortschritt behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-3331">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="5f12f-3332">Verwendung des ARM-Endpunkts aus der aktuellen Cloud für die Erstellung des Abonnementclients</span><span class="sxs-lookup"><span data-stu-id="5f12f-3332">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="5f12f-3333">Gleichzeitige Verarbeitung der Datei „clouds.config“ verbessert (3636)</span><span class="sxs-lookup"><span data-stu-id="5f12f-3333">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="5f12f-3334">Aktualisierung der Clientanforderungs-ID für jede Befehlsausführung</span><span class="sxs-lookup"><span data-stu-id="5f12f-3334">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="5f12f-3335">Erstellung von Abonnementclients mit richtigem SDK-Profil (3635)</span><span class="sxs-lookup"><span data-stu-id="5f12f-3335">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="5f12f-3336">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="5f12f-3336">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="5f12f-3337">Unterstützung für Auswahl von Tabellenausgabefeldern über jmespath Abfrage hinzugefügt (3581)</span><span class="sxs-lookup"><span data-stu-id="5f12f-3337">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="5f12f-3338">Stummschaltung von Analyseargumenten und Anfügeverlauf mit Gesten verbessert (3434)</span><span class="sxs-lookup"><span data-stu-id="5f12f-3338">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="5f12f-3339">Erstellung von Abonnementclients mit richtigem SDK-Profil</span><span class="sxs-lookup"><span data-stu-id="5f12f-3339">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="5f12f-3340">Verschiebung aller vorhandenen Erfassungsdateien in den neuesten Ordner</span><span class="sxs-lookup"><span data-stu-id="5f12f-3340">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="5f12f-3341">Idempotenz für VM-/VMSS-Erstellung behoben (3586)</span><span class="sxs-lookup"><span data-stu-id="5f12f-3341">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="5f12f-3342">Bei Befehlspfaden wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="5f12f-3342">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="5f12f-3343">Bei bestimmten booleschen Parametern wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="5f12f-3343">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="5f12f-3344">Unterstützung der Anmeldung bei lokalem AD FS-Server wie Azure Stack</span><span class="sxs-lookup"><span data-stu-id="5f12f-3344">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="5f12f-3345">Gleichzeitige Schreibvorgänge in „clouds.config“ behoben (3255)</span><span class="sxs-lookup"><span data-stu-id="5f12f-3345">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="5f12f-3346">ACR</span><span class="sxs-lookup"><span data-stu-id="5f12f-3346">ACR</span></span>

* <span data-ttu-id="5f12f-3347">Befehl `show-usage` für verwaltete Registrierungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3347">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="5f12f-3348">Unterstützung der SKU-Aktualisierung für verwaltete Registrierungen</span><span class="sxs-lookup"><span data-stu-id="5f12f-3348">Support SKU update for managed registries</span></span>
* <span data-ttu-id="5f12f-3349">Verwaltete Registrierungen mit verwalteter SKU hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3349">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="5f12f-3350">Webhooks für verwaltete Registrierungen mit ACR-Webhook-Befehlsmodul hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3350">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="5f12f-3351">AAD-Authentifizierung mit ACR-Anmeldebefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3351">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="5f12f-3352">Löschbefehl für Docker-Repositorys, Manifeste und Tags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3352">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="5f12f-3353">ACS</span><span class="sxs-lookup"><span data-stu-id="5f12f-3353">ACS</span></span>

* <span data-ttu-id="5f12f-3354">Unterstützung der API-Version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="5f12f-3354">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="5f12f-3355">AppService</span><span class="sxs-lookup"><span data-stu-id="5f12f-3355">Appservice</span></span>

* <span data-ttu-id="5f12f-3356">Fehler behoben, aufgrund dessen die Auflistung der Linux-Web-App keine Werte zurückgegeben hat</span><span class="sxs-lookup"><span data-stu-id="5f12f-3356">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="5f12f-3357">Unterstützung für das Abrufen von Anmeldeinformationen aus dem ACR</span><span class="sxs-lookup"><span data-stu-id="5f12f-3357">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="5f12f-3358">Entfernung aller Befehle unter `appservice web`</span><span class="sxs-lookup"><span data-stu-id="5f12f-3358">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="5f12f-3359">Maskierung von Docker-Registrierungskennwörtern aus der Befehlsausgabe (3656)</span><span class="sxs-lookup"><span data-stu-id="5f12f-3359">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="5f12f-3360">Gewährleistung der fehlerfreien Verwendung des Standardbrowsers unter macOS (3623)</span><span class="sxs-lookup"><span data-stu-id="5f12f-3360">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="5f12f-3361">Verbesserung des Nutzens von `webapp log tail` und `webapp log download` (3624)</span><span class="sxs-lookup"><span data-stu-id="5f12f-3361">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="5f12f-3362">Befehl `traffic-routing` zum Konfigurieren des statischen Routings verfügbar gemacht (3566)</span><span class="sxs-lookup"><span data-stu-id="5f12f-3362">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="5f12f-3363">Zuverlässigkeit beim Konfigurieren der Quellcodeverwaltung verbessert (3245)</span><span class="sxs-lookup"><span data-stu-id="5f12f-3363">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="5f12f-3364">Nicht unterstütztes Argument `--node-version` aus `webapp config update` für Windows-Web-Apps entfernt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-3364">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="5f12f-3365">Verwenden Sie stattdessen `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="5f12f-3365">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="5f12f-3366">Batch</span><span class="sxs-lookup"><span data-stu-id="5f12f-3366">Batch</span></span>

* <span data-ttu-id="5f12f-3367">Auf Batch SDK 3.0.0 mit Unterstützung virtueller Computer mit niedriger Priorität in Pools aktualisiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-3367">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="5f12f-3368">`pool create`-Option `--target-dedicated` in `--target-dedicated-nodes` umbenannt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3368">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="5f12f-3369">`pool create`-Optionen `--target-low-priority-nodes` und `--application-licenses` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3369">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="5f12f-3370">CDN</span><span class="sxs-lookup"><span data-stu-id="5f12f-3370">CDN</span></span>

* <span data-ttu-id="5f12f-3371">Besser verständliche Fehlermeldung für `cdn endpoint list`, wenn das von `--profile-name` angegebene Profil nicht vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="5f12f-3371">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="5f12f-3372">Cloud</span><span class="sxs-lookup"><span data-stu-id="5f12f-3372">Cloud</span></span>

* <span data-ttu-id="5f12f-3373">API-Version des Cloudmetadaten-Endpunkts in das Format JJJJ-MM-TT umgewandelt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3373">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="5f12f-3374">Katalogendpunkt nicht erforderlich</span><span class="sxs-lookup"><span data-stu-id="5f12f-3374">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="5f12f-3375">Unterstützung für die Cloudregistrierung nur mit ARM-Endpunkt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3375">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="5f12f-3376">Option für `cloud set` bereitgestellt, um beim Auswählen der aktuellen Cloud das Profil auswählen zu können</span><span class="sxs-lookup"><span data-stu-id="5f12f-3376">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="5f12f-3377">`endpoint_vm_image_alias_doc` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="5f12f-3377">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="5f12f-3378">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="5f12f-3378">CosmosDB</span></span>

* <span data-ttu-id="5f12f-3379">Möglichkeit zum Erstellen einer Auflistung mit benutzerdefiniertem Partitionsschlüssel behoben</span><span class="sxs-lookup"><span data-stu-id="5f12f-3379">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="5f12f-3380">Unterstützung für Auflistungs-Standardgültigkeitsdauer hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3380">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="5f12f-3381">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="5f12f-3381">Data Lake Analytics</span></span>

* <span data-ttu-id="5f12f-3382">Zusätzliche Befehle für Compute-Richtlinienverwaltung unter der Überschrift `dla account compute-policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3382">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="5f12f-3383">`dla job pipeline show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3383">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="5f12f-3384">`dla job recurrence list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3384">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="5f12f-3385">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="5f12f-3385">Data Lake Store</span></span>

* <span data-ttu-id="5f12f-3386">Unterstützung für vom Benutzer verwaltete Schlüsseltresor-Schlüsselrotation in `dls account update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3386">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="5f12f-3387">Zugrunde liegende SDK-Version des Data Lake Store-Dateisystems aktualisiert, um ein Leistungsproblem zu behandeln</span><span class="sxs-lookup"><span data-stu-id="5f12f-3387">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="5f12f-3388">Befehl `dls enable-key-vault` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-3388">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="5f12f-3389">Dieser Befehl versucht, eine vom Benutzer angegebene Key Vault-Instanz zur Verschlüsselung der Daten in einem Data Lake Store-Konto zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="5f12f-3389">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="5f12f-3390">Interactive</span><span class="sxs-lookup"><span data-stu-id="5f12f-3390">Interactive</span></span>

* <span data-ttu-id="5f12f-3391">Startzeit durch Verwendung zwischengespeicherter Befehle verbessert</span><span class="sxs-lookup"><span data-stu-id="5f12f-3391">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="5f12f-3392">Testabdeckung verbessert</span><span class="sxs-lookup"><span data-stu-id="5f12f-3392">Increased test coverage</span></span>
* <span data-ttu-id="5f12f-3393">?-Geste erweitert, sodass sie auch in den nächsten Befehl eingefügt wird</span><span class="sxs-lookup"><span data-stu-id="5f12f-3393">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="5f12f-3394">Interaktive Fehler mit dem Profil „2017-03-09-profile-preview“ behoben (3587)</span><span class="sxs-lookup"><span data-stu-id="5f12f-3394">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="5f12f-3395">`--version` als Parameter für den interaktiven Modus zugelassen (3645)</span><span class="sxs-lookup"><span data-stu-id="5f12f-3395">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="5f12f-3396">Beseitigung von Fehlern im interaktiven Modus beim Abschluss von Überprüfungen (3570)</span><span class="sxs-lookup"><span data-stu-id="5f12f-3396">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="5f12f-3397">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="5f12f-3397">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="5f12f-3398">Flag `--progress` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3398">Added `--progress` flag</span></span>
* <span data-ttu-id="5f12f-3399">`--debug` und `--verbose` aus Abschlüssen entfernt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3399">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="5f12f-3400">`interactive` aus Abschlüssen entfernt (3324)</span><span class="sxs-lookup"><span data-stu-id="5f12f-3400">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="5f12f-3401">IoT</span><span class="sxs-lookup"><span data-stu-id="5f12f-3401">IoT</span></span>

* <span data-ttu-id="5f12f-3402">Behoben: Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="5f12f-3402">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="5f12f-3403">(3934)</span><span class="sxs-lookup"><span data-stu-id="5f12f-3403">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="5f12f-3404">Schlüsseltresor</span><span class="sxs-lookup"><span data-stu-id="5f12f-3404">Key vault</span></span>

* <span data-ttu-id="5f12f-3405">Befehle für Schlüsseltresor-Wiederherstellungsfeatures hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="5f12f-3405">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="5f12f-3406">`keyvault`-Unterbefehle: `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="5f12f-3406">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="5f12f-3407">`keyvault secret`-Unterbefehle: `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="5f12f-3407">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="5f12f-3408">`keyvault certificate`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="5f12f-3408">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="5f12f-3409">`keyvault key`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="5f12f-3409">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="5f12f-3410">Dienstprinzipal-Schlüsseltresorintegration hinzugefügt (3133)</span><span class="sxs-lookup"><span data-stu-id="5f12f-3410">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="5f12f-3411">Schlüsseltresor-Datenebene auf 0.3.2. aktualisiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-3411">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="5f12f-3412">(3307)</span><span class="sxs-lookup"><span data-stu-id="5f12f-3412">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="5f12f-3413">Labor</span><span class="sxs-lookup"><span data-stu-id="5f12f-3413">Lab</span></span>

* <span data-ttu-id="5f12f-3414">Unterstützung für Übernahme eines beliebigen virtuellen Computers im Labor über `az lab vm claim` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3414">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="5f12f-3415">Tabellenausgabeformatierer für `az lab vm list` und `az lab vm show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3415">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="5f12f-3416">Überwachen</span><span class="sxs-lookup"><span data-stu-id="5f12f-3416">Monitor</span></span>

* <span data-ttu-id="5f12f-3417">Korrektur für Vorlagendatei mit Befehl `monitor autoscale-settings get-parameters-template` (3349)</span><span class="sxs-lookup"><span data-stu-id="5f12f-3417">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="5f12f-3418">`monitor alert-rule-incidents list` in `monitor alert list-incidents` umbenannt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3418">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="5f12f-3419">`monitor alert-rule-incidents show` in `monitor alert show-incident` umbenannt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3419">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="5f12f-3420">`monitor metric-defintions list` in `monitor metrics list-definitions` umbenannt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3420">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="5f12f-3421">`monitor alert-rules` in `monitor alert` umbenannt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3421">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="5f12f-3422">`monitor alert create` geändert:</span><span class="sxs-lookup"><span data-stu-id="5f12f-3422">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="5f12f-3423">Unterbefehle vom Typ `condition` und `action` akzeptieren keinen JSON-Code mehr.</span><span class="sxs-lookup"><span data-stu-id="5f12f-3423">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="5f12f-3424">Hinzufügung zahlreicher Parameter zur Vereinfachung der Regelerstellung</span><span class="sxs-lookup"><span data-stu-id="5f12f-3424">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="5f12f-3425">`location` nicht mehr erforderlich</span><span class="sxs-lookup"><span data-stu-id="5f12f-3425">`location` no longer required</span></span>
  * <span data-ttu-id="5f12f-3426">Hinzufügung von Namen- und ID-Unterstützung für Ziel</span><span class="sxs-lookup"><span data-stu-id="5f12f-3426">Add name and ID support for target</span></span>
  * <span data-ttu-id="5f12f-3427">Entfernung von `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="5f12f-3427">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="5f12f-3428">Umbenennung von `is-enabled` in `enabled` (nicht mehr erforderlich)</span><span class="sxs-lookup"><span data-stu-id="5f12f-3428">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="5f12f-3429">`description` wird nun abhängig von der angegebenen Bedingung auf einen Standardwert festgelegt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-3429">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="5f12f-3430">Hinzufügung von Beispielen zur Verdeutlichung des neuen Formats</span><span class="sxs-lookup"><span data-stu-id="5f12f-3430">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="5f12f-3431">Unterstützung von Namen oder IDs für Befehle vom Typ `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="5f12f-3431">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="5f12f-3432">Komfortargumente und Beispiele zu `monitor alert rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3432">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="5f12f-3433">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="5f12f-3433">Network</span></span>

* <span data-ttu-id="5f12f-3434">Befehl `list-private-access-services` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3434">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="5f12f-3435">Argument `--private-access-services` zu `vnet subnet create` und `vnet subnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3435">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="5f12f-3436">Problem behoben, das einen Fehler für `application-gateway redirect-config create` zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="5f12f-3436">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="5f12f-3437">Problem behoben, aufgrund dessen `application-gateway redirect-config update` nicht mit `--no-wait` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="5f12f-3437">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="5f12f-3438">Fehler behoben, der bei der Verwendung des Arguments `--servers` mit `application-gateway address-pool create` und `application-gateway address-pool update` aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="5f12f-3438">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="5f12f-3439">Befehle vom Typ `application-gateway redirect-config` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3439">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="5f12f-3440">Befehle zu `application-gateway ssl-policy` hinzugefügt: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="5f12f-3440">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="5f12f-3441">Argumente zu `application-gateway ssl-policy set` hinzugefügt: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="5f12f-3441">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="5f12f-3442">Argumente zu `application-gateway http-settings create` und `application-gateway http-settings update` hinzugefügt: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="5f12f-3442">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="5f12f-3443">Argumente zu `application-gateway url-path-map create` und `application-gateway url-path-map update` hinzugefügt: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="5f12f-3443">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="5f12f-3444">Argument `--redirect-config` zu `application-gateway url-path-map rule create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3444">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="5f12f-3445">Unterstützung für `--no-wait` zu `application-gateway url-path-map rule delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3445">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="5f12f-3446">Argumente zu `application-gateway probe create` und `application-gateway probe update` hinzugefügt: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="5f12f-3446">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="5f12f-3447">Argument `--redirect-config` zu `application-gateway rule create` und `application-gateway rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3447">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="5f12f-3448">Unterstützung für `--accelerated-networking` zu `nic create` und `nic update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3448">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="5f12f-3449">Argument `--internal-dns-name-suffix` von `nic create` entfernt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3449">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="5f12f-3450">Unterstützung für `--dns-servers` zu `nic update` und `nic create` hinzugefügt: Hinzufügung von Unterstützung für --dns-servers</span><span class="sxs-lookup"><span data-stu-id="5f12f-3450">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="5f12f-3451">Fehler korrigiert, aufgrund dessen `--local-address-prefixes` von `local-gateway create` ignoriert wurde</span><span class="sxs-lookup"><span data-stu-id="5f12f-3451">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="5f12f-3452">Unterstützung für `--dns-servers` zu `vnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3452">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="5f12f-3453">Fehler beim Erstellen eines Peerings ohne Routenfilterung mit `express-route peering create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-3453">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="5f12f-3454">Fehler korrigiert, aufgrund dessen die Argumente `--provider` und `--bandwidth` nicht mit `express-route update` verwendet werden konnten</span><span class="sxs-lookup"><span data-stu-id="5f12f-3454">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="5f12f-3455">Fehler mit Standardlogik von `network watcher show-topology` korrigiert</span><span class="sxs-lookup"><span data-stu-id="5f12f-3455">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="5f12f-3456">Ausgabeformatierung für `network list-usages` verbessert</span><span class="sxs-lookup"><span data-stu-id="5f12f-3456">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="5f12f-3457">Verwendung der standardmäßigen Front-End-IP-Adresse für `application-gateway http-listener create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="5f12f-3457">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="5f12f-3458">Verwendung des Standardadresspools, der HTTP-Standardeinstellungen und des HTTP-Standardlisteners für `application-gateway rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="5f12f-3458">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="5f12f-3459">Verwendung der standardmäßigen Front-End-IP-Adresse und des standardmäßigen Back-End-Pools für `lb rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="5f12f-3459">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="5f12f-3460">Verwendung der standardmäßigen Front-End-IP-Adresse für `lb inbound-nat-rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="5f12f-3460">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="5f12f-3461">Profil</span><span class="sxs-lookup"><span data-stu-id="5f12f-3461">Profile</span></span>

* <span data-ttu-id="5f12f-3462">Unterstützung der Anmeldung innerhalb eines virtuellen Computers mit einer verwalteten Identität</span><span class="sxs-lookup"><span data-stu-id="5f12f-3462">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="5f12f-3463">Unterstützung der Ausgabe für `account show` im SDK-Authentifizierungsdateiformat</span><span class="sxs-lookup"><span data-stu-id="5f12f-3463">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="5f12f-3464">Anzeige von Warnungen für veraltete Befehle bei Verwendung von „--expanded-view“</span><span class="sxs-lookup"><span data-stu-id="5f12f-3464">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="5f12f-3465">Befehl `get-access-token` für die Bereitstellung eines unformatierten AAD-Tokens hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3465">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="5f12f-3466">Unterstützung der Anmeldung mit einem Benutzerkonto ohne zugeordnete Abonnements</span><span class="sxs-lookup"><span data-stu-id="5f12f-3466">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="5f12f-3467">RDBMS</span><span class="sxs-lookup"><span data-stu-id="5f12f-3467">RDBMS</span></span>

* <span data-ttu-id="5f12f-3468">Unterstützung der abonnementübergreifenden Auflistung von Servern (3417)</span><span class="sxs-lookup"><span data-stu-id="5f12f-3468">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="5f12f-3469">Behoben: `%s` wird aufgrund von fehlendem `% server_type` nicht verarbeitet (3393)</span><span class="sxs-lookup"><span data-stu-id="5f12f-3469">Fixed `%s` not processed because of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="5f12f-3470">Dokumentquellenzuordnung behoben und CI-Aufgabe zur Überprüfung hinzugefügt (3361)</span><span class="sxs-lookup"><span data-stu-id="5f12f-3470">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="5f12f-3471">MySQL- und PostgreSQL-Hilfe korrigiert (3369)</span><span class="sxs-lookup"><span data-stu-id="5f12f-3471">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="5f12f-3472">Resource</span><span class="sxs-lookup"><span data-stu-id="5f12f-3472">Resource</span></span>

* <span data-ttu-id="5f12f-3473">Eingabeaufforderungen bei fehlenden Parametern für `group deployment create` verbessert</span><span class="sxs-lookup"><span data-stu-id="5f12f-3473">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="5f12f-3474">Analyse der Syntax `--parameters KEY=VALUE` verbessert</span><span class="sxs-lookup"><span data-stu-id="5f12f-3474">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="5f12f-3475">Probleme behoben, durch die Parameterdateien von `group deployment create` bei Verwendung der Syntax `@<file>` nicht mehr erkannt wurden</span><span class="sxs-lookup"><span data-stu-id="5f12f-3475">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="5f12f-3476">Unterstützung des Arguments `--ids` für Befehle vom Typ `resource` und `managedapp`</span><span class="sxs-lookup"><span data-stu-id="5f12f-3476">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="5f12f-3477">Einige Analyse- und Fehlermeldungen korrigiert (3584)</span><span class="sxs-lookup"><span data-stu-id="5f12f-3477">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="5f12f-3478">Analyse vom Typ `--resource-type` für den Befehl `lock` korrigiert, sodass `<resource-namespace>` und `<resource-type>` akzeptiert werden</span><span class="sxs-lookup"><span data-stu-id="5f12f-3478">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="5f12f-3479">Parameterüberprüfung für Vorlagenlinkvorlagen hinzugefügt (3629)</span><span class="sxs-lookup"><span data-stu-id="5f12f-3479">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="5f12f-3480">Unterstützung für die Angabe von Bereitstellungsparametern mit der Syntax `KEY=VALUE` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3480">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="5f12f-3481">Role</span><span class="sxs-lookup"><span data-stu-id="5f12f-3481">Role</span></span>

* <span data-ttu-id="5f12f-3482">Unterstützung der Ausgabe im SDK-Authentifizierungsdateiformat für `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="5f12f-3482">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="5f12f-3483">Rollenzuweisungen und dazugehörige AAD-Anwendung beim Löschen eines Dienstprinzipals bereinigt (3610)</span><span class="sxs-lookup"><span data-stu-id="5f12f-3483">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="5f12f-3484">Einbeziehung des Zeitformats in Beschreibungen vom Typ `--start-date` und `--end-date` für `app create`-Argumente</span><span class="sxs-lookup"><span data-stu-id="5f12f-3484">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="5f12f-3485">Anzeige von Warnungen für veraltete Befehle bei Verwendung von `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="5f12f-3485">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="5f12f-3486">Schlüsseltresorintegration zu den Befehlen `create-for-rbac` und `reset-credentials` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3486">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="5f12f-3487">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="5f12f-3487">Service Fabric</span></span>
* <span data-ttu-id="5f12f-3488">Problem behoben, aufgrund dessen große Dateien in Anwendungen beim Hochladen gekürzt wurden (3666)</span><span class="sxs-lookup"><span data-stu-id="5f12f-3488">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="5f12f-3489">Tests für Service Fabric-Befehle hinzugefügt (3424)</span><span class="sxs-lookup"><span data-stu-id="5f12f-3489">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="5f12f-3490">Zahlreiche Service Fabric-Befehle korrigiert (3234)</span><span class="sxs-lookup"><span data-stu-id="5f12f-3490">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="5f12f-3491">SQL</span><span class="sxs-lookup"><span data-stu-id="5f12f-3491">SQL</span></span>

* <span data-ttu-id="5f12f-3492">Fehlerhafte1 Parameter `--identity` für `sql server create` entfernt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3492">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="5f12f-3493">Kennwortwerte aus der Befehlsausgabe von `sql server create` und `sql server update` entfernt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3493">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="5f12f-3494">Befehle `sql db list-editions` und `sql elastic-pool list-editions` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3494">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="5f12f-3495">Storage</span><span class="sxs-lookup"><span data-stu-id="5f12f-3495">Storage</span></span>

* <span data-ttu-id="5f12f-3496">Option `--marker` für die Befehle `storage blob list`, `storage container list` und `storage share list` entfernt (3745)</span><span class="sxs-lookup"><span data-stu-id="5f12f-3496">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="5f12f-3497">Erstellung eines reinen HTTPS-Speicherkontos ermöglicht</span><span class="sxs-lookup"><span data-stu-id="5f12f-3497">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="5f12f-3498">Speichermetriken, Protokollierung und CORS-Befehle aktualisiert (3495)</span><span class="sxs-lookup"><span data-stu-id="5f12f-3498">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="5f12f-3499">Ausnahmemeldung von „cors add“ umformuliert (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="5f12f-3499">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="5f12f-3500">Generator im Probelaufmodus des Downloadbatchbefehls in eine Liste konvertiert (3592)</span><span class="sxs-lookup"><span data-stu-id="5f12f-3500">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="5f12f-3501">Problem bei Probelauf des Blobdownloadbatchs behoben (3640) (3592)</span><span class="sxs-lookup"><span data-stu-id="5f12f-3501">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="5f12f-3502">VM</span><span class="sxs-lookup"><span data-stu-id="5f12f-3502">VM</span></span>

* <span data-ttu-id="5f12f-3503">Unterstützung der NSG-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="5f12f-3503">Support configuring nsg</span></span>
* <span data-ttu-id="5f12f-3504">Fehler behoben, aufgrund dessen der DNS-Server nicht ordnungsgemäß konfiguriert wurde</span><span class="sxs-lookup"><span data-stu-id="5f12f-3504">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="5f12f-3505">Unterstützung verwalteter Dienstidentitäten</span><span class="sxs-lookup"><span data-stu-id="5f12f-3505">Support managed service identities</span></span>
* <span data-ttu-id="5f12f-3506">Problem behoben, aufgrund dessen `cmss create` mit einem vorhandenen Lastenausgleich `--backend-pool-name` benötigte</span><span class="sxs-lookup"><span data-stu-id="5f12f-3506">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="5f12f-3507">Festlegung, dass die LUN von mit `vm image create` erstellten Datenträgern mit 0 beginnt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3507">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="5f12f-3508">10. Mai 2017</span><span class="sxs-lookup"><span data-stu-id="5f12f-3508">May 10, 2017</span></span>

<span data-ttu-id="5f12f-3509">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="5f12f-3509">Version 2.0.6</span></span>

* <span data-ttu-id="5f12f-3510">Umbenennen von „documentdb“ in „cosmosdb“</span><span class="sxs-lookup"><span data-stu-id="5f12f-3510">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="5f12f-3511">Hinzufügen von rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="5f12f-3511">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="5f12f-3512">Einbeziehen der Data Lake Analytics- und Data Lake Store-Module</span><span class="sxs-lookup"><span data-stu-id="5f12f-3512">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="5f12f-3513">Einbeziehen des Cognitive Services-Moduls</span><span class="sxs-lookup"><span data-stu-id="5f12f-3513">Include Cognitive Services module</span></span>
* <span data-ttu-id="5f12f-3514">Einbeziehen des Service Fabric-Moduls</span><span class="sxs-lookup"><span data-stu-id="5f12f-3514">Include Service Fabric module</span></span>
* <span data-ttu-id="5f12f-3515">Einbeziehen des interaktiven Moduls (Umbenennen von „az-shell“)</span><span class="sxs-lookup"><span data-stu-id="5f12f-3515">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="5f12f-3516">Hinzufügen von Unterstützung für CDN-Befehle</span><span class="sxs-lookup"><span data-stu-id="5f12f-3516">Add support for CDN commands</span></span>
* <span data-ttu-id="5f12f-3517">Entfernen des Containermoduls</span><span class="sxs-lookup"><span data-stu-id="5f12f-3517">Remove Container module</span></span>
* <span data-ttu-id="5f12f-3518">Hinzufügen von „az -v“ als Verknüpfung für „az --version“ ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="5f12f-3518">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="5f12f-3519">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="5f12f-3519">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="5f12f-3520">Core</span><span class="sxs-lookup"><span data-stu-id="5f12f-3520">Core</span></span>

* <span data-ttu-id="5f12f-3521">Core: Erfassen von Ausnahmen, die durch einen nicht registrierten Anbieter verursacht werden, und automatische Registrierung</span><span class="sxs-lookup"><span data-stu-id="5f12f-3521">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="5f12f-3522">Leistung: Dauerhaftes Speichern des ADAL-Tokencaches im Arbeitsspeicher bis zum Prozessende ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="5f12f-3522">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="5f12f-3523">Korrigieren der vom hexadezimalen Fingerabdruck -o tsv zurückgegebenen Bytes ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="5f12f-3523">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="5f12f-3524">Verbessern des Downloads des Schlüsseltresorzertifikats und der AAD-SP-Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="5f12f-3524">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="5f12f-3525">Hinzufügen des Python-Speicherorts zu „az –version“ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="5f12f-3525">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="5f12f-3526">Anmeldung: Unterstützung der Anmeldung, wenn keine Abonnements vorhanden sind ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="5f12f-3526">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="5f12f-3527">Core: Beheben eines Fehlers bei zweimaliger Verwendung eines Dienstprinzipals bei der Anmeldung ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="5f12f-3527">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="5f12f-3528">Core: Ermöglichen der Konfiguration des Dateipfads von „accessTokens.json“ über eine Umgebungsvariable ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="5f12f-3528">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="5f12f-3529">Core: Zulassen der Anwendung konfigurierter Standardwerte auf optionale Argumente ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="5f12f-3529">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="5f12f-3530">Core: Verbesserte Leistung</span><span class="sxs-lookup"><span data-stu-id="5f12f-3530">core: Improved performance</span></span>
* <span data-ttu-id="5f12f-3531">Core: Zertifikate von benutzerdefinierter Zertifizierungsstelle – Unterstützung für das Festlegen der REQUESTS_CA_BUNDLE-Umgebungsvariablen</span><span class="sxs-lookup"><span data-stu-id="5f12f-3531">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="5f12f-3532">Core: Cloudkonfiguration – Verwenden des Endpunkts „resource manager“, wenn Endpunkt „management“ nicht festgelegt ist</span><span class="sxs-lookup"><span data-stu-id="5f12f-3532">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="5f12f-3533">ACS</span><span class="sxs-lookup"><span data-stu-id="5f12f-3533">ACS</span></span>

* <span data-ttu-id="5f12f-3534">Korrigieren der Master- und Agentanzahl als ganze Zahl statt Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5f12f-3534">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="5f12f-3535">Verfügbarmachen von „az acs create --no-wait“ und „az acs wait“ für die asynchrone Erstellung</span><span class="sxs-lookup"><span data-stu-id="5f12f-3535">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="5f12f-3536">Verfügbarmachen von „az acs create --validate“ für Probelaufüberprüfungen</span><span class="sxs-lookup"><span data-stu-id="5f12f-3536">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="5f12f-3537">Entfernen von Windows-Profil vor PUT-Aufruf für Skalierungsbefehl ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="5f12f-3537">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="5f12f-3538">AppService</span><span class="sxs-lookup"><span data-stu-id="5f12f-3538">AppService</span></span>

* <span data-ttu-id="5f12f-3539">functionapp: Hinzufügen der vollständigen functionapp-Unterstützung, einschließlich Erstellen, Anzeigen, Auflisten, Löschen, Hostname, SSL usw.</span><span class="sxs-lookup"><span data-stu-id="5f12f-3539">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="5f12f-3540">Hinzufügen von Team Services (vsts) als Continuous Delivery-Option zu „appservice web source-control config“</span><span class="sxs-lookup"><span data-stu-id="5f12f-3540">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="5f12f-3541">Erstellen von „az webapp“ als Ersatz für „az appservice web“ (für Abwärtskompatibilität bleibt „az appservice web“ für 2 weitere Releases erhalten)</span><span class="sxs-lookup"><span data-stu-id="5f12f-3541">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="5f12f-3542">Verfügbarmachen von Argumenten zum Konfigurieren von Bereitstellung und Laufzeitstapeln beim Erstellen von Web-Apps</span><span class="sxs-lookup"><span data-stu-id="5f12f-3542">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="5f12f-3543">Verfügbarmachen von „webapp list-runtimes“</span><span class="sxs-lookup"><span data-stu-id="5f12f-3543">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="5f12f-3544">Unterstützen der Konfiguration von Verbindungszeichenfolgen ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="5f12f-3544">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="5f12f-3545">Unterstützen des Slottauschs mit Vorschau</span><span class="sxs-lookup"><span data-stu-id="5f12f-3545">support slot swap with preview</span></span>
* <span data-ttu-id="5f12f-3546">Beheben von Fehlern in appservice-Befehlen ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="5f12f-3546">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="5f12f-3547">Verwenden der Ressourcengruppe des App Service-Plans für Zertifizierungsvorgänge ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="5f12f-3547">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="5f12f-3548">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="5f12f-3548">CosmosDB</span></span>

* <span data-ttu-id="5f12f-3549">Umbenennen des documentdb-Moduls in cosmosdb</span><span class="sxs-lookup"><span data-stu-id="5f12f-3549">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="5f12f-3550">Zusätzliche Unterstützung für documentdb-APIs auf Datenebene: Datenbank- und Sammlungsverwaltung</span><span class="sxs-lookup"><span data-stu-id="5f12f-3550">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="5f12f-3551">Zusätzliche Unterstützung für das Aktivieren des automatischen Failovers für Datenbankkonten</span><span class="sxs-lookup"><span data-stu-id="5f12f-3551">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="5f12f-3552">Zusätzliche Unterstützung für die neue ConsistentPrefix-Konsistenzrichtlinie</span><span class="sxs-lookup"><span data-stu-id="5f12f-3552">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="5f12f-3553">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="5f12f-3553">Data Lake Analytics</span></span>

* <span data-ttu-id="5f12f-3554">Beheben eines Fehlers, bei dem das Filtern von Auftragslisten nach Ergebnis und Status einen Fehler auslöst</span><span class="sxs-lookup"><span data-stu-id="5f12f-3554">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="5f12f-3555">Hinzufügen von Unterstützung für den neuen Katalogelementtyp „Paket“</span><span class="sxs-lookup"><span data-stu-id="5f12f-3555">Add support for new catalog item type: package.</span></span> <span data-ttu-id="5f12f-3556">Zugriff über: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="5f12f-3556">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="5f12f-3557">Ermöglichen der Auflistung folgender Katalogelemente innerhalb einer Datenbank (keine Schemaspezifikation erforderlich):</span><span class="sxs-lookup"><span data-stu-id="5f12f-3557">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="5f12f-3558">Tabelle</span><span class="sxs-lookup"><span data-stu-id="5f12f-3558">Table</span></span>
  * <span data-ttu-id="5f12f-3559">Tabellenwertfunktion</span><span class="sxs-lookup"><span data-stu-id="5f12f-3559">Table valued function</span></span>
  * <span data-ttu-id="5f12f-3560">Sicht</span><span class="sxs-lookup"><span data-stu-id="5f12f-3560">View</span></span>
  * <span data-ttu-id="5f12f-3561">Tabellenstatistiken.</span><span class="sxs-lookup"><span data-stu-id="5f12f-3561">Table Statistics.</span></span> <span data-ttu-id="5f12f-3562">Können auch mit einem Schema, jedoch ohne Angabe eines Tabellennamens aufgelistet werden.</span><span class="sxs-lookup"><span data-stu-id="5f12f-3562">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="5f12f-3563">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="5f12f-3563">Data Lake Store</span></span>

* <span data-ttu-id="5f12f-3564">Aktualisieren der Version des zugrunde liegenden Dateisystem-SDK, wodurch eine bessere Unterstützung für die Verarbeitung von Drosselungsszenarien auf Serverseite gewährt wird</span><span class="sxs-lookup"><span data-stu-id="5f12f-3564">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="5f12f-3565">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="5f12f-3565">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="5f12f-3566">Fehlende Hilfe für Zugriffsanzeige</span><span class="sxs-lookup"><span data-stu-id="5f12f-3566">missed help for access show.</span></span> <span data-ttu-id="5f12f-3567">hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="5f12f-3567">adding it.</span></span> <span data-ttu-id="5f12f-3568">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="5f12f-3568">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="5f12f-3569">Suchen</span><span class="sxs-lookup"><span data-stu-id="5f12f-3569">Find</span></span>

* <span data-ttu-id="5f12f-3570">Verbessern von Suchergebnissen und Ermöglichen der Versionsverwaltung des Suchindex</span><span class="sxs-lookup"><span data-stu-id="5f12f-3570">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="5f12f-3571">KeyVault</span><span class="sxs-lookup"><span data-stu-id="5f12f-3571">KeyVault</span></span>

* <span data-ttu-id="5f12f-3572">BC:`az keyvault certificate download` Ändern von „-e“ von Zeichenfolge oder Binärdatentyp in PEM oder DER zur besseren Darstellung der Optionen</span><span class="sxs-lookup"><span data-stu-id="5f12f-3572">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="5f12f-3573">BC: Entfernen von „--expires“ und „--not-before“ aus `keyvault certificate create`, da diese Parameter nicht vom Dienst unterstützt werden</span><span class="sxs-lookup"><span data-stu-id="5f12f-3573">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="5f12f-3574">Hinzufügen des Parameters „--validity“ zu `keyvault certificate create`, um gezielt den Wert in „--policy“ zu überschreiben</span><span class="sxs-lookup"><span data-stu-id="5f12f-3574">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="5f12f-3575">Beheben des Problems in `keyvault certificate get-default-policy`, bei dem „expires“ und „not_before“ verfügbar gemacht wurden, „validity_in_months“ hingegen nicht</span><span class="sxs-lookup"><span data-stu-id="5f12f-3575">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="5f12f-3576">Keyvault-Korrektur für den Import von PEM und PFX ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="5f12f-3576">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="5f12f-3577">Labor</span><span class="sxs-lookup"><span data-stu-id="5f12f-3577">Lab</span></span>

* <span data-ttu-id="5f12f-3578">Hinzufügen der Befehle „create“, „show“, „delete“ und „list“ für die Laborumgebung</span><span class="sxs-lookup"><span data-stu-id="5f12f-3578">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="5f12f-3579">Hinzufügen der Befehle „show“ und „list“ zur Anzeige von ARM-Vorlagen im Labor</span><span class="sxs-lookup"><span data-stu-id="5f12f-3579">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="5f12f-3580">Hinzufügen des Kennzeichens „--environment“ in `az lab vm list`, um virtuelle Computer nach Umgebung im Labor zu filtern</span><span class="sxs-lookup"><span data-stu-id="5f12f-3580">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="5f12f-3581">Hinzufügen des benutzerfreundlichen Befehls `az lab formula export-artifacts` zum Exportieren des Artefaktgerüsts innerhalb der Formel eines Labors</span><span class="sxs-lookup"><span data-stu-id="5f12f-3581">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="5f12f-3582">Hinzufügen von Befehlen zum Verwalten von Geheimnissen in einem Labor</span><span class="sxs-lookup"><span data-stu-id="5f12f-3582">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="5f12f-3583">Überwachen</span><span class="sxs-lookup"><span data-stu-id="5f12f-3583">Monitor</span></span>

* <span data-ttu-id="5f12f-3584">Fehlerbehebung: Modellieren von `--actions` von `az alert-rules create` zum Verarbeiten von JSON-Zeichenfolgen ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="5f12f-3584">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="5f12f-3585">Programmfehlerbehebung: Beim Erstellen von Diagnoseeinstellungen werden Protokolle/Metriken aus Anzeigebefehlen nicht akzeptiert ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="5f12f-3585">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="5f12f-3586">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="5f12f-3586">Network</span></span>

* <span data-ttu-id="5f12f-3587">Hinzufügen des `network watcher test-connectivity`-Befehls</span><span class="sxs-lookup"><span data-stu-id="5f12f-3587">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="5f12f-3588">Hinzufügen von Unterstützung für den `--filters`-Parameter für `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="5f12f-3588">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="5f12f-3589">Hinzufügen von Unterstützung für den Application Gateway-Verbindungsausgleich</span><span class="sxs-lookup"><span data-stu-id="5f12f-3589">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="5f12f-3590">Hinzufügen von Unterstützung für die Konfiguration von Application Gateway-WAF-Regelsätzen</span><span class="sxs-lookup"><span data-stu-id="5f12f-3590">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="5f12f-3591">Hinzufügen von Unterstützung für ExpressRoute-Routenfilter und -Regeln</span><span class="sxs-lookup"><span data-stu-id="5f12f-3591">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="5f12f-3592">Hinzufügen von Unterstützung für geografisches TrafficManager-Routing</span><span class="sxs-lookup"><span data-stu-id="5f12f-3592">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="5f12f-3593">Hinzufügen von Unterstützung für richtlinienbasierte Datenverkehrsselektoren für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="5f12f-3593">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="5f12f-3594">Hinzufügen von Unterstützung für IPSec-Richtlinien für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="5f12f-3594">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="5f12f-3595">Korrektur eines Fehlers bei `vpn-connection create` bei Verwendung der Parameter `--no-wait` oder `--validate`</span><span class="sxs-lookup"><span data-stu-id="5f12f-3595">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="5f12f-3596">Hinzufügen von Unterstützung für Aktiv/Aktiv-VNET-Gateways</span><span class="sxs-lookup"><span data-stu-id="5f12f-3596">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="5f12f-3597">Entfernen von NULL-Werten aus der Ausgabe von `network vpn-connection list/show`-Befehlen</span><span class="sxs-lookup"><span data-stu-id="5f12f-3597">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="5f12f-3598">BC: Korrektur eines Fehlers in der Ausgabe von `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="5f12f-3598">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="5f12f-3599">Korrektur eines Fehlers, bei dem das Argument „--key-length“ von „vpn-connection create“ nicht ordnungsgemäß analysiert wurde</span><span class="sxs-lookup"><span data-stu-id="5f12f-3599">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="5f12f-3600">Korrektur eines Fehlers in `dns zone import`, bei dem Datensätze nicht ordnungsgemäß importiert wurden</span><span class="sxs-lookup"><span data-stu-id="5f12f-3600">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="5f12f-3601">Korrektur eines Fehlers, bei dem `traffic-manager endpoint update` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="5f12f-3601">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="5f12f-3602">Hinzufügen von Network Watcher-Vorschaubefehlen</span><span class="sxs-lookup"><span data-stu-id="5f12f-3602">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="5f12f-3603">Profil</span><span class="sxs-lookup"><span data-stu-id="5f12f-3603">Profile</span></span>

* <span data-ttu-id="5f12f-3604">Unterstützung der Anmeldung, wenn keine Abonnements gefunden werden ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="5f12f-3604">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="5f12f-3605">Unterstützung für kurze Parameternamen in „az account set --subscription“ ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="5f12f-3605">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="5f12f-3606">Redis</span><span class="sxs-lookup"><span data-stu-id="5f12f-3606">Redis</span></span>

* <span data-ttu-id="5f12f-3607">Hinzufügen des Updatebefehls, durch den auch die Möglichkeit zum Skalieren für Redis Cache hinzugefügt wird</span><span class="sxs-lookup"><span data-stu-id="5f12f-3607">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="5f12f-3608">Verwerfen des Befehls „update-settings“</span><span class="sxs-lookup"><span data-stu-id="5f12f-3608">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="5f12f-3609">Resource</span><span class="sxs-lookup"><span data-stu-id="5f12f-3609">Resource</span></span>

* <span data-ttu-id="5f12f-3610">Hinzufügen der Befehle „managedapp“ und „managedapp definition“ ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="5f12f-3610">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="5f12f-3611">Unterstützung für die „provider operation“-Befehle ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="5f12f-3611">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="5f12f-3612">Unterstützung für die Erstellung generischer Ressourcen ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="5f12f-3612">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="5f12f-3613">Korrigieren der Ressourcenanalyse und der API-Versionssuche</span><span class="sxs-lookup"><span data-stu-id="5f12f-3613">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="5f12f-3614">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="5f12f-3614">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="5f12f-3615">Hinzufügen von Dokumenten für „az lock update“</span><span class="sxs-lookup"><span data-stu-id="5f12f-3615">Add docs for az lock update.</span></span> <span data-ttu-id="5f12f-3616">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="5f12f-3616">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="5f12f-3617">Beenden mit Fehler bei dem Versuch, Ressourcen für eine nicht vorhandene Gruppe aufzulisten</span><span class="sxs-lookup"><span data-stu-id="5f12f-3617">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="5f12f-3618">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="5f12f-3618">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="5f12f-3619">[Compute] Beheben von Problemen mit dem Update von VMSS- und VM-Verfügbarkeitsgruppen</span><span class="sxs-lookup"><span data-stu-id="5f12f-3619">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="5f12f-3620">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="5f12f-3620">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="5f12f-3621">Korrigieren des Erstellungs- und Löschvorgangs für Sperren, wenn „parent-resource-path“ auf „None“ festgelegt ist ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="5f12f-3621">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="5f12f-3622">Role</span><span class="sxs-lookup"><span data-stu-id="5f12f-3622">Role</span></span>

* <span data-ttu-id="5f12f-3623">create-for-rbac: Sicherstellen, dass das SP-Enddatum nicht das Ablaufdatum des Zertifikats überschreitet ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="5f12f-3623">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="5f12f-3624">RBAC: Hinzufügen vollständiger Unterstützung für „ad group“ ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="5f12f-3624">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="5f12f-3625">Rolle: Beheben von Probleme beim Rollendefinitionsupdate ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="5f12f-3625">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="5f12f-3626">create-for-rbac: Sicherstellen, dass das angegebene Benutzerkennwort übernommen wird</span><span class="sxs-lookup"><span data-stu-id="5f12f-3626">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="5f12f-3627">SQL</span><span class="sxs-lookup"><span data-stu-id="5f12f-3627">SQL</span></span>

* <span data-ttu-id="5f12f-3628">Hinzufügen der Befehle „az sql server list-usages“ und „az sql db list-usages“</span><span class="sxs-lookup"><span data-stu-id="5f12f-3628">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="5f12f-3629">SQL: Möglichkeit zur direkten Verbindung mit Ressourcenanbieter ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="5f12f-3629">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="5f12f-3630">Storage</span><span class="sxs-lookup"><span data-stu-id="5f12f-3630">Storage</span></span>

* <span data-ttu-id="5f12f-3631">Festlegen des Ressourcengruppenstandorts als Standardstandort für `storage account create`</span><span class="sxs-lookup"><span data-stu-id="5f12f-3631">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="5f12f-3632">Hinzufügen von Unterstützung für das inkrementelle Kopieren von Blobs</span><span class="sxs-lookup"><span data-stu-id="5f12f-3632">Add support for incremental blob copy</span></span>
* <span data-ttu-id="5f12f-3633">Hinzufügen von Unterstützung für den Upload umfangreicher Blockblobs</span><span class="sxs-lookup"><span data-stu-id="5f12f-3633">Add support for large block blob upload</span></span>
* <span data-ttu-id="5f12f-3634">Ändern der Blockgröße auf 100 MB, wenn die hochzuladende Datei größer als 200 GB ist</span><span class="sxs-lookup"><span data-stu-id="5f12f-3634">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="5f12f-3635">VM</span><span class="sxs-lookup"><span data-stu-id="5f12f-3635">VM</span></span>

* <span data-ttu-id="5f12f-3636">avail-set: Festlegen der UD- und FD-Domänenanzahl als optional</span><span class="sxs-lookup"><span data-stu-id="5f12f-3636">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="5f12f-3637">Hinweis: VM-Befehle in unabhängigen Clouds: Vermeiden Sie Features im Zusammenhang mit verwalteten Datenträgern, einschließlich der folgenden:</span><span class="sxs-lookup"><span data-stu-id="5f12f-3637">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="5f12f-3638">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="5f12f-3638">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="5f12f-3639">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="5f12f-3639">az vm/vmss disk</span></span>
  3. <span data-ttu-id="5f12f-3640">Verwenden Sie in „az vm/vmss create“ den Befehl „—use-unmanaged-disk“, um verwaltete Datenträger zu vermeiden. Andere Befehle sollten funktionieren.</span><span class="sxs-lookup"><span data-stu-id="5f12f-3640">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="5f12f-3641">vm/vmss: Verbessern des Warnungstexts beim Generieren von SSH-Schlüsselpaaren</span><span class="sxs-lookup"><span data-stu-id="5f12f-3641">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="5f12f-3642">vm/vmss: Unterstützen der Erstellung über ein Marketplace-Image, für das Planinformationen erforderlich sind ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="5f12f-3642">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="5f12f-3643">3\. April 2017</span><span class="sxs-lookup"><span data-stu-id="5f12f-3643">April 3, 2017</span></span>

<span data-ttu-id="5f12f-3644">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="5f12f-3644">Version 2.0.2</span></span>

<span data-ttu-id="5f12f-3645">In dieser Version wurden die Komponenten ACR, Batch, KeyVault und SQL eingeführt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-3645">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="5f12f-3646">Core</span><span class="sxs-lookup"><span data-stu-id="5f12f-3646">Core</span></span>

* <span data-ttu-id="5f12f-3647">Hinzufügen der Module „acr“, „lab“, „monitor“ und „find“ zur Standardliste</span><span class="sxs-lookup"><span data-stu-id="5f12f-3647">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="5f12f-3648">Anmeldung: Überspringen des fehlerhaften Mandanten ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="5f12f-3648">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="5f12f-3649">Anmeldung: Festlegen des Standardabonnements auf ein Abonnement mit dem Status „Enabled“ ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="5f12f-3649">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="5f12f-3650">Hinzufügen von wait-Befehlen und Unterstützung von „--no-wait“ für mehr Befehle ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="5f12f-3650">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="5f12f-3651">Core: Unterstützen der Anmeldung per Dienstprinzipal mit einem Zertifikat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="5f12f-3651">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="5f12f-3652">Hinzufügen der Meldung zu fehlenden Vorlagenparametern</span><span class="sxs-lookup"><span data-stu-id="5f12f-3652">Add prompting for missing template parameters.</span></span> <span data-ttu-id="5f12f-3653">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="5f12f-3653">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="5f12f-3654">Unterstützen des Festlegens von Standardwerten für häufig verwendete Argumente, z.B. Standardressourcengruppe, Standardweb und Standard-VM</span><span class="sxs-lookup"><span data-stu-id="5f12f-3654">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="5f12f-3655">Unterstützen der Anmeldung an einem bestimmten Mandanten</span><span class="sxs-lookup"><span data-stu-id="5f12f-3655">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="5f12f-3656">ACS</span><span class="sxs-lookup"><span data-stu-id="5f12f-3656">ACS</span></span>

* <span data-ttu-id="5f12f-3657">[ACS] Hinzufügen von Unterstützung für die Konfiguration eines ACS-Standardclusters ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="5f12f-3657">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="5f12f-3658">Hinzufügen von Unterstützung der Aufforderung zur Kennworteingabe für SSH-Schlüssel</span><span class="sxs-lookup"><span data-stu-id="5f12f-3658">Add support for ssh key password prompting.</span></span> <span data-ttu-id="5f12f-3659">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="5f12f-3659">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="5f12f-3660">Hinzufügen von Unterstützung für Windows-Cluster</span><span class="sxs-lookup"><span data-stu-id="5f12f-3660">Add support for windows clusters.</span></span> <span data-ttu-id="5f12f-3661">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="5f12f-3661">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="5f12f-3662">Wechseln von der Rolle „Besitzer“ zur Rolle „Mitwirkender“</span><span class="sxs-lookup"><span data-stu-id="5f12f-3662">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="5f12f-3663">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="5f12f-3663">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="5f12f-3664">AppService</span><span class="sxs-lookup"><span data-stu-id="5f12f-3664">AppService</span></span>

* <span data-ttu-id="5f12f-3665">appservice: Unterstützung für das Abrufen der externen IP-Adresse für DNS A-Einträge ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="5f12f-3665">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="5f12f-3666">appservice: Unterstützung der Bindung von Platzhalterzertifikaten ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="5f12f-3666">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="5f12f-3667">appservice: Unterstützung von Veröffentlichungsprofilen für Listen ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="5f12f-3667">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="5f12f-3668">AppService: Auslösen der Synchronisierung der Quellcodeverwaltung nach der Konfiguration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="5f12f-3668">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="5f12f-3669">DataLake</span><span class="sxs-lookup"><span data-stu-id="5f12f-3669">DataLake</span></span>

* <span data-ttu-id="5f12f-3670">Erste Version des Data Lake Analytics-Moduls</span><span class="sxs-lookup"><span data-stu-id="5f12f-3670">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="5f12f-3671">Erste Version des Data Lake Store-Moduls</span><span class="sxs-lookup"><span data-stu-id="5f12f-3671">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="5f12f-3672">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="5f12f-3672">DocuemntDB</span></span>

* <span data-ttu-id="5f12f-3673">DocumentDB: Hinzufügen von Unterstützung für das Auflisten von Verbindungszeichenfolgen ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="5f12f-3673">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="5f12f-3674">VM</span><span class="sxs-lookup"><span data-stu-id="5f12f-3674">VM</span></span>

* <span data-ttu-id="5f12f-3675">[Compute] Hinzufügen von AppGateway-Unterstützung für Erstellung von VM-Skalierungsgruppen ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="5f12f-3675">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="5f12f-3676">[VM/VMSS] Verbesserte Unterstützung für die Datenträgerzwischenspeicherung ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="5f12f-3676">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="5f12f-3677">VM/VMSS: Einbinden der vom Portal verwendeten Logik zur Überprüfung von Anmeldeinformationen ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="5f12f-3677">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="5f12f-3678">Hinzufügen von wait-Befehlen und Unterstützung für „--no-wait“ ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="5f12f-3678">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="5f12f-3679">VM-Skalierungsgruppe: Unterstützung von „\*“ zum Auflisten der übergreifenden Instanzansicht für VMs ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="5f12f-3679">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="5f12f-3680">Hinzufügen – Geheimnisse für virtuellen Computer und VM-Skalierungsgruppe ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="5f12f-3680">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="5f12f-3681">Zulassen der VM-Erstellung mit spezialisierter VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="5f12f-3681">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="5f12f-3682">27. Februar 2017</span><span class="sxs-lookup"><span data-stu-id="5f12f-3682">February 27, 2017</span></span>

<span data-ttu-id="5f12f-3683">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="5f12f-3683">Version 2.0.0</span></span>

<span data-ttu-id="5f12f-3684">Diese Version der Azure CLI 2.0 ist die erste „allgemein verfügbare“ Version. Die allgemeine Verfügbarkeit gilt für die folgenden Befehlsmodule:</span><span class="sxs-lookup"><span data-stu-id="5f12f-3684">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="5f12f-3685">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="5f12f-3685">Container Service (acs)</span></span>
- <span data-ttu-id="5f12f-3686">Compute (einschließlich Resource Manager, VM, VM-Skalierungsgruppen, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="5f12f-3686">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="5f12f-3687">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="5f12f-3687">Networking</span></span>
- <span data-ttu-id="5f12f-3688">Storage</span><span class="sxs-lookup"><span data-stu-id="5f12f-3688">Storage</span></span>

<span data-ttu-id="5f12f-3689">Diese Befehlsmodule können in der Produktion verwendet werden und verfügen über Unterstützung durch eine Standard-SLA von Microsoft. Sie können Anfragen zu Problemen direkt beim Microsoft-Support oder in der [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/) öffnen. Sie haben die Möglichkeit, Fragen in [StackOverflow mit dem Tag „azure-cli“](http://stackoverflow.com/questions/tagged/azure-cli) zu stellen oder sich unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) an das Produktteam zu wenden. Außerdem können Sie über die Befehlszeile mit dem Befehl `az feedback` Feedback senden.</span><span class="sxs-lookup"><span data-stu-id="5f12f-3689">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="5f12f-3690">Die Befehle in diesen Modulen sind stabil, und es ist nicht zu erwarten, dass sich die Syntax in den anstehenden Veröffentlichungen dieser Version der Azure CLI ändern.</span><span class="sxs-lookup"><span data-stu-id="5f12f-3690">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="5f12f-3691">Verwenden Sie zum Überprüfen der Version der CLI den Befehl `az --version`. In der Ausgabe werden die Version der CLI selbst (für diese Veröffentlichung 2.0.0), die einzelnen Befehlsmodule und die von Ihnen genutzten Versionen von Python und GCC aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="5f12f-3691">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="5f12f-3692">Einige Befehlsmodule verfügen über das Postfix „b*n*“ oder „rc*n*“. Diese Befehlsmodule befinden sich noch in der Vorschauphase und werden später die allgemeine Verfügbarkeit erlangen.</span><span class="sxs-lookup"><span data-stu-id="5f12f-3692">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="5f12f-3693">Außerdem werden jeden Abend Vorschaubuilds der CLI bereitgestellt. Informationen hierzu finden Sie in der [Anleitung zum Abrufen der abendlichen Builds](https://github.com/Azure/azure-cli#nightly-builds) und im Abschnitt zum [Setup für Entwickler und Beitragen von Code](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="5f12f-3693">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="5f12f-3694">Sie können für die abendlichen Vorschaubuilds wie folgt Probleme melden:</span><span class="sxs-lookup"><span data-stu-id="5f12f-3694">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="5f12f-3695">Über die [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="5f12f-3695">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="5f12f-3696">Per Kontaktaufnahme mit dem Produktteam unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="5f12f-3696">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="5f12f-3697">Senden von Feedback über die Befehlszeile mit dem Befehl `az feedback`</span><span class="sxs-lookup"><span data-stu-id="5f12f-3697">Provide feedback from the command line with the `az feedback` command</span></span>

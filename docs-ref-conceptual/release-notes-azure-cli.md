---
title: Versionshinweise für die Azure CLI
description: Enthält Informationen zu den aktuellen Updates der Azure CLI.
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 01/07/2020
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 9fc54add3bfb2a75d1912c47f0a2571d9d065ec0
ms.sourcegitcommit: 5646008e7a521dd9a8a627418f57bd92ee180352
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/07/2020
ms.locfileid: "75694273"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="6288a-103">Versionshinweise für die Azure CLI</span><span class="sxs-lookup"><span data-stu-id="6288a-103">Azure CLI release notes</span></span>

## <a name="january-07-2020"></a><span data-ttu-id="6288a-104">7\. Januar 2020</span><span class="sxs-lookup"><span data-stu-id="6288a-104">January 07, 2020</span></span>

<span data-ttu-id="6288a-105">Version 2.0.79</span><span class="sxs-lookup"><span data-stu-id="6288a-105">Version 2.0.79</span></span>

### <a name="acr"></a><span data-ttu-id="6288a-106">ACR</span><span class="sxs-lookup"><span data-stu-id="6288a-106">ACR</span></span>

* <span data-ttu-id="6288a-107">[BREAKING CHANGE] Parameter „--os“ für „acr build“, „acr task create/update“, „acr run“ und „acr pack“ wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="6288a-107">[BREAKING CHANGE] Remove '--os' parameter for 'acr build', 'acr task create/update', 'acr run', and 'acr pack'.</span></span> <span data-ttu-id="6288a-108">Verwenden Sie stattdessen „--platform“.</span><span class="sxs-lookup"><span data-stu-id="6288a-108">Use '--platform' instead.</span></span>

### <a name="appconfig"></a><span data-ttu-id="6288a-109">AppConfig</span><span class="sxs-lookup"><span data-stu-id="6288a-109">AppConfig</span></span>

* <span data-ttu-id="6288a-110">Unterstützung für das Importieren/Exportieren von Featureflags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-110">Add support for importing/exporting feature flags</span></span>
* <span data-ttu-id="6288a-111">Neuer Befehl „az appconfig kv set-keyvault“ für das Erstellen einer KeyVault-Referenz hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-111">Add new command 'az appconfig kv set-keyvault' for creating keyvault reference</span></span>
* <span data-ttu-id="6288a-112">Unterstützung verschiedener Benennungskonventionen beim Exportieren von Featureflags in eine Datei</span><span class="sxs-lookup"><span data-stu-id="6288a-112">Support various naming conventions when exporting feature flags to file</span></span>

### <a name="appservice"></a><span data-ttu-id="6288a-113">AppService</span><span class="sxs-lookup"><span data-stu-id="6288a-113">AppService</span></span>

* <span data-ttu-id="6288a-114">Behebung von Problem Nr. 7154: Aktualisierung der Dokumentation für Befehl „<>“, sodass Backticks anstelle von einfachen Anführungszeichen verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="6288a-114">Fix issue #7154: Updating documentation for command <> to use back ticks instead of single quotes</span></span>
* <span data-ttu-id="6288a-115">Behebung von Problem Nr. 11287: „webapp up“: Für die mit „up“ erstellte App muss standardmäßig SSL aktiviert sein.</span><span class="sxs-lookup"><span data-stu-id="6288a-115">Fix issue #11287: webapp up: By default make the app created using up 'should be 'SSL enabled'</span></span>
* <span data-ttu-id="6288a-116">Behebung von Problem Nr. 11592: Flag „az webapp up“ für statische HTML-Websites hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-116">Fix issue #11592: Add az webapp up flag for html static sites</span></span>

### <a name="arm"></a><span data-ttu-id="6288a-117">ARM</span><span class="sxs-lookup"><span data-stu-id="6288a-117">ARM</span></span>

* <span data-ttu-id="6288a-118">Behebung `az resource tag`: Recovery Services-Tresor-Tags können nicht aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="6288a-118">Fix `az resource tag`: Recovery Services Vault tags cannot be updated</span></span>

### <a name="backup"></a><span data-ttu-id="6288a-119">Backup</span><span class="sxs-lookup"><span data-stu-id="6288a-119">Backup</span></span>

* <span data-ttu-id="6288a-120">Neuer Befehl „backup protection undelete“ hinzugefügt, um die Funktion zum vorläufigen Löschen für IaasVM-Workloads zu aktivieren</span><span class="sxs-lookup"><span data-stu-id="6288a-120">Added new command 'backup protection undelete' to enable soft-delete feature for IaasVM workload</span></span>
* <span data-ttu-id="6288a-121">Neuer Parameter „--soft-delete-feature-state“ hinzugefügt, um den Befehl „backup-properties“ festzulegen</span><span class="sxs-lookup"><span data-stu-id="6288a-121">Added new parameter '--soft-delete-feature-state' to set backup-properties command</span></span>
* <span data-ttu-id="6288a-122">Unterstützung für den Ausschluss von Datenträgern für IaasVM-Workload hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-122">Added disk exclusion support for IaasVM workload</span></span>

### <a name="compute"></a><span data-ttu-id="6288a-123">Compute</span><span class="sxs-lookup"><span data-stu-id="6288a-123">Compute</span></span>

* <span data-ttu-id="6288a-124">Fehler `vm create` in Azure Stack-Profil behoben.</span><span class="sxs-lookup"><span data-stu-id="6288a-124">Fix `vm create` failure in Azure Stack profile.</span></span>
* <span data-ttu-id="6288a-125">vm monitor metrics tail/list-definitions: Unterstützung einer Abfragemetrik und von Listendefinitionen für eine VM.</span><span class="sxs-lookup"><span data-stu-id="6288a-125">vm monitor metrics tail/list-definitions: support query metric and list definitions for a vm.</span></span>
* <span data-ttu-id="6288a-126">Neue Aktion des Befehls zum erneuten Anwenden für „az vm“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-126">Add new reapply command action for az vm</span></span>

### <a name="misc"></a><span data-ttu-id="6288a-127">Verschiedenes:</span><span class="sxs-lookup"><span data-stu-id="6288a-127">Misc.</span></span>

* <span data-ttu-id="6288a-128">Vorschaubefehl `az version show` hinzugefügt, um die Versionen der Azure CLI-Module und Erweiterungen standardmäßig im JSON-Format oder im mit „--output“ konfigurierten Format anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="6288a-128">Add preview command `az version show` to show the versions of Azure CLI modules and extensions in JSON format by default or format configured by --output</span></span>

### <a name="event-hubs"></a><span data-ttu-id="6288a-129">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="6288a-129">Event Hubs</span></span>

* <span data-ttu-id="6288a-130">[BREAKING CHANGE] Statusoption „ReceiveDisabled“ aus „az eventhubs eventhub update“ und „az eventhubs eventhub create“ entfernt.</span><span class="sxs-lookup"><span data-stu-id="6288a-130">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az eventhubs eventhub update' and 'az eventhubs eventhub create'.</span></span> <span data-ttu-id="6288a-131">Diese Option ist für Event Hub-Entitäten nicht gültig.</span><span class="sxs-lookup"><span data-stu-id="6288a-131">This option is not valid for Event Hub entities.</span></span>

### <a name="service-bus"></a><span data-ttu-id="6288a-132">Service Bus</span><span class="sxs-lookup"><span data-stu-id="6288a-132">Service Bus</span></span>

* <span data-ttu-id="6288a-133">[BREAKING CHANGE] Statusoption „ReceiveDisabled“ aus Befehlen „az servicebus topic create“, „az servicebus topic update“, „az servicebus queue create“ und „az servicebus queue update“ entfernt.</span><span class="sxs-lookup"><span data-stu-id="6288a-133">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az servicebus topic create', 'az servicebus topic update', 'az servicebus queue create', and 'az servicebus queue update'.</span></span> <span data-ttu-id="6288a-134">Diese Option ist für Service Bus-Themen und -Warteschlangen nicht gültig.</span><span class="sxs-lookup"><span data-stu-id="6288a-134">This option is not valid for Service Bus topics and queues.</span></span>

### <a name="rbac"></a><span data-ttu-id="6288a-135">RBAC</span><span class="sxs-lookup"><span data-stu-id="6288a-135">RBAC</span></span>

* <span data-ttu-id="6288a-136">Behebung Nr. 11712: `az ad app/sp show` gibt nicht den Exitcode 3 zurück, wenn die Anwendung oder der Dienstprinzipal nicht vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="6288a-136">Fix #11712: `az ad app/sp show` does not return exit code 3 when the application or service principal does not exist</span></span>

### <a name="storage"></a><span data-ttu-id="6288a-137">Storage</span><span class="sxs-lookup"><span data-stu-id="6288a-137">Storage</span></span>

* <span data-ttu-id="6288a-138">`az storage account create`: Vorschaukennzeichnung für Parameter „--enable-hierarchical-namespace“ entfernt</span><span class="sxs-lookup"><span data-stu-id="6288a-138">`az storage account create`: Remove preview flag for --enable-hierarchical-namespace parameter</span></span>
* <span data-ttu-id="6288a-139">azure-mgmt-storage-Version auf 7.0.0 aktualisiert, um API-Version 2019-06-01 zu verwenden</span><span class="sxs-lookup"><span data-stu-id="6288a-139">Update azure-mgmt-storage version to 7.0.0 to use api version 2019-06-01</span></span>
* <span data-ttu-id="6288a-140">Neue Parameter `--enable-delete-retention` und `--delete-retention-days` hinzugefügt, um die Verwaltung der Aufbewahrungsrichtlinie für Löschen für „blob-service-properties“ von Speicherkonten zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="6288a-140">Add new parameters `--enable-delete-retention` and `--delete-retention-days` to support managing delete retention policy for storage account blob-service-properties.</span></span>

## <a name="december-17-2019"></a><span data-ttu-id="6288a-141">17. Dezember 2019</span><span class="sxs-lookup"><span data-stu-id="6288a-141">December 17, 2019</span></span>

<span data-ttu-id="6288a-142">2.0.78</span><span class="sxs-lookup"><span data-stu-id="6288a-142">2.0.78</span></span>

### <a name="acr"></a><span data-ttu-id="6288a-143">ACR</span><span class="sxs-lookup"><span data-stu-id="6288a-143">ACR</span></span>

* <span data-ttu-id="6288a-144">Unterstützung für lokalen Kontext in „acr task run“</span><span class="sxs-lookup"><span data-stu-id="6288a-144">Added support Local context in acr task run</span></span>

### <a name="acs"></a><span data-ttu-id="6288a-145">ACS</span><span class="sxs-lookup"><span data-stu-id="6288a-145">ACS</span></span>

* <span data-ttu-id="6288a-146">[BREAKING CHANGE] az openshift create: `--workspace-resource-id` in `--workspace-id` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="6288a-146">[BREAKING CHANGE]az openshift create: rename `--workspace-resource-id` to `--workspace-id`.</span></span>

### <a name="ams"></a><span data-ttu-id="6288a-147">AMS</span><span class="sxs-lookup"><span data-stu-id="6288a-147">AMS</span></span>

* <span data-ttu-id="6288a-148">Befehle zum Anzeigen aktualisiert, sodass 3 zurückgegeben wird, wenn die Ressource nicht gefunden wurde</span><span class="sxs-lookup"><span data-stu-id="6288a-148">Updated show commands to return 3 when resource not found</span></span>

### <a name="appconfig"></a><span data-ttu-id="6288a-149">AppConfig</span><span class="sxs-lookup"><span data-stu-id="6288a-149">AppConfig</span></span>

* <span data-ttu-id="6288a-150">Fehler beim Anhängen der API-Version an die Anforderungs-URL korrigiert.</span><span class="sxs-lookup"><span data-stu-id="6288a-150">Fixed bug when appending api-version to request url.</span></span> <span data-ttu-id="6288a-151">Die vorhandene Lösung funktioniert nicht mit Paginierung.</span><span class="sxs-lookup"><span data-stu-id="6288a-151">The existing solution doesn't work with pagination.</span></span>
* <span data-ttu-id="6288a-152">Unterstützung für die Anzeige von weiteren Sprachen neben Englisch hinzugefügt, da der Back-End-Dienst Unicode für die Globalisierung unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6288a-152">Added support for showing languages besides English as our backend service support unicode for globalization.</span></span>

### <a name="appservice"></a><span data-ttu-id="6288a-153">AppService</span><span class="sxs-lookup"><span data-stu-id="6288a-153">AppService</span></span>

* <span data-ttu-id="6288a-154">Problem Nr. 11217 behoben: Web-App: „az webapp config ssl upload“ muss Slot-Parameter unterstützen.</span><span class="sxs-lookup"><span data-stu-id="6288a-154">Fixed issue #11217: webapp: az webapp config ssl upload should support slot parameter</span></span>
* <span data-ttu-id="6288a-155">Problem Nr. 10965 behoben: Error: Der Name darf nicht leer sein.</span><span class="sxs-lookup"><span data-stu-id="6288a-155">Fixed issue #10965: Error: Name cannot be empty.</span></span> <span data-ttu-id="6288a-156">Entfernen anhand von „ip_address“ und „subnet“ zulassen</span><span class="sxs-lookup"><span data-stu-id="6288a-156">Allow remove by ip_address and subnet</span></span>
* <span data-ttu-id="6288a-157">Unterstützung des Imports von Zertifikaten aus Key Vault hinzugefügt `az webapp config ssl import`</span><span class="sxs-lookup"><span data-stu-id="6288a-157">Added support for importing certificates from Key Vault `az webapp config ssl import`</span></span>

### <a name="arm"></a><span data-ttu-id="6288a-158">ARM</span><span class="sxs-lookup"><span data-stu-id="6288a-158">ARM</span></span>

* <span data-ttu-id="6288a-159">Paket „azure-mgmt-resource“ auf die Verwendung von 6.0.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="6288a-159">Updated azure-mgmt-resource package to use 6.0.0</span></span>
* <span data-ttu-id="6288a-160">Mandantenübergreifende Unterstützung für Befehl `az group deployment create` durch Hinzufügen des neuen Parameters `--aux-subs`</span><span class="sxs-lookup"><span data-stu-id="6288a-160">Cross Tenant Support for `az group deployment create` command by adding new parameter `--aux-subs`</span></span>
* <span data-ttu-id="6288a-161">Neuer Parameter `--metadata` hinzugefügt, um das Hinzufügen von Metadateninformationen für Richtliniensatzdefinitionen zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="6288a-161">Added new parameter `--metadata` to support adding metadata information for policy set definitions.</span></span>

### <a name="backup"></a><span data-ttu-id="6288a-162">Backup</span><span class="sxs-lookup"><span data-stu-id="6288a-162">Backup</span></span>

* <span data-ttu-id="6288a-163">Unterstützung der Sicherung für SQL- und SAP Hana-Workloads hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-163">Added Backup support for SQL and SAP Hana workload.</span></span>

### <a name="botservice"></a><span data-ttu-id="6288a-164">BotService</span><span class="sxs-lookup"><span data-stu-id="6288a-164">BotService</span></span>

* <span data-ttu-id="6288a-165">[Breaking Change] Flag „--version“ aus Vorschaubefehl „az bot create“ entfernt.</span><span class="sxs-lookup"><span data-stu-id="6288a-165">[Breaking change] Remove '--version' flag from preview command 'az bot create'.</span></span> <span data-ttu-id="6288a-166">Nur v4-SDK-Bots werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6288a-166">Only v4 SDK bots are supported.</span></span>
* <span data-ttu-id="6288a-167">Überprüfung der Namensverfügbarkeit für „az bot create“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-167">Added name availability check for 'az bot create'.</span></span>
* <span data-ttu-id="6288a-168">Unterstützung für das Aktualisieren der Symbol-URL für einen Bot über „az bot update“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-168">Added support for updating the icon URL for a bot via 'az bot update'.</span></span>
* <span data-ttu-id="6288a-169">Unterstützung für das Aktualisieren eines Direct Line-Kanals über „az bot directline update“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-169">Added support for updating a Direct Line channel via 'az bot directline update'.</span></span>
* <span data-ttu-id="6288a-170">Unterstützung für Flag „--enable-enhanced-auth“ zu „az bot directline create“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-170">Added '--enable-enhanced-auth' flag support to 'az bot directline create'.</span></span>
* <span data-ttu-id="6288a-171">Die folgenden Befehlsgruppen sind allgemein verfügbar und befinden sich nicht in der Vorschau: „az bot authsetting“.</span><span class="sxs-lookup"><span data-stu-id="6288a-171">The following command groups are GA and not in preview: 'az bot authsetting'.</span></span>
* <span data-ttu-id="6288a-172">Die folgenden Befehle in „az bot“ sind allgemein verfügbar und befinden sich nicht in der Vorschau: „create“, „prepare-deploy“, „show“, „delete“, „update“.</span><span class="sxs-lookup"><span data-stu-id="6288a-172">The following commands in 'az bot' are GA and not in preview: 'create', 'prepare-deploy', 'show', 'delete', 'update'.</span></span>
* <span data-ttu-id="6288a-173">„az bot prepare-deploy“ korrigiert, indem der Wert voon „--proj-file-path“ in Kleinschreibung geändert wurde (z. B. „Test.csproj“ in „test.csproj“).</span><span class="sxs-lookup"><span data-stu-id="6288a-173">Fixed 'az bot prepare-deploy' changing '--proj-file-path' value to lower case (e.g. "Test.csproj" to "test.csproj").</span></span>

### <a name="compute"></a><span data-ttu-id="6288a-174">Compute</span><span class="sxs-lookup"><span data-stu-id="6288a-174">Compute</span></span>

* <span data-ttu-id="6288a-175">vmss create/update: „--scale-in-policy“ hinzugefügt, womit entschieden wird, welche virtuellen Computer beim horizontalen Herunterskalieren einer VM-Skalierungsgruppe zum Entfernen ausgewählt werden.</span><span class="sxs-lookup"><span data-stu-id="6288a-175">vmss create/update: Added --scale-in-policy, which decides which virtual machines are chosen for removal when a VMSS is scaled-in.</span></span>
* <span data-ttu-id="6288a-176">vm/vmss update: „--priority“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-176">vm/vmss update: Added --priority.</span></span>
* <span data-ttu-id="6288a-177">vm/vmss update: „--max-price“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-177">vm/vmss update: Added --max-price.</span></span>
* <span data-ttu-id="6288a-178">Befehlsgruppe „disk-encryption-set“ hinzugefügt (create, show, update, delete, list).</span><span class="sxs-lookup"><span data-stu-id="6288a-178">Added disk-encryption-set command group (create, show, update, delete, list).</span></span>
* <span data-ttu-id="6288a-179">disk create: „--encryption-type“ und „--disk-encryption-set“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-179">disk create: Added --encryption-type and --disk-encryption-set.</span></span>
* <span data-ttu-id="6288a-180">vm/vmss create: „--os-disk-encryption-set“ und „--data-disk-encryption-sets“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-180">vm/vmss create: Added --os-disk-encryption-set and --data-disk-encryption-sets.</span></span>

### <a name="core"></a><span data-ttu-id="6288a-181">Core</span><span class="sxs-lookup"><span data-stu-id="6288a-181">Core</span></span>

* <span data-ttu-id="6288a-182">Unterstützung für Python 3.4 entfernt</span><span class="sxs-lookup"><span data-stu-id="6288a-182">Removed support for Python 3.4</span></span>
* <span data-ttu-id="6288a-183">Plug-In für HaTS-Umfrage in mehreren Befehlen</span><span class="sxs-lookup"><span data-stu-id="6288a-183">Plug in HaTS survey in multiple commands</span></span>

### <a name="dls"></a><span data-ttu-id="6288a-184">DLS</span><span class="sxs-lookup"><span data-stu-id="6288a-184">DLS</span></span>

* <span data-ttu-id="6288a-185">ADLS-SDK-Version aktualisiert (0.0.48).</span><span class="sxs-lookup"><span data-stu-id="6288a-185">Updated ADLS sdk version (0.0.48).</span></span>

### <a name="install"></a><span data-ttu-id="6288a-186">Installieren</span><span class="sxs-lookup"><span data-stu-id="6288a-186">Install</span></span>

* <span data-ttu-id="6288a-187">Installationsskript unterstützt Python 3.8</span><span class="sxs-lookup"><span data-stu-id="6288a-187">Install script support python 3.8</span></span>

### <a name="iot"></a><span data-ttu-id="6288a-188">IoT</span><span class="sxs-lookup"><span data-stu-id="6288a-188">IOT</span></span>

* <span data-ttu-id="6288a-189">[BREAKING CHANGE] Parameter „--failover-region“ aus „manual-failover“ entfernt.</span><span class="sxs-lookup"><span data-stu-id="6288a-189">[BREAKING CHANGE] Removed --failover-region parameter from manual-failover.</span></span> <span data-ttu-id="6288a-190">Das Failover erfolgt jetzt in eine zugewiesene, geografisch gekoppelte sekundäre Region.</span><span class="sxs-lookup"><span data-stu-id="6288a-190">Now it will failover to assigned geo-paired secondary region.</span></span>

### <a name="key-vault"></a><span data-ttu-id="6288a-191">Key Vault</span><span class="sxs-lookup"><span data-stu-id="6288a-191">Key Vault</span></span>

* <span data-ttu-id="6288a-192">Nr. 8095 behoben: `az keyvault storage remove`: Hilfemeldung verbessert</span><span class="sxs-lookup"><span data-stu-id="6288a-192">Fixed #8095: `az keyvault storage remove`: improve the help message</span></span>
* <span data-ttu-id="6288a-193">Nr. 8921 behoben: `az keyvault key/secret/certificate list/list-deleted/list-versions`: Validierungsfehler in Parameter `--maxresults` behoben</span><span class="sxs-lookup"><span data-stu-id="6288a-193">Fixed #8921: `az keyvault key/secret/certificate list/list-deleted/list-versions`: fix the validation bug on parameter `--maxresults`</span></span>
* <span data-ttu-id="6288a-194">Nr. 10512 behoben: `az keyvault set-policy`: Fehlermeldung verbessert, wenn weder `--object-id`, `--spn` noch `--upn` angegeben ist</span><span class="sxs-lookup"><span data-stu-id="6288a-194">Fixed #10512: `az keyvault set-policy`: improve the error message when none of `--object-id`, `--spn` or `--upn` is specified</span></span>
* <span data-ttu-id="6288a-195">Nr. 10846 behoben: `az keyvault secret show-deleted`: Wenn `--id` angegeben ist, ist `--name/-n` nicht erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6288a-195">Fixed #10846: `az keyvault secret show-deleted`: when `--id` is specified, `--name/-n` is not required</span></span>
* <span data-ttu-id="6288a-196">Nr. 11084 behoben: `az keyvault secret download`: Hilfemeldung von Parameter `--encoding` verbessert</span><span class="sxs-lookup"><span data-stu-id="6288a-196">Fixed #11084: `az keyvault secret download`: improve the help message of parameter `--encoding`</span></span>

### <a name="network"></a><span data-ttu-id="6288a-197">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6288a-197">Network</span></span>

* <span data-ttu-id="6288a-198">az network application-gateway probe: Unterstützung für Option „--port“ hinzugefügt, um einen Port zum Prüfen von Back-End-Servern beim Erstellen und Aktualisieren anzugeben</span><span class="sxs-lookup"><span data-stu-id="6288a-198">az network application-gateway probe: Added support --port option to specify a port for probing backend servers when create and update</span></span>
* <span data-ttu-id="6288a-199">az network application-gateway url-path-map create/update: Fehlerbehebung für `--waf-policy`</span><span class="sxs-lookup"><span data-stu-id="6288a-199">az network application-gateway url-path-map create/update: bug fix for `--waf-policy`</span></span>
* <span data-ttu-id="6288a-200">az network application-gateway: Unterstützung für `--rewrite-rule-set` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-200">az network application-gateway: Added support `--rewrite-rule-set`</span></span>
* <span data-ttu-id="6288a-201">az network list-service-aliases: Unterstützung für Listendienstaliase hinzugefügt, die für Dienstendpunktrichtlinien verwendet werden können</span><span class="sxs-lookup"><span data-stu-id="6288a-201">az network list-service-aliases: Added support list service aliases which can be used for Service Endpoint Policies</span></span>
* <span data-ttu-id="6288a-202">az network dns zone import: Unterstützung für „.@“ in Datensatzname hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-202">az network dns zone import: Added support .@ in record name</span></span>

### <a name="packaging"></a><span data-ttu-id="6288a-203">Verpackung</span><span class="sxs-lookup"><span data-stu-id="6288a-203">Packaging</span></span>

* <span data-ttu-id="6288a-204">Back-Edge-Builds für PIP-Installation hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-204">Added back edge builds for pip install</span></span>
* <span data-ttu-id="6288a-205">Ubuntu-Eoan-Paket hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-205">Added Ubuntu eoan package</span></span>

### <a name="policy"></a><span data-ttu-id="6288a-206">Richtlinie</span><span class="sxs-lookup"><span data-stu-id="6288a-206">Policy</span></span>

* <span data-ttu-id="6288a-207">Unterstützung für Version 2019-09-01 der Richtlinien-API hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-207">Added support for Policy API version 2019-09-01.</span></span>
* <span data-ttu-id="6288a-208">az policy set-definition: Unterstützung der Gruppierung innerhalb von Richtliniensatzdefinitionen mit `--definition-groups`-Parameter hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-208">az policy set-definition: Added support grouping within policy set definitions with `--definition-groups` parameter</span></span>

### <a name="redis"></a><span data-ttu-id="6288a-209">Redis</span><span class="sxs-lookup"><span data-stu-id="6288a-209">Redis</span></span>

* <span data-ttu-id="6288a-210">Vorschauparameter `--replicas-per-master` zu Befehl `az redis create`hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-210">Added preview param `--replicas-per-master` to `az redis create` command</span></span>
* <span data-ttu-id="6288a-211">„azure-mgmt-redis“ von 6.0.0 auf 7.0.0rc1 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="6288a-211">Updated azure-mgmt-redis from 6.0.0 to 7.0.0rc1</span></span>

### <a name="servicefabric"></a><span data-ttu-id="6288a-212">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="6288a-212">ServiceFabric</span></span>

* <span data-ttu-id="6288a-213">Hinzufügen von Logik in Knotentyp korrigiert, einschließlich Nr. 10963: Beim Hinzufügen eines neuen Knotentyps mit Dauerhaftigkeitsstufe „Gold“ wird immer ein CLI-Fehler ausgegeben.</span><span class="sxs-lookup"><span data-stu-id="6288a-213">Fixed in node-type add logic including #10963: Adding new node type with durability level Gold will always throw CLI error</span></span>
* <span data-ttu-id="6288a-214">ServiceFabricNodeVmExt-Version in Erstellungsvorlage auf 1.1 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="6288a-214">Updated ServiceFabricNodeVmExt version to 1.1 in creation template</span></span>

### <a name="sql"></a><span data-ttu-id="6288a-215">SQL</span><span class="sxs-lookup"><span data-stu-id="6288a-215">SQL</span></span>

* <span data-ttu-id="6288a-216">Parameter „--read-scale“ und „--read-replicas“ zu Befehlen „sql db create“ und „sql db update“ hinzugefügt, um Leseskalierungsverwaltung zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="6288a-216">Added "--read-scale" and "--read-replicas" parameters to sql db create and update commands, to support read scale management.</span></span>

### <a name="storage"></a><span data-ttu-id="6288a-217">Storage</span><span class="sxs-lookup"><span data-stu-id="6288a-217">Storage</span></span>

* <span data-ttu-id="6288a-218">Allgemein verfügbares Release – Eigenschaft „Large File Shares“ für Befehle „storage account create“ und „storage account update“</span><span class="sxs-lookup"><span data-stu-id="6288a-218">GA Release Large File Shares property for storage account create and update command</span></span>
* <span data-ttu-id="6288a-219">Allgemein verfügbares Release – Unterstützung von SAS-Token für die Benutzerdelegierung</span><span class="sxs-lookup"><span data-stu-id="6288a-219">GA Release User Delegation SAS token Support</span></span>
* <span data-ttu-id="6288a-220">Neue Befehle `az storage account blob-service-properties show` und `az storage account blob-service-properties update --enable-change-feed` hinzugefügt, um Blob-Diensteigenschaften für das Speicherkonto zu verwalten.</span><span class="sxs-lookup"><span data-stu-id="6288a-220">Added new commands `az storage account blob-service-properties show` and `az storage account blob-service-properties update --enable-change-feed` to manage blob service properties for storage account.</span></span>
* <span data-ttu-id="6288a-221">[BEVORSTEHENDER BREAKING CHANGE] `az storage copy`: Das Zeichen `*` wird nicht mehr als Platzhalter in der URL, es werden jedoch die neuen Parameter „--include-pattern“ und „--exclude-pattern“ mit Unterstützung des Platzhalters `*` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-221">[COMING BREAKING CHANGE] `az storage copy`: `*` character is no longer supported as a wildcard in URL, but new parameters --include-pattern and --exclude-pattern will be added with `*` wildcard support.</span></span>
* <span data-ttu-id="6288a-222">Problem Nr. 11043 behoben: Unterstützung für das Entfernen des gesamten Containers/der gesamten Freigabe in `az storage remove` Befehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-222">Fixed issue #11043: Added support to remove whole container/share in `az storage remove` command</span></span>

## <a name="november-26-2019"></a><span data-ttu-id="6288a-223">26. November 2019</span><span class="sxs-lookup"><span data-stu-id="6288a-223">November 26, 2019</span></span>

<span data-ttu-id="6288a-224">Version 2.0.77</span><span class="sxs-lookup"><span data-stu-id="6288a-224">Version 2.0.77</span></span>

### <a name="acr"></a><span data-ttu-id="6288a-225">ACR</span><span class="sxs-lookup"><span data-stu-id="6288a-225">ACR</span></span>

* <span data-ttu-id="6288a-226">Parameter `--branch` in „acr task create/update“ als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="6288a-226">Deprecated parameter `--branch` from acr task create/update</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="6288a-227">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="6288a-227">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="6288a-228">`--workspace-resource-id`-Flag hinzugefügt, um die Erstellung eines Azure Red Hat OpenShift-Clusters mit Überwachung zuzulassen</span><span class="sxs-lookup"><span data-stu-id="6288a-228">Added `--workspace-resource-id` flag to allow creation of Azure Red Hat Openshift cluster with monitoring</span></span>
* <span data-ttu-id="6288a-229">`monitor_profile`-Flag hinzugefügt, um einen Azure Red Hat OpenShift-Clusters mit Überwachung zu erstellen</span><span class="sxs-lookup"><span data-stu-id="6288a-229">Added `monitor_profile` to create Azure Red Hat OpenShift cluster with monitoring</span></span>

### <a name="aks"></a><span data-ttu-id="6288a-230">AKS</span><span class="sxs-lookup"><span data-stu-id="6288a-230">AKS</span></span>

* <span data-ttu-id="6288a-231">Unterstützung des Rotationsvorgangs für Clusterzertifikate mithilfe von für Cluster Zertifikat Rotation mit „az aks rotate-certs“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-231">Added support cluster certificate rotation operation using "az aks rotate-certs".</span></span>

### <a name="appconfig"></a><span data-ttu-id="6288a-232">AppConfig</span><span class="sxs-lookup"><span data-stu-id="6288a-232">AppConfig</span></span>

* <span data-ttu-id="6288a-233">Unterstützung für die Verwendung von „:“ für `as az appconfig kv import`-Trennzeichen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-233">Added support for using ":" for `as az appconfig kv import` separator</span></span>
* <span data-ttu-id="6288a-234">Problem beim Auflisten von Schlüsselwerten mit mehreren Bezeichnungen, einschließlich NULL-Bezeichnung, behoben.</span><span class="sxs-lookup"><span data-stu-id="6288a-234">Fixed issue for listing key values with multiple labels including null label.</span></span> 
* <span data-ttu-id="6288a-235">Verwaltungsebenen-SDK, „azure-mgmt-appconfiguration“, auf Version 0.3.0 aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="6288a-235">Updated management plane sdk, azure-mgmt-appconfiguration, to version 0.3.0.</span></span> 

### <a name="appservice"></a><span data-ttu-id="6288a-236">AppService</span><span class="sxs-lookup"><span data-stu-id="6288a-236">AppService</span></span>

* <span data-ttu-id="6288a-237">Problem Nr. 11100 behoben AttributeError für „az webapp up“ beim Erstellen eines Dienstplans</span><span class="sxs-lookup"><span data-stu-id="6288a-237">Fixed issue #11100: AttributeError for az webapp up when create service plan</span></span>
* <span data-ttu-id="6288a-238">az webapp up: Erzwingen der Erstellung oder Bereitstellung auf einer Website für unterstützte Sprachen, es werden keine Standardeinstellungen verwendet.</span><span class="sxs-lookup"><span data-stu-id="6288a-238">az webapp up: Forcing the creation or deployment to a site for supported languages, no defaults used.</span></span>
* <span data-ttu-id="6288a-239">Unterstützung für App Service-Umgebung hinzugefügt: az appservice ase show | list | list-addresses | list-plans | create | update | delete</span><span class="sxs-lookup"><span data-stu-id="6288a-239">Added support for App Service Environment: az appservice ase show | list | list-addresses | list-plans | create | update | delete</span></span>

### <a name="backup"></a><span data-ttu-id="6288a-240">Backup</span><span class="sxs-lookup"><span data-stu-id="6288a-240">Backup</span></span>

* <span data-ttu-id="6288a-241">Problem in Az-Sicherungsrichtlinie „list-associated-items“ behoben.</span><span class="sxs-lookup"><span data-stu-id="6288a-241">Fixed issue in az backup policy list-associated-items.</span></span> <span data-ttu-id="6288a-242">Optionaler Parameter „BackupManagementType“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-242">Added optional BackupManagementType parameter.</span></span>

### <a name="compute"></a><span data-ttu-id="6288a-243">Compute</span><span class="sxs-lookup"><span data-stu-id="6288a-243">Compute</span></span>

* <span data-ttu-id="6288a-244">API-Version von Compute, Datenträger, Momentaufnahmen auf 2019-07-01 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="6288a-244">Upgraded API version of compute, disks, snapshots to 2019-07-01</span></span>
* <span data-ttu-id="6288a-245">vmss create: Verbesserung für – Orchestrierungsmodus</span><span class="sxs-lookup"><span data-stu-id="6288a-245">vmss create: Improvement for --orchestration-mode</span></span>
* <span data-ttu-id="6288a-246">sig image-definition create: „--os-state“ hinzugefügt, um die Angabe zu ermöglichen, ob die unter diesem Image erstellten virtuellen Computer „generalisiert“ oder „spezialisiert“ sind</span><span class="sxs-lookup"><span data-stu-id="6288a-246">sig image-definition create: Added --os-state to allow specifying whether the virtual machines created under this image are 'Generalized' or 'Specialized'</span></span>
* <span data-ttu-id="6288a-247">sig image-definition create: „--hyper-v-generation“ hinzugefügt, um die Angabe der Hypervisorgeneration zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="6288a-247">sig image-definition create: Added --hyper-v-generation to allow specifying the hypervisor generation</span></span>
* <span data-ttu-id="6288a-248">sig image-version create: Unterstützung für „--os-snapshot“ und „--data-snapshots“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-248">sig image-version create: Added support --os-snapshot and --data-snapshots</span></span>
* <span data-ttu-id="6288a-249">image create: „--data-disk-caching“ hinzugefügt, um die Angabe der Zwischenspeicherungseinstellung von Datenträger zu ermöflichen</span><span class="sxs-lookup"><span data-stu-id="6288a-249">image create: Added --data-disk-caching to allow specifying caching setting of data disks</span></span>
* <span data-ttu-id="6288a-250">Upgrade des Python-Compute-SDK auf 10.0.0</span><span class="sxs-lookup"><span data-stu-id="6288a-250">Upgraded Python Compute SDK to 10.0.0</span></span>
* <span data-ttu-id="6288a-251">vm/vmss create: „Spot“ zu Aufzählungseigenschaft „Priority“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-251">vm/vmss create: Added 'Spot' to 'Priority' enum property</span></span>
* <span data-ttu-id="6288a-252">[Breaking Change] Parameter „--max-billing“ für sowohl VM als auch VMSS in „--max-price“ umbenannt, um die Konsistenz mit Swagger- und PowerShell-Cmdlets sicherzustellen</span><span class="sxs-lookup"><span data-stu-id="6288a-252">[Breaking change] Renamed '--max-billing' parameter to '--max-price', for both VM and VMSS, to be consistent with Swagger and Powershell cmdlets</span></span>
* <span data-ttu-id="6288a-253">vm monitor log show: Unterstützung für das Abfragen von Protokollen über verknüpften Protokollanalyse-Arbeitsbereich hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-253">vm monitor log show: Added support for querying log over linked log analytics workspace.</span></span>

### <a name="iot"></a><span data-ttu-id="6288a-254">IoT</span><span class="sxs-lookup"><span data-stu-id="6288a-254">IOT</span></span>

* <span data-ttu-id="6288a-255">Behebung Nr. 2531: Argumente für Benutzerfreundlichkeit für Hub-Update hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-255">Fix #2531: Added convenience arguments for hub update.</span></span>
* <span data-ttu-id="6288a-256">Behebung Nr. 8323: Fehlende Parameter zum Erstellen eines benutzerdefinierten Speicherendpunkts hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-256">Fix #8323: Added missing parameters to create storage custom endpoint.</span></span>
* <span data-ttu-id="6288a-257">Regressionsfehler behoben: Die Änderungen wurden rückgängig gemacht, sodass der standardmäßige Speicherendpunkt überschrieben wurde.</span><span class="sxs-lookup"><span data-stu-id="6288a-257">Fix regression bug: Reverted the changes which overrides the default storage endpoint.</span></span>

### <a name="key-vault"></a><span data-ttu-id="6288a-258">Key Vault</span><span class="sxs-lookup"><span data-stu-id="6288a-258">Key Vault</span></span>

* <span data-ttu-id="6288a-259">Nr. 11121 behoben: Bei der Verwendung von `az keyvault certificate list` erfordert die Übergabe von `--include-pending` jetzt nicht mehr den Wert `true` oder `false`.</span><span class="sxs-lookup"><span data-stu-id="6288a-259">Fixed #11121: When using `az keyvault certificate list`, passing `--include-pending` now doesn't require a value of `true` or `false`</span></span>

### <a name="netappfiles"></a><span data-ttu-id="6288a-260">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="6288a-260">NetAppFiles</span></span>

* <span data-ttu-id="6288a-261">Upgrade von „azure-mgmt-netapp“ auf Version 0.7.0, die einige zusätzliche Volumeeigenschaften enthält, die bevorstehenden Replikationsvorgängen zugeordnet sind</span><span class="sxs-lookup"><span data-stu-id="6288a-261">Upgraded azure-mgmt-netapp to 0.7.0 which includes some additional volume properties associated with upcoming replication operations</span></span>

### <a name="network"></a><span data-ttu-id="6288a-262">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6288a-262">Network</span></span>

* <span data-ttu-id="6288a-263">application-gateway waf-config: veraltet</span><span class="sxs-lookup"><span data-stu-id="6288a-263">application-gateway waf-config: deprecated</span></span>
* <span data-ttu-id="6288a-264">application-gateway waf-policy: Untergruppe „managed-rules“ zur Verwaltung von verwalteten Regelsätzen und Ausschlussregeln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-264">application-gateway waf-policy: Added subgroup managed-rules to manage managed rule sets and exclusion rules</span></span>
* <span data-ttu-id="6288a-265">application-gateway waf-policy: Untergruppe „policy-setting“ zur Verwaltung der globalen Konfiguration von „waf-policy“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-265">application-gateway waf-policy: Added subgroup policy-setting to manage global configuration of a waf-policy</span></span>
* <span data-ttu-id="6288a-266">[BREAKING CHANGE] application-gateway waf-policy: Untergruppenregel in „custom-rule“ umbenannt</span><span class="sxs-lookup"><span data-stu-id="6288a-266">[BREAKING CHANGE] application-gateway waf-policy: Renamed subgroup rule to custom-rule</span></span>
* <span data-ttu-id="6288a-267">application-gateway http-listener: „--firewall-policy“ beim Erstellen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-267">application-gateway http-listener: Added --firewall-policy when create</span></span>
* <span data-ttu-id="6288a-268">application-gateway url-path-map rule: „--firewall-policy“ beim Erstellen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-268">application-gateway url-path-map rule: Added --firewall-policy when create</span></span>

### <a name="packaging"></a><span data-ttu-id="6288a-269">Verpackung</span><span class="sxs-lookup"><span data-stu-id="6288a-269">Packaging</span></span>

* <span data-ttu-id="6288a-270">Az-Wrapper in Python neu geschrieben</span><span class="sxs-lookup"><span data-stu-id="6288a-270">Rewrote the az wrapper in Python</span></span>
* <span data-ttu-id="6288a-271">Unterstützung für Python 3.8 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-271">Added support for Python 3.8</span></span>
* <span data-ttu-id="6288a-272">Für RPM-Paket in Python 3 geändert</span><span class="sxs-lookup"><span data-stu-id="6288a-272">Changed to Python 3 for RPM package</span></span>

### <a name="profile"></a><span data-ttu-id="6288a-273">Profil</span><span class="sxs-lookup"><span data-stu-id="6288a-273">Profile</span></span>

* <span data-ttu-id="6288a-274">Fehler beim Ausführen von `az login -u {} -p {}` mit Microsoft-Konto entfernt</span><span class="sxs-lookup"><span data-stu-id="6288a-274">Polished error when running `az login -u {} -p {}` with Microsoft account</span></span>
* <span data-ttu-id="6288a-275">`SSLError` beim Ausführen von `az login` hinter einem Proxy mit einem selbstsignierten Stammzertifikat entfernt</span><span class="sxs-lookup"><span data-stu-id="6288a-275">Polished `SSLError` when running `az login` behind a proxy with self-signed root certificate</span></span>
* <span data-ttu-id="6288a-276">Nr. 10578 behoben: `az login` hängt, wenn mehrere Instanzen gleichzeitig unter Windows oder WSL gestartet werden.</span><span class="sxs-lookup"><span data-stu-id="6288a-276">Fixed #10578: `az login` hangs when more than one instances are launched at the same time on Windows or WSL</span></span>
* <span data-ttu-id="6288a-277">Nr. 11059 behoben: `az login --allow-no-subscriptions` schlägt fehl, wenn Abonnements im Mandanten vorhanden sind.</span><span class="sxs-lookup"><span data-stu-id="6288a-277">Fixed #11059: `az login --allow-no-subscriptions` fails if there are subscriptions in the tenant</span></span>
* <span data-ttu-id="6288a-278">Nr. 11238 behoben: Nach dem Umbenennen eines Abonnements führt die Anmeldung mit MSI dazu, dass das gleiche Abonnement zweimal angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="6288a-278">Fixed #11238: After renaming a subscription, logging in with MSI will result in the same subscription appearing twice</span></span>

### <a name="rbac"></a><span data-ttu-id="6288a-279">RBAC</span><span class="sxs-lookup"><span data-stu-id="6288a-279">RBAC</span></span>

* <span data-ttu-id="6288a-280">Nr. 10996 behoben: Fehler für `--force-change-password-next-login` in `az ad user update` entfernt, wenn `--password` nicht angegeben ist</span><span class="sxs-lookup"><span data-stu-id="6288a-280">Fixed #10996: Polish error for `--force-change-password-next-login` in `az ad user update` when `--password` is not specified</span></span>

### <a name="redis"></a><span data-ttu-id="6288a-281">Redis</span><span class="sxs-lookup"><span data-stu-id="6288a-281">Redis</span></span>

* <span data-ttu-id="6288a-282">Nr. 2902 behoben: Festlegen von Speicherkonfigurationen beim Aktualisieren des Basic-SKU-Cache vermeiden</span><span class="sxs-lookup"><span data-stu-id="6288a-282">Fixed #2902: Avoid setting memory configs while updating Basic SKU cache</span></span>

### <a name="reservations"></a><span data-ttu-id="6288a-283">Reservations</span><span class="sxs-lookup"><span data-stu-id="6288a-283">Reservations</span></span>

* <span data-ttu-id="6288a-284">SDK-Version auf 0.6.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="6288a-284">Upgraded SDK Version to 0.6.0</span></span>
* <span data-ttu-id="6288a-285">Abrechnungsplandetails nach dem Aufrufen von „Get-Gatalogs“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-285">Added billingplan details info after calling Get-Gatalogs</span></span>
* <span data-ttu-id="6288a-286">Neuer Befehl `az reservations reservation-order calculate` zum Berechnen des Preises für eine Reservierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-286">Added new command `az reservations reservation-order calculate` to calculate the price for a reservation</span></span>
* <span data-ttu-id="6288a-287">Neuer Befehl `az reservations reservation-order purchase` zum Erwerb einer neuen Reservierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-287">Added new command `az reservations reservation-order purchase` to purchase a new reservation</span></span>

### <a name="rest"></a><span data-ttu-id="6288a-288">REST</span><span class="sxs-lookup"><span data-stu-id="6288a-288">Rest</span></span>
* <span data-ttu-id="6288a-289">`az rest` in allgemeine Verfügbarkeit geändert</span><span class="sxs-lookup"><span data-stu-id="6288a-289">Changed `az rest` to GA</span></span>

### <a name="sql"></a><span data-ttu-id="6288a-290">SQL</span><span class="sxs-lookup"><span data-stu-id="6288a-290">SQL</span></span>

* <span data-ttu-id="6288a-291">„azure-mgmt-sql“ auf Version 0.15.0 aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="6288a-291">Updated azure-mgmt-sql to version 0.15.0.</span></span>

### <a name="storage"></a><span data-ttu-id="6288a-292">Storage</span><span class="sxs-lookup"><span data-stu-id="6288a-292">Storage</span></span>

* <span data-ttu-id="6288a-293">storage account create: „--enable-hierarchical-namespace“ hinzugefügt, um Dateisystemsemantik in Blobdienst zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="6288a-293">storage account create: Added --enable-hierarchical-namespace to support filesystem semantics in blob service.</span></span>
* <span data-ttu-id="6288a-294">Ausnahme ohne Zusammenhang aus Fehlermeldung entfernt</span><span class="sxs-lookup"><span data-stu-id="6288a-294">Removed unrelated exception from error message</span></span>
* <span data-ttu-id="6288a-295">Probleme mit falscher Fehlermeldung „Sie verfügen nicht über die erforderlichen Berechtigungen zum Ausführen dieses Vorgangs“ behoben.</span><span class="sxs-lookup"><span data-stu-id="6288a-295">Fixed issues with incorrect error message "You do not have the required permissions needed to perform this operation."</span></span> <span data-ttu-id="6288a-296">bei Blockierung durch Netzwerkregeln oder bei „AuthenticationFailed“.</span><span class="sxs-lookup"><span data-stu-id="6288a-296">when blocked by network rules or AuthenticationFailed.</span></span>

## <a name="november-4-2019"></a><span data-ttu-id="6288a-297">4\. November 2019</span><span class="sxs-lookup"><span data-stu-id="6288a-297">November 4, 2019</span></span>

<span data-ttu-id="6288a-298">Version 2.0.76</span><span class="sxs-lookup"><span data-stu-id="6288a-298">Version 2.0.76</span></span>

### <a name="acr"></a><span data-ttu-id="6288a-299">ACR</span><span class="sxs-lookup"><span data-stu-id="6288a-299">ACR</span></span>

* <span data-ttu-id="6288a-300">Vorschauparameter `--pack-image-tag` wurde dem Befehl `az acr pack build` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-300">Added a preview parameter `--pack-image-tag` to command `az acr pack build`.</span></span>
* <span data-ttu-id="6288a-301">Unterstützung der Aktivierung der Überwachung beim Erstellen einer Registrierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-301">Added support for enabling auditing on creating a registry</span></span>
* <span data-ttu-id="6288a-302">Unterstützung von RBAC mit Repositoryumfang hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-302">Added support for Repository-scoped RBAC</span></span>

### <a name="aks"></a><span data-ttu-id="6288a-303">AKS</span><span class="sxs-lookup"><span data-stu-id="6288a-303">AKS</span></span>

* <span data-ttu-id="6288a-304">`--enable-cluster-autoscaler`, `--min-count` und `--max-count` wurden dem Befehl `az aks create` hinzugefügt, sodass die automatische Clusterskalierung für den Knotenpool aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="6288a-304">Added `--enable-cluster-autoscaler`, `--min-count` and `--max-count` to the `az aks create` command, which enables cluster autoscaler for the node pool.</span></span>
* <span data-ttu-id="6288a-305">Die obigen Flags sowie `--update-cluster-autoscaler` und `--disable-cluster-autoscaler` wurden dem Befehl `az aks update` hinzugefügt, sodass Updates der automatischen Clusterskalierung zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="6288a-305">Added the above flags as well as `--update-cluster-autoscaler` and `--disable-cluster-autoscaler` to the `az aks update` command, allowing updates to cluster autoscaler.</span></span>

### <a name="appconfig"></a><span data-ttu-id="6288a-306">AppConfig</span><span class="sxs-lookup"><span data-stu-id="6288a-306">AppConfig</span></span>

* <span data-ttu-id="6288a-307">Befehlsgruppe der AppConfig-Funktion zum Verwalten von in einer App Configuration-Instanz gespeicherten Featureflags wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-307">Added appconfig feature command group to manage feature flags stored in an App Configuration.</span></span>
* <span data-ttu-id="6288a-308">Geringfügiger Programmfehler für Befehl „appconfig kv export to file“ wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="6288a-308">Fixed minor bug for appconfig kv export to file command.</span></span> <span data-ttu-id="6288a-309">Das Lesen der Zieldateiinhalte wird während des Exports angehalten.</span><span class="sxs-lookup"><span data-stu-id="6288a-309">Stop reading dest file contents during export.</span></span>

### <a name="appservice"></a><span data-ttu-id="6288a-310">AppService</span><span class="sxs-lookup"><span data-stu-id="6288a-310">AppService</span></span>

* <span data-ttu-id="6288a-311">`az appservice plan create`: Unterstützung für das Festlegen von „persitescalung“ beim Erstellen eines App-Serviceplans wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-311">`az appservice plan create`: Added support to set 'persitescaling' on appservice plan create.</span></span>
* <span data-ttu-id="6288a-312">Ein Problem wurde behoben, aufgrund dessen der Vorgang „webapp config ssl bind“ vorhandene Tags aus der Ressource entfernt hat.</span><span class="sxs-lookup"><span data-stu-id="6288a-312">Fixed an issue where webapp config ssl bind operation was removing existing tags from the resource</span></span>
* <span data-ttu-id="6288a-313">Flag `--build-remote` wurde für `az functionapp deployment source config-zip` hinzugefügt, um die Remotebuildaktion während der Funktions-App-Bereitstellung zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="6288a-313">Added `--build-remote` flag for `az functionapp deployment source config-zip` to support remote build action during function app deployment.</span></span>
* <span data-ttu-id="6288a-314">Die Standardknotenversion in Funktions-Apps wurde für Windows in ~ 10 geändert.</span><span class="sxs-lookup"><span data-stu-id="6288a-314">Changed default node version on function apps to ~10 for Windows</span></span>
* <span data-ttu-id="6288a-315">`--runtime-version`-Eigenschaft zu `az functionapp create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-315">Added `--runtime-version` property to `az functionapp create`</span></span>

### <a name="arm"></a><span data-ttu-id="6288a-316">ARM</span><span class="sxs-lookup"><span data-stu-id="6288a-316">ARM</span></span>

* <span data-ttu-id="6288a-317">`az deployment/group deployment validate`: Parameter `--handle-extended-json-format` wurde hinzugefügt, um bei der Bereitstellung mehrere Zeilen und Kommentare in der JSON-Vorlage zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="6288a-317">`az deployment/group deployment validate`: Added `--handle-extended-json-format` parameter to support multiline and comments in json template when deployment.</span></span>
* <span data-ttu-id="6288a-318">„azure-mgmt-resource“ auf „2019-07-01“ festgelegt</span><span class="sxs-lookup"><span data-stu-id="6288a-318">Bumped azure-mgmt-resource to 2019-07-01</span></span>

### <a name="backup"></a><span data-ttu-id="6288a-319">Backup</span><span class="sxs-lookup"><span data-stu-id="6288a-319">Backup</span></span>

* <span data-ttu-id="6288a-320">Unterstützung für AzureFiles-Sicherung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-320">Added AzureFiles backup support</span></span>

### <a name="compute"></a><span data-ttu-id="6288a-321">Compute</span><span class="sxs-lookup"><span data-stu-id="6288a-321">Compute</span></span>

* <span data-ttu-id="6288a-322">`az vm create`: Beim gleichzeitigen Festlegen von beschleunigtem Netzwerkbetrieb und einer vorhandenen NIC wurde eine Warnung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-322">`az vm create`: Added warning when specifying accelerated networking and an existing NIC together.</span></span>
* <span data-ttu-id="6288a-323">`az vm create`: `--vmss` hinzugefügt, um eine vorhandene VM-Skalierungsgruppe anzugeben, welcher der virtuelle Computer zugewiesen werden soll.</span><span class="sxs-lookup"><span data-stu-id="6288a-323">`az vm create`: Added `--vmss` to specify an existing virtual machine scale set that the virtual machine should be assigned to.</span></span>
* <span data-ttu-id="6288a-324">`az vm/vmss create`: Eine lokale Kopie der Imagealiasdatei wurde hinzugefügt, sodass in einer eingeschränkten Netzwerkumgebung darauf zugegriffen werden kann.</span><span class="sxs-lookup"><span data-stu-id="6288a-324">`az vm/vmss create`: Added a local copy of image alias file so that it can be accessed in a restricted network environment.</span></span>
* <span data-ttu-id="6288a-325">`az vmss create`: `--orchestration-mode` hinzugefügt, um anzugeben, wie virtuelle Computer von der Skalierungsgruppe verwaltet werden.</span><span class="sxs-lookup"><span data-stu-id="6288a-325">`az vmss create`: Added `--orchestration-mode` to specify how virtual machines are managed by the scale set.</span></span>
* <span data-ttu-id="6288a-326">`az vm/vmss update`: `--ultra-ssd-enabled` hinzugefügt, um das Aktualisieren der SSD-Einstellung zuzulassen.</span><span class="sxs-lookup"><span data-stu-id="6288a-326">`az vm/vmss update`: Added `--ultra-ssd-enabled` to allow updating ultra SSD setting.</span></span>
* <span data-ttu-id="6288a-327">[BREAKING CHANGE] `az vm extension set`: Ein Fehler wurde behoben, aufgrund dessen Benutzer mit `--ids` keine Erweiterung auf einem virtuellen Computer festlegen konnten.</span><span class="sxs-lookup"><span data-stu-id="6288a-327">[BREAKING CHANGE] `az vm extension set`: Fixed bug where users could not set an extension on a VM with `--ids`.</span></span>
* <span data-ttu-id="6288a-328">Neue Befehle wurden zu `az vm image terms accept/cancel/show` hinzugefügt , um Azure Marketplace-Imagebedingungen zu verwalten.</span><span class="sxs-lookup"><span data-stu-id="6288a-328">Added new commands `az vm image terms accept/cancel/show` to manage Azure Marketplace image terms.</span></span>
* <span data-ttu-id="6288a-329">VMAccessForLinux auf Version 1.5 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="6288a-329">Updated VMAccessForLinux to version 1.5</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="6288a-330">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="6288a-330">CosmosDB</span></span>

* <span data-ttu-id="6288a-331">[BREAKING CHANGE] `az sql container create`: `--partition-key-path` in erforderlichen Parameter geändert</span><span class="sxs-lookup"><span data-stu-id="6288a-331">[BREAKING CHANGE] `az sql container create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="6288a-332">[BREAKING CHANGE] `az gremlin graph create`: `--partition-key-path` in erforderlichen Parameter geändert</span><span class="sxs-lookup"><span data-stu-id="6288a-332">[BREAKING CHANGE] `az gremlin graph create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="6288a-333">`az sql container create`: `--unique-key-policy` und `--conflict-resolution-policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-333">`az sql container create`: Added `--unique-key-policy` and `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="6288a-334">`az sql container create/update`: Aktualisierung des `--idx`-Standardschemas</span><span class="sxs-lookup"><span data-stu-id="6288a-334">`az sql container create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="6288a-335">`gremlin graph create`: `--conflict-resolution-policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-335">`gremlin graph create`: Added `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="6288a-336">`gremlin graph create/update`: Aktualisierung des `--idx`-Standardschemas</span><span class="sxs-lookup"><span data-stu-id="6288a-336">`gremlin graph create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="6288a-337">Tippfehler in Hilfemeldung korrigiert</span><span class="sxs-lookup"><span data-stu-id="6288a-337">Fixed typo in help message</span></span>
* <span data-ttu-id="6288a-338">Datenbank: Ablaufinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-338">database: Added deprecation infomation</span></span>
* <span data-ttu-id="6288a-339">Auflistung: Ablaufinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-339">collection: Added deprecation infomation</span></span>

### <a name="iot"></a><span data-ttu-id="6288a-340">IoT</span><span class="sxs-lookup"><span data-stu-id="6288a-340">IoT</span></span>

* <span data-ttu-id="6288a-341">Neuer Routingquelltyp hinzugefügt: DigitalTwinChangeEvents</span><span class="sxs-lookup"><span data-stu-id="6288a-341">Added new routing source type: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="6288a-342">Fehlende Features in `az iot hub create` behoben</span><span class="sxs-lookup"><span data-stu-id="6288a-342">Fixed missing features in `az iot hub create`</span></span>

### <a name="key-vault"></a><span data-ttu-id="6288a-343">Key Vault</span><span class="sxs-lookup"><span data-stu-id="6288a-343">Key Vault</span></span>

* <span data-ttu-id="6288a-344">Ein unerwarteter Fehler wurde behoben, bei dem keine Zertifikatdatei vorhanden war.</span><span class="sxs-lookup"><span data-stu-id="6288a-344">Fixed an unexpected error when certificate file does not exist</span></span>
* <span data-ttu-id="6288a-345">Funktionsunfähigkeit von `az keyvault recover/purge` behoben</span><span class="sxs-lookup"><span data-stu-id="6288a-345">Fixed `az keyvault recover/purge` not working</span></span>

### <a name="netappfiles"></a><span data-ttu-id="6288a-346">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="6288a-346">NetAppFiles</span></span>

* <span data-ttu-id="6288a-347">„azure-mgmt-netapp“ wurde auf 0.6.0 aktualisiert, um API-Version 2019-07-01 zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="6288a-347">Upgraded azure-mgmt-netapp to 0.6.0 to use API version 2019-07-01.</span></span> <span data-ttu-id="6288a-348">Diese neue API-Version umfasst:</span><span class="sxs-lookup"><span data-stu-id="6288a-348">This new API version includes:</span></span>

    - <span data-ttu-id="6288a-349">Volumeerstellung `--protocol-types` akzeptiert jetzt „NFSv4.1“ anstelle von „NFSv4“.</span><span class="sxs-lookup"><span data-stu-id="6288a-349">Volume creation `--protocol-types` accepts now "NFSv4.1" not "NFSv4"</span></span>
    - <span data-ttu-id="6288a-350">Die Richtlinie der Volumeexportrichtlinie heißt jetzt „nfsv41“ anstelle von „nfsv4“.</span><span class="sxs-lookup"><span data-stu-id="6288a-350">Volume export policy property now named 'nfsv41' not 'nfsv4'</span></span>
    - <span data-ttu-id="6288a-351">Volume `--creation-token` wurde in `--file-path` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="6288a-351">Volume `--creation-token` renamed to `--file-path`</span></span>
    - <span data-ttu-id="6288a-352">Das Erstellungsdatum einer Momentaufnahme heißt jetzt einfach „erstellt“.</span><span class="sxs-lookup"><span data-stu-id="6288a-352">Snapshot creation date now named just 'created'</span></span>

### <a name="network"></a><span data-ttu-id="6288a-353">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6288a-353">Network</span></span>

* <span data-ttu-id="6288a-354">`az network private-dns link vnet create/update`: Unterstützung für mandantenübergreifende Verknüpfung virtueller Netzwerke.</span><span class="sxs-lookup"><span data-stu-id="6288a-354">`az network private-dns link vnet create/update`: Support cross-tenant virtual network linking.</span></span>
* <span data-ttu-id="6288a-355">[BREAKING CHANGE] `az network vnet subnet list`: `--resource-group` und `--vnet-name` wurden geändert und sind jetzt erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6288a-355">[BREAKING CHANGE] `az network vnet subnet list`: Changed `--resource-group` and `--vnet-name` to be required now.</span></span>
* <span data-ttu-id="6288a-356">`az network public-ip prefix create`: Unterstützung der Angabe der IP-Adressversion (IPv4, IPv6) bei der Erstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-356">`az network public-ip prefix create`: Added support to specify IP address version (IPv4, IPv6) when creation</span></span>
* <span data-ttu-id="6288a-357">„azure-mgmt-network“ auf 7.0.0 und „api-version“ auf 2019-09-01 festgelegt</span><span class="sxs-lookup"><span data-stu-id="6288a-357">Bumped azure-mgmt-network to 7.0.0 and api-version to 2019-09-01</span></span>
* <span data-ttu-id="6288a-358">`az network vrouter`: Unterstützung für neuen virtuellen Dienstrouter und virtuelles Routerpeering hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-358">`az network vrouter`: Added support for new service virtual router and virtual router peering</span></span>
* <span data-ttu-id="6288a-359">`az network express-route gateway connection`: Unterstützung für `--internet-security` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-359">`az network express-route gateway connection`: Added support for `--internet-security`</span></span>

### <a name="profile"></a><span data-ttu-id="6288a-360">Profil</span><span class="sxs-lookup"><span data-stu-id="6288a-360">Profile</span></span>

* <span data-ttu-id="6288a-361">Funktionsunfähigkeit von `az account get-access-token --resource-type ms-graph` behoben</span><span class="sxs-lookup"><span data-stu-id="6288a-361">Fixed `az account get-access-token --resource-type ms-graph` not working</span></span>
* <span data-ttu-id="6288a-362">Warnung aus `az login` entfernt</span><span class="sxs-lookup"><span data-stu-id="6288a-362">Removed warning from `az login`</span></span>

### <a name="rbac"></a><span data-ttu-id="6288a-363">RBAC</span><span class="sxs-lookup"><span data-stu-id="6288a-363">RBAC</span></span>

* <span data-ttu-id="6288a-364">Funktionsunfähigkeit von `az ad app update --id {} --display-name {}` behoben</span><span class="sxs-lookup"><span data-stu-id="6288a-364">Fixed `az ad app update --id {} --display-name {}` doesn't work</span></span>

### <a name="servicefabric"></a><span data-ttu-id="6288a-365">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="6288a-365">ServiceFabric</span></span>

* <span data-ttu-id="6288a-366">`az sf cluster create`: Ein Problem wurde behoben, indem die Compute-VMSS von „template.json“ für Service Fabric unter Linux und Windows von Standarddatenträgern auf verwaltete Datenträger umgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="6288a-366">`az sf cluster create`: Fixed an issue by modifying service fabric linux and windows template.json compute vmss from standard to managed disks</span></span>

### <a name="sql"></a><span data-ttu-id="6288a-367">SQL</span><span class="sxs-lookup"><span data-stu-id="6288a-367">SQL</span></span>

* <span data-ttu-id="6288a-368">Die Parameter `--compute-model`, `--auto-pause-delay` und `--min-capacity` wurden hinzugefügt, um CRUD-Vorgänge für das neue SQL-Datenbank-Angebot zu unterstützen: Serverloses Computemodell.</span><span class="sxs-lookup"><span data-stu-id="6288a-368">Added `--compute-model`, `--auto-pause-delay`, and `--min-capacity` parameters to support CRUD operations for new SQL Database offering: Serverless compute model.</span></span>

### <a name="storage"></a><span data-ttu-id="6288a-369">Storage</span><span class="sxs-lookup"><span data-stu-id="6288a-369">Storage</span></span>

* <span data-ttu-id="6288a-370">`az storage account create/update`: Parameter „--enable-files-adds“ und Azure Active Directory-Eigenschaftenargumentgruppe hinzugefügt, um Active Directory Domain-Dienstauthentifizierung für Azure Files zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="6288a-370">`az storage account create/update`: Added --enable-files-adds parameter and Azure Active Directory Properties Argument group to support Azure Files Active Directory Domain Service Authentication</span></span>
* <span data-ttu-id="6288a-371">`az storage account keys list/renew` wurde erweitert, um die Auflistung oder erneute Generierung von Kerberos-Schlüsseln des Speicherkontos zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="6288a-371">Expanded `az storage account keys list/renew` to support listing or regenerating Kerberos keys of storage account.</span></span>

## <a name="october-15-2019"></a><span data-ttu-id="6288a-372">15. Oktober 2019</span><span class="sxs-lookup"><span data-stu-id="6288a-372">October 15, 2019</span></span>

<span data-ttu-id="6288a-373">Version 2.0.75</span><span class="sxs-lookup"><span data-stu-id="6288a-373">Version 2.0.75</span></span>

### <a name="aks"></a><span data-ttu-id="6288a-374">AKS</span><span class="sxs-lookup"><span data-stu-id="6288a-374">AKS</span></span>

* <span data-ttu-id="6288a-375">Standardwert `--load-balancer-sku` in `standard` geändert, sofern von der Kubernetes-Version unterstützt</span><span class="sxs-lookup"><span data-stu-id="6288a-375">Changed `--load-balancer-sku` default value to `standard` if supported by the kubernetes version</span></span>
* <span data-ttu-id="6288a-376">Standardwert `--vm-set-type` in `virtualmachinescalesets` geändert, sofern von der Kubernetes-Version unterstützt</span><span class="sxs-lookup"><span data-stu-id="6288a-376">Changed `--vm-set-type` default value to `virtualmachinescalesets` if supported by the kubernetes version</span></span>

### <a name="ams"></a><span data-ttu-id="6288a-377">AMS</span><span class="sxs-lookup"><span data-stu-id="6288a-377">AMS</span></span>

* <span data-ttu-id="6288a-378">[BREAKING CHANGE] Name von `job start` in `job create` geändert</span><span class="sxs-lookup"><span data-stu-id="6288a-378">[BREAKING CHANGE] Changed the name of `job start` to `job create`</span></span>
* <span data-ttu-id="6288a-379">[BREAKING CHANGE] Parameter `--ask` von `content-key-policy create` geändert, sodass eine hexadezimale Zeichenfolge mit 32 Zeichen anstelle von UTF8 verwendet wird</span><span class="sxs-lookup"><span data-stu-id="6288a-379">[BREAKING CHANGE] Changed the `--ask` parameter of `content-key-policy create` to use a 32-character hex string instead of UTF8</span></span>

### <a name="appservice"></a><span data-ttu-id="6288a-380">AppService</span><span class="sxs-lookup"><span data-stu-id="6288a-380">AppService</span></span>

* <span data-ttu-id="6288a-381">Befehle vom Typ `webapp config access-restriction show|set|add|remove` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-381">Added commands `webapp config access-restriction show|set|add|remove`</span></span>
* <span data-ttu-id="6288a-382">Bessere Fehlerbehandlung zu `webapp up` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-382">Added better error handling to `webapp up`</span></span>
* <span data-ttu-id="6288a-383">Unterstützung für SKU `Isolated` zu `appservice plan update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-383">Added support for `Isolated` SKU to `appservice plan update`</span></span>

### <a name="arm"></a><span data-ttu-id="6288a-384">ARM</span><span class="sxs-lookup"><span data-stu-id="6288a-384">ARM</span></span>

* <span data-ttu-id="6288a-385">Parameter `--handle-extended-json-format` zu `deployment create` hinzugefügt, um mehrere Zeilen und Kommentare in der JSON-Vorlage zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="6288a-385">Added `--handle-extended-json-format` parameter `deployment create` to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="6288a-386">Compute</span><span class="sxs-lookup"><span data-stu-id="6288a-386">Compute</span></span>

* <span data-ttu-id="6288a-387">Parameter `--enable-agent` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-387">Added `--enable-agent` parameter to `vm create`</span></span>
* <span data-ttu-id="6288a-388">`vm create` geändert, um bei der Verwendung von Zonen die SKU „Standard“ für die öffentliche IP-Adresse zu verwenden</span><span class="sxs-lookup"><span data-stu-id="6288a-388">Changed `vm create` to use standard public IP SKU automatically when using zones</span></span>
* <span data-ttu-id="6288a-389">`vm create` geändert, um automatisch einen gültigen Computernamen für eine VM zu erstellen, falls keiner angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="6288a-389">Changed `vm create` to automatically create a valid computer name for a VM if none is provided</span></span>
* <span data-ttu-id="6288a-390">Parameter `--computer-name-prefix` zu `vmss create` hinzugefügt, um das benutzerdefinierte Computernamenspräfix virtueller Computer in VMSS zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="6288a-390">Added `--computer-name-prefix` parameter to `vmss create` to support custom computer name prefix of virtual machines in the VMSS</span></span>
* <span data-ttu-id="6288a-391">Parameter `--workspace` zu `vm create` hinzugefügt, um automatisch einen Log Analytics-Arbeitsbereich zu aktivieren</span><span class="sxs-lookup"><span data-stu-id="6288a-391">Add `--workspace` parameter to `vm create` to enable log analytics workspace automatically</span></span>
* <span data-ttu-id="6288a-392">API-Version für Kataloge auf 2019-07-01 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="6288a-392">Updated galleries API version to 2019-07-01</span></span>

### <a name="core"></a><span data-ttu-id="6288a-393">Core</span><span class="sxs-lookup"><span data-stu-id="6288a-393">Core</span></span>

* <span data-ttu-id="6288a-394">Syntaxprüfung für Parameter `--set` im generischen Updatebefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-394">Added syntax check for `--set` parameter in generic update command</span></span>

### <a name="iot"></a><span data-ttu-id="6288a-395">IoT</span><span class="sxs-lookup"><span data-stu-id="6288a-395">IoT</span></span>

* <span data-ttu-id="6288a-396">Problem behoben, bei dem für `iot hub show` der Fehler „Ressource nicht gefunden.“ zurückgegeben wurde</span><span class="sxs-lookup"><span data-stu-id="6288a-396">Fixed an issue where `iot hub show` would incorrectly error with "resource not found"</span></span>

### <a name="monitor"></a><span data-ttu-id="6288a-397">Überwachen</span><span class="sxs-lookup"><span data-stu-id="6288a-397">Monitor</span></span>

* <span data-ttu-id="6288a-398">Unterstützung für CRUD zu `monitor log-analytics workspace` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-398">Added support for CRUD to `monitor log-analytics workspace`</span></span>

### <a name="network"></a><span data-ttu-id="6288a-399">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6288a-399">Network</span></span>

* <span data-ttu-id="6288a-400">Unterstützung für mandantenübergreifende virtuelle Verbindung zu `network private-dns link vnet [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-400">Added support for cross-tenant virtual linking to `network private-dns link vnet [create|update]`</span></span>
* <span data-ttu-id="6288a-401">[BREAKING CHANGE]`network vnet subnet list` geändert, um Parameter `--resource-group` und `--vnet-name` vorauszusetzen</span><span class="sxs-lookup"><span data-stu-id="6288a-401">[BREAKING CHANGE] Changed `network vnet subnet list` to require `--resource-group` and `--vnet-name` parameters</span></span>

### <a name="sql"></a><span data-ttu-id="6288a-402">SQL</span><span class="sxs-lookup"><span data-stu-id="6288a-402">SQL</span></span>

* <span data-ttu-id="6288a-403">Befehle zu `sql mi ad-admin` hinzugefügt, die das Festlegen eines AAD-Administrators für verwaltete Instanzen unterstützen</span><span class="sxs-lookup"><span data-stu-id="6288a-403">Added commands to `sql mi ad-admin` that support setting an AAD administrator on managed instances</span></span>

### <a name="storage"></a><span data-ttu-id="6288a-404">Storage</span><span class="sxs-lookup"><span data-stu-id="6288a-404">Storage</span></span>

* <span data-ttu-id="6288a-405">Parameter `--preserve-s2s-access-tier` zu `storage copy` hinzugefügt, um die Zugriffsebene beim Kopieren von Dienst zu Dienst beizubehalten</span><span class="sxs-lookup"><span data-stu-id="6288a-405">Added `--preserve-s2s-access-tier` parameter `storage copy` to preserve access tier during service to service copy</span></span>
* <span data-ttu-id="6288a-406">Parameter `--enable-large-file-share` zu `storage account [create|update]` hinzugefügt, um große Dateifreigaben für ein Speicherkonto zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="6288a-406">Added `--enable-large-file-share` parameter to `storage account [create|update]` to support large file shares for storage account</span></span>

## <a name="september-24-2019"></a><span data-ttu-id="6288a-407">24. September 2019</span><span class="sxs-lookup"><span data-stu-id="6288a-407">September 24, 2019</span></span>

<span data-ttu-id="6288a-408">Version 2.0.74</span><span class="sxs-lookup"><span data-stu-id="6288a-408">Version 2.0.74</span></span>

### <a name="acr"></a><span data-ttu-id="6288a-409">ACR</span><span class="sxs-lookup"><span data-stu-id="6288a-409">ACR</span></span>

* <span data-ttu-id="6288a-410">Erforderlicher Parameter `--type` zu `acr config retention update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-410">Added a required `--type` parameter to `acr config retention update`</span></span>
* <span data-ttu-id="6288a-411">[BREAKING CHANGE] Umbenannter Parameter `--name -n` in `--registry -r ` für Befehlsgruppe `acr config` geändert</span><span class="sxs-lookup"><span data-stu-id="6288a-411">[BREAKING CHNAGE] Renamed parameter `--name -n` changed to `--registry -r ` for `acr config` command group</span></span>

### <a name="aks"></a><span data-ttu-id="6288a-412">AKS</span><span class="sxs-lookup"><span data-stu-id="6288a-412">AKS</span></span>

* <span data-ttu-id="6288a-413">Parameter `--load-balancer-sku` zum Befehl `aks create` hinzugefügt, um die Erstellung von AKS-Clustern mit SLB zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="6288a-413">Added `--load-balancer-sku` parameter to `aks create` command, which allows for creating AKS cluster with SLB</span></span>
* <span data-ttu-id="6288a-414">Parameter `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` und `--load-balancer-outbound-ip-prefixes` zu den Befehlen `aks [create|update]` hinzugefügt,um die Aktualisierung des Lastenausgleichsprofils eines AKS-Clusters mit SLB zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="6288a-414">Added `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` and `--load-balancer-outbound-ip-prefixes` parameters to `aks [create|update]` commands, which allow for updating load balancer profile of an AKS cluster with SLB</span></span>
* <span data-ttu-id="6288a-415">Parameter `--vm-set-type` zum Befehl `aks create` hinzugefügt, um die Angabe von VM-Typen eines AKS-Clusters (vmas oder vmss) zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="6288a-415">Added `--vm-set-type` parameter to `aks create` command, which allows to specify vm types of an AKS Cluster (vmas or vmss)</span></span>

### <a name="arm"></a><span data-ttu-id="6288a-416">ARM</span><span class="sxs-lookup"><span data-stu-id="6288a-416">ARM</span></span>

* <span data-ttu-id="6288a-417">Parameter `--handle-extended-json-format` zum Befehl `group deployment create` hinzugefügt, um mehrere Zeilen und Kommentare in der JSON-Vorlage zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="6288a-417">Added `--handle-extended-json-format` parameter to `group deployment create` command to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="6288a-418">Compute</span><span class="sxs-lookup"><span data-stu-id="6288a-418">Compute</span></span>

* <span data-ttu-id="6288a-419">Parameter `--terminate-notification-time` zu den Befehlen `vmss [create|update]` hinzugefügt, um die Konfigurierbarkeit der Beendigung geplanter Ereignisse zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="6288a-419">Added `--terminate-notification-time` parameter to `vmss [create|update]` commands to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="6288a-420">Parameter `--enable-terminate-notification` zu den Befehlen `vmss update` hinzugefügt, um die Konfigurierbarkeit der Beendigung geplanter Ereignisse zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="6288a-420">Added `--enable-terminate-notification` parameter to `vmss update` command to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="6288a-421">Parameter `--priority,` `--eviction-policy,` `--max-billing` zu `[vm|vmss] create`-Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-421">Added `--priority,` `--eviction-policy,` `--max-billing` parameters to `[vm|vmss] create` commands</span></span>
* <span data-ttu-id="6288a-422">`disk create` geändert, um die Angabe der genauen Größe des Datenträgeruploads zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="6288a-422">Changed `disk create` to allow specifying the exact size of the disk upload</span></span>
* <span data-ttu-id="6288a-423">Unterstützung für inkrementelle Momentaufnahmen für verwaltete Datenträger zu `snapshot create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-423">Added support for incremental snapshots for managed disks to `snapshot create`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="6288a-424">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="6288a-424">Cosmos DB</span></span>

* <span data-ttu-id="6288a-425">Parameter `--type <key-type>` zum Befehl `cosmosdb keys list` hinzugefügt, um Schlüssel, schreibgeschützte Schlüssel oder Verbindungszeichenfolgen anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="6288a-425">Added `--type <key-type>` parameter to `cosmosdb keys list` command to show key, read only keys or connection strings</span></span>
* <span data-ttu-id="6288a-426">Befehl `cosmosdb keys regenerate` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-426">Added `cosmosdb keys regenerate` command</span></span>
* <span data-ttu-id="6288a-427">[VERALTET] Befehle `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` und `cosmosdb list-read-only-keys` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="6288a-427">[DEPRECATED] Deprecated `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` and `cosmosdb list-read-only-keys` commands</span></span>

### <a name="eventgrid"></a><span data-ttu-id="6288a-428">EventGrid</span><span class="sxs-lookup"><span data-stu-id="6288a-428">EventGrid</span></span>

* <span data-ttu-id="6288a-429">Endpunkthilfetext korrigiert, um auf den richtigen Parameter zu verweisen</span><span class="sxs-lookup"><span data-stu-id="6288a-429">Fixed the endpoint help text to refer to the right parameter</span></span>

### <a name="key-vault"></a><span data-ttu-id="6288a-430">Key Vault</span><span class="sxs-lookup"><span data-stu-id="6288a-430">Key Vault</span></span>

* <span data-ttu-id="6288a-431">Problem behoben, aufgrund dessen die Anmeldung mit einem Mandanten (`login -t`) unter Umständen zu einem Fehler von `keyvault create` führte</span><span class="sxs-lookup"><span data-stu-id="6288a-431">Fixed issue where logging in with a tenant (`login -t`) could cause `keyvault create` to fail</span></span>

### <a name="monitor"></a><span data-ttu-id="6288a-432">Überwachen</span><span class="sxs-lookup"><span data-stu-id="6288a-432">Monitor</span></span>

* <span data-ttu-id="6288a-433">Problem behoben, aufgrund dessen das Zeichen `:` in `--condition` für `monitor metrics alert create` nicht zulässig war</span><span class="sxs-lookup"><span data-stu-id="6288a-433">Fixed issue where `:` character was not allowed in `--condition` argument to `monitor metrics alert create`</span></span>

### <a name="policy"></a><span data-ttu-id="6288a-434">Richtlinie</span><span class="sxs-lookup"><span data-stu-id="6288a-434">Policy</span></span>

* <span data-ttu-id="6288a-435">Unterstützung für Policy-API-Version 2019-06-01 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-435">Added support for Policy API version 2019-06-01</span></span>
* <span data-ttu-id="6288a-436">Parameter `--enforcement-mode` zum Befehl `policy assignment create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-436">Added `--enforcement-mode` parameter to `policy assignment create` command</span></span>

### <a name="storage"></a><span data-ttu-id="6288a-437">Storage</span><span class="sxs-lookup"><span data-stu-id="6288a-437">Storage</span></span>

* <span data-ttu-id="6288a-438">Parameter `--blob-type` zum Befehl `az storage copy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-438">Added `--blob-type` parameter to `az storage copy` command</span></span>

## <a name="september-10-2019"></a><span data-ttu-id="6288a-439">10. September 2019</span><span class="sxs-lookup"><span data-stu-id="6288a-439">September 10, 2019</span></span>

### <a name="acr"></a><span data-ttu-id="6288a-440">ACR</span><span class="sxs-lookup"><span data-stu-id="6288a-440">ACR</span></span>

* <span data-ttu-id="6288a-441">Befehlsgruppe `acr config retention` zum Konfigurieren der Aufbewahrungsrichtlinie hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-441">Added command group `acr config retention` to configure retention policy</span></span>

### <a name="aks"></a><span data-ttu-id="6288a-442">AKS</span><span class="sxs-lookup"><span data-stu-id="6288a-442">AKS</span></span>

* <span data-ttu-id="6288a-443">Unterstützung für die ACR-Integration mit den folgenden Befehlen hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="6288a-443">Added support for ACR integration with the following commands:</span></span>
  * <span data-ttu-id="6288a-444">Parameter `--attach-acr` zu `aks [create|update]` hinzugefügt, um einen ACR an einen AKS-Cluster anzufügen</span><span class="sxs-lookup"><span data-stu-id="6288a-444">Added `--attach-acr` parameter to `aks [create|update]` to attach an ACR to an AKS cluster</span></span>
  * <span data-ttu-id="6288a-445">Parameter `--detach-acr` zu `aks update` hinzugefügt, um den ACR von einem AKS-Cluster zu trennen</span><span class="sxs-lookup"><span data-stu-id="6288a-445">Added `--detach-acr` parameter to `aks update` to detach the ACR from an AKS cluster</span></span>

### <a name="arm"></a><span data-ttu-id="6288a-446">ARM</span><span class="sxs-lookup"><span data-stu-id="6288a-446">ARM</span></span>

* <span data-ttu-id="6288a-447">Zur Verwendung der API-Version 2019-05-10 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="6288a-447">Updated to use API version 2019-05-10</span></span>

### <a name="batch"></a><span data-ttu-id="6288a-448">Batch</span><span class="sxs-lookup"><span data-stu-id="6288a-448">Batch</span></span>

* <span data-ttu-id="6288a-449">Neue JSON-Konfigurationseinstellungen für `batch pool create` zu `--json-file` hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="6288a-449">Added new JSON configuration settings to `--json-file` for `batch pool create`:</span></span>
  * <span data-ttu-id="6288a-450">`MountConfigurations` für Dateisystemeinbindungen hinzugefügt (Details siehe https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body )</span><span class="sxs-lookup"><span data-stu-id="6288a-450">Added `MountConfigurations` for file system mounts (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
  * <span data-ttu-id="6288a-451">Optionale Eigenschaft `publicIPs` in `NetworkConfiguration` für öffentliche IP-Adressen für Pools hinzugefügt (Details siehe https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body )</span><span class="sxs-lookup"><span data-stu-id="6288a-451">Added optional property `publicIPs` on `NetworkConfiguration` for public IPs on pools (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
* <span data-ttu-id="6288a-452">Unterstützung für Kataloge mit freigegebenen Images zu `--image` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-452">Added support for shared image galleries to `--image`</span></span>
* <span data-ttu-id="6288a-453">[BREAKING CHANGE] Standardwert von `--start-task-wait-for-success` für `batch pool create` in `true` geändert</span><span class="sxs-lookup"><span data-stu-id="6288a-453">[BREAKING CHANGE] Changed default value of `--start-task-wait-for-success` on `batch pool create` to be `true`</span></span>
* <span data-ttu-id="6288a-454">[BREAKING CHANGE] Standardwert von `Scope` für `AutoUserSpecification` geändert, damit immer „Pool“ verwendet wird (vormals `Task` für Windows-Knoten bzw. `Pool` für Linux-Knoten)</span><span class="sxs-lookup"><span data-stu-id="6288a-454">[BREAKING CHANGE] Changed default value for `Scope` on `AutoUserSpecification` to always be Pool (was `Task` on Windows nodes, `Pool` on Linux nodes)</span></span>
  * <span data-ttu-id="6288a-455">Dieses Argument kann nur über eine JSON-Konfiguration mit `--json-file` festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="6288a-455">This argument can only be set from a JSON configuration with `--json-file`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="6288a-456">HDInsight</span><span class="sxs-lookup"><span data-stu-id="6288a-456">HDInsight</span></span>

* <span data-ttu-id="6288a-457">Allgemein verfügbares Release</span><span class="sxs-lookup"><span data-stu-id="6288a-457">GA release</span></span>
* <span data-ttu-id="6288a-458">[BREAKING CHANGE] Parameter `--workernode-count/-c` von `az hdinsight resize` in erforderlich geändert</span><span class="sxs-lookup"><span data-stu-id="6288a-458">[BREAKING CHANGE] Changed parameter `--workernode-count/-c` of `az hdinsight resize` to be required.</span></span>

### <a name="key-vault"></a><span data-ttu-id="6288a-459">Key Vault</span><span class="sxs-lookup"><span data-stu-id="6288a-459">Key Vault</span></span>

* <span data-ttu-id="6288a-460">Problem behoben, aufgrund dessen Subnetze nicht aus Netzwerkregeln gelöscht werden konnten</span><span class="sxs-lookup"><span data-stu-id="6288a-460">Fixed issue where subnets couldn't be deleted from network rules</span></span>
* <span data-ttu-id="6288a-461">Problem behoben, aufgrund dessen doppelte Subnetze und IP-Adressen zu Netzwerkregeln hinzugefügt werden konnten</span><span class="sxs-lookup"><span data-stu-id="6288a-461">Fixed issue where duplicated subnets and IP addresses could be added to network rules</span></span>

### <a name="network"></a><span data-ttu-id="6288a-462">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6288a-462">Network</span></span>

* <span data-ttu-id="6288a-463">Parameter `--interval` zu `network watcher flow-log` hinzugefügt, um den Wert für das Intervall der Datenverkehrsanalyse festzulegen</span><span class="sxs-lookup"><span data-stu-id="6288a-463">Added `--interval` parameter to `network watcher flow-log` to set traffic analysis interval value</span></span>
* <span data-ttu-id="6288a-464">`network application-gateway identity` zum Verwalten der Gatewayidentität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-464">Added `network application-gateway identity` to manage gateway identity</span></span>
* <span data-ttu-id="6288a-465">Unterstützung zum Festlegen der Key Vault-ID zu `network application-gateway ssl-cert` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-465">Added support for setting Key Vault ID to `network application-gateway ssl-cert`</span></span>
* <span data-ttu-id="6288a-466">`network express-route peering peer-connection [show|list]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-466">Added `network express-route peering peer-connection [show|list]`</span></span>

### <a name="policy"></a><span data-ttu-id="6288a-467">Richtlinie</span><span class="sxs-lookup"><span data-stu-id="6288a-467">Policy</span></span>

* <span data-ttu-id="6288a-468">Zur Verwendung der API-Version 2019-01-01 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="6288a-468">Updated to use API version 2019-01-01</span></span>

## <a name="august-27-2019"></a><span data-ttu-id="6288a-469">27. August 2019</span><span class="sxs-lookup"><span data-stu-id="6288a-469">August 27, 2019</span></span>

<span data-ttu-id="6288a-470">Version 2.0.72</span><span class="sxs-lookup"><span data-stu-id="6288a-470">Version 2.0.72</span></span>

### <a name="acr"></a><span data-ttu-id="6288a-471">ACR</span><span class="sxs-lookup"><span data-stu-id="6288a-471">ACR</span></span>

* <span data-ttu-id="6288a-472">[BREAKING CHANGE] Unterstützung für SKU `classic` entfernt</span><span class="sxs-lookup"><span data-stu-id="6288a-472">[BREAKING CHANGE] Removed support for the `classic` SKU</span></span>

### <a name="api-management"></a><span data-ttu-id="6288a-473">API Management</span><span class="sxs-lookup"><span data-stu-id="6288a-473">API Management</span></span>

* <span data-ttu-id="6288a-474">[VORSCHAU] Befehlsgruppe `apim` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-474">[PREVIEW] Added `apim` command group</span></span>

### <a name="appservice"></a><span data-ttu-id="6288a-475">AppService</span><span class="sxs-lookup"><span data-stu-id="6288a-475">AppService</span></span>

* <span data-ttu-id="6288a-476">Problem mit dem Befehl `webapp webjob continuous start` bei Angabe eines Slots behoben</span><span class="sxs-lookup"><span data-stu-id="6288a-476">Fixed issue with `webapp webjob continuous start` command when specifying a slot</span></span>
* <span data-ttu-id="6288a-477">`webapp up` geändert, um den Ordner `env` zu erkennen und aus der für die Bereitstellung verwendeten Datei zu entfernen</span><span class="sxs-lookup"><span data-stu-id="6288a-477">Changed `webapp up` to detect `env` folder and remove it from the file used for deployment</span></span>

### <a name="keyvault"></a><span data-ttu-id="6288a-478">KeyVault</span><span class="sxs-lookup"><span data-stu-id="6288a-478">Keyvault</span></span>

* <span data-ttu-id="6288a-479">Fehler in `keyvault secret set` behoben, aufgrund dessen das Argument `--expires` ignoriert wurde</span><span class="sxs-lookup"><span data-stu-id="6288a-479">Fixed a bug in `keyvault secret set` that igored the `--expires` argument</span></span>

### <a name="network"></a><span data-ttu-id="6288a-480">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6288a-480">Network</span></span>

* <span data-ttu-id="6288a-481">Unterstützung für IPv6-Adressen zu Argumenten vom Typ `--private-ip-address-version` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-481">Added support for IPv6 addresses to `--private-ip-address-version` arguments</span></span>
* <span data-ttu-id="6288a-482">Neue Befehle vom Typ `network private-endpoint [create|update|list-types]` für die Verwaltung privater Endpunkte hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-482">Added new commands `network private-endpoint [create|update|list-types]` for private endpoint management</span></span>
* <span data-ttu-id="6288a-483">Befehlsgruppe `network private-link-service` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-483">Added command group `network private-link-service`</span></span>
* <span data-ttu-id="6288a-484">Argumente `--private-endpoint-network-policies` und `--private-link-service-network-policies` zu `network vnet subnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-484">Added `--private-endpoint-network-policies` and `--private-link-service-network-policies` arguments to `network vnet subnet update`</span></span>

### <a name="rbac"></a><span data-ttu-id="6288a-485">RBAC</span><span class="sxs-lookup"><span data-stu-id="6288a-485">RBAC</span></span>

* <span data-ttu-id="6288a-486">Problem mit `ad app update --homepage` behoben, aufgrund dessen die Startseite nicht aktualisiert wurde</span><span class="sxs-lookup"><span data-stu-id="6288a-486">Fixed issue with `ad app update --homepage` where homepage would not be updated</span></span>

### <a name="servicefabric"></a><span data-ttu-id="6288a-487">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="6288a-487">ServiceFabric</span></span>

* <span data-ttu-id="6288a-488">Unterstützung für Key Vault-Namen mit Groß- und Kleinschreibung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-488">Added support for mixed-case Key Vault names</span></span>
* <span data-ttu-id="6288a-489">Problem bei der Verwendung von Zertifikaten in Key Vault behoben</span><span class="sxs-lookup"><span data-stu-id="6288a-489">Fixed issue when using certificates in Key Vault</span></span>
* <span data-ttu-id="6288a-490">Problem bei der Verwendung von PFX-Zertifikatdateien behoben</span><span class="sxs-lookup"><span data-stu-id="6288a-490">Fixed issue with using PFX certificate files</span></span>
* <span data-ttu-id="6288a-491">Problem mit `sf cluster certificate add` behoben, wenn keine Key Vault-Ressourcengruppe angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="6288a-491">Fixed issue with `sf cluster certificate add` when Key Vault resource group wasn't specified</span></span>
* <span data-ttu-id="6288a-492">Problem behoben, aufgrund dessen `sf cluster set` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="6288a-492">Fixed issue with `sf cluster set` not working</span></span>

### <a name="signalr"></a><span data-ttu-id="6288a-493">SignalR</span><span class="sxs-lookup"><span data-stu-id="6288a-493">SignalR</span></span>

* <span data-ttu-id="6288a-494">Neue Befehle hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="6288a-494">Added new commands:</span></span>
  * <span data-ttu-id="6288a-495">`signalr cors`: Verwalten von CORS für SignalR</span><span class="sxs-lookup"><span data-stu-id="6288a-495">`signalr cors`: Manage SignalR CORS</span></span>
  * <span data-ttu-id="6288a-496">`signalr restart`: Starten eines SignalR-Diensts</span><span class="sxs-lookup"><span data-stu-id="6288a-496">`signalr restart`: Restart a SignalR service</span></span>
  * <span data-ttu-id="6288a-497">`signalr update`: Aktualisieren eines SignalR-Diensts</span><span class="sxs-lookup"><span data-stu-id="6288a-497">`signalr update`: Update a SignalR service</span></span>
* <span data-ttu-id="6288a-498">Argument `--service-mode` zu `signalr create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-498">Added `--service-mode` argument to `signalr create`</span></span>

### <a name="storage"></a><span data-ttu-id="6288a-499">Storage</span><span class="sxs-lookup"><span data-stu-id="6288a-499">Storage</span></span>

* <span data-ttu-id="6288a-500">Befehl `storage account revoke-delegation-keys` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-500">Added `storage account revoke-delegation-keys` command</span></span>

## <a name="august-13-2019"></a><span data-ttu-id="6288a-501">13. August 2019</span><span class="sxs-lookup"><span data-stu-id="6288a-501">August 13, 2019</span></span>

<span data-ttu-id="6288a-502">Version 2.0.71</span><span class="sxs-lookup"><span data-stu-id="6288a-502">Version 2.0.71</span></span>

### <a name="appservice"></a><span data-ttu-id="6288a-503">AppService</span><span class="sxs-lookup"><span data-stu-id="6288a-503">AppService</span></span>

* <span data-ttu-id="6288a-504">Problem behoben, aufgrund dessen bei Befehlen vom Typ `webapp webjob continuous` für Slots Fehler auftraten</span><span class="sxs-lookup"><span data-stu-id="6288a-504">Fixed issue where `webapp webjob continuous` commands were failing for slots</span></span>

### <a name="botservice"></a><span data-ttu-id="6288a-505">BotService</span><span class="sxs-lookup"><span data-stu-id="6288a-505">BotService</span></span>

* <span data-ttu-id="6288a-506">[BREAKING CHANGE] Unterstützung für die Erstellung von Bots der Version 3 entfernt</span><span class="sxs-lookup"><span data-stu-id="6288a-506">[BREAKING CHANGE] Removed support for creating v3 SDK bots</span></span>

### <a name="cognitiveservices"></a><span data-ttu-id="6288a-507">CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="6288a-507">CognitiveServices</span></span>

* <span data-ttu-id="6288a-508">Befehle vom Typ `cognitiveservices account network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-508">Added `cognitiveservices account network-rule` commands</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="6288a-509">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="6288a-509">Cosmos DB</span></span>

* <span data-ttu-id="6288a-510">Beim Aktualisieren mehrerer Schreibstandorte wurde eine Warnung entfernt.</span><span class="sxs-lookup"><span data-stu-id="6288a-510">Removed warning when updating multiple write locations</span></span>
* <span data-ttu-id="6288a-511">CRUD-Befehle für CosmosDB SQL-, MongoDB-, Cassandra-, Gremlin- und Tabellenressourcen sowie den Ressourcendurchsatz hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-511">Added CRUD commands for CosmosDB SQL, MongoDB, Cassandra, Gremlin and Table resources and resource's throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="6288a-512">HDInsight</span><span class="sxs-lookup"><span data-stu-id="6288a-512">HDInsight</span></span>

<span data-ttu-id="6288a-513">Dieses Release enthält zahlreiche wichtige Änderungen.</span><span class="sxs-lookup"><span data-stu-id="6288a-513">This release contains a large number of breaking changes.</span></span>

* <span data-ttu-id="6288a-514">[BREAKING CHANGE] Parameter für `hdinsight create` umbenannt:</span><span class="sxs-lookup"><span data-stu-id="6288a-514">[BREAKING CHANGE] Renamed parameters for `hdinsight create`:</span></span>
  * <span data-ttu-id="6288a-515">`--storage-default-container` in `--storage-container` umbenannt</span><span class="sxs-lookup"><span data-stu-id="6288a-515">Renamed `--storage-default-container` to `--storage-container`</span></span>
  * <span data-ttu-id="6288a-516">`--storage-default-filesystem` in `--storage-filesystem` umbenannt</span><span class="sxs-lookup"><span data-stu-id="6288a-516">Renamed `--storage-default-filesystem` to `--storage-filesystem`</span></span>
* <span data-ttu-id="6288a-517">[BREAKING CHANGE] Das Argument `--name` von `application create` wurde so geändert, dass es den Anwendungsnamen anstelle des Clusternamens darstellt.</span><span class="sxs-lookup"><span data-stu-id="6288a-517">[BREAKING CHANGE] Changed the `--name` argument of `application create` to represent the application name instead of the cluster name</span></span>
* <span data-ttu-id="6288a-518">Argument `--cluster-name` zu `application create` hinzugefügt, um die alte Funktion `--name` zu ersetzen</span><span class="sxs-lookup"><span data-stu-id="6288a-518">Added `--cluster-name` argument to `application create` to replace old `--name` functionality</span></span>
* <span data-ttu-id="6288a-519">[BREAKING CHANGE] Parameter für `application create` umbenannt:</span><span class="sxs-lookup"><span data-stu-id="6288a-519">[BREAKING CHANGE] Renamed parameters for `application create`:</span></span>
  * <span data-ttu-id="6288a-520">`--application-type` in `--type` umbenannt</span><span class="sxs-lookup"><span data-stu-id="6288a-520">Renamed `--application-type` to `--type`</span></span>
  * <span data-ttu-id="6288a-521">`--marketplace-identifier` in `--marketplace-id` umbenannt</span><span class="sxs-lookup"><span data-stu-id="6288a-521">Renamed `--marketplace-identifier` to `--marketplace-id`</span></span>
  * <span data-ttu-id="6288a-522">`--https-endpoint-access-mode` in `--access-mode` umbenannt</span><span class="sxs-lookup"><span data-stu-id="6288a-522">Renamed `--https-endpoint-access-mode` to `--access-mode`</span></span>
  * <span data-ttu-id="6288a-523">`--https-endpoint-destination-port` in `--destination-port` umbenannt</span><span class="sxs-lookup"><span data-stu-id="6288a-523">Renamed  `--https-endpoint-destination-port` to `--destination-port`</span></span>
* <span data-ttu-id="6288a-524">[BREAKING CHANGE] Parameter für `application create` entfernt:</span><span class="sxs-lookup"><span data-stu-id="6288a-524">[BREAKING CHANGE] Removed parameters for `application create`:</span></span>
  * `--https-endpoint-location`
  * `--https-endpoint-public-port`
  * `--ssh-endpoint-destination-port`
  * `--ssh-endpoint-location`
  * `--ssh-endpoint-public-port`
* <span data-ttu-id="6288a-525">[WICHTIGE ÄNDERUNG] `--target-instance-count` für `hdinsight resize` in `--workernode-count` umbenannt</span><span class="sxs-lookup"><span data-stu-id="6288a-525">[BREAKING CHNAGE] Renamed `--target-instance-count` to `--workernode-count` for `hdinsight resize`</span></span>
* <span data-ttu-id="6288a-526">[BREAKING CHANGE] Alle Befehle in der Gruppe `hdinsight script-action` wurden so geändert, dass sie den Parameter `--name` als Namen der Skriptaktion verwenden.</span><span class="sxs-lookup"><span data-stu-id="6288a-526">[BREAKING CHANGE] Changed all commands in the `hdinsight script-action` group to use the `--name` parameter as the name of the script action.</span></span>
* <span data-ttu-id="6288a-527">Argument `--cluster-name` zu allen Befehlen vom Typ `hdinsight script-action` hinzugefügt, um die alte Funktion `--name` zu ersetzen</span><span class="sxs-lookup"><span data-stu-id="6288a-527">Added `--cluster-name` argument to all `hdinsight script-action` commands to replace old `--name` functionality</span></span>
* <span data-ttu-id="6288a-528">[BREAKING CHANGE]`--script-execution-id` für alle Befehle vom Typ `hdinsight script-action` in `--execution-id` umbenannt</span><span class="sxs-lookup"><span data-stu-id="6288a-528">[BREAKING CHANGE] Renamed `--script-execution-id` to `--execution-id` for all `hdinsight script-action` commands</span></span>
* <span data-ttu-id="6288a-529">[BREAKING CHANGE]`hdinsight script-action show` in `hdinsight script-action show-execution-details` umbenannt</span><span class="sxs-lookup"><span data-stu-id="6288a-529">[BREAKING CHANGE] Renamed `hdinsight script-action show` to `hdinsight script-action show-execution-details`</span></span>
* <span data-ttu-id="6288a-530">[WICHTIGE ÄNDERUNG] Parameter in `hdinsight script-action execute --roles` geändert, sodass sie durch Leerzeichen anstelle von Kommas getrennt sind</span><span class="sxs-lookup"><span data-stu-id="6288a-530">[BREAKING CHNAGE] Changed parameters to `hdinsight script-action execute --roles` to be space-separated instead of comma-separated</span></span>
* <span data-ttu-id="6288a-531">[BREAKING CHANGE] Parameter `--persisted` für `hdinsight script-action list` entfernt</span><span class="sxs-lookup"><span data-stu-id="6288a-531">[BREAKING CHANGE] Removed the `--persisted` parameter of `hdinsight script-action list`</span></span>
* <span data-ttu-id="6288a-532">Der Parameter `hdinsight create --cluster-configurations` wurde so geändert, dass er einen Pfad zu einer lokalen JSON-Datei oder JSON-Zeichenfolge akzeptiert.</span><span class="sxs-lookup"><span data-stu-id="6288a-532">Changed the `hdinsight create --cluster-configurations` parameter to accept a path to a local JSON file or a JSON string</span></span>
* <span data-ttu-id="6288a-533">Befehl `hdinsight script-action list-execution-history` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-533">Added command `hdinsight script-action list-execution-history`</span></span>
* <span data-ttu-id="6288a-534">`hdinsight monitor enable --workspace` geändert, um die ID oder den Namen eines Log Analytics-Arbeitsbereichs zu akzeptieren</span><span class="sxs-lookup"><span data-stu-id="6288a-534">Changed `hdinsight monitor enable --workspace` to accept a Log Analytics workspace ID or workspace name</span></span>
* <span data-ttu-id="6288a-535">Argument `hdinsight monitor enable --primary-key` hinzugefügt. Dieses Argument wird benötigt, wenn eine Arbeitsbereichs-ID als Parameter angegeben wird.</span><span class="sxs-lookup"><span data-stu-id="6288a-535">Added the `hdinsight monitor enable --primary-key` argument, which is needed if a workspace ID is provided as the parameter</span></span>
* <span data-ttu-id="6288a-536">Weitere Beispiele und aktualisierte Beschreibungen für Hilfemeldungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-536">Added more examples and updated descriptions for help messages</span></span>

### <a name="interactive"></a><span data-ttu-id="6288a-537">Interactive</span><span class="sxs-lookup"><span data-stu-id="6288a-537">Interactive</span></span>

* <span data-ttu-id="6288a-538">Ladefehler behoben</span><span class="sxs-lookup"><span data-stu-id="6288a-538">Fixed a loading error</span></span>

### <a name="kubernetes"></a><span data-ttu-id="6288a-539">Kubernetes</span><span class="sxs-lookup"><span data-stu-id="6288a-539">Kubernetes</span></span>

* <span data-ttu-id="6288a-540">Änderung, um `https` zu verwenden, wenn der Dashboardcontainerport `https` verwendet</span><span class="sxs-lookup"><span data-stu-id="6288a-540">Changed to use `https` if dashboard container port is using `https`</span></span>

### <a name="network"></a><span data-ttu-id="6288a-541">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6288a-541">Network</span></span>

* <span data-ttu-id="6288a-542">Argument `--yes` hinzugefügt zu `network dns record-set cname delete`</span><span class="sxs-lookup"><span data-stu-id="6288a-542">Added `--yes` argument `network dns record-set cname delete`</span></span>

### <a name="profile"></a><span data-ttu-id="6288a-543">Profil</span><span class="sxs-lookup"><span data-stu-id="6288a-543">Profile</span></span>

* <span data-ttu-id="6288a-544">Argument `--resource-type` zu `account get-access-token` zum Abrufen von Ressourcenzugriffstoken hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-544">Added `--resource-type` argument to `account get-access-token` to get resource access tokens</span></span>

### <a name="servicefabric"></a><span data-ttu-id="6288a-545">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="6288a-545">ServiceFabric</span></span>

* <span data-ttu-id="6288a-546">Alle unterstützten Betriebssystemversionen für „sf cluster create“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-546">Added all supported os version for sf cluster create</span></span>
* <span data-ttu-id="6288a-547">Fehler beim Überprüfen des primären Zertifikats behoben</span><span class="sxs-lookup"><span data-stu-id="6288a-547">Fixed primary certificate validation bug</span></span>

### <a name="storage"></a><span data-ttu-id="6288a-548">Storage</span><span class="sxs-lookup"><span data-stu-id="6288a-548">Storage</span></span>

* <span data-ttu-id="6288a-549">Befehl `storage copy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-549">Added command `storage copy`</span></span>

## <a name="july-30-2019"></a><span data-ttu-id="6288a-550">30. Juli 2019</span><span class="sxs-lookup"><span data-stu-id="6288a-550">July 30, 2019</span></span>

<span data-ttu-id="6288a-551">Version 2.0.70</span><span class="sxs-lookup"><span data-stu-id="6288a-551">Version 2.0.70</span></span>

### <a name="acr"></a><span data-ttu-id="6288a-552">ACR</span><span class="sxs-lookup"><span data-stu-id="6288a-552">ACR</span></span>

* <span data-ttu-id="6288a-553">Problem #9952 behoben (Regression im Befehl `acr pack build`)</span><span class="sxs-lookup"><span data-stu-id="6288a-553">Fixed issue #9952 (a regression in the `acr pack build` command)</span></span>
* <span data-ttu-id="6288a-554">Standardname des Generatorimages in `acr pack build` entfernt</span><span class="sxs-lookup"><span data-stu-id="6288a-554">Removed the default builder image name in `acr pack build`</span></span>

### <a name="appservice"></a><span data-ttu-id="6288a-555">AppService</span><span class="sxs-lookup"><span data-stu-id="6288a-555">Appservice</span></span>

* <span data-ttu-id="6288a-556">`webapp config ssl` geändert, um eine Meldung anzuzeigen, wenn eine Ressource nicht gefunden wurde</span><span class="sxs-lookup"><span data-stu-id="6288a-556">Changed `webapp config ssl` to show a message if a resource is not found</span></span>
* <span data-ttu-id="6288a-557">Problem behoben, aufgrund dessen `functionapp create` den Speicherkontotypen `Standard_RAGRS` nicht akzeptiert hat</span><span class="sxs-lookup"><span data-stu-id="6288a-557">Fixed issue where `functionapp create` does not accept `Standard_RAGRS` storage account type</span></span>
* <span data-ttu-id="6288a-558">Problem behoben, aufgrund dessen für `webapp up` ein Fehler auftrat, wenn für die Ausführung ältere Python-Versionen verwendet wurden</span><span class="sxs-lookup"><span data-stu-id="6288a-558">Fixed an issue where `webapp up` would fail if run using older versions of python</span></span>

### <a name="network"></a><span data-ttu-id="6288a-559">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6288a-559">Network</span></span>

* <span data-ttu-id="6288a-560">Ungültiger Parameter `--ids` aus `network nic ip-config add` entfernt (Fehlerbehebungen #9861)</span><span class="sxs-lookup"><span data-stu-id="6288a-560">Removed invalid parameter `--ids` from `network nic ip-config add` (fixes #9861)</span></span>
* <span data-ttu-id="6288a-561">Fehlerbehebungen #9604.</span><span class="sxs-lookup"><span data-stu-id="6288a-561">Fixes #9604.</span></span> <span data-ttu-id="6288a-562">Parameter `--root-certs` zu `network application-gateway http-settings [create|update]` hinzugefügt, um vom Benutzer zugewiesene vertrauenswürdige Stammzertifikate zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="6288a-562">Added `--root-certs` parameter to `network application-gateway http-settings [create|update]` to support user associate trusted root certificates.</span></span>
* <span data-ttu-id="6288a-563">Argument `--subscription` für `network dns record-set ns create` korrigiert (#9965)</span><span class="sxs-lookup"><span data-stu-id="6288a-563">Fixed arguent `--subscription` for `network dns record-set ns create` (#9965)</span></span>

### <a name="rbac"></a><span data-ttu-id="6288a-564">RBAC</span><span class="sxs-lookup"><span data-stu-id="6288a-564">RBAC</span></span>

* <span data-ttu-id="6288a-565">Befehl `user update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-565">Added `user update` command</span></span>
* <span data-ttu-id="6288a-566">[VERALTET]`--upn-or-object-id` in benutzerbezogenen Befehlen als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="6288a-566">[DEPRECATED] Deprecated `--upn-or-object-id` from user-related commands</span></span>
    * <span data-ttu-id="6288a-567">Verwenden Sie das Ersatzargument `--id`.</span><span class="sxs-lookup"><span data-stu-id="6288a-567">Use replacement argument `--id`</span></span>
* <span data-ttu-id="6288a-568">Argument `--id` zu benutzerbezogenen Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-568">Added `--id` argument to user-related commands</span></span>

### <a name="sql"></a><span data-ttu-id="6288a-569">SQL</span><span class="sxs-lookup"><span data-stu-id="6288a-569">SQL</span></span>

* <span data-ttu-id="6288a-570">Verwaltungsbefehle für Schlüssel verwalteter Instanzen und TDE-Schutzvorrichtung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-570">Added management commands for managed instance keys and TDE protector</span></span>

### <a name="storage"></a><span data-ttu-id="6288a-571">Storage</span><span class="sxs-lookup"><span data-stu-id="6288a-571">Storage</span></span>

* <span data-ttu-id="6288a-572">Befehl `storage remove` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-572">Added `storage remove` command</span></span>
* <span data-ttu-id="6288a-573">Problem mit `storage blob update` behoben</span><span class="sxs-lookup"><span data-stu-id="6288a-573">Fixed an issue with `storage blob update`</span></span>

### <a name="vm"></a><span data-ttu-id="6288a-574">VM</span><span class="sxs-lookup"><span data-stu-id="6288a-574">VM</span></span>

* <span data-ttu-id="6288a-575">`list-skus` wurde geändert, um eine neuere API-Version für die Ausgabe von Zonendetails zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="6288a-575">Changed `list-skus` to use newer api-version to output zone details</span></span>
* <span data-ttu-id="6288a-576">Standardwert `--single-placement-group` für `vmss create` in `false` geändert</span><span class="sxs-lookup"><span data-stu-id="6288a-576">Changed default of `--single-placement-group` to `false` for `vmss create`</span></span>
* <span data-ttu-id="6288a-577">Möglichkeit zum Auswählen von ZRS-Speicher-SKUs für `[snapshot|disk] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-577">Added ability to select ZRS storage SKUs for `[snapshot|disk] create`</span></span>
* <span data-ttu-id="6288a-578">Neue Befehlsgruppe `vm host` zur Unterstützung dedizierter Hosts hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-578">Added new command group `vm host` to support dedicated hosts</span></span>
* <span data-ttu-id="6288a-579">Parameter `--host` und `--host-group` für `vm create` hinzugefügt, um den dedizierten VM-Host festzulegen</span><span class="sxs-lookup"><span data-stu-id="6288a-579">Added parameters `--host` and `--host-group` on `vm create` to set VM dedicated host</span></span>

## <a name="july-16-2019"></a><span data-ttu-id="6288a-580">16. Juli 2019</span><span class="sxs-lookup"><span data-stu-id="6288a-580">July 16, 2019</span></span>

<span data-ttu-id="6288a-581">Version 2.0.69</span><span class="sxs-lookup"><span data-stu-id="6288a-581">Version 2.0.69</span></span>

### <a name="appservice"></a><span data-ttu-id="6288a-582">AppService</span><span class="sxs-lookup"><span data-stu-id="6288a-582">Appservice</span></span>

* <span data-ttu-id="6288a-583">`webapp identity`-Befehle geändert, um eine korrekte Fehlermeldung zurückzugeben, wenn „ResourceGroupName“ oder der App-Name ungültig sind</span><span class="sxs-lookup"><span data-stu-id="6288a-583">Changed `webapp identity` commands to return a proper error message if ResourceGroupName or App name are invalid</span></span>
* <span data-ttu-id="6288a-584">`webapp list` korrigiert, sodass der korrekte Wert für „numberOfSites“ zurückgegeben wird, wenn „ResourceGroup“ nicht angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="6288a-584">Fixed `webapp list` to return the correct value for numberOfSites if no ResourceGroup was provided</span></span>
* <span data-ttu-id="6288a-585">Nebeneffekte von `appservice plan create` und `webapp create` behoben</span><span class="sxs-lookup"><span data-stu-id="6288a-585">Fixed side-effects of `appservice plan create` and `webapp create`</span></span>

### <a name="core"></a><span data-ttu-id="6288a-586">Core</span><span class="sxs-lookup"><span data-stu-id="6288a-586">Core</span></span>

* <span data-ttu-id="6288a-587">Problem behoben, aufgrund dessen `--subscription` angezeigt wurde, obwohl nicht anwendbar</span><span class="sxs-lookup"><span data-stu-id="6288a-587">Fixed issue where `--subscription` would appear despite being not applicable</span></span>

### <a name="batch"></a><span data-ttu-id="6288a-588">Batch</span><span class="sxs-lookup"><span data-stu-id="6288a-588">Batch</span></span>

* <span data-ttu-id="6288a-589">[BREAKING CHANGE]`batch pool node-agent-skus list` durch `batch pool supported-images list` ersetzt</span><span class="sxs-lookup"><span data-stu-id="6288a-589">[BREAKING CHANGE] Replaced `batch pool node-agent-skus list` with `batch pool supported-images list`</span></span>
* <span data-ttu-id="6288a-590">Unterstützung für Sicherheitsregeln hinzugefügt, die den Netzwerkzugriff auf einen Pool basierend auf dem Quellport des Datenverkehrs blockieren, wenn die Option `--json-file` von `batch pool create network` verwendet wird</span><span class="sxs-lookup"><span data-stu-id="6288a-590">Added support for security rules blocking network access to a pool based on the source port of the traffic when using the `--json-file` option of `batch pool create network`</span></span>
* <span data-ttu-id="6288a-591">Unterstützung für die Ausführung der Aufgabe im Arbeitsverzeichnis des Containers oder der Batch-Aufgabe hinzugefügt, wenn die Option `--json-file` von `batch task create` verwendet wird</span><span class="sxs-lookup"><span data-stu-id="6288a-591">Added support for executing the task in the container working directory or in the Batch task working directory when using the `--json-file` option of `batch task create`</span></span>
* <span data-ttu-id="6288a-592">Fehler in Option `--application-package-references` von `batch pool create` behoben, aufgrund dessen nur Standardeinstellungen möglich waren</span><span class="sxs-lookup"><span data-stu-id="6288a-592">Fixed error in `--application-package-references` option of `batch pool create` where it would only work with defaults</span></span>

### <a name="eventhubs"></a><span data-ttu-id="6288a-593">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="6288a-593">Eventhubs</span></span>

* <span data-ttu-id="6288a-594">Validierung für Parameter `--rights` von `authorizationrule`-Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-594">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="rdbms"></a><span data-ttu-id="6288a-595">RDBMS</span><span class="sxs-lookup"><span data-stu-id="6288a-595">RDBMS</span></span>

* <span data-ttu-id="6288a-596">Optionaler Parameter zum Angeben der Replikat-SKU für den Befehl zum Erstellen von Replikaten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-596">Added optional parameter to specify replica SKU for create replica command</span></span>
* <span data-ttu-id="6288a-597">Problem mit CI-Testfehler bei der Erstellung von MySQL-Replikaten behoben</span><span class="sxs-lookup"><span data-stu-id="6288a-597">Fixed the issue with CI test failure with creating MySQL replica</span></span>

### <a name="relay"></a><span data-ttu-id="6288a-598">Relay</span><span class="sxs-lookup"><span data-stu-id="6288a-598">Relay</span></span>

* <span data-ttu-id="6288a-599">Problem mit Hybridverbindung behoben, wenn die Client-Autorisierung deaktiviert ist [#8775](https://github.com/azure/azure-cli/issues/8775)</span><span class="sxs-lookup"><span data-stu-id="6288a-599">Fixed issue with hybrid connection when client authroization disabled [#8775](https://github.com/azure/azure-cli/issues/8775)</span></span>
* <span data-ttu-id="6288a-600">Parameter `--requires-transport-security` zu `relay wcfrelay create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-600">Added parameter `--requires-transport-security` to `relay wcfrelay create`</span></span>

### <a name="servicebus"></a><span data-ttu-id="6288a-601">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="6288a-601">Servicebus</span></span>

* <span data-ttu-id="6288a-602">Validierung für Parameter `--rights` von `authorizationrule`-Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-602">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="storage"></a><span data-ttu-id="6288a-603">Storage</span><span class="sxs-lookup"><span data-stu-id="6288a-603">Storage</span></span>

* <span data-ttu-id="6288a-604">AADDS für Files für Speicherkontoaktualisierung aktiviert</span><span class="sxs-lookup"><span data-stu-id="6288a-604">Enable Files AADDS for storage account update</span></span>
* <span data-ttu-id="6288a-605">Problem `storage blob service-properties update --set` behoben</span><span class="sxs-lookup"><span data-stu-id="6288a-605">Fixed issue `storage blob service-properties update --set`</span></span>

## <a name="july-2-2019"></a><span data-ttu-id="6288a-606">2\. Juli 2019</span><span class="sxs-lookup"><span data-stu-id="6288a-606">July 2, 2019</span></span>

<span data-ttu-id="6288a-607">Version 2.0.68</span><span class="sxs-lookup"><span data-stu-id="6288a-607">Version 2.0.68</span></span>

### <a name="core"></a><span data-ttu-id="6288a-608">Core</span><span class="sxs-lookup"><span data-stu-id="6288a-608">Core</span></span>

* <span data-ttu-id="6288a-609">Befehlsmodule sind jetzt in einer einzelnen verteilbaren Python-Komponente zusammengefasst.</span><span class="sxs-lookup"><span data-stu-id="6288a-609">Command modules are now consolidated into a single Python distributable.</span></span> <span data-ttu-id="6288a-610">Die direkte Verwendung zahlreicher Pakete vom Typ `azure-cli-` in PyPI ist daher veraltet.</span><span class="sxs-lookup"><span data-stu-id="6288a-610">This deprecates direct use of many `azure-cli-` packages on PyPI.</span></span>
  <span data-ttu-id="6288a-611">Dadurch sollte sich die Installationsgröße reduzieren. Darüber hinaus sollte es nur Benutzer betreffen, die eine direkte Installation über `pip` ausgeführt haben.</span><span class="sxs-lookup"><span data-stu-id="6288a-611">This should reduce install size and only affect users who have directly installed via `pip`.</span></span>

### <a name="acr"></a><span data-ttu-id="6288a-612">ACR</span><span class="sxs-lookup"><span data-stu-id="6288a-612">ACR</span></span>

* <span data-ttu-id="6288a-613">Unterstützung für Trigger mit Timer zu Aufgabe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-613">Added support for Timer Triggers to Task</span></span>

### <a name="appservice"></a><span data-ttu-id="6288a-614">AppService</span><span class="sxs-lookup"><span data-stu-id="6288a-614">Appservice</span></span>

* <span data-ttu-id="6288a-615">`functionapp create` wurde so geändert, das Application Insights standardmäßig aktiviert wird.</span><span class="sxs-lookup"><span data-stu-id="6288a-615">Changed `functionapp create` to enable application insights by default</span></span>
* <span data-ttu-id="6288a-616">[BREAKING CHANGE] Veralteter Befehl `functionapp devops-build` entfernt.</span><span class="sxs-lookup"><span data-stu-id="6288a-616">[BREAKING CHANGE] Removed deprecated `functionapp devops-build` command.</span></span>
  *  <span data-ttu-id="6288a-617">Verwenden Sie stattdessen den neuen Befehl `az functionapp devops-pipeline`.</span><span class="sxs-lookup"><span data-stu-id="6288a-617">Use the new command `az functionapp devops-pipeline` instead</span></span>
* <span data-ttu-id="6288a-618">Unterstützung des Funktions-App-Plans für Linux-Verbrauch zu `functionapp deployment config-zip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-618">Added Linux Consumption function app plan support to `functionapp deployment config-zip`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="6288a-619">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="6288a-619">Cosmos DB</span></span>

* <span data-ttu-id="6288a-620">Unterstützung für das Deaktivieren von TTL hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-620">Added support for disabling TTL</span></span>

### <a name="dls"></a><span data-ttu-id="6288a-621">DLS</span><span class="sxs-lookup"><span data-stu-id="6288a-621">DLS</span></span>

* <span data-ttu-id="6288a-622">Aktualisierte ADLS-Version (0.0.45)</span><span class="sxs-lookup"><span data-stu-id="6288a-622">Updated ADLS version (0.0.45)</span></span>

### <a name="feedback"></a><span data-ttu-id="6288a-623">Feedback</span><span class="sxs-lookup"><span data-stu-id="6288a-623">Feedback</span></span>

* <span data-ttu-id="6288a-624">Wird ein fehlgeschlagener Erweiterungsbefehl gemeldet, versucht `az feedback` nun, über den Index die Projekt-/Repository-URL der Erweiterung im Browser zu öffnen.</span><span class="sxs-lookup"><span data-stu-id="6288a-624">When reporting a failed extension command, `az feedback` now attempts to open the browser to the project/repo url of the extension from the index</span></span>

### <a name="hdinsight"></a><span data-ttu-id="6288a-625">HDInsight</span><span class="sxs-lookup"><span data-stu-id="6288a-625">HDInsight</span></span>

* <span data-ttu-id="6288a-626">[BREAKING CHANGE] Der Befehlsgruppenname `oms` wurde in `monitor` geändert.</span><span class="sxs-lookup"><span data-stu-id="6288a-626">[BREAKING CHANGE] Changed `oms` command group name to `monitor`</span></span>
* <span data-ttu-id="6288a-627">[BREAKING CHANGE]`--http-password/-p` als erforderlicher Parameter festgelegt</span><span class="sxs-lookup"><span data-stu-id="6288a-627">[BREAKING CHANGE] Made `--http-password/-p` a required parameter</span></span> 
* <span data-ttu-id="6288a-628">Vervollständigungen für `--cluster-admin-account` und `cluster-users-group-dns` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-628">Added completers for `--cluster-admin-account` and `cluster-users-group-dns` parameters completer</span></span> 
* <span data-ttu-id="6288a-629">Parameter `cluster-users-group-dns` so geändert, dass er erforderlich ist, wenn `—esp` vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="6288a-629">Changed `cluster-users-group-dns` parameter to be required when `—esp` is present</span></span>
* <span data-ttu-id="6288a-630">Timeout für alle vorhandenen automatischen Argumentvervollständigungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-630">Added a timeout for all existing argument auto-completers</span></span>
* <span data-ttu-id="6288a-631">Timeout für das Transformieren des Ressourcennamens in eine Ressourcen-ID hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-631">Added a timeout for transforming resource name to resource id</span></span>
* <span data-ttu-id="6288a-632">Die automatischen Vervollständigungen wurden so geändert, dass Ressourcen aus einer beliebigen Ressourcengruppe ausgewählt werden.</span><span class="sxs-lookup"><span data-stu-id="6288a-632">Changed Auto-completers to select resources from any resource group.</span></span> <span data-ttu-id="6288a-633">Dabei kann es sich um eine andere Ressourcengruppe als die mit `-g` angegebene Gruppe handeln.</span><span class="sxs-lookup"><span data-stu-id="6288a-633">It can be a different resource group than the one specified with `-g`</span></span>
* <span data-ttu-id="6288a-634">Unterstützung für die Parameter `--sub-domain-suffix` und `--disable_gateway_auth` im Befehl `hdinsight application create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-634">Added support for `--sub-domain-suffix` and `--disable_gateway_auth` parameters in the `hdinsight application create` command</span></span>

### <a name="managed-services"></a><span data-ttu-id="6288a-635">Verwaltete Dienste</span><span class="sxs-lookup"><span data-stu-id="6288a-635">Managed Services</span></span>

* <span data-ttu-id="6288a-636">Befehlsmodul für verwaltete Dienste als Vorschau eingeführt</span><span class="sxs-lookup"><span data-stu-id="6288a-636">Introducing managed service command module in preview</span></span>

### <a name="profile"></a><span data-ttu-id="6288a-637">Profil</span><span class="sxs-lookup"><span data-stu-id="6288a-637">Profile</span></span>
* <span data-ttu-id="6288a-638">Argument `--subscription` für Abmeldebefehl unterdrückt</span><span class="sxs-lookup"><span data-stu-id="6288a-638">Suppress `--subscription` argument for logout command</span></span>

### <a name="rbac"></a><span data-ttu-id="6288a-639">RBAC</span><span class="sxs-lookup"><span data-stu-id="6288a-639">RBAC</span></span>

* <span data-ttu-id="6288a-640">[BREAKING CHANGE] Argument `--password` für `create-for-rbac` entfernt</span><span class="sxs-lookup"><span data-stu-id="6288a-640">[BREAKING CHANGE] Removed `--password` argument for `create-for-rbac`</span></span>
* <span data-ttu-id="6288a-641">Parameter `--assignee-principal-type` zum Befehl `create` hinzugefügt, um zeitweilige Fehler zu vermeiden, die durch die Replikationswartezeit des AAD-Graph-Servers verursacht werden</span><span class="sxs-lookup"><span data-stu-id="6288a-641">Added `--assignee-principal-type` parameter to `create` command to avoid intermittent failures caused by AAD graph server replication latency</span></span>
* <span data-ttu-id="6288a-642">Absturz in `ad signed-in-user` beim Auflisten von in Besitz befindlichen Objekten behoben</span><span class="sxs-lookup"><span data-stu-id="6288a-642">Fixed a crash in `ad signed-in-user` when listing owned objects</span></span>
* <span data-ttu-id="6288a-643">Problem behoben, aufgrund dessen `ad sp` nicht die richtige Anwendung über einen Dienstprinzipal fand</span><span class="sxs-lookup"><span data-stu-id="6288a-643">Fixed issue where `ad sp` would not find the right application from a service principal</span></span>

### <a name="rdbms"></a><span data-ttu-id="6288a-644">RDBMS</span><span class="sxs-lookup"><span data-stu-id="6288a-644">RDBMS</span></span>

* <span data-ttu-id="6288a-645">Unterstützung für die Replikation für MariaDB hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-645">Added support for replication for MariaDB</span></span>

### <a name="sql"></a><span data-ttu-id="6288a-646">SQL</span><span class="sxs-lookup"><span data-stu-id="6288a-646">SQL</span></span>

* <span data-ttu-id="6288a-647">Zulässige Werte für `sql db create --sample-name` dokumentiert</span><span class="sxs-lookup"><span data-stu-id="6288a-647">Documented allowed values for `sql db create --sample-name`</span></span>

### <a name="storage"></a><span data-ttu-id="6288a-648">Storage</span><span class="sxs-lookup"><span data-stu-id="6288a-648">Storage</span></span>

* <span data-ttu-id="6288a-649">Unterstützung von SAS-Token für die Benutzerdelegierung mit `--as-user` zu `storage blob generate-sas` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-649">Added user delegation SAS token support with `--as-user` to `storage blob generate-sas`</span></span> 
* <span data-ttu-id="6288a-650">Unterstützung von SAS-Token für die Benutzerdelegierung mit `--as-user` zu `storage container generate-sas` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-650">Added user delegation SAS token support with `--as-user` to `storage container generate-sas`</span></span> 

### <a name="vm"></a><span data-ttu-id="6288a-651">VM</span><span class="sxs-lookup"><span data-stu-id="6288a-651">VM</span></span>

* <span data-ttu-id="6288a-652">Fehler behoben, aufgrund dessen `vmss create` bei der Ausführung mit `--no-wait` eine Fehlermeldung zurückgab</span><span class="sxs-lookup"><span data-stu-id="6288a-652">Fixed bug where `vmss create` returns an error message when run with `--no-wait`</span></span>
* <span data-ttu-id="6288a-653">Die clientseitige Validierung für `vmss create --single-placement-group` wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="6288a-653">Removed client-side validation for `vmss create --single-placement-group`.</span></span> <span data-ttu-id="6288a-654">Es tritt kein Fehler auf, wenn `--single-placement-group` auf `true` und für `--instance-count` ein größerer Wert als 100 festgelegt wird oder wenn Verfügbarkeitszonen angegeben werden. Diese Validierung wird jedoch dem Computedienst überlassen.</span><span class="sxs-lookup"><span data-stu-id="6288a-654">Does not fail if `--single-placement-group` is set to `true` and`--instance-count` is greater than 100 or availability zones are specified, but leaves this validation to the compute service</span></span>
* <span data-ttu-id="6288a-655">Problem behoben, aufgrund dessen bei der Verwendung von `--latest` für `[vm|vmss] extension image list` ein Fehler auftrat</span><span class="sxs-lookup"><span data-stu-id="6288a-655">Fixed bug where `[vm|vmss] extension image list` fails when used with `--latest`</span></span>


## <a name="june-18-2019"></a><span data-ttu-id="6288a-656">18. Juni 2019</span><span class="sxs-lookup"><span data-stu-id="6288a-656">June 18, 2019</span></span>

<span data-ttu-id="6288a-657">Version 2.0.67</span><span class="sxs-lookup"><span data-stu-id="6288a-657">Version 2.0.67</span></span>

### <a name="core"></a><span data-ttu-id="6288a-658">Core</span><span class="sxs-lookup"><span data-stu-id="6288a-658">Core</span></span>

<span data-ttu-id="6288a-659">In diesem Release wird das neue [Preview]-Tag eingeführt, um Kunden gegenüber deutlich zu machen, dass sich eine Befehlsgruppe, ein Befehl oder ein Argument in der Vorschauphase befindet.</span><span class="sxs-lookup"><span data-stu-id="6288a-659">This release introduces a new [Preview] tag to more clearly communicate to customers when a command group, command or argument is in preview status.</span></span> <span data-ttu-id="6288a-660">Diese Information war zuvor im Hilfetext oder implizit durch die Versionsnummer des Befehlsmoduls angegeben.</span><span class="sxs-lookup"><span data-stu-id="6288a-660">This was previously called out in help text or communicated implicitly by the command module version number.</span></span>
<span data-ttu-id="6288a-661">Die Befehlszeilenschnittstelle wird künftig Versionsnummern für einzelne Pakete entfernen.</span><span class="sxs-lookup"><span data-stu-id="6288a-661">The CLI will be removing version numbers for individual packages in the future.</span></span> <span data-ttu-id="6288a-662">Wenn sich ein Befehl in der Vorschauphase befindet, gilt dies auch für alle seine Argumente.</span><span class="sxs-lookup"><span data-stu-id="6288a-662">If a command is in preview, all of its arguments are as well.</span></span> <span data-ttu-id="6288a-663">Wenn eine Befehlsgruppe als Vorschau gekennzeichnet ist, befinden sich auch alle Befehle und Argumente in der Vorschauphase.</span><span class="sxs-lookup"><span data-stu-id="6288a-663">If a command group is labeled as being in preview, then all commands and arguments are considered to be in preview as well.</span></span>

<span data-ttu-id="6288a-664">Infolge dieser Änderung befinden sich in diesem Release verschiedene Befehlsgruppen anscheinend „plötzlich“ in der Vorschauphase.</span><span class="sxs-lookup"><span data-stu-id="6288a-664">As a result of this change, several command groups may seem to "suddenly" appear to be in a preview status with this release.</span></span> <span data-ttu-id="6288a-665">Tatsächlich ist es jedoch so, dass sich die meisten Pakete in der Vorschauphase befanden, in diesem Release jedoch als allgemein verfügbar gelten.</span><span class="sxs-lookup"><span data-stu-id="6288a-665">What actually happened is that most packages were in a preview status, but are being deemed GA with this release</span></span>

### <a name="acr"></a><span data-ttu-id="6288a-666">ACR</span><span class="sxs-lookup"><span data-stu-id="6288a-666">ACR</span></span>
* <span data-ttu-id="6288a-667">Befehl „acr check-health“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-667">Added 'acr check-health' command</span></span>
* <span data-ttu-id="6288a-668">Verbesserte Fehlerbehandlung für AAD-Token und für das Abrufen externer Befehle</span><span class="sxs-lookup"><span data-stu-id="6288a-668">Improved error handling for AAD tokens and for retrieving external commands</span></span>

### <a name="acs"></a><span data-ttu-id="6288a-669">ACS</span><span class="sxs-lookup"><span data-stu-id="6288a-669">ACS</span></span>
* <span data-ttu-id="6288a-670">Veraltete ACS-Befehle werden jetzt in der Hilfeansicht ausgeblendet.</span><span class="sxs-lookup"><span data-stu-id="6288a-670">Deprecated ACS commands are now hidden from help view</span></span>

### <a name="ams"></a><span data-ttu-id="6288a-671">AMS</span><span class="sxs-lookup"><span data-stu-id="6288a-671">AMS</span></span>
* <span data-ttu-id="6288a-672">[BREAKING CHANGE] Änderung, damit ISO 8601-Zeitzeichenfolgen für „archive-window-length“ und „key-frame-interval-duration“ zurückgegeben werden</span><span class="sxs-lookup"><span data-stu-id="6288a-672">[BREAKING CHANGE] Changed to return ISO 8601 time strings for archive-window-length and key-frame-interval-duration</span></span>

### <a name="appservice"></a><span data-ttu-id="6288a-673">AppService</span><span class="sxs-lookup"><span data-stu-id="6288a-673">AppService</span></span>
* <span data-ttu-id="6288a-674">Standortbasiertes Routing für `webapp deleted list` und `webapp deleted restore` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-674">Added location based routing for `webapp deleted list` and `webapp deleted restore`</span></span>
* <span data-ttu-id="6288a-675">Problem behoben, aufgrund dessen in Azure Cloud Shell nicht auf die von einer Web-App protokollierte Ziel-URL („Sie können die App starten unter...“) geklickt werden konnte</span><span class="sxs-lookup"><span data-stu-id="6288a-675">Fixed issue where webapp up logged target URL ("You can launch the app at...") was not clickable in Azure Cloud Shell</span></span>
* <span data-ttu-id="6288a-676">Problem behoben, aufgrund dessen beim Erstellen von Apps bei einigen SKUs ein AlwaysOn-Fehler auftrat</span><span class="sxs-lookup"><span data-stu-id="6288a-676">Fixed an issue where creating apps with the some SKUs was failing with an AlwaysOn error</span></span>
* <span data-ttu-id="6288a-677">Vorabüberprüfung zu `[appservice|webapp] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-677">Added pre-validation to `[appservice|webapp] create`</span></span>
* <span data-ttu-id="6288a-678">`[webapp|functionapp] traffic-routing` korrigiert, damit der richtige actionHostName-Wert verwendet wird</span><span class="sxs-lookup"><span data-stu-id="6288a-678">Fixed `[webapp|functionapp] traffic-routing` to use the correct actionHostName</span></span>
* <span data-ttu-id="6288a-679">Slotunterstützung zu `functionapp`-Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-679">Added slot support to `functionapp` commands</span></span>

### <a name="batch"></a><span data-ttu-id="6288a-680">Batch</span><span class="sxs-lookup"><span data-stu-id="6288a-680">Batch</span></span>
* <span data-ttu-id="6288a-681">AAD-Authentifizierungsregression korrigiert, die von übermäßiger Berichterstellung für Authentifizierung mit gemeinsam verwendetem Schlüssel verursacht wurde</span><span class="sxs-lookup"><span data-stu-id="6288a-681">Fixed AAD auth regression caused by over-aggressive error reporting for Shared Key Auth</span></span>

### <a name="batchai"></a><span data-ttu-id="6288a-682">Batch AI</span><span class="sxs-lookup"><span data-stu-id="6288a-682">BatchAI</span></span>
* <span data-ttu-id="6288a-683">BatchAI-Befehle sind jetzt veraltet und ausgeblendet.</span><span class="sxs-lookup"><span data-stu-id="6288a-683">BatchAI commands are now deprecated and hidden</span></span>

### <a name="botservice"></a><span data-ttu-id="6288a-684">BotService</span><span class="sxs-lookup"><span data-stu-id="6288a-684">BotService</span></span>
* <span data-ttu-id="6288a-685">Für Befehle, die Version 3 des SDK unterstützen, wurden die Warnmeldungen „Support eingestellt“/„Wartungsmodus“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-685">Added "discontinued support"/"maintenance mode" warning messages for commands that support the v3 SDK</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="6288a-686">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="6288a-686">CosmosDB</span></span>
* <span data-ttu-id="6288a-687">[VERALTET] Der Befehl `cosmosdb list-keys` wurde als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="6288a-687">[DEPRECATED] Deprecated the `cosmosdb list-keys` command</span></span>
* <span data-ttu-id="6288a-688">Befehl `cosmosdb keys list` hinzugefügt, er ersetzt `cosmosdb list-keys`.</span><span class="sxs-lookup"><span data-stu-id="6288a-688">Added the `cosmosdb keys list` command - replaces `cosmosdb list-keys`</span></span>
* <span data-ttu-id="6288a-689">`cosmsodb create/update`: Neues Format für „--location“ hinzugefügt, um das Festlegen der Eigenschaft „isZoneRedundant“ zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="6288a-689">`cosmsodb create/update`: Added new format for --location to allow setting "isZoneRedundant" property.</span></span> <span data-ttu-id="6288a-690">Das alte Format wurde als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="6288a-690">Deprecated old format</span></span>

### <a name="eventgrid"></a><span data-ttu-id="6288a-691">EventGrid</span><span class="sxs-lookup"><span data-stu-id="6288a-691">EventGrid</span></span>
* <span data-ttu-id="6288a-692">`eventgrid domain`-Befehle für CRUD-Vorgänge für Domänen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-692">Added `eventgrid domain` commands for domain CRUD operations</span></span>
* <span data-ttu-id="6288a-693">`eventgrid domain topic`-Befehle für CRUD-Vorgänge für Domänenthemen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-693">Added `eventgrid domain topic` commands for domain topics CRUD operations</span></span>
* <span data-ttu-id="6288a-694">Argument `--odata-query` zu `eventgrid [topic|event-subscription] list` zum Filtern der Ergebnisse mithilfe von OData-Syntax hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-694">Added `--odata-query` argument to `eventgrid [topic|event-subscription] list` for filtering results using OData syntax</span></span>
* <span data-ttu-id="6288a-695">`event-subscription create/update`: „servicebusqueue“ als neue Werte für den Parameter `--endpoint-type` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-695">`event-subscription create/update`: Added servicebusqueue as new values for the `--endpoint-type` parameter</span></span>
* <span data-ttu-id="6288a-696">[BREAKING CHANGE] Unterstützung für `--included-event-types All` mit `eventgrid event-subscription [create|update]` entfernt</span><span class="sxs-lookup"><span data-stu-id="6288a-696">[BREAKING CHANGE] Removed support for `--included-event-types All` with `eventgrid event-subscription [create|update]`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="6288a-697">HDInsight</span><span class="sxs-lookup"><span data-stu-id="6288a-697">HDInsight</span></span>
* <span data-ttu-id="6288a-698">Unterstützung für den Parameter `--ssh-public-key` im Befehl vom Typ `hdinsight create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-698">Added support for `--ssh-public-key` parameter in `hdinsight create` command</span></span>

### <a name="iot"></a><span data-ttu-id="6288a-699">IoT</span><span class="sxs-lookup"><span data-stu-id="6288a-699">IoT</span></span>
* <span data-ttu-id="6288a-700">Unterstützung für das erneute Generieren von Autorisierungsrichtlinienschlüsseln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-700">Added support to regenerate authorization policy keys</span></span>
* <span data-ttu-id="6288a-701">SDK und Unterstützung für den Bereitstellungsdienst des DigitalTwin-Repositorys hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-701">Added SDK and support for DigitalTwin Repository Provisioning Service</span></span>

### <a name="network"></a><span data-ttu-id="6288a-702">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6288a-702">Network</span></span>
* <span data-ttu-id="6288a-703">Zonenunterstützung für NAT Gateway hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-703">Added Zone support for Nat Gateway</span></span>
* <span data-ttu-id="6288a-704">Befehl `network list-service-tags` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-704">Added command `network list-service-tags`</span></span>
* <span data-ttu-id="6288a-705">Problem mit `dns zone import` behoben, aufgrund dessen Benutzer keine A-Platzhaltereinträge importieren konnten</span><span class="sxs-lookup"><span data-stu-id="6288a-705">Fixed issue with `dns zone import` where users could not import wildcard A records</span></span>
* <span data-ttu-id="6288a-706">Problem mit `watcher flow-log configure` behoben, aufgrund dessen die Flowprotokollierung in bestimmten Regionen nicht aktiviert werden konnte</span><span class="sxs-lookup"><span data-stu-id="6288a-706">Fixed issue with `watcher flow-log configure` where flow logging could not be enabled in certain regions</span></span>

### <a name="resource"></a><span data-ttu-id="6288a-707">Resource</span><span class="sxs-lookup"><span data-stu-id="6288a-707">Resource</span></span>
* <span data-ttu-id="6288a-708">Befehl `az rest` zum Ausführen von REST-Aufrufen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-708">Added `az rest` command for making REST calls</span></span>
* <span data-ttu-id="6288a-709">Fehler behoben, der bei Verwendung von `policy assignment list` mit `--scope` auf Ressourcengruppen- oder Abonnementebene auftrat</span><span class="sxs-lookup"><span data-stu-id="6288a-709">Fixed error when using `policy assignment list` with a resource group or subscription level `--scope`</span></span>

### <a name="servicebus"></a><span data-ttu-id="6288a-710">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="6288a-710">ServiceBus</span></span>
* <span data-ttu-id="6288a-711">Problem mit `servicebus topic create --max-size` behoben [Nr. 9319](https://github.com/azure/azure-cli/issues/9319)</span><span class="sxs-lookup"><span data-stu-id="6288a-711">Fixed issue with `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span></span>

### <a name="sql"></a><span data-ttu-id="6288a-712">SQL</span><span class="sxs-lookup"><span data-stu-id="6288a-712">SQL</span></span>
* <span data-ttu-id="6288a-713">`--location` wurde geändert und ist nun für `sql [server|mi] create` optional. Ohne Angabe wird der Ressourcengruppenstandort verwendet.</span><span class="sxs-lookup"><span data-stu-id="6288a-713">Changed `--location` to be optional for `sql [server|mi] create` - uses resource group location if not specified</span></span>
* <span data-ttu-id="6288a-714">Der Fehler, dass das Objekt „NoneType“ nicht wiederholbar ist, wurde für `sql db list-editions --available` behoben.</span><span class="sxs-lookup"><span data-stu-id="6288a-714">Fixed "'NoneType' object is not iterable" error for `sql db list-editions --available`</span></span>

### <a name="sqlvm"></a><span data-ttu-id="6288a-715">SQLVm</span><span class="sxs-lookup"><span data-stu-id="6288a-715">SQLVm</span></span>
* <span data-ttu-id="6288a-716">[WICHTIGE ÄNDERUNG] `sql vm create` wurde geändert und erfordert nun den Parameter `--license-type`.</span><span class="sxs-lookup"><span data-stu-id="6288a-716">[BREAKING CHNAGE] Changed `sql vm create` to require `--license-type` parameter</span></span>
* <span data-ttu-id="6288a-717">Änderung, um beim Erstellen oder Aktualisieren einer SQL-VM das Festlegen der SQL-Image-SKU zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="6288a-717">Changed to allow setting SQL image SKU when creating or updating a sql vm</span></span>

### <a name="storage"></a><span data-ttu-id="6288a-718">Storage</span><span class="sxs-lookup"><span data-stu-id="6288a-718">Storage</span></span>
* <span data-ttu-id="6288a-719">Problem mit fehlendem Kontoschlüssel für `storage container generate-sas` behoben</span><span class="sxs-lookup"><span data-stu-id="6288a-719">Fixed issue with missing account key for `storage container generate-sas`</span></span>
* <span data-ttu-id="6288a-720">Problem mit `storage blob sync` unter Linux behoben</span><span class="sxs-lookup"><span data-stu-id="6288a-720">Fixed issue with `storage blob sync` on Linux</span></span>

### <a name="vm"></a><span data-ttu-id="6288a-721">VM</span><span class="sxs-lookup"><span data-stu-id="6288a-721">VM</span></span>
* <span data-ttu-id="6288a-722">[VORSCHAU] Befehle vom Typ `vm image template` zum Erstellen von VM-Images hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-722">[PREVIEW] Added `vm image template` commands to build VM images</span></span>

## <a name="june-4-2019"></a><span data-ttu-id="6288a-723">4\. Juni 2019</span><span class="sxs-lookup"><span data-stu-id="6288a-723">June 4, 2019</span></span>

<span data-ttu-id="6288a-724">Version 2.0.66</span><span class="sxs-lookup"><span data-stu-id="6288a-724">Version 2.0.66</span></span>

### <a name="core"></a><span data-ttu-id="6288a-725">Core</span><span class="sxs-lookup"><span data-stu-id="6288a-725">Core</span></span>
* <span data-ttu-id="6288a-726">Fehler behoben, aufgrund dessen bei Befehlen ein Fehler auftrat, wenn `--output yaml` mit `--query` verwendet wurde</span><span class="sxs-lookup"><span data-stu-id="6288a-726">Fixed bug where commands fail if `--output yaml` is used with `--query`</span></span>

### <a name="acr"></a><span data-ttu-id="6288a-727">ACR</span><span class="sxs-lookup"><span data-stu-id="6288a-727">ACR</span></span>
* <span data-ttu-id="6288a-728">Befehlsgruppe „acr pack“ zum Erstellen von Aufgaben zur Schnellerstellung mit Buildpacks hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-728">Added 'acr pack' command group for creating quick build Tasks using Buildpacks.</span></span>

### <a name="acs"></a><span data-ttu-id="6288a-729">ACS</span><span class="sxs-lookup"><span data-stu-id="6288a-729">ACS</span></span>
* <span data-ttu-id="6288a-730">Zulassen der Aktivierung/Deaktivierung des AKS-Add-Ons für das Kube-Dashboard</span><span class="sxs-lookup"><span data-stu-id="6288a-730">Allow enabling/disabling AKS kube-dashboard addon</span></span>
* <span data-ttu-id="6288a-731">Ausgeben einer benutzerfreundlichen Nachricht, wenn das Abonnement nicht in der Whitelist zur Verwendung von Azure Red Hat OpenShift enthalten ist</span><span class="sxs-lookup"><span data-stu-id="6288a-731">Print a friendly message when the subscription is not whitelisted to use Azure Red Hat OpenShift</span></span>

### <a name="batch"></a><span data-ttu-id="6288a-732">Batch</span><span class="sxs-lookup"><span data-stu-id="6288a-732">Batch</span></span>
* <span data-ttu-id="6288a-733">Bessere Fehlerbehandlung, wenn der Benutzer nicht bei einem Konto angemeldet ist \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span><span class="sxs-lookup"><span data-stu-id="6288a-733">Improved error handling when not logged in to an account \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span></span>

### <a name="iot"></a><span data-ttu-id="6288a-734">IoT</span><span class="sxs-lookup"><span data-stu-id="6288a-734">IoT</span></span>
* <span data-ttu-id="6288a-735">Unterstützung für manuelles Failover hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-735">Added support for manual failover</span></span>

### <a name="network"></a><span data-ttu-id="6288a-736">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6288a-736">Network</span></span>
* <span data-ttu-id="6288a-737">Befehle vom Typ `network application-gateway waf-policy` hinzugefügt, um benutzerdefinierte WAF-Regeln zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="6288a-737">Added `network application-gateway waf-policy` commands to support custom WAF rules.</span></span>
* <span data-ttu-id="6288a-738">Argumente `--waf-policy` und `--max-capacity` zu `network application-gateway [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-738">Added `--waf-policy` and `--max-capacity` arguments to `network application-gateway [create|update]`</span></span> 

### <a name="resource"></a><span data-ttu-id="6288a-739">Resource</span><span class="sxs-lookup"><span data-stu-id="6288a-739">Resource</span></span>
* <span data-ttu-id="6288a-740">Verbesserte Fehlermeldungen aus `deployment create`, wenn TTY nicht verfügbar ist</span><span class="sxs-lookup"><span data-stu-id="6288a-740">Improved error message from `deployment create` when there is no TTY available</span></span>

### <a name="role"></a><span data-ttu-id="6288a-741">Role</span><span class="sxs-lookup"><span data-stu-id="6288a-741">Role</span></span>
* <span data-ttu-id="6288a-742">Hilfetext aktualisiert</span><span class="sxs-lookup"><span data-stu-id="6288a-742">Updated help text.</span></span>

### <a name="compute"></a><span data-ttu-id="6288a-743">Compute</span><span class="sxs-lookup"><span data-stu-id="6288a-743">Compute</span></span>
* <span data-ttu-id="6288a-744">Unterstützung zu `vm create` für virtuelle Computer aus einem verwalteten Image mit Datenträger-LUNs hinzugefügt, die nicht bei 0 beginnen oder die Nummern überspringen</span><span class="sxs-lookup"><span data-stu-id="6288a-744">Added support to `vm create` for VMs from a managed image with data-disk luns that do not start from 0 or that skip numbers</span></span>

## <a name="may-21-2019"></a><span data-ttu-id="6288a-745">21. Mai 2019</span><span class="sxs-lookup"><span data-stu-id="6288a-745">May 21, 2019</span></span>

<span data-ttu-id="6288a-746">Version 2.0.65</span><span class="sxs-lookup"><span data-stu-id="6288a-746">Version 2.0.65</span></span>

### <a name="core"></a><span data-ttu-id="6288a-747">Core</span><span class="sxs-lookup"><span data-stu-id="6288a-747">Core</span></span>
* <span data-ttu-id="6288a-748">Besseres Feedback für Authentifizierungsfehler hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-748">Added better feedback for authentication errors</span></span>
* <span data-ttu-id="6288a-749">Problem behoben, aufgrund dessen die CLI Erweiterungen lädt, die nicht mit der Core-Version kompatibel waren</span><span class="sxs-lookup"><span data-stu-id="6288a-749">Fixed issue where the CLI would load extensions that were not compatible with its core version</span></span>
* <span data-ttu-id="6288a-750">Problem beim Starten behoben, wenn `clouds.config` beschädigt ist</span><span class="sxs-lookup"><span data-stu-id="6288a-750">Fixed issue with launching when `clouds.config` is corrupted</span></span>

### <a name="acr"></a><span data-ttu-id="6288a-751">ACR</span><span class="sxs-lookup"><span data-stu-id="6288a-751">ACR</span></span>
* <span data-ttu-id="6288a-752">Unterstützung für verwaltete Identitäten zu Aufgaben hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-752">Added support for Managed Identities to Tasks</span></span>

### <a name="acs"></a><span data-ttu-id="6288a-753">ACS</span><span class="sxs-lookup"><span data-stu-id="6288a-753">ACS</span></span>
* <span data-ttu-id="6288a-754">`openshift create`-Befehl bei der Verwendung mit dem AAD-Kundenclient korrigiert</span><span class="sxs-lookup"><span data-stu-id="6288a-754">Fixed `openshift create` command when used with customer AAD client</span></span>

### <a name="appservice"></a><span data-ttu-id="6288a-755">AppService</span><span class="sxs-lookup"><span data-stu-id="6288a-755">AppService</span></span>
* <span data-ttu-id="6288a-756">[VERALTET] Befehl `functionapp devops-build` als veraltet gekennzeichnet – wird in der nächsten Version entfernt</span><span class="sxs-lookup"><span data-stu-id="6288a-756">[DEPRECATED] Deprecated `functionapp devops-build` command - will be removed in next release</span></span>
* <span data-ttu-id="6288a-757">`functionapp devops-pipeline` geändert, um das Buildprotokoll von Azure DevOps im ausführlichen Modus abzurufen</span><span class="sxs-lookup"><span data-stu-id="6288a-757">Changed `functionapp devops-pipeline` to fetch build log from Azure DevOps in verbose mode</span></span>
* <span data-ttu-id="6288a-758">[BREAKING CHANGE] Flag `--use_local_settings` aus dem Befehl `functionapp devops-pipeline` entfernt – kein Vorgang wurde ausgeführt</span><span class="sxs-lookup"><span data-stu-id="6288a-758">[BREAKING CHANGE] Removed `--use_local_settings` flag from `functionapp devops-pipeline` command - was a no-op</span></span>
* <span data-ttu-id="6288a-759">`webapp up` geändert, sodass die JSON-Ausgabe zurückgegeben wird, wenn `--logs` nicht verwendet wird</span><span class="sxs-lookup"><span data-stu-id="6288a-759">Changed `webapp up` to return JSON output if `--logs` is not used</span></span>
* <span data-ttu-id="6288a-760">Unterstützung hinzugefügt zum Schreiben von Standardressourcen in die lokale Konfiguration für `webapp up`</span><span class="sxs-lookup"><span data-stu-id="6288a-760">Added support for writing default resources to local config for `webapp up`</span></span>
* <span data-ttu-id="6288a-761">Unterstützung zu `webapp up` hinzugefügt für die erneute Bereitstellung einer App ohne Verwendung des `--location`-Arguments</span><span class="sxs-lookup"><span data-stu-id="6288a-761">Added support to `webapp up` for redeploying an app without using the `--location` argument</span></span>
* <span data-ttu-id="6288a-762">Problem behoben, bei dem für die ASP-Erstellung der Linux-SKU „Free“ der SKU-Wert „Free“ nicht funktioniert hat</span><span class="sxs-lookup"><span data-stu-id="6288a-762">Fixed an issue where for Linux Free SKU ASP creation use Free as SKU value was not working</span></span>

### <a name="botservice"></a><span data-ttu-id="6288a-763">BotService</span><span class="sxs-lookup"><span data-stu-id="6288a-763">BotService</span></span>
* <span data-ttu-id="6288a-764">Geändert, sodass Groß-/Kleinschreibung für `--lang`-Parameter für Befehle zulässig ist</span><span class="sxs-lookup"><span data-stu-id="6288a-764">Changed to allow all casing for `--lang` parameters for commands</span></span>
* <span data-ttu-id="6288a-765">Beschreibung für das Befehlsmodul aktualisiert</span><span class="sxs-lookup"><span data-stu-id="6288a-765">Updated description for command module</span></span>

### <a name="consumption"></a><span data-ttu-id="6288a-766">Nutzung</span><span class="sxs-lookup"><span data-stu-id="6288a-766">Consumption</span></span>
* <span data-ttu-id="6288a-767">Fehlende erforderliche Parameter bei der Ausführung von `consumption usage list --billing-period-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-767">Added missing required parameter when running `consumption usage list --billing-period-name`</span></span>

### <a name="iot"></a><span data-ttu-id="6288a-768">IoT</span><span class="sxs-lookup"><span data-stu-id="6288a-768">IoT</span></span>
* <span data-ttu-id="6288a-769">Unterstützung für das Auflisten aller Schlüssel hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-769">Added support to list all keys</span></span>

### <a name="network"></a><span data-ttu-id="6288a-770">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6288a-770">Network</span></span>
* [BREAKING CHANGE]: Removed `network interface-endpoints` command group - use `network private-endpoints` 
* <span data-ttu-id="6288a-772">`--nat-gateway`-Argument zu `network vnet subnet [create|update]` für das Anfügen an ein NAT-Gateway hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-772">Added `--nat-gateway` argument to `network vnet subnet [create|update]` for attaching to a NAT gateway</span></span>
* <span data-ttu-id="6288a-773">Problem mit `dns zone import` behoben, aufgrund dessen Eintragsnamen keinem Datensatztyp entsprochen haben</span><span class="sxs-lookup"><span data-stu-id="6288a-773">Fixed issue with `dns zone import` where record names could not match a record type</span></span>

### <a name="rdbms"></a><span data-ttu-id="6288a-774">RDBMS</span><span class="sxs-lookup"><span data-stu-id="6288a-774">RDBMS</span></span>
* <span data-ttu-id="6288a-775">Postgres- und MySLQ-Unterstützung für die Georeplikation hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-775">Added postgres and mysql support for geo replication</span></span>

### <a name="rbac"></a><span data-ttu-id="6288a-776">RBAC</span><span class="sxs-lookup"><span data-stu-id="6288a-776">RBAC</span></span>
* <span data-ttu-id="6288a-777">Unterstützung für den Verwaltungsgruppenumfang zu `role assignment` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-777">Added support for management group scope to `role assignment`</span></span>

### <a name="storage"></a><span data-ttu-id="6288a-778">Storage</span><span class="sxs-lookup"><span data-stu-id="6288a-778">Storage</span></span>
* <span data-ttu-id="6288a-779">`storage blob sync`: Synchronisierungsbefehl für Speicherblob hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-779">`storage blob sync`: add sync command for storage blob</span></span>

### <a name="compute"></a><span data-ttu-id="6288a-780">Compute</span><span class="sxs-lookup"><span data-stu-id="6288a-780">Compute</span></span>
* <span data-ttu-id="6288a-781">`--computer-name` zu `vm create` zum Festlegen des Computernamens eines virtuellen Computers hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-781">Added `--computer-name` to `vm create` for setting a VM's computer name</span></span>
* <span data-ttu-id="6288a-782">`--ssh-key-value` umbenannt in `--ssh-key-values` für `[vm|vmss] create`: Jetzt können mehrere öffentliche SSH-Schlüsselwerte oder -pfade akzeptiert werden.</span><span class="sxs-lookup"><span data-stu-id="6288a-782">Renamed `--ssh-key-value` renamed to `--ssh-key-values` for `[vm|vmss] create` - can now accept multiple ssh public key values or paths</span></span>
  * <span data-ttu-id="6288a-783">__Hinweis__: Dies ist **kein** Breaking Change: `--ssh-key-value` wird korrekt analysiert, da nur eine Übereinstimmung mit `--ssh-key-values` besteht.</span><span class="sxs-lookup"><span data-stu-id="6288a-783">__Note__: This is **not** a breaking change - `--ssh-key-value` will be parsed correctly as it matches only `--ssh-key-values`</span></span>
* <span data-ttu-id="6288a-784">`--type`-Argument von `ppg create` in optionales Argument geändert</span><span class="sxs-lookup"><span data-stu-id="6288a-784">Changed the `--type` argument of `ppg create` to be optional</span></span>

## <a name="may-6-2019"></a><span data-ttu-id="6288a-785">6\. Mai 2019</span><span class="sxs-lookup"><span data-stu-id="6288a-785">May 6, 2019</span></span>

<span data-ttu-id="6288a-786">Version 2.0.64</span><span class="sxs-lookup"><span data-stu-id="6288a-786">Version 2.0.64</span></span>

### <a name="acs"></a><span data-ttu-id="6288a-787">ACS</span><span class="sxs-lookup"><span data-stu-id="6288a-787">ACS</span></span>
* <span data-ttu-id="6288a-788">[BREAKING CHANGE] Flag `--fqdn` aus den `openshift`-Befehlen entfernt</span><span class="sxs-lookup"><span data-stu-id="6288a-788">[BREAKING CHANGE] Removed `--fqdn` flag on `openshift` commands</span></span>
* <span data-ttu-id="6288a-789">Geändert, sodass die allgemein verfügbare Azure Red Hat Openshift-API-Version verwendet wird</span><span class="sxs-lookup"><span data-stu-id="6288a-789">Changed to use Azure Red Hat Openshift GA API Version</span></span>
* <span data-ttu-id="6288a-790">Flag `customer-admin-group-id` wurde zu `openshift create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-790">Added `customer-admin-group-id` flag to `openshift create`</span></span>
* <span data-ttu-id="6288a-791">[ALLGEMEIN VERFÜGBAR] `(PREVIEW)` aus der `aks create`-Option `--network-policy` entfernt</span><span class="sxs-lookup"><span data-stu-id="6288a-791">[GA] Removed `(PREVIEW)` from `aks create` option `--network-policy`</span></span>

### <a name="appservice"></a><span data-ttu-id="6288a-792">AppService</span><span class="sxs-lookup"><span data-stu-id="6288a-792">Appservice</span></span>
* <span data-ttu-id="6288a-793">[VERALTET] Befehl `functionapp devops-build` als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="6288a-793">[DEPRECATED] Deprecated `functionapp devops-build` command</span></span>
  * <span data-ttu-id="6288a-794">Umbenannt in `functionapp devops-pipeline`</span><span class="sxs-lookup"><span data-stu-id="6288a-794">Renamed to `functionapp devops-pipeline`</span></span>
* <span data-ttu-id="6288a-795">Fehler beim Abrufen des richtigen Benutzernamens für Cloud Shell behoben, der einen Fehler von `webapp up` verursachte</span><span class="sxs-lookup"><span data-stu-id="6288a-795">Fixed getting the correct username for cloudshell which was causing `webapp up` to fail</span></span>
* <span data-ttu-id="6288a-796">Dokumentation von `appservice plan --sku` mit den unterstützten App Service-Plänen aktualisiert</span><span class="sxs-lookup"><span data-stu-id="6288a-796">Updated `appservice plan --sku` documentation updated to reflect the supported appserviceplans</span></span>
* <span data-ttu-id="6288a-797">Optionale Argumente für Ressourcengruppe und Plan zu `webapp up` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-797">Added optional arguments for resource group and plan to `webapp up`</span></span>
* <span data-ttu-id="6288a-798">Unterstützung zur Berücksichtigung der Umgebungsvariablen `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` zu `webapp ssh` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-798">Added support to `webapp ssh` to respect `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>
* <span data-ttu-id="6288a-799">Unterstützung für `appserviceplan create` für die kostenlose Linux-SKU hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-799">Added `appserviceplan create` support for Linux Free SKU</span></span>
* <span data-ttu-id="6288a-800">`webapp up` geändert, um nach dem Festlegen der App-Einstellung `SCM_DO_BUILD_DURING_DEPLOYMENT=true` zum Verarbeiten des Kudu-Kaltstarts für 30 Sekunden in den Energiesparmodus zu wechseln</span><span class="sxs-lookup"><span data-stu-id="6288a-800">Changed `webapp up` to have a 30s sleep after setting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` appsetting to handle kudu cold start</span></span>
* <span data-ttu-id="6288a-801">Unterstützung für die `powershell`-Runtime zu `functionapp create` unter Windows hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-801">Added support for `powershell` runtime to `functionapp create` on Windows</span></span>
* <span data-ttu-id="6288a-802">Befehl `create-remote-connection` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-802">Added `create-remote-connection` command</span></span>

### <a name="batch"></a><span data-ttu-id="6288a-803">Batch</span><span class="sxs-lookup"><span data-stu-id="6288a-803">Batch</span></span>
* <span data-ttu-id="6288a-804">Fehler im Validierungssteuerelement für `--application-package-references`-Optionen korrigiert</span><span class="sxs-lookup"><span data-stu-id="6288a-804">Fixed bug in validator for `--application-package-references` options</span></span>

### <a name="botservice"></a><span data-ttu-id="6288a-805">Botservice</span><span class="sxs-lookup"><span data-stu-id="6288a-805">Botservice</span></span>
* <span data-ttu-id="6288a-806">[BREAKING CHANGE]`bot create -v v4 -k webapp` geändert, sodass standardmäßig eine leerer Web-App-Bot erstellt wird (d. h. kein Bot wird in App Service bereitgestellt)</span><span class="sxs-lookup"><span data-stu-id="6288a-806">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to create an empty Web App Bot by default (i.e. no bot is deployed to the App Service)</span></span>
* <span data-ttu-id="6288a-807">`--echo`-Flag zu `bot create` hinzugefügt, sodass das alte Verhalten mit `-v v4` verwendet wird</span><span class="sxs-lookup"><span data-stu-id="6288a-807">Added `--echo` flag to `bot create` to use the old behavior with `-v v4`</span></span>
* <span data-ttu-id="6288a-808">[BREAKING CHANGE] Standardwert von `--version` in `v4` geändert</span><span class="sxs-lookup"><span data-stu-id="6288a-808">[BREAKING CHANGE] Changed the default value of  `--version` to `v4`</span></span>
  * <span data-ttu-id="6288a-809">__HINWEIS:__ `bot prepare-publish` verwendet weiterhin den alten Standard.</span><span class="sxs-lookup"><span data-stu-id="6288a-809">__NOTE:__ `bot prepare-publish` still uses the its old default</span></span>
* <span data-ttu-id="6288a-810">[BREAKING CHANGE]`--lang` geändert, sodass der Standard nicht mehr `Csharp` ist.</span><span class="sxs-lookup"><span data-stu-id="6288a-810">[BREAKING CHANGE] Changed `--lang` to no longer default to `Csharp`.</span></span> <span data-ttu-id="6288a-811">Wenn der Befehl `--lang` erfordert und dies nicht angegeben ist, wird der Befehl nun mit Fehler beendet.</span><span class="sxs-lookup"><span data-stu-id="6288a-811">If the command requires `--lang` and it is not provided, the command will now error out</span></span>
* <span data-ttu-id="6288a-812">[BREAKING CHANGE]`--appid`- und `--password`-Argumente für `bot create` in erforderlich geändert, sie können jetzt über `ad app create` erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="6288a-812">[BREAKING CHANGE] Changed the `--appid` and `--password` args for `bot create` to be required and can now be created via `ad app create`</span></span>
* <span data-ttu-id="6288a-813">`--appid`- und `--password`-Validierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-813">Added `--appid` and `--password` validation</span></span>
* <span data-ttu-id="6288a-814">[BREAKING CHANGE]`bot create -v v4` geändert, sodass kein Speicherkonto bzw. keine Application Insights-Instanz erstellt oder verwendet wird</span><span class="sxs-lookup"><span data-stu-id="6288a-814">[BREAKING CHANGE] Changed `bot create -v v4` to not create or use a Storage Account or Application Insights</span></span>
* <span data-ttu-id="6288a-815">[BREAKING CHANGE]`bot create -v v3` geändert, sodass eine Region erforderlich ist, in der Application Insights verfügbar ist</span><span class="sxs-lookup"><span data-stu-id="6288a-815">[BREAKING CHANGE] Changed `bot create -v v3` to require a region where Application Insights is available</span></span>
* <span data-ttu-id="6288a-816">[BREAKING CHANGE]`bot update` geändert, sodass es sich jetzt nur auf spezifische Eigenschaften eines Bots auswirkt</span><span class="sxs-lookup"><span data-stu-id="6288a-816">[BREAKING CHANGE] Changed `bot update` to now affect only specific properties of a bot</span></span>
* <span data-ttu-id="6288a-817">[BREAKING CHANGE]`--lang`-Flags geändert, sodass `Javascript` anstelle von `Node` akzeptiert wird</span><span class="sxs-lookup"><span data-stu-id="6288a-817">[BREAKING CHANGE] Changed `--lang` flags to accept `Javascript` instead of `Node`</span></span>
* <span data-ttu-id="6288a-818">[BREAKING CHANGE]`Node` als zulässiger `--lang`-Wert entfernt.</span><span class="sxs-lookup"><span data-stu-id="6288a-818">[BREAKING CHANGE] Removed `Node` as an allowed `--lang` value</span></span>
* <span data-ttu-id="6288a-819">[BREAKING CHANGE]`bot create -v v4 -k webapp` geändert, sodass `SCM_DO_BUILD_DURING_DEPLOYMENT` nicht mehr auf TRUE festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="6288a-819">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to no longer set `SCM_DO_BUILD_DURING_DEPLOYMENT` to true.</span></span> <span data-ttu-id="6288a-820">Alle Bereitstellungen über Kudu fungieren ihrem Standardverhalten entsprechend.</span><span class="sxs-lookup"><span data-stu-id="6288a-820">All deployments through Kudu will act according to their default behavior</span></span>
* <span data-ttu-id="6288a-821">`bot download` für Bots ohne `.bot`-Dateien geändert, sodass die sprachspezifische Konfigurationsdatei mit Werten aus den Anwendungseinstellungen für den Bot erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="6288a-821">Changed `bot download` for bots without `.bot` files to create the language-specific configuration file with values from the Application Settings for the bot</span></span>
* <span data-ttu-id="6288a-822">Unterstützung für `Typescript` zu `bot prepare-deploy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-822">Added `Typescript` support to `bot prepare-deploy`</span></span>
* <span data-ttu-id="6288a-823">Warnmeldung zu `bot prepare-deploy` für `Javascript`- und `Typescript`-Bots hinzugefügt, wenn `package.json` in `--code-dir` nicht enthalten ist</span><span class="sxs-lookup"><span data-stu-id="6288a-823">Added warning message to `bot prepare-deploy` for `Javascript` and `Typescript` bots for when `--code-dir` does not contain `package.json`</span></span>
* <span data-ttu-id="6288a-824">`bot prepare-deploy` geändert, sodass bei Erfolg `true` zurückgegeben wird</span><span class="sxs-lookup"><span data-stu-id="6288a-824">Changed `bot prepare-deploy` to return `true` if successful</span></span>
* <span data-ttu-id="6288a-825">Ausführliche Protokollierung zu `bot prepare-deploy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-825">Added verbose logging to `bot prepare-deploy`</span></span>
* <span data-ttu-id="6288a-826">Mehr verfügbare Application Insights-Regionen zu `az bot create -v v3` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-826">Added more available Application Insights regions to `az bot create -v v3`</span></span>

### <a name="configure"></a><span data-ttu-id="6288a-827">Konfigurieren</span><span class="sxs-lookup"><span data-stu-id="6288a-827">Configure</span></span>
* <span data-ttu-id="6288a-828">Unterstützung für die ordnerbasierte Argument-Standardwertkonfigurationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-828">Added support for folder based argument default value configurations</span></span>

### <a name="eventhubs"></a><span data-ttu-id="6288a-829">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="6288a-829">Eventhubs</span></span>
* <span data-ttu-id="6288a-830">Befehle vom Typ `namespace network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-830">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="6288a-831">`--default-action`-Argument für Netzwerkregeln zu `namespace [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-831">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="6288a-832">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6288a-832">Network</span></span>
* <span data-ttu-id="6288a-833">[BREAKING CHANGE]`--cache`-Argument mit `--defer` für `vnet [create|update]` ersetzt</span><span class="sxs-lookup"><span data-stu-id="6288a-833">[BREAKING CHANGE] Replaced `--cache` arugment with `--defer` for `vnet [create|update]`</span></span> 

### <a name="policy-insights"></a><span data-ttu-id="6288a-834">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="6288a-834">Policy Insights</span></span>
* <span data-ttu-id="6288a-835">Unterstützung für `--expand PolicyEvaluationDetails` hinzugefügt, sodass Richtlinienauswertungsdetails von der Ressource abgefragt werden</span><span class="sxs-lookup"><span data-stu-id="6288a-835">Added support for `--expand PolicyEvaluationDetails` to query policy evaluation details on the resource</span></span>

### <a name="role"></a><span data-ttu-id="6288a-836">Role</span><span class="sxs-lookup"><span data-stu-id="6288a-836">Role</span></span>
* <span data-ttu-id="6288a-837">[VERALTET]: Ausblenden des „--password"-Arguments von `create-for-rbac` geändert; Unterstützung wird im Mai 2019 entfernt</span><span class="sxs-lookup"><span data-stu-id="6288a-837">[DEPRECATED] Changed `create-for-rbac` hide '--password' argument - support will be removed in May 2019</span></span>

### <a name="service-bus"></a><span data-ttu-id="6288a-838">Service Bus</span><span class="sxs-lookup"><span data-stu-id="6288a-838">Service Bus</span></span>
* <span data-ttu-id="6288a-839">Befehle vom Typ `namespace network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-839">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="6288a-840">`--default-action`-Argument für Netzwerkregeln zu `namespace [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-840">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>
* <span data-ttu-id="6288a-841">`topic [create|update]` korrigiert, sodass `--max-size`-Unterstützung für 10-, 20-, 40- und 80-GB-Werte mit Premium-SKU zulässig ist</span><span class="sxs-lookup"><span data-stu-id="6288a-841">Fixed `topic [create|update]` to allow `--max-size` support for 10, 20, 40 and 80GB values with premium SKU</span></span>

### <a name="sql"></a><span data-ttu-id="6288a-842">SQL</span><span class="sxs-lookup"><span data-stu-id="6288a-842">SQL</span></span>
* <span data-ttu-id="6288a-843">Befehle vom Typ `sql virtual-cluster [list|show|delete]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-843">Added `sql virtual-cluster [list|show|delete]` commands</span></span>

### <a name="vm"></a><span data-ttu-id="6288a-844">VM</span><span class="sxs-lookup"><span data-stu-id="6288a-844">VM</span></span>
* <span data-ttu-id="6288a-845">`--protect-from-scale-in` und `--protect-from-scale-set-actions` zu `vmss update` hinzugefügt, sodass Aktualisierungen der Schutzrichtlinie von VMSS-VM-Instanzen aktiviert sind</span><span class="sxs-lookup"><span data-stu-id="6288a-845">Added `--protect-from-scale-in` and `--protect-from-scale-set-actions` to `vmss update` to enable updates to the protection policy of VMSS VM instances</span></span>
* <span data-ttu-id="6288a-846">`--instance-id` zu `vmss update` hinzugefügt, sodass allgemeine Aktualisierungen von VMSS-VM-Instanzen aktiviert sind</span><span class="sxs-lookup"><span data-stu-id="6288a-846">Added `--instance-id` to `vmss update` to enable generic update of VMSS VM instances</span></span>
* <span data-ttu-id="6288a-847">`--instance-id` zu `vmss wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-847">Added `--instance-id` to `vmss wait`</span></span>
* <span data-ttu-id="6288a-848">Neue `ppg`-Befehlsgruppe für die Verwaltung von Näherungsplatzierungsgruppen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-848">Added new `ppg` command group for managing Proximity Placement Groups</span></span>
* <span data-ttu-id="6288a-849">`--ppg` zu `[vm|vmss] create` und `vm availability-set create` für die Verwaltung von PPGs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-849">Added `--ppg` to `[vm|vmss] create` and `vm availability-set create` for managing PPGs</span></span>
* <span data-ttu-id="6288a-850">Parameter `--hyper-v-generation` zu `image create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-850">Added `--hyper-v-generation` parameter to `image create`</span></span>

## <a name="april-23-2019"></a><span data-ttu-id="6288a-851">23. April 2019</span><span class="sxs-lookup"><span data-stu-id="6288a-851">April 23, 2019</span></span>

<span data-ttu-id="6288a-852">Version 2.0.63</span><span class="sxs-lookup"><span data-stu-id="6288a-852">Version 2.0.63</span></span>

### <a name="acs"></a><span data-ttu-id="6288a-853">ACS</span><span class="sxs-lookup"><span data-stu-id="6288a-853">ACS</span></span>
* <span data-ttu-id="6288a-854">`aks get-credentials` zur Anzeige einer Eingabeaufforderung zum Überschreiben doppelter Werte geändert</span><span class="sxs-lookup"><span data-stu-id="6288a-854">Changed `aks get-credentials` to prompt to overwrite duplicated values</span></span>
* <span data-ttu-id="6288a-855">`(PREVIEW)` aus Dev Spaces-Befehlen „aks use-dev-spaces“ und „aks remove-dev-spaces“ entfernt</span><span class="sxs-lookup"><span data-stu-id="6288a-855">Removed `(PREVIEW)` from Dev Spaces commands "aks use-dev-spaces" and "aks remove-dev-spaces"</span></span>

### <a name="ams"></a><span data-ttu-id="6288a-856">AMS</span><span class="sxs-lookup"><span data-stu-id="6288a-856">AMS</span></span>
* <span data-ttu-id="6288a-857">Fehler bei der Objekt- und Kontofilteraktualisierung behoben</span><span class="sxs-lookup"><span data-stu-id="6288a-857">Fixed bug with asset and account filters update</span></span>

### <a name="appservice"></a><span data-ttu-id="6288a-858">AppService</span><span class="sxs-lookup"><span data-stu-id="6288a-858">AppService</span></span>
* <span data-ttu-id="6288a-859">Unterstützung für die App Service-Umgebung (App Service Environment, ASE) und Zeitlimit zu `webapp ssh` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-859">Added support for ASE and timeout to `webapp ssh`</span></span>
* <span data-ttu-id="6288a-860">Unterstützung für die Einrichtung von CI/CD für eine Azure DevOps-Pipeline aus einem GitHub-Repository zu Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-860">Added support for establishing CI CD to an Azure DevOps pipeline from a Github repository to Function apps</span></span>
* <span data-ttu-id="6288a-861">`--github-pat`-Argument zu `functionapp devops-build create` hinzugefügt, um persönliche GitHub-Zugriffstoken zu akzeptieren</span><span class="sxs-lookup"><span data-stu-id="6288a-861">Added `--github-pat` argument to `functionapp devops-build create` to accept Github personal access token</span></span>
* <span data-ttu-id="6288a-862">`--github-repository`-Argument zu `functionapp devops-build create` hinzugefügt, um das GitHub-Repository mit dem Quellcode einer Funktions-App zu akzeptieren</span><span class="sxs-lookup"><span data-stu-id="6288a-862">Added `--github-repository` argument to `functionapp devops-build create` to accept Github repository that contains a functionapp source code</span></span>
* <span data-ttu-id="6288a-863">Problem behoben, aufgrund dessen bei `az webapp up --logs` ein Fehler auftrat und die .NET Core-Standardversion auf 2.1 aktualisiert wurde</span><span class="sxs-lookup"><span data-stu-id="6288a-863">Fixed issue where `az webapp up --logs` was failing with a error and updating default .NETCORE version to 2.1</span></span>
* <span data-ttu-id="6288a-864">Unnötige Funktions-App-Einstellungen beim Erstellen einer Funktions-App mit Verbrauchsplan entfernt</span><span class="sxs-lookup"><span data-stu-id="6288a-864">Removed unnecessary functionapp settings when creating a function app with consumption plan</span></span>
* <span data-ttu-id="6288a-865">`webapp up` geändert, sodass die ASP-Standardzeichenfolge jetzt eine Zahl am Ende anfügt, um einen neuen ASP basierend auf SKU-Optionen zu erstellen</span><span class="sxs-lookup"><span data-stu-id="6288a-865">Changed `webapp up` so the default asp string now appends number at the end to create a new ASP based on SKU options</span></span>
* <span data-ttu-id="6288a-866">`-b` als Option für `webapp up` hinzugefügt, um die App im Browser zu starten</span><span class="sxs-lookup"><span data-stu-id="6288a-866">Added `-b` as an option to `webapp up` to launch the app in the browser</span></span>
* <span data-ttu-id="6288a-867">`webapp deployment source config zip` geändert, um die `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`-Umgebungsvariable zu behandeln</span><span class="sxs-lookup"><span data-stu-id="6288a-867">Changed `webapp deployment source config zip` to handle `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="6288a-868">Bereitstellungs-Manager</span><span class="sxs-lookup"><span data-stu-id="6288a-868">Deployment Manager</span></span>
* <span data-ttu-id="6288a-869">[VORSCHAUVERSIPN] Erstellen und Verwalten von Artefakten, die Rollouts unterstützen</span><span class="sxs-lookup"><span data-stu-id="6288a-869">[PREVIEW] Create and manage artifacts that support rollouts</span></span>

### <a name="lab"></a><span data-ttu-id="6288a-870">Labor</span><span class="sxs-lookup"><span data-stu-id="6288a-870">Lab</span></span>
* <span data-ttu-id="6288a-871">Fehler behoben, der zu einer vorzeitigen Beendigung führen würde</span><span class="sxs-lookup"><span data-stu-id="6288a-871">Fixed bug which would cause an early exit</span></span>

### <a name="network"></a><span data-ttu-id="6288a-872">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6288a-872">Network</span></span>
* <span data-ttu-id="6288a-873">Automatische Delegierung des Namenservers im übergeordneten Element während der Erstellung der untergeordneten Zone zu `dns zone create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-873">Added auto name server delegation to `dns zone create` in parent during child zone creation</span></span>

### <a name="resource"></a><span data-ttu-id="6288a-874">Resource</span><span class="sxs-lookup"><span data-stu-id="6288a-874">Resource</span></span>
* <span data-ttu-id="6288a-875">[VERALTET]: Argumente `--link-id`, `--target-id` und `--filter-string` von `resource link` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="6288a-875">[DEPRECATED] Deprecated `--link-id`, `--target-id` and `--filter-string` arguments of `resource link`</span></span>
  * <span data-ttu-id="6288a-876">Verwenden Sie stattdessen die Argumente `--link`, `--target` und `--filter`.</span><span class="sxs-lookup"><span data-stu-id="6288a-876">Use the arguments `--link`, `--target`, and `--filter` instead</span></span>
* <span data-ttu-id="6288a-877">Problem behoben, aufgrund dessen `resource link [create|update]`-Befehle nicht verwendet werden konnten</span><span class="sxs-lookup"><span data-stu-id="6288a-877">Fixed issue where `resource link [create|update]` commands would not work</span></span>
* <span data-ttu-id="6288a-878">Problem behoben, aufgrund dessen das Löschen anhand einer Ressourcen-ID bei einem Fehler zu einem Absturz führen konnte</span><span class="sxs-lookup"><span data-stu-id="6288a-878">Fixed an issue where deleting using a resource ID could crash on error</span></span>

### <a name="sql"></a><span data-ttu-id="6288a-879">SQL</span><span class="sxs-lookup"><span data-stu-id="6288a-879">SQL</span></span>
* <span data-ttu-id="6288a-880">Unterstützung für benutzerdefinierte Zeitzonen auf verwalteten Instanzen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-880">Added support for custom time zone on managed instances</span></span>
* <span data-ttu-id="6288a-881">Geändert, um die Verwendung des Namens eines Pools für elastische Datenbanken mit `sql db update` zuzulassen</span><span class="sxs-lookup"><span data-stu-id="6288a-881">Changed to allow elastic pool name to be used with `sql db update`</span></span>
* <span data-ttu-id="6288a-882">Unterstützung für `--no-wait` zu `sql server [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-882">Added `--no-wait` support to `sql server [create|update]`</span></span>
* <span data-ttu-id="6288a-883">Befehl `sql server wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-883">Added command `sql server wait`</span></span>

### <a name="storage"></a><span data-ttu-id="6288a-884">Storage</span><span class="sxs-lookup"><span data-stu-id="6288a-884">Storage</span></span>
* <span data-ttu-id="6288a-885">Problem mit doppelt codierten SAS-Token in `storage blob generate-sas` behoben</span><span class="sxs-lookup"><span data-stu-id="6288a-885">Fixed issue with double-encoded SAS tokens in `storage blob generate-sas`</span></span>

### <a name="vm"></a><span data-ttu-id="6288a-886">VM</span><span class="sxs-lookup"><span data-stu-id="6288a-886">VM</span></span>
* <span data-ttu-id="6288a-887">`--skip-shutdown`-Flag zum Ausschalten von VMs ohne Herunterfahren zu `vm|vmss stop` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-887">Added `--skip-shutdown` flag to `vm|vmss stop` to power-off VMs without shutdown</span></span>
* <span data-ttu-id="6288a-888">`--storage-account-type`-Argument zum Festlegen des Kontotyps des Veröffentlichungsprofils zu `sig image-version create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-888">Added `--storage-account-type` argument to `sig image-version create` to set the publishing profile's account type</span></span>
* <span data-ttu-id="6288a-889">`--target-regions`-Argument zu `sig image-version create` hinzugefügt, um das Festlegen von regionsspezifischen Speicherkontotypen zuzulassen</span><span class="sxs-lookup"><span data-stu-id="6288a-889">Added `--target-regions` argument to `sig image-version create` to allow setting region-specific storage account types</span></span>

## <a name="april-9-2019"></a><span data-ttu-id="6288a-890">9\. April 2019</span><span class="sxs-lookup"><span data-stu-id="6288a-890">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="6288a-891">Core</span><span class="sxs-lookup"><span data-stu-id="6288a-891">Core</span></span>
* <span data-ttu-id="6288a-892">Problem behoben, aufgrund dessen einige Erweiterungen mit der Version `Unknown` angezeigt wurden und nicht aktualisiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="6288a-892">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="6288a-893">ACR</span><span class="sxs-lookup"><span data-stu-id="6288a-893">ACR</span></span>
* <span data-ttu-id="6288a-894">Unterstützung für die kontextlose Ausführung eines Images hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-894">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="6288a-895">AMS</span><span class="sxs-lookup"><span data-stu-id="6288a-895">AMS</span></span>
* [VERALTET]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
[DEPRECATED]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [BREAKING CHANGE]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="6288a-898">Unterstützung für neue Verschlüsselungsparameter in `ams streaming-policy create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-898">Added new encryption parameters support in `ams streaming-policy create`</span></span>
* <span data-ttu-id="6288a-899">Neuer Parameter `--filters` zu `ams streaming-locator create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-899">Added new paramter `--filters` to `ams streaming-locator create`</span></span>

### <a name="appservice"></a><span data-ttu-id="6288a-900">AppService</span><span class="sxs-lookup"><span data-stu-id="6288a-900">AppService</span></span>
* <span data-ttu-id="6288a-901">Unterstützung für `--logs` zu `webapp up` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-901">Added `--logs` support to `webapp up`</span></span>
* <span data-ttu-id="6288a-902">Probleme bei der Generierung von `azure-pipelines.yml` beim Befehl `functionapp devops-build create` behoben</span><span class="sxs-lookup"><span data-stu-id="6288a-902">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="6288a-903">Fehlerbehandlung und Indikatoren für `unctionapp devops-build create` verbessert</span><span class="sxs-lookup"><span data-stu-id="6288a-903">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="6288a-904">[BREAKING CHANGE] Flag `--local-git` für den Befehl `devops-build` entfernt; lokale Git-Erkennung und -Verarbeitung sind zum Erstellen von Azure DevOps-Pipelines obligatorisch</span><span class="sxs-lookup"><span data-stu-id="6288a-904">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="6288a-905">Unterstützung für das Erstellen von Linux-Functions-Plänen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-905">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="6288a-906">Möglichkeit zum Wechseln eines Plans unter einer Funktions-App mit `functionapp update --plan` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-906">Added ability to switch a plan underneath a function app using `functionapp update --plan`</span></span>
* <span data-ttu-id="6288a-907">Unterstützung für Einstellungen zum horizontalen Hochskalieren für den Azure Functions-Premium-Plan hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-907">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="6288a-908">CDN</span><span class="sxs-lookup"><span data-stu-id="6288a-908">CDN</span></span>
* <span data-ttu-id="6288a-909">Unterstützung hinzugefügt für `Microsoft_Standard` und `Standard_ChinaCdn`</span><span class="sxs-lookup"><span data-stu-id="6288a-909">Added support for `Microsoft_Standard` and `Standard_ChinaCdn`</span></span>

### <a name="feedback"></a><span data-ttu-id="6288a-910">Feedback</span><span class="sxs-lookup"><span data-stu-id="6288a-910">Feedback</span></span>
* <span data-ttu-id="6288a-911">`feedback` zur Anzeige von Metadaten zu den zuletzt ausgeführten Befehlen geändert</span><span class="sxs-lookup"><span data-stu-id="6288a-911">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="6288a-912">`feedback` geändert, um den Benutzer zur Unterstützung beim Issueerstellungsprozess aufzufordern (durch Öffnen eines Browsers und Verwenden einer Issuevorlage)</span><span class="sxs-lookup"><span data-stu-id="6288a-912">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="6288a-913">`feedback` geändert, um den Issuetext bei der Ausführung mit „--verbose“ auszugeben</span><span class="sxs-lookup"><span data-stu-id="6288a-913">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="6288a-914">Überwachen</span><span class="sxs-lookup"><span data-stu-id="6288a-914">Monitor</span></span>
* <span data-ttu-id="6288a-915">Problem behoben, aufgrund dessen „Count“ kein zulässiger Wert für `metrics alert [create|update]` war</span><span class="sxs-lookup"><span data-stu-id="6288a-915">Fixed issue where "count" was not a permitted value with `metrics alert [create|update]`</span></span> 

### <a name="network"></a><span data-ttu-id="6288a-916">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6288a-916">Network</span></span>
* <span data-ttu-id="6288a-917">Problem behoben, aufgrund dessen das Tabellenformat mit `vnet-gateway list-bgp-peer-status` nicht angezeigt wurde</span><span class="sxs-lookup"><span data-stu-id="6288a-917">Fixed table format not displaying with `vnet-gateway list-bgp-peer-status`</span></span>
* <span data-ttu-id="6288a-918">Befehle `list-request-headers` und `list-response-headers` zu `application-gateway rewrite-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-918">Added `list-request-headers` and `list-response-headers` commands to `application-gateway rewrite-rule`</span></span>
* <span data-ttu-id="6288a-919">Befehl `list-server-variables` zu `application-gateway rewrite-rule condition` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-919">Added `list-server-variables` command to `application-gateway rewrite-rule condition`</span></span>
* <span data-ttu-id="6288a-920">Problem behoben, aufgrund dessen durch das Aktualisieren des Linkstatus für einen ExpressRoute-Port eine Ausnahme vom Typ „unbekanntes Attribut“ ausgelöst wurde: `express-route port update`</span><span class="sxs-lookup"><span data-stu-id="6288a-920">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception `express-route port update`</span></span>

### <a name="privatedns"></a><span data-ttu-id="6288a-921">PrivateDNS</span><span class="sxs-lookup"><span data-stu-id="6288a-921">PrivateDNS</span></span>
* <span data-ttu-id="6288a-922">`network private-dns` für private DNS-Zonen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-922">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="6288a-923">Resource</span><span class="sxs-lookup"><span data-stu-id="6288a-923">Resource</span></span>
* <span data-ttu-id="6288a-924">Problem mit `deployment create` und `group deployment create` behoben, aufgrund dessen eine Parameterdatei mit leerem Parametersatz nicht verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="6288a-924">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="6288a-925">Role</span><span class="sxs-lookup"><span data-stu-id="6288a-925">Role</span></span>
* <span data-ttu-id="6288a-926">`create-for-rbac` korrigiert, um `--years` korrekt zu verarbeiten</span><span class="sxs-lookup"><span data-stu-id="6288a-926">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="6288a-927">[BREAKING CHANGE]`role assignment delete` geändert, um eine Eingabeaufforderung anzuzeigen, wenn alle Zuweisungen im Abonnement ohne Bedingungen gelöscht werden</span><span class="sxs-lookup"><span data-stu-id="6288a-927">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="6288a-928">SQL</span><span class="sxs-lookup"><span data-stu-id="6288a-928">SQL</span></span>
* <span data-ttu-id="6288a-929">`sql mi [create|update]` mit den Eigenschaften „proxyOverride“ und „publicDataEndpointEnabled“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="6288a-929">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="6288a-930">Storage</span><span class="sxs-lookup"><span data-stu-id="6288a-930">Storage</span></span>
* <span data-ttu-id="6288a-931">[BREAKING CHANGE] Ergebnis von `storage blob delete` entfernt</span><span class="sxs-lookup"><span data-stu-id="6288a-931">[BREAKING CHANGE] Removed result of `storage blob delete`</span></span>
* <span data-ttu-id="6288a-932">`--full-uri` zu `storage blob generate-sas` hinzugefügt, um den vollständigen URI für das Blob mit SAS zu erstellen</span><span class="sxs-lookup"><span data-stu-id="6288a-932">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="6288a-933">`--file-snapshot` zu `storage file copy start` hinzugefügt, um die Datei aus der Momentaufnahme zu kopieren</span><span class="sxs-lookup"><span data-stu-id="6288a-933">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="6288a-934">`storage blob copy cancel` geändert, um anstelle der Ausnahme für „NoPendingCopyOperation“ nur den Fehler anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="6288a-934">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="6288a-935">26. März 2019</span><span class="sxs-lookup"><span data-stu-id="6288a-935">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="6288a-936">Core</span><span class="sxs-lookup"><span data-stu-id="6288a-936">Core</span></span>
* <span data-ttu-id="6288a-937">Probleme mit der Inkompatibilität der Entwicklungserweiterung behoben</span><span class="sxs-lookup"><span data-stu-id="6288a-937">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="6288a-938">Die Fehlerbehandlung verweist Kunden jetzt auf die Problemseite.</span><span class="sxs-lookup"><span data-stu-id="6288a-938">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="6288a-939">Cloud</span><span class="sxs-lookup"><span data-stu-id="6288a-939">Cloud</span></span>
* <span data-ttu-id="6288a-940">Fehler „Abonnement nicht gefunden“ in `cloud set` behoben</span><span class="sxs-lookup"><span data-stu-id="6288a-940">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="6288a-941">ACR</span><span class="sxs-lookup"><span data-stu-id="6288a-941">ACR</span></span>
* <span data-ttu-id="6288a-942">Redundante Quellen im Imageimport korrigiert</span><span class="sxs-lookup"><span data-stu-id="6288a-942">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="6288a-943">`--auth-mode` wurde den Befehlen `acr build`, `acr run`, `acr task create` und `acr task update` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-943">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="6288a-944">Befehlsgruppe „acr task credential“ zum Verwalten von Anmeldeinformationen für eine Aufgabe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-944">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="6288a-945">„--no-wait“ zum Befehl `acr build` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-945">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="6288a-946">AppService</span><span class="sxs-lookup"><span data-stu-id="6288a-946">AppService</span></span>
* <span data-ttu-id="6288a-947">Problem behoben, das dazu führte, dass die Ausführung aus einem leeren Verzeichnis oder ein Szenario mit unbekannten Code von `webapp up` nicht korrekt behandelt wurde</span><span class="sxs-lookup"><span data-stu-id="6288a-947">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="6288a-948">Problem behoben, aufgrund dessen Slots für `[webapp|functionapp] config ssl bind` nicht verwendet werden konnten</span><span class="sxs-lookup"><span data-stu-id="6288a-948">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="6288a-949">Bot Service</span><span class="sxs-lookup"><span data-stu-id="6288a-949">BOT Service</span></span>
* <span data-ttu-id="6288a-950">`bot prepare-deploy` hinzugefügt, um die Bereitstellung von Bots über `webapp` vorzubereiten</span><span class="sxs-lookup"><span data-stu-id="6288a-950">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="6288a-951">`bot create --kind registration` geändert, um das Kennwort anzuzeigen, falls kein Kennwort angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="6288a-951">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="6288a-952">[BREAKING CHANGE]`--endpoint` wurde in `bot create --kind registration` geändert, sodass nun standardmäßig eine leere Zeichenfolge verwendet wird, anstatt eine Angabe zu erfordern.</span><span class="sxs-lookup"><span data-stu-id="6288a-952">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="6288a-953">`SCM_DO_BUILD_DURING_DEPLOYMENT` zu den Anwendungseinstellungen der ARM-Vorlage für Web-App-Bot (v4) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-953">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="6288a-954">CDN</span><span class="sxs-lookup"><span data-stu-id="6288a-954">CDN</span></span>
* <span data-ttu-id="6288a-955">Unterstützung für `--no-wait` zu `cdn endpoint [create|update|start|stop|delete|load|purge]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-955">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* <span data-ttu-id="6288a-956">[BREAKING CHANGE] Das standardmäßige Zwischenspeicherverhalten für Abfragezeichenfolgen von `cdn endpoint create` wurde geändert.</span><span class="sxs-lookup"><span data-stu-id="6288a-956">[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour.</span></span> <span data-ttu-id="6288a-957">Es wird nicht mehr standardmäßig „IgnoreQueryString“ festgelegt.</span><span class="sxs-lookup"><span data-stu-id="6288a-957">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="6288a-958">Er wird jetzt vom Dienst festgelegt.</span><span class="sxs-lookup"><span data-stu-id="6288a-958">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="6288a-959">Cosmosdb</span><span class="sxs-lookup"><span data-stu-id="6288a-959">Cosmosdb</span></span>
* <span data-ttu-id="6288a-960">Unterstützung für `--enable-multiple-write-locations` bei Kontoaktualisierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-960">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="6288a-961">Untergruppe `network-rule` mit Befehlen `add`, `remove` und `list` zum Verwalten von VNET-Regeln eines Cosmos DB-Kontos hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-961">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="6288a-962">Interactive</span><span class="sxs-lookup"><span data-stu-id="6288a-962">Interactive</span></span>
* <span data-ttu-id="6288a-963">Inkompatibilität mit der über azdev installierten interaktiven Erweiterung korrigiert</span><span class="sxs-lookup"><span data-stu-id="6288a-963">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="6288a-964">Überwachen</span><span class="sxs-lookup"><span data-stu-id="6288a-964">Monitor</span></span>
* <span data-ttu-id="6288a-965">Geändert, sodass der Dimensionswert `*` für `monitor metrics alert [create|update]` zulässig ist</span><span class="sxs-lookup"><span data-stu-id="6288a-965">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="6288a-966">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6288a-966">Network</span></span>
* <span data-ttu-id="6288a-967">Befehlsgruppe `rewrite-rule` zu `application-gateway` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-967">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="6288a-968">Profil</span><span class="sxs-lookup"><span data-stu-id="6288a-968">Profile</span></span>
* <span data-ttu-id="6288a-969">Kontounterstützung auf Mandantenebene für verwaltete Dienstidentität zu `login` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-969">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="6288a-970">Postgres</span><span class="sxs-lookup"><span data-stu-id="6288a-970">Postgres</span></span> 
* <span data-ttu-id="6288a-971">postgresql-Befehle vom Typ `replica` und Befehl `restart server` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-971">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="6288a-972">Änderungen vorgenommen, um den Standardspeicherort aus der Ressourcengruppe abzurufen, wenn er für die Erstellung von Servern nicht angegeben wurde, und um eine Überprüfung für die Aufbewahrungstage hinzuzufügen</span><span class="sxs-lookup"><span data-stu-id="6288a-972">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="6288a-973">Resource</span><span class="sxs-lookup"><span data-stu-id="6288a-973">Resource</span></span>
* <span data-ttu-id="6288a-974">Verbesserte Tabellenausgabe für `deployment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="6288a-974">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="6288a-975">Problem mit `deployment [create|validate]` behoben, aufgrund dessen der Typ „secureObject“ nicht erkannt wurde</span><span class="sxs-lookup"><span data-stu-id="6288a-975">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="6288a-976">Graph</span><span class="sxs-lookup"><span data-stu-id="6288a-976">Graph</span></span>
* <span data-ttu-id="6288a-977">Unterstützung für `--end-date` zu `ad [app|sp] credential reset` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-977">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="6288a-978">Unterstützung für das Hinzufügen von Berechtigungen mit `ad app permission add` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-978">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="6288a-979">Fehler mit `ad app permission list` behoben, wenn keine Berechtigungen vorlagen</span><span class="sxs-lookup"><span data-stu-id="6288a-979">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="6288a-980">Änderung an `ad sp delete` vorgenommen, um das Entfernen einer Rollenzuweisung zu überspringen, wenn das aktuelle Konto kein Abonnement enthält</span><span class="sxs-lookup"><span data-stu-id="6288a-980">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="6288a-981">`ad app create` geändert, sodass ohne Angabe für `--identifier-uris` standardmäßig eine leere Liste verwendet wird</span><span class="sxs-lookup"><span data-stu-id="6288a-981">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="6288a-982">storage</span><span class="sxs-lookup"><span data-stu-id="6288a-982">storage</span></span>
* <span data-ttu-id="6288a-983">`--snapshot` zu `storage file download-batch` für den Download von einer Freigabemomentaufnahme hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-983">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="6288a-984">Statusanzeige für `storage blob [download-batch|upload-batch]` geändert, damit sie weniger ausführlich dargestellt wird und das aktuelle Blob angibt</span><span class="sxs-lookup"><span data-stu-id="6288a-984">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="6288a-985">Problem mit `storage account update` behoben, das beim Aktualisieren von Verschlüsselungsparametern auftrat</span><span class="sxs-lookup"><span data-stu-id="6288a-985">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="6288a-986">Problem behoben, bei dem für `storage blob show` ein Fehler auftrat, wenn oauth (`--auth-mode=login`) verwendet wurde</span><span class="sxs-lookup"><span data-stu-id="6288a-986">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="6288a-987">VM</span><span class="sxs-lookup"><span data-stu-id="6288a-987">VM</span></span>
* <span data-ttu-id="6288a-988">Befehl `image update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-988">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="6288a-989">12. März 2019</span><span class="sxs-lookup"><span data-stu-id="6288a-989">March 12, 2019</span></span>

<span data-ttu-id="6288a-990">Version 2.0.60</span><span class="sxs-lookup"><span data-stu-id="6288a-990">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="6288a-991">Core</span><span class="sxs-lookup"><span data-stu-id="6288a-991">Core</span></span>

* <span data-ttu-id="6288a-992">Falsche Fehlermeldung in `cloud set` zu nicht gefundenem Abonnement korrigiert</span><span class="sxs-lookup"><span data-stu-id="6288a-992">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="6288a-993">ACR</span><span class="sxs-lookup"><span data-stu-id="6288a-993">ACR</span></span>

* <span data-ttu-id="6288a-994">Redundante Quellen im Imageimport korrigiert</span><span class="sxs-lookup"><span data-stu-id="6288a-994">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="6288a-995">ACS</span><span class="sxs-lookup"><span data-stu-id="6288a-995">ACS</span></span>

* <span data-ttu-id="6288a-996">Änderung vorgenommen, um den Parameter `--listen-address` für `aks browse` zu ignorieren, wenn er nicht von kubectl unterstützt wird</span><span class="sxs-lookup"><span data-stu-id="6288a-996">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="6288a-997">AppService</span><span class="sxs-lookup"><span data-stu-id="6288a-997">AppService</span></span>

* <span data-ttu-id="6288a-998">`[webapp|functionapp] deployment list-publishing-credentials` hinzugefügt, um die Kudu-Veröffentlichungs-URL und die entsprechenden Anmeldeinformationen abzurufen</span><span class="sxs-lookup"><span data-stu-id="6288a-998">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="6288a-999">Fehlerhafte Ausgabeanweisung für `webapp auth update` entfernt</span><span class="sxs-lookup"><span data-stu-id="6288a-999">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="6288a-1000">`functionapp` korrigiert, um das korrekte Image für die Runtime in App Service-Plänen unter Linux festzulegen</span><span class="sxs-lookup"><span data-stu-id="6288a-1000">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="6288a-1001">Vorschau-Tag für `webapp up` entfernt und Verbesserungen am Befehl implementiert</span><span class="sxs-lookup"><span data-stu-id="6288a-1001">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="6288a-1002">Botservice</span><span class="sxs-lookup"><span data-stu-id="6288a-1002">Botservice</span></span>

* <span data-ttu-id="6288a-1003">`SCM_DO_BUILD_DURING_DEPLOYMENT` zu den Anwendungseinstellungen der ARM-Vorlage für Web-App-Bot (v4) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1003">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="6288a-1004">`Microsoft-BotFramework-AppId` und `Microsoft-BotFramework-AppPassword` zu den Anwendungseinstellungen der ARM-Vorlage für Web-App-Bot (v4) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1004">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="6288a-1005">Einfache Anführungszeichen aus der Befehlsausgabe von `bot publish` am Ende von `bot create` entfernt</span><span class="sxs-lookup"><span data-stu-id="6288a-1005">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="6288a-1006">`bot publish` wurde geändert und ist jetzt asynchron.</span><span class="sxs-lookup"><span data-stu-id="6288a-1006">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="6288a-1007">Container</span><span class="sxs-lookup"><span data-stu-id="6288a-1007">Container</span></span>

* <span data-ttu-id="6288a-1008">Argument `--no-wait` zu `container [start|restart]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1008">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="6288a-1009">EventHub</span><span class="sxs-lookup"><span data-stu-id="6288a-1009">EventHub</span></span>

* <span data-ttu-id="6288a-1010">Flag `--skip-empty-archives` zu `eventhub create|update` hinzugefügt, um leere Archive in der Aufzeichnung zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="6288a-1010">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="6288a-1011">Suchen</span><span class="sxs-lookup"><span data-stu-id="6288a-1011">Find</span></span>

* <span data-ttu-id="6288a-1012">Umfangreiches Funktionsupdate</span><span class="sxs-lookup"><span data-stu-id="6288a-1012">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="6288a-1013">HDInsight</span><span class="sxs-lookup"><span data-stu-id="6288a-1013">HDInsight</span></span>

* <span data-ttu-id="6288a-1014">Parameter `--storage-account-managed-identity` zu `hdinsight create` hinzugefügt, um MSI in ADLS Gen2 zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="6288a-1014">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="6288a-1015">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6288a-1015">Network</span></span>

* <span data-ttu-id="6288a-1016">Problem mit `vpn-connection update` behoben, aufgrund dessen die Aktualisierung einer VPN-Verbindung zwischen Gateways in verschiedenen Abonnements fehlschlug</span><span class="sxs-lookup"><span data-stu-id="6288a-1016">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="6288a-1017">Rdbms</span><span class="sxs-lookup"><span data-stu-id="6288a-1017">Rdbms</span></span>

* <span data-ttu-id="6288a-1018">Kleinere Korrekturen, um den Standardspeicherort aus der Ressourcengruppe abzurufen, wenn er für die Erstellung von Servern nicht angegeben wurde, und um eine Überprüfung für die Aufbewahrungstage hinzuzufügen</span><span class="sxs-lookup"><span data-stu-id="6288a-1018">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="6288a-1019">Role</span><span class="sxs-lookup"><span data-stu-id="6288a-1019">Role</span></span>

* <span data-ttu-id="6288a-1020">`role definition update` wurde korrigiert und nutzt nun die ID, um die Definition korrekt aufzulösen.</span><span class="sxs-lookup"><span data-stu-id="6288a-1020">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="6288a-1021">`ad app credential reset` geändert, um die Annahme zu entfernen, dass der Dienstprinzipal der App stets vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="6288a-1021">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="6288a-1022">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="6288a-1022">Service Fabric</span></span>

* <span data-ttu-id="6288a-1023">Das Problem, dass `sf cluster list` nicht wiederholbar war, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="6288a-1023">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="6288a-1024">26. Februar 2019</span><span class="sxs-lookup"><span data-stu-id="6288a-1024">February 26, 2019</span></span>

<span data-ttu-id="6288a-1025">Version 2.0.59</span><span class="sxs-lookup"><span data-stu-id="6288a-1025">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="6288a-1026">Core</span><span class="sxs-lookup"><span data-stu-id="6288a-1026">Core</span></span>

* <span data-ttu-id="6288a-1027">Problem behoben, aufgrund dessen die Verwendung von `--subscription NAME` in einigen Instanzen eine Ausnahme ausgelöst hat</span><span class="sxs-lookup"><span data-stu-id="6288a-1027">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="6288a-1028">ACR</span><span class="sxs-lookup"><span data-stu-id="6288a-1028">ACR</span></span>

* <span data-ttu-id="6288a-1029">Parameter `--target` für die Befehle `acr build`, `acr task create` und `acr task update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1029">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="6288a-1030">Verbesserte Fehlerbehandlung für Runtimebefehle, wenn keine Anmeldung bei Azure besteht</span><span class="sxs-lookup"><span data-stu-id="6288a-1030">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="6288a-1031">ACS</span><span class="sxs-lookup"><span data-stu-id="6288a-1031">ACS</span></span>

* <span data-ttu-id="6288a-1032">Option `--listen-address` zu `aks port-forward` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1032">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="6288a-1033">AppService</span><span class="sxs-lookup"><span data-stu-id="6288a-1033">AppService</span></span>

* <span data-ttu-id="6288a-1034">Befehl `functionapp devops-build` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1034">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="6288a-1035">Batch</span><span class="sxs-lookup"><span data-stu-id="6288a-1035">Batch</span></span>
* <span data-ttu-id="6288a-1036">[BREAKING CHANGE] Befehl `batch pool upgrade os` entfernt</span><span class="sxs-lookup"><span data-stu-id="6288a-1036">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="6288a-1037">[BREAKING CHANGE]`Pacakges`-Eigenschaft aus `Application`-Antworten entfernt</span><span class="sxs-lookup"><span data-stu-id="6288a-1037">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="6288a-1038">Befehl `batch application package list` zum Auflisten von Paketen einer Anwendung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1038">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="6288a-1039">[BREAKING CHANGE]`--application-id` in allen `batch application`-Befehlen in `--application-name` geändert</span><span class="sxs-lookup"><span data-stu-id="6288a-1039">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="6288a-1040">Argument `--json-file` für Befehle zum Anfordern der unformatierten API-Antwort hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1040">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="6288a-1041">Validierung aktualisiert, sodass das `https://`-Element automatisch in alle Endpunkte aufgenommen wird, wenn es fehlt</span><span class="sxs-lookup"><span data-stu-id="6288a-1041">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="6288a-1042">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="6288a-1042">CosmosDB</span></span>

* <span data-ttu-id="6288a-1043">Untergruppe `network-rule` mit Befehlen `add`, `remove` und `list` zum Verwalten von VNET-Regeln eines Cosmos DB-Kontos hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1043">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="6288a-1044">Kusto</span><span class="sxs-lookup"><span data-stu-id="6288a-1044">Kusto</span></span>

* <span data-ttu-id="6288a-1045">[BREAKING CHANGE] Typen `hot_cache_period` und `soft_delete_period` für Datenbank in Format der Zeitspanne nach ISO8601 geändert</span><span class="sxs-lookup"><span data-stu-id="6288a-1045">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="6288a-1046">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6288a-1046">Network</span></span>

* <span data-ttu-id="6288a-1047">Argument `--express-route-gateway-bypass` zu `vpn-connection [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1047">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="6288a-1048">Befehlsgruppen aus `express-route`-Erweiterungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1048">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="6288a-1049">Befehlsgruppen `express-route gateway` und `express-route port` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1049">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="6288a-1050">Argument `--legacy-mode` zu `express-route peering [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1050">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="6288a-1051">Argumente `--allow-classic-operations` und `--express-route-port` zu `express-route [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1051">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="6288a-1052">Argument `--gateway-default-site` zu `vnet-gateway [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1052">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="6288a-1053">Befehle vom Typ `ipsec-policy` zu `vnet-gateway` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1053">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="6288a-1054">Resource</span><span class="sxs-lookup"><span data-stu-id="6288a-1054">Resource</span></span>

* <span data-ttu-id="6288a-1055">Problem mit `deployment create` behoben, aufgrund dessen beim Feld „Typ“ die Groß-/Kleinschreibung beachtet wurde</span><span class="sxs-lookup"><span data-stu-id="6288a-1055">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="6288a-1056">Unterstützung für URI-basierte Parameterdatei zu `policy assignment create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1056">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="6288a-1057">Unterstützung für URI-basierte Parameter und Definitionen zu `policy set-definition update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1057">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="6288a-1058">Verarbeitung von Parametern und Regeln für `policy definition update` korrigiert</span><span class="sxs-lookup"><span data-stu-id="6288a-1058">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="6288a-1059">Problem mit `resource show/update/delete/tag/invoke-action` behoben, aufgrund dessen bei abonnementübergreifenden IDs die Abonnement-ID nicht ordnungsgemäß berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="6288a-1059">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="6288a-1060">Role</span><span class="sxs-lookup"><span data-stu-id="6288a-1060">Role</span></span>

* <span data-ttu-id="6288a-1061">Unterstützung für App-Rollen zu `ad app [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1061">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="6288a-1062">VM</span><span class="sxs-lookup"><span data-stu-id="6288a-1062">VM</span></span>

* <span data-ttu-id="6288a-1063">Problem mit `vm create where ` behoben, aufgrund dessen der beschleunigte Netzwerkbetrieb für Ubuntu 18.0 nicht standardmäßig aktiviert war</span><span class="sxs-lookup"><span data-stu-id="6288a-1063">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="6288a-1064">12. Februar 2019</span><span class="sxs-lookup"><span data-stu-id="6288a-1064">February 12, 2019</span></span>

<span data-ttu-id="6288a-1065">Version 2.0.58</span><span class="sxs-lookup"><span data-stu-id="6288a-1065">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="6288a-1066">Core</span><span class="sxs-lookup"><span data-stu-id="6288a-1066">Core</span></span>

* <span data-ttu-id="6288a-1067">`az --version` zeigt jetzt eine Benachrichtigung an, wenn Sie Pakete haben, für die ein Update verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="6288a-1067">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="6288a-1068">Die Regression, dass `--ids` nicht mehr mit JSON-Ausgaben verwendet werden konnte, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="6288a-1068">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="6288a-1069">ACR</span><span class="sxs-lookup"><span data-stu-id="6288a-1069">ACR</span></span>
* <span data-ttu-id="6288a-1070">[BREAKING CHANGE] Die Befehlsgruppe `acr build-task` wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="6288a-1070">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="6288a-1071">[BREAKING CHANGE] Die Optionen `--tag` und `--manifest` wurden aus `acr repository delete` entfernt.</span><span class="sxs-lookup"><span data-stu-id="6288a-1071">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="6288a-1072">ACS</span><span class="sxs-lookup"><span data-stu-id="6288a-1072">ACS</span></span>
* <span data-ttu-id="6288a-1073">Unterstützung für Namen ohne Berücksichtigung von Groß-/Kleinschreibung wurde zu `aks [enable-addons|disable-addons]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-1073">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="6288a-1074">Unterstützung für Azure Active Directory-Aktualisierungsvorgang mithilfe von `aks update-credentials --reset-aad` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-1074">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="6288a-1075">Die Information, dass `--output` für `aks get-credentials` ignoriert wird, wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-1075">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="6288a-1076">AMS</span><span class="sxs-lookup"><span data-stu-id="6288a-1076">AMS</span></span>
* <span data-ttu-id="6288a-1077">Befehle vom Typ `ams streaming-endpoint [start | stop | create | update] wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1077">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="6288a-1078">Befehle vom Typ `ams live-event [create | start | stop | reset] wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1078">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="6288a-1079">AppService</span><span class="sxs-lookup"><span data-stu-id="6288a-1079">Appservice</span></span>
* <span data-ttu-id="6288a-1080">Die Möglichkeit zum Erstellen und Konfigurieren von Funktionen mithilfe von ACR-Containern wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-1080">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="6288a-1081">Unterstützung für das Aktualisieren von Web-App-Konfigurationen über JSON wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-1081">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="6288a-1082">Die Hilfe für `appservice-plan-update` wurde verbessert.</span><span class="sxs-lookup"><span data-stu-id="6288a-1082">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="6288a-1083">Unterstützung für App-Erkenntnisse beim Erstellen von Funktions-Apps wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-1083">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="6288a-1084">Probleme mit der Web-App SSH wurden behoben.</span><span class="sxs-lookup"><span data-stu-id="6288a-1084">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="6288a-1085">Botservice</span><span class="sxs-lookup"><span data-stu-id="6288a-1085">Botservice</span></span>
* <span data-ttu-id="6288a-1086">Die Benutzeroberfläche für `bot publish` wurde verbessert.</span><span class="sxs-lookup"><span data-stu-id="6288a-1086">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="6288a-1087">Eine Warnung für Zeitlimit bei der Ausführung von `npm install` während `az bot publish` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-1087">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="6288a-1088">Ungültiges char-Element wurde `.` aus `--name` in `az bot create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="6288a-1088">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="6288a-1089">Eine Änderung wurde vorgenommen, um die zufällige Zuordnung von Ressourcennamen beim Erstellen von Azure Storage-Instanzen, App Service-Plänen, Funktions-/Web-Apps und Application Insights-Instanzen zu verhindern.</span><span class="sxs-lookup"><span data-stu-id="6288a-1089">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="6288a-1090">[VERALTET] Argument `--proj-name` zugunsten von `--proj-file-path` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="6288a-1090">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="6288a-1091">`az bot publish` wurde geändert, um abgerufene IIS-Bereitstellungsdateien vom Typ „Node.js“ zu entfernen, wenn sie nicht bereits vorhanden waren.</span><span class="sxs-lookup"><span data-stu-id="6288a-1091">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="6288a-1092">Das `--keep-node-modules` Argument wurde zu `az bot publish` hinzugefügt, damit der Ordner `node_modules` in App Service nicht gelöscht wird.</span><span class="sxs-lookup"><span data-stu-id="6288a-1092">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="6288a-1093">Das Schlüssel-Wert-Paar `"publishCommand"` wurde der Ausgabe von `az bot create` beim Erstellen einer Funktions-App oder eines Web-App-Bots hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-1093">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="6288a-1094">Der Wert von `"publishCommand"` ist ein `az bot publish`-Befehl, der bereits die erforderlichen Parameter zum Veröffentlichen des neu erstellten Bots enthält.</span><span class="sxs-lookup"><span data-stu-id="6288a-1094">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="6288a-1095">`"WEBSITE_NODE_DEFAULT_VERSION"` in der ARM-Vorlage wurde so aktualisiert, dass v4-SDK-Bots 10.14.1 anstelle von 8.9.4 verwenden.</span><span class="sxs-lookup"><span data-stu-id="6288a-1095">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="6288a-1096">Key Vault</span><span class="sxs-lookup"><span data-stu-id="6288a-1096">Key Vault</span></span>
* <span data-ttu-id="6288a-1097">Ein Problem mit `keyvault secret backup` wurde behoben, aufgrund dessen einige Benutzer bei Verwendung von `--id` einen `unexpected_keyword`-Fehler erhielten.</span><span class="sxs-lookup"><span data-stu-id="6288a-1097">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="6288a-1098">Überwachen</span><span class="sxs-lookup"><span data-stu-id="6288a-1098">Monitor</span></span>
* <span data-ttu-id="6288a-1099">`monitor metrics alert [create|update]` wurde so geändert, dass der Dimensionswert `*` zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="6288a-1099">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="6288a-1100">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6288a-1100">Network</span></span>
* <span data-ttu-id="6288a-1101">`dns zone export` wurde geändert, um sicherzustellen, dass es sich bei exportierten CNAMEs um FQDNs handelt.</span><span class="sxs-lookup"><span data-stu-id="6288a-1101">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="6288a-1102">Parameter `--gateway-name` wurde zu `nic ip-config address-pool [add|remove]` hinzugefügt, um Back-End-Adresspools von Anwendungsgateways zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="6288a-1102">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="6288a-1103">Argumente `--traffic-analytics` und `--workspace` wurden zu `network watcher flow-log configure` hinzugefügt, um Datenverkehrsanalysen über einen Log Analytics-Arbeitsbereich zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="6288a-1103">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="6288a-1104">`--idle-timeout` und `--floating-ip` wurden zu `lb inbound-nat-pool [create|update]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-1104">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="6288a-1105">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="6288a-1105">Policy Insights</span></span>
* <span data-ttu-id="6288a-1106">`policy remediation`-Befehle wurden hinzugefügt, um Korrekturfunktionen der Ressourcenrichtlinie zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="6288a-1106">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="6288a-1107">RDBMS</span><span class="sxs-lookup"><span data-stu-id="6288a-1107">RDBMS</span></span>
* <span data-ttu-id="6288a-1108">Hilfemeldung und Befehlsparameter wurden verbessert.</span><span class="sxs-lookup"><span data-stu-id="6288a-1108">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="6288a-1109">Redis</span><span class="sxs-lookup"><span data-stu-id="6288a-1109">Redis</span></span>
* <span data-ttu-id="6288a-1110">Befehle zum Verwalten von „firewall-rules“ (erstellen, aktualisieren, löschen, anzeigen, auflisten) wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-1110">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="6288a-1111">Befehle zum Verwalten von „server-link“ (erstellen, aktualisieren, löschen, anzeigen, auflisten) wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-1111">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="6288a-1112">Befehle zum Verwalten von „patch-schedule“ (erstellen, aktualisieren, löschen, anzeigen, auflisten) wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-1112">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="6288a-1113">Unterstützung für Verfügbarkeitszonen und TLS-Mindestversion wurden zu „redis create“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-1113">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="6288a-1114">[BREAKING CHANGE] Befehle `redis update-settings` und `redis list-all` wurden entfernt.</span><span class="sxs-lookup"><span data-stu-id="6288a-1114">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="6288a-1115">[BREAKING CHANGE] Parameter für `redis create`: „Mandanteneinstellungen“ werden im Format „Schlüssel[=Wert] nicht akzeptiert.</span><span class="sxs-lookup"><span data-stu-id="6288a-1115">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="6288a-1116">[VERALTET] Warnmeldung zur Markierung des Befehls `redis import-method` als veraltet hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1116">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="6288a-1117">Role</span><span class="sxs-lookup"><span data-stu-id="6288a-1117">Role</span></span>
* <span data-ttu-id="6288a-1118">[BREAKING CHANGE] Befehl `az identity` wurde aus den `vm`-Befehlen hierher verschoben.</span><span class="sxs-lookup"><span data-stu-id="6288a-1118">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="6288a-1119">SQL-VM</span><span class="sxs-lookup"><span data-stu-id="6288a-1119">SQL VM</span></span>
* <span data-ttu-id="6288a-1120">[VERALTET] Argument `--boostrap-acc-pwd` aufgrund eines Tippfehlers als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="6288a-1120">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="6288a-1121">VM</span><span class="sxs-lookup"><span data-stu-id="6288a-1121">VM</span></span>
* <span data-ttu-id="6288a-1122">`vm list-skus` wurde so geändert, dass `--all` anstelle von `--all true` verwendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="6288a-1122">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="6288a-1123">`vmss run-command [invoke | list | show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1123">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="6288a-1124">Ein Fehler wurde behoben, aufgrund dessen bei der Ausführung von `vmss encryption enable` bisher ein Fehler auftrat.</span><span class="sxs-lookup"><span data-stu-id="6288a-1124">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="6288a-1125">[BREAKING CHANGE] Die Befehle vom Typ `az identity` wurden zu `role`-Befehlen verschoben.</span><span class="sxs-lookup"><span data-stu-id="6288a-1125">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="6288a-1126">31. Januar 2019</span><span class="sxs-lookup"><span data-stu-id="6288a-1126">January 31, 2019</span></span>

<span data-ttu-id="6288a-1127">Version 2.0.57</span><span class="sxs-lookup"><span data-stu-id="6288a-1127">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="6288a-1128">Core</span><span class="sxs-lookup"><span data-stu-id="6288a-1128">Core</span></span>

* <span data-ttu-id="6288a-1129">Hotfix für [Problem 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="6288a-1129">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="6288a-1130">28. Januar 2019</span><span class="sxs-lookup"><span data-stu-id="6288a-1130">January 28, 2019</span></span>

<span data-ttu-id="6288a-1131">Version 2.0.56</span><span class="sxs-lookup"><span data-stu-id="6288a-1131">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="6288a-1132">ACR</span><span class="sxs-lookup"><span data-stu-id="6288a-1132">ACR</span></span>
* <span data-ttu-id="6288a-1133">Unterstützung für VNet/IP-Regeln wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-1133">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="6288a-1134">ACS</span><span class="sxs-lookup"><span data-stu-id="6288a-1134">ACS</span></span>
* <span data-ttu-id="6288a-1135">Virtuelle Knoten (Vorschau) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1135">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="6288a-1136">Verwaltete OpenShift-Befehle wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-1136">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="6288a-1137">Unterstützung für den Dienstprinzipal-Updatevorgang mit `aks update-credentials -reset-service-principal` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-1137">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="6288a-1138">AMS</span><span class="sxs-lookup"><span data-stu-id="6288a-1138">AMS</span></span>
* <span data-ttu-id="6288a-1139">[BREAKING CHANGE]`ams asset get-streaming-locators` in `ams asset list-streaming-locators` umbenannt</span><span class="sxs-lookup"><span data-stu-id="6288a-1139">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="6288a-1140">[BREAKING CHANGE]`ams streaming-locator get-content-keys` in `ams streaming-locator list-content-keys` umbenannt</span><span class="sxs-lookup"><span data-stu-id="6288a-1140">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="6288a-1141">AppService</span><span class="sxs-lookup"><span data-stu-id="6288a-1141">Appservice</span></span>
* <span data-ttu-id="6288a-1142">Unterstützung für App-Erkenntnisse in `functionapp create` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-1142">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="6288a-1143">Unterstützung für die Erstellung von App Service-Plänen (einschließlich Elastic Premium) wurde zu Funktions-Apps hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-1143">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="6288a-1144">Probleme bei einer App-Einstellung mit Elastic Premium-Plänen wurden behoben.</span><span class="sxs-lookup"><span data-stu-id="6288a-1144">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="6288a-1145">Container</span><span class="sxs-lookup"><span data-stu-id="6288a-1145">Container</span></span>
* <span data-ttu-id="6288a-1146">Befehl `container start` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1146">Added `container start` command</span></span>
* <span data-ttu-id="6288a-1147">Eine Änderung wurde vorgenommen, um bei der Containererstellung die Verwendung von Dezimalwerten für die CPU zuzulassen.</span><span class="sxs-lookup"><span data-stu-id="6288a-1147">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="6288a-1148">EventGrid</span><span class="sxs-lookup"><span data-stu-id="6288a-1148">EventGrid</span></span>
* <span data-ttu-id="6288a-1149">Parameter `--deadletter-endpoint` zu `event-subscription [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1149">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="6288a-1150">„storagequeue“ und „hybridconnection“ wurden als neue Werte für „event-subscription [create|update] --endpoint-type“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-1150">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="6288a-1151">Parameter `--max-delivery-attempts` und `--event-ttl` wurden zu `event-subscription create` hinzugefügt, um die Wiederholungsrichtlinie für Ereignisse anzugeben.</span><span class="sxs-lookup"><span data-stu-id="6288a-1151">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="6288a-1152">Eine Warnmeldung wurde zu `event-subscription [create|update]` hinzugefügt, wenn Webhook als Ziel für ein Ereignisabonnement verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="6288a-1152">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="6288a-1153">Parameter „source-resource-id“ wurde für alle Befehle im Zusammenhang mit Ereignisabonnements hinzugefügt, und alle anderen Parameter im Zusammenhang mit Quellressourcen wurden als veraltet markiert.</span><span class="sxs-lookup"><span data-stu-id="6288a-1153">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="6288a-1154">HDInsight</span><span class="sxs-lookup"><span data-stu-id="6288a-1154">HDInsight</span></span>
* <span data-ttu-id="6288a-1155">[BREAKING CHANGE] Die Parameter `--virtual-network` und `--subnet-name` wurden aus `hdinsight [application] create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="6288a-1155">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="6288a-1156">[BREAKING CHANGE]`hdinsight create --storage-account` wurde so geändert, dass der Name oder die ID eines Speicherkontos anstellen von Blobendpunkten akzeptiert wird.</span><span class="sxs-lookup"><span data-stu-id="6288a-1156">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="6288a-1157">Parameter `--vnet-name` und `--subnet-name` zu `hdinsight create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1157">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="6288a-1158">Unterstützung für das Enterprise-Sicherheitspaket und Datenträgerverschlüsselung wurde zu `hdinsight create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-1158">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="6288a-1159">Befehl `hdinsight rotate-disk-encryption-key` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1159">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="6288a-1160">Befehl `hdinsight update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1160">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="6288a-1161">IoT</span><span class="sxs-lookup"><span data-stu-id="6288a-1161">IoT</span></span>
* <span data-ttu-id="6288a-1162">Codierungsformat wurde zu Befehl „routing-endpoint“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-1162">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="6288a-1163">Kusto</span><span class="sxs-lookup"><span data-stu-id="6288a-1163">Kusto</span></span>
* <span data-ttu-id="6288a-1164">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="6288a-1164">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="6288a-1165">Überwachen</span><span class="sxs-lookup"><span data-stu-id="6288a-1165">Monitor</span></span>
* <span data-ttu-id="6288a-1166">ID-Vergleich wurde so geändert, dass Groß-/Kleinschreibung nicht mehr beachtet wird.</span><span class="sxs-lookup"><span data-stu-id="6288a-1166">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="6288a-1167">Profil</span><span class="sxs-lookup"><span data-stu-id="6288a-1167">Profile</span></span>
* <span data-ttu-id="6288a-1168">Konto auf Mandantenebene für verwaltete Dienstidentität für `login` wird aktiviert.</span><span class="sxs-lookup"><span data-stu-id="6288a-1168">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="6288a-1169">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6288a-1169">Network</span></span>
* <span data-ttu-id="6288a-1170">Ein Problem mit `express-route update` wurde behoben, aufgrund dessen das Argument `--bandwidth` ignoriert wurde.</span><span class="sxs-lookup"><span data-stu-id="6288a-1170">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="6288a-1171">Ein Problem mit `ddos-protection update` wurde behoben, aufgrund dessen das festgelegte Verständnis zu einer Stapelüberwachung führte.</span><span class="sxs-lookup"><span data-stu-id="6288a-1171">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="6288a-1172">Resource</span><span class="sxs-lookup"><span data-stu-id="6288a-1172">Resource</span></span>
* <span data-ttu-id="6288a-1173">Unterstützung für die URI-Parameterdatei wurde zu `group deployment create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-1173">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="6288a-1174">Unterstützung für verwaltete Identitäten wurde zu `policy assignment [create|list|show]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-1174">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="6288a-1175">Virtueller SQL-Computer</span><span class="sxs-lookup"><span data-stu-id="6288a-1175">SQL Virtual Machine</span></span>
* <span data-ttu-id="6288a-1176">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="6288a-1176">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="6288a-1177">Storage</span><span class="sxs-lookup"><span data-stu-id="6288a-1177">Storage</span></span>
* <span data-ttu-id="6288a-1178">Eine Lösung wurde so geändert, dass nur Eigenschaften aktualisiert werden, die im selben Objekt geändert werden.</span><span class="sxs-lookup"><span data-stu-id="6288a-1178">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="6288a-1179">Nr. 8021 wurde korrigiert, Binärdaten werden bei der Rückgabe in Base64 codiert.</span><span class="sxs-lookup"><span data-stu-id="6288a-1179">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="6288a-1180">VM</span><span class="sxs-lookup"><span data-stu-id="6288a-1180">VM</span></span>
* <span data-ttu-id="6288a-1181">`vm encryption enable` wurde geändert, um den Schlüsseltresor für die Datenträgerverschlüsselung zu überprüfen und sicherzustellen, dass der Schlüsseltresor für die Schlüsselverschlüsselung vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="6288a-1181">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="6288a-1182">Flag `--force` wurde zu `vm encryption enable` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-1182">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="6288a-1183">15. Januar 2019</span><span class="sxs-lookup"><span data-stu-id="6288a-1183">January 15, 2019</span></span>

<span data-ttu-id="6288a-1184">Version 2.0.55</span><span class="sxs-lookup"><span data-stu-id="6288a-1184">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="6288a-1185">ACR</span><span class="sxs-lookup"><span data-stu-id="6288a-1185">ACR</span></span>
* <span data-ttu-id="6288a-1186">Wurde geändert, um den Push eines nicht vorhandenen Helm-Diagramms zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="6288a-1186">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="6288a-1187">Wurde geändert, um Laufzeitvorgänge ohne ARM-Anforderungen zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="6288a-1187">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="6288a-1188">[VERALTET] Parameter `--resource-group` in folgenden Befehlen als veraltet markiert:</span><span class="sxs-lookup"><span data-stu-id="6288a-1188">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="6288a-1189">ACS</span><span class="sxs-lookup"><span data-stu-id="6288a-1189">ACS</span></span>
* <span data-ttu-id="6288a-1190">Unterstützung für neue ACI-Regionen wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-1190">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="6288a-1191">AppService</span><span class="sxs-lookup"><span data-stu-id="6288a-1191">Appservice</span></span>
* <span data-ttu-id="6288a-1192">Ein Problem beim Hochladen von Zertifikaten für in einer ASE gehostete Apps wurde behoben, aufgrund dessen die AS-RG und die App-RG nicht übereinstimmten.</span><span class="sxs-lookup"><span data-stu-id="6288a-1192">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="6288a-1193">`webapp up` wurde geändert, sodass SKU P1V1 als Standard für Linux verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="6288a-1193">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="6288a-1194">`[webapp|functionapp] deployment source config-zip` wurde korrigiert, sodass beim Fehlschlagen einer Bereitstellung die richtige Fehlermeldung angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="6288a-1194">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="6288a-1195">Befehl `webapp ssh` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1195">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="6288a-1196">Botservice</span><span class="sxs-lookup"><span data-stu-id="6288a-1196">Botservice</span></span>
* <span data-ttu-id="6288a-1197">Aktualisierungen des Bereitstellungsstatus wurden zu `bot create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-1197">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="6288a-1198">Konfigurieren</span><span class="sxs-lookup"><span data-stu-id="6288a-1198">Configure</span></span>
* <span data-ttu-id="6288a-1199">`none` wurde als konfigurierbares Ausgabeformat hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-1199">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="6288a-1200">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="6288a-1200">CosmosDB</span></span>
* <span data-ttu-id="6288a-1201">Unterstützung für das Erstellen einer Datenbank mit gemeinsam genutztem Durchsatz wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-1201">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="6288a-1202">HDInsight</span><span class="sxs-lookup"><span data-stu-id="6288a-1202">HDInsight</span></span>
* <span data-ttu-id="6288a-1203">Befehle zum Verwalten von Anwendungen wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-1203">Added commands for managing applications</span></span>
* <span data-ttu-id="6288a-1204">Befehle zum Verwalten von Skriptaktionen wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-1204">Added commands for managing script actions</span></span>
* <span data-ttu-id="6288a-1205">Befehle zum Verwalten von der Operations Management Suite (OMS) wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-1205">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="6288a-1206">Unterstützung zum Auflisten der regionalen Nutzung wurde zu `hdinsight list-usage` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-1206">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="6288a-1207">[BREAKING CHANGE] Standardclustertyp wurde aus `hdinsight create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="6288a-1207">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="6288a-1208">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6288a-1208">Network</span></span>
* <span data-ttu-id="6288a-1209">Argumente `--custom-headers` und `--status-code-ranges` zu `traffic-manager profile [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1209">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="6288a-1210">Neue Routingtypen wurden hinzugefügt: Subnetz und MultiValue</span><span class="sxs-lookup"><span data-stu-id="6288a-1210">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="6288a-1211">Argumente `--custom-headers` und `--subnets` zu `traffic-manager endpoint [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1211">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="6288a-1212">Eine Problem wurde behoben, aufgrund dessen die Angabe von `--vnets ""` für `ddos-protection update` einen Fehler verursacht hat.</span><span class="sxs-lookup"><span data-stu-id="6288a-1212">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="6288a-1213">Role</span><span class="sxs-lookup"><span data-stu-id="6288a-1213">Role</span></span>
* <span data-ttu-id="6288a-1214">[VERALTET] Argument `--password` als veraltet markiert für `create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="6288a-1214">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="6288a-1215">Verwenden Sie stattdessen sichere, von der CLI generierte Kennwörter.</span><span class="sxs-lookup"><span data-stu-id="6288a-1215">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="6288a-1216">Sicherheit</span><span class="sxs-lookup"><span data-stu-id="6288a-1216">Security</span></span>
* <span data-ttu-id="6288a-1217">Erstrelease</span><span class="sxs-lookup"><span data-stu-id="6288a-1217">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="6288a-1218">Storage</span><span class="sxs-lookup"><span data-stu-id="6288a-1218">Storage</span></span>
* <span data-ttu-id="6288a-1219">[BREAKING CHANGE] Die Standardanzahl von Ergebnissen wurde für `storage [blob|file|container|share] list` in 5.000 geändert.</span><span class="sxs-lookup"><span data-stu-id="6288a-1219">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="6288a-1220">Verwenden Sie `--num-results *` für das ursprüngliche Verhalten, alle Ergebnisse zurückzugeben.</span><span class="sxs-lookup"><span data-stu-id="6288a-1220">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="6288a-1221">Parameter `--marker` zu `storage [blob|file|container|share] list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1221">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="6288a-1222">Ein Protokollmarker für die nächste Seite wurde zur STDERR für `storage [blob|file|container|share] list` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-1222">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="6288a-1223">Der Befehl `storage blob service-properties update` mit Unterstützung für statische Websites wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-1223">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="6288a-1224">VM</span><span class="sxs-lookup"><span data-stu-id="6288a-1224">VM</span></span>
* <span data-ttu-id="6288a-1225">`vm [disk|unmanaged-disk]` und `vmss disk` wurden geändert, sodass sie konsistentere Parameter enthalten.</span><span class="sxs-lookup"><span data-stu-id="6288a-1225">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="6288a-1226">Unterstützung für mandantenübergreifende Imageverweise wurden zu `[vm|vmss] create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-1226">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="6288a-1227">Fehler bei Standardkonfiguration in `vm diagnostics get-default-config --windows-os` wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="6288a-1227">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="6288a-1228">Argument `--provision-after-extensions` wurde zu `vmss extension set` hinzugefügt, um zu definieren, welche Erweiterungen vor dem Festlegen der Erweiterung bereitgestellt werden müssen.</span><span class="sxs-lookup"><span data-stu-id="6288a-1228">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="6288a-1229">Argument `--replica-count` wurde zu `sig image-version update` hinzugefügt, um die Standardanzahl für die Replikation festzulegen.</span><span class="sxs-lookup"><span data-stu-id="6288a-1229">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="6288a-1230">Fehler bei `image create --source` wurde behoben, aufgrund dessen, der Quellbetriebssystem-Datenträger für einen virtuellen Computer mit dem gleichen Namen gehalten wurde, selbst wenn die vollständige Ressourcen-ID angegeben war.</span><span class="sxs-lookup"><span data-stu-id="6288a-1230">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="6288a-1231">20. Dezember 2018</span><span class="sxs-lookup"><span data-stu-id="6288a-1231">December 20, 2018</span></span>

<span data-ttu-id="6288a-1232">Version 2.0.54</span><span class="sxs-lookup"><span data-stu-id="6288a-1232">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="6288a-1233">AppService</span><span class="sxs-lookup"><span data-stu-id="6288a-1233">Appservice</span></span>
* <span data-ttu-id="6288a-1234">Problem behoben, bei dem `webapp up` nicht erneut bereitgestellt werden konnte</span><span class="sxs-lookup"><span data-stu-id="6288a-1234">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="6288a-1235">Unterstützung für das Auflisten und Wiederherstellen von Web-App-Momentaufnahmen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1235">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="6288a-1236">Unterstützung für das Flag `--runtime` zu Windows-Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1236">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="6288a-1237">IoTCentral</span><span class="sxs-lookup"><span data-stu-id="6288a-1237">IoTCentral</span></span>
* <span data-ttu-id="6288a-1238">Fehler bei API-Aufruf für update-Befehl behoben</span><span class="sxs-lookup"><span data-stu-id="6288a-1238">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="6288a-1239">Role</span><span class="sxs-lookup"><span data-stu-id="6288a-1239">Role</span></span>
* <span data-ttu-id="6288a-1240">[BREAKING CHANGE]`ad [app|sp] list` geändert, damit standardmäßig nur die ersten 100 Objekte aufgelistet werden</span><span class="sxs-lookup"><span data-stu-id="6288a-1240">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="6288a-1241">SQL</span><span class="sxs-lookup"><span data-stu-id="6288a-1241">SQL</span></span>
* <span data-ttu-id="6288a-1242">Unterstützung für die benutzerdefinierte Sortierung auf verwalteten Instanzen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1242">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="6288a-1243">VM</span><span class="sxs-lookup"><span data-stu-id="6288a-1243">VM</span></span>
* <span data-ttu-id="6288a-1244">Parameter `---os-type` zu `disk create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1244">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="6288a-1245">18. Dezember 2018</span><span class="sxs-lookup"><span data-stu-id="6288a-1245">December 18, 2018</span></span>

<span data-ttu-id="6288a-1246">Version 2.0.53</span><span class="sxs-lookup"><span data-stu-id="6288a-1246">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="6288a-1247">ACR</span><span class="sxs-lookup"><span data-stu-id="6288a-1247">ACR</span></span>
* <span data-ttu-id="6288a-1248">Unterstützung für Imageimport aus externen Containerregistrierungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1248">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="6288a-1249">Tabellenlayout für Aufgabenliste komprimiert</span><span class="sxs-lookup"><span data-stu-id="6288a-1249">Condensed the table layout for task list</span></span>
* <span data-ttu-id="6288a-1250">Unterstützung für Azure DevOps-URLs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1250">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="6288a-1251">ACS</span><span class="sxs-lookup"><span data-stu-id="6288a-1251">ACS</span></span>
* <span data-ttu-id="6288a-1252">Virtuelle Knoten (Vorschau) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1252">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="6288a-1253">„(PREVIEW)“ aus AAD-Argumenten für `aks create` entfernt</span><span class="sxs-lookup"><span data-stu-id="6288a-1253">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="6288a-1254">[VERALTET]`az acs`-Befehle als veraltet markiert.</span><span class="sxs-lookup"><span data-stu-id="6288a-1254">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="6288a-1255">ACS wird am 31. Januar 2020 eingestellt</span><span class="sxs-lookup"><span data-stu-id="6288a-1255">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="6288a-1256">Unterstützung für Netzwerkrichtlinie bei der Erstellung neuer AKS-Cluster hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1256">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="6288a-1257">Anforderung des Arguments `--nodepool-name` bei nur einem Knotenpool für `aks scale` entfernt</span><span class="sxs-lookup"><span data-stu-id="6288a-1257">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="6288a-1258">AppService</span><span class="sxs-lookup"><span data-stu-id="6288a-1258">Appservice</span></span>
* <span data-ttu-id="6288a-1259">Problem behoben, bei dem für `webapp config container` der Parameter `--slot` nicht berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="6288a-1259">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="6288a-1260">Botservice</span><span class="sxs-lookup"><span data-stu-id="6288a-1260">Botservice</span></span>
* <span data-ttu-id="6288a-1261">Unterstützung für Analyse von `.bot`-Dateien beim Aufrufen von `bot show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1261">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="6288a-1262">Fehler bei der AppInsights-Bereitstellung behoben</span><span class="sxs-lookup"><span data-stu-id="6288a-1262">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="6288a-1263">Leerzeichenfehler bei Dateipfaden behoben</span><span class="sxs-lookup"><span data-stu-id="6288a-1263">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="6288a-1264">Kudu-Netzwerkaufrufe reduziert</span><span class="sxs-lookup"><span data-stu-id="6288a-1264">Reduced Kudu network calls</span></span>
* <span data-ttu-id="6288a-1265">Allgemeine Verbesserungen bei Befehlen der Benutzeroberfläche durchgeführt</span><span class="sxs-lookup"><span data-stu-id="6288a-1265">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="6288a-1266">Nutzung</span><span class="sxs-lookup"><span data-stu-id="6288a-1266">Consumption</span></span>
* <span data-ttu-id="6288a-1267">Fehler für Budget-API zum Anzeigen von Benachrichtigungen behoben</span><span class="sxs-lookup"><span data-stu-id="6288a-1267">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="6288a-1268">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="6288a-1268">CosmosDB</span></span>
* <span data-ttu-id="6288a-1269">Unterstützung für die Aktualisierung des Kontos von „Singlemaster“ auf „Multimaster“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1269">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="6288a-1270">Karten</span><span class="sxs-lookup"><span data-stu-id="6288a-1270">Maps</span></span>
* <span data-ttu-id="6288a-1271">Unterstützung für SKU „S1“ für `maps account [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1271">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="6288a-1272">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6288a-1272">Network</span></span>
* <span data-ttu-id="6288a-1273">Unterstützung für `--format` und `--log-version` für `watcher flow-log configure` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1273">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="6288a-1274">Problem mit `dns zone update` behoben, bei dem die Verwendung von "" zum Löschen von Auflösungs- und Registrierungs-VNETs nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="6288a-1274">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="6288a-1275">Resource</span><span class="sxs-lookup"><span data-stu-id="6288a-1275">Resource</span></span>
* <span data-ttu-id="6288a-1276">Verarbeitung des Bereichsparameters für Verwaltungsgruppen in `policy assignment [create|list|delete|show|update]` behoben</span><span class="sxs-lookup"><span data-stu-id="6288a-1276">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="6288a-1277">Neuen Befehl `resource wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1277">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="6288a-1278">Storage</span><span class="sxs-lookup"><span data-stu-id="6288a-1278">Storage</span></span>
*  <span data-ttu-id="6288a-1279">Möglichkeit zum Aktualisieren der Protokollschemaversion für Speicherdienste in `storage logging update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1279">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="6288a-1280">VM</span><span class="sxs-lookup"><span data-stu-id="6288a-1280">VM</span></span>
* <span data-ttu-id="6288a-1281">Absturz in `vm identity remove` behoben, der aufgetreten ist, wenn der angegebenen VM keine verwalteten Dienstidentitäten zugewiesen waren</span><span class="sxs-lookup"><span data-stu-id="6288a-1281">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="6288a-1282">4\. Dezember 2018</span><span class="sxs-lookup"><span data-stu-id="6288a-1282">December 4, 2018</span></span>

<span data-ttu-id="6288a-1283">Version 2.0.52</span><span class="sxs-lookup"><span data-stu-id="6288a-1283">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="6288a-1284">Core</span><span class="sxs-lookup"><span data-stu-id="6288a-1284">Core</span></span>
* <span data-ttu-id="6288a-1285">Unterstützung für mandantenübergreifende Ressourcenbereitstellung für mehrinstanzenfähigen Dienstprinzipal hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1285">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="6288a-1286">Behebung eines Fehlers, aufgrund dessen IDs, die von einem Befehl mit Ausgabe im TSV-Format weitergeleitet wurden, nicht ordnungsgemäß analysiert wurden</span><span class="sxs-lookup"><span data-stu-id="6288a-1286">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="6288a-1287">AppService</span><span class="sxs-lookup"><span data-stu-id="6288a-1287">Appservice</span></span>
* <span data-ttu-id="6288a-1288">[VORSCHAU] Befehl `webapp up` hinzugefügt, der Benutzer beim Erstellen und Bereitstellen von Inhalten in Apps unterstützt</span><span class="sxs-lookup"><span data-stu-id="6288a-1288">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="6288a-1289">Behebung eines Fehlers in einer containerbasierten Windows-App, der aufgrund einer Back-End-Änderung auftrat</span><span class="sxs-lookup"><span data-stu-id="6288a-1289">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="6288a-1290">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6288a-1290">Network</span></span>
* <span data-ttu-id="6288a-1291">Argument `--exclusion` zu `application-gateway waf-config set` hinzugefügt, um WAF-Ausschlüsse zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="6288a-1291">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="6288a-1292">Role</span><span class="sxs-lookup"><span data-stu-id="6288a-1292">Role</span></span>
* <span data-ttu-id="6288a-1293">Unterstützung für benutzerdefinierte Bezeichner für Kennwortanmeldeinformation hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1293">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="6288a-1294">VM</span><span class="sxs-lookup"><span data-stu-id="6288a-1294">VM</span></span>
* <span data-ttu-id="6288a-1295">[VERALTET] Parameter `vm extension [show|wait] --expand` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="6288a-1295">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="6288a-1296">Parameter `--force` zu `vm restart` hinzugefügt, um nicht reagierende virtuelle Computer erneut bereitzustellen</span><span class="sxs-lookup"><span data-stu-id="6288a-1296">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="6288a-1297">`[vm|vmss] create --authentication-type` geändert, um „all“ zu akzeptieren und einen virtuellen Computer mit Kennwort- und SSH-Authentifizierung zu erstellen</span><span class="sxs-lookup"><span data-stu-id="6288a-1297">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="6288a-1298">Parameter `image create --os-disk-caching` hinzugefügt, um die Zwischenspeicherung von Betriebssystemdatenträgern für ein Image festzulegen</span><span class="sxs-lookup"><span data-stu-id="6288a-1298">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="6288a-1299">20. November 2018</span><span class="sxs-lookup"><span data-stu-id="6288a-1299">November 20, 2018</span></span>

<span data-ttu-id="6288a-1300">Version 2.0.51</span><span class="sxs-lookup"><span data-stu-id="6288a-1300">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="6288a-1301">Core</span><span class="sxs-lookup"><span data-stu-id="6288a-1301">Core</span></span>
* <span data-ttu-id="6288a-1302">MSI-Anmeldung geändert, sodass der Abonnementname nicht in der Identität wiederverwendet wird</span><span class="sxs-lookup"><span data-stu-id="6288a-1302">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="6288a-1303">ACR</span><span class="sxs-lookup"><span data-stu-id="6288a-1303">ACR</span></span>
* <span data-ttu-id="6288a-1304">Kontexttoken zum Aufgabenschritt hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1304">Added context token to task step</span></span>
* <span data-ttu-id="6288a-1305">Unterstützung für das Festlegen von Geheimnissen in „acr run“ zum Spiegeln der ACR-Aufgabe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1305">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="6288a-1306">Unterstützung für `--top` und `--orderby` für die Befehle `show-tags` und `show-manifests` verbessert</span><span class="sxs-lookup"><span data-stu-id="6288a-1306">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="6288a-1307">AppService</span><span class="sxs-lookup"><span data-stu-id="6288a-1307">Appservice</span></span>
* <span data-ttu-id="6288a-1308">Standardtimeout der ZIP-Bereitstellung für das Abrufen des Status auf fünf Minuten erhöht und Timeout-Eigenschaft zum Anpassen dieses Werts hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1308">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="6288a-1309">Aktualisierung der standardmäßigen `node_version`.</span><span class="sxs-lookup"><span data-stu-id="6288a-1309">Updated the default `node_version`.</span></span> <span data-ttu-id="6288a-1310">Während eines Austauschvorgangs mit zwei Phasen werden bei der Austauschaktion zum Zurücksetzen des Slots alle App-Einstellungen und Verbindungszeichenfolgen beibehalten.</span><span class="sxs-lookup"><span data-stu-id="6288a-1310">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="6288a-1311">Clientseitige SKU-Überprüfung für die Erstellung eines Linux-App Service-Plans entfernt</span><span class="sxs-lookup"><span data-stu-id="6288a-1311">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="6288a-1312">Behebung eines Fehlers beim Abrufen des ZipDeploy-Status</span><span class="sxs-lookup"><span data-stu-id="6288a-1312">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="6288a-1313">IotCentral</span><span class="sxs-lookup"><span data-stu-id="6288a-1313">IotCentral</span></span>
* <span data-ttu-id="6288a-1314">Verfügbarkeitsprüfung für Unterdomänen beim Erstellen einer IoT Central-Anwendung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1314">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="6288a-1315">KeyVault</span><span class="sxs-lookup"><span data-stu-id="6288a-1315">KeyVault</span></span>
* <span data-ttu-id="6288a-1316">Behebung eines Fehlers, aufgrund dessen Fehler mitunter ignoriert wurden</span><span class="sxs-lookup"><span data-stu-id="6288a-1316">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="6288a-1317">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6288a-1317">Network</span></span>
* <span data-ttu-id="6288a-1318">`root-cert`-Unterbefehle zum Behandeln von vertrauenswürdigen Stammzertifikaten zu `application-gateway` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1318">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="6288a-1319">Optionen `--min-capacity` und `--custom-error-pages` zu `application-gateway [create|update]` hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="6288a-1319">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="6288a-1320">`--zones` zur Unterstützung von Verfügbarkeitszonen zu `application-gateway create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1320">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="6288a-1321">Argumente `--file-upload-limit`, `--max-request-body-size` und `--request-body-check` zu `application-gateway waf-config set` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1321">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="6288a-1322">Rdbms</span><span class="sxs-lookup"><span data-stu-id="6288a-1322">Rdbms</span></span>
* <span data-ttu-id="6288a-1323">MariaDB-VNET-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1323">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="6288a-1324">RBAC</span><span class="sxs-lookup"><span data-stu-id="6288a-1324">Rbac</span></span>
* <span data-ttu-id="6288a-1325">Problem beim Aktualisieren unveränderlicher Anmeldeinformationen in `ad app update` behoben</span><span class="sxs-lookup"><span data-stu-id="6288a-1325">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="6288a-1326">Ausgabewarnungen zur Ankündigung bevorstehender Breaking Changes für `ad [app|sp] list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1326">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="6288a-1327">Storage</span><span class="sxs-lookup"><span data-stu-id="6288a-1327">Storage</span></span>
* <span data-ttu-id="6288a-1328">Behandlung von Ausnahmefällen für Speicherkopierbefehle verbessert</span><span class="sxs-lookup"><span data-stu-id="6288a-1328">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="6288a-1329">Problem behoben, aufgrund dessen `storage blob copy start-batch` bei identischen Ziel- und Quellkonten keine Anmeldeinformationen verwendete</span><span class="sxs-lookup"><span data-stu-id="6288a-1329">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="6288a-1330">Fehler bei `storage [blob|file] url` behoben, aufgrund dessen `sas_token` nicht in die URL eingebunden wurde</span><span class="sxs-lookup"><span data-stu-id="6288a-1330">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="6288a-1331">Breaking Change-Warnung zu `[blob|container] list` hinzugefügt: In Kürze werden standardmäßig nur die ersten 5.000 Ergebnisse ausgegeben.</span><span class="sxs-lookup"><span data-stu-id="6288a-1331">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="6288a-1332">VM</span><span class="sxs-lookup"><span data-stu-id="6288a-1332">VM</span></span>
* <span data-ttu-id="6288a-1333">Unterstützung für die separate Angabe einer Speicherkonto-SKU für verwaltete Betriebssystemdatenträger und Datenträger zu `[vm|vmss] create --storage-sku` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1333">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="6288a-1334">Parameter für den Versionsnamen von `sig image-version` in `--image-version -e` geändert</span><span class="sxs-lookup"><span data-stu-id="6288a-1334">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="6288a-1335">`sig image-version`-Argument `--image-version-name` als veraltet markiert und durch `--image-version` ersetzt</span><span class="sxs-lookup"><span data-stu-id="6288a-1335">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="6288a-1336">Unterstützung für die Verwendung des lokalen Betriebssystemdatenträgers für `[vm|vmss] create --ephemeral-os-disk` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1336">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="6288a-1337">Unterstützung für `--no-wait` zu `snapshot create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1337">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="6288a-1338">Befehl `snapshot wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1338">Added `snapshot wait` command</span></span>
* <span data-ttu-id="6288a-1339">Unterstützung für die Verwendung von Instanznamen mit `[vm|vmss] extension set --extension-instance-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1339">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="6288a-1340">6\. November 2018</span><span class="sxs-lookup"><span data-stu-id="6288a-1340">November 6, 2018</span></span>

<span data-ttu-id="6288a-1341">Version 2.0.50</span><span class="sxs-lookup"><span data-stu-id="6288a-1341">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="6288a-1342">Core</span><span class="sxs-lookup"><span data-stu-id="6288a-1342">Core</span></span>
* <span data-ttu-id="6288a-1343">Unterstützung für die Dienstprinzipalauthentifizierung (SN und Aussteller) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1343">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="6288a-1344">ACR</span><span class="sxs-lookup"><span data-stu-id="6288a-1344">ACR</span></span>
* <span data-ttu-id="6288a-1345">Unterstützung für Commit- und Pull Request-Git-Ereignisse für Aufgabenquellentrigger hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1345">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="6288a-1346">Auf Verwendung des Standard-Dockerfiles umgestellt, falls im Erstellungsbefehl kein Dockerfile angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="6288a-1346">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="6288a-1347">ACS</span><span class="sxs-lookup"><span data-stu-id="6288a-1347">ACS</span></span>
* <span data-ttu-id="6288a-1348">[BREAKING CHANGE]`enable_cloud_console_aks_browse` entfernt, um standardmäßig „az aks browse“ zu aktivieren</span><span class="sxs-lookup"><span data-stu-id="6288a-1348">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="6288a-1349">Advisor</span><span class="sxs-lookup"><span data-stu-id="6288a-1349">Advisor</span></span>
* <span data-ttu-id="6288a-1350">Allgemein verfügbares Release</span><span class="sxs-lookup"><span data-stu-id="6288a-1350">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="6288a-1351">AMS</span><span class="sxs-lookup"><span data-stu-id="6288a-1351">AMS</span></span>
* <span data-ttu-id="6288a-1352">Neue Befehlsgruppen hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="6288a-1352">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="6288a-1353">Neue Befehle hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="6288a-1353">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="6288a-1354">Unterstützung von Verschlüsselungsparametern für `ams streaming-policy create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1354">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="6288a-1355">Für `ams transform output remove` kann jetzt der zu entfernende Ausgabeindex angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="6288a-1355">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="6288a-1356">Argumente `--correlation-data` und `--label` zur Befehlsgruppe `ams job` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1356">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="6288a-1357">Argumente `--storage-account` und `--container` zur Befehlsgruppe `ams asset` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1357">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="6288a-1358">Standardwerte für Ablaufzeit (aktueller Zeitpunkt + 23 Std.) und Berechtigungen (Lesen) im Befehl `ams asset get-sas-url` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1358">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="6288a-1359">[BREAKING CHANGE] Befehl `ams streaming locator` durch `ams streaming-locator` ersetzt</span><span class="sxs-lookup"><span data-stu-id="6288a-1359">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="6288a-1360">[BREAKING CHANGE] Argument `--content-keys` von `ams streaming locator` aktualisiert</span><span class="sxs-lookup"><span data-stu-id="6288a-1360">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="6288a-1361">[BREAKING CHANGE]`--content-policy-name` im Befehl `ams streaming locator` in `--content-key-policy-name` umbenannt</span><span class="sxs-lookup"><span data-stu-id="6288a-1361">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="6288a-1362">[BREAKING CHANGE] Befehl `ams streaming policy` durch `ams streaming-policy` ersetzt</span><span class="sxs-lookup"><span data-stu-id="6288a-1362">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="6288a-1363">[BREAKING CHANGE] Das Argument `--preset-names` wurde in der Befehlsgruppe `--preset` durch `ams transform` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="6288a-1363">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="6288a-1364">Ab sofort kann nur noch eine einzelne Ausgabe/Voreinstellung festgelegt werden. (Wenn Sie weitere hinzufügen möchten, müssen Sie `ams transform output add` ausführen.)</span><span class="sxs-lookup"><span data-stu-id="6288a-1364">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="6288a-1365">Darüber hinaus können Sie eine benutzerdefinierte Voreinstellung für den Standard-Encoder (StandardEncoderPreset) festlegen, indem Sie den Pfad an Ihr benutzerdefiniertes JSON-Objekt übergeben.</span><span class="sxs-lookup"><span data-stu-id="6288a-1365">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="6288a-1366">[BREAKING CHANGE]`--output-asset-names ` wurde im Befehl `ams job start` in `--output-assets` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="6288a-1366">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="6288a-1367">Ab sofort wird eine durch Leerzeichen getrennte Ressourcenliste im Format „assetName=Bezeichnung“ akzeptiert.</span><span class="sxs-lookup"><span data-stu-id="6288a-1367">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="6288a-1368">Ressourcen ohne Bezeichnung können wie folgt gesendet werden: „assetName=“.</span><span class="sxs-lookup"><span data-stu-id="6288a-1368">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="6288a-1369">AppService</span><span class="sxs-lookup"><span data-stu-id="6288a-1369">AppService</span></span>
* <span data-ttu-id="6288a-1370">Fehler in `az webapp config backup update` behoben, der dazu führte, dass kein Sicherungszeitplan festgelegt werden konnte, wenn noch keiner festgelegt war</span><span class="sxs-lookup"><span data-stu-id="6288a-1370">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="6288a-1371">Konfigurieren</span><span class="sxs-lookup"><span data-stu-id="6288a-1371">Configure</span></span>
* <span data-ttu-id="6288a-1372">YAML zu Ausgabeformatoptionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1372">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="6288a-1373">Container</span><span class="sxs-lookup"><span data-stu-id="6288a-1373">Container</span></span>
* <span data-ttu-id="6288a-1374">Auf Anzeige der Identität umgestellt, wenn eine Containergruppe nach YAML exportiert wird</span><span class="sxs-lookup"><span data-stu-id="6288a-1374">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="6288a-1375">EventHub</span><span class="sxs-lookup"><span data-stu-id="6288a-1375">EventHub</span></span>
* <span data-ttu-id="6288a-1376">Flag `--enable-kafka` hinzugefügt, um Kafka in `eventhub namespace [create|update]` zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="6288a-1376">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="6288a-1377">Interactive</span><span class="sxs-lookup"><span data-stu-id="6288a-1377">Interactive</span></span>
* <span data-ttu-id="6288a-1378">Interactive installiert nun die Erweiterung `interactive`, um schnellere Updates und schnelleren Support zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="6288a-1378">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="6288a-1379">Überwachen</span><span class="sxs-lookup"><span data-stu-id="6288a-1379">Monitor</span></span>
* <span data-ttu-id="6288a-1380">Unterstützung für Metriknamen mit Schrägstrichen und Punkten zu `--condition` in `monitor metrics alert [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1380">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="6288a-1381">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6288a-1381">Network</span></span>
* <span data-ttu-id="6288a-1382">Befehlsnamen vom Typ `network interface-endpoint` zugunsten von `network private-endpoint` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="6288a-1382">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="6288a-1383">Problem behoben, das dazu führte, dass das Argument `--peer-circuit` in `express-route peering connection create` keine ID akzeptiert</span><span class="sxs-lookup"><span data-stu-id="6288a-1383">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="6288a-1384">Problem behoben, das dazu führte, dass `--ip-tags` mit `public-ip create` nicht ordnungsgemäß funktioniert</span><span class="sxs-lookup"><span data-stu-id="6288a-1384">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="6288a-1385">Profil</span><span class="sxs-lookup"><span data-stu-id="6288a-1385">Profile</span></span>
* <span data-ttu-id="6288a-1386">`--use-cert-sn-issuer` zu `az login` hinzugefügt, um Dienstprinzipalanmeldungen mit automatischem Zertifikatrollover zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="6288a-1386">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="6288a-1387">RDBMS</span><span class="sxs-lookup"><span data-stu-id="6288a-1387">RDBMS</span></span>
* <span data-ttu-id="6288a-1388">MySQL-Replikatbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1388">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="6288a-1389">Resource</span><span class="sxs-lookup"><span data-stu-id="6288a-1389">Resource</span></span>
* <span data-ttu-id="6288a-1390">Unterstützung für Verwaltungsgruppen und Abonnements zu Befehlen vom Typ `policy definition|set-definition` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1390">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="6288a-1391">Role</span><span class="sxs-lookup"><span data-stu-id="6288a-1391">Role</span></span>
* <span data-ttu-id="6288a-1392">Unterstützung für die API-Berechtigungsverwaltung, den angemeldeten Benutzer und die Verwaltung von Anwendungskennwörtern und Zertifikatanmeldeinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1392">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="6288a-1393">`ad sp create-for-rbac` geändert, um „displayName“ und Dienstprinzipalname besser unterscheiden zu können</span><span class="sxs-lookup"><span data-stu-id="6288a-1393">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="6288a-1394">Unterstützung der Gewährung von Berechtigungen für AAD-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1394">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="6288a-1395">Storage</span><span class="sxs-lookup"><span data-stu-id="6288a-1395">Storage</span></span>
* <span data-ttu-id="6288a-1396">Möglichkeit hinzugefügt, allein mit SAS und Endpunkten (ohne Kontoname oder Schlüssel) eine Verbindung mit Speicherdiensten herzustellen, wie unter `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>` beschrieben</span><span class="sxs-lookup"><span data-stu-id="6288a-1396">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="6288a-1397">VM</span><span class="sxs-lookup"><span data-stu-id="6288a-1397">VM</span></span>
* <span data-ttu-id="6288a-1398">Argument `storage-sku` zu `image create` hinzugefügt, um das Festlegen des standardmäßigen Speicherkontotyps für das Image zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="6288a-1398">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="6288a-1399">Fehler für `vm resize` behoben, durch den die Option `--no-wait` einen Absturz des Befehls verursachte</span><span class="sxs-lookup"><span data-stu-id="6288a-1399">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="6288a-1400">Tabellenausgabeformat für `vm encryption show` geändert, um den Status anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="6288a-1400">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="6288a-1401">`vm secret format` geändert, um JSON/JSONC-Ausgabe erforderlich zu machen.</span><span class="sxs-lookup"><span data-stu-id="6288a-1401">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="6288a-1402">Der Benutzer wird gewarnt, und es wird standardmäßig die JSON-Ausgabe verwendet, wenn ein unzulässiges Ausgabeformat ausgewählt wird.</span><span class="sxs-lookup"><span data-stu-id="6288a-1402">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="6288a-1403">Argumentüberprüfung für `vm create --image` verbessert</span><span class="sxs-lookup"><span data-stu-id="6288a-1403">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="6288a-1404">23. Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="6288a-1404">October 23, 2018</span></span>

<span data-ttu-id="6288a-1405">Version 2.0.49</span><span class="sxs-lookup"><span data-stu-id="6288a-1405">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="6288a-1406">Core</span><span class="sxs-lookup"><span data-stu-id="6288a-1406">Core</span></span>
* <span data-ttu-id="6288a-1407">Problem mit `--ids` behoben, aufgrund dessen `--subscription` Vorrang vor dem Abonnement in `--ids` hatte</span><span class="sxs-lookup"><span data-stu-id="6288a-1407">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="6288a-1408">Ausdrückliche Warnungen hinzugefügt, wenn Parameter durch die Verwendung von `--ids` ignoriert würden</span><span class="sxs-lookup"><span data-stu-id="6288a-1408">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="6288a-1409">ACR</span><span class="sxs-lookup"><span data-stu-id="6288a-1409">ACR</span></span>
* <span data-ttu-id="6288a-1410">Problem mit der ACR Build-Codierung in Python2 behoben</span><span class="sxs-lookup"><span data-stu-id="6288a-1410">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="6288a-1411">CDN</span><span class="sxs-lookup"><span data-stu-id="6288a-1411">CDN</span></span>
* <span data-ttu-id="6288a-1412">[BREAKING CHANGE] Standardverhalten beim Zwischenspeichern der Abfragezeichenfolge von `cdn endpoint create` so geändert, dass der Standardwert nicht mehr „IgnoreQueryString“ ist.</span><span class="sxs-lookup"><span data-stu-id="6288a-1412">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="6288a-1413">Er wird jetzt vom Dienst festgelegt.</span><span class="sxs-lookup"><span data-stu-id="6288a-1413">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="6288a-1414">Container</span><span class="sxs-lookup"><span data-stu-id="6288a-1414">Container</span></span>
* <span data-ttu-id="6288a-1415">`Private` als gültiger Typ für die Übergabe an „--ip-address“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1415">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="6288a-1416">Geändert, sodass nur eine Subnetz-ID für das Einrichten eines virtuellen Netzwerks für die Containergruppe zulässig ist</span><span class="sxs-lookup"><span data-stu-id="6288a-1416">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="6288a-1417">Geändert, sodass das Verwenden eines VNET-Namens oder einer Ressourcen-ID zulässig ist, um die Verwendung von VNETs aus verschiedenen Ressourcengruppen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="6288a-1417">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="6288a-1418">`--assign-identity` hinzugefügt, um einer Containergruppe eine MSI-Identität hinzuzufügen</span><span class="sxs-lookup"><span data-stu-id="6288a-1418">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="6288a-1419">`--scope` hinzugefügt, um eine Rollenzuweisung für die vom System zugewiesene MSI-Identität zu erstellen</span><span class="sxs-lookup"><span data-stu-id="6288a-1419">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="6288a-1420">Warnung hinzugefügt, wenn eine Containergruppe mit einem Image ohne Prozess mit langer Ausführungszeit erstellt wird</span><span class="sxs-lookup"><span data-stu-id="6288a-1420">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="6288a-1421">Probleme mit der Tabellenausgabe für Befehle `list` und `show` behoben</span><span class="sxs-lookup"><span data-stu-id="6288a-1421">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="6288a-1422">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="6288a-1422">CosmosDB</span></span>
* <span data-ttu-id="6288a-1423">Unterstützung für `--enable-multiple-write-locations` zu `cosmosdb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1423">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="6288a-1424">Interactive</span><span class="sxs-lookup"><span data-stu-id="6288a-1424">Interactive</span></span>
* <span data-ttu-id="6288a-1425">Geändert, um sicherzustellen, dass der Parameter für globales Abonnement in Parametern angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="6288a-1425">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="6288a-1426">IoT Central</span><span class="sxs-lookup"><span data-stu-id="6288a-1426">IoT Central</span></span>
* <span data-ttu-id="6288a-1427">Optionen für Vorlagen und Anzeigenamen für die Erstellung von IoT Central-Anwendungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1427">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="6288a-1428">[BREAKING CHANGE] Unterstützung für F1-SKU entfernt; stattdessen ist die S1-SKU zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="6288a-1428">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="6288a-1429">Überwachen</span><span class="sxs-lookup"><span data-stu-id="6288a-1429">Monitor</span></span>
* <span data-ttu-id="6288a-1430">Änderungen an `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="6288a-1430">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="6288a-1431">Unterstützung für das Auflisten aller Ereignisse auf Abonnementebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1431">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="6288a-1432">`--offset`-Parameter für das einfachere Erstellen von Zeitabfragen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1432">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="6288a-1433">Validierung für `--start-time` und `--end-time` verbessert, um die Verwendung von mehr ISO8601-Formate und benutzerfreundlicheren datetime-Formaten zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="6288a-1433">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="6288a-1434">`--namespace` als Alias für veraltete Option `--resource-provider` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1434">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="6288a-1435">`--filters` als veraltet markiert, da vom Dienst ausschließlich Werte mit stark typisierten Optionen unterstützt werden</span><span class="sxs-lookup"><span data-stu-id="6288a-1435">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="6288a-1436">Änderungen an `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="6288a-1436">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="6288a-1437">`--offset`-Parameter für das einfachere Erstellen von Zeitabfragen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1437">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="6288a-1438">Validierung für `--start-time` und `--end-time` verbessert, um die Verwendung von mehr ISO8601-Formate und benutzerfreundlicheren datetime-Formaten zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="6288a-1438">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="6288a-1439">Validierung für `--event-hub`- und `--event-hub-rule`-Argumente an `monitor diagnostic-settings create` verbessert</span><span class="sxs-lookup"><span data-stu-id="6288a-1439">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="6288a-1440">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6288a-1440">Network</span></span>
* <span data-ttu-id="6288a-1441">`--app-gateway-address-pools`- und `--gateway-name`-Argumente zu `nic create` hinzugefügt, um das Hinzufügen von Back-End-Adresspools für Anwendungsgateways zu einer NIC zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="6288a-1441">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="6288a-1442">`--app-gateway-address-pools`- und `--gateway-name`-Argumente zu `nic ip-config create/update` hinzugefügt, um das Hinzufügen von Back-End-Adresspools für Anwendungsgateways zu einer NIC zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="6288a-1442">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="6288a-1443">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="6288a-1443">ServiceBus</span></span>
* <span data-ttu-id="6288a-1444">Schreibgeschütztes `migration_state`-Element zu „MigrationConfigProperties“ hinzugefügt, um den aktuellen Status der Migration von Service Bus Standard- zu Premium-Namespace anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="6288a-1444">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="6288a-1445">SQL</span><span class="sxs-lookup"><span data-stu-id="6288a-1445">SQL</span></span>
* <span data-ttu-id="6288a-1446">`sql failover-group create` und `sql failover-group update` korrigiert, damit die Verwendung einer Richtlinie für manuelles Failover möglich ist</span><span class="sxs-lookup"><span data-stu-id="6288a-1446">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="6288a-1447">Storage</span><span class="sxs-lookup"><span data-stu-id="6288a-1447">Storage</span></span>
* <span data-ttu-id="6288a-1448">Formatierung der `az storage cors list`-Ausgabe korrigiert, sodass alle Elemente den richtigen Dienstschlüssel anzeigen</span><span class="sxs-lookup"><span data-stu-id="6288a-1448">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="6288a-1449">`--bypass-immutability-policy`-Parameter für das Löschen von durch Unveränderlichkeitsrichtlinien blockierten Containern hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1449">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="6288a-1450">VM</span><span class="sxs-lookup"><span data-stu-id="6288a-1450">VM</span></span>
* <span data-ttu-id="6288a-1451">Datenträger-Zwischenspeicherungsmodus `None` für Lv/Lv2-Computerserine in `[vm|vmss] create` erzwungen</span><span class="sxs-lookup"><span data-stu-id="6288a-1451">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="6288a-1452">Liste der unterstützten Größen für unterstützenden Netzwerkbeschleuniger für `vm create` aktualisiert</span><span class="sxs-lookup"><span data-stu-id="6288a-1452">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="6288a-1453">Stark typisierte Argumente für UltraSSD-IOPS und MBit/s-Konfigurationen für `disk create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1453">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="6288a-1454">16. Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="6288a-1454">October 16, 2018</span></span>

<span data-ttu-id="6288a-1455">Version 2.0.48</span><span class="sxs-lookup"><span data-stu-id="6288a-1455">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="6288a-1456">VM</span><span class="sxs-lookup"><span data-stu-id="6288a-1456">VM</span></span>
* <span data-ttu-id="6288a-1457">SDK-Problem behoben, das ein Fehlschlagen der Homebrew-Installation verursacht hat</span><span class="sxs-lookup"><span data-stu-id="6288a-1457">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="6288a-1458">9\. Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="6288a-1458">October 9, 2018</span></span>

<span data-ttu-id="6288a-1459">Version 2.0.47</span><span class="sxs-lookup"><span data-stu-id="6288a-1459">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="6288a-1460">Core</span><span class="sxs-lookup"><span data-stu-id="6288a-1460">Core</span></span>
* <span data-ttu-id="6288a-1461">Verbesserte Fehlerbehandlung für Fehler vom Typ „Ungültige Anforderung“</span><span class="sxs-lookup"><span data-stu-id="6288a-1461">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="6288a-1462">ACR</span><span class="sxs-lookup"><span data-stu-id="6288a-1462">ACR</span></span>
* <span data-ttu-id="6288a-1463">Unterstützung für ähnliches Tabellenformat wie Helm-Client hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1463">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="6288a-1464">ACS</span><span class="sxs-lookup"><span data-stu-id="6288a-1464">ACS</span></span>
* <span data-ttu-id="6288a-1465">`aks [create|scale] --nodepool-name` zum Konfigurieren des Knotenpoolnamens hinzugefügt, auf 12 Zeichen gekürzt, Standard: nodepool1</span><span class="sxs-lookup"><span data-stu-id="6288a-1465">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="6288a-1466">Korrektur, bei der auf „scp“ zurückgegriffen wird, wenn Parimiko nicht funktioniert</span><span class="sxs-lookup"><span data-stu-id="6288a-1466">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="6288a-1467">`aks create` geändert, sodass `--aad-tenant-id` nicht mehr erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="6288a-1467">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="6288a-1468">Verbesserte Zusammenführung von Kubernetes-Anmeldeinformationen, wenn doppelte Einträge vorhanden sind</span><span class="sxs-lookup"><span data-stu-id="6288a-1468">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="6288a-1469">Container</span><span class="sxs-lookup"><span data-stu-id="6288a-1469">Container</span></span>
* <span data-ttu-id="6288a-1470">`functionapp create` geändert, sodass das Erstellen eines Linux-Nutzungsplans mit einer bestimmten Runtime unterstützt wird</span><span class="sxs-lookup"><span data-stu-id="6288a-1470">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="6288a-1471">[VORSCHAUVERSION] Unterstützung für das Hosten von Web-Apps in Windows-Containern hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1471">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="6288a-1472">Event Hub</span><span class="sxs-lookup"><span data-stu-id="6288a-1472">Event Hub</span></span>
* <span data-ttu-id="6288a-1473">Befehl `eventhub update` korrigiert</span><span class="sxs-lookup"><span data-stu-id="6288a-1473">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="6288a-1474">[BREAKING CHANGE]`list`-Befehle geändert, sodass Fehler von Typ „NotFound(404)“ für Ressourcen mit der typische Vorgehensweise behandelt werden, anstatt eine leere Liste anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="6288a-1474">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="6288a-1475">Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="6288a-1475">Extensions</span></span>
* <span data-ttu-id="6288a-1476">Problem beim Hinzufügen einer Erweiterung behoben, die bereits installiert ist</span><span class="sxs-lookup"><span data-stu-id="6288a-1476">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="6288a-1477">HDInsight</span><span class="sxs-lookup"><span data-stu-id="6288a-1477">HDInsight</span></span>
* <span data-ttu-id="6288a-1478">Erste Veröffentlichung</span><span class="sxs-lookup"><span data-stu-id="6288a-1478">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="6288a-1479">IoT</span><span class="sxs-lookup"><span data-stu-id="6288a-1479">IoT</span></span>
* <span data-ttu-id="6288a-1480">Befehl zur Erweiterungsinstallation zu Banner bei der ersten Ausführung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1480">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="6288a-1481">KeyVault</span><span class="sxs-lookup"><span data-stu-id="6288a-1481">KeyVault</span></span>
* <span data-ttu-id="6288a-1482">Geändert, sodass Key Vault-Speicherbefehle auf das aktuelle API-Profil beschränkt sind</span><span class="sxs-lookup"><span data-stu-id="6288a-1482">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="6288a-1483">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6288a-1483">Network</span></span>
* <span data-ttu-id="6288a-1484">`network dns zone create` korrigiert: Befehl ist auch erfolgreich, wenn der Benutzer einen Standardspeicherort konfiguriert hat.</span><span class="sxs-lookup"><span data-stu-id="6288a-1484">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="6288a-1485">Siehe Nr. 6052</span><span class="sxs-lookup"><span data-stu-id="6288a-1485">See #6052</span></span>
* <span data-ttu-id="6288a-1486">`--remote-vnet-id` für `network vnet peering create` eingestellt</span><span class="sxs-lookup"><span data-stu-id="6288a-1486">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="6288a-1487">`--remote-vnet` zum `network vnet peering create`-Element hinzugefügt, das einen Namen oder eine ID akzeptiert</span><span class="sxs-lookup"><span data-stu-id="6288a-1487">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="6288a-1488">Unterstützung für mehrere Subnetzpräfixe zu `network vnet create` in `--subnet-prefixes` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1488">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="6288a-1489">Unterstützung für mehrere Subnetzpräfixe zu `network vnet subnet [create|update]` in `--address-prefixes` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1489">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="6288a-1490">Problem mit `network application-gateway create` behoben, das die Erstellung von Gateways mit der SKU `WAF_v2` oder `Standard_v2` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="6288a-1490">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="6288a-1491">`--service-endpoint-policy`-Argument für Benutzerfreundlichkeit zu `network vnet subnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1491">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="6288a-1492">Role</span><span class="sxs-lookup"><span data-stu-id="6288a-1492">Role</span></span>
* <span data-ttu-id="6288a-1493">Unterstützung für das Auflisten von Azure AD-App-Besitzern in `ad app owner` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1493">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="6288a-1494">Unterstützung für das Auflisten von Azure AD-Dienstprinzipalbesitzern in `ad sp owner` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1494">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="6288a-1495">Geändert, um sicherzustellen, dass die Erstellungs- und Aktualisierungsbefehle für die Rollendefinition Konfigurationen mit mehreren Berechtigungen akzeptieren</span><span class="sxs-lookup"><span data-stu-id="6288a-1495">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="6288a-1496">`ad sp create-for-rbac` geändert, um sicherzustellen, dass der Homepage-URI immer „https“ ist</span><span class="sxs-lookup"><span data-stu-id="6288a-1496">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="6288a-1497">Service Bus</span><span class="sxs-lookup"><span data-stu-id="6288a-1497">Service Bus</span></span>
* <span data-ttu-id="6288a-1498">[BREAKING CHANGE]`list`-Befehle geändert, sodass Fehler von Typ „NotFound(404)“ für Ressourcen mit der typische Vorgehensweise behandelt werden, anstatt eine leere Liste anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="6288a-1498">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="6288a-1499">VM</span><span class="sxs-lookup"><span data-stu-id="6288a-1499">VM</span></span>
* <span data-ttu-id="6288a-1500">Leeres `accessSas`-Feld in `disk grant-access` korrigiert</span><span class="sxs-lookup"><span data-stu-id="6288a-1500">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="6288a-1501">`vmss create` geändert, sodass ein ausreichend großer Front-End-Portbereich zur Verarbeitung von Überbereitstellung reserviert ist</span><span class="sxs-lookup"><span data-stu-id="6288a-1501">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="6288a-1502">Aktualisierungsbefehle für `sig` korrigiert</span><span class="sxs-lookup"><span data-stu-id="6288a-1502">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="6288a-1503">`--no-wait`-Unterstützung für die Verwaltung von Imageversionen in `sig` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1503">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="6288a-1504">`vm list-ip-addresses` geändert, sodass die Verfügbarkeitszone von öffentlichen IP-Adressen angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="6288a-1504">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="6288a-1505">`[vm|vmss] disk attach` geändert, sodass die Standard-LUN eines Datenträgers standardmäßig auf die erste verfügbare Stelle festgelegt wird</span><span class="sxs-lookup"><span data-stu-id="6288a-1505">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="6288a-1506">21. September 2018</span><span class="sxs-lookup"><span data-stu-id="6288a-1506">September 21, 2018</span></span>

<span data-ttu-id="6288a-1507">Version 2.0.46</span><span class="sxs-lookup"><span data-stu-id="6288a-1507">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="6288a-1508">ACR</span><span class="sxs-lookup"><span data-stu-id="6288a-1508">ACR</span></span>
* <span data-ttu-id="6288a-1509">ACR-Aufgabenbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1509">Added ACR Task commands</span></span>
* <span data-ttu-id="6288a-1510">Befehl für die Schnellausführung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1510">Added quick run command</span></span>
* <span data-ttu-id="6288a-1511">`build-task`-Befehlsgruppe als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="6288a-1511">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="6288a-1512">`helm`-Befehlsgruppe hinzugefügt, um die Verwaltung von Helm-Diagrammen mit ACR zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="6288a-1512">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="6288a-1513">Unterstützung für idempotentes Erstellen für die verwaltete Registrierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1513">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="6288a-1514">Formatfreies Flag für die Anzeige von Buildprotokollen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1514">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="6288a-1515">ACS</span><span class="sxs-lookup"><span data-stu-id="6288a-1515">ACS</span></span>
* <span data-ttu-id="6288a-1516">Befehl `install-connector` zum Festlegen des AKS-Master-FQDN geändert</span><span class="sxs-lookup"><span data-stu-id="6288a-1516">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="6288a-1517">Erstellen der Rollenzuweisung für „vnet-subnet-id“ (wenn kein Dienstprinzipal angegeben wurde) und „skip-role-assignment“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="6288a-1517">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="6288a-1518">AppService</span><span class="sxs-lookup"><span data-stu-id="6288a-1518">AppService</span></span>

* <span data-ttu-id="6288a-1519">Unterstützung für WebJobs-Vorgangsverwaltung hinzugefügt (kontinuierlich/ausgelöst)</span><span class="sxs-lookup"><span data-stu-id="6288a-1519">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="6288a-1520">„az webapp config set“ unterstützt die Eigenschaft „--fts-state“; Unterstützung für „az functionapp config set/show“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1520">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="6288a-1521">Unterstützung für Bring Your Own Storage für Web-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1521">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="6288a-1522">Unterstützung für das Auflisten und Wiederherstellen gelöschter Web-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1522">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="6288a-1523">Batch</span><span class="sxs-lookup"><span data-stu-id="6288a-1523">Batch</span></span>
* <span data-ttu-id="6288a-1524">Hinzufügen von Aufgaben über `--json-file` geändert, um die AddTaskCollectionParameter-Syntax zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="6288a-1524">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="6288a-1525">Dokumentation akzeptierter `--json-file`-Formate aktualisiert</span><span class="sxs-lookup"><span data-stu-id="6288a-1525">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="6288a-1526">`--max-tasks-per-node-option` zu `batch pool create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1526">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="6288a-1527">Verhalten von `batch account` geändert, um das aktuell angemeldete Konto anzuzeigen, wenn keine Optionen angegeben wurden</span><span class="sxs-lookup"><span data-stu-id="6288a-1527">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="6288a-1528">Batch KI</span><span class="sxs-lookup"><span data-stu-id="6288a-1528">Batch AI</span></span> 
* <span data-ttu-id="6288a-1529">Fehler bei der automatischen Speicherkontoerstellung im Befehl `batchai cluster create` behoben</span><span class="sxs-lookup"><span data-stu-id="6288a-1529">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="6288a-1530">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="6288a-1530">Cognitive Services</span></span>
* <span data-ttu-id="6288a-1531">Vervollständigung für die Argumente `--sku`, `--kind` und `--location` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1531">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="6288a-1532">Befehl `cognitiveservices account list-usage` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1532">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="6288a-1533">Befehl `cognitiveservices account list-kinds` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1533">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="6288a-1534">Befehl `cognitiveservices account list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1534">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="6288a-1535">`cognitiveservices list` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="6288a-1535">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="6288a-1536">`--name` geändert (ist jetzt optional für `cognitiveservices account list-skus`)</span><span class="sxs-lookup"><span data-stu-id="6288a-1536">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="6288a-1537">Container</span><span class="sxs-lookup"><span data-stu-id="6288a-1537">Container</span></span>
* <span data-ttu-id="6288a-1538">Möglichkeit zum Neustarten und Beenden einer ausgeführten Containergruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1538">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="6288a-1539">`--network-profile` zum Übergeben eines Netzwerkprofils hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1539">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="6288a-1540">`--subnet` und `--vnet_name` hinzugefügt, um das Erstellen von Containergruppen in einem VNET zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="6288a-1540">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="6288a-1541">Tabellenausgabe geändert, sodass der Status der Containergruppe angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="6288a-1541">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="6288a-1542">Data Lake</span><span class="sxs-lookup"><span data-stu-id="6288a-1542">Datalake</span></span>
* <span data-ttu-id="6288a-1543">Befehle für VNET-Regeln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1543">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="6288a-1544">Interaktive Shell</span><span class="sxs-lookup"><span data-stu-id="6288a-1544">Interactive Shell</span></span>
* <span data-ttu-id="6288a-1545">Fehler in Windows behoben, durch den Befehle nicht ordnungsgemäß ausgeführt wurden</span><span class="sxs-lookup"><span data-stu-id="6288a-1545">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="6288a-1546">Durch veraltete Objekte verursachtes Problem beim Laden von Befehlen im interaktiven Modus behoben</span><span class="sxs-lookup"><span data-stu-id="6288a-1546">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="6288a-1547">IoT</span><span class="sxs-lookup"><span data-stu-id="6288a-1547">IoT</span></span>
* <span data-ttu-id="6288a-1548">Routingunterstützung für IoT Hubs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1548">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="6288a-1549">Key Vault</span><span class="sxs-lookup"><span data-stu-id="6288a-1549">Key Vault</span></span>
* <span data-ttu-id="6288a-1550">Key Vault-Schlüsselimport für RSA-Schlüssel korrigiert</span><span class="sxs-lookup"><span data-stu-id="6288a-1550">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="6288a-1551">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6288a-1551">Network</span></span>
* <span data-ttu-id="6288a-1552">Befehle vom Typ `network public-ip prefix` hinzugefügt, um Präfixe von öffentlichen IP-Adressen zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="6288a-1552">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="6288a-1553">Befehle vom Typ `network service-endpoint` hinzugefügt, um Dienstendpunktrichtlinien-Features zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="6288a-1553">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="6288a-1554">Befehle vom Typ `network lb outbound-rule` hinzugefügt, um die Erstellung von Ausgangsregeln für Load Balancer Standard zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="6288a-1554">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="6288a-1555">`--public-ip-prefix` zu `network lb frontend-ip create/update` hinzugefügt, um Front-End-IP-Konfigurationen mit Präfixen von öffentlichen IP-Adressen zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="6288a-1555">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="6288a-1556">`--enable-tcp-reset` zu `network lb rule/inbound-nat-rule/inbound-nat-pool create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1556">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="6288a-1557">`--disable-outbound-snat` zu `network lb rule create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1557">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="6288a-1558">Verwendung von `network watcher flow-log show/configure` mit klassischen NSGs ermöglicht</span><span class="sxs-lookup"><span data-stu-id="6288a-1558">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="6288a-1559">Hinzufügen des `network watcher run-configuration-diagnostic`-Befehls</span><span class="sxs-lookup"><span data-stu-id="6288a-1559">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="6288a-1560">Befehl `network watcher test-connectivity` korrigiert und Eigenschaften `--method`, `--valid-status-codes` und `--headers` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1560">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="6288a-1561">`network express-route create/update`: Flag `--allow-global-reach` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1561">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="6288a-1562">`network vnet subnet create/update`: Unterstützung für `--delegation` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1562">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="6288a-1563">Befehl `network vnet subnet list-available-delegations` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1563">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="6288a-1564">`network traffic-manager profile create/update`: Unterstützung für `--interval`, `--timeout` und `--max-failures` für die Überwachungskonfiguration hinzugefügt; Optionen `--monitor-path`, `--monitor-port` und `--monitor-protocol` zugunsten von `--path`, `--port` und `--protocol` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="6288a-1564">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="6288a-1565">`network lb frontend-ip create/update`: Logik für das Festlegen der Zuweisungsmethode für private IP-Adressen korrigiert. Bei Angabe einer privaten IP-Adresse ist die Zuweisung statisch. Wird keine private IP-Adresse (oder eine leere Zeichenfolge für die private IP-Adresse) angegeben, erfolgt eine dynamische Zuweisung.</span><span class="sxs-lookup"><span data-stu-id="6288a-1565">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="6288a-1566">`dns record-set * create/update`: Unterstützung für `--target-resource` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1566">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="6288a-1567">Befehle vom Typ `network interface-endpoint` hinzugefügt, um Schnittstellenendpunkt-Objekte abzufragen</span><span class="sxs-lookup"><span data-stu-id="6288a-1567">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="6288a-1568">`network profile show/list/delete` für die partielle Verwaltung von Netzwerkprofilen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1568">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="6288a-1569">Befehle vom Typ `network express-route peering connection` für die Verwaltung von Peeringverbindungen zwischen ExpressRoute-Instanzen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1569">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="6288a-1570">RDBMS</span><span class="sxs-lookup"><span data-stu-id="6288a-1570">RDBMS</span></span>
* <span data-ttu-id="6288a-1571">Unterstützung für den MariaDB-Dienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1571">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="6288a-1572">Reservierung</span><span class="sxs-lookup"><span data-stu-id="6288a-1572">Reservation</span></span>
* <span data-ttu-id="6288a-1573">Cosmos DB im Enumerationstyp für reservierte Ressourcen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1573">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="6288a-1574">Namenseigenschaft im Patchmodell hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1574">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="6288a-1575">App-Verwaltung</span><span class="sxs-lookup"><span data-stu-id="6288a-1575">Manage App</span></span>
* <span data-ttu-id="6288a-1576">Fehler in `managedapp create --kind MarketPlace` korrigiert, der zum Absturz der Instanzerstellung einer verwalteten Marketplace-App führte</span><span class="sxs-lookup"><span data-stu-id="6288a-1576">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="6288a-1577">Befehle vom Typ `feature` geändert, um sie auf unterstützte Profile zu beschränken</span><span class="sxs-lookup"><span data-stu-id="6288a-1577">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="6288a-1578">Role</span><span class="sxs-lookup"><span data-stu-id="6288a-1578">Role</span></span>
* <span data-ttu-id="6288a-1579">Unterstützung für das Auflisten der Gruppenmitgliedschaften des Benutzers hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1579">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="6288a-1580">SignalR</span><span class="sxs-lookup"><span data-stu-id="6288a-1580">SignalR</span></span>
* <span data-ttu-id="6288a-1581">Erste Version</span><span class="sxs-lookup"><span data-stu-id="6288a-1581">First release</span></span>

### <a name="storage"></a><span data-ttu-id="6288a-1582">Storage</span><span class="sxs-lookup"><span data-stu-id="6288a-1582">Storage</span></span>
* <span data-ttu-id="6288a-1583">Parameter `--auth-mode login` für die Verwendung der Anmeldeinformationen des Benutzers für die Blob- und Warteschlangenautorisierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1583">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="6288a-1584">`storage container immutability-policy/legal-hold` für die Verwaltung von unveränderlichem Speicher hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1584">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="6288a-1585">VM</span><span class="sxs-lookup"><span data-stu-id="6288a-1585">VM</span></span>
* <span data-ttu-id="6288a-1586">Problem behoben, das dazu führte, dass die Datei mit dem privaten Schlüssel durch `vm create --generate-ssh-keys` überschrieben wird, wenn die Datei mit dem privaten Schlüssel fehlt (Nr. 4725, 6780)</span><span class="sxs-lookup"><span data-stu-id="6288a-1586">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="6288a-1587">Unterstützung für den gemeinsamen Image-Katalog über `az sig` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1587">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="6288a-1588">28. August 2018</span><span class="sxs-lookup"><span data-stu-id="6288a-1588">August 28, 2018</span></span>

<span data-ttu-id="6288a-1589">Version 2.0.45</span><span class="sxs-lookup"><span data-stu-id="6288a-1589">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="6288a-1590">Core</span><span class="sxs-lookup"><span data-stu-id="6288a-1590">Core</span></span>

* <span data-ttu-id="6288a-1591">Das Problem, aufgrund dessen eine leere Konfigurationsdatei geladen wurde, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="6288a-1591">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="6288a-1592">Unterstützung für Profil `2018-03-01-hybrid` für Azure Stack hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1592">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="6288a-1593">ACR</span><span class="sxs-lookup"><span data-stu-id="6288a-1593">ACR</span></span>

* <span data-ttu-id="6288a-1594">Problemumgehung für Laufzeitvorgänge ohne ARM-Anforderungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1594">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="6288a-1595">Änderung vorgenommen, um im Befehl `build` Versionskontrolldateien (etwa „.git“ und „.gitignore“) standardmäßig aus der TAR-Datei auszuschließen</span><span class="sxs-lookup"><span data-stu-id="6288a-1595">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="6288a-1596">ACS</span><span class="sxs-lookup"><span data-stu-id="6288a-1596">ACS</span></span>

* <span data-ttu-id="6288a-1597">`aks create` geändert, dass standardmäßig virtuelle Computer vom Typ `Standard_DS2_v2` erstellt werden</span><span class="sxs-lookup"><span data-stu-id="6288a-1597">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="6288a-1598">`aks get-credentials` geändert, um nun neue APIs zum Abrufen der Clusteranmeldeinformationen aufzurufen</span><span class="sxs-lookup"><span data-stu-id="6288a-1598">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="6288a-1599">AppService</span><span class="sxs-lookup"><span data-stu-id="6288a-1599">AppService</span></span>

* <span data-ttu-id="6288a-1600">Unterstützung für CORS in „functionapp“ und „webapp“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1600">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="6288a-1601">ARM-Tagunterstützung in Erstellungsbefehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1601">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="6288a-1602">`[webapp|functionapp] identity show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="6288a-1602">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="6288a-1603">Backup</span><span class="sxs-lookup"><span data-stu-id="6288a-1603">Backup</span></span>

* <span data-ttu-id="6288a-1604">`backup vault backup-properties show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="6288a-1604">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="6288a-1605">Botdienst</span><span class="sxs-lookup"><span data-stu-id="6288a-1605">Bot Service</span></span>

* <span data-ttu-id="6288a-1606">Anfängliches Release der Botdienst-CLI</span><span class="sxs-lookup"><span data-stu-id="6288a-1606">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="6288a-1607">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="6288a-1607">Cognitive Services</span></span>

* <span data-ttu-id="6288a-1608">Neuer Parameter `--api-properties,` hinzugefügt, der zum Erstellen einiger Dienste erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="6288a-1608">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="6288a-1609">IoT</span><span class="sxs-lookup"><span data-stu-id="6288a-1609">IoT</span></span>

* <span data-ttu-id="6288a-1610">Problem mit dem Zuweisen verknüpfter Hubs behoben</span><span class="sxs-lookup"><span data-stu-id="6288a-1610">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="6288a-1611">Überwachen</span><span class="sxs-lookup"><span data-stu-id="6288a-1611">Monitor</span></span>

* <span data-ttu-id="6288a-1612">`monitor metrics alert`-Befehle für Metrikwarnungen nahezu in Echtzeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1612">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="6288a-1613">`monitor alert`-Befehle als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="6288a-1613">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="6288a-1614">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6288a-1614">Network</span></span>

* <span data-ttu-id="6288a-1615">`network application-gateway ssl-policy predefined show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="6288a-1615">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="6288a-1616">Resource</span><span class="sxs-lookup"><span data-stu-id="6288a-1616">Resource</span></span>

* <span data-ttu-id="6288a-1617">`provider operation show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="6288a-1617">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="6288a-1618">Storage</span><span class="sxs-lookup"><span data-stu-id="6288a-1618">Storage</span></span>

* <span data-ttu-id="6288a-1619">`storage share policy show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="6288a-1619">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="6288a-1620">VM</span><span class="sxs-lookup"><span data-stu-id="6288a-1620">VM</span></span>

* <span data-ttu-id="6288a-1621">`vm/vmss identity show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="6288a-1621">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="6288a-1622">`--storage-caching` für `vm create` eingestellt</span><span class="sxs-lookup"><span data-stu-id="6288a-1622">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="6288a-1623">14. August 2018</span><span class="sxs-lookup"><span data-stu-id="6288a-1623">Auguest 14, 2018</span></span>

<span data-ttu-id="6288a-1624">Version 2.0.44</span><span class="sxs-lookup"><span data-stu-id="6288a-1624">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="6288a-1625">Core</span><span class="sxs-lookup"><span data-stu-id="6288a-1625">Core</span></span>

* <span data-ttu-id="6288a-1626">Numerische Anzeige in `table`-Ausgabe korrigiert</span><span class="sxs-lookup"><span data-stu-id="6288a-1626">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="6288a-1627">YAML-Ausgabeformat hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1627">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="6288a-1628">Telemetrie</span><span class="sxs-lookup"><span data-stu-id="6288a-1628">Telemetry</span></span>

* <span data-ttu-id="6288a-1629">Verbesserte Berichterstellung für Telemetriedaten</span><span class="sxs-lookup"><span data-stu-id="6288a-1629">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="6288a-1630">ACR</span><span class="sxs-lookup"><span data-stu-id="6288a-1630">ACR</span></span>

* <span data-ttu-id="6288a-1631">Befehle vom Typ `content-trust policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1631">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="6288a-1632">Problem behoben, aufgrund dessen `.dockerignore` nicht richtig verarbeitet wurde</span><span class="sxs-lookup"><span data-stu-id="6288a-1632">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="6288a-1633">ACS</span><span class="sxs-lookup"><span data-stu-id="6288a-1633">ACS</span></span>

* <span data-ttu-id="6288a-1634">`az acs/aks install-cli` für die Installation in `%USERPROFILE%\.azure-kubectl` unter Windows geändert</span><span class="sxs-lookup"><span data-stu-id="6288a-1634">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="6288a-1635">`az aks install-connector` geändert, um zu ermitteln, ob der Cluster über RBAC verfügt, und um den ACI-Connector entsprechend zu konfigurieren</span><span class="sxs-lookup"><span data-stu-id="6288a-1635">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="6288a-1636">Geändert in Rollenzuweisung zum Subnetz bei entsprechender Angabe</span><span class="sxs-lookup"><span data-stu-id="6288a-1636">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="6288a-1637">Neue Option zum Überspringen der Rollenzuweisung für Subnetz hinzugefügt, wenn dieses angegeben ist</span><span class="sxs-lookup"><span data-stu-id="6288a-1637">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="6288a-1638">Geändert, um Rollenzuweisung zum Subnetz zu überspringen, wenn bereits eine Zuweisung vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="6288a-1638">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="6288a-1639">AppService</span><span class="sxs-lookup"><span data-stu-id="6288a-1639">AppService</span></span>

* <span data-ttu-id="6288a-1640">Fehler behoben, der das Erstellen einer Funktions-App mithilfe von Speicherkonten in externen Ressourcengruppen verhinderte</span><span class="sxs-lookup"><span data-stu-id="6288a-1640">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="6288a-1641">Absturz bei ZIP-Bereitstellung behoben</span><span class="sxs-lookup"><span data-stu-id="6288a-1641">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="6288a-1642">Batch AI</span><span class="sxs-lookup"><span data-stu-id="6288a-1642">BatchAI</span></span>

* <span data-ttu-id="6288a-1643">Protokollierungsausgabe für die automatische Speicherkontoerstellung geändert, sodass nun „Ressourcen*gruppe*“ angegeben wird</span><span class="sxs-lookup"><span data-stu-id="6288a-1643">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="6288a-1644">Container</span><span class="sxs-lookup"><span data-stu-id="6288a-1644">Container</span></span>

* <span data-ttu-id="6288a-1645">`--secure-environment-variables` zum Übergeben sicherer Umgebungsvariablen an einen Container hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1645">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="6288a-1646">IoT</span><span class="sxs-lookup"><span data-stu-id="6288a-1646">IoT</span></span>

* <span data-ttu-id="6288a-1647">[BREAKING CHANGE] Veraltete Befehle entfernt, die in die IoT-Erweiterung verschoben wurden</span><span class="sxs-lookup"><span data-stu-id="6288a-1647">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="6288a-1648">Elemente aktualisiert, um nicht die Domäne `azure-devices.net` anzunehmen</span><span class="sxs-lookup"><span data-stu-id="6288a-1648">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="6288a-1649">Iot Central</span><span class="sxs-lookup"><span data-stu-id="6288a-1649">Iot Central</span></span>

* <span data-ttu-id="6288a-1650">Erstes Release des IoT Central-Moduls</span><span class="sxs-lookup"><span data-stu-id="6288a-1650">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="6288a-1651">KeyVault</span><span class="sxs-lookup"><span data-stu-id="6288a-1651">KeyVault</span></span>


* <span data-ttu-id="6288a-1652">Befehle zum Verwalten von Speicherkonten und SAS-Definitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1652">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="6288a-1653">Befehle für Netzwerkregeln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1653">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="6288a-1654">Parameter `--id` zu Geheimnis-, Schlüssel- und Zertifikatvorgängen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1654">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="6288a-1655">Unterstützung für Version mit mehreren APIs zur Schlüsseltresorverwaltung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1655">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="6288a-1656">Unterstützung für Version mit mehreren APIs zur Schlüsseltresordatenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1656">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="6288a-1657">Relay</span><span class="sxs-lookup"><span data-stu-id="6288a-1657">Relay</span></span>

* <span data-ttu-id="6288a-1658">Erste Veröffentlichung</span><span class="sxs-lookup"><span data-stu-id="6288a-1658">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="6288a-1659">Sql</span><span class="sxs-lookup"><span data-stu-id="6288a-1659">Sql</span></span>

* <span data-ttu-id="6288a-1660">Befehle vom Typ `sql failover-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1660">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="6288a-1661">Storage</span><span class="sxs-lookup"><span data-stu-id="6288a-1661">Storage</span></span>

* <span data-ttu-id="6288a-1662">[BREAKING CHANGE]`storage account show-usage` geändert, um Parameter `--location` erforderlich zu machen. Auflistung nach Region</span><span class="sxs-lookup"><span data-stu-id="6288a-1662">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="6288a-1663">Parameter `--resource-group` geändert, sodass er für `storage account`-Befehle optional ist</span><span class="sxs-lookup"><span data-stu-id="6288a-1663">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="6288a-1664">Warnungen vom Typ „Fehler bei Vorbedingung“ für einzelne Fehler in Batch-Befehlen für eine aggregiert Nachricht entfernt</span><span class="sxs-lookup"><span data-stu-id="6288a-1664">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="6288a-1665">`[blob|file] delete-batch`-Befehle geändert, sodass kein Array mit Null-Werten mehr ausgegeben wird</span><span class="sxs-lookup"><span data-stu-id="6288a-1665">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="6288a-1666">`blob [download|upload|delete-batch]`-Befehle geändert, um SAS-Token aus Container-URL zu lesen</span><span class="sxs-lookup"><span data-stu-id="6288a-1666">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="6288a-1667">VM</span><span class="sxs-lookup"><span data-stu-id="6288a-1667">VM</span></span>

* <span data-ttu-id="6288a-1668">Allgemeine Filter zu `vm list-skus` für höhere Benutzerfreundlichkeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1668">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="6288a-1669">31. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="6288a-1669">July 31, 2018</span></span>

<span data-ttu-id="6288a-1670">Version 2.0.43</span><span class="sxs-lookup"><span data-stu-id="6288a-1670">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="6288a-1671">ACR</span><span class="sxs-lookup"><span data-stu-id="6288a-1671">ACR</span></span>

* <span data-ttu-id="6288a-1672">Flag `--with-secure-properties` zum Befehl `acr build-task show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1672">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="6288a-1673">Befehl `acr build-task update-build` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1673">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="6288a-1674">ACS</span><span class="sxs-lookup"><span data-stu-id="6288a-1674">ACS</span></span>

* <span data-ttu-id="6288a-1675">Änderung, um 0 (Erfolg) zurückzugeben, wenn `az aks browse` durch Drücken von [STRG+C] beendet wird</span><span class="sxs-lookup"><span data-stu-id="6288a-1675">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="6288a-1676">Batch</span><span class="sxs-lookup"><span data-stu-id="6288a-1676">Batch</span></span>

* <span data-ttu-id="6288a-1677">Korrektur eines Fehlers bei der Anzeige des AAD-Tokens in Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="6288a-1677">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="6288a-1678">Container</span><span class="sxs-lookup"><span data-stu-id="6288a-1678">Container</span></span>

* <span data-ttu-id="6288a-1679">Voraussetzung von `--log-analytics-workspace-key` für Name oder ID im festgelegten Abonnement entfernt</span><span class="sxs-lookup"><span data-stu-id="6288a-1679">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="6288a-1680">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6288a-1680">Network</span></span>

* <span data-ttu-id="6288a-1681">DNS-Unterstützung zu „2017-03-09-profile“ für Azure Stack hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1681">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="6288a-1682">Resource</span><span class="sxs-lookup"><span data-stu-id="6288a-1682">Resource</span></span>

* <span data-ttu-id="6288a-1683">`--rollback-on-error` zu `group deployment create` hinzugefügt, um bei einem Fehler eine als funktionierend bekannte Bereitstellung auszuführen</span><span class="sxs-lookup"><span data-stu-id="6288a-1683">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="6288a-1684">Problem behoben, aufgrund dessen `--parameters {}` mit `group deployment create` zu einem Fehler führte</span><span class="sxs-lookup"><span data-stu-id="6288a-1684">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="6288a-1685">Role</span><span class="sxs-lookup"><span data-stu-id="6288a-1685">Role</span></span>

* <span data-ttu-id="6288a-1686">Unterstützung für das Stack-Profil „2017-03-09-profile“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1686">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="6288a-1687">Problem behoben, aufgrund dessen das generische Update von Parametern auf `app update` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="6288a-1687">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="6288a-1688">Suchen,</span><span class="sxs-lookup"><span data-stu-id="6288a-1688">Search</span></span>

* <span data-ttu-id="6288a-1689">Befehle für Azure Search-Dienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1689">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="6288a-1690">Service Bus</span><span class="sxs-lookup"><span data-stu-id="6288a-1690">Service Bus</span></span>

* <span data-ttu-id="6288a-1691">Migrationsbefehlsgruppe hinzugefügt, um einen Namespace von Service Bus Standard zu Premium zu migrieren</span><span class="sxs-lookup"><span data-stu-id="6288a-1691">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="6288a-1692">Neue optionale Eigenschaften zu Service Bus-Warteschlange und -Abonnement hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1692">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="6288a-1693">`--enable-batched-operations` und `--enable-dead-lettering-on-message-expiration` in `queue`</span><span class="sxs-lookup"><span data-stu-id="6288a-1693">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="6288a-1694">`--dead-letter-on-filter-exceptions` in `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="6288a-1694">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="6288a-1695">Storage</span><span class="sxs-lookup"><span data-stu-id="6288a-1695">Storage</span></span>

* <span data-ttu-id="6288a-1696">Unterstützung für den Download großer Dateien über eine einzelne Verbindung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1696">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="6288a-1697">`show`-Befehle konvertiert, bei denen im Falle einer fehlenden Ressource kein Fehler mit dem Exitcode 3 ausgelöst wurde</span><span class="sxs-lookup"><span data-stu-id="6288a-1697">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="6288a-1698">VM</span><span class="sxs-lookup"><span data-stu-id="6288a-1698">VM</span></span>

* <span data-ttu-id="6288a-1699">Unterstützung zum Auflisten von Verfügbarkeitsgruppen nach Abonnement hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1699">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="6288a-1700">Unterstützung für `StandardSSD_LRS` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-1700">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="6288a-1701">Unterstützung für Anwendungssicherheitsgruppe beim Erstellen einer VM-Skalierungsgruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1701">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="6288a-1702">[BREAKING CHANGE]`[vm|vmss] create`, `[vm|vmss] identity assign` und `[vm|vmss] identity remove` wurden geändert, um vom Benutzer zugewiesene Identitäten im Wörterbuchformat auszugeben.</span><span class="sxs-lookup"><span data-stu-id="6288a-1702">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="6288a-1703">18. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="6288a-1703">July 18, 2018</span></span>

<span data-ttu-id="6288a-1704">Version 2.0.42</span><span class="sxs-lookup"><span data-stu-id="6288a-1704">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="6288a-1705">Core</span><span class="sxs-lookup"><span data-stu-id="6288a-1705">Core</span></span>

* <span data-ttu-id="6288a-1706">Unterstützung für browserbasierte Anmeldung WSL-Bash-Fenster hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1706">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="6288a-1707">`--force-string`-Flag für alle generischen Updatebefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1707">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="6288a-1708">[BREAKING CHANGE] Befehle vom Typ „show“ so geändert, dass die Fehlermeldung protokolliert wird und der Vorgang bei einer fehlenden Ressource mit dem Exitcode 3 fehlschlägt</span><span class="sxs-lookup"><span data-stu-id="6288a-1708">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="6288a-1709">ACR</span><span class="sxs-lookup"><span data-stu-id="6288a-1709">ACR</span></span>

* <span data-ttu-id="6288a-1710">[BREAKING CHANGE] „--no-push“ in Befehl „acr build“ in reines Flag geändert</span><span class="sxs-lookup"><span data-stu-id="6288a-1710">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="6288a-1711">Befehle `show` und `update` unter Gruppe `acr repository` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1711">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="6288a-1712">`--detail`-Flag für `show-manifests` und `show-tags` hinzugefügt, um ausführlichere Informationen anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="6288a-1712">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="6288a-1713">Parameter `--image` zur Unterstützung des Abrufs von Builddetails oder Protokollen anhand eines Images hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1713">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="6288a-1714">ACS</span><span class="sxs-lookup"><span data-stu-id="6288a-1714">ACS</span></span>

* <span data-ttu-id="6288a-1715">`az aks create` so geändert, dass mit Fehler beendet wird, wenn `--max-pods` kleiner als 5 ist</span><span class="sxs-lookup"><span data-stu-id="6288a-1715">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="6288a-1716">AppService</span><span class="sxs-lookup"><span data-stu-id="6288a-1716">AppService</span></span>

* <span data-ttu-id="6288a-1717">Unterstützung für PremiumV2-SKUs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1717">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="6288a-1718">Batch</span><span class="sxs-lookup"><span data-stu-id="6288a-1718">Batch</span></span>

* <span data-ttu-id="6288a-1719">Korrektur eines Fehlers bei der Verwendung von Anmeldeinformationen im Cloud Shell-Modus</span><span class="sxs-lookup"><span data-stu-id="6288a-1719">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="6288a-1720">JSON-Eingabe so geändert, dass Groß-/Kleinschreibung nicht beachtet wird</span><span class="sxs-lookup"><span data-stu-id="6288a-1720">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="6288a-1721">Batch KI</span><span class="sxs-lookup"><span data-stu-id="6288a-1721">Batch AI</span></span>

* <span data-ttu-id="6288a-1722">Befehl `az batchai job exec` korrigiert</span><span class="sxs-lookup"><span data-stu-id="6288a-1722">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="6288a-1723">Container</span><span class="sxs-lookup"><span data-stu-id="6288a-1723">Container</span></span>

* <span data-ttu-id="6288a-1724">Anforderung von Benutzername und Kennwort für Nicht-DockerHub-Registrierungen entfernt</span><span class="sxs-lookup"><span data-stu-id="6288a-1724">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="6288a-1725">Fehler beim Erstellen von Containergruppen aus YAML-Datei behoben</span><span class="sxs-lookup"><span data-stu-id="6288a-1725">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="6288a-1726">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6288a-1726">Network</span></span>

* <span data-ttu-id="6288a-1727">Unterstützung für `--no-wait` zu `network nic [create|update|delete]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1727">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="6288a-1728">`network nic wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1728">Added `network nic wait`</span></span>
* <span data-ttu-id="6288a-1729">`--ids`-Argument für `network vnet [subnet|peering] list` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="6288a-1729">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="6288a-1730">`--include-default`-Flag hinzugefügt, um Standardsicherheitsregeln in die Ausgabe von `network nsg rule list` aufzunehmen</span><span class="sxs-lookup"><span data-stu-id="6288a-1730">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="6288a-1731">Resource</span><span class="sxs-lookup"><span data-stu-id="6288a-1731">Resource</span></span>

* <span data-ttu-id="6288a-1732">Unterstützung für `--no-wait` zu `group deployment delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1732">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="6288a-1733">Unterstützung für `--no-wait` zu `deployment delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1733">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="6288a-1734">Befehl `deployment wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1734">Added `deployment wait` command</span></span>
* <span data-ttu-id="6288a-1735">Problem behoben, aufgrund dessen die `az deployment`-Befehle auf Abonnementebene fälschlicherweise für Profil „2017-03-09-profile“ angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="6288a-1735">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="6288a-1736">SQL</span><span class="sxs-lookup"><span data-stu-id="6288a-1736">SQL</span></span>

* <span data-ttu-id="6288a-1737">Fehler „Der angegebene Ressourcengruppenname ... entsprach nicht dem Namen in der URL“ beim Angeben des Namens des Pools für elastische Datenbanken für `sql db copy`-und `sql db replica create`-Befehle behoben</span><span class="sxs-lookup"><span data-stu-id="6288a-1737">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="6288a-1738">Konfigurieren des Standard-SQL Servers durch Ausführen von `az configure --defaults sql-server=<name>` zulässig</span><span class="sxs-lookup"><span data-stu-id="6288a-1738">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="6288a-1739">Tabellenformatierer für Befehle `sql server`, `sql server firewall-rule`, `sql list-usages` und `sql show-usage` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1739">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="6288a-1740">Storage</span><span class="sxs-lookup"><span data-stu-id="6288a-1740">Storage</span></span>

* <span data-ttu-id="6288a-1741">`pageRanges`-Eigenschaft zu `storage blob show`-Ausgabe hinzugefügt, die für Seitenblobs ausgefüllt wird</span><span class="sxs-lookup"><span data-stu-id="6288a-1741">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="6288a-1742">VM</span><span class="sxs-lookup"><span data-stu-id="6288a-1742">VM</span></span>

* <span data-ttu-id="6288a-1743">[BREAKING CHANGE]`vmss create` so geändert, dass `Standard_DS1_v2` als standardmäßige Instanzgröße verwendet wird</span><span class="sxs-lookup"><span data-stu-id="6288a-1743">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="6288a-1744">Unterstützung für `--no-wait` zu `vm extension [set|delete]` und `vmss extension [set|delete]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1744">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="6288a-1745">`vm extension wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1745">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="6288a-1746">3\. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="6288a-1746">July 3, 2018</span></span>

<span data-ttu-id="6288a-1747">Version 2.0.41</span><span class="sxs-lookup"><span data-stu-id="6288a-1747">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="6288a-1748">AKS</span><span class="sxs-lookup"><span data-stu-id="6288a-1748">AKS</span></span>

* <span data-ttu-id="6288a-1749">Überwachung geändert, sodass Abonnement-ID verwendet wird</span><span class="sxs-lookup"><span data-stu-id="6288a-1749">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="6288a-1750">3\. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="6288a-1750">July 3, 2018</span></span>

<span data-ttu-id="6288a-1751">Version 2.0.40</span><span class="sxs-lookup"><span data-stu-id="6288a-1751">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="6288a-1752">Core</span><span class="sxs-lookup"><span data-stu-id="6288a-1752">Core</span></span>

* <span data-ttu-id="6288a-1753">Neuer Autorisierungscode-Flow für interaktive Anmeldung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1753">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="6288a-1754">ACR</span><span class="sxs-lookup"><span data-stu-id="6288a-1754">ACR</span></span>

* <span data-ttu-id="6288a-1755">Abruf-Buildstatus hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1755">Added polling build status</span></span>
* <span data-ttu-id="6288a-1756">Unterstützung für Enumerationswerte ohne Berücksichtigung von Groß-/Kleinschreibung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1756">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="6288a-1757">Parameter `--top` und `--orderby` für `show-manifests` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1757">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="6288a-1758">ACS</span><span class="sxs-lookup"><span data-stu-id="6288a-1758">ACS</span></span>

* <span data-ttu-id="6288a-1759">[BREAKING CHANGE] Standardmäßiges Aktivieren der rollenbasierten Zugriffssteuerung für Kubernetes</span><span class="sxs-lookup"><span data-stu-id="6288a-1759">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="6288a-1760">Argument `--disable-rbac` hinzugefügt und `--enable-rbac` als veraltet festgelegt, da es nun der Standard ist</span><span class="sxs-lookup"><span data-stu-id="6288a-1760">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="6288a-1761">Optionen für Befehl `aks browse` wurden aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="6288a-1761">Updated options for `aks browse` command.</span></span> <span data-ttu-id="6288a-1762">Unterstützung für `--listen-port` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1762">Added `--listen-port` support</span></span>
* <span data-ttu-id="6288a-1763">Standardmäßiges Helm-Diagrammpaket für Befehl `aks install-connector` wurde aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="6288a-1763">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="6288a-1764">Verwenden von „virtual-kubelet-for-aks-latest.tgz“</span><span class="sxs-lookup"><span data-stu-id="6288a-1764">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="6288a-1765">Befehle `aks enable-addons` und `aks disable-addons` zum Aktualisieren eines vorhandenen Clusters hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1765">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="6288a-1766">AppService</span><span class="sxs-lookup"><span data-stu-id="6288a-1766">AppService</span></span>

* <span data-ttu-id="6288a-1767">Unterstützung für das Deaktivieren der Identität über `webapp identity remove` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1767">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="6288a-1768">`preview`-Tag für Identitätsfunktion entfernt</span><span class="sxs-lookup"><span data-stu-id="6288a-1768">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="6288a-1769">Backup</span><span class="sxs-lookup"><span data-stu-id="6288a-1769">Backup</span></span>

* <span data-ttu-id="6288a-1770">Moduldefinition aktualisiert</span><span class="sxs-lookup"><span data-stu-id="6288a-1770">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="6288a-1771">Batch AI</span><span class="sxs-lookup"><span data-stu-id="6288a-1771">BatchAI</span></span>

* <span data-ttu-id="6288a-1772">Tabellenausgabe für Befehle `batchai cluster node list` und `batchai job node list` korrigiert</span><span class="sxs-lookup"><span data-stu-id="6288a-1772">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="6288a-1773">Cloud</span><span class="sxs-lookup"><span data-stu-id="6288a-1773">Cloud</span></span>

* <span data-ttu-id="6288a-1774">Serversuffix `acr login` zu Cloudkonfiguration hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1774">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="6288a-1775">Container</span><span class="sxs-lookup"><span data-stu-id="6288a-1775">Container</span></span>

* <span data-ttu-id="6288a-1776">`container create` zu Standard für Vorgang mit langer Ausführungsdauer geändert</span><span class="sxs-lookup"><span data-stu-id="6288a-1776">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="6288a-1777">Log Analytics-Parameter `--log-analytics-workspace` und `--log-analytics-workspace-key` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1777">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="6288a-1778">Parameter `--protocol` zum Festlegen des zu verwendenden Netzwerkprotokolls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1778">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="6288a-1779">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="6288a-1779">Extension</span></span>

* <span data-ttu-id="6288a-1780">`extension list-available` geändert, sodass nur mit der CLI-Version kompatible Erweiterungen angezeigt werden</span><span class="sxs-lookup"><span data-stu-id="6288a-1780">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="6288a-1781">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6288a-1781">Network</span></span>

* <span data-ttu-id="6288a-1782">Problem behoben, aufgrund dessen bei Datensatztypen die Groß-/Kleinschreibung beachtet werden musste ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="6288a-1782">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="6288a-1783">Rdbms</span><span class="sxs-lookup"><span data-stu-id="6288a-1783">Rdbms</span></span>

* <span data-ttu-id="6288a-1784">Befehle vom Typ `[postgres|myql] server vnet-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1784">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="6288a-1785">Resource</span><span class="sxs-lookup"><span data-stu-id="6288a-1785">Resource</span></span>

* <span data-ttu-id="6288a-1786">Neue Vorgangsgruppe `deployment` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1786">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="6288a-1787">VM</span><span class="sxs-lookup"><span data-stu-id="6288a-1787">VM</span></span>

* <span data-ttu-id="6288a-1788">Unterstützung für das Entfernen der vom System zugewiesenen Identität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1788">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="6288a-1789">25. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="6288a-1789">June 25, 2018</span></span>

<span data-ttu-id="6288a-1790">Version 2.0.39</span><span class="sxs-lookup"><span data-stu-id="6288a-1790">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="6288a-1791">Befehlszeilenschnittstelle (CLI)</span><span class="sxs-lookup"><span data-stu-id="6288a-1791">CLI</span></span>

* <span data-ttu-id="6288a-1792">Dateieinschränkung in MSI-Installer aktualisiert, um Problem mit der Erweiterungsinstallation zu beheben</span><span class="sxs-lookup"><span data-stu-id="6288a-1792">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="6288a-1793">19. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="6288a-1793">June 19, 2018</span></span>

<span data-ttu-id="6288a-1794">Version 2.0.38</span><span class="sxs-lookup"><span data-stu-id="6288a-1794">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="6288a-1795">Core</span><span class="sxs-lookup"><span data-stu-id="6288a-1795">Core</span></span>

* <span data-ttu-id="6288a-1796">Globale Unterstützung für `--subscription` zu den meisten Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1796">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="6288a-1797">ACR</span><span class="sxs-lookup"><span data-stu-id="6288a-1797">ACR</span></span>

* <span data-ttu-id="6288a-1798">`azure-storage-blob` als Abhängigkeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1798">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="6288a-1799">CPU-Standardkonfiguration für `acr build-task create` geändert, sodass zwei Kerne verwendet werden</span><span class="sxs-lookup"><span data-stu-id="6288a-1799">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="6288a-1800">ACS</span><span class="sxs-lookup"><span data-stu-id="6288a-1800">ACS</span></span>

* <span data-ttu-id="6288a-1801">Optionen des Befehls `aks use-dev-spaces` wurden aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="6288a-1801">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="6288a-1802">Unterstützung für `--update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1802">Added `--update` support</span></span>
* <span data-ttu-id="6288a-1803">`aks get-credentials --admin` geändert, sodass der Benutzerkontext in `$HOME/.kube/config` ersetzt wird</span><span class="sxs-lookup"><span data-stu-id="6288a-1803">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="6288a-1804">Schreibgeschützte `nodeResourceGroup`-Eigenschaft in verwalteten Clustern verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="6288a-1804">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="6288a-1805">Befehlsfehler `acs browse` korrigiert</span><span class="sxs-lookup"><span data-stu-id="6288a-1805">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="6288a-1806">`--connector-name` für `aks install-connector`, `aks upgrade-connector` und `aks remove-connector` als optional festgelegt</span><span class="sxs-lookup"><span data-stu-id="6288a-1806">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="6288a-1807">Neue Azure Container Instances-Regionen für `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1807">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="6288a-1808">Normalisierter Speicherort im Helm-Versionsnamen und Knotenname zu `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1808">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="6288a-1809">AppService</span><span class="sxs-lookup"><span data-stu-id="6288a-1809">AppService</span></span>

* <span data-ttu-id="6288a-1810">Unterstützung für neuere Versionen von „urllib“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1810">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="6288a-1811">Unterstützung der Verwendung eines App Service-Plans aus externen Ressourcengruppen zu `functionapp create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1811">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="6288a-1812">Batch</span><span class="sxs-lookup"><span data-stu-id="6288a-1812">Batch</span></span>

* <span data-ttu-id="6288a-1813">`azure-batch-extensions`-Abhängigkeit entfernt</span><span class="sxs-lookup"><span data-stu-id="6288a-1813">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="6288a-1814">Batch KI</span><span class="sxs-lookup"><span data-stu-id="6288a-1814">Batch AI</span></span>

* <span data-ttu-id="6288a-1815">Unterstützung für Arbeitsbereiche wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-1815">Added support for workspaces.</span></span> <span data-ttu-id="6288a-1816">Arbeitsbereiche ermöglichen das Zusammenfassen von Clustern, Dateiservern und Experimenten in Gruppen ohne Beschränkung der Anzahl von Ressourcen, die erstellt werden können.</span><span class="sxs-lookup"><span data-stu-id="6288a-1816">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="6288a-1817">Unterstützung für Experimente wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-1817">Added support for experiments.</span></span> <span data-ttu-id="6288a-1818">Experimente ermöglichen das Zusammenfassen von Aufträgen in Sammlungen ohne Beschränkung der Anzahl von erstellten Aufträgen.</span><span class="sxs-lookup"><span data-stu-id="6288a-1818">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="6288a-1819">Unterstützung für das Konfigurieren von `/dev/shm` für Aufträge hinzugefügt, die in einem Docker-Container ausgeführt werden</span><span class="sxs-lookup"><span data-stu-id="6288a-1819">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="6288a-1820">Die Befehle `batchai cluster node exec` und `batchai job node exec` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-1820">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="6288a-1821">Diese Befehle ermöglichen die Ausführung aller Befehle direkt auf Knoten und bieten Funktionen zur Portweiterleitung.</span><span class="sxs-lookup"><span data-stu-id="6288a-1821">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="6288a-1822">Unterstützung für `--ids` zu `batchai`-Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1822">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="6288a-1823">[BREAKING CHANGE] Alle Cluster und Dateiserver müssen unter Arbeitsbereichen erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="6288a-1823">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="6288a-1824">[BREAKING CHANGE] Aufträge müssen unter Experimenten erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="6288a-1824">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="6288a-1825">[BREAKING CHANGE]`--nfs-resource-group` wurde aus den Befehlen `cluster create` und `job create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="6288a-1825">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="6288a-1826">Geben Sie zum Bereitstellen eines NFS, das einem anderen Arbeitsbereich/einer anderen Ressourcengruppe angehört, die ARM-ID des Dateiservers über die Option `--nfs` an.</span><span class="sxs-lookup"><span data-stu-id="6288a-1826">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="6288a-1827">[BREAKING CHANGE]`--cluster-resource-group` wurde aus dem Befehl `job create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="6288a-1827">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="6288a-1828">Geben Sie zum Übermitteln eines Auftrags, der einem anderen Arbeitsbereich/einer anderen Ressourcengruppe angehört, die ARM-ID des Clusters über die Option `--cluster` an.</span><span class="sxs-lookup"><span data-stu-id="6288a-1828">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="6288a-1829">[BREAKING CHANGE] Attribut `location` wurde aus Aufträgen, Clustern und Dateiservern entfernt.</span><span class="sxs-lookup"><span data-stu-id="6288a-1829">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="6288a-1830">„Location“ ist jetzt ein Attribut eines Arbeitsbereichs.</span><span class="sxs-lookup"><span data-stu-id="6288a-1830">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="6288a-1831">[BREAKING CHANGE]`--location` wurde aus den Befehlen `job create`, `cluster create` und `file-server create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="6288a-1831">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="6288a-1832">[BREAKING CHANGE] Namen von Kurzoptionen wurden geändert, um die Schnittstelle konsistenter zu machen:</span><span class="sxs-lookup"><span data-stu-id="6288a-1832">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="6288a-1833">[`--config`, `-c`] in [`--config-file`, `-f`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="6288a-1833">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="6288a-1834">[`--cluster`, `-r`] in [`--cluster`, `-c`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="6288a-1834">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="6288a-1835">[`--cluster`, `-n`] in [`--cluster`, `-c`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="6288a-1835">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="6288a-1836">[`--job`, `-n`] in [`--job`, `-j`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="6288a-1836">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="6288a-1837">Karten</span><span class="sxs-lookup"><span data-stu-id="6288a-1837">Maps</span></span>

* <span data-ttu-id="6288a-1838">[BREAKING CHANGE]`maps account create` wurde so geändert, dass Nutzungsbedingungen entweder durch interaktive Eingabeaufforderung oder `--accept-tos`-Flag akzeptiert werden müssen.</span><span class="sxs-lookup"><span data-stu-id="6288a-1838">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="6288a-1839">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6288a-1839">Network</span></span>

* <span data-ttu-id="6288a-1840">Unterstützung für `https` zu `network lb probe create` hinzugefügt [Nr. 6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="6288a-1840">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="6288a-1841">Problem behoben, aufgrund dessen die Groß-/Kleinschreibung von `--endpoint-status` berücksichtigt wurde.</span><span class="sxs-lookup"><span data-stu-id="6288a-1841">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="6288a-1842">#6502</span><span class="sxs-lookup"><span data-stu-id="6288a-1842">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="6288a-1843">Reservations</span><span class="sxs-lookup"><span data-stu-id="6288a-1843">Reservations</span></span>

* <span data-ttu-id="6288a-1844">[BREAKING CHANGE] Erforderlicher Parameter `ReservedResourceType` zu `reservations catalog show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1844">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="6288a-1845">Parameter `Location` zu `reservations catalog show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1845">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="6288a-1846">[BREAKING CHANGE]`kind` aus `ReservationProperties` entfernt</span><span class="sxs-lookup"><span data-stu-id="6288a-1846">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="6288a-1847">[BREAKING CHANGE]`capabilities` wurde in `Catalog` in `sku_properties` umbenannt</span><span class="sxs-lookup"><span data-stu-id="6288a-1847">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="6288a-1848">[BREAKING CHANGE] Eigenschaften `size` und `tier` aus `Catalog` entfernt</span><span class="sxs-lookup"><span data-stu-id="6288a-1848">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="6288a-1849">Parameter `InstanceFlexibility` zu `reservations reservation update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1849">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="6288a-1850">Role</span><span class="sxs-lookup"><span data-stu-id="6288a-1850">Role</span></span>

* <span data-ttu-id="6288a-1851">Fehlerbehandlung verbessert</span><span class="sxs-lookup"><span data-stu-id="6288a-1851">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="6288a-1852">SQL</span><span class="sxs-lookup"><span data-stu-id="6288a-1852">SQL</span></span>

* <span data-ttu-id="6288a-1853">Verwirrender Fehler behoben, der beim Ausführen von `az sql db list-editions` für einen Ort auftrat, der für Ihr Abonnement nicht verfügbar ist</span><span class="sxs-lookup"><span data-stu-id="6288a-1853">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="6288a-1854">Storage</span><span class="sxs-lookup"><span data-stu-id="6288a-1854">Storage</span></span>

* <span data-ttu-id="6288a-1855">Lesbarkeit der Tabellenausgabe für `storage blob download` verbessert</span><span class="sxs-lookup"><span data-stu-id="6288a-1855">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="6288a-1856">VM</span><span class="sxs-lookup"><span data-stu-id="6288a-1856">VM</span></span>

* <span data-ttu-id="6288a-1857">Verbesserte Einschränkung der VM-Größenüberprüfung für Unterstützung von beschleunigten Netzwerken in `vm create`</span><span class="sxs-lookup"><span data-stu-id="6288a-1857">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="6288a-1858">Warnung für `vmss create` hinzugefügt, dass die VM-Standardgröße von `Standard_D1_v2` auf `Standard_DS1_v2` umgestellt wird</span><span class="sxs-lookup"><span data-stu-id="6288a-1858">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="6288a-1859">`--force-update` zu `[vm|vmss] extension set` hinzugefügt, um die Erweiterung auch dann zu aktualisieren, wenn die Konfiguration nicht geändert wurde</span><span class="sxs-lookup"><span data-stu-id="6288a-1859">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="6288a-1860">13. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="6288a-1860">June 13, 2018</span></span>

<span data-ttu-id="6288a-1861">Version 2.0.37</span><span class="sxs-lookup"><span data-stu-id="6288a-1861">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="6288a-1862">Core</span><span class="sxs-lookup"><span data-stu-id="6288a-1862">Core</span></span>

* <span data-ttu-id="6288a-1863">Verbesserte interaktive Telemetrie</span><span class="sxs-lookup"><span data-stu-id="6288a-1863">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="6288a-1864">13. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="6288a-1864">June 13, 2018</span></span>

<span data-ttu-id="6288a-1865">Version 2.0.36</span><span class="sxs-lookup"><span data-stu-id="6288a-1865">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="6288a-1866">AKS</span><span class="sxs-lookup"><span data-stu-id="6288a-1866">AKS</span></span>

* <span data-ttu-id="6288a-1867">Zusätzliche erweiterte Netzwerkoptionen zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1867">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="6288a-1868">Argumente zu `aks create` zum Aktivieren der Überwachung und HTTP-Routing hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1868">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="6288a-1869">Argument `--no-ssh-key` zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1869">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="6288a-1870">Argument `--enable-rbac` zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1870">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="6288a-1871">[VORSCHAUVERSION] Unterstützung für Azure Active Directory-Authentifizierung zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1871">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="6288a-1872">AppService</span><span class="sxs-lookup"><span data-stu-id="6288a-1872">AppService</span></span>

* <span data-ttu-id="6288a-1873">Problem mit inkompatiblen urllib-Versionen behoben</span><span class="sxs-lookup"><span data-stu-id="6288a-1873">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="6288a-1874">5\. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="6288a-1874">June 5, 2018</span></span>

<span data-ttu-id="6288a-1875">Version 2.0.35</span><span class="sxs-lookup"><span data-stu-id="6288a-1875">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="6288a-1876">Interactive</span><span class="sxs-lookup"><span data-stu-id="6288a-1876">Interactive</span></span>

* <span data-ttu-id="6288a-1877">Grenzwerte für die Abhängigkeiten des interaktiven Modus hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1877">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="6288a-1878">5\. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="6288a-1878">June 5, 2018</span></span>

<span data-ttu-id="6288a-1879">Version 2.0.34</span><span class="sxs-lookup"><span data-stu-id="6288a-1879">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="6288a-1880">Core</span><span class="sxs-lookup"><span data-stu-id="6288a-1880">Core</span></span>

* <span data-ttu-id="6288a-1881">Unterstützung für mandantenübergreifende Ressourcenverweise hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1881">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="6288a-1882">Verbesserte Zuverlässigkeit bei Telemetrieuploads</span><span class="sxs-lookup"><span data-stu-id="6288a-1882">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="6288a-1883">ACR</span><span class="sxs-lookup"><span data-stu-id="6288a-1883">ACR</span></span>

* <span data-ttu-id="6288a-1884">Unterstützung für VSTS als Remotequellort hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1884">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="6288a-1885">Befehl `acr import` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1885">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="6288a-1886">AKS</span><span class="sxs-lookup"><span data-stu-id="6288a-1886">AKS</span></span>

* <span data-ttu-id="6288a-1887">`aks get-credentials` wurde geändert, um die Kube-Konfigurationsdatei mit sichereren Dateisystemberechtigungen zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="6288a-1887">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="6288a-1888">Batch</span><span class="sxs-lookup"><span data-stu-id="6288a-1888">Batch</span></span>

* <span data-ttu-id="6288a-1889">Fehler bei der Formatierung der Poollistentabelle behoben [[Problem 4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="6288a-1889">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="6288a-1890">IoT</span><span class="sxs-lookup"><span data-stu-id="6288a-1890">IOT</span></span>

* <span data-ttu-id="6288a-1891">Unterstützung für das Erstellen von IoT Hub-Instanzen im Tarif „Basic“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1891">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="6288a-1892">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6288a-1892">Network</span></span>

* <span data-ttu-id="6288a-1893">`network vnet peering` wurde verbessert.</span><span class="sxs-lookup"><span data-stu-id="6288a-1893">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="6288a-1894">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="6288a-1894">Policy Insights</span></span>

* <span data-ttu-id="6288a-1895">Erstrelease</span><span class="sxs-lookup"><span data-stu-id="6288a-1895">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="6288a-1896">ARM</span><span class="sxs-lookup"><span data-stu-id="6288a-1896">ARM</span></span>

* <span data-ttu-id="6288a-1897">Befehle vom Typ `account management-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1897">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="6288a-1898">SQL</span><span class="sxs-lookup"><span data-stu-id="6288a-1898">SQL</span></span>

* <span data-ttu-id="6288a-1899">Neue Befehle für verwaltete Instanzen hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="6288a-1899">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="6288a-1900">Neue Befehle für verwaltete Datenbanken hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="6288a-1900">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="6288a-1901">Storage</span><span class="sxs-lookup"><span data-stu-id="6288a-1901">Storage</span></span>

* <span data-ttu-id="6288a-1902">Zusätzliche MimeTypes für JSON und JavaScript hinzugefügt (abzuleiten aus Dateierweiterungen)</span><span class="sxs-lookup"><span data-stu-id="6288a-1902">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="6288a-1903">VM</span><span class="sxs-lookup"><span data-stu-id="6288a-1903">VM</span></span>

* <span data-ttu-id="6288a-1904">`vm list-skus` wurde geändert, um feste Spalten zu verwenden und eine Warnung hinzuzufügen, dass `Tier` und `Size` entfernt werden.</span><span class="sxs-lookup"><span data-stu-id="6288a-1904">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="6288a-1905">Option `--accelerated-networking` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1905">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="6288a-1906">`--tags` zu `identity create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1906">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="6288a-1907">22. Mai 2018</span><span class="sxs-lookup"><span data-stu-id="6288a-1907">May 22, 2018</span></span>

<span data-ttu-id="6288a-1908">Version 2.0.33</span><span class="sxs-lookup"><span data-stu-id="6288a-1908">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="6288a-1909">Core</span><span class="sxs-lookup"><span data-stu-id="6288a-1909">Core</span></span>

* <span data-ttu-id="6288a-1910">Unterstützung für das Erweitern von `@` in Dateinamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1910">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="6288a-1911">ACS</span><span class="sxs-lookup"><span data-stu-id="6288a-1911">ACS</span></span>

* <span data-ttu-id="6288a-1912">Neue Dev Spaces-Befehle `aks use-dev-spaces` und `aks remove-dev-spaces` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1912">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="6288a-1913">Tippfehler in Hilfemeldung korrigiert</span><span class="sxs-lookup"><span data-stu-id="6288a-1913">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="6288a-1914">AppService</span><span class="sxs-lookup"><span data-stu-id="6288a-1914">AppService</span></span>

* <span data-ttu-id="6288a-1915">Verbesserte generische Aktualisierungsbefehle</span><span class="sxs-lookup"><span data-stu-id="6288a-1915">Improved generic update commands</span></span>
* <span data-ttu-id="6288a-1916">Asynchrone Unterstützung für `webapp deployment source config-zip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1916">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="6288a-1917">Container</span><span class="sxs-lookup"><span data-stu-id="6288a-1917">Container</span></span>

* <span data-ttu-id="6288a-1918">Unterstützung für das Exportieren einer Containergruppe im YAML-Format hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1918">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="6288a-1919">Unterstützung für die Verwendung einer YAML-Datei zum Erstellen/Aktualisieren einer Containergruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1919">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="6288a-1920">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="6288a-1920">Extension</span></span>

* <span data-ttu-id="6288a-1921">Verbesserte Entfernung von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="6288a-1921">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="6288a-1922">Interactive</span><span class="sxs-lookup"><span data-stu-id="6288a-1922">Interactive</span></span>

* <span data-ttu-id="6288a-1923">Protokollierung geändert, um Parser für Abschlüsse zu deaktivieren</span><span class="sxs-lookup"><span data-stu-id="6288a-1923">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="6288a-1924">Verbesserte Verarbeitung beschädigter Hilfscaches</span><span class="sxs-lookup"><span data-stu-id="6288a-1924">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="6288a-1925">KeyVault</span><span class="sxs-lookup"><span data-stu-id="6288a-1925">KeyVault</span></span>

* <span data-ttu-id="6288a-1926">keyvault-Befehle wurden korrigiert, damit sie in Cloud Shell oder auf virtuellen Computern mit Identität verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="6288a-1926">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="6288a-1927">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6288a-1927">Network</span></span>

* <span data-ttu-id="6288a-1928">Problem behoben, aufgrund dessen `network watcher show-topology` nicht mit einem VNET und/oder Subnetznamen verwendet werden konnte ([#6326](https://github.com/Azure/azure-cli/issues/6326))</span><span class="sxs-lookup"><span data-stu-id="6288a-1928">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="6288a-1929">Problem behoben, aufgrund dessen einige `network watcher`-Befehle fälschlicherweise angaben, dass Network Watcher nicht für bestimmte Regionen aktiviert ist ([#6264](https://github.com/Azure/azure-cli/issues/6264))</span><span class="sxs-lookup"><span data-stu-id="6288a-1929">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="6288a-1930">SQL</span><span class="sxs-lookup"><span data-stu-id="6288a-1930">SQL</span></span>

* <span data-ttu-id="6288a-1931">[BREAKING CHANGE] Von den Befehlen `db` und `dw` zurückgegebene Antwortobjekte geändert:</span><span class="sxs-lookup"><span data-stu-id="6288a-1931">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="6288a-1932">Eigenschaft `serviceLevelObjective` in `currentServiceObjectiveName` umbenannt</span><span class="sxs-lookup"><span data-stu-id="6288a-1932">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="6288a-1933">Eigenschaften `currentServiceObjectiveId` und `requestedServiceObjectiveId` entfernt</span><span class="sxs-lookup"><span data-stu-id="6288a-1933">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="6288a-1934">Eigenschaft `maxSizeBytes` geändert (ist nun keine Zeichenfolge mehr, sondern ein Ganzzahlwert)</span><span class="sxs-lookup"><span data-stu-id="6288a-1934">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="6288a-1935">[BREAKING CHANGE] Die folgenden `db`- und `dw`-Eigenschaften wurden geändert und sind jetzt schreibgeschützt:</span><span class="sxs-lookup"><span data-stu-id="6288a-1935">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="6288a-1936">[https://login.microsoftonline.com/consumers/](`requestedServiceObjectiveName`).</span><span class="sxs-lookup"><span data-stu-id="6288a-1936">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="6288a-1937">Verwenden Sie zum Aktualisieren den Parameter `--service-objective`, oder legen Sie die Eigenschaft `sku.name` fest.</span><span class="sxs-lookup"><span data-stu-id="6288a-1937">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="6288a-1938">[https://login.microsoftonline.com/consumers/](`edition`).</span><span class="sxs-lookup"><span data-stu-id="6288a-1938">`edition`.</span></span> <span data-ttu-id="6288a-1939">Verwenden Sie zum Aktualisieren den Parameter `--edition`, oder legen Sie die Eigenschaft `sku.tier` fest.</span><span class="sxs-lookup"><span data-stu-id="6288a-1939">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="6288a-1940">[https://login.microsoftonline.com/consumers/](`elasticPoolName`).</span><span class="sxs-lookup"><span data-stu-id="6288a-1940">`elasticPoolName`.</span></span> <span data-ttu-id="6288a-1941">Verwenden Sie zum Aktualisieren den Parameter `--elastic-pool`, oder legen Sie die Eigenschaft `elasticPoolId` fest.</span><span class="sxs-lookup"><span data-stu-id="6288a-1941">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="6288a-1942">[BREAKING CHANGE] Die folgenden `elastic-pool`-Eigenschaften wurden geändert und sind jetzt schreibgeschützt:</span><span class="sxs-lookup"><span data-stu-id="6288a-1942">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="6288a-1943">[https://login.microsoftonline.com/consumers/](`edition`).</span><span class="sxs-lookup"><span data-stu-id="6288a-1943">`edition`.</span></span> <span data-ttu-id="6288a-1944">Verwenden Sie zum Aktualisieren den Parameter `--edition`.</span><span class="sxs-lookup"><span data-stu-id="6288a-1944">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="6288a-1945">[https://login.microsoftonline.com/consumers/](`dtu`).</span><span class="sxs-lookup"><span data-stu-id="6288a-1945">`dtu`.</span></span> <span data-ttu-id="6288a-1946">Verwenden Sie zum Aktualisieren den Parameter `--capacity`.</span><span class="sxs-lookup"><span data-stu-id="6288a-1946">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="6288a-1947">[https://login.microsoftonline.com/consumers/](`databaseDtuMin`).</span><span class="sxs-lookup"><span data-stu-id="6288a-1947">`databaseDtuMin`.</span></span> <span data-ttu-id="6288a-1948">Verwenden Sie zum Aktualisieren den Parameter `--db-min-capacity`.</span><span class="sxs-lookup"><span data-stu-id="6288a-1948">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="6288a-1949">[https://login.microsoftonline.com/consumers/](`databaseDtuMax`).</span><span class="sxs-lookup"><span data-stu-id="6288a-1949">`databaseDtuMax`.</span></span> <span data-ttu-id="6288a-1950">Verwenden Sie zum Aktualisieren den Parameter `--db-max-capacity`.</span><span class="sxs-lookup"><span data-stu-id="6288a-1950">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="6288a-1951">Die Parameter `--family` und `--capacity` wurden zu den `db`-, `dw`- und `elastic-pool`-Befehlen hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-1951">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="6288a-1952">Den `db`-, `dw`- und `elastic-pool`-Befehlen wurden Tabellenformatierer hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-1952">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="6288a-1953">Storage</span><span class="sxs-lookup"><span data-stu-id="6288a-1953">Storage</span></span>

* <span data-ttu-id="6288a-1954">Vervollständigung für das Argument `--account-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1954">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="6288a-1955">Problem mit `storage entity query` behoben</span><span class="sxs-lookup"><span data-stu-id="6288a-1955">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="6288a-1956">VM</span><span class="sxs-lookup"><span data-stu-id="6288a-1956">VM</span></span>

* <span data-ttu-id="6288a-1957">[BREAKING CHANGE]`--write-accelerator` aus `vm create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="6288a-1957">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="6288a-1958">Die gleiche Unterstützung kann über `vm update` oder `vm disk attach` erzielt werden.</span><span class="sxs-lookup"><span data-stu-id="6288a-1958">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="6288a-1959">Erweiterungsimageabgleich in `[vm|vmss] extension` korrigiert</span><span class="sxs-lookup"><span data-stu-id="6288a-1959">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="6288a-1960">`--boot-diagnostics-storage` zu `vm create` zur Erfassung des Startprotokolls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1960">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="6288a-1961">`--license-type` zu `[vm|vmss] update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1961">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="6288a-1962">7\. Mai 2018</span><span class="sxs-lookup"><span data-stu-id="6288a-1962">May 7, 2018</span></span>

<span data-ttu-id="6288a-1963">Version 2.0.32</span><span class="sxs-lookup"><span data-stu-id="6288a-1963">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="6288a-1964">Core</span><span class="sxs-lookup"><span data-stu-id="6288a-1964">Core</span></span>

* <span data-ttu-id="6288a-1965">Ein Ausnahmefehler wurde behoben, der beim Abrufen von Geheimnissen aus einem Dienstprinzipalkonto mit Zertifikat auftrat.</span><span class="sxs-lookup"><span data-stu-id="6288a-1965">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="6288a-1966">Eingeschränkte Unterstützung für positionelle Argumente hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1966">Added limited support for positional arguments</span></span>
* <span data-ttu-id="6288a-1967">Problem behoben, aufgrund dessen `--query` nicht mit `--ids` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="6288a-1967">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="6288a-1968">#5591</span><span class="sxs-lookup"><span data-stu-id="6288a-1968">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="6288a-1969">Pipingszenarien von Befehlen bei Verwendung von `--ids` verbessert</span><span class="sxs-lookup"><span data-stu-id="6288a-1969">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="6288a-1970">Unterstützt `-o tsv` mit angegebener Abfrage bzw. `-o json` ohne angegeben Abfrage</span><span class="sxs-lookup"><span data-stu-id="6288a-1970">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="6288a-1971">Befehlsvorschläge bei Fehler hinzugefügt, wenn Befehle Tippfehler enthielten</span><span class="sxs-lookup"><span data-stu-id="6288a-1971">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="6288a-1972">Fehler bei der Eingabe von `az ''` behandelt</span><span class="sxs-lookup"><span data-stu-id="6288a-1972">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="6288a-1973">Unterstützung für benutzerdefinierte Ressourcentypen für Befehlsmodule und -erweiterungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1973">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="6288a-1974">ACR</span><span class="sxs-lookup"><span data-stu-id="6288a-1974">ACR</span></span>

* <span data-ttu-id="6288a-1975">ACR Build-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1975">Added ACR Build commands</span></span>
* <span data-ttu-id="6288a-1976">Fehlermeldungen vom Typ „Ressource nicht gefunden.“ verbessert</span><span class="sxs-lookup"><span data-stu-id="6288a-1976">Improved resource not found error messages</span></span>
* <span data-ttu-id="6288a-1977">Höhere Leistung bei der Ressourcenerstellung und optimierte Fehlerbehandlung</span><span class="sxs-lookup"><span data-stu-id="6288a-1977">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="6288a-1978">ACR-Anmeldung bei nicht standardmäßigen Konsolen und WSL optimiert</span><span class="sxs-lookup"><span data-stu-id="6288a-1978">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="6288a-1979">Fehlermeldungen zu Repositorybefehlen optimiert</span><span class="sxs-lookup"><span data-stu-id="6288a-1979">Improved repository commands error messages</span></span>
* <span data-ttu-id="6288a-1980">Tabellenspalten und -reihenfolge aktualisiert</span><span class="sxs-lookup"><span data-stu-id="6288a-1980">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="6288a-1981">ACS</span><span class="sxs-lookup"><span data-stu-id="6288a-1981">ACS</span></span>

* <span data-ttu-id="6288a-1982">Warnung hinzugefügt, dass `az aks` eine Vorschauversion des Diensts ist</span><span class="sxs-lookup"><span data-stu-id="6288a-1982">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="6288a-1983">Berechtigungsproblem in `aks install-connector` behoben, wenn `--aci-resource-group` nicht angegeben wird</span><span class="sxs-lookup"><span data-stu-id="6288a-1983">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="6288a-1984">AMS</span><span class="sxs-lookup"><span data-stu-id="6288a-1984">AMS</span></span>

* <span data-ttu-id="6288a-1985">Erste Version: Verwalten von Azure Media Services-Ressourcen</span><span class="sxs-lookup"><span data-stu-id="6288a-1985">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="6288a-1986">AppService</span><span class="sxs-lookup"><span data-stu-id="6288a-1986">Appservice</span></span>

* <span data-ttu-id="6288a-1987">Ein Problem in `webapp delete` wurde behoben, das bei Angabe von `--slot` auftrat.</span><span class="sxs-lookup"><span data-stu-id="6288a-1987">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="6288a-1988">`--runtime-version` aus `webapp auth update` entfernt</span><span class="sxs-lookup"><span data-stu-id="6288a-1988">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="6288a-1989">Unterstützung für „min\_tls\_version“ und „https2.0“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1989">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="6288a-1990">Unterstützung für mehrere Container hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1990">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="6288a-1991">Batch KI</span><span class="sxs-lookup"><span data-stu-id="6288a-1991">Batch AI</span></span>

* <span data-ttu-id="6288a-1992">`batchai create cluster` wurde geändert, um die in der Konfigurationsdatei des Clusters konfigurierte VM-Priorität zu berücksichtigen.</span><span class="sxs-lookup"><span data-stu-id="6288a-1992">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="6288a-1993">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="6288a-1993">Cognitive Services</span></span>

* <span data-ttu-id="6288a-1994">Tippfehler im Beispiel für `cognitiveservices account create` behoben [Nr. 5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="6288a-1994">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="6288a-1995">Nutzung</span><span class="sxs-lookup"><span data-stu-id="6288a-1995">Consumption</span></span>

* <span data-ttu-id="6288a-1996">Neue Befehle für Budget-API hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-1996">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="6288a-1997">Container</span><span class="sxs-lookup"><span data-stu-id="6288a-1997">Container</span></span>

* <span data-ttu-id="6288a-1998">`--registry-server` muss nicht mehr für `container create` angegeben werden, wenn ein Registrierungsserver im Imagenamen enthalten ist.</span><span class="sxs-lookup"><span data-stu-id="6288a-1998">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="6288a-1999">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="6288a-1999">Cosmos DB</span></span>

* <span data-ttu-id="6288a-2000">VNET-Unterstützung für Azure CLI eingeführt: Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="6288a-2000">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="6288a-2001">DMS</span><span class="sxs-lookup"><span data-stu-id="6288a-2001">DMS</span></span>

* <span data-ttu-id="6288a-2002">Erste Version: Die Migration von SQL zu Azure SQL wird nun unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6288a-2002">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="6288a-2003">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="6288a-2003">Extension</span></span>

* <span data-ttu-id="6288a-2004">Fehler behoben, aufgrund dessen Erweiterungsmetadaten nicht mehr angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="6288a-2004">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="6288a-2005">Interactive</span><span class="sxs-lookup"><span data-stu-id="6288a-2005">Interactive</span></span>

* <span data-ttu-id="6288a-2006">Interaktive Vervollständigung funktioniert nun auch mit positionellen Argumenten.</span><span class="sxs-lookup"><span data-stu-id="6288a-2006">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="6288a-2007">Benutzerfreundlichere Ausgabe bei der Eingabe von '\'</span><span class="sxs-lookup"><span data-stu-id="6288a-2007">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="6288a-2008">Abschlüsse für Parameter ohne Hilfe korrigiert</span><span class="sxs-lookup"><span data-stu-id="6288a-2008">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="6288a-2009">Beschreibungen für Befehlsgruppen korrigiert</span><span class="sxs-lookup"><span data-stu-id="6288a-2009">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="6288a-2010">Labor</span><span class="sxs-lookup"><span data-stu-id="6288a-2010">Lab</span></span>

* <span data-ttu-id="6288a-2011">Regressionen aus Knack-Umwandlung korrigiert</span><span class="sxs-lookup"><span data-stu-id="6288a-2011">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="6288a-2012">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6288a-2012">Network</span></span>

* <span data-ttu-id="6288a-2013">[BREAKING CHANGE] Parameter `--ids` entfernt für:</span><span class="sxs-lookup"><span data-stu-id="6288a-2013">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="6288a-2014">Profil</span><span class="sxs-lookup"><span data-stu-id="6288a-2014">Profile</span></span>

* <span data-ttu-id="6288a-2015">Quellerkennung für `disk create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="6288a-2015">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="6288a-2016">[BREAKING CHANGE]`--msi-port` und `--identity-port` entfernt, da sie nicht mehr verwendet werden</span><span class="sxs-lookup"><span data-stu-id="6288a-2016">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="6288a-2017">Tippfehler in kurzer Zusammenfassung für `account get-access-token` korrigiert</span><span class="sxs-lookup"><span data-stu-id="6288a-2017">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="6288a-2018">Redis</span><span class="sxs-lookup"><span data-stu-id="6288a-2018">Redis</span></span>

* <span data-ttu-id="6288a-2019">`redis patch-schedule patch-schedule show` wurde durch `redis patch-schedule show` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="6288a-2019">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="6288a-2020">`redis list-all` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="6288a-2020">Deprecated `redis list-all`.</span></span> <span data-ttu-id="6288a-2021">Diese Funktion wurde in `redis list` integriert.</span><span class="sxs-lookup"><span data-stu-id="6288a-2021">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="6288a-2022">`redis import-method` wurde durch `redis import` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="6288a-2022">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="6288a-2023">Unterstützung für `--ids` zu verschiedenen Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2023">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="6288a-2024">Role</span><span class="sxs-lookup"><span data-stu-id="6288a-2024">Role</span></span>

* <span data-ttu-id="6288a-2025">[BREAKING CHANGE] Veralteter Befehl `ad sp reset-credentials` entfernt</span><span class="sxs-lookup"><span data-stu-id="6288a-2025">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="6288a-2026">Storage</span><span class="sxs-lookup"><span data-stu-id="6288a-2026">Storage</span></span>

* <span data-ttu-id="6288a-2027">Zulassen, dass das Ziel-SAS-Token für die Blobkopie auf die Quelle angewendet wird, wenn Quell-SAS und Kontoschlüssel nicht angegeben werden</span><span class="sxs-lookup"><span data-stu-id="6288a-2027">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="6288a-2028">Verfügbar gemacht: Socket-Timeout für Blobuploads und -downloads</span><span class="sxs-lookup"><span data-stu-id="6288a-2028">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="6288a-2029">Blobnamen, die mit Pfadtrennzeichen beginnen, als relative Pfade behandeln</span><span class="sxs-lookup"><span data-stu-id="6288a-2029">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="6288a-2030">Zulassen, dass `storage blob copy --source-sas` mit dem Abfragezeichen „?“ beginnt</span><span class="sxs-lookup"><span data-stu-id="6288a-2030">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="6288a-2031">`storage entity query --marker` korrigiert, um Liste von Schlüsselwerten zu akzeptieren</span><span class="sxs-lookup"><span data-stu-id="6288a-2031">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="6288a-2032">VM</span><span class="sxs-lookup"><span data-stu-id="6288a-2032">VM</span></span>

* <span data-ttu-id="6288a-2033">Ungültige Erkennungslogik für nicht verwalteten Blob-URI korrigiert</span><span class="sxs-lookup"><span data-stu-id="6288a-2033">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="6288a-2034">Unterstützung für Datenträgerverschlüsselung ohne vom Benutzer bereitgestellte Dienstprinzipale hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2034">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="6288a-2035">[BREAKING CHANGE] Verwenden Sie nicht „ManagedIdentityExtension“ des virtuellen Computers für MSI-Unterstützung.</span><span class="sxs-lookup"><span data-stu-id="6288a-2035">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="6288a-2036">Unterstützung für Entfernungsrichtlinie zu `vmss` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2036">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="6288a-2037">[BREAKING CHANGE]`--ids` entfernt aus:</span><span class="sxs-lookup"><span data-stu-id="6288a-2037">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="6288a-2038">Unterstützung für Schreibbeschleunigung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2038">Added write accelerator support</span></span>
* <span data-ttu-id="6288a-2039">`vmss perform-maintenance` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2039">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="6288a-2040">`vm diagnostics set` korrigiert, um zuverlässig den Betriebssystemtyp des virtuellen Computers zu erkennen</span><span class="sxs-lookup"><span data-stu-id="6288a-2040">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="6288a-2041">`vm resize` geändert, um zu überprüfen, ob die angeforderte Größe von der derzeit festgelegten Größe abweicht, und nur bei einer Änderung eine Aktualisierung auszuführen</span><span class="sxs-lookup"><span data-stu-id="6288a-2041">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="6288a-2042">10. April 2018</span><span class="sxs-lookup"><span data-stu-id="6288a-2042">April 10, 2018</span></span>

<span data-ttu-id="6288a-2043">Version 2.0.31</span><span class="sxs-lookup"><span data-stu-id="6288a-2043">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="6288a-2044">ACR</span><span class="sxs-lookup"><span data-stu-id="6288a-2044">ACR</span></span>

* <span data-ttu-id="6288a-2045">Verbesserte Fehlerbehandlung für wincred-Fallback</span><span class="sxs-lookup"><span data-stu-id="6288a-2045">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="6288a-2046">ACS</span><span class="sxs-lookup"><span data-stu-id="6288a-2046">ACS</span></span>

* <span data-ttu-id="6288a-2047">Gültigkeit von per AKS erstellten SPNs in fünf Jahre geändert</span><span class="sxs-lookup"><span data-stu-id="6288a-2047">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="6288a-2048">AppService</span><span class="sxs-lookup"><span data-stu-id="6288a-2048">Appservice</span></span>

* [BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="6288a-2050">Nicht abgefangene Ausnahme für nicht vorhandene Web-App-Pläne behoben</span><span class="sxs-lookup"><span data-stu-id="6288a-2050">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="6288a-2051">Batch AI</span><span class="sxs-lookup"><span data-stu-id="6288a-2051">BatchAI</span></span>

* <span data-ttu-id="6288a-2052">Unterstützung für API 2018-03-01 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2052">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="6288a-2053">Bereitstellung auf Auftragsebene</span><span class="sxs-lookup"><span data-stu-id="6288a-2053">Job level mounting</span></span>
  - <span data-ttu-id="6288a-2054">Umgebungsvariablen mit Geheimniswerten</span><span class="sxs-lookup"><span data-stu-id="6288a-2054">Environment variables with secret values</span></span>
  - <span data-ttu-id="6288a-2055">Einstellungen von Leistungsindikatoren</span><span class="sxs-lookup"><span data-stu-id="6288a-2055">Performance counters settings</span></span>
  - <span data-ttu-id="6288a-2056">Berichtstellung für auftragsspezifisches Pfadsegment</span><span class="sxs-lookup"><span data-stu-id="6288a-2056">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="6288a-2057">Unterstützung für Unterordner in Listendateien-API</span><span class="sxs-lookup"><span data-stu-id="6288a-2057">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="6288a-2058">Berichterstellung zur Nutzung und zu Grenzwerten</span><span class="sxs-lookup"><span data-stu-id="6288a-2058">Usage and limits reporting</span></span>
  - <span data-ttu-id="6288a-2059">Zulassen der Angabe des Cachetyps für NFS-Server</span><span class="sxs-lookup"><span data-stu-id="6288a-2059">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="6288a-2060">Unterstützung für benutzerdefinierte Images</span><span class="sxs-lookup"><span data-stu-id="6288a-2060">Support for custom images</span></span>
  - <span data-ttu-id="6288a-2061">Unterstützung für pyTorch-Toolkit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2061">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="6288a-2062">Befehl `job wait` hinzugefügt, der das Warten auf die Auftragsfertigstellung ermöglicht und den Code für die Auftragsbeendigung meldet</span><span class="sxs-lookup"><span data-stu-id="6288a-2062">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="6288a-2063">Befehl `usage show` hinzugefügt, mit dem die aktuelle Nutzung von Batch KI-Ressourcen und die Grenzwerte für verschiedene Regionen aufgelistet werden</span><span class="sxs-lookup"><span data-stu-id="6288a-2063">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="6288a-2064">Nationale Clouds werden unterstützt</span><span class="sxs-lookup"><span data-stu-id="6288a-2064">National clouds are supported</span></span>
* <span data-ttu-id="6288a-2065">Befehlszeilenargumente für Aufträge hinzugefügt, um das Bereitstellen von Dateisystemen auf Auftragsebene zusätzlich zu Konfigurationsdateien zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="6288a-2065">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="6288a-2066">Weitere Optionen zum Anpassen von Clustern hinzugefügt – VM-Priorität, Subnetz, anfängliche Knotenanzahl für Cluster mit automatischer Skalierung, Angeben eines benutzerdefinierten Images</span><span class="sxs-lookup"><span data-stu-id="6288a-2066">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="6288a-2067">Befehlszeilenoption zum Angeben des Cachetyps für NFS mit Verwaltung per Batch KI hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2067">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="6288a-2068">Angeben der Bereitstellung von Dateisystemen in Konfigurationsdateien vereinfacht.</span><span class="sxs-lookup"><span data-stu-id="6288a-2068">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="6288a-2069">Weglassen von Anmeldeinformationen für Azure-Dateifreigaben und Azure-Blobcontainer ist jetzt möglich. Die CLI füllt fehlende Anmeldeinformationen auf, indem der Speicherkontoschlüssel verwendet wird, der über Befehlszeilenparameter oder per Umgebungsvariable angegeben wird, oder der Schlüssel wird über Azure Storage abgefragt (sofern das Speicherkonto zum aktuellen Abonnement gehört).</span><span class="sxs-lookup"><span data-stu-id="6288a-2069">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="6288a-2070">Der Befehl zum Streamen von Auftragsdateien wird jetzt automatisch abgeschlossen, nachdem der Auftrag beendet ist (Erfolg, Fehler, Beendigung oder Löschung)</span><span class="sxs-lookup"><span data-stu-id="6288a-2070">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="6288a-2071">Verbesserte `table`-Ausgabe für `show`-Vorgänge</span><span class="sxs-lookup"><span data-stu-id="6288a-2071">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="6288a-2072">Option `--use-auto-storage` für die Clustererstellung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-2072">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="6288a-2073">Diese Option erleichtert die Verwaltung von Speicherkonten und die Bereitstellung von Azure-Dateifreigaben und Azure-Blobcontainern in Clustern.</span><span class="sxs-lookup"><span data-stu-id="6288a-2073">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="6288a-2074">`--generate-ssh-keys` für `cluster create` und `file-server create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2074">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="6288a-2075">Möglichkeit zum Angeben der Knotensetupaufgabe über die Befehlszeile</span><span class="sxs-lookup"><span data-stu-id="6288a-2075">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="6288a-2076">[BREAKING CHANGE] Befehl `job stream-file` und `job list-files` in die Gruppe `job file` verschoben</span><span class="sxs-lookup"><span data-stu-id="6288a-2076">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="6288a-2077">[BREAKING CHANGE]`--admin-user-name` im Befehl `file-server create` in `--user-name` umbenannt, um Einheitlichkeit mit dem Befehl `cluster create` zu erzielen</span><span class="sxs-lookup"><span data-stu-id="6288a-2077">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="6288a-2078">Abrechnung</span><span class="sxs-lookup"><span data-stu-id="6288a-2078">Billing</span></span>

* <span data-ttu-id="6288a-2079">Registrierungskontobefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2079">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="6288a-2080">Nutzung</span><span class="sxs-lookup"><span data-stu-id="6288a-2080">Consumption</span></span>

* <span data-ttu-id="6288a-2081">Befehle vom Typ `marketplace` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2081">Added `marketplace` commands</span></span>
* <span data-ttu-id="6288a-2082">[BREAKING CHANGE]`reservations summaries` in `reservation summary` umbenannt</span><span class="sxs-lookup"><span data-stu-id="6288a-2082">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="6288a-2083">[BREAKING CHANGE]`reservations details` in `reservation detail` umbenannt</span><span class="sxs-lookup"><span data-stu-id="6288a-2083">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="6288a-2084">[BREAKING CHANGE] Kurzoptionen `--reservation-order-id` und `--reservation-id` für `reservation`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="6288a-2084">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="6288a-2085">[BREAKING CHANGE]`--grain`-Kurzoptionen für `reservation summary`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="6288a-2085">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="6288a-2086">[BREAKING CHANGE]`--include-meter-details`-Kurzoptionen für `pricesheet`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="6288a-2086">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="6288a-2087">Container</span><span class="sxs-lookup"><span data-stu-id="6288a-2087">Container</span></span>

* <span data-ttu-id="6288a-2088">Parameter für die Volumebereitstellung für das Git-Repository hinzugefügt: `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` und `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="6288a-2088">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="6288a-2089">[#5926](https://github.com/Azure/azure-cli/issues/5926) behoben: Fehler bei `az container exec`, wenn „--container-name“ angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="6288a-2089">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="6288a-2090">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="6288a-2090">Extension</span></span>

* <span data-ttu-id="6288a-2091">Meldung für Distributionsüberprüfung in Debugebene geändert</span><span class="sxs-lookup"><span data-stu-id="6288a-2091">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="6288a-2092">Interactive</span><span class="sxs-lookup"><span data-stu-id="6288a-2092">Interactive</span></span>

* <span data-ttu-id="6288a-2093">Geändert: Verhinderung des Abschlusses bei nicht erkannten Befehlen</span><span class="sxs-lookup"><span data-stu-id="6288a-2093">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="6288a-2094">Ereignishooks vor und nach der Erstellung der Teilstruktur von Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2094">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="6288a-2095">Abschluss für `--ids`-Parameter hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2095">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="6288a-2096">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6288a-2096">Network</span></span>

* <span data-ttu-id="6288a-2097">[#5936](https://github.com/Azure/azure-cli/issues/5936) behoben: `application-gateway create`-Tags konnten nicht festgelegt werden</span><span class="sxs-lookup"><span data-stu-id="6288a-2097">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="6288a-2098">Argument `--auth-certs` zum Anfügen von Authentifizierungszertifikaten für `application-gateway http-settings [create|update]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-2098">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="6288a-2099">#4910</span><span class="sxs-lookup"><span data-stu-id="6288a-2099">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="6288a-2100">`ddos-protection`-Befehle zum Erstellen von DDoS-Schutzplänen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2100">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="6288a-2101">Unterstützung von `--ddos-protection-plan` für `vnet [create|update]` hinzugefügt, um das Zuordnen eines VNET zu einem DDoS-Schutzplan zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="6288a-2101">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="6288a-2102">Problem mit `--disable-bgp-route-propagation`-Flag in `network route-table [create|update]` behoben</span><span class="sxs-lookup"><span data-stu-id="6288a-2102">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="6288a-2103">Dummy-Argumente `--public-ip-address-type` und `--subnet-type` für `network lb [create|update]` entfernt</span><span class="sxs-lookup"><span data-stu-id="6288a-2103">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="6288a-2104">Unterstützung für TXT-Datensätze mit RFC 1035-Escapesequenzen für `network dns zone [import|export]` und `network dns record-set txt add-record` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2104">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="6288a-2105">Profil</span><span class="sxs-lookup"><span data-stu-id="6288a-2105">Profile</span></span>

* <span data-ttu-id="6288a-2106">Unterstützung für klassische Azure-Konten in `account list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2106">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="6288a-2107">[BREAKING CHANGE]`--msi` & `--msi-port`-Argumente entfernt</span><span class="sxs-lookup"><span data-stu-id="6288a-2107">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="6288a-2108">RDBMS</span><span class="sxs-lookup"><span data-stu-id="6288a-2108">RDBMS</span></span>

* <span data-ttu-id="6288a-2109">Befehl `georestore` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2109">Added `georestore` command</span></span>
* <span data-ttu-id="6288a-2110">Speichergrößenbeschränkung aus Befehl `create` entfernt</span><span class="sxs-lookup"><span data-stu-id="6288a-2110">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="6288a-2111">Resource</span><span class="sxs-lookup"><span data-stu-id="6288a-2111">Resource</span></span>

* <span data-ttu-id="6288a-2112">Unterstützung für `--metadata` zu `policy definition create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2112">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="6288a-2113">Unterstützung von `--metadata`, `--set`, `--add`, `--remove` für `policy definition update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2113">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="6288a-2114">SQL</span><span class="sxs-lookup"><span data-stu-id="6288a-2114">SQL</span></span>

* <span data-ttu-id="6288a-2115">`sql elastic-pool op list` und `sql elastic-pool op cancel` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2115">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="6288a-2116">Storage</span><span class="sxs-lookup"><span data-stu-id="6288a-2116">Storage</span></span>

* <span data-ttu-id="6288a-2117">Fehlermeldungen für falsch formatierte Verbindungszeichenfolgen verbessert</span><span class="sxs-lookup"><span data-stu-id="6288a-2117">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="6288a-2118">VM</span><span class="sxs-lookup"><span data-stu-id="6288a-2118">VM</span></span>

* <span data-ttu-id="6288a-2119">Unterstützung für die Konfiguration der Plattform-Fehlerdomänenanzahl für `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2119">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="6288a-2120">`vmss create` geändert, damit standardmäßig „Standard LB“ für zonales, großes oder per einzelner Platzierungsgruppe deaktiviertes Scale Set festgelegt wird</span><span class="sxs-lookup"><span data-stu-id="6288a-2120">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret`
* <span data-ttu-id="6288a-2122">Unterstützung für SKU mit öffentlicher IP für `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2122">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="6288a-2123">Argumente `--keyvault` und `--resource-group` für `vm secret format` hinzugefügt, um Szenarien zu unterstützen, bei denen der Befehl die Tresor-ID nicht auflösen kann.</span><span class="sxs-lookup"><span data-stu-id="6288a-2123">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="6288a-2124">#5718</span><span class="sxs-lookup"><span data-stu-id="6288a-2124">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="6288a-2125">Bessere Fehler für `[vm|vmss create]`, wenn der Standort einer Ressourcengruppe keine Zonenunterstützung aufweist</span><span class="sxs-lookup"><span data-stu-id="6288a-2125">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="6288a-2126">27. März 2018</span><span class="sxs-lookup"><span data-stu-id="6288a-2126">March 27, 2018</span></span>

<span data-ttu-id="6288a-2127">Version 2.0.30</span><span class="sxs-lookup"><span data-stu-id="6288a-2127">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="6288a-2128">Core</span><span class="sxs-lookup"><span data-stu-id="6288a-2128">Core</span></span>

* <span data-ttu-id="6288a-2129">Anzeigen einer Meldung für Erweiterungen, die in der Hilfe als Vorschauversion gekennzeichnet sind</span><span class="sxs-lookup"><span data-stu-id="6288a-2129">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="6288a-2130">ACS</span><span class="sxs-lookup"><span data-stu-id="6288a-2130">ACS</span></span>

* <span data-ttu-id="6288a-2131">Behebung eines Fehlers bei der SSL-Zertifikatprüfung für `aks install-cli` in Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="6288a-2131">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="6288a-2132">AppService</span><span class="sxs-lookup"><span data-stu-id="6288a-2132">Appservice</span></span>

* <span data-ttu-id="6288a-2133">Unterstützung nur von HTTPS zu `webapp update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2133">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="6288a-2134">Unterstützung für Slots zu `az webapp identity [assign|show]` und `az functionapp identity [assign|show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2134">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="6288a-2135">Backup</span><span class="sxs-lookup"><span data-stu-id="6288a-2135">Backup</span></span>

* <span data-ttu-id="6288a-2136">Neuer Befehl `az backup protection isenabled-for-vm` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-2136">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="6288a-2137">Mit diesem Befehl kann überprüft werden, ob ein virtueller Computer von einem beliebigen Tresor im Abonnement gesichert wird.</span><span class="sxs-lookup"><span data-stu-id="6288a-2137">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="6288a-2138">Azure-Objekt-IDs für Parameter `--resource-group` und `--vault-name` für die folgenden Befehle aktiviert:</span><span class="sxs-lookup"><span data-stu-id="6288a-2138">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="6288a-2139">`--name`-Parameter wurden geändert, um das Ausgabeformat von `backup ... show`-Befehlen zu akzeptieren.</span><span class="sxs-lookup"><span data-stu-id="6288a-2139">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="6288a-2140">Container</span><span class="sxs-lookup"><span data-stu-id="6288a-2140">Container</span></span>

* <span data-ttu-id="6288a-2141">Befehl `container exec` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-2141">Added `container exec` command.</span></span> <span data-ttu-id="6288a-2142">Ausführung von Befehlen in einem Container für eine ausgeführte Containergruppe</span><span class="sxs-lookup"><span data-stu-id="6288a-2142">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="6288a-2143">Zulassen der Tabellenausgabe zum Erstellen und Aktualisieren einer Containergruppe</span><span class="sxs-lookup"><span data-stu-id="6288a-2143">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="6288a-2144">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="6288a-2144">Extension</span></span>

* <span data-ttu-id="6288a-2145">Meldung für `extension add` hinzugefügt, wenn sich die Erweiterung in der Vorschauphase befindet</span><span class="sxs-lookup"><span data-stu-id="6288a-2145">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="6288a-2146">`extension list-available` geändert, um vollständige Erweiterungsdaten mit `--show-details` anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="6288a-2146">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="6288a-2147">[BREAKING CHANGE]`extension list-available` geändert, um standardmäßig vereinfachte Erweiterungsdaten anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="6288a-2147">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="6288a-2148">Interactive</span><span class="sxs-lookup"><span data-stu-id="6288a-2148">Interactive</span></span>

* <span data-ttu-id="6288a-2149">Vervollständigungen wurden geändert und werden jetzt aktiviert, sobald das Laden der Befehlstabelle abgeschlossen ist.</span><span class="sxs-lookup"><span data-stu-id="6288a-2149">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="6288a-2150">Fehler bei der Verwendung des Parameters `--style` behoben</span><span class="sxs-lookup"><span data-stu-id="6288a-2150">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="6288a-2151">Interaktiver Lexer nach Befehlstabellensicherung instanziiert (sofern nicht vorhanden)</span><span class="sxs-lookup"><span data-stu-id="6288a-2151">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="6288a-2152">Verbesserte Unterstützung der Vervollständigung</span><span class="sxs-lookup"><span data-stu-id="6288a-2152">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="6288a-2153">Labor</span><span class="sxs-lookup"><span data-stu-id="6288a-2153">Lab</span></span>

* <span data-ttu-id="6288a-2154">Probleme mit Befehl `create environment` behoben</span><span class="sxs-lookup"><span data-stu-id="6288a-2154">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="6288a-2155">Überwachen</span><span class="sxs-lookup"><span data-stu-id="6288a-2155">Monitor</span></span>

* <span data-ttu-id="6288a-2156">Unterstützung für `--top`, `--orderby` und `--namespace` zu `metrics list` hinzugefügt [Nr. 5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="6288a-2156">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="6288a-2157">[#4529](https://github.com/Azure/azure-cli/issues/5785) behoben: `metrics list` akzeptiert eine durch Leerzeichen getrennte Liste von abzurufenden Metriken</span><span class="sxs-lookup"><span data-stu-id="6288a-2157">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="6288a-2158">Unterstützung für `--namespace` zu `metrics list-definitions` hinzugefügt [Nr. 5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="6288a-2158">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="6288a-2159">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6288a-2159">Network</span></span>

* <span data-ttu-id="6288a-2160">Unterstützung für private DNS-Zonen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2160">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="6288a-2161">Profil</span><span class="sxs-lookup"><span data-stu-id="6288a-2161">Profile</span></span>

* <span data-ttu-id="6288a-2162">Warnung für `--identity-port` und `--msi-port` zu `login` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2162">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="6288a-2163">RDBMS</span><span class="sxs-lookup"><span data-stu-id="6288a-2163">RDBMS</span></span>

* <span data-ttu-id="6288a-2164">GA-API-Version 2017-12-01 (Geschäftsmodell) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2164">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="6288a-2165">Resource</span><span class="sxs-lookup"><span data-stu-id="6288a-2165">Resource</span></span>

* [BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="6288a-2167">Role</span><span class="sxs-lookup"><span data-stu-id="6288a-2167">Role</span></span>

* <span data-ttu-id="6288a-2168">Unterstützung für erforderliche Zugriffskonfigurationen und native Clients zu `az ad app create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2168">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="6288a-2169">`rbac`-Befehle geändert, um maximal 1.000 IDs für Objektauflösung zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="6288a-2169">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="6288a-2170">Befehle zur Verwaltung von Anmeldeinformationen (`ad sp credential [reset|list|delete]`) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2170">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="6288a-2171">[BREAKING CHANGE] „properties“ aus `az role assignment [list|show]`-Ausgabe entfernt</span><span class="sxs-lookup"><span data-stu-id="6288a-2171">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="6288a-2172">Unterstützung für `dataActions`- und `notDataActions`-Berechtigungen zu `role definition` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2172">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="6288a-2173">Storage</span><span class="sxs-lookup"><span data-stu-id="6288a-2173">Storage</span></span>

* <span data-ttu-id="6288a-2174">Problem beim Hochladen von Dateien mit einer Größe von 195 GB bis 200 GB behoben</span><span class="sxs-lookup"><span data-stu-id="6288a-2174">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="6288a-2175">[#4049](https://github.com/Azure/azure-cli/issues/4049) behoben: Probleme bei Uploads von Anfügeblobs behoben, die ein Ignorieren der Bedingungsparameter verursacht haben</span><span class="sxs-lookup"><span data-stu-id="6288a-2175">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="6288a-2176">VM</span><span class="sxs-lookup"><span data-stu-id="6288a-2176">VM</span></span>

* <span data-ttu-id="6288a-2177">Warnung für anstehende BREAKING CHANGEen für Sätze mit mehr als 100 Instanzen zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2177">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="6288a-2178">Unterstützung der Zonenresilienz zu `vm [snapshot|image]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2178">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="6288a-2179">Datenträgerinstanzansicht geändert, um besseren Verschlüsselungsstatus zu melden</span><span class="sxs-lookup"><span data-stu-id="6288a-2179">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="6288a-2180">[BREAKING CHANGE]`vm extension delete` geändert, um keine Ausgabe mehr zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="6288a-2180">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="6288a-2181">13. März 2018</span><span class="sxs-lookup"><span data-stu-id="6288a-2181">March 13, 2018</span></span>

<span data-ttu-id="6288a-2182">Version 2.0.29</span><span class="sxs-lookup"><span data-stu-id="6288a-2182">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="6288a-2183">ACR</span><span class="sxs-lookup"><span data-stu-id="6288a-2183">ACR</span></span>

* <span data-ttu-id="6288a-2184">Unterstützung für den Parameter `--image` zu `repository delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2184">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="6288a-2185">Parameter `--manifest` und `--tag` des Befehls `repository delete` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="6288a-2185">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="6288a-2186">Befehl `repository untag` zum Entfernen eines Tags ohne das Löschen von Daten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2186">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="6288a-2187">ACS</span><span class="sxs-lookup"><span data-stu-id="6288a-2187">ACS</span></span>

* <span data-ttu-id="6288a-2188">Befehl `aks upgrade-connector` zum Aktualisieren eines vorhandenen Connectors hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2188">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="6288a-2189">`kubectl`-Konfigurationsdateien zur Verwendung von besser lesbarem YAML im Blockstil geändert</span><span class="sxs-lookup"><span data-stu-id="6288a-2189">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="6288a-2190">Advisor</span><span class="sxs-lookup"><span data-stu-id="6288a-2190">Advisor</span></span>

* <span data-ttu-id="6288a-2191">[BREAKING CHANGE]`advisor configuration get` in `advisor configuration list` umbenannt</span><span class="sxs-lookup"><span data-stu-id="6288a-2191">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="6288a-2192">[BREAKING CHANGE]`advisor configuration set` in `advisor configuration update` umbenannt</span><span class="sxs-lookup"><span data-stu-id="6288a-2192">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="6288a-2193">[BREAKING CHANGE]`advisor recommendation generate` entfernt</span><span class="sxs-lookup"><span data-stu-id="6288a-2193">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="6288a-2194">Parameter `--refresh` zu `advisor recommendation list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2194">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="6288a-2195">Befehl `advisor recommendation show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2195">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="6288a-2196">AppService</span><span class="sxs-lookup"><span data-stu-id="6288a-2196">Appservice</span></span>

* <span data-ttu-id="6288a-2197">`[webapp|functionapp] assign-identity` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="6288a-2197">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="6288a-2198">Befehle `webapp identity [assign|show]` und `functionapp identity [assign|show]` für verwaltete Identität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2198">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="6288a-2199">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="6288a-2199">Eventhubs</span></span>

* <span data-ttu-id="6288a-2200">Erste Veröffentlichung</span><span class="sxs-lookup"><span data-stu-id="6288a-2200">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="6288a-2201">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="6288a-2201">Extension</span></span>

* <span data-ttu-id="6288a-2202">Überprüfung zum Warnen von Benutzern hinzugefügt, wenn sich die verwendete Distribution von der in der Paketquelldatei gespeicherten Distribution unterscheidet, da dies Fehlern führen kann</span><span class="sxs-lookup"><span data-stu-id="6288a-2202">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="6288a-2203">Interactive</span><span class="sxs-lookup"><span data-stu-id="6288a-2203">Interactive</span></span>

* <span data-ttu-id="6288a-2204">[#5625](https://github.com/Azure/azure-cli/issues/5625) behoben: Verlauf über verschiedene Sitzungen hinweg beibehalten</span><span class="sxs-lookup"><span data-stu-id="6288a-2204">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="6288a-2205">[#3016](https://github.com/Azure/azure-cli/issues/3016) behoben: Verlauf nicht aufgezeichnet, obwohl er innerhalb des Bereichs liegt</span><span class="sxs-lookup"><span data-stu-id="6288a-2205">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="6288a-2206">[#5688](https://github.com/Azure/azure-cli/issues/5688) behoben: Abschlüsse wurden nicht angezeigt, wenn beim Laden der Befehlstabelle eine Ausnahme aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="6288a-2206">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="6288a-2207">Statusanzeige für lang ausgeführte Vorgänge korrigiert</span><span class="sxs-lookup"><span data-stu-id="6288a-2207">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="6288a-2208">Überwachen</span><span class="sxs-lookup"><span data-stu-id="6288a-2208">Monitor</span></span>

* <span data-ttu-id="6288a-2209">`monitor autoscale-settings`-Befehle als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="6288a-2209">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="6288a-2210">Befehle vom Typ `monitor autoscale` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2210">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="6288a-2211">Befehle vom Typ `monitor autoscale profile` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2211">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="6288a-2212">Befehle vom Typ `monitor autoscale rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2212">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="6288a-2213">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6288a-2213">Network</span></span>

* <span data-ttu-id="6288a-2214">[BREAKING CHANGE] Parameter `--tags` aus `route-filter rule create` entfernt</span><span class="sxs-lookup"><span data-stu-id="6288a-2214">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="6288a-2215">Einige fehlerhafte Standardwerte für die folgenden Befehle entfernt:</span><span class="sxs-lookup"><span data-stu-id="6288a-2215">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="6288a-2216">`network watcher connection-monitor`-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2216">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="6288a-2217">Parameter `--vnet` und `--subnet` zu `network watcher show-topology` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2217">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="6288a-2218">Profil</span><span class="sxs-lookup"><span data-stu-id="6288a-2218">Profile</span></span>

* <span data-ttu-id="6288a-2219">Parameter `--msi` für `az login` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="6288a-2219">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="6288a-2220">Parameter `--identity` für `az login` als Ersatz vor `--msi` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2220">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="6288a-2221">RDBMS</span><span class="sxs-lookup"><span data-stu-id="6288a-2221">RDBMS</span></span>

* <span data-ttu-id="6288a-2222">[VORSCHAU] Geändert, sodass die API „2017-12-01-preview“ verwendet wird</span><span class="sxs-lookup"><span data-stu-id="6288a-2222">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="6288a-2223">Service Bus</span><span class="sxs-lookup"><span data-stu-id="6288a-2223">Service Bus</span></span>

* <span data-ttu-id="6288a-2224">Erste Veröffentlichung</span><span class="sxs-lookup"><span data-stu-id="6288a-2224">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="6288a-2225">Storage</span><span class="sxs-lookup"><span data-stu-id="6288a-2225">Storage</span></span>

* <span data-ttu-id="6288a-2226">[#4971](https://github.com/Azure/azure-cli/issues/4971) behoben: `storage blob copy` unterstützt jetzt andere Azure-Clouds.</span><span class="sxs-lookup"><span data-stu-id="6288a-2226">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="6288a-2227">[#5286](https://github.com/Azure/azure-cli/issues/5286) behoben: Batchbefehle `storage blob [delete-batch|download-batch|upload-batch]` lösen bei Vorbedingungsfehlern keinen Fehler mehr aus</span><span class="sxs-lookup"><span data-stu-id="6288a-2227">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="6288a-2228">VM</span><span class="sxs-lookup"><span data-stu-id="6288a-2228">VM</span></span>

* <span data-ttu-id="6288a-2229">`[vm|vmss] create` unterstützt jetzt das Anfügen nicht verwalteter Datenträger und das Konfigurieren der Zwischenspeicherung.</span><span class="sxs-lookup"><span data-stu-id="6288a-2229">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="6288a-2230">`[vm|vmss] assign-identity` und `[vm|vmss] remove-identity` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="6288a-2230">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="6288a-2231">Befehle `vm identity [assign|remove|show]` und `vmss identity [assign|remove|show]` als Ersatz für veraltete Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2231">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="6288a-2232">Standardpriorität in `vmss create` auf „Keine“ geändert</span><span class="sxs-lookup"><span data-stu-id="6288a-2232">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="6288a-2233">27. Februar 2018</span><span class="sxs-lookup"><span data-stu-id="6288a-2233">February 27, 2018</span></span>

<span data-ttu-id="6288a-2234">Version 2.0.28</span><span class="sxs-lookup"><span data-stu-id="6288a-2234">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="6288a-2235">Core</span><span class="sxs-lookup"><span data-stu-id="6288a-2235">Core</span></span>

* <span data-ttu-id="6288a-2236">[#5184](https://github.com/Azure/azure-cli/issues/5184) behoben: Problem beim Installieren von Homebrew</span><span class="sxs-lookup"><span data-stu-id="6288a-2236">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="6288a-2237">Unterstützung für Erweiterungstelemetrie mit benutzerdefinierten Schlüsseln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2237">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="6288a-2238">HTTP-Protokollierung zu `--debug` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2238">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="6288a-2239">ACS</span><span class="sxs-lookup"><span data-stu-id="6288a-2239">ACS</span></span>

* <span data-ttu-id="6288a-2240">Geändert, sodass für `aks install-connector` standardmäßig das Helm-Diagramm `virtual-kubelet-for-aks` verwendet wird</span><span class="sxs-lookup"><span data-stu-id="6288a-2240">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="6288a-2241">Problem behoben: Unzureichende Berechtigungen für Dienstprinzipale zum Erstellen einer ACI-Containergruppe</span><span class="sxs-lookup"><span data-stu-id="6288a-2241">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="6288a-2242">Parameter `--aci-container-group`, `--location` und `--image-tag` zu `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2242">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="6288a-2243">Veraltungshinweis aus `aks get-versions` entfernt</span><span class="sxs-lookup"><span data-stu-id="6288a-2243">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="6288a-2244">AppService</span><span class="sxs-lookup"><span data-stu-id="6288a-2244">Appservice</span></span>

* <span data-ttu-id="6288a-2245">Updates für die neue SDK-Version (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="6288a-2245">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="6288a-2246">[5538](https://github.com/Azure/azure-cli/issues/5538) behoben: `Free` wurde als ungültige SKU gemeldet.</span><span class="sxs-lookup"><span data-stu-id="6288a-2246">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="6288a-2247">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="6288a-2247">Cognitive Services</span></span>

* <span data-ttu-id="6288a-2248">Hinweis beim Erstellen eines neuen Cognitive Services-Kontos aktualisiert</span><span class="sxs-lookup"><span data-stu-id="6288a-2248">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="6288a-2249">Nutzung</span><span class="sxs-lookup"><span data-stu-id="6288a-2249">Consumption</span></span>

* <span data-ttu-id="6288a-2250">Neue Befehle für PriceSheet-API hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2250">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="6288a-2251">Vorhandene Formate für Nutzungsdetails und Reservierungsdetails aktualisiert</span><span class="sxs-lookup"><span data-stu-id="6288a-2251">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="6288a-2252">Container</span><span class="sxs-lookup"><span data-stu-id="6288a-2252">Container</span></span>

* <span data-ttu-id="6288a-2253">Argumente `--secrets` und `--secrets-mount-path` zu `container create` hinzugefügt, um Geheimnisse in ACI verwenden zu können</span><span class="sxs-lookup"><span data-stu-id="6288a-2253">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="6288a-2254">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6288a-2254">Network</span></span>

* <span data-ttu-id="6288a-2255">[#5559](https://github.com/Azure/azure-cli/issues/5559) behoben: Fehlender Client in `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="6288a-2255">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="6288a-2256">Resource</span><span class="sxs-lookup"><span data-stu-id="6288a-2256">Resource</span></span>

* <span data-ttu-id="6288a-2257">`group deployment export` geändert, um eine partielle Vorlage und ggf. Fehler anzuzeigen, wenn der Vorgang nicht erfolgreich war</span><span class="sxs-lookup"><span data-stu-id="6288a-2257">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="6288a-2258">Role</span><span class="sxs-lookup"><span data-stu-id="6288a-2258">Role</span></span>

* <span data-ttu-id="6288a-2259">`role assignment list-changelogs` hinzugefügt, um die Überprüfung von Dienstprinzipalrollen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="6288a-2259">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="6288a-2260">SQL</span><span class="sxs-lookup"><span data-stu-id="6288a-2260">SQL</span></span>

* <span data-ttu-id="6288a-2261">Zonenredundanzunterstützung für Datenbanken und Pools für elastische Datenbanken hinzugefügt (bei Erstellung und Aktualisierung)</span><span class="sxs-lookup"><span data-stu-id="6288a-2261">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="6288a-2262">Storage</span><span class="sxs-lookup"><span data-stu-id="6288a-2262">Storage</span></span>

* <span data-ttu-id="6288a-2263">Angabe von Zielpfad/Präfix für `storage blob [upload-batch|download-batch]` ermöglicht</span><span class="sxs-lookup"><span data-stu-id="6288a-2263">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="6288a-2264">VM</span><span class="sxs-lookup"><span data-stu-id="6288a-2264">VM</span></span>

* <span data-ttu-id="6288a-2265">Unterstützung für das Anfügen/Trennen von Datenträgern für eine einzelne VMSS-Instanz hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2265">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="6288a-2266">13. Februar 2018</span><span class="sxs-lookup"><span data-stu-id="6288a-2266">February 13, 2018</span></span>

<span data-ttu-id="6288a-2267">Version 2.0.27</span><span class="sxs-lookup"><span data-stu-id="6288a-2267">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="6288a-2268">Core</span><span class="sxs-lookup"><span data-stu-id="6288a-2268">Core</span></span>

* <span data-ttu-id="6288a-2269">Authentifizierung für Abonnement-ID und Namen bei der MSI-Anmeldung in Authentifizierung mit Schlüssel geändert</span><span class="sxs-lookup"><span data-stu-id="6288a-2269">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="6288a-2270">ACS</span><span class="sxs-lookup"><span data-stu-id="6288a-2270">ACS</span></span>

* <span data-ttu-id="6288a-2271">[BREAKING CHANGE]`aks get-versions` aus Gründen der Genauigkeit in `aks get-upgrades` umbenannt</span><span class="sxs-lookup"><span data-stu-id="6288a-2271">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="6288a-2272">`aks get-versions` zur Anzeige der verfügbaren Kubernetes-Versionen für `aks create` geändert</span><span class="sxs-lookup"><span data-stu-id="6288a-2272">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="6288a-2273">Standardwerte von `aks create` in Auswahl der Kubernetes-Version durch den Server geändert</span><span class="sxs-lookup"><span data-stu-id="6288a-2273">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="6288a-2274">Hilfemeldungen zu dem von AKS generierten Dienstprinzipal aktualisiert</span><span class="sxs-lookup"><span data-stu-id="6288a-2274">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="6288a-2275">Standardknotengrößen für `aks create` von „Standard\_D1\_v2“ in „Standard\_DS1\_v2“ geändert</span><span class="sxs-lookup"><span data-stu-id="6288a-2275">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="6288a-2276">Zuverlässigkeit der Suche nach dem Dashboardpod für `az aks browse` verbessert</span><span class="sxs-lookup"><span data-stu-id="6288a-2276">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="6288a-2277">`aks get-credentials` korrigiert, um Unicode-Fehler beim Laden von Kubernetes-Konfigurationsdateien zu behandeln</span><span class="sxs-lookup"><span data-stu-id="6288a-2277">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="6288a-2278">Meldung zu `az aks install-cli` hinzugefügt, um das Abrufen von `kubectl` in `$PATH` zu erleichtern</span><span class="sxs-lookup"><span data-stu-id="6288a-2278">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="6288a-2279">AppService</span><span class="sxs-lookup"><span data-stu-id="6288a-2279">Appservice</span></span>

* <span data-ttu-id="6288a-2280">Problem behoben, das zu einem Fehler von `webapp [backup|restore]` aufgrund eines Nullverweises führte</span><span class="sxs-lookup"><span data-stu-id="6288a-2280">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="6288a-2281">Unterstützung für Standard-App Service-Pläne durch `az configure --defaults appserviceplan=my-asp` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2281">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="6288a-2282">CDN</span><span class="sxs-lookup"><span data-stu-id="6288a-2282">CDN</span></span>

* <span data-ttu-id="6288a-2283">Befehle vom Typ `cdn custom-domain [enable-https|disable-https]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2283">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="6288a-2284">Container</span><span class="sxs-lookup"><span data-stu-id="6288a-2284">Container</span></span>

* <span data-ttu-id="6288a-2285">Option `--follow` zu `az container logs` für Streamingprotokolle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2285">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="6288a-2286">Befehl `container attach` hinzugefügt, der die lokale Standardausgabe und Fehlerdatenströme an einen Container in einer Containergruppe angefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2286">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="6288a-2287">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="6288a-2287">CosmosDB</span></span>

* <span data-ttu-id="6288a-2288">Unterstützung für Einstellungsfunktionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2288">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="6288a-2289">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="6288a-2289">Extension</span></span>

* <span data-ttu-id="6288a-2290">Unterstützung für den Parameter `--pip-proxy` zu Befehlen vom Typ `az extension [add|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2290">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="6288a-2291">Unterstützung für das Argument `--pip-extra-index-urls` zu Befehlen vom Typ `az extension [add|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2291">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="6288a-2292">Feedback</span><span class="sxs-lookup"><span data-stu-id="6288a-2292">Feedback</span></span>

* <span data-ttu-id="6288a-2293">Erweiterungsinformationen zu Telemetriedaten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2293">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="6288a-2294">Interactive</span><span class="sxs-lookup"><span data-stu-id="6288a-2294">Interactive</span></span>

* <span data-ttu-id="6288a-2295">Problem behoben, aufgrund dessen der Benutzer bei Verwendung des interaktiven Modus in Cloud Shell zur Anmeldung aufgefordert wird</span><span class="sxs-lookup"><span data-stu-id="6288a-2295">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="6288a-2296">Regression mit fehlenden Parametervervollständigungen korrigiert</span><span class="sxs-lookup"><span data-stu-id="6288a-2296">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="6288a-2297">IoT</span><span class="sxs-lookup"><span data-stu-id="6288a-2297">IoT</span></span>

* <span data-ttu-id="6288a-2298">Problem behoben, aufgrund dessen `iot dps access policy [create|update]` bei erfolgreicher Ausführung einen Fehler „nicht gefunden“ zurückgibt</span><span class="sxs-lookup"><span data-stu-id="6288a-2298">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="6288a-2299">Problem behoben, aufgrund dessen `iot dps linked-hub [create|update]` bei erfolgreicher Ausführung einen Fehler „nicht gefunden“ zurückgibt</span><span class="sxs-lookup"><span data-stu-id="6288a-2299">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="6288a-2300">Unterstützung für `--no-wait` zu `iot dps access policy [create|update]` und `iot dps linked-hub [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2300">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="6288a-2301">`iot hub create` geändert, um die Angabe der Anzahl von Partitionen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="6288a-2301">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="6288a-2302">Überwachen</span><span class="sxs-lookup"><span data-stu-id="6288a-2302">Monitor</span></span>

* <span data-ttu-id="6288a-2303">Befehl `az monitor log-profiles create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="6288a-2303">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="6288a-2304">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6288a-2304">Network</span></span>

* <span data-ttu-id="6288a-2305">Option `--tags` für folgende Befehle korrigiert:</span><span class="sxs-lookup"><span data-stu-id="6288a-2305">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="6288a-2306">Profil</span><span class="sxs-lookup"><span data-stu-id="6288a-2306">Profile</span></span>

* <span data-ttu-id="6288a-2307">`az login` im interaktiven Modus aktiviert</span><span class="sxs-lookup"><span data-stu-id="6288a-2307">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="6288a-2308">Resource</span><span class="sxs-lookup"><span data-stu-id="6288a-2308">Resource</span></span>

* <span data-ttu-id="6288a-2309">`feature show` wieder hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2309">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="6288a-2310">Role</span><span class="sxs-lookup"><span data-stu-id="6288a-2310">Role</span></span>

* <span data-ttu-id="6288a-2311">Argument `--available-to-other-tenants` zu `ad app update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2311">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="6288a-2312">SQL</span><span class="sxs-lookup"><span data-stu-id="6288a-2312">SQL</span></span>

* <span data-ttu-id="6288a-2313">Befehle vom Typ `sql server dns-alias` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2313">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="6288a-2314">`sql db rename` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2314">Added `sql db rename`</span></span>
* <span data-ttu-id="6288a-2315">Unterstützung für das Argument `--ids` für alle SQL-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2315">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="6288a-2316">Storage</span><span class="sxs-lookup"><span data-stu-id="6288a-2316">Storage</span></span>

* <span data-ttu-id="6288a-2317">Befehle `storage blob service-properties delete-policy` und `storage blob undelete` hinzugefügt, um vorläufiges Löschen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="6288a-2317">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="6288a-2318">VM</span><span class="sxs-lookup"><span data-stu-id="6288a-2318">VM</span></span>

* <span data-ttu-id="6288a-2319">Absturz bei unvollständiger Initialisierung der VM-Verschlüsselung behoben</span><span class="sxs-lookup"><span data-stu-id="6288a-2319">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="6288a-2320">Prinzipal-ID-Ausgabe beim Aktivieren von MSI hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2320">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="6288a-2321">`vm boot-diagnostics get-boot-log` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="6288a-2321">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="6288a-2322">31. Januar 2018</span><span class="sxs-lookup"><span data-stu-id="6288a-2322">January 31, 2018</span></span>

<span data-ttu-id="6288a-2323">Version 2.0.26</span><span class="sxs-lookup"><span data-stu-id="6288a-2323">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="6288a-2324">Core</span><span class="sxs-lookup"><span data-stu-id="6288a-2324">Core</span></span>

* <span data-ttu-id="6288a-2325">Unterstützung für das Abrufen von unformatierten Token im MSI-Kontext hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2325">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="6288a-2326">Abrufindikator-Zeichenfolge nach Fertigstellung von LRO für die Windows-Datei „cmd.exe“ entfernt</span><span class="sxs-lookup"><span data-stu-id="6288a-2326">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="6288a-2327">Warnung hinzugefügt, die angezeigt wird, wenn ein konfigurierter Standardwert in einen Eintrag auf INFO-Ebene geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="6288a-2327">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="6288a-2328">`--verbose` zum Anzeigen verwenden.</span><span class="sxs-lookup"><span data-stu-id="6288a-2328">Use `--verbose` to see</span></span>
* <span data-ttu-id="6288a-2329">Statusanzeige für Wait-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2329">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="6288a-2330">ACS</span><span class="sxs-lookup"><span data-stu-id="6288a-2330">ACS</span></span>

* <span data-ttu-id="6288a-2331">Argument `--disable-browser` erläutert</span><span class="sxs-lookup"><span data-stu-id="6288a-2331">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="6288a-2332">Vervollständigung mit der TAB-TASTE für Argumente vom Typ `--vm-size` verbessert</span><span class="sxs-lookup"><span data-stu-id="6288a-2332">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="6288a-2333">AppService</span><span class="sxs-lookup"><span data-stu-id="6288a-2333">Appservice</span></span>

* <span data-ttu-id="6288a-2334">`webapp log [tail|download]` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="6288a-2334">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="6288a-2335">Überprüfung `kind` für Web-Apps und Funktionen entfernt</span><span class="sxs-lookup"><span data-stu-id="6288a-2335">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="6288a-2336">CDN</span><span class="sxs-lookup"><span data-stu-id="6288a-2336">CDN</span></span>

* <span data-ttu-id="6288a-2337">Problem mit fehlendem Client für `cdn custom-domain create` behoben</span><span class="sxs-lookup"><span data-stu-id="6288a-2337">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="6288a-2338">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="6288a-2338">CosmosDB</span></span>

* <span data-ttu-id="6288a-2339">Parameterbeschreibung für Failoverrichtlinien korrigiert</span><span class="sxs-lookup"><span data-stu-id="6288a-2339">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="6288a-2340">Interactive</span><span class="sxs-lookup"><span data-stu-id="6288a-2340">Interactive</span></span>

* <span data-ttu-id="6288a-2341">Problem behoben, aufgrund dessen Vervollständigungen von Befehlsoptionen nicht mehr angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="6288a-2341">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="6288a-2342">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6288a-2342">Network</span></span>

* <span data-ttu-id="6288a-2343">Schutz für `--cert-password` zu `application-gateway create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2343">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="6288a-2344">Problem mit `application-gateway update` behoben, aufgrund dessen `--sku` fälschlicherweise einen Standardwert anwendete</span><span class="sxs-lookup"><span data-stu-id="6288a-2344">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="6288a-2345">Schutz für `--shared-key` und `--authorization-key` zu `vpn-connection create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2345">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="6288a-2346">Problem mit fehlendem Client für `asg create` behoben</span><span class="sxs-lookup"><span data-stu-id="6288a-2346">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="6288a-2347">Parameter `--file-name / -f` für exportierte Namen zu `dns zone export` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2347">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="6288a-2348">Folgende Probleme mit `dns zone export` behoben:</span><span class="sxs-lookup"><span data-stu-id="6288a-2348">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="6288a-2349">Problem behoben, aufgrund dessen lange TXT-Einträge nicht korrekt exportiert wurden</span><span class="sxs-lookup"><span data-stu-id="6288a-2349">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="6288a-2350">Problem behoben, aufgrund dessen TXT-Einträge in Anführungszeichen fälschlich ohne Anführungszeichen in Escapezeichen exportiert wurden</span><span class="sxs-lookup"><span data-stu-id="6288a-2350">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="6288a-2351">Problem behoben, aufgrund dessen bestimmte Datensätze zweimal mit `dns zone import` importiert wurden</span><span class="sxs-lookup"><span data-stu-id="6288a-2351">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="6288a-2352">Befehle `vnet-gateway root-cert` und `vnet-gateway revoked-cert` wiederhergestellt</span><span class="sxs-lookup"><span data-stu-id="6288a-2352">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="6288a-2353">Profil</span><span class="sxs-lookup"><span data-stu-id="6288a-2353">Profile</span></span>

* <span data-ttu-id="6288a-2354">`get-access-token` zur Verwendung auf einer VM mit Identität korrigiert</span><span class="sxs-lookup"><span data-stu-id="6288a-2354">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="6288a-2355">Resource</span><span class="sxs-lookup"><span data-stu-id="6288a-2355">Resource</span></span>

* <span data-ttu-id="6288a-2356">Fehler mit `deployment [create|validate]` korrigiert, aufgrund dessen fälschlich eine Warnung angezeigt wurde, wenn ein Vorlagenfeld „Typ“ Werte in Großbuchstaben enthielt</span><span class="sxs-lookup"><span data-stu-id="6288a-2356">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="6288a-2357">Storage</span><span class="sxs-lookup"><span data-stu-id="6288a-2357">Storage</span></span>

* <span data-ttu-id="6288a-2358">Problem mit der Migration von Storage V1-Konten zu Storage V2 behoben</span><span class="sxs-lookup"><span data-stu-id="6288a-2358">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="6288a-2359">Statusberichterstellung für alle Upload-/Downloadbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2359">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="6288a-2360">Fehler korrigiert, der die Verwendung der arg-Option „-n“ mit `storage account check-name` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="6288a-2360">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="6288a-2361">Spalte „Momentaufnahme“ zur Tabellenausgabe für `blob [list|show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2361">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="6288a-2362">Fehler mit verschiedenen Parametern korrigiert, die als Int-Typen analysiert werden mussten</span><span class="sxs-lookup"><span data-stu-id="6288a-2362">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="6288a-2363">VM</span><span class="sxs-lookup"><span data-stu-id="6288a-2363">VM</span></span>

* <span data-ttu-id="6288a-2364">Befehl `vm image accept-terms` hinzugefügt, um die Erstellung von VMs aus Images mit zusätzlichen Gebühren zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="6288a-2364">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="6288a-2365">`[vm|vmss create]` korrigiert, um sicherzustellen, dass Befehle unter einem Proxy mit nicht signierten Zertifikaten ausgeführt werden können</span><span class="sxs-lookup"><span data-stu-id="6288a-2365">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="6288a-2366">[VORSCHAU] Unterstützung für „niedrige“ Priorität zu VMSS hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2366">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="6288a-2367">Schutz für `--admin-password` zu `[vm|vmss] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2367">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="6288a-2368">17. Januar 2018</span><span class="sxs-lookup"><span data-stu-id="6288a-2368">January 17, 2018</span></span>

<span data-ttu-id="6288a-2369">Version 2.0.25</span><span class="sxs-lookup"><span data-stu-id="6288a-2369">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="6288a-2370">ACR</span><span class="sxs-lookup"><span data-stu-id="6288a-2370">ACR</span></span>

* <span data-ttu-id="6288a-2371">Fallback auf ACR-Anmeldung bei Fehlern mit Windows-Anmeldeinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2371">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="6288a-2372">Registrierungsprotokolle aktiviert</span><span class="sxs-lookup"><span data-stu-id="6288a-2372">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="6288a-2373">ACS</span><span class="sxs-lookup"><span data-stu-id="6288a-2373">ACS</span></span>

* <span data-ttu-id="6288a-2374">Befehl `get-credentials` korrigiert</span><span class="sxs-lookup"><span data-stu-id="6288a-2374">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="6288a-2375">SPN-Rollenanforderung entfernt</span><span class="sxs-lookup"><span data-stu-id="6288a-2375">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="6288a-2376">AppService</span><span class="sxs-lookup"><span data-stu-id="6288a-2376">Appservice</span></span>

* <span data-ttu-id="6288a-2377">Fehler mit `config ssl upload` behoben, bei dem `hosting_environment_profile` NULL war</span><span class="sxs-lookup"><span data-stu-id="6288a-2377">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="6288a-2378">Unterstützung benutzerdefinierter URLs zu `browse` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2378">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="6288a-2379">Slotunterstützung für `log tail` korrigiert</span><span class="sxs-lookup"><span data-stu-id="6288a-2379">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="6288a-2380">Backup</span><span class="sxs-lookup"><span data-stu-id="6288a-2380">Backup</span></span>

* <span data-ttu-id="6288a-2381">Option `--container-name` von `backup item list` geändert (ist jetzt optional)</span><span class="sxs-lookup"><span data-stu-id="6288a-2381">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="6288a-2382">Speicherkontooptionen zu `backup restore restore-disks` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2382">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="6288a-2383">Standortüberprüfung in `backup protection enable-for-vm` korrigiert (Groß-/Kleinschreibung wird jetzt nicht mehr beachtet)</span><span class="sxs-lookup"><span data-stu-id="6288a-2383">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="6288a-2384">Problem behoben, durch das bei Befehlen mit ungültigem Containernamen ein Fehler auftrat</span><span class="sxs-lookup"><span data-stu-id="6288a-2384">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="6288a-2385">`backup item list` geändert (Integritätsstatus jetzt standardmäßig enthalten)</span><span class="sxs-lookup"><span data-stu-id="6288a-2385">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="6288a-2386">Batch</span><span class="sxs-lookup"><span data-stu-id="6288a-2386">Batch</span></span>

* <span data-ttu-id="6288a-2387">`batch login` geändert, um Authentifizierungsdetails zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="6288a-2387">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="6288a-2388">Cloud</span><span class="sxs-lookup"><span data-stu-id="6288a-2388">Cloud</span></span>

* <span data-ttu-id="6288a-2389">Beim Festlegen von `--profile` für eine Cloud werden nun keine Endpunkte mehr benötigt.</span><span class="sxs-lookup"><span data-stu-id="6288a-2389">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="6288a-2390">Nutzung</span><span class="sxs-lookup"><span data-stu-id="6288a-2390">Consumption</span></span>

* <span data-ttu-id="6288a-2391">Neue Befehle für Reservierungen hinzugefügt: `consumption reservations summaries` und `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="6288a-2391">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="6288a-2392">Event Grid</span><span class="sxs-lookup"><span data-stu-id="6288a-2392">Event Grid</span></span>

* <span data-ttu-id="6288a-2393">[BREAKING CHANGE] Die Befehle vom Typ `az eventgrid topic event-subscription` wurden in `eventgrid event-subscription` verschoben.</span><span class="sxs-lookup"><span data-stu-id="6288a-2393">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="6288a-2394">[BREAKING CHANGE] Die Befehle vom Typ `az eventgrid resource event-subscription` wurden in `eventgrid event-subscription` verschoben.</span><span class="sxs-lookup"><span data-stu-id="6288a-2394">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="6288a-2395">[BREAKING CHANGE] Der Befehl `eventgrid event-subscription show-endpoint-url` wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="6288a-2395">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="6288a-2396">Verwenden Sie stattdessen `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="6288a-2396">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="6288a-2397">Befehl `eventgrid topic update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2397">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="6288a-2398">Befehl `eventgrid event-subscription update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2398">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="6288a-2399">Parameter `--ids` für Befehle vom Typ `eventgrid topic` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2399">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="6288a-2400">Unterstützung der Vervollständigung mit der TAB-TASTE für Themennamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2400">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="6288a-2401">Interactive</span><span class="sxs-lookup"><span data-stu-id="6288a-2401">Interactive</span></span>

* <span data-ttu-id="6288a-2402">Problem behoben, das dazu führte, dass der interaktive Modus nicht mit Python 2.x verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="6288a-2402">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="6288a-2403">Fehler beim Start behoben</span><span class="sxs-lookup"><span data-stu-id="6288a-2403">Fixed errors on startup</span></span>
* <span data-ttu-id="6288a-2404">Problem behoben, das dazu führte, dass einige Befehle nicht im interaktiven Modus ausgeführt werden konnten</span><span class="sxs-lookup"><span data-stu-id="6288a-2404">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="6288a-2405">IoT</span><span class="sxs-lookup"><span data-stu-id="6288a-2405">IoT</span></span>

* <span data-ttu-id="6288a-2406">Unterstützung für Gerätebereitstellungsdienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2406">Added support for device provisioning service</span></span>
* <span data-ttu-id="6288a-2407">Benachrichtigungen zu veralteten Elementen in Befehlen und in der Befehlshilfe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2407">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="6288a-2408">IoT-Überprüfung hinzugefügt, um Benutzer über die IoT-Erweiterung zu informieren</span><span class="sxs-lookup"><span data-stu-id="6288a-2408">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="6288a-2409">Überwachen</span><span class="sxs-lookup"><span data-stu-id="6288a-2409">Monitor</span></span>

* <span data-ttu-id="6288a-2410">Unterstützung mehrerer Diagnoseeinstellung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-2410">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="6288a-2411">Der Parameter `--name` ist nun für `az monitor diagnostic-settings create` erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6288a-2411">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="6288a-2412">Befehl `monitor diagnostic-settings categories` zum Abrufen der Diagnoseeinstellungskategorie hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2412">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="6288a-2413">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6288a-2413">Network</span></span>

* <span data-ttu-id="6288a-2414">Problem behoben, das beim Ändern des aktiven Standbymodus mit `vnet-gateway update` auftrat</span><span class="sxs-lookup"><span data-stu-id="6288a-2414">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="6288a-2415">Unterstützung für HTTP2 zu `application-gateway [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2415">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="6288a-2416">Profil</span><span class="sxs-lookup"><span data-stu-id="6288a-2416">Profile</span></span>

* <span data-ttu-id="6288a-2417">Unterstützung für die Anmeldung mit durch Benutzer zugewiesenen Identitäten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2417">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="6288a-2418">Role</span><span class="sxs-lookup"><span data-stu-id="6288a-2418">Role</span></span>

* <span data-ttu-id="6288a-2419">Argument `--assignee-object-id` zu `role assignment create` hinzugefügt, um Graph-Abfrage zu umgehen</span><span class="sxs-lookup"><span data-stu-id="6288a-2419">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="6288a-2420">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="6288a-2420">Service Fabric</span></span>

* <span data-ttu-id="6288a-2421">Ausführliche Fehler zur Überprüfungsantwort bei der Clustererstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2421">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="6288a-2422">Problem mit fehlendem Client für verschiedene Befehle behoben</span><span class="sxs-lookup"><span data-stu-id="6288a-2422">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="6288a-2423">VM</span><span class="sxs-lookup"><span data-stu-id="6288a-2423">VM</span></span>

* <span data-ttu-id="6288a-2424">[VORSCHAUVERSION] Zonenübergreifende Unterstützung für `vmss`</span><span class="sxs-lookup"><span data-stu-id="6288a-2424">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="6288a-2425">[BREAKING CHANGE] Standard für Einzelzone (`vmss`) in Standardlastenausgleich geändert</span><span class="sxs-lookup"><span data-stu-id="6288a-2425">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="6288a-2426">[BREAKING CHANGE]`externalIdentities` in `userAssignedIdentities` geändert für EMSI</span><span class="sxs-lookup"><span data-stu-id="6288a-2426">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="6288a-2427">[VORSCHAUVERSION] Unterstützung für Austausch des Betriebssystemdatenträgers hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2427">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="6288a-2428">Unterstützung der Verwendung von VM-Images aus anderen Abonnements hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2428">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="6288a-2429">Argumente `--plan-name`, `--plan-product`, `--plan-promotion-code` und `--plan-publisher` zu `[vm|vmss] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2429">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="6288a-2430">Fehlerbedingte Probleme mit `[vm|vmss] create` behoben</span><span class="sxs-lookup"><span data-stu-id="6288a-2430">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="6288a-2431">Übermäßige Ressourcenverwendung durch `vm image list --all` behoben</span><span class="sxs-lookup"><span data-stu-id="6288a-2431">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="6288a-2432">19. Dezember 2017</span><span class="sxs-lookup"><span data-stu-id="6288a-2432">December 19, 2017</span></span>

<span data-ttu-id="6288a-2433">Version 2.0.23</span><span class="sxs-lookup"><span data-stu-id="6288a-2433">Version 2.0.23</span></span>

* <span data-ttu-id="6288a-2434">Unterstützung für die Anmeldung mit durch Benutzer zugewiesenen Identitäten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2434">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="6288a-2435">Container</span><span class="sxs-lookup"><span data-stu-id="6288a-2435">Container</span></span>

* <span data-ttu-id="6288a-2436">Falsche Reihenfolge der Parameter für Containerprotokolle behoben</span><span class="sxs-lookup"><span data-stu-id="6288a-2436">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="6288a-2437">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6288a-2437">Network</span></span>

* <span data-ttu-id="6288a-2438">Argument `--disable-bgp-route-propagation` zu `route-table [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2438">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="6288a-2439">Argument `--ip-tags` zu `public-ip [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2439">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="6288a-2440">Storage</span><span class="sxs-lookup"><span data-stu-id="6288a-2440">Storage</span></span>

* <span data-ttu-id="6288a-2441">Unterstützung für Storage V2 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2441">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="6288a-2442">VM</span><span class="sxs-lookup"><span data-stu-id="6288a-2442">VM</span></span>

* <span data-ttu-id="6288a-2443">[VORSCHAUVERSION] Unterstützung für durch Benutzer zugewiesene Identitäten für virtuelle Computer und VMSSs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2443">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="6288a-2444">5\. Dezember 2017</span><span class="sxs-lookup"><span data-stu-id="6288a-2444">December 5, 2017</span></span>

<span data-ttu-id="6288a-2445">Version 2.0.22</span><span class="sxs-lookup"><span data-stu-id="6288a-2445">Version 2.0.22</span></span>

* <span data-ttu-id="6288a-2446">`az component`-Befehle wurden entfernt.</span><span class="sxs-lookup"><span data-stu-id="6288a-2446">Removed `az component` commands.</span></span> <span data-ttu-id="6288a-2447">Verwenden Sie stattdessen `az extension`.</span><span class="sxs-lookup"><span data-stu-id="6288a-2447">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="6288a-2448">Core</span><span class="sxs-lookup"><span data-stu-id="6288a-2448">Core</span></span>
* <span data-ttu-id="6288a-2449">Der `AZURE_US_GOV_CLOUD`-Autoritätsendpunkt von AAD wurde von „login.microsoftonline.com“ in „login.microsoftonline.us“ geändert.</span><span class="sxs-lookup"><span data-stu-id="6288a-2449">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="6288a-2450">Problem behoben, aufgrund dessen Telemetriedaten fortlaufend neu gesendet wurden</span><span class="sxs-lookup"><span data-stu-id="6288a-2450">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="6288a-2451">ACS</span><span class="sxs-lookup"><span data-stu-id="6288a-2451">ACS</span></span>

* <span data-ttu-id="6288a-2452">Die Befehle `aks install-connector` und `aks remove-connector` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-2452">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="6288a-2453">Verbesserte Fehlerberichterstellung für `acs create`</span><span class="sxs-lookup"><span data-stu-id="6288a-2453">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="6288a-2454">Feste Verwendung von `aks get-credentials -f` ohne vollqualifizierten Pfad</span><span class="sxs-lookup"><span data-stu-id="6288a-2454">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="6288a-2455">Advisor</span><span class="sxs-lookup"><span data-stu-id="6288a-2455">Advisor</span></span>

* <span data-ttu-id="6288a-2456">Erste Veröffentlichung</span><span class="sxs-lookup"><span data-stu-id="6288a-2456">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="6288a-2457">AppService</span><span class="sxs-lookup"><span data-stu-id="6288a-2457">Appservice</span></span>

* <span data-ttu-id="6288a-2458">Erstellung feststehender Zertifikatnamen mit `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="6288a-2458">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="6288a-2459">`webapp [list|show]` und `functionapp [list|show]` wurden verbessert, um die richtigen Apps anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="6288a-2459">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="6288a-2460">Standardwert für `WEBSITE_NODE_DEFAULT_VERSION` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2460">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="6288a-2461">Nutzung</span><span class="sxs-lookup"><span data-stu-id="6288a-2461">Consumption</span></span>

* <span data-ttu-id="6288a-2462">Unterstützung für API-Version 2017-11-30 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2462">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="6288a-2463">Container</span><span class="sxs-lookup"><span data-stu-id="6288a-2463">Container</span></span>

* <span data-ttu-id="6288a-2464">Feste Regression für Standardports</span><span class="sxs-lookup"><span data-stu-id="6288a-2464">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="6288a-2465">Überwachen</span><span class="sxs-lookup"><span data-stu-id="6288a-2465">Monitor</span></span>

* <span data-ttu-id="6288a-2466">Unterstützung mehrerer Dimensionen zu Metrikbefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2466">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="6288a-2467">Resource</span><span class="sxs-lookup"><span data-stu-id="6288a-2467">Resource</span></span>

* <span data-ttu-id="6288a-2468">Argument `--include-response-body` zu `resource show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2468">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="6288a-2469">Role</span><span class="sxs-lookup"><span data-stu-id="6288a-2469">Role</span></span>

* <span data-ttu-id="6288a-2470">Anzeige von Standardzuweisungen für „klassische“ Administratoren zu `role assignment list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2470">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="6288a-2471">Unterstützung für das Hinzufügen (anstelle der Überschreibung) von Anmeldeinformationen zu `ad sp reset-credentials` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2471">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="6288a-2472">Verbesserte Fehlerberichterstellung für `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="6288a-2472">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="6288a-2473">SQL</span><span class="sxs-lookup"><span data-stu-id="6288a-2473">SQL</span></span>

* <span data-ttu-id="6288a-2474">Die Befehle `sql db list-usages` und `sql db show-usage` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-2474">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="6288a-2475">Die Befehle `sql server conn-policy show` und `sql server conn-policy update` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-2475">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="6288a-2476">VM</span><span class="sxs-lookup"><span data-stu-id="6288a-2476">VM</span></span>

* <span data-ttu-id="6288a-2477">Zoneninformationen zu `az vm list-skus` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2477">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="6288a-2478">14. November 2017</span><span class="sxs-lookup"><span data-stu-id="6288a-2478">November 14, 2017</span></span>

<span data-ttu-id="6288a-2479">Version 2.0.21</span><span class="sxs-lookup"><span data-stu-id="6288a-2479">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="6288a-2480">ACR</span><span class="sxs-lookup"><span data-stu-id="6288a-2480">ACR</span></span>

* <span data-ttu-id="6288a-2481">Unterstützung für das Erstellen von Webhooks in Replikationsregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2481">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="6288a-2482">ACS</span><span class="sxs-lookup"><span data-stu-id="6288a-2482">ACS</span></span>

* <span data-ttu-id="6288a-2483">Formulierung in AKS von „Agent“ in „Knoten“ geändert</span><span class="sxs-lookup"><span data-stu-id="6288a-2483">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="6288a-2484">Option `--orchestrator-release` für `acs create` als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="6288a-2484">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="6288a-2485">VM-Standardgröße für AKS in `Standard_D1_v2` geändert</span><span class="sxs-lookup"><span data-stu-id="6288a-2485">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="6288a-2486">`az aks browse` für Windows korrigiert</span><span class="sxs-lookup"><span data-stu-id="6288a-2486">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="6288a-2487">`az aks get-credentials` für Windows korrigiert</span><span class="sxs-lookup"><span data-stu-id="6288a-2487">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="6288a-2488">AppService</span><span class="sxs-lookup"><span data-stu-id="6288a-2488">Appservice</span></span>

* <span data-ttu-id="6288a-2489">Bereitstellungsquelle `config-zip` für Web-Apps und Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2489">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="6288a-2490">Option `--docker-container-logging` zu `az webapp log config` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2490">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="6288a-2491">Option `storage` aus dem Parameter `--web-server-logging` von `az webapp log config` entfernt</span><span class="sxs-lookup"><span data-stu-id="6288a-2491">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="6288a-2492">Fehlermeldungen für `deployment user set` verbessert</span><span class="sxs-lookup"><span data-stu-id="6288a-2492">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="6288a-2493">Unterstützung für das Erstellen von Linux-Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2493">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="6288a-2494">`list-locations` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="6288a-2494">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="6288a-2495">Batch</span><span class="sxs-lookup"><span data-stu-id="6288a-2495">Batch</span></span>

* <span data-ttu-id="6288a-2496">Fehler im Poolerstellungsbefehl korrigiert, der bei Verwendung einer Ressourcen-ID mit dem Flag `--image` aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="6288a-2496">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="6288a-2497">BatchAI</span><span class="sxs-lookup"><span data-stu-id="6288a-2497">Batchai</span></span>

* <span data-ttu-id="6288a-2498">Kurzoption (`-s`) für `--vm-size` zur Angabe der VM-Größe im Befehl `file-server create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2498">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="6288a-2499">Argumente für Speicherkontoname und -schlüssel zum Parameter `cluster create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2499">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="6288a-2500">Dokumentation für `job list-files` und `job stream-file` korrigiert</span><span class="sxs-lookup"><span data-stu-id="6288a-2500">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="6288a-2501">Kurzoption (`-r`) für `--cluster-name` zur Angabe des Clusternamens im Befehl `job create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2501">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="6288a-2502">Cloud</span><span class="sxs-lookup"><span data-stu-id="6288a-2502">Cloud</span></span>

* <span data-ttu-id="6288a-2503">`cloud [register|update]` geändert, um die Registrierung von Clouds ohne erforderliche Endpunkte zu verhindern</span><span class="sxs-lookup"><span data-stu-id="6288a-2503">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="6288a-2504">Container</span><span class="sxs-lookup"><span data-stu-id="6288a-2504">Container</span></span>

* <span data-ttu-id="6288a-2505">Unterstützung für das Öffnen mehrerer Ports hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2505">Added support to open multiple ports</span></span>
* <span data-ttu-id="6288a-2506">Neustartrichtlinie für Containergruppen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2506">Added container group restart policy</span></span>
* <span data-ttu-id="6288a-2507">Unterstützung zum Einbinden einer Azure-Dateifreigabe als Volume hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2507">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="6288a-2508">Hilfedokumente aktualisiert</span><span class="sxs-lookup"><span data-stu-id="6288a-2508">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="6288a-2509">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="6288a-2509">Data Lake Analytics</span></span>

* <span data-ttu-id="6288a-2510">`[job|account] list` geändert, um präzisere Informationen zu erhalten</span><span class="sxs-lookup"><span data-stu-id="6288a-2510">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="6288a-2511">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="6288a-2511">Data Lake Store</span></span>

* <span data-ttu-id="6288a-2512">`account list` geändert, um präzisere Informationen zu erhalten</span><span class="sxs-lookup"><span data-stu-id="6288a-2512">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="6288a-2513">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="6288a-2513">Extension</span></span>

* <span data-ttu-id="6288a-2514">`extension list-available` hinzugefügt, um das Auflisten offizieller Microsoft-Erweiterungen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="6288a-2514">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="6288a-2515">`--name` zu `extension [add|update]` hinzugefügt, um das Installieren von Erweiterungen nach Name zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="6288a-2515">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="6288a-2516">IoT</span><span class="sxs-lookup"><span data-stu-id="6288a-2516">IoT</span></span>

* <span data-ttu-id="6288a-2517">Unterstützung für Zertifizierungsstellen (CAs) und Zertifikatketten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2517">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="6288a-2518">Überwachen</span><span class="sxs-lookup"><span data-stu-id="6288a-2518">Monitor</span></span>

* <span data-ttu-id="6288a-2519">Befehle vom Typ `activity-log alert` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2519">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="6288a-2520">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6288a-2520">Network</span></span>

* <span data-ttu-id="6288a-2521">Unterstützung für CAA-DNS-Einträge hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2521">Added support for CAA DNS records</span></span>
* <span data-ttu-id="6288a-2522">Problem behoben, durch das Endpunkte nicht mit `traffic-manager profile update` aktualisiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="6288a-2522">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="6288a-2523">Problem behoben, durch das `vnet update --dns-servers` je nach VNet-Erstellungsmethode nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="6288a-2523">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="6288a-2524">Problem behoben, durch das relative DNS-Namen durch `dns zone import` nicht korrekt importiert wurden</span><span class="sxs-lookup"><span data-stu-id="6288a-2524">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="6288a-2525">Reservations</span><span class="sxs-lookup"><span data-stu-id="6288a-2525">Reservations</span></span>

* <span data-ttu-id="6288a-2526">Erste Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="6288a-2526">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="6288a-2527">Resource</span><span class="sxs-lookup"><span data-stu-id="6288a-2527">Resource</span></span>

* <span data-ttu-id="6288a-2528">Unterstützung für Ressourcen-IDs zum Parameter `--resource` und Sperren auf Ressourcenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2528">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="6288a-2529">SQL</span><span class="sxs-lookup"><span data-stu-id="6288a-2529">SQL</span></span>

* <span data-ttu-id="6288a-2530">Parameter `--ignore-missing-vnet-service-endpoint` zu `sql server vnet-rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2530">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="6288a-2531">Storage</span><span class="sxs-lookup"><span data-stu-id="6288a-2531">Storage</span></span>

* <span data-ttu-id="6288a-2532">`storage account create` geändert, sodass die SKU `Standard_RAGRS` als Standard verwendet wird</span><span class="sxs-lookup"><span data-stu-id="6288a-2532">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="6288a-2533">Fehler im Zusammenhang mit Datei-/Blobnamen korrigiert, die ASCII-fremde Zeichen enthalten</span><span class="sxs-lookup"><span data-stu-id="6288a-2533">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="6288a-2534">Fehler korrigiert, der die Verwendung von `--source-uri` mit `storage [blob|file] copy start-batch` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="6288a-2534">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="6288a-2535">Befehle zum Globalisieren und Löschen mehrerer Objekte mit `storage [blob|file] delete-batch` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2535">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="6288a-2536">Problem beim Aktivieren von Metriken mit `storage metrics update` behoben</span><span class="sxs-lookup"><span data-stu-id="6288a-2536">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="6288a-2537">Problem mit Dateien über 200 GB bei Verwendung von `storage blob upload-batch` behoben</span><span class="sxs-lookup"><span data-stu-id="6288a-2537">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="6288a-2538">Problem behoben, durch das `--bypass` und `--default-action` von `storage account [create|update]` ignoriert wurden</span><span class="sxs-lookup"><span data-stu-id="6288a-2538">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="6288a-2539">VM</span><span class="sxs-lookup"><span data-stu-id="6288a-2539">VM</span></span>

* <span data-ttu-id="6288a-2540">Fehler mit `vmss create` korrigiert, der die Verwendung der Größenebene `Basic` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="6288a-2540">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="6288a-2541">`--plan`-Argumente zu `[vm|vmss] create` für benutzerdefinierte Images mit Abrechnungsinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2541">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="6288a-2542">Befehle hinzugefügt: `vm secret `[add|remove|list]</span><span class="sxs-lookup"><span data-stu-id="6288a-2542">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="6288a-2543">`vm format-secret` in `vm secret format` umbenannt</span><span class="sxs-lookup"><span data-stu-id="6288a-2543">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="6288a-2544">Argument `--encrypt format` zu `vm encryption enable` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2544">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="6288a-2545">24. Oktober 2017</span><span class="sxs-lookup"><span data-stu-id="6288a-2545">October 24, 2017</span></span>

<span data-ttu-id="6288a-2546">Version 2.0.20</span><span class="sxs-lookup"><span data-stu-id="6288a-2546">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="6288a-2547">Core</span><span class="sxs-lookup"><span data-stu-id="6288a-2547">Core</span></span>

* <span data-ttu-id="6288a-2548">Aktualisierung von `2017-03-09-profile` zur Verwendung von Version `2016-01-01` der `MGMT_STORAGE`-API</span><span class="sxs-lookup"><span data-stu-id="6288a-2548">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="6288a-2549">ACR</span><span class="sxs-lookup"><span data-stu-id="6288a-2549">ACR</span></span>

* <span data-ttu-id="6288a-2550">Die Ressourcenverwaltung wurde aktualisiert und verweist nun auf die API-Version `2017-10-01`.</span><span class="sxs-lookup"><span data-stu-id="6288a-2550">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="6288a-2551">SKU „Bring Your Own Storage“ wurde in „Klassisch“ geändert.</span><span class="sxs-lookup"><span data-stu-id="6288a-2551">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="6288a-2552">Die Registrierungs-SKUs wurden in „Basic“, „Standard“ und „Premium“ umbenannt.</span><span class="sxs-lookup"><span data-stu-id="6288a-2552">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="6288a-2553">ACS</span><span class="sxs-lookup"><span data-stu-id="6288a-2553">ACS</span></span>

* <span data-ttu-id="6288a-2554">[VORSCHAUVERSION] Befehle vom Typ `az aks` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2554">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="6288a-2555">Problem mit `get-credentials` in Kubernetes behoben</span><span class="sxs-lookup"><span data-stu-id="6288a-2555">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="6288a-2556">AppService</span><span class="sxs-lookup"><span data-stu-id="6288a-2556">Appservice</span></span>

* <span data-ttu-id="6288a-2557">Problem behoben, aufgrund dessen heruntergeladene `webapp`-Protokolle unter Umständen ungültig waren</span><span class="sxs-lookup"><span data-stu-id="6288a-2557">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="6288a-2558">Komponente</span><span class="sxs-lookup"><span data-stu-id="6288a-2558">Component</span></span>

* <span data-ttu-id="6288a-2559">Deutlichere Meldung zur Einstellung für alle Installer und für Bestätigungsaufforderung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2559">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="6288a-2560">Überwachen</span><span class="sxs-lookup"><span data-stu-id="6288a-2560">Monitor</span></span>

* <span data-ttu-id="6288a-2561">Befehle vom Typ `action-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2561">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="6288a-2562">Resource</span><span class="sxs-lookup"><span data-stu-id="6288a-2562">Resource</span></span>

* <span data-ttu-id="6288a-2563">Inkompatibilität mit der aktuellen Version der msrest-Abhängigkeit in `group export` behoben</span><span class="sxs-lookup"><span data-stu-id="6288a-2563">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="6288a-2564">Problem mit `policy assignment create` behoben, sodass der Befehl mit integrierten Richtliniendefinitionen und Richtliniensatzdefinitionen verwendet werden kann</span><span class="sxs-lookup"><span data-stu-id="6288a-2564">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="6288a-2565">VM</span><span class="sxs-lookup"><span data-stu-id="6288a-2565">VM</span></span>

* <span data-ttu-id="6288a-2566">Argument `--accelerated-networking` zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2566">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="6288a-2567">9\. Oktober 2017</span><span class="sxs-lookup"><span data-stu-id="6288a-2567">October 9, 2017</span></span>

<span data-ttu-id="6288a-2568">Version 2.0.19</span><span class="sxs-lookup"><span data-stu-id="6288a-2568">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="6288a-2569">Core</span><span class="sxs-lookup"><span data-stu-id="6288a-2569">Core</span></span>

* <span data-ttu-id="6288a-2570">Verarbeitung von ADFS-Autoritäts-URLs wurde mit einem nachgestellten Schrägstrich zu Azure Stack hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-2570">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="6288a-2571">AppService</span><span class="sxs-lookup"><span data-stu-id="6288a-2571">Appservice</span></span>

* <span data-ttu-id="6288a-2572">Mit dem neuen Befehl `webapp update` wurde ein allgemeines Update hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-2572">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="6288a-2573">Batch</span><span class="sxs-lookup"><span data-stu-id="6288a-2573">Batch</span></span>

* <span data-ttu-id="6288a-2574">Aktualisierung auf Batch SDK 4.0.0</span><span class="sxs-lookup"><span data-stu-id="6288a-2574">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="6288a-2575">Die Option `--image` von „VirtualMachineConfiguration“ wurde aktualisiert, um zusätzlich zu „publish:offer:sku:version“ ARM-Imageverweise zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="6288a-2575">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="6288a-2576">Unterstützung für das neue CLI-Erweiterungsmodell für Batch-Erweiterungsbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2576">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="6288a-2577">Batch-Unterstützung aus dem Komponentenmodell entfernt</span><span class="sxs-lookup"><span data-stu-id="6288a-2577">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="6288a-2578">BatchAI</span><span class="sxs-lookup"><span data-stu-id="6288a-2578">Batchai</span></span>

* <span data-ttu-id="6288a-2579">Erste Version des Batch KI-Moduls</span><span class="sxs-lookup"><span data-stu-id="6288a-2579">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="6288a-2580">KeyVault</span><span class="sxs-lookup"><span data-stu-id="6288a-2580">Keyvault</span></span>

* <span data-ttu-id="6288a-2581">Key Vault-Authentifizierungsproblem behoben, das bei Verwendung von ADFS in Azure Stack auftrat.</span><span class="sxs-lookup"><span data-stu-id="6288a-2581">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="6288a-2582">(#4448)</span><span class="sxs-lookup"><span data-stu-id="6288a-2582">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="6288a-2583">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6288a-2583">Network</span></span>

* <span data-ttu-id="6288a-2584">Das Argument `--server` von `application-gateway address-pool create` ist nun optional, sodass leere Adresspools zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="6288a-2584">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="6288a-2585">`traffic-manager` wurde aktualisiert, um aktuelle Features zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="6288a-2585">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="6288a-2586">Resource</span><span class="sxs-lookup"><span data-stu-id="6288a-2586">Resource</span></span>

* <span data-ttu-id="6288a-2587">Zusätzliche Unterstützung für `--resource-group/-g`-Optionen für Ressourcengruppennamen zu `group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2587">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="6288a-2588">Befehle für `account lock` hinzugefügt, um die Verwendung mit Sperren auf Abonnementebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="6288a-2588">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="6288a-2589">Befehle für `group lock` hinzugefügt, um die Verwendung mit Sperren auf Gruppenebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="6288a-2589">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="6288a-2590">Befehle für `resource lock` hinzugefügt, um die Verwendung mit Sperren auf Ressourcenebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="6288a-2590">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="6288a-2591">Sql</span><span class="sxs-lookup"><span data-stu-id="6288a-2591">Sql</span></span>

* <span data-ttu-id="6288a-2592">Unterstützung für SQL Transparent Data Encryption (TDE) und TDE für Bring Your Own Key-Szenarien hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2592">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="6288a-2593">Der Befehl `db list-deleted` und der Parameter `db restore --deleted-time` wurden hinzugefügt, um die Ermittlung und Wiederherstellung gelöschter Datenbanken zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="6288a-2593">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="6288a-2594">`db op list` und `db op cancel` wurden hinzugefügt, um das Auflisten und Abbrechen ausgeführter Vorgänge für eine Datenbank zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="6288a-2594">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="6288a-2595">Storage</span><span class="sxs-lookup"><span data-stu-id="6288a-2595">Storage</span></span>

* <span data-ttu-id="6288a-2596">Unterstützung für Momentaufnahme von Dateifreigaben hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2596">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="6288a-2597">VM</span><span class="sxs-lookup"><span data-stu-id="6288a-2597">Vm</span></span>

* <span data-ttu-id="6288a-2598">Korrektur eines Fehlers in `vm show`, bei dem die Verwendung von `-d` in Verbindung mit fehlenden privaten IP-Adressen einen Absturz verursachte</span><span class="sxs-lookup"><span data-stu-id="6288a-2598">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="6288a-2599">[VORSCHAUVERSION] Unterstützung für paralleles Upgrade zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2599">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="6288a-2600">Unterstützung für das Aktualisieren der Verschlüsselungseinstellungen mit `vm encryption enable` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2600">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="6288a-2601">Parameter `--os-disk-size-gb` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2601">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="6288a-2602">Parameter `--license-type` für Windows zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2602">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="6288a-2603">22. September 2017</span><span class="sxs-lookup"><span data-stu-id="6288a-2603">September 22, 2017</span></span>

<span data-ttu-id="6288a-2604">Version 2.0.18</span><span class="sxs-lookup"><span data-stu-id="6288a-2604">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="6288a-2605">Resource</span><span class="sxs-lookup"><span data-stu-id="6288a-2605">Resource</span></span>

* <span data-ttu-id="6288a-2606">Unterstützung für das Anzeigen integrierter Richtliniendefinitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2606">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="6288a-2607">Unterstützungsmodusparameter zum Erstellen von Richtliniendefinitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2607">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="6288a-2608">Unterstützung für UI-Definitionen und -Vorlagen zu `managedapp definition create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2608">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="6288a-2609">[BREAKING CHANGE] Der Ressourcentyp `managedapp` wurde von `appliances` in `applications` und von `applianceDefinitions` in `applicationDefinitions` geändert.</span><span class="sxs-lookup"><span data-stu-id="6288a-2609">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="6288a-2610">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6288a-2610">Network</span></span>

* <span data-ttu-id="6288a-2611">Unterstützung für Verfügbarkeitszone zu Unterbefehlen `network lb` und `network public-ip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2611">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="6288a-2612">Unterstützung für IPv6-Microsoft-Peering zu `express-route` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2612">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="6288a-2613">Befehle für Anwendungssicherheitsgruppe `asg` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2613">Added `asg` application security group commands</span></span>
* <span data-ttu-id="6288a-2614">Argument `--application-security-groups` zu `nic [create|ip-config create|ip-config update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2614">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="6288a-2615">Argumente `--source-asgs` und `--destination-asgs` zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2615">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="6288a-2616">Argumente `--ddos-protection` und `--vm-protection` zu `vnet [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2616">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="6288a-2617">Befehle vom Typ `network [vnet-gateway|vpn-client|show-url]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2617">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="6288a-2618">Storage</span><span class="sxs-lookup"><span data-stu-id="6288a-2618">Storage</span></span>

* <span data-ttu-id="6288a-2619">Problem behoben, das nach der Aktualisierung des SDK unter Umständen einen Fehler der `storage account network-rule`-Befehle zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="6288a-2619">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="6288a-2620">Eventgrid</span><span class="sxs-lookup"><span data-stu-id="6288a-2620">Eventgrid</span></span>

* <span data-ttu-id="6288a-2621">Azure Event Grid Python SDK für die Verwendung der neueren API-Version „2017-09-15-preview“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="6288a-2621">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="6288a-2622">SQL</span><span class="sxs-lookup"><span data-stu-id="6288a-2622">SQL</span></span>

* <span data-ttu-id="6288a-2623">`sql server list`-Argument `--resource-group` geändert, sodass es nun optional ist.</span><span class="sxs-lookup"><span data-stu-id="6288a-2623">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="6288a-2624">Wird es nicht angegeben, werden alle SQL Server-Instanzen im Abonnement zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6288a-2624">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="6288a-2625">Parameter `--no-wait` zu `db [create|copy|restore|update|replica create|create|update]` und `dw [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2625">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="6288a-2626">KeyVault</span><span class="sxs-lookup"><span data-stu-id="6288a-2626">Keyvault</span></span>

* <span data-ttu-id="6288a-2627">Unterstützung für die Keyvault-Befehlsausführung hinter einem Proxy hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2627">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="6288a-2628">VM</span><span class="sxs-lookup"><span data-stu-id="6288a-2628">VM</span></span>

* <span data-ttu-id="6288a-2629">Unterstützung für Verfügbarkeitszone zu `[vm|vmss|disk] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2629">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="6288a-2630">Problem behoben, das bei Verwendung von `--app-gateway ID` mit `vmss create` einen Fehler zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="6288a-2630">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="6288a-2631">Argument `--asgs` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2631">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="6288a-2632">Unterstützung für die Ausführung von Befehlen auf virtuellen Computern mit `vm run-command` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2632">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="6288a-2633">[VORSCHAU] Unterstützung für VMSS-Datenträgerverschlüsselung mit `vmss encryption` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2633">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="6288a-2634">Unterstützung für die Durchführung der Wartung auf virtuellen Computern mit `vm perform-maintenance` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2634">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="6288a-2635">ACS</span><span class="sxs-lookup"><span data-stu-id="6288a-2635">ACS</span></span>

* <span data-ttu-id="6288a-2636">[VORSCHAU] Argument `--orchestrator-release` zu `acs create` für ACS-Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2636">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="6288a-2637">AppService</span><span class="sxs-lookup"><span data-stu-id="6288a-2637">Appservice</span></span>

* <span data-ttu-id="6288a-2638">Neue Möglichkeit zum Aktualisieren und Anzeigen der Authentifizierungseinstellungen mit `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="6288a-2638">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="6288a-2639">Backup</span><span class="sxs-lookup"><span data-stu-id="6288a-2639">Backup</span></span>

* <span data-ttu-id="6288a-2640">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="6288a-2640">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="6288a-2641">11. September 2017</span><span class="sxs-lookup"><span data-stu-id="6288a-2641">September 11, 2017</span></span>

<span data-ttu-id="6288a-2642">Version 2.0.17</span><span class="sxs-lookup"><span data-stu-id="6288a-2642">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="6288a-2643">Core</span><span class="sxs-lookup"><span data-stu-id="6288a-2643">Core</span></span>

* <span data-ttu-id="6288a-2644">Festlegung einer eigenen Korrelations-ID in Telemetrie durch das Befehlsmodul aktiviert</span><span class="sxs-lookup"><span data-stu-id="6288a-2644">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="6288a-2645">Ein Problem mit der JSON-Sicherungsdatei wurde behoben, das beim Festlegen des Diagnosemodus für Telemetrie auftrat</span><span class="sxs-lookup"><span data-stu-id="6288a-2645">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="6288a-2646">ACS</span><span class="sxs-lookup"><span data-stu-id="6288a-2646">Acs</span></span>

* <span data-ttu-id="6288a-2647">Befehl `acs list-locations` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2647">Added `acs list-locations` command</span></span>
* <span data-ttu-id="6288a-2648">`ssh-key-file` wird mit dem erwarteten Standardwert versehen.</span><span class="sxs-lookup"><span data-stu-id="6288a-2648">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="6288a-2649">AppService</span><span class="sxs-lookup"><span data-stu-id="6288a-2649">Appservice</span></span>

* <span data-ttu-id="6288a-2650">Neue Möglichkeit zum Erstellen einer Web-App in einer anderen Ressourcengruppe als der des aktiven Diensttarifs</span><span class="sxs-lookup"><span data-stu-id="6288a-2650">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="6288a-2651">CDN</span><span class="sxs-lookup"><span data-stu-id="6288a-2651">CDN</span></span>

* <span data-ttu-id="6288a-2652">Der Fehler bei `cdn custom-domain create`, dass „CustomDomain“ nicht wiederholbar ist, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="6288a-2652">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="6288a-2653">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="6288a-2653">Extension</span></span>

* <span data-ttu-id="6288a-2654">Erstrelease</span><span class="sxs-lookup"><span data-stu-id="6288a-2654">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="6288a-2655">KeyVault</span><span class="sxs-lookup"><span data-stu-id="6288a-2655">Keyvault</span></span>

* <span data-ttu-id="6288a-2656">Problem behoben, aufgrund dessen bei den Berechtigungen für `keyvault set-policy` die Groß-/Kleinschreibung beachtet werden musste</span><span class="sxs-lookup"><span data-stu-id="6288a-2656">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="6288a-2657">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6288a-2657">Network</span></span>

* <span data-ttu-id="6288a-2658">`vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="6288a-2658">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="6288a-2659">Das Argument `--private-access-services` wurde für `vnet subnet create/update` in `--service-endpoints` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="6288a-2659">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="6288a-2660">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2660">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="6288a-2661">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2661">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="6288a-2662">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2662">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="6288a-2663">Resource</span><span class="sxs-lookup"><span data-stu-id="6288a-2663">Resource</span></span>

* <span data-ttu-id="6288a-2664">Übergabe von Parameterdefinitionen für Ressourcenrichtlinien in `policy definition create` und `policy definition update` zulassen</span><span class="sxs-lookup"><span data-stu-id="6288a-2664">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="6288a-2665">Übergabe von Parameterwerten für `policy assignment create` zulassen</span><span class="sxs-lookup"><span data-stu-id="6288a-2665">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="6288a-2666">Übergabe von JSON-Code oder einer Datei für alle Parameter zulassen</span><span class="sxs-lookup"><span data-stu-id="6288a-2666">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="6288a-2667">Inkrementierte API-Version</span><span class="sxs-lookup"><span data-stu-id="6288a-2667">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="6288a-2668">SQL</span><span class="sxs-lookup"><span data-stu-id="6288a-2668">SQL</span></span>

* <span data-ttu-id="6288a-2669">Befehle vom Typ `sql server vnet-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2669">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="6288a-2670">VM</span><span class="sxs-lookup"><span data-stu-id="6288a-2670">VM</span></span>

* <span data-ttu-id="6288a-2671">Behoben: Zugriff nur zuweisen, wenn `--scope` angegeben wird</span><span class="sxs-lookup"><span data-stu-id="6288a-2671">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="6288a-2672">Behoben: Gleiche Erweiterungsbenennung wie Portal verwenden</span><span class="sxs-lookup"><span data-stu-id="6288a-2672">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="6288a-2673">`subscription` aus der Ausgabe von `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="6288a-2673">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="6288a-2674">Behoben: Speicher-SKU vom Typ `[vm|vmss] create` wird nicht auf Datenträger mit einem Image angewendet.</span><span class="sxs-lookup"><span data-stu-id="6288a-2674">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="6288a-2675">Behoben: `vm format-secret --secrets` akzeptierte keine durch neue Zeilen getrennte IDs.</span><span class="sxs-lookup"><span data-stu-id="6288a-2675">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="6288a-2676">31. August 2017</span><span class="sxs-lookup"><span data-stu-id="6288a-2676">August 31, 2017</span></span>

<span data-ttu-id="6288a-2677">Version 2.0.16</span><span class="sxs-lookup"><span data-stu-id="6288a-2677">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="6288a-2678">KeyVault</span><span class="sxs-lookup"><span data-stu-id="6288a-2678">Keyvault</span></span>

* <span data-ttu-id="6288a-2679">Fehler behoben, der beim Versuch auftrat, die Geheimniscodierung mit `secret download` automatisch aufzulösen</span><span class="sxs-lookup"><span data-stu-id="6288a-2679">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="6288a-2680">Sf</span><span class="sxs-lookup"><span data-stu-id="6288a-2680">Sf</span></span>

* <span data-ttu-id="6288a-2681">Alle Befehle wurden durch die Service Fabric-Befehlszeilenschnittstelle (sfctl) ersetzt.</span><span class="sxs-lookup"><span data-stu-id="6288a-2681">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="6288a-2682">Storage</span><span class="sxs-lookup"><span data-stu-id="6288a-2682">Storage</span></span>

* <span data-ttu-id="6288a-2683">Problem behoben, aufgrund dessen Speicherkonten nicht in Regionen erstellt werden konnten, die die NetworkACLs-Funktion nicht unterstützen</span><span class="sxs-lookup"><span data-stu-id="6288a-2683">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="6288a-2684">Festlegen des Inhaltstyps und der Inhaltscodierung während Blob- und Dateiuploads, wenn weder Inhaltstyp noch Inhaltscodierung angegeben sind</span><span class="sxs-lookup"><span data-stu-id="6288a-2684">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="6288a-2685">28. August 2017</span><span class="sxs-lookup"><span data-stu-id="6288a-2685">August 28, 2017</span></span>

<span data-ttu-id="6288a-2686">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="6288a-2686">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="6288a-2687">Befehlszeilenschnittstelle (CLI)</span><span class="sxs-lookup"><span data-stu-id="6288a-2687">CLI</span></span>

* <span data-ttu-id="6288a-2688">Rechtlichen Hinweis zu `--version` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2688">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="6288a-2689">ACS</span><span class="sxs-lookup"><span data-stu-id="6288a-2689">ACS</span></span>

* <span data-ttu-id="6288a-2690">Vorschauregionen korrigiert</span><span class="sxs-lookup"><span data-stu-id="6288a-2690">Corrected preview regions</span></span>
* <span data-ttu-id="6288a-2691">Standardmäßiges DNS-Namenspräfix (`dns_name_prefix`) ordnungsgemäß formatiert</span><span class="sxs-lookup"><span data-stu-id="6288a-2691">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="6288a-2692">ACS-Befehlsausgabe optimiert</span><span class="sxs-lookup"><span data-stu-id="6288a-2692">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="6288a-2693">AppService</span><span class="sxs-lookup"><span data-stu-id="6288a-2693">Appservice</span></span>

* <span data-ttu-id="6288a-2694">[BREAKING CHANGE] Inkonsistenzen in der Ausgabe von `az webapp config appsettings [delete|set]` behoben</span><span class="sxs-lookup"><span data-stu-id="6288a-2694">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="6288a-2695">Neuen Alias (`-i`) für `az webapp config container set --docker-custom-image-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2695">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="6288a-2696">`az webapp log show` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="6288a-2696">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="6288a-2697">Neue Argumente aus `az webapp delete` verfügbar gemacht, um App Service-Plan, Metriken oder DNS-Registrierung beizubehalten</span><span class="sxs-lookup"><span data-stu-id="6288a-2697">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="6288a-2698">Behoben: Korrekte Erkennung der Sloteinstellungen</span><span class="sxs-lookup"><span data-stu-id="6288a-2698">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="6288a-2699">IoT</span><span class="sxs-lookup"><span data-stu-id="6288a-2699">IoT</span></span>

* <span data-ttu-id="6288a-2700">#3934 behoben: Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="6288a-2700">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="6288a-2701">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6288a-2701">Network</span></span>

* <span data-ttu-id="6288a-2702">[BREAKING CHANGE]`vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="6288a-2702">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="6288a-2703">[BREAKING CHANGE] Option `--private-access-services` für `--service-endpoints` in `vnet subnet [create|update]` umbenannt</span><span class="sxs-lookup"><span data-stu-id="6288a-2703">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="6288a-2704">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2704">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="6288a-2705">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2705">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="6288a-2706">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2706">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="6288a-2707">Profil</span><span class="sxs-lookup"><span data-stu-id="6288a-2707">Profile</span></span>

* <span data-ttu-id="6288a-2708">`--msi` und `--msi-port` für die Anmeldung mit der Identität eines virtuellen Computers verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="6288a-2708">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="6288a-2709">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="6288a-2709">Service Fabric</span></span>

* <span data-ttu-id="6288a-2710">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="6288a-2710">Preview release</span></span>
* <span data-ttu-id="6288a-2711">Registrierungsbenutzer-/-kennwortregeln für Befehl vereinfacht</span><span class="sxs-lookup"><span data-stu-id="6288a-2711">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="6288a-2712">Kennwortanforderung für Benutzer trotz Parameterübergabe behoben</span><span class="sxs-lookup"><span data-stu-id="6288a-2712">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="6288a-2713">Unterstützung für leere Registrierungsanmeldeinformationen (`registry_cred`) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2713">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="6288a-2714">Storage</span><span class="sxs-lookup"><span data-stu-id="6288a-2714">Storage</span></span>

* <span data-ttu-id="6288a-2715">Festlegen des Blobtarifs ermöglicht</span><span class="sxs-lookup"><span data-stu-id="6288a-2715">Enabled setting blob tier</span></span>
* <span data-ttu-id="6288a-2716">Argumente `--bypass` und `--default-action` zur Unterstützung von Diensttunneling zu `storage account [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2716">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="6288a-2717">Befehle zum Hinzufügen von VNet-Regeln und IP-basierten Regeln zu `storage account network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2717">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="6288a-2718">Dienstverschlüsselung durch vom Kunden verwalteten Schlüssel ermöglicht</span><span class="sxs-lookup"><span data-stu-id="6288a-2718">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="6288a-2719">[BREAKING CHANGE] Option `--encryption` für Befehl `az storage account create and az storage account update` in `--encryption-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="6288a-2719">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="6288a-2720">Behoben (4220): `az storage account update encryption` – Syntaxkonflikt</span><span class="sxs-lookup"><span data-stu-id="6288a-2720">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="6288a-2721">VM</span><span class="sxs-lookup"><span data-stu-id="6288a-2721">VM</span></span>

* <span data-ttu-id="6288a-2722">Problem behoben, aufgrund dessen bei Verwendung von `--instance-id *` zusätzliche, fehlerhafte Informationen für `vmss get-instance-view` angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="6288a-2722">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="6288a-2723">Unterstützung für `--lb-sku` zu `vmss create` hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="6288a-2723">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="6288a-2724">Menschliche Namen aus der Administratornamen-Blacklist für `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="6288a-2724">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="6288a-2725">Problem behoben, aufgrund dessen `[vm|vmss] create` einen Fehler ausgelöst hat, wenn aus einem Image keine Tarifinformationen extrahiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="6288a-2725">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="6288a-2726">Absturzproblem beim Erstellen einer VMMS-Skalierungsgruppe mit einem internen Lastenausgleich behoben</span><span class="sxs-lookup"><span data-stu-id="6288a-2726">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="6288a-2727">Problem behoben, aufgrund dessen das Argument `--no-wait` nicht mit `vm availability-set create` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="6288a-2727">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="6288a-2728">15. August 2017</span><span class="sxs-lookup"><span data-stu-id="6288a-2728">August 15, 2017</span></span>

<span data-ttu-id="6288a-2729">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="6288a-2729">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="6288a-2730">ACS</span><span class="sxs-lookup"><span data-stu-id="6288a-2730">ACS</span></span>

* <span data-ttu-id="6288a-2731">sshMaster0-Portnummer für Kubernetes korrigiert</span><span class="sxs-lookup"><span data-stu-id="6288a-2731">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="6288a-2732">AppService</span><span class="sxs-lookup"><span data-stu-id="6288a-2732">Appservice</span></span>

* <span data-ttu-id="6288a-2733">Ausnahme beim Erstellen einer neuen Git-basierten Linux-Web-App behoben</span><span class="sxs-lookup"><span data-stu-id="6288a-2733">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="6288a-2734">Event Grid</span><span class="sxs-lookup"><span data-stu-id="6288a-2734">Event Grid</span></span>

* <span data-ttu-id="6288a-2735">SDK-Abhängigkeiten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2735">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="6288a-2736">11. August 2017</span><span class="sxs-lookup"><span data-stu-id="6288a-2736">August 11, 2017</span></span>

<span data-ttu-id="6288a-2737">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="6288a-2737">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="6288a-2738">ACS</span><span class="sxs-lookup"><span data-stu-id="6288a-2738">ACS</span></span>

* <span data-ttu-id="6288a-2739">Weitere Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2739">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="6288a-2740">Batch</span><span class="sxs-lookup"><span data-stu-id="6288a-2740">Batch</span></span>

* <span data-ttu-id="6288a-2741">Auf Batch SDK 3.1.0 und Batch Management SDK 4.1.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="6288a-2741">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="6288a-2742">Neuen Befehl zum Anzeigen der Aufgabenanzahl eines Auftrags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2742">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="6288a-2743">Fehler in der SAS-URL-Verarbeitung der Ressourcendatei behoben</span><span class="sxs-lookup"><span data-stu-id="6288a-2743">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="6288a-2744">Batch-Kontoendpunkt unterstützt nun optionales Präfix „https://“</span><span class="sxs-lookup"><span data-stu-id="6288a-2744">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="6288a-2745">Unterstützung für das Hinzufügen von Listen mit mehr als 100 Aufgaben zu einem Auftrag</span><span class="sxs-lookup"><span data-stu-id="6288a-2745">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="6288a-2746">Debugprotokollierung für das Laden des Erweiterungsbefehlsmoduls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2746">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="6288a-2747">Komponente</span><span class="sxs-lookup"><span data-stu-id="6288a-2747">Component</span></span>

* <span data-ttu-id="6288a-2748">Warnung für veraltete Befehle vom Typ „az component“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2748">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="6288a-2749">Container</span><span class="sxs-lookup"><span data-stu-id="6288a-2749">Container</span></span>

* <span data-ttu-id="6288a-2750">`create`: Problem behoben, aufgrund dessen das Gleichheitszeichen innerhalb einer Umgebungsvariablen nicht zulässig war</span><span class="sxs-lookup"><span data-stu-id="6288a-2750">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="6288a-2751">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="6288a-2751">Data Lake Store</span></span>

* <span data-ttu-id="6288a-2752">Fortschrittsüberwachung ermöglicht</span><span class="sxs-lookup"><span data-stu-id="6288a-2752">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="6288a-2753">Event Grid</span><span class="sxs-lookup"><span data-stu-id="6288a-2753">Event Grid</span></span>

* <span data-ttu-id="6288a-2754">Erste Veröffentlichung</span><span class="sxs-lookup"><span data-stu-id="6288a-2754">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="6288a-2755">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6288a-2755">Network</span></span>

* <span data-ttu-id="6288a-2756">`lb`: Problem behoben, aufgrund dessen bestimmte Namen untergeordneter Ressourcen bei Auslassung nicht richtig aufgelöst wurden</span><span class="sxs-lookup"><span data-stu-id="6288a-2756">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="6288a-2757">`application-gateway {subresource} delete`: Problem behoben, aufgrund dessen `--no-wait` nicht berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="6288a-2757">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="6288a-2758">`application-gateway http-settings update`: Problem behoben, aufgrund dessen `--connection-draining-timeout` nicht deaktiviert werden konnte</span><span class="sxs-lookup"><span data-stu-id="6288a-2758">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="6288a-2759">Fehler behoben: Unerwartetes Schlüsselwortargument `sa_data_size_kilobyes` bei `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="6288a-2759">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="6288a-2760">Profil</span><span class="sxs-lookup"><span data-stu-id="6288a-2760">Profile</span></span>

* <span data-ttu-id="6288a-2761">`account list`: `--refresh` hinzugefügt, um die neuesten Abonnements vom Server zu synchronisieren</span><span class="sxs-lookup"><span data-stu-id="6288a-2761">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="6288a-2762">Storage</span><span class="sxs-lookup"><span data-stu-id="6288a-2762">Storage</span></span>

* <span data-ttu-id="6288a-2763">Aktualisieren des Speicherkontos mit vom System zugewiesener Identität ermöglicht</span><span class="sxs-lookup"><span data-stu-id="6288a-2763">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="6288a-2764">VM</span><span class="sxs-lookup"><span data-stu-id="6288a-2764">VM</span></span>

* <span data-ttu-id="6288a-2765">`availability-set`: Fehlerdomänenanzahl bei Konvertierung verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="6288a-2765">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="6288a-2766">Befehl `list-skus` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="6288a-2766">Exposed `list-skus` command</span></span>
* <span data-ttu-id="6288a-2767">Unterstützung der Identitätszuweisung ohne Erstellung von Rollenzuweisungen</span><span class="sxs-lookup"><span data-stu-id="6288a-2767">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="6288a-2768">Anwenden von Speicher-SKU beim Anfügen von Datenträgern</span><span class="sxs-lookup"><span data-stu-id="6288a-2768">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="6288a-2769">Standardmäßiger Betriebssystemdatenträger-Name und Speicher-SKU bei Verwendung verwalteter Datenträger entfernt</span><span class="sxs-lookup"><span data-stu-id="6288a-2769">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="6288a-2770">28. Juli 2017</span><span class="sxs-lookup"><span data-stu-id="6288a-2770">July 28, 2017</span></span>

<span data-ttu-id="6288a-2771">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="6288a-2771">Version 2.0.12</span></span>

* <span data-ttu-id="6288a-2772">Containerbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2772">Added container commands</span></span>
* <span data-ttu-id="6288a-2773">Abrechnungs- und Nutzungsmodule hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2773">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="6288a-2774">Core</span><span class="sxs-lookup"><span data-stu-id="6288a-2774">Core</span></span>

* <span data-ttu-id="6288a-2775">Ausgabe von SDK-Authentifizierungsinformationen für Dienstprinzipale mit Zertifikaten</span><span class="sxs-lookup"><span data-stu-id="6288a-2775">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="6288a-2776">Ausnahmen beim Bereitstellungsfortschritt behoben</span><span class="sxs-lookup"><span data-stu-id="6288a-2776">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="6288a-2777">Verwendung des ARM-Endpunkts aus der aktuellen Cloud für die Erstellung des Abonnementclients</span><span class="sxs-lookup"><span data-stu-id="6288a-2777">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="6288a-2778">Gleichzeitige Verarbeitung der Datei „clouds.config“ verbessert (3636)</span><span class="sxs-lookup"><span data-stu-id="6288a-2778">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="6288a-2779">Aktualisierung der Clientanforderungs-ID für jede Befehlsausführung</span><span class="sxs-lookup"><span data-stu-id="6288a-2779">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="6288a-2780">Erstellung von Abonnementclients mit richtigem SDK-Profil (3635)</span><span class="sxs-lookup"><span data-stu-id="6288a-2780">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="6288a-2781">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="6288a-2781">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="6288a-2782">Unterstützung für Auswahl von Tabellenausgabefeldern über jmespath Abfrage hinzugefügt (3581)</span><span class="sxs-lookup"><span data-stu-id="6288a-2782">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="6288a-2783">Stummschaltung von Analyseargumenten und Anfügeverlauf mit Gesten verbessert (3434)</span><span class="sxs-lookup"><span data-stu-id="6288a-2783">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="6288a-2784">Erstellung von Abonnementclients mit richtigem SDK-Profil</span><span class="sxs-lookup"><span data-stu-id="6288a-2784">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="6288a-2785">Verschiebung aller vorhandenen Erfassungsdateien in den neuesten Ordner</span><span class="sxs-lookup"><span data-stu-id="6288a-2785">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="6288a-2786">Idempotenz für VM-/VMSS-Erstellung behoben (3586)</span><span class="sxs-lookup"><span data-stu-id="6288a-2786">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="6288a-2787">Bei Befehlspfaden wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="6288a-2787">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="6288a-2788">Bei bestimmten booleschen Parametern wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="6288a-2788">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="6288a-2789">Unterstützung der Anmeldung bei lokalem AD FS-Server wie Azure Stack</span><span class="sxs-lookup"><span data-stu-id="6288a-2789">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="6288a-2790">Gleichzeitige Schreibvorgänge in „clouds.config“ behoben (3255)</span><span class="sxs-lookup"><span data-stu-id="6288a-2790">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="6288a-2791">ACR</span><span class="sxs-lookup"><span data-stu-id="6288a-2791">ACR</span></span>

* <span data-ttu-id="6288a-2792">Befehl `show-usage` für verwaltete Registrierungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2792">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="6288a-2793">Unterstützung der SKU-Aktualisierung für verwaltete Registrierungen</span><span class="sxs-lookup"><span data-stu-id="6288a-2793">Support SKU update for managed registries</span></span>
* <span data-ttu-id="6288a-2794">Verwaltete Registrierungen mit verwalteter SKU hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2794">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="6288a-2795">Webhooks für verwaltete Registrierungen mit ACR-Webhook-Befehlsmodul hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2795">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="6288a-2796">AAD-Authentifizierung mit ACR-Anmeldebefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2796">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="6288a-2797">Löschbefehl für Docker-Repositorys, Manifeste und Tags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2797">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="6288a-2798">ACS</span><span class="sxs-lookup"><span data-stu-id="6288a-2798">ACS</span></span>

* <span data-ttu-id="6288a-2799">Unterstützung der API-Version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="6288a-2799">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="6288a-2800">AppService</span><span class="sxs-lookup"><span data-stu-id="6288a-2800">Appservice</span></span>

* <span data-ttu-id="6288a-2801">Fehler behoben, aufgrund dessen die Auflistung der Linux-Web-App keine Werte zurückgegeben hat</span><span class="sxs-lookup"><span data-stu-id="6288a-2801">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="6288a-2802">Unterstützung für das Abrufen von Anmeldeinformationen aus dem ACR</span><span class="sxs-lookup"><span data-stu-id="6288a-2802">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="6288a-2803">Entfernung aller Befehle unter `appservice web`</span><span class="sxs-lookup"><span data-stu-id="6288a-2803">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="6288a-2804">Maskierung von Docker-Registrierungskennwörtern aus der Befehlsausgabe (3656)</span><span class="sxs-lookup"><span data-stu-id="6288a-2804">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="6288a-2805">Gewährleistung der fehlerfreien Verwendung des Standardbrowsers unter macOS (3623)</span><span class="sxs-lookup"><span data-stu-id="6288a-2805">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="6288a-2806">Verbesserung des Nutzens von `webapp log tail` und `webapp log download` (3624)</span><span class="sxs-lookup"><span data-stu-id="6288a-2806">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="6288a-2807">Befehl `traffic-routing` zum Konfigurieren des statischen Routings verfügbar gemacht (3566)</span><span class="sxs-lookup"><span data-stu-id="6288a-2807">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="6288a-2808">Zuverlässigkeit beim Konfigurieren der Quellcodeverwaltung verbessert (3245)</span><span class="sxs-lookup"><span data-stu-id="6288a-2808">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="6288a-2809">Nicht unterstütztes Argument `--node-version` aus `webapp config update` für Windows-Web-Apps entfernt.</span><span class="sxs-lookup"><span data-stu-id="6288a-2809">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="6288a-2810">Verwenden Sie stattdessen `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="6288a-2810">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="6288a-2811">Batch</span><span class="sxs-lookup"><span data-stu-id="6288a-2811">Batch</span></span>

* <span data-ttu-id="6288a-2812">Auf Batch SDK 3.0.0 mit Unterstützung virtueller Computer mit niedriger Priorität in Pools aktualisiert</span><span class="sxs-lookup"><span data-stu-id="6288a-2812">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="6288a-2813">`pool create`-Option `--target-dedicated` in `--target-dedicated-nodes` umbenannt</span><span class="sxs-lookup"><span data-stu-id="6288a-2813">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="6288a-2814">`pool create`-Optionen `--target-low-priority-nodes` und `--application-licenses` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2814">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="6288a-2815">CDN</span><span class="sxs-lookup"><span data-stu-id="6288a-2815">CDN</span></span>

* <span data-ttu-id="6288a-2816">Besser verständliche Fehlermeldung für `cdn endpoint list`, wenn das von `--profile-name` angegebene Profil nicht vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="6288a-2816">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="6288a-2817">Cloud</span><span class="sxs-lookup"><span data-stu-id="6288a-2817">Cloud</span></span>

* <span data-ttu-id="6288a-2818">API-Version des Cloudmetadaten-Endpunkts in das Format JJJJ-MM-TT umgewandelt</span><span class="sxs-lookup"><span data-stu-id="6288a-2818">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="6288a-2819">Katalogendpunkt nicht erforderlich</span><span class="sxs-lookup"><span data-stu-id="6288a-2819">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="6288a-2820">Unterstützung für die Cloudregistrierung nur mit ARM-Endpunkt</span><span class="sxs-lookup"><span data-stu-id="6288a-2820">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="6288a-2821">Option für `cloud set` bereitgestellt, um beim Auswählen der aktuellen Cloud das Profil auswählen zu können</span><span class="sxs-lookup"><span data-stu-id="6288a-2821">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="6288a-2822">`endpoint_vm_image_alias_doc` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="6288a-2822">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="6288a-2823">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="6288a-2823">CosmosDB</span></span>

* <span data-ttu-id="6288a-2824">Möglichkeit zum Erstellen einer Auflistung mit benutzerdefiniertem Partitionsschlüssel behoben</span><span class="sxs-lookup"><span data-stu-id="6288a-2824">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="6288a-2825">Unterstützung für Auflistungs-Standardgültigkeitsdauer hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2825">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="6288a-2826">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="6288a-2826">Data Lake Analytics</span></span>

* <span data-ttu-id="6288a-2827">Zusätzliche Befehle für Compute-Richtlinienverwaltung unter der Überschrift `dla account compute-policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2827">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="6288a-2828">`dla job pipeline show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2828">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="6288a-2829">`dla job recurrence list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2829">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="6288a-2830">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="6288a-2830">Data Lake Store</span></span>

* <span data-ttu-id="6288a-2831">Unterstützung für vom Benutzer verwaltete Schlüsseltresor-Schlüsselrotation in `dls account update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2831">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="6288a-2832">Zugrunde liegende SDK-Version des Data Lake Store-Dateisystems aktualisiert, um ein Leistungsproblem zu behandeln</span><span class="sxs-lookup"><span data-stu-id="6288a-2832">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="6288a-2833">Befehl `dls enable-key-vault` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="6288a-2833">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="6288a-2834">Dieser Befehl versucht, eine vom Benutzer angegebene Key Vault-Instanz zur Verschlüsselung der Daten in einem Data Lake Store-Konto zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="6288a-2834">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="6288a-2835">Interactive</span><span class="sxs-lookup"><span data-stu-id="6288a-2835">Interactive</span></span>

* <span data-ttu-id="6288a-2836">Startzeit durch Verwendung zwischengespeicherter Befehle verbessert</span><span class="sxs-lookup"><span data-stu-id="6288a-2836">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="6288a-2837">Testabdeckung verbessert</span><span class="sxs-lookup"><span data-stu-id="6288a-2837">Increased test coverage</span></span>
* <span data-ttu-id="6288a-2838">?-Geste erweitert, sodass sie auch in den nächsten Befehl eingefügt wird</span><span class="sxs-lookup"><span data-stu-id="6288a-2838">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="6288a-2839">Interaktive Fehler mit dem Profil „2017-03-09-profile-preview“ behoben (3587)</span><span class="sxs-lookup"><span data-stu-id="6288a-2839">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="6288a-2840">`--version` als Parameter für den interaktiven Modus zugelassen (3645)</span><span class="sxs-lookup"><span data-stu-id="6288a-2840">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="6288a-2841">Beseitigung von Fehlern im interaktiven Modus beim Abschluss von Überprüfungen (3570)</span><span class="sxs-lookup"><span data-stu-id="6288a-2841">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="6288a-2842">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="6288a-2842">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="6288a-2843">Flag `--progress` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2843">Added `--progress` flag</span></span>
* <span data-ttu-id="6288a-2844">`--debug` und `--verbose` aus Abschlüssen entfernt</span><span class="sxs-lookup"><span data-stu-id="6288a-2844">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="6288a-2845">`interactive` aus Abschlüssen entfernt (3324)</span><span class="sxs-lookup"><span data-stu-id="6288a-2845">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="6288a-2846">IoT</span><span class="sxs-lookup"><span data-stu-id="6288a-2846">IoT</span></span>

* <span data-ttu-id="6288a-2847">Behoben: Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="6288a-2847">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="6288a-2848">(3934)</span><span class="sxs-lookup"><span data-stu-id="6288a-2848">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="6288a-2849">Schlüsseltresor</span><span class="sxs-lookup"><span data-stu-id="6288a-2849">Key vault</span></span>

* <span data-ttu-id="6288a-2850">Befehle für Schlüsseltresor-Wiederherstellungsfeatures hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="6288a-2850">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="6288a-2851">`keyvault`-Unterbefehle: `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="6288a-2851">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="6288a-2852">`keyvault secret`-Unterbefehle: `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="6288a-2852">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="6288a-2853">`keyvault certificate`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="6288a-2853">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="6288a-2854">`keyvault key`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="6288a-2854">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="6288a-2855">Dienstprinzipal-Schlüsseltresorintegration hinzugefügt (3133)</span><span class="sxs-lookup"><span data-stu-id="6288a-2855">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="6288a-2856">Schlüsseltresor-Datenebene auf 0.3.2. aktualisiert</span><span class="sxs-lookup"><span data-stu-id="6288a-2856">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="6288a-2857">(3307)</span><span class="sxs-lookup"><span data-stu-id="6288a-2857">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="6288a-2858">Labor</span><span class="sxs-lookup"><span data-stu-id="6288a-2858">Lab</span></span>

* <span data-ttu-id="6288a-2859">Unterstützung für Übernahme eines beliebigen virtuellen Computers im Labor über `az lab vm claim` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2859">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="6288a-2860">Tabellenausgabeformatierer für `az lab vm list` und `az lab vm show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2860">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="6288a-2861">Überwachen</span><span class="sxs-lookup"><span data-stu-id="6288a-2861">Monitor</span></span>

* <span data-ttu-id="6288a-2862">Korrektur für Vorlagendatei mit Befehl `monitor autoscale-settings get-parameters-template` (3349)</span><span class="sxs-lookup"><span data-stu-id="6288a-2862">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="6288a-2863">`monitor alert-rule-incidents list` in `monitor alert list-incidents` umbenannt</span><span class="sxs-lookup"><span data-stu-id="6288a-2863">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="6288a-2864">`monitor alert-rule-incidents show` in `monitor alert show-incident` umbenannt</span><span class="sxs-lookup"><span data-stu-id="6288a-2864">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="6288a-2865">`monitor metric-defintions list` in `monitor metrics list-definitions` umbenannt</span><span class="sxs-lookup"><span data-stu-id="6288a-2865">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="6288a-2866">`monitor alert-rules` in `monitor alert` umbenannt</span><span class="sxs-lookup"><span data-stu-id="6288a-2866">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="6288a-2867">`monitor alert create` geändert:</span><span class="sxs-lookup"><span data-stu-id="6288a-2867">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="6288a-2868">Unterbefehle vom Typ `condition` und `action` akzeptieren keinen JSON-Code mehr.</span><span class="sxs-lookup"><span data-stu-id="6288a-2868">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="6288a-2869">Hinzufügung zahlreicher Parameter zur Vereinfachung der Regelerstellung</span><span class="sxs-lookup"><span data-stu-id="6288a-2869">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="6288a-2870">`location` nicht mehr erforderlich</span><span class="sxs-lookup"><span data-stu-id="6288a-2870">`location` no longer required</span></span>
  * <span data-ttu-id="6288a-2871">Hinzufügung von Namen- und ID-Unterstützung für Ziel</span><span class="sxs-lookup"><span data-stu-id="6288a-2871">Add name and ID support for target</span></span>
  * <span data-ttu-id="6288a-2872">Entfernung von `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="6288a-2872">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="6288a-2873">Umbenennung von `is-enabled` in `enabled` (nicht mehr erforderlich)</span><span class="sxs-lookup"><span data-stu-id="6288a-2873">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="6288a-2874">`description` wird nun abhängig von der angegebenen Bedingung auf einen Standardwert festgelegt.</span><span class="sxs-lookup"><span data-stu-id="6288a-2874">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="6288a-2875">Hinzufügung von Beispielen zur Verdeutlichung des neuen Formats</span><span class="sxs-lookup"><span data-stu-id="6288a-2875">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="6288a-2876">Unterstützung von Namen oder IDs für Befehle vom Typ `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="6288a-2876">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="6288a-2877">Komfortargumente und Beispiele zu `monitor alert rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2877">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="6288a-2878">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6288a-2878">Network</span></span>

* <span data-ttu-id="6288a-2879">Befehl `list-private-access-services` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2879">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="6288a-2880">Argument `--private-access-services` zu `vnet subnet create` und `vnet subnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2880">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="6288a-2881">Problem behoben, das einen Fehler für `application-gateway redirect-config create` zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="6288a-2881">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="6288a-2882">Problem behoben, aufgrund dessen `application-gateway redirect-config update` nicht mit `--no-wait` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="6288a-2882">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="6288a-2883">Fehler behoben, der bei der Verwendung des Arguments `--servers` mit `application-gateway address-pool create` und `application-gateway address-pool update` aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="6288a-2883">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="6288a-2884">Befehle vom Typ `application-gateway redirect-config` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2884">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="6288a-2885">Befehle zu `application-gateway ssl-policy` hinzugefügt: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="6288a-2885">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="6288a-2886">Argumente zu `application-gateway ssl-policy set` hinzugefügt: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="6288a-2886">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="6288a-2887">Argumente zu `application-gateway http-settings create` und `application-gateway http-settings update` hinzugefügt: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="6288a-2887">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="6288a-2888">Argumente zu `application-gateway url-path-map create` und `application-gateway url-path-map update` hinzugefügt: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="6288a-2888">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="6288a-2889">Argument `--redirect-config` zu `application-gateway url-path-map rule create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2889">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="6288a-2890">Unterstützung für `--no-wait` zu `application-gateway url-path-map rule delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2890">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="6288a-2891">Argumente zu `application-gateway probe create` und `application-gateway probe update` hinzugefügt: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="6288a-2891">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="6288a-2892">Argument `--redirect-config` zu `application-gateway rule create` und `application-gateway rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2892">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="6288a-2893">Unterstützung für `--accelerated-networking` zu `nic create` und `nic update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2893">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="6288a-2894">Argument `--internal-dns-name-suffix` von `nic create` entfernt</span><span class="sxs-lookup"><span data-stu-id="6288a-2894">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="6288a-2895">Unterstützung für `--dns-servers` zu `nic update` und `nic create` hinzugefügt: Hinzufügung von Unterstützung für --dns-servers</span><span class="sxs-lookup"><span data-stu-id="6288a-2895">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="6288a-2896">Fehler korrigiert, aufgrund dessen `--local-address-prefixes` von `local-gateway create` ignoriert wurde</span><span class="sxs-lookup"><span data-stu-id="6288a-2896">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="6288a-2897">Unterstützung für `--dns-servers` zu `vnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2897">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="6288a-2898">Fehler beim Erstellen eines Peerings ohne Routenfilterung mit `express-route peering create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="6288a-2898">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="6288a-2899">Fehler korrigiert, aufgrund dessen die Argumente `--provider` und `--bandwidth` nicht mit `express-route update` verwendet werden konnten</span><span class="sxs-lookup"><span data-stu-id="6288a-2899">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="6288a-2900">Fehler mit Standardlogik von `network watcher show-topology` korrigiert</span><span class="sxs-lookup"><span data-stu-id="6288a-2900">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="6288a-2901">Ausgabeformatierung für `network list-usages` verbessert</span><span class="sxs-lookup"><span data-stu-id="6288a-2901">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="6288a-2902">Verwendung der standardmäßigen Front-End-IP-Adresse für `application-gateway http-listener create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="6288a-2902">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="6288a-2903">Verwendung des Standardadresspools, der HTTP-Standardeinstellungen und des HTTP-Standardlisteners für `application-gateway rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="6288a-2903">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="6288a-2904">Verwendung der standardmäßigen Front-End-IP-Adresse und des standardmäßigen Back-End-Pools für `lb rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="6288a-2904">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="6288a-2905">Verwendung der standardmäßigen Front-End-IP-Adresse für `lb inbound-nat-rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="6288a-2905">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="6288a-2906">Profil</span><span class="sxs-lookup"><span data-stu-id="6288a-2906">Profile</span></span>

* <span data-ttu-id="6288a-2907">Unterstützung der Anmeldung innerhalb eines virtuellen Computers mit einer verwalteten Identität</span><span class="sxs-lookup"><span data-stu-id="6288a-2907">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="6288a-2908">Unterstützung der Ausgabe für `account show` im SDK-Authentifizierungsdateiformat</span><span class="sxs-lookup"><span data-stu-id="6288a-2908">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="6288a-2909">Anzeige von Warnungen für veraltete Befehle bei Verwendung von „--expanded-view“</span><span class="sxs-lookup"><span data-stu-id="6288a-2909">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="6288a-2910">Befehl `get-access-token` für die Bereitstellung eines unformatierten AAD-Tokens hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2910">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="6288a-2911">Unterstützung der Anmeldung mit einem Benutzerkonto ohne zugeordnete Abonnements</span><span class="sxs-lookup"><span data-stu-id="6288a-2911">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="6288a-2912">RDBMS</span><span class="sxs-lookup"><span data-stu-id="6288a-2912">RDBMS</span></span>

* <span data-ttu-id="6288a-2913">Unterstützung der abonnementübergreifenden Auflistung von Servern (3417)</span><span class="sxs-lookup"><span data-stu-id="6288a-2913">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="6288a-2914">Behoben: `%s` wird aufgrund von fehlendem `% server_type` nicht verarbeitet (3393)</span><span class="sxs-lookup"><span data-stu-id="6288a-2914">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="6288a-2915">Dokumentquellenzuordnung behoben und CI-Aufgabe zur Überprüfung hinzugefügt (3361)</span><span class="sxs-lookup"><span data-stu-id="6288a-2915">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="6288a-2916">MySQL- und PostgreSQL-Hilfe korrigiert (3369)</span><span class="sxs-lookup"><span data-stu-id="6288a-2916">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="6288a-2917">Resource</span><span class="sxs-lookup"><span data-stu-id="6288a-2917">Resource</span></span>

* <span data-ttu-id="6288a-2918">Eingabeaufforderungen bei fehlenden Parametern für `group deployment create` verbessert</span><span class="sxs-lookup"><span data-stu-id="6288a-2918">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="6288a-2919">Analyse der Syntax `--parameters KEY=VALUE` verbessert</span><span class="sxs-lookup"><span data-stu-id="6288a-2919">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="6288a-2920">Probleme behoben, durch die Parameterdateien von `group deployment create` bei Verwendung der Syntax `@<file>` nicht mehr erkannt wurden</span><span class="sxs-lookup"><span data-stu-id="6288a-2920">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="6288a-2921">Unterstützung des Arguments `--ids` für Befehle vom Typ `resource` und `managedapp`</span><span class="sxs-lookup"><span data-stu-id="6288a-2921">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="6288a-2922">Einige Analyse- und Fehlermeldungen korrigiert (3584)</span><span class="sxs-lookup"><span data-stu-id="6288a-2922">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="6288a-2923">Analyse vom Typ `--resource-type` für den Befehl `lock` korrigiert, sodass `<resource-namespace>` und `<resource-type>` akzeptiert werden</span><span class="sxs-lookup"><span data-stu-id="6288a-2923">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="6288a-2924">Parameterüberprüfung für Vorlagenlinkvorlagen hinzugefügt (3629)</span><span class="sxs-lookup"><span data-stu-id="6288a-2924">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="6288a-2925">Unterstützung für die Angabe von Bereitstellungsparametern mit der Syntax `KEY=VALUE` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2925">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="6288a-2926">Role</span><span class="sxs-lookup"><span data-stu-id="6288a-2926">Role</span></span>

* <span data-ttu-id="6288a-2927">Unterstützung der Ausgabe im SDK-Authentifizierungsdateiformat für `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="6288a-2927">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="6288a-2928">Rollenzuweisungen und dazugehörige AAD-Anwendung beim Löschen eines Dienstprinzipals bereinigt (3610)</span><span class="sxs-lookup"><span data-stu-id="6288a-2928">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="6288a-2929">Einbeziehung des Zeitformats in Beschreibungen vom Typ `--start-date` und `--end-date` für `app create`-Argumente</span><span class="sxs-lookup"><span data-stu-id="6288a-2929">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="6288a-2930">Anzeige von Warnungen für veraltete Befehle bei Verwendung von `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="6288a-2930">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="6288a-2931">Schlüsseltresorintegration zu den Befehlen `create-for-rbac` und `reset-credentials` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2931">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="6288a-2932">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="6288a-2932">Service Fabric</span></span>
* <span data-ttu-id="6288a-2933">Problem behoben, aufgrund dessen große Dateien in Anwendungen beim Hochladen gekürzt wurden (3666)</span><span class="sxs-lookup"><span data-stu-id="6288a-2933">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="6288a-2934">Tests für Service Fabric-Befehle hinzugefügt (3424)</span><span class="sxs-lookup"><span data-stu-id="6288a-2934">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="6288a-2935">Zahlreiche Service Fabric-Befehle korrigiert (3234)</span><span class="sxs-lookup"><span data-stu-id="6288a-2935">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="6288a-2936">SQL</span><span class="sxs-lookup"><span data-stu-id="6288a-2936">SQL</span></span>

* <span data-ttu-id="6288a-2937">Fehlerhafte1 Parameter `--identity` für `sql server create` entfernt</span><span class="sxs-lookup"><span data-stu-id="6288a-2937">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="6288a-2938">Kennwortwerte aus der Befehlsausgabe von `sql server create` und `sql server update` entfernt</span><span class="sxs-lookup"><span data-stu-id="6288a-2938">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="6288a-2939">Befehle `sql db list-editions` und `sql elastic-pool list-editions` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-2939">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="6288a-2940">Storage</span><span class="sxs-lookup"><span data-stu-id="6288a-2940">Storage</span></span>

* <span data-ttu-id="6288a-2941">Option `--marker` für die Befehle `storage blob list`, `storage container list` und `storage share list` entfernt (3745)</span><span class="sxs-lookup"><span data-stu-id="6288a-2941">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="6288a-2942">Erstellung eines reinen HTTPS-Speicherkontos ermöglicht</span><span class="sxs-lookup"><span data-stu-id="6288a-2942">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="6288a-2943">Speichermetriken, Protokollierung und CORS-Befehle aktualisiert (3495)</span><span class="sxs-lookup"><span data-stu-id="6288a-2943">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="6288a-2944">Ausnahmemeldung von „cors add“ umformuliert (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="6288a-2944">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="6288a-2945">Generator im Probelaufmodus des Downloadbatchbefehls in eine Liste konvertiert (3592)</span><span class="sxs-lookup"><span data-stu-id="6288a-2945">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="6288a-2946">Problem bei Probelauf des Blobdownloadbatchs behoben (3640) (3592)</span><span class="sxs-lookup"><span data-stu-id="6288a-2946">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="6288a-2947">VM</span><span class="sxs-lookup"><span data-stu-id="6288a-2947">VM</span></span>

* <span data-ttu-id="6288a-2948">Unterstützung der NSG-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="6288a-2948">Support configuring nsg</span></span>
* <span data-ttu-id="6288a-2949">Fehler behoben, aufgrund dessen der DNS-Server nicht ordnungsgemäß konfiguriert wurde</span><span class="sxs-lookup"><span data-stu-id="6288a-2949">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="6288a-2950">Unterstützung verwalteter Dienstidentitäten</span><span class="sxs-lookup"><span data-stu-id="6288a-2950">Support managed service identities</span></span>
* <span data-ttu-id="6288a-2951">Problem behoben, aufgrund dessen `cmss create` mit einem vorhandenen Lastenausgleich `--backend-pool-name` benötigte</span><span class="sxs-lookup"><span data-stu-id="6288a-2951">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="6288a-2952">Festlegung, dass die LUN von mit `vm image create` erstellten Datenträgern mit 0 beginnt</span><span class="sxs-lookup"><span data-stu-id="6288a-2952">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="6288a-2953">10. Mai 2017</span><span class="sxs-lookup"><span data-stu-id="6288a-2953">May 10, 2017</span></span>

<span data-ttu-id="6288a-2954">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="6288a-2954">Version 2.0.6</span></span>

* <span data-ttu-id="6288a-2955">Umbenennen von „documentdb“ in „cosmosdb“</span><span class="sxs-lookup"><span data-stu-id="6288a-2955">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="6288a-2956">Hinzufügen von rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="6288a-2956">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="6288a-2957">Einbeziehen der Data Lake Analytics- und Data Lake Store-Module</span><span class="sxs-lookup"><span data-stu-id="6288a-2957">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="6288a-2958">Einbeziehen des Cognitive Services-Moduls</span><span class="sxs-lookup"><span data-stu-id="6288a-2958">Include Cognitive Services module</span></span>
* <span data-ttu-id="6288a-2959">Einbeziehen des Service Fabric-Moduls</span><span class="sxs-lookup"><span data-stu-id="6288a-2959">Include Service Fabric module</span></span>
* <span data-ttu-id="6288a-2960">Einbeziehen des interaktiven Moduls (Umbenennen von „az-shell“)</span><span class="sxs-lookup"><span data-stu-id="6288a-2960">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="6288a-2961">Hinzufügen von Unterstützung für CDN-Befehle</span><span class="sxs-lookup"><span data-stu-id="6288a-2961">Add support for CDN commands</span></span>
* <span data-ttu-id="6288a-2962">Entfernen des Containermoduls</span><span class="sxs-lookup"><span data-stu-id="6288a-2962">Remove Container module</span></span>
* <span data-ttu-id="6288a-2963">Hinzufügen von „az -v“ als Verknüpfung für „az --version“ ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="6288a-2963">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="6288a-2964">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="6288a-2964">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="6288a-2965">Core</span><span class="sxs-lookup"><span data-stu-id="6288a-2965">Core</span></span>

* <span data-ttu-id="6288a-2966">Core: Erfassen von Ausnahmen, die durch einen nicht registrierten Anbieter verursacht werden, und automatische Registrierung</span><span class="sxs-lookup"><span data-stu-id="6288a-2966">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="6288a-2967">Leistung: Dauerhaftes Speichern des ADAL-Tokencaches im Arbeitsspeicher bis zum Prozessende ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="6288a-2967">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="6288a-2968">Korrigieren der vom hexadezimalen Fingerabdruck -o tsv zurückgegebenen Bytes ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="6288a-2968">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="6288a-2969">Verbessern des Downloads des Schlüsseltresorzertifikats und der AAD-SP-Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="6288a-2969">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="6288a-2970">Hinzufügen des Python-Speicherorts zu „az –version“ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="6288a-2970">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="6288a-2971">Anmeldung: Unterstützung der Anmeldung, wenn keine Abonnements vorhanden sind ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="6288a-2971">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="6288a-2972">Core: Beheben eines Fehlers bei zweimaliger Verwendung eines Dienstprinzipals bei der Anmeldung ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="6288a-2972">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="6288a-2973">Core: Ermöglichen der Konfiguration des Dateipfads von „accessTokens.json“ über eine Umgebungsvariable ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="6288a-2973">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="6288a-2974">Core: Zulassen der Anwendung konfigurierter Standardwerte auf optionale Argumente ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="6288a-2974">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="6288a-2975">Core: Verbesserte Leistung</span><span class="sxs-lookup"><span data-stu-id="6288a-2975">core: Improved performance</span></span>
* <span data-ttu-id="6288a-2976">Core: Zertifikate von benutzerdefinierter Zertifizierungsstelle – Unterstützung für das Festlegen der REQUESTS_CA_BUNDLE-Umgebungsvariablen</span><span class="sxs-lookup"><span data-stu-id="6288a-2976">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="6288a-2977">Core: Cloudkonfiguration – Verwenden des Endpunkts „resource manager“, wenn Endpunkt „management“ nicht festgelegt ist</span><span class="sxs-lookup"><span data-stu-id="6288a-2977">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="6288a-2978">ACS</span><span class="sxs-lookup"><span data-stu-id="6288a-2978">ACS</span></span>

* <span data-ttu-id="6288a-2979">Korrigieren der Master- und Agentanzahl als ganze Zahl statt Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6288a-2979">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="6288a-2980">Verfügbarmachen von „az acs create --no-wait“ und „az acs wait“ für die asynchrone Erstellung</span><span class="sxs-lookup"><span data-stu-id="6288a-2980">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="6288a-2981">Verfügbarmachen von „az acs create --validate“ für Probelaufüberprüfungen</span><span class="sxs-lookup"><span data-stu-id="6288a-2981">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="6288a-2982">Entfernen von Windows-Profil vor PUT-Aufruf für Skalierungsbefehl ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="6288a-2982">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="6288a-2983">AppService</span><span class="sxs-lookup"><span data-stu-id="6288a-2983">AppService</span></span>

* <span data-ttu-id="6288a-2984">functionapp: Hinzufügen der vollständigen functionapp-Unterstützung, einschließlich Erstellen, Anzeigen, Auflisten, Löschen, Hostname, SSL usw.</span><span class="sxs-lookup"><span data-stu-id="6288a-2984">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="6288a-2985">Hinzufügen von Team Services (vsts) als Continuous Delivery-Option zu „appservice web source-control config“</span><span class="sxs-lookup"><span data-stu-id="6288a-2985">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="6288a-2986">Erstellen von „az webapp“ als Ersatz für „az appservice web“ (für Abwärtskompatibilität bleibt „az appservice web“ für 2 weitere Releases erhalten)</span><span class="sxs-lookup"><span data-stu-id="6288a-2986">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="6288a-2987">Verfügbarmachen von Argumenten zum Konfigurieren von Bereitstellung und Laufzeitstapeln beim Erstellen von Web-Apps</span><span class="sxs-lookup"><span data-stu-id="6288a-2987">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="6288a-2988">Verfügbarmachen von „webapp list-runtimes“</span><span class="sxs-lookup"><span data-stu-id="6288a-2988">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="6288a-2989">Unterstützen der Konfiguration von Verbindungszeichenfolgen ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="6288a-2989">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="6288a-2990">Unterstützen des Slottauschs mit Vorschau</span><span class="sxs-lookup"><span data-stu-id="6288a-2990">support slot swap with preview</span></span>
* <span data-ttu-id="6288a-2991">Beheben von Fehlern in appservice-Befehlen ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="6288a-2991">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="6288a-2992">Verwenden der Ressourcengruppe des App Service-Plans für Zertifizierungsvorgänge ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="6288a-2992">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="6288a-2993">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="6288a-2993">CosmosDB</span></span>

* <span data-ttu-id="6288a-2994">Umbenennen des documentdb-Moduls in cosmosdb</span><span class="sxs-lookup"><span data-stu-id="6288a-2994">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="6288a-2995">Zusätzliche Unterstützung für documentdb-APIs auf Datenebene: Datenbank- und Sammlungsverwaltung</span><span class="sxs-lookup"><span data-stu-id="6288a-2995">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="6288a-2996">Zusätzliche Unterstützung für das Aktivieren des automatischen Failovers für Datenbankkonten</span><span class="sxs-lookup"><span data-stu-id="6288a-2996">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="6288a-2997">Zusätzliche Unterstützung für die neue ConsistentPrefix-Konsistenzrichtlinie</span><span class="sxs-lookup"><span data-stu-id="6288a-2997">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="6288a-2998">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="6288a-2998">Data Lake Analytics</span></span>

* <span data-ttu-id="6288a-2999">Beheben eines Fehlers, bei dem das Filtern von Auftragslisten nach Ergebnis und Status einen Fehler auslöst</span><span class="sxs-lookup"><span data-stu-id="6288a-2999">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="6288a-3000">Hinzufügen von Unterstützung für den neuen Katalogelementtyp „Paket“</span><span class="sxs-lookup"><span data-stu-id="6288a-3000">Add support for new catalog item type: package.</span></span> <span data-ttu-id="6288a-3001">Zugriff über: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="6288a-3001">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="6288a-3002">Ermöglichen der Auflistung folgender Katalogelemente innerhalb einer Datenbank (keine Schemaspezifikation erforderlich):</span><span class="sxs-lookup"><span data-stu-id="6288a-3002">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="6288a-3003">Tabelle</span><span class="sxs-lookup"><span data-stu-id="6288a-3003">Table</span></span>
  * <span data-ttu-id="6288a-3004">Tabellenwertfunktion</span><span class="sxs-lookup"><span data-stu-id="6288a-3004">Table valued function</span></span>
  * <span data-ttu-id="6288a-3005">Sicht</span><span class="sxs-lookup"><span data-stu-id="6288a-3005">View</span></span>
  * <span data-ttu-id="6288a-3006">Tabellenstatistiken.</span><span class="sxs-lookup"><span data-stu-id="6288a-3006">Table Statistics.</span></span> <span data-ttu-id="6288a-3007">Können auch mit einem Schema, jedoch ohne Angabe eines Tabellennamens aufgelistet werden.</span><span class="sxs-lookup"><span data-stu-id="6288a-3007">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="6288a-3008">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="6288a-3008">Data Lake Store</span></span>

* <span data-ttu-id="6288a-3009">Aktualisieren der Version des zugrunde liegenden Dateisystem-SDK, wodurch eine bessere Unterstützung für die Verarbeitung von Drosselungsszenarien auf Serverseite gewährt wird</span><span class="sxs-lookup"><span data-stu-id="6288a-3009">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="6288a-3010">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="6288a-3010">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="6288a-3011">Fehlende Hilfe für Zugriffsanzeige</span><span class="sxs-lookup"><span data-stu-id="6288a-3011">missed help for access show.</span></span> <span data-ttu-id="6288a-3012">hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="6288a-3012">adding it.</span></span> <span data-ttu-id="6288a-3013">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="6288a-3013">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="6288a-3014">Suchen</span><span class="sxs-lookup"><span data-stu-id="6288a-3014">Find</span></span>

* <span data-ttu-id="6288a-3015">Verbessern von Suchergebnissen und Ermöglichen der Versionsverwaltung des Suchindex</span><span class="sxs-lookup"><span data-stu-id="6288a-3015">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="6288a-3016">KeyVault</span><span class="sxs-lookup"><span data-stu-id="6288a-3016">KeyVault</span></span>

* <span data-ttu-id="6288a-3017">BC:`az keyvault certificate download` Ändern von „-e“ von Zeichenfolge oder Binärdatentyp in PEM oder DER zur besseren Darstellung der Optionen</span><span class="sxs-lookup"><span data-stu-id="6288a-3017">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="6288a-3018">BC: Entfernen von „--expires“ und „--not-before“ aus `keyvault certificate create`, da diese Parameter nicht vom Dienst unterstützt werden</span><span class="sxs-lookup"><span data-stu-id="6288a-3018">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="6288a-3019">Hinzufügen des Parameters „--validity“ zu `keyvault certificate create`, um gezielt den Wert in „--policy“ zu überschreiben</span><span class="sxs-lookup"><span data-stu-id="6288a-3019">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="6288a-3020">Beheben des Problems in `keyvault certificate get-default-policy`, bei dem „expires“ und „not_before“ verfügbar gemacht wurden, „validity_in_months“ hingegen nicht</span><span class="sxs-lookup"><span data-stu-id="6288a-3020">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="6288a-3021">Keyvault-Korrektur für den Import von PEM und PFX ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="6288a-3021">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="6288a-3022">Labor</span><span class="sxs-lookup"><span data-stu-id="6288a-3022">Lab</span></span>

* <span data-ttu-id="6288a-3023">Hinzufügen der Befehle „create“, „show“, „delete“ und „list“ für die Laborumgebung</span><span class="sxs-lookup"><span data-stu-id="6288a-3023">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="6288a-3024">Hinzufügen der Befehle „show“ und „list“ zur Anzeige von ARM-Vorlagen im Labor</span><span class="sxs-lookup"><span data-stu-id="6288a-3024">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="6288a-3025">Hinzufügen des Kennzeichens „--environment“ in `az lab vm list`, um virtuelle Computer nach Umgebung im Labor zu filtern</span><span class="sxs-lookup"><span data-stu-id="6288a-3025">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="6288a-3026">Hinzufügen des benutzerfreundlichen Befehls `az lab formula export-artifacts` zum Exportieren des Artefaktgerüsts innerhalb der Formel eines Labors</span><span class="sxs-lookup"><span data-stu-id="6288a-3026">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="6288a-3027">Hinzufügen von Befehlen zum Verwalten von Geheimnissen in einem Labor</span><span class="sxs-lookup"><span data-stu-id="6288a-3027">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="6288a-3028">Überwachen</span><span class="sxs-lookup"><span data-stu-id="6288a-3028">Monitor</span></span>

* <span data-ttu-id="6288a-3029">Fehlerbehebung: Modellieren von `--actions` von `az alert-rules create` zum Verarbeiten von JSON-Zeichenfolgen ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="6288a-3029">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="6288a-3030">Programmfehlerbehebung: Beim Erstellen von Diagnoseeinstellungen werden Protokolle/Metriken aus Anzeigebefehlen nicht akzeptiert ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="6288a-3030">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="6288a-3031">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6288a-3031">Network</span></span>

* <span data-ttu-id="6288a-3032">Hinzufügen des `network watcher test-connectivity`-Befehls</span><span class="sxs-lookup"><span data-stu-id="6288a-3032">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="6288a-3033">Hinzufügen von Unterstützung für den `--filters`-Parameter für `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="6288a-3033">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="6288a-3034">Hinzufügen von Unterstützung für den Application Gateway-Verbindungsausgleich</span><span class="sxs-lookup"><span data-stu-id="6288a-3034">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="6288a-3035">Hinzufügen von Unterstützung für die Konfiguration von Application Gateway-WAF-Regelsätzen</span><span class="sxs-lookup"><span data-stu-id="6288a-3035">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="6288a-3036">Hinzufügen von Unterstützung für ExpressRoute-Routenfilter und -Regeln</span><span class="sxs-lookup"><span data-stu-id="6288a-3036">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="6288a-3037">Hinzufügen von Unterstützung für geografisches TrafficManager-Routing</span><span class="sxs-lookup"><span data-stu-id="6288a-3037">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="6288a-3038">Hinzufügen von Unterstützung für richtlinienbasierte Datenverkehrsselektoren für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="6288a-3038">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="6288a-3039">Hinzufügen von Unterstützung für IPSec-Richtlinien für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="6288a-3039">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="6288a-3040">Korrektur eines Fehlers bei `vpn-connection create` bei Verwendung der Parameter `--no-wait` oder `--validate`</span><span class="sxs-lookup"><span data-stu-id="6288a-3040">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="6288a-3041">Hinzufügen von Unterstützung für Aktiv/Aktiv-VNET-Gateways</span><span class="sxs-lookup"><span data-stu-id="6288a-3041">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="6288a-3042">Entfernen von NULL-Werten aus der Ausgabe von `network vpn-connection list/show`-Befehlen</span><span class="sxs-lookup"><span data-stu-id="6288a-3042">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="6288a-3043">BC: Korrektur eines Fehlers in der Ausgabe von `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="6288a-3043">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="6288a-3044">Korrektur eines Fehlers, bei dem das Argument „--key-length“ von „vpn-connection create“ nicht ordnungsgemäß analysiert wurde</span><span class="sxs-lookup"><span data-stu-id="6288a-3044">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="6288a-3045">Korrektur eines Fehlers in `dns zone import`, bei dem Datensätze nicht ordnungsgemäß importiert wurden</span><span class="sxs-lookup"><span data-stu-id="6288a-3045">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="6288a-3046">Korrektur eines Fehlers, bei dem `traffic-manager endpoint update` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="6288a-3046">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="6288a-3047">Hinzufügen von Network Watcher-Vorschaubefehlen</span><span class="sxs-lookup"><span data-stu-id="6288a-3047">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="6288a-3048">Profil</span><span class="sxs-lookup"><span data-stu-id="6288a-3048">Profile</span></span>

* <span data-ttu-id="6288a-3049">Unterstützung der Anmeldung, wenn keine Abonnements gefunden werden ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="6288a-3049">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="6288a-3050">Unterstützung für kurze Parameternamen in „az account set --subscription“ ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="6288a-3050">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="6288a-3051">Redis</span><span class="sxs-lookup"><span data-stu-id="6288a-3051">Redis</span></span>

* <span data-ttu-id="6288a-3052">Hinzufügen des Updatebefehls, durch den auch die Möglichkeit zum Skalieren für Redis Cache hinzugefügt wird</span><span class="sxs-lookup"><span data-stu-id="6288a-3052">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="6288a-3053">Verwerfen des Befehls „update-settings“</span><span class="sxs-lookup"><span data-stu-id="6288a-3053">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="6288a-3054">Resource</span><span class="sxs-lookup"><span data-stu-id="6288a-3054">Resource</span></span>

* <span data-ttu-id="6288a-3055">Hinzufügen der Befehle „managedapp“ und „managedapp definition“ ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="6288a-3055">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="6288a-3056">Unterstützung für die „provider operation“-Befehle ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="6288a-3056">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="6288a-3057">Unterstützung für die Erstellung generischer Ressourcen ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="6288a-3057">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="6288a-3058">Korrigieren der Ressourcenanalyse und der API-Versionssuche</span><span class="sxs-lookup"><span data-stu-id="6288a-3058">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="6288a-3059">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="6288a-3059">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="6288a-3060">Hinzufügen von Dokumenten für „az lock update“</span><span class="sxs-lookup"><span data-stu-id="6288a-3060">Add docs for az lock update.</span></span> <span data-ttu-id="6288a-3061">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="6288a-3061">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="6288a-3062">Beenden mit Fehler bei dem Versuch, Ressourcen für eine nicht vorhandene Gruppe aufzulisten</span><span class="sxs-lookup"><span data-stu-id="6288a-3062">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="6288a-3063">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="6288a-3063">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="6288a-3064">[Compute] Beheben von Problemen mit dem Update von VMSS- und VM-Verfügbarkeitsgruppen</span><span class="sxs-lookup"><span data-stu-id="6288a-3064">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="6288a-3065">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="6288a-3065">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="6288a-3066">Korrigieren des Erstellungs- und Löschvorgangs für Sperren, wenn „parent-resource-path“ auf „None“ festgelegt ist ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="6288a-3066">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="6288a-3067">Role</span><span class="sxs-lookup"><span data-stu-id="6288a-3067">Role</span></span>

* <span data-ttu-id="6288a-3068">create-for-rbac: Sicherstellen, dass das SP-Enddatum nicht das Ablaufdatum des Zertifikats überschreitet ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="6288a-3068">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="6288a-3069">RBAC: Hinzufügen vollständiger Unterstützung für „ad group“ ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="6288a-3069">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="6288a-3070">Rolle: Beheben von Probleme beim Rollendefinitionsupdate ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="6288a-3070">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="6288a-3071">create-for-rbac: Sicherstellen, dass das angegebene Benutzerkennwort übernommen wird</span><span class="sxs-lookup"><span data-stu-id="6288a-3071">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="6288a-3072">SQL</span><span class="sxs-lookup"><span data-stu-id="6288a-3072">SQL</span></span>

* <span data-ttu-id="6288a-3073">Hinzufügen der Befehle „az sql server list-usages“ und „az sql db list-usages“</span><span class="sxs-lookup"><span data-stu-id="6288a-3073">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="6288a-3074">SQL: Möglichkeit zur direkten Verbindung mit Ressourcenanbieter ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="6288a-3074">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="6288a-3075">Storage</span><span class="sxs-lookup"><span data-stu-id="6288a-3075">Storage</span></span>

* <span data-ttu-id="6288a-3076">Festlegen des Ressourcengruppenstandorts als Standardstandort für `storage account create`</span><span class="sxs-lookup"><span data-stu-id="6288a-3076">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="6288a-3077">Hinzufügen von Unterstützung für das inkrementelle Kopieren von Blobs</span><span class="sxs-lookup"><span data-stu-id="6288a-3077">Add support for incremental blob copy</span></span>
* <span data-ttu-id="6288a-3078">Hinzufügen von Unterstützung für den Upload umfangreicher Blockblobs</span><span class="sxs-lookup"><span data-stu-id="6288a-3078">Add support for large block blob upload</span></span>
* <span data-ttu-id="6288a-3079">Ändern der Blockgröße auf 100 MB, wenn die hochzuladende Datei größer als 200 GB ist</span><span class="sxs-lookup"><span data-stu-id="6288a-3079">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="6288a-3080">VM</span><span class="sxs-lookup"><span data-stu-id="6288a-3080">VM</span></span>

* <span data-ttu-id="6288a-3081">avail-set: Festlegen der UD- und FD-Domänenanzahl als optional</span><span class="sxs-lookup"><span data-stu-id="6288a-3081">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="6288a-3082">Hinweis: VM-Befehle in unabhängigen Clouds: Vermeiden Sie Features im Zusammenhang mit verwalteten Datenträgern, einschließlich der folgenden:</span><span class="sxs-lookup"><span data-stu-id="6288a-3082">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="6288a-3083">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="6288a-3083">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="6288a-3084">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="6288a-3084">az vm/vmss disk</span></span>
  3. <span data-ttu-id="6288a-3085">Verwenden Sie in „az vm/vmss create“ den Befehl „—use-unmanaged-disk“, um verwaltete Datenträger zu vermeiden. Andere Befehle sollten funktionieren.</span><span class="sxs-lookup"><span data-stu-id="6288a-3085">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="6288a-3086">vm/vmss: Verbessern des Warnungstexts beim Generieren von SSH-Schlüsselpaaren</span><span class="sxs-lookup"><span data-stu-id="6288a-3086">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="6288a-3087">vm/vmss: Unterstützen der Erstellung über ein Marketplace-Image, für das Planinformationen erforderlich sind ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="6288a-3087">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="6288a-3088">3\. April 2017</span><span class="sxs-lookup"><span data-stu-id="6288a-3088">April 3, 2017</span></span>

<span data-ttu-id="6288a-3089">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="6288a-3089">Version 2.0.2</span></span>

<span data-ttu-id="6288a-3090">In dieser Version wurden die Komponenten ACR, Batch, KeyVault und SQL eingeführt.</span><span class="sxs-lookup"><span data-stu-id="6288a-3090">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="6288a-3091">Core</span><span class="sxs-lookup"><span data-stu-id="6288a-3091">Core</span></span>

* <span data-ttu-id="6288a-3092">Hinzufügen der Module „acr“, „lab“, „monitor“ und „find“ zur Standardliste</span><span class="sxs-lookup"><span data-stu-id="6288a-3092">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="6288a-3093">Anmeldung: Überspringen des fehlerhaften Mandanten ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="6288a-3093">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="6288a-3094">Anmeldung: Festlegen des Standardabonnements auf ein Abonnement mit dem Status „Enabled“ ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="6288a-3094">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="6288a-3095">Hinzufügen von wait-Befehlen und Unterstützung von „--no-wait“ für mehr Befehle ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="6288a-3095">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="6288a-3096">Core: Unterstützen der Anmeldung per Dienstprinzipal mit einem Zertifikat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="6288a-3096">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="6288a-3097">Hinzufügen der Meldung zu fehlenden Vorlagenparametern</span><span class="sxs-lookup"><span data-stu-id="6288a-3097">Add prompting for missing template parameters.</span></span> <span data-ttu-id="6288a-3098">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="6288a-3098">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="6288a-3099">Unterstützen des Festlegens von Standardwerten für häufig verwendete Argumente, z.B. Standardressourcengruppe, Standardweb und Standard-VM</span><span class="sxs-lookup"><span data-stu-id="6288a-3099">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="6288a-3100">Unterstützen der Anmeldung an einem bestimmten Mandanten</span><span class="sxs-lookup"><span data-stu-id="6288a-3100">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="6288a-3101">ACS</span><span class="sxs-lookup"><span data-stu-id="6288a-3101">ACS</span></span>

* <span data-ttu-id="6288a-3102">[ACS] Hinzufügen von Unterstützung für die Konfiguration eines ACS-Standardclusters ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="6288a-3102">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="6288a-3103">Hinzufügen von Unterstützung der Aufforderung zur Kennworteingabe für SSH-Schlüssel</span><span class="sxs-lookup"><span data-stu-id="6288a-3103">Add support for ssh key password prompting.</span></span> <span data-ttu-id="6288a-3104">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="6288a-3104">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="6288a-3105">Hinzufügen von Unterstützung für Windows-Cluster</span><span class="sxs-lookup"><span data-stu-id="6288a-3105">Add support for windows clusters.</span></span> <span data-ttu-id="6288a-3106">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="6288a-3106">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="6288a-3107">Wechseln von der Rolle „Besitzer“ zur Rolle „Mitwirkender“</span><span class="sxs-lookup"><span data-stu-id="6288a-3107">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="6288a-3108">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="6288a-3108">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="6288a-3109">AppService</span><span class="sxs-lookup"><span data-stu-id="6288a-3109">AppService</span></span>

* <span data-ttu-id="6288a-3110">appservice: Unterstützung für das Abrufen der externen IP-Adresse für DNS A-Einträge ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="6288a-3110">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="6288a-3111">appservice: Unterstützung der Bindung von Platzhalterzertifikaten ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="6288a-3111">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="6288a-3112">appservice: Unterstützung von Veröffentlichungsprofilen für Listen ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="6288a-3112">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="6288a-3113">AppService: Auslösen der Synchronisierung der Quellcodeverwaltung nach der Konfiguration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="6288a-3113">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="6288a-3114">DataLake</span><span class="sxs-lookup"><span data-stu-id="6288a-3114">DataLake</span></span>

* <span data-ttu-id="6288a-3115">Erste Version des Data Lake Analytics-Moduls</span><span class="sxs-lookup"><span data-stu-id="6288a-3115">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="6288a-3116">Erste Version des Data Lake Store-Moduls</span><span class="sxs-lookup"><span data-stu-id="6288a-3116">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="6288a-3117">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="6288a-3117">DocuemntDB</span></span>

* <span data-ttu-id="6288a-3118">DocumentDB: Hinzufügen von Unterstützung für das Auflisten von Verbindungszeichenfolgen ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="6288a-3118">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="6288a-3119">VM</span><span class="sxs-lookup"><span data-stu-id="6288a-3119">VM</span></span>

* <span data-ttu-id="6288a-3120">[Compute] Hinzufügen von AppGateway-Unterstützung für Erstellung von VM-Skalierungsgruppen ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="6288a-3120">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="6288a-3121">[VM/VMSS] Verbesserte Unterstützung für die Datenträgerzwischenspeicherung ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="6288a-3121">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="6288a-3122">VM/VMSS: Einbinden der vom Portal verwendeten Logik zur Überprüfung von Anmeldeinformationen ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="6288a-3122">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="6288a-3123">Hinzufügen von wait-Befehlen und Unterstützung für „--no-wait“ ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="6288a-3123">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="6288a-3124">VM-Skalierungsgruppe: Unterstützung von „\*“ zum Auflisten der übergreifenden Instanzansicht für VMs ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="6288a-3124">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="6288a-3125">Hinzufügen – Geheimnisse für virtuellen Computer und VM-Skalierungsgruppe ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="6288a-3125">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="6288a-3126">Zulassen der VM-Erstellung mit spezialisierter VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="6288a-3126">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="6288a-3127">27. Februar 2017</span><span class="sxs-lookup"><span data-stu-id="6288a-3127">February 27, 2017</span></span>

<span data-ttu-id="6288a-3128">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="6288a-3128">Version 2.0.0</span></span>

<span data-ttu-id="6288a-3129">Diese Version der Azure CLI 2.0 ist die erste „allgemein verfügbare“ Version. Die allgemeine Verfügbarkeit gilt für die folgenden Befehlsmodule:</span><span class="sxs-lookup"><span data-stu-id="6288a-3129">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="6288a-3130">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="6288a-3130">Container Service (acs)</span></span>
- <span data-ttu-id="6288a-3131">Compute (einschließlich Resource Manager, VM, VM-Skalierungsgruppen, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="6288a-3131">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="6288a-3132">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="6288a-3132">Networking</span></span>
- <span data-ttu-id="6288a-3133">Storage</span><span class="sxs-lookup"><span data-stu-id="6288a-3133">Storage</span></span>

<span data-ttu-id="6288a-3134">Diese Befehlsmodule können in der Produktion verwendet werden und verfügen über Unterstützung durch eine Standard-SLA von Microsoft. Sie können Anfragen zu Problemen direkt beim Microsoft-Support oder in der [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/) öffnen. Sie haben die Möglichkeit, Fragen in [StackOverflow mit dem Tag „azure-cli“](http://stackoverflow.com/questions/tagged/azure-cli) zu stellen oder sich unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) an das Produktteam zu wenden. Außerdem können Sie über die Befehlszeile mit dem Befehl `az feedback` Feedback senden.</span><span class="sxs-lookup"><span data-stu-id="6288a-3134">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="6288a-3135">Die Befehle in diesen Modulen sind stabil, und es ist nicht zu erwarten, dass sich die Syntax in den anstehenden Veröffentlichungen dieser Version der Azure CLI ändern.</span><span class="sxs-lookup"><span data-stu-id="6288a-3135">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="6288a-3136">Verwenden Sie zum Überprüfen der Version der CLI den Befehl `az --version`. In der Ausgabe werden die Version der CLI selbst (für diese Veröffentlichung 2.0.0), die einzelnen Befehlsmodule und die von Ihnen genutzten Versionen von Python und GCC aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="6288a-3136">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="6288a-3137">Einige Befehlsmodule verfügen über das Postfix „b*n*“ oder „rc*n*“. Diese Befehlsmodule befinden sich noch in der Vorschauphase und werden später die allgemeine Verfügbarkeit erlangen.</span><span class="sxs-lookup"><span data-stu-id="6288a-3137">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="6288a-3138">Außerdem werden jeden Abend Vorschaubuilds der CLI bereitgestellt. Informationen hierzu finden Sie in der [Anleitung zum Abrufen der abendlichen Builds](https://github.com/Azure/azure-cli#nightly-builds) und im Abschnitt zum [Setup für Entwickler und Beitragen von Code](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="6288a-3138">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="6288a-3139">Sie können für die abendlichen Vorschaubuilds wie folgt Probleme melden:</span><span class="sxs-lookup"><span data-stu-id="6288a-3139">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="6288a-3140">Über die [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="6288a-3140">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="6288a-3141">Per Kontaktaufnahme mit dem Produktteam unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="6288a-3141">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="6288a-3142">Senden von Feedback über die Befehlszeile mit dem Befehl `az feedback`</span><span class="sxs-lookup"><span data-stu-id="6288a-3142">Provide feedback from the command line with the `az feedback` command</span></span>


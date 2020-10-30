---
title: Versionshinweise für die Azure CLI
description: Enthält Informationen zu den aktuellen Updates der Azure CLI.
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 10/27/2020
ms.topic: article
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: 4e1f03268ccd001d6fe371b1ecdecb869791b198
ms.sourcegitcommit: 1187fb75b68426c46e84b3f294c509ee7b7da9be
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 10/27/2020
ms.locfileid: "92687131"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="018bf-103">Versionshinweise für die Azure CLI</span><span class="sxs-lookup"><span data-stu-id="018bf-103">Azure CLI release notes</span></span>

# <a name="current-release-notes"></a>[<span data-ttu-id="018bf-104">Aktuelle Versionshinweise</span><span class="sxs-lookup"><span data-stu-id="018bf-104">Current release notes</span></span>](#tab/azure-cli)

## <a name="october-27-2020"></a><span data-ttu-id="018bf-105">27. Oktober 2020</span><span class="sxs-lookup"><span data-stu-id="018bf-105">October 27, 2020</span></span>

<span data-ttu-id="018bf-106">Version 2.14.0</span><span class="sxs-lookup"><span data-stu-id="018bf-106">Version 2.14.0</span></span>

### <a name="aks"></a><span data-ttu-id="018bf-107">AKS</span><span class="sxs-lookup"><span data-stu-id="018bf-107">AKS</span></span>

* <span data-ttu-id="018bf-108">PPG-Unterstützung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-108">Add PPG support</span></span>
* <span data-ttu-id="018bf-109">Maximales Timeout für den Lastenausgleich auf 100 Minuten aktualisiert</span><span class="sxs-lookup"><span data-stu-id="018bf-109">Update max standard load balancer timeout to 100 minutes</span></span>

### <a name="apim"></a><span data-ttu-id="018bf-110">APIM</span><span class="sxs-lookup"><span data-stu-id="018bf-110">APIM</span></span>

* <span data-ttu-id="018bf-111">Problem beim Erstellen der Tarifinstanz „Consumption“ behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-111">Fix issue with creating consumption tier instance</span></span>

### <a name="app-config"></a><span data-ttu-id="018bf-112">App-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="018bf-112">App Config</span></span>

* <span data-ttu-id="018bf-113">Abfrage von Schlüsselwerten anhand von kommagetrennten Bezeichnungen korrigiert</span><span class="sxs-lookup"><span data-stu-id="018bf-113">Fix querying key-values by comma separated labels</span></span>

### <a name="app-service"></a><span data-ttu-id="018bf-114">App Service</span><span class="sxs-lookup"><span data-stu-id="018bf-114">App Service</span></span>

* <span data-ttu-id="018bf-115">Fehlerbehebung: Fehler bei „az webapp up“, wenn der Benutzer nicht über Schreibberechtigungen für das übergeordnete Verzeichnis des Projekts verfügt</span><span class="sxs-lookup"><span data-stu-id="018bf-115">Bugfix: az webapp up fails when user doesn't have write permissions to project's parent directory</span></span>
* <span data-ttu-id="018bf-116">Fehlerbehebung Nr. 13777: Fehlerbehebung zum Entfernen von Escapezeichen aus XML</span><span class="sxs-lookup"><span data-stu-id="018bf-116">Fix #13777: Fix to remove escape chars from XML</span></span>
* <span data-ttu-id="018bf-117">Fehlerbehebung Nr. 15441: Fehler „AttributeError“ bei „az webapp create-remote-connection“: Das Objekt „Thread“ besitzt kein Attribut vom Typ „isAlive“.</span><span class="sxs-lookup"><span data-stu-id="018bf-117">Fix #15441: az webapp create-remote-connection fails with AttributeError: 'Thread' object has no attribute 'isAlive'</span></span>
* <span data-ttu-id="018bf-118">[BREAKING CHANGE] az webapp up: Optionale Parameter hinzugefügt (Betriebssystem und Runtime) und Runtimes aktualisiert</span><span class="sxs-lookup"><span data-stu-id="018bf-118">[BREAKING CHANGE] az webapp up: add optional params (os & runtime) and updated runtimes</span></span>

### <a name="arm"></a><span data-ttu-id="018bf-119">ARM</span><span class="sxs-lookup"><span data-stu-id="018bf-119">ARM</span></span>

* <span data-ttu-id="018bf-120">Was-wäre-wenn-Befehle für Vorlagenbereitstellung nun allgemein verfügbar</span><span class="sxs-lookup"><span data-stu-id="018bf-120">Make template deployment What-If commands GA</span></span>
* <span data-ttu-id="018bf-121">[BREAKING CHANGE] Benutzerbestätigung für „az ts create“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-121">[BREAKING CHANGE] Add user confirmation for az ts create</span></span>
* <span data-ttu-id="018bf-122">Zurückgegebene Daten beim Markieren mehrerer Ressourcen korrigiert</span><span class="sxs-lookup"><span data-stu-id="018bf-122">Fix the returned data when tagging multiple resources</span></span>

### <a name="backup"></a><span data-ttu-id="018bf-123">Backup</span><span class="sxs-lookup"><span data-stu-id="018bf-123">Backup</span></span>

* <span data-ttu-id="018bf-124">`az backup policy create`: Unterstützung für die Erstellung von IaaSVM-Sicherungsrichtlinien über die CLI hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-124">`az backup policy create`: Add support for IaaSVM backup policy creation from CLI</span></span>
* <span data-ttu-id="018bf-125">Grenzwert für den VM-Schutz von 100 auf 1.000 erhöht</span><span class="sxs-lookup"><span data-stu-id="018bf-125">Increasing VM protection limit from 100 to 1000</span></span>

### <a name="compute"></a><span data-ttu-id="018bf-126">Compute</span><span class="sxs-lookup"><span data-stu-id="018bf-126">Compute</span></span>

* <span data-ttu-id="018bf-127">sig image-definition create: „--features“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-127">sig image-definition create: add --features</span></span>
* <span data-ttu-id="018bf-128">Neue API-Version von gallery_images 2020-09-30</span><span class="sxs-lookup"><span data-stu-id="018bf-128">New API version of gallery_images 2020-09-30</span></span>
* <span data-ttu-id="018bf-129">`az vm update / az sig image-version update`: Unterstützung der Aktualisierung der VM-/Imageversion (auch bei Verwendung eines mandantenübergreifenden Images)</span><span class="sxs-lookup"><span data-stu-id="018bf-129">`az vm update / az sig image-version update`: Support update vm/image-version even it uses a cross tenant image</span></span>
* <span data-ttu-id="018bf-130">Überprüfung von VM-Host-SKUs entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-130">Remove validation of vm host SKUs</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="018bf-131">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="018bf-131">Cosmos DB</span></span>

* <span data-ttu-id="018bf-132">`az cosmosdb create/update`: Fehlermeldung für falsche Eingabe für „--locations“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="018bf-132">`az cosmosdb create/update`: Improve error message from incorrect --locations input</span></span>
* <span data-ttu-id="018bf-133">`az cosmosdb sql container create/update`: Parameter „--analytical-storage-ttl“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-133">`az cosmosdb sql container create/update`: Add --analytical-storage-ttl parameter</span></span>

### <a name="hdinsight"></a><span data-ttu-id="018bf-134">HDInsight</span><span class="sxs-lookup"><span data-stu-id="018bf-134">HDInsight</span></span>

* <span data-ttu-id="018bf-135">[BREAKING CHANGE] az hdinsight create: Zwei Parameter entfernt: --public-network-access-type und --outbound-public-network-access-type</span><span class="sxs-lookup"><span data-stu-id="018bf-135">[BREAKING CHANGE] az hdinsight create: remove two parameters: --public-network-access-type and  --outbound-public-network-access-type</span></span>

### <a name="iot-central"></a><span data-ttu-id="018bf-136">IoT Central</span><span class="sxs-lookup"><span data-stu-id="018bf-136">IoT Central</span></span>

* <span data-ttu-id="018bf-137">Vorschauwarnung entfernt, da die Version bereits allgemein verfügbar ist</span><span class="sxs-lookup"><span data-stu-id="018bf-137">Remove preview warning since it is already GAed</span></span>

### <a name="key-vault"></a><span data-ttu-id="018bf-138">Key Vault</span><span class="sxs-lookup"><span data-stu-id="018bf-138">Key Vault</span></span>

* <span data-ttu-id="018bf-139">`--enable-soft-delete false` beim Erstellen oder Aktualisieren von Tresoren als ungültig erklärt</span><span class="sxs-lookup"><span data-stu-id="018bf-139">Invalidate `--enable-soft-delete false` while creating or updating vaults</span></span>
* <span data-ttu-id="018bf-140">`--bypass` und `--default-action` funktionieren nun gemeinsam mit Netzwerk-ACL-Parametern bei der Erstellung von Tresoren</span><span class="sxs-lookup"><span data-stu-id="018bf-140">Make `--bypass` and `--default-action` work together with network acl parameters while creating vaults</span></span>

### <a name="misc"></a><span data-ttu-id="018bf-141">Verschiedenes:</span><span class="sxs-lookup"><span data-stu-id="018bf-141">Misc.</span></span>

* <span data-ttu-id="018bf-142">„bash-completion“ zu Dockerfile hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-142">Add bash-completion to Dockerfile</span></span>

### <a name="rdbms"></a><span data-ttu-id="018bf-143">RDBMS</span><span class="sxs-lookup"><span data-stu-id="018bf-143">RDBMS</span></span>

* <span data-ttu-id="018bf-144">Befehl „List-SKUS“, Tabellentransformer, lokaler Kontext für Postgres, MySQL, MariaDB (Einzelserver) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-144">Add List-SKUS Command, Table Transformers, Local Context for Postgres, MySQL, Mariadb Single Server</span></span>
* <span data-ttu-id="018bf-145">[BREAKING CHANGE] Aktualisierungen von Parameternamen.</span><span class="sxs-lookup"><span data-stu-id="018bf-145">[BREAKING CHANGE] Parameter name updates.</span></span> <span data-ttu-id="018bf-146">Verbesserungen der Verwaltungsebene für MySQL und PostgreSQL</span><span class="sxs-lookup"><span data-stu-id="018bf-146">Improvements to Management Plane for MySQL and PostgreSQL</span></span>
* <span data-ttu-id="018bf-147">`az postgres|mariadb|mysql server create`: Erstellungsumgebung für Postgres, MySQL und MariaDB aktualisiert: Neue Felder in der Ausgabe, neue Werte für Parameter `--public` im create-Befehl eingeführt (all,<IP>,<IPRange>,0.0.0.0)</span><span class="sxs-lookup"><span data-stu-id="018bf-147">`az postgres|mariadb|mysql server create` : Update create experience for Postgres, MySQL and MariaDB - new fields in the output , Introduce new values for `--public` parameter in create command (all,<IP>,<IPRange>,0.0.0.0)</span></span>

### <a name="signalr"></a><span data-ttu-id="018bf-148">SignalR</span><span class="sxs-lookup"><span data-stu-id="018bf-148">SignalR</span></span>

* <span data-ttu-id="018bf-149">`az signalr create`: Neue Option `--enable-messaging-logs` hinzugefügt, um zu steuern, ob der Dienst Messagingprotokolle generiert</span><span class="sxs-lookup"><span data-stu-id="018bf-149">`az signalr create`: Add new option `--enable-messaging-logs` for controling service generate messaging logs or not</span></span>
* <span data-ttu-id="018bf-150">`az signalr update`: Neue Option `--enable-messaging-logs` hinzugefügt, um zu steuern, ob der Dienst Messagingprotokolle generiert</span><span class="sxs-lookup"><span data-stu-id="018bf-150">`az signalr update`: Add new option `--enable-messaging-logs` for controling service generate messaging logs or not</span></span>

### <a name="sql"></a><span data-ttu-id="018bf-151">SQL</span><span class="sxs-lookup"><span data-stu-id="018bf-151">SQL</span></span>

* <span data-ttu-id="018bf-152">[BREAKING CHANGE] Antwort für den Parameternamen der Sicherungsspeicherredundanz und Wert für MI korrigiert</span><span class="sxs-lookup"><span data-stu-id="018bf-152">[BREAKING CHANGE] Fix response for backup storage redundancy param name and value for MI</span></span>
* <span data-ttu-id="018bf-153">`az sql db audit-policy show`: Erweitert, um die Überwachungsrichtlinie der Datenbank (einschließlich LA- und EH-Daten) anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="018bf-153">`az sql db audit-policy show`: extend to show database's audit policy including LA and EH data</span></span>
* <span data-ttu-id="018bf-154">`az sql db audit-policy update`: Erweitert, um das LA- und EH-Update zusammen mit der Überwachungsrichtlinie der Datenbank zuzulassen</span><span class="sxs-lookup"><span data-stu-id="018bf-154">`az sql db audit-policy update`: extend to allow LA and EH update along with database's audit policy</span></span>
* <span data-ttu-id="018bf-155">`az sql db audit-policy wait`: CLI im Wartezustand platziert, bis eine Bedingung der Überwachungsrichtlinie der Datenbank erfüllt ist</span><span class="sxs-lookup"><span data-stu-id="018bf-155">`az sql db audit-policy wait`: place the CLI in a waiting state until a condition of the database's audit policy is met.</span></span>
* <span data-ttu-id="018bf-156">`az sql server audit-policy show`: Erweitert, um die Überwachungsrichtlinie des Servers (einschließlich LA- und EH-Daten) anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="018bf-156">`az sql server audit-policy show`: extend to show servers's audit policy including LA and EH data</span></span>
* <span data-ttu-id="018bf-157">`az sql server audit-policy update`: Erweitert, um das LA- und EH-Update zusammen mit der Überwachungsrichtlinie des Servers zuzulassen</span><span class="sxs-lookup"><span data-stu-id="018bf-157">`az sql server audit-policy update`: extend to allow LA and EH update along with server's audit policy</span></span>
* <span data-ttu-id="018bf-158">`az sql server audit-policy wait`: CLI im Wartezustand platziert, bis eine Bedingung der Überwachungsrichtlinie des Servers erfüllt ist</span><span class="sxs-lookup"><span data-stu-id="018bf-158">`az sql server audit-policy wait`: place the CLI in a waiting state until a condition of the server's audit policy is met.</span></span>
* <span data-ttu-id="018bf-159">Reine AAD-Unterstützung für SQL Managed Instance und Server hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-159">Add AAD-only Support for SQL Managed Instances and Servers</span></span>
* <span data-ttu-id="018bf-160">`az sql db replica create`: Argument „--partner-database“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-160">`az sql db replica create`: Add --partner-database argument</span></span>

### <a name="storage"></a><span data-ttu-id="018bf-161">Storage</span><span class="sxs-lookup"><span data-stu-id="018bf-161">Storage</span></span>

* <span data-ttu-id="018bf-162">Fehlerbehebung Nr. 15111: Fehler bei `az storage logging update` ohne optionales Argument</span><span class="sxs-lookup"><span data-stu-id="018bf-162">Fix #15111: `az storage logging update` fails without optional argument</span></span>
* <span data-ttu-id="018bf-163">Problem behoben, das auftrat, wenn der Befehl „set-tier“ mit Dienstprinzipalanmeldung verwendet wurde</span><span class="sxs-lookup"><span data-stu-id="018bf-163">Fix bug when using set-tier command with service principal login</span></span>
* <span data-ttu-id="018bf-164">Version für Data Lake für Dateien auf 2020-02-10 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="018bf-164">Upgrade version for file datalake to 2020-02-10</span></span>
* <span data-ttu-id="018bf-165">`az storage queue list`: Unterstützung für Track2</span><span class="sxs-lookup"><span data-stu-id="018bf-165">`az storage queue list`: Track2 supported</span></span>
* <span data-ttu-id="018bf-166">`az storage fs access`: Unterstützung der rekursiven Verwaltung von ACLs</span><span class="sxs-lookup"><span data-stu-id="018bf-166">`az storage fs access`: Support managing ACLs recursively</span></span>

### <a name="synapse"></a><span data-ttu-id="018bf-167">Synapse</span><span class="sxs-lookup"><span data-stu-id="018bf-167">Synapse</span></span>

* <span data-ttu-id="018bf-168">Cmdlets für Pipeline, verknüpften Dienst, Trigger, Notebook, Datenfluss und Dataset hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-168">Add pipeline, linked service, trigger, notebook, data flow and dataset related cmdlets</span></span>

## <a name="october-13-2020"></a><span data-ttu-id="018bf-169">13. Oktober 2020</span><span class="sxs-lookup"><span data-stu-id="018bf-169">October 13, 2020</span></span>

<span data-ttu-id="018bf-170">Version 2.13.0</span><span class="sxs-lookup"><span data-stu-id="018bf-170">Version 2.13.0</span></span>

### <a name="acr"></a><span data-ttu-id="018bf-171">ACR</span><span class="sxs-lookup"><span data-stu-id="018bf-171">ACR</span></span>

* <span data-ttu-id="018bf-172">`az acr helm`: URL zur eingestellten Unterstützung aktualisiert</span><span class="sxs-lookup"><span data-stu-id="018bf-172">`az acr helm`: Update deprecation url</span></span>
* <span data-ttu-id="018bf-173">logtemplate- und systemtask-Änderungen für ACR Tasks hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-173">Add logtemplate and systemtask changes for ACR Tasks</span></span>

### <a name="aks"></a><span data-ttu-id="018bf-174">AKS</span><span class="sxs-lookup"><span data-stu-id="018bf-174">AKS</span></span>

* <span data-ttu-id="018bf-175">Unterstützung von „virtual-node“ bei „aks create“: `az aks create --enable-addons virtual-node`</span><span class="sxs-lookup"><span data-stu-id="018bf-175">Support virtual-node with aks create: `az aks create --enable-addons virtual-node`</span></span>
* <span data-ttu-id="018bf-176">Option nur für Knotenimages für CLI hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-176">Add node image only option for CLI</span></span>
* <span data-ttu-id="018bf-177">Es wird erwartet, dass das Add-On „kube-dashboard“ standardmäßig deaktiviert wird.</span><span class="sxs-lookup"><span data-stu-id="018bf-177">Expect kube-dashboard addon be disabled by default</span></span>
* <span data-ttu-id="018bf-178">`az aks create/update`: LicenseType-Unterstützung für Windows hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-178">`az aks create/update`: Add LicenseType support for Windows</span></span>
* <span data-ttu-id="018bf-179">Unterstützung für das Hinzufügen eines Spot-Knotenpools</span><span class="sxs-lookup"><span data-stu-id="018bf-179">Support add Spot node pool</span></span>
* <span data-ttu-id="018bf-180">Beachten der in der Azure CLI definierten Add-On-Namen</span><span class="sxs-lookup"><span data-stu-id="018bf-180">Honor addon names defined in Azure CLI</span></span>

### <a name="ams"></a><span data-ttu-id="018bf-181">AMS</span><span class="sxs-lookup"><span data-stu-id="018bf-181">AMS</span></span>

* <span data-ttu-id="018bf-182">Fehlerbehebung Nr. 14687: Gemischte Ressourcengruppen- und Kontonamen im Befehl „az ams streaming-endpoint show“</span><span class="sxs-lookup"><span data-stu-id="018bf-182">Fix #14687: Mixed resource group and account name in command "az ams streaming-endpoint show"</span></span>

### <a name="app-config"></a><span data-ttu-id="018bf-183">App-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="018bf-183">App Config</span></span>

* <span data-ttu-id="018bf-184">Testfehler behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-184">Fix test bug</span></span>
* <span data-ttu-id="018bf-185">Unterstützung der AAD-Authentifizierung für Datenvorgänge</span><span class="sxs-lookup"><span data-stu-id="018bf-185">Support AAD auth for data operations</span></span>

### <a name="app-service"></a><span data-ttu-id="018bf-186">App Service</span><span class="sxs-lookup"><span data-stu-id="018bf-186">App Service</span></span>

* <span data-ttu-id="018bf-187">`az functionapp deployment source config-zip`: Es wurde ein Problem behoben, das dazu führte, dass „config-zip“ bei Erfolg unter Linux ggf. eine Ausnahme auslöste.</span><span class="sxs-lookup"><span data-stu-id="018bf-187">`az functionapp deployment source config-zip`: Fixed an issue where config-zip could throw an exception on success on linux consumption</span></span>
* <span data-ttu-id="018bf-188">Fehlerbehebung: Bessere Fehlermeldungen für Befehle vom Typ „webapp“</span><span class="sxs-lookup"><span data-stu-id="018bf-188">Bugfix: Better error messages for webapp commands</span></span>
* <span data-ttu-id="018bf-189">`az appservice domain create, show-terms`: Option zum Erstellen einer App Service-Domäne hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-189">`az appservice domain create, show-terms`: Add ability to create app service domain</span></span>
* <span data-ttu-id="018bf-190">`az functionapp create`: Vorschauflag aus Java 11 beim Erstellen einer neuen Funktions-App entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-190">`az functionapp create`: Removed the preview flag from Java 11 when creating a new function app</span></span>
* <span data-ttu-id="018bf-191">[BREAKING CHANGE:] az webapp create, az webapp up – verfügbare webapp-Runtimes aktualisiert</span><span class="sxs-lookup"><span data-stu-id="018bf-191">[BREAKING CHANGE] az webapp create, az webapp up - Update available webapp runtimes</span></span>

### <a name="arm"></a><span data-ttu-id="018bf-192">ARM</span><span class="sxs-lookup"><span data-stu-id="018bf-192">ARM</span></span>

* <span data-ttu-id="018bf-193">`az ts`: Neue Befehle für Vorlagenspezifikationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-193">`az ts`: Add new commands for template specs</span></span>
* <span data-ttu-id="018bf-194">`az deployment` : Unterstützung für „--template-spec -s“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-194">`az deployment` : Add support for --template-spec -s</span></span>

### <a name="compute"></a><span data-ttu-id="018bf-195">Compute</span><span class="sxs-lookup"><span data-stu-id="018bf-195">Compute</span></span>

* <span data-ttu-id="018bf-196">Beschränkung der FD-Anzahl bei der Hostgruppenerstellung korrigiert</span><span class="sxs-lookup"><span data-stu-id="018bf-196">Fix host group creation FD count limitation</span></span>
* <span data-ttu-id="018bf-197">Neuer Befehl hinzugefügt, um das Upgrade von Erweiterungen für VMSS zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="018bf-197">Add new command to support upgrading extensions for VMSS</span></span>
* <span data-ttu-id="018bf-198">Problem des fehlenden Imageverweises behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-198">Fix the image reference is missing issue</span></span>

### <a name="hdinsight"></a><span data-ttu-id="018bf-199">HDInsight</span><span class="sxs-lookup"><span data-stu-id="018bf-199">HDInsight</span></span>

* <span data-ttu-id="018bf-200">`az hdinsight create`: Informationen zur Einstellung für Argument „--public-networrk-access-type“ und „--outbound-public-network-access-type“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-200">`az hdinsight create`: add deprecate information for argument --public-networrk-access-type and --outbound-public-network-access-type</span></span>
* <span data-ttu-id="018bf-201">`az hdinsight create`: Informationen zur Einstellung für Argument `--public-networrk-access-type` und `--outbound-public-network-access-type` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-201">`az hdinsight create`: add deprecate information for argument `--public-networrk-access-type` and `--outbound-public-network-access-type`</span></span>
* <span data-ttu-id="018bf-202">`az hdinsight create`: Parameter `--idbroker` hinzugefügt, um die Erstellung von ESP-Clustern mit HDInsight-Identitätsbroker für Kunden zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="018bf-202">`az hdinsight create`:  add parameter `--idbroker` to support customer to create ESP cluster with HDInsight Id Broker</span></span>

### <a name="iot-central"></a><span data-ttu-id="018bf-203">IoT Central</span><span class="sxs-lookup"><span data-stu-id="018bf-203">IoT Central</span></span>

* <span data-ttu-id="018bf-204">Veraltetes Befehlsmodul „az iotcentral“ entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-204">Remove deprecated 'az iotcentral' command module</span></span>

### <a name="key-vault"></a><span data-ttu-id="018bf-205">Key Vault</span><span class="sxs-lookup"><span data-stu-id="018bf-205">Key Vault</span></span>

* <span data-ttu-id="018bf-206">Unterstützung von `--hsm-name` für `az keyvault key encrypt/decrypt`</span><span class="sxs-lookup"><span data-stu-id="018bf-206">Support `--hsm-name` for `az keyvault key encrypt/decrypt`</span></span>

### <a name="lab"></a><span data-ttu-id="018bf-207">Labor</span><span class="sxs-lookup"><span data-stu-id="018bf-207">Lab</span></span>

* <span data-ttu-id="018bf-208">Fehlerbehebung Nr. 14127: `__init__()` akzeptiert ein positionelles Argument, angegeben wurden jedoch zwei.</span><span class="sxs-lookup"><span data-stu-id="018bf-208">Fix #14127: `__init__()` takes 1 positional argument but 2 were given</span></span>

### <a name="network"></a><span data-ttu-id="018bf-209">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="018bf-209">Network</span></span>

* <span data-ttu-id="018bf-210">`az network application-gateway ssl-cert show`: Beispiel zur Veranschaulichung des Zertifikatformats und der Abrufinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-210">`az network application-gateway ssl-cert show`: Add example to demonstrate certificate format and fetch information</span></span>
* <span data-ttu-id="018bf-211">`az network application-gateway rule`: Unterstützung für die Option „--priority“</span><span class="sxs-lookup"><span data-stu-id="018bf-211">`az network application-gateway rule`: Support --priority option</span></span>
* <span data-ttu-id="018bf-212">`az network application-gateway create`: Fehler behoben, dass die Erstellung ohne Angabe der öffentlichen IP-Adresse nicht möglich ist</span><span class="sxs-lookup"><span data-stu-id="018bf-212">`az network application-gateway create`: Fix bug that cannot create without public IP sepcified</span></span>
* <span data-ttu-id="018bf-213">`az network application-gateway waf-policy managed-rule rule-set add`: Verfügbarmachen des Serverfehlers für den Benutzer, um eine intuitivere Hinweismeldung zu ermöglich</span><span class="sxs-lookup"><span data-stu-id="018bf-213">`az network application-gateway waf-policy managed-rule rule-set add`: Expose server error to user to give more intuitive hint message.</span></span>
* <span data-ttu-id="018bf-214">`az network application-gateway waf-policy managed-rule rule-set update`: Unterstützung zur Änderung der Typversion des Regelsatzes</span><span class="sxs-lookup"><span data-stu-id="018bf-214">`az network application-gateway waf-policy managed-rule rule-set update`: Support to change rule set type version.</span></span>

### <a name="rdbms"></a><span data-ttu-id="018bf-215">RDBMS</span><span class="sxs-lookup"><span data-stu-id="018bf-215">RDBMS</span></span>

* <span data-ttu-id="018bf-216">Fehlerbehebung: az postgres flexible-server create – hartcodierte API-Version aus Netzwerkclient entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-216">Bugfix: az postgres flexible-server create Remove hardcoded API version from network client.</span></span>

### <a name="role"></a><span data-ttu-id="018bf-217">Role</span><span class="sxs-lookup"><span data-stu-id="018bf-217">Role</span></span>

* <span data-ttu-id="018bf-218">Fehlerbehebung Nr. 15278: `az role assignment list/delete`: Leere Zeichenfolgenargumente verboten</span><span class="sxs-lookup"><span data-stu-id="018bf-218">Fix #15278: `az role assignment list/delete`: Forbid empty string arguments</span></span>

### <a name="sql"></a><span data-ttu-id="018bf-219">SQL</span><span class="sxs-lookup"><span data-stu-id="018bf-219">SQL</span></span>

* <span data-ttu-id="018bf-220">`az sql midb log-replay`: Unterstützung für den Protokollwiedergabedienst in der verwalteten Datenbank</span><span class="sxs-lookup"><span data-stu-id="018bf-220">`az sql midb log-replay`: Support for log replay service on managed database</span></span>
* <span data-ttu-id="018bf-221">Ignorieren der Groß-/Kleinschreibung im Parameterwert für die Sicherungsspeicherredundanz für verwaltete Instanzen</span><span class="sxs-lookup"><span data-stu-id="018bf-221">Ignore character casing for backup storage redundancy param value for managed instance</span></span>
* <span data-ttu-id="018bf-222">[BREAKING CHANGE:] az sql db create: Parameter „--backup-storage-redundancy“ hinzugefügt. Warnung, wenn folgende Angabe fehlt: bsr/bsr == Geo</span><span class="sxs-lookup"><span data-stu-id="018bf-222">[BREAKING CHANGE] az sql db create: Add --backup-storage-redundancy parameter; add warning for unspecified bsr/bsr == Geo.</span></span>

### <a name="sql-vm"></a><span data-ttu-id="018bf-223">SQL-VM</span><span class="sxs-lookup"><span data-stu-id="018bf-223">SQL VM</span></span>

* <span data-ttu-id="018bf-224">`az sql vm show`: Konfigurationsoptionen für das Flag „--expand“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-224">`az sql vm show`: Add configuration options to --expand flag</span></span>

### <a name="storage"></a><span data-ttu-id="018bf-225">Storage</span><span class="sxs-lookup"><span data-stu-id="018bf-225">Storage</span></span>

* <span data-ttu-id="018bf-226">[BREAKING CHANGE] `az storage blob copy start`: Formatproblem für `--destination-if-modified-since` und `--destination-if-unmodified-since` behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-226">[BREAKING CHANGE] `az storage blob copy start`: Fix format issue for `--destination-if-modified-since` and `--destination-if-unmodified-since`</span></span>
* <span data-ttu-id="018bf-227">[BREAKING CHANGE] `az storage blob incremental-copy start`: Formatproblem für `--destination-if-modified-since` und `--destination-if-unmodified-since` behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-227">[BREAKING CHANGE] `az storage blob incremental-copy start`: Fix format issue for `--destination-if-modified-since` and `--destination-if-unmodified-since`</span></span>
* <span data-ttu-id="018bf-228">`az storage fs`: Problem mit Verbindungszeichenfolge behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-228">`az storage fs`: Fix connection string issue</span></span>
* <span data-ttu-id="018bf-229">`az storage share-rm`: Zugriffsebene der GA-Version</span><span class="sxs-lookup"><span data-stu-id="018bf-229">`az storage share-rm`: GA release access tier</span></span>
* <span data-ttu-id="018bf-230">`az storage container-rm`: Neue Befehlsgruppe hinzugefügt, um den Ressourcenanbieter „Microsoft.Storage“ für Verwaltungsvorgänge für Container zu verwenden</span><span class="sxs-lookup"><span data-stu-id="018bf-230">`az storage container-rm`: Add a new command group to use the Microsoft.Storage resource provider for container management operations.</span></span>

## <a name="september-29-2020"></a><span data-ttu-id="018bf-231">29. September 2020</span><span class="sxs-lookup"><span data-stu-id="018bf-231">September 29, 2020</span></span>

<span data-ttu-id="018bf-232">Version 2.12.1</span><span class="sxs-lookup"><span data-stu-id="018bf-232">Version 2.12.1</span></span>

### <a name="rdbms"></a><span data-ttu-id="018bf-233">RDBMS</span><span class="sxs-lookup"><span data-stu-id="018bf-233">RDBMS</span></span>

* <span data-ttu-id="018bf-234">Hotfix: `az postgres flexible-server create`: VnetName zum Ausschließen des Servernamens aktualisiert und Standardregion für MySQL aktualisiert</span><span class="sxs-lookup"><span data-stu-id="018bf-234">Hotfix: `az postgres flexible-server create` : Update VnetName to exclude servername and update default region for MySQL</span></span>

## <a name="september-22-2020"></a><span data-ttu-id="018bf-235">22. September 2020</span><span class="sxs-lookup"><span data-stu-id="018bf-235">September 22, 2020</span></span>

<span data-ttu-id="018bf-236">Version 2.12.0</span><span class="sxs-lookup"><span data-stu-id="018bf-236">Version 2.12.0</span></span>

### <a name="acr"></a><span data-ttu-id="018bf-237">ACR</span><span class="sxs-lookup"><span data-stu-id="018bf-237">ACR</span></span>

* <span data-ttu-id="018bf-238">Fehlerbehebung Nr. 14811: Hinzufügen von Unterstützung für die Außerkraftsetzung von „dockerignore“</span><span class="sxs-lookup"><span data-stu-id="018bf-238">Fix #14811 Add support for dockerignore override</span></span>

### <a name="aks"></a><span data-ttu-id="018bf-239">AKS</span><span class="sxs-lookup"><span data-stu-id="018bf-239">AKS</span></span>

* <span data-ttu-id="018bf-240">Die CLI sollte eine leere kubeconfig-Datei tolerieren.</span><span class="sxs-lookup"><span data-stu-id="018bf-240">CLI should tolerate empty kubeconfig</span></span>
* <span data-ttu-id="018bf-241">Fehlerbehebung Nr. 12871: az aks enable-addons: Das automatisch generierte Hilfebeispiel ist für die Option „virtual-node“ falsch.</span><span class="sxs-lookup"><span data-stu-id="018bf-241">FIX #12871: az aks enable-addons: Autogenerated help example is wrong for vitual-node option</span></span>
* <span data-ttu-id="018bf-242">Legacyaktionen für ACI-Connectors entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-242">Remove legacy aci connector actions</span></span>
* <span data-ttu-id="018bf-243">Unterstützung für Richtlinien-Add-On in der Azure CLI</span><span class="sxs-lookup"><span data-stu-id="018bf-243">Support azure policy addon in azure-cli</span></span>
* <span data-ttu-id="018bf-244">Problem mit Groß-/Kleinbuchstaben für AKS-Dashboard-Add-On behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-244">Fix case sensitive issue for AKS dashboard addon</span></span>
* <span data-ttu-id="018bf-245">„mgmt-containerservice“ auf 9.4.0 aktualisiert und 09-01-API aktiviert</span><span class="sxs-lookup"><span data-stu-id="018bf-245">Update mgmt-containerservice to 9.4.0 and enable 09-01 API</span></span>

### <a name="apim"></a><span data-ttu-id="018bf-246">APIM</span><span class="sxs-lookup"><span data-stu-id="018bf-246">APIM</span></span>

* <span data-ttu-id="018bf-247">Unterstützung der Befehle für die Entitäten „product“/„productapi“/„namedValue“ und SDK-Version aktualisiert</span><span class="sxs-lookup"><span data-stu-id="018bf-247">Support product / productapi / namedValue entity commands && bump sdk version</span></span>

### <a name="app-config"></a><span data-ttu-id="018bf-248">App-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="018bf-248">App Config</span></span>

* <span data-ttu-id="018bf-249">Unterstützung für die Aktivierung/Deaktivierung von PublicNetworkAccess für vorhandene Speicher</span><span class="sxs-lookup"><span data-stu-id="018bf-249">Support enabling/disabling PublicNetworkAccess for existing stores</span></span>

### <a name="app-service"></a><span data-ttu-id="018bf-250">App Service</span><span class="sxs-lookup"><span data-stu-id="018bf-250">App Service</span></span>

* <span data-ttu-id="018bf-251">Unterstützung für den Tarif „Premium V3“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-251">Add support for Premium V3 pricing tier</span></span>
* <span data-ttu-id="018bf-252">Fehlerbehebung Nr. 12653: az webapp log config --application-logging: keine Deaktivierung, wenn „false“ festgelegt ist</span><span class="sxs-lookup"><span data-stu-id="018bf-252">Fix #12653: az webapp log config --application-logging false doesn't turn it off</span></span>
* <span data-ttu-id="018bf-253">Fehlerbehebung Nr. 14684: Entfernen von „access-restriction“ nach IP-Adresse funktioniert nicht. Fehlerbehebung Nr. 13837: -az webapp create – Beispiel für verschiedene RSgroups für Plan und WebApp</span><span class="sxs-lookup"><span data-stu-id="018bf-253">Fix #14684: access-restriction remove by ip address does not work; #13837-az webapp create - Example for different RSgroups for Plan and WebApp</span></span>
* <span data-ttu-id="018bf-254">functionapp: Unterstützung für benutzerdefinierte Handler hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-254">functionapp: Add support for custom handlers.</span></span> <span data-ttu-id="018bf-255">Powershell 6.2 wurde als veraltet markiert.</span><span class="sxs-lookup"><span data-stu-id="018bf-255">Deprecated Powershell 6.2.</span></span>
* <span data-ttu-id="018bf-256">functionapp: Problem behoben, das dazu führte, dass die App-Einstellung für benutzerdefinierte Linux-Images falsch festgelegt wurde</span><span class="sxs-lookup"><span data-stu-id="018bf-256">functionapp: Fix issue where app setting was being incorrectly set for linux custom images</span></span>

### <a name="arm"></a><span data-ttu-id="018bf-257">ARM</span><span class="sxs-lookup"><span data-stu-id="018bf-257">ARM</span></span>

* <span data-ttu-id="018bf-258">`az deployment group/sub/mg/tenant what-if`: Ignorierte Ressourcenänderungen als letztes anzeigen</span><span class="sxs-lookup"><span data-stu-id="018bf-258">`az deployment group/sub/mg/tenant what-if`: Show "Ignore" resource changes last</span></span>

### <a name="compute"></a><span data-ttu-id="018bf-259">Compute</span><span class="sxs-lookup"><span data-stu-id="018bf-259">Compute</span></span>

* <span data-ttu-id="018bf-260">Neuer Lizenztyp bei VM-Erstellung/-Aktualisierung hinzugefügt: RHEL_BYOS, SLES_BYOS</span><span class="sxs-lookup"><span data-stu-id="018bf-260">Add new license_type in vm create/update: RHEL_BYOS, SLES_BYOS</span></span>
* <span data-ttu-id="018bf-261">Upgrade der Datenträger-API-Version auf 2020-06-30 durchgeführt</span><span class="sxs-lookup"><span data-stu-id="018bf-261">Upgrade disk API version to 2020-06-30</span></span>
* <span data-ttu-id="018bf-262">Datenträgererstellung: „--logical-sector-size“ und „--tier“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-262">disk create: add --logical-sector-size, --tier</span></span>
* <span data-ttu-id="018bf-263">Datenträgeraktualisierung: Unterstützung für „--disk-iops-read-only“, „--disk-mbps-read-only“, „--max-shares“</span><span class="sxs-lookup"><span data-stu-id="018bf-263">disk update: Support --disk-iops-read-only, --disk-mbps-read-only, --max-shares</span></span>
* <span data-ttu-id="018bf-264">Neuer Befehl: disk-encryption-set list-associated-resources</span><span class="sxs-lookup"><span data-stu-id="018bf-264">New command disk-encryption-set list-associated-resources</span></span>
* <span data-ttu-id="018bf-265">vm boot-diagnostics enable: „--storage“ wird optional.</span><span class="sxs-lookup"><span data-stu-id="018bf-265">vm boot-diagnostics enable: --storage becomes optional</span></span>
* <span data-ttu-id="018bf-266">Neuer Befehl: vm boot-diagnostics get-boot-log-uris</span><span class="sxs-lookup"><span data-stu-id="018bf-266">New command: vm boot-diagnostics get-boot-log-uris</span></span>
* <span data-ttu-id="018bf-267">vm boot-diagnostics get-boot-log: Unterstützung für verwalteten Speicher</span><span class="sxs-lookup"><span data-stu-id="018bf-267">vm boot-diagnostics get-boot-log: support managed storage</span></span>

### <a name="config"></a><span data-ttu-id="018bf-268">Konfigurationen</span><span class="sxs-lookup"><span data-stu-id="018bf-268">Config</span></span>

* <span data-ttu-id="018bf-269">„local-context“ in „config param-persist“ umbenannt</span><span class="sxs-lookup"><span data-stu-id="018bf-269">Rename local-context to config param-persist</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="018bf-270">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="018bf-270">Cosmos DB</span></span>

* <span data-ttu-id="018bf-271">Unterstützung für Migrations-APIs für Durchsatzressource für das Autoskalierungsfeature in CosmosDB</span><span class="sxs-lookup"><span data-stu-id="018bf-271">Support for Migration APIs for Throughput resource for Autoscale feature in CosmosDB</span></span>

### <a name="eventhub"></a><span data-ttu-id="018bf-272">Eventhub</span><span class="sxs-lookup"><span data-stu-id="018bf-272">Eventhub</span></span>

<span data-ttu-id="018bf-273">Clusterbefehle und Parameter „trusted_service_access_enabled“ für Networkruleset hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-273">Added Cluster commands and trusted_service_access_enabled parameter for Networkruleset</span></span>

### <a name="extension"></a><span data-ttu-id="018bf-274">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="018bf-274">Extension</span></span>

* <span data-ttu-id="018bf-275">`az extension add`: Option `--upgrade` hinzugefügt, um die Erweiterung zu aktualisieren, sofern sie bereits installiert ist</span><span class="sxs-lookup"><span data-stu-id="018bf-275">`az extension add`: Add `--upgrade` option to update the extension if already installed</span></span>
* <span data-ttu-id="018bf-276">Dynamische Installation standardmäßig aktivieren</span><span class="sxs-lookup"><span data-stu-id="018bf-276">Turn on dynamic install by default</span></span>

### <a name="iot"></a><span data-ttu-id="018bf-277">IoT</span><span class="sxs-lookup"><span data-stu-id="018bf-277">IoT</span></span>

* <span data-ttu-id="018bf-278">Minimale TLS-Version bei IoT Hub-Erstellung zulässig</span><span class="sxs-lookup"><span data-stu-id="018bf-278">Enabled minimum TLS version on IoT Hub Create</span></span>

### <a name="iot-central"></a><span data-ttu-id="018bf-279">IoT Central</span><span class="sxs-lookup"><span data-stu-id="018bf-279">IoT Central</span></span>

* <span data-ttu-id="018bf-280">Der Vorgang zum Löschen der App ist jetzt ein zeitintensiver Vorgang.</span><span class="sxs-lookup"><span data-stu-id="018bf-280">App delete operation is now long running operation</span></span>

### <a name="iot-hub"></a><span data-ttu-id="018bf-281">IoT Hub</span><span class="sxs-lookup"><span data-stu-id="018bf-281">Iot Hub</span></span>

* <span data-ttu-id="018bf-282">Befehl „show-connection-string“ als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="018bf-282">Deprecated 'show-connection-string' command</span></span>

### <a name="key-vault"></a><span data-ttu-id="018bf-283">Key Vault</span><span class="sxs-lookup"><span data-stu-id="018bf-283">Key Vault</span></span>

* <span data-ttu-id="018bf-284">Public Preview von verwaltetem HSM</span><span class="sxs-lookup"><span data-stu-id="018bf-284">Managed HSM public preview</span></span>
* <span data-ttu-id="018bf-285">Problem behoben, dass `--maxresults` beim Auflisten von Ressourcen oder Ressourcenversionen nicht wirksam wird</span><span class="sxs-lookup"><span data-stu-id="018bf-285">Fix the issue that `--maxresults` does not take effect while listing resources or resource versions</span></span>

### <a name="kusto"></a><span data-ttu-id="018bf-286">Kusto</span><span class="sxs-lookup"><span data-stu-id="018bf-286">Kusto</span></span>

* <span data-ttu-id="018bf-287">Nachricht zur Einstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-287">Add deprecating message</span></span>

### <a name="monitor"></a><span data-ttu-id="018bf-288">Überwachen</span><span class="sxs-lookup"><span data-stu-id="018bf-288">Monitor</span></span>

* <span data-ttu-id="018bf-289">`az monitor log-analytics workspace linked-storage`: detaillierte Fehlermeldung für Kunden verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="018bf-289">`az monitor log-analytics workspace linked-storage`: expose detailed error message to customers</span></span>

### <a name="network"></a><span data-ttu-id="018bf-290">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="018bf-290">Network</span></span>

* <span data-ttu-id="018bf-291">`az network vnet subnet`: Unterstützung für „--disable-private-endpoint-network-policies“ und „--disable-private-link-service-network-policies“</span><span class="sxs-lookup"><span data-stu-id="018bf-291">`az network vnet subnet`: Support --disable-private-endpoint-network-policies and --disable-private-link-service-network-policies</span></span>
* <span data-ttu-id="018bf-292">Problem behoben, das beim Aktualisieren von „flow-log“ auftrat, wenn die untergeordnete Eigenschaft „network_watcher_flow_analytics_configuration“ auf „None“ festgelegt war</span><span class="sxs-lookup"><span data-stu-id="018bf-292">Fix bug while updateing flow-log when its subproperty network_watcher_flow_analytics_configuration is None</span></span>
* <span data-ttu-id="018bf-293">Aktualisierung der API-Version auf 2020-06-01</span><span class="sxs-lookup"><span data-stu-id="018bf-293">API version bump to 2020-06-01</span></span>
* <span data-ttu-id="018bf-294">Unterstützung für „--tcp-port-behavior“ beim Konfigurieren einer TCP-Konfiguration von Verbindungsmonitor V2</span><span class="sxs-lookup"><span data-stu-id="018bf-294">Support --tcp-port-behavior while configuring a TCP configuration of a Connection Monitor V2</span></span>
* <span data-ttu-id="018bf-295">Unterstützung für mehr Typen und Abdeckungsebenen beim Erstellen eines Endpunkts von Verbindungsmonitor V2</span><span class="sxs-lookup"><span data-stu-id="018bf-295">Support more types and coverage level while creating Endpoint of Connection Monitor V2</span></span>
* <span data-ttu-id="018bf-296">Unterstützung für „--host-subnet“, um VirtualHub unter VirtualRouter zu erstellen</span><span class="sxs-lookup"><span data-stu-id="018bf-296">Support --host-subnet to create VirtualHub underneath as VirtualRouter</span></span>

### <a name="rdbms"></a><span data-ttu-id="018bf-297">RDBMS</span><span class="sxs-lookup"><span data-stu-id="018bf-297">RDBMS</span></span>

* <span data-ttu-id="018bf-298">Aktualisierungen der Verwaltungsebene für PostgreSQL und MySQL</span><span class="sxs-lookup"><span data-stu-id="018bf-298">Management Plane updates for PostgreSQL and MySQL</span></span>

### <a name="role"></a><span data-ttu-id="018bf-299">Role</span><span class="sxs-lookup"><span data-stu-id="018bf-299">Role</span></span>

* <span data-ttu-id="018bf-300">`az role assignment create/update`: Unterstützung für `--description`, `--condition` und `--condition-version`</span><span class="sxs-lookup"><span data-stu-id="018bf-300">`az role assignment create/update`: Support `--description`, `--condition` and `--condition-version`</span></span>
* <span data-ttu-id="018bf-301">`az ad app permission delete`: Unterstützung für `--api-permissions` zum Löschen spezifischer `ResourceAccess`-Elemente</span><span class="sxs-lookup"><span data-stu-id="018bf-301">`az ad app permission delete`: Support `--api-permissions` to delete specific `ResourceAccess`</span></span>

### <a name="service-fabric"></a><span data-ttu-id="018bf-302">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="018bf-302">Service Fabric</span></span>

* <span data-ttu-id="018bf-303">Befehle für verwaltete Cluster und Knotentypen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-303">Add managed cluster and node type commands</span></span>

### <a name="sql"></a><span data-ttu-id="018bf-304">SQL</span><span class="sxs-lookup"><span data-stu-id="018bf-304">SQL</span></span>

* <span data-ttu-id="018bf-305">„azure-mgmt-sql“ auf 0.20.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="018bf-305">Upgrade azure-mgmt-sql to 0.20.0</span></span>
* <span data-ttu-id="018bf-306">Optionaler Parameter für Redundanz des Sicherungsspeichers zum Cmdlet „mi create“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-306">Add backup storage redundancy optional parameter to MI create cmdlet</span></span>

### <a name="storage"></a><span data-ttu-id="018bf-307">Storage</span><span class="sxs-lookup"><span data-stu-id="018bf-307">Storage</span></span>

* <span data-ttu-id="018bf-308">`az storage share-rm stats`: Abrufen der Nutzung (in Bytes) der auf der Freigabe gespeicherten Daten</span><span class="sxs-lookup"><span data-stu-id="018bf-308">`az storage share-rm stats`: Get the usage bytes of the data stored on the share.</span></span>
* <span data-ttu-id="018bf-309">Allgemein verfügbares Release für Zeitpunktwiederherstellung von Speicherblobs</span><span class="sxs-lookup"><span data-stu-id="018bf-309">GA release storage blob PITR</span></span>
* <span data-ttu-id="018bf-310">`az storage blob query`: Unterstützung für Azure Storage-Abfragebeschleunigung</span><span class="sxs-lookup"><span data-stu-id="018bf-310">`az storage blob query`: Support Azure Storage Query Acceleration</span></span>
* <span data-ttu-id="018bf-311">Unterstützung des vorläufigen Löschens für Dateifreigaben</span><span class="sxs-lookup"><span data-stu-id="018bf-311">Support Soft Delete for file share</span></span>
* <span data-ttu-id="018bf-312">`az storage copy`: Unterstützung für Kontoanmeldeinformationen hinzugefügt und `--source-local-path`, `--destination-local-path` und `--destination-account-name` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="018bf-312">`az storage copy`: Add account credentials support and deprecate `--source-local-path`, `--destination-local-path`, `--destination-account-name`</span></span>
* <span data-ttu-id="018bf-313">`az storage account blob-service-properties update`: Unterstützung der Aufbewahrungsrichtlinie für Containerlöschungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-313">`az storage account blob-service-properties update`: Add container delete retention policy support</span></span>

### <a name="synapse"></a><span data-ttu-id="018bf-314">Synapse</span><span class="sxs-lookup"><span data-stu-id="018bf-314">Synapse</span></span>

* <span data-ttu-id="018bf-315">Tippfehler im Beispiel für „az synapse role assignment create“ und „az synapse role assignment delete“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="018bf-315">Fixed typo in example of az synapse role assignment create and delete</span></span>

## <a name="august-28-2020"></a><span data-ttu-id="018bf-316">28. August 2020</span><span class="sxs-lookup"><span data-stu-id="018bf-316">August 28, 2020</span></span>

<span data-ttu-id="018bf-317">Version 2.11.1</span><span class="sxs-lookup"><span data-stu-id="018bf-317">Version 2.11.1</span></span>

### <a name="acr"></a><span data-ttu-id="018bf-318">ACR</span><span class="sxs-lookup"><span data-stu-id="018bf-318">ACR</span></span>

* <span data-ttu-id="018bf-319">Dienstebene „Isoliert“ zum Agentpool hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-319">Add Isolated Tier to Agent Pool</span></span>
* <span data-ttu-id="018bf-320">Quellkontext des OCI-Artefakts hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-320">Add OCI Artifact Source Context</span></span>

### <a name="aks"></a><span data-ttu-id="018bf-321">AKS</span><span class="sxs-lookup"><span data-stu-id="018bf-321">AKS</span></span>

* <span data-ttu-id="018bf-322">Problem bei der Erstellung des AKS-Clusters behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-322">Fix aks cluster create issue</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="018bf-323">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="018bf-323">Cognitive Services</span></span>

* <span data-ttu-id="018bf-324">[BREAKING CHANGE] Anzeigen zusätzlicher rechtlicher Bedingungen für bestimmte APIs</span><span class="sxs-lookup"><span data-stu-id="018bf-324">[BREAKING CHANGE] Show additional legal term for certain APIs</span></span>

### <a name="network"></a><span data-ttu-id="018bf-325">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="018bf-325">Network</span></span>

* <span data-ttu-id="018bf-326">[BREAKING CHANGE] Erstellung öffentlicher und privater IP-Adressen beim Erstellen einer Application Gateway-Instanz zulässig</span><span class="sxs-lookup"><span data-stu-id="018bf-326">[BREAKING CHANGE] Allow to create both public and private IP while creating an Application Gateway</span></span>
* <span data-ttu-id="018bf-327">`az network list-service-tags`: Details zur Verwendung des Standortparameters zur Hilfemeldung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-327">`az network list-service-tags`: add details on location parameter use to the help message</span></span>

### <a name="storage"></a><span data-ttu-id="018bf-328">Storage</span><span class="sxs-lookup"><span data-stu-id="018bf-328">Storage</span></span>

* <span data-ttu-id="018bf-329">`az storage blob list`: Unterstützung der OR-Eigenschaften mit neuer API-Version</span><span class="sxs-lookup"><span data-stu-id="018bf-329">`az storage blob list`: Support OR properties with new api version</span></span>

## <a name="august-25-2020"></a><span data-ttu-id="018bf-330">25. August 2020</span><span class="sxs-lookup"><span data-stu-id="018bf-330">August 25, 2020</span></span>

<span data-ttu-id="018bf-331">Version 2.11.0</span><span class="sxs-lookup"><span data-stu-id="018bf-331">Version 2.11.0</span></span>

### <a name="aks"></a><span data-ttu-id="018bf-332">AKS</span><span class="sxs-lookup"><span data-stu-id="018bf-332">AKS</span></span>

* <span data-ttu-id="018bf-333">Vorschautag aus dem Add-On für virtuelle Knoten entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-333">Remove preview tag from Virtual Node add-on</span></span>
* <span data-ttu-id="018bf-334">AKS-CMK-Argument bei Clustererstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-334">Add AKS CMK argument in cluster creation</span></span>
* <span data-ttu-id="018bf-335">Netzwerkprofil bei Verwendung des Lastenausgleichs im Basic-Tarif festgelegt</span><span class="sxs-lookup"><span data-stu-id="018bf-335">Set network profile when using basic load balancer.</span></span>
* <span data-ttu-id="018bf-336">Überprüfung der maximalen Pods aus CLI entfernt, wird nun durch Preflight verarbeitet</span><span class="sxs-lookup"><span data-stu-id="018bf-336">Remove max pods validation from CLI and let preflight handle it</span></span>
* <span data-ttu-id="018bf-337">Add-Ons korrigiert, die in der Hilfemeldung in `az aks create` verfügbar sind</span><span class="sxs-lookup"><span data-stu-id="018bf-337">Fixing add-ons available in the help message in `az aks create`</span></span>
* <span data-ttu-id="018bf-338">Unterstützung für das Autoskalierungsprofil für Cluster in Core-CLI hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-338">Bring in support for cluster autoscaler profile in core CLI</span></span>

### <a name="appservice"></a><span data-ttu-id="018bf-339">AppService</span><span class="sxs-lookup"><span data-stu-id="018bf-339">AppService</span></span>

* <span data-ttu-id="018bf-340">`az webapp`: Befehl „list-instances“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-340">`az webapp`: Add list-instances command</span></span>
* <span data-ttu-id="018bf-341">`az webapp ssh`: Parameter „--instance“ für die Verbindungsherstellung mit einer bestimmten Instanz hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-341">`az webapp ssh`: Add --instance parameter to connect to a specific instance</span></span>
* <span data-ttu-id="018bf-342">`az webapp create-remote-connection`: Parameter „--instance“ für die Verbindungsherstellung mit einer bestimmten Instanz hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-342">`az webapp create-remote-connection`: Add --instance parameter to connect to a specific instance</span></span>
* <span data-ttu-id="018bf-343">Fehlerbehebung Nr. 14758: Fehler bei „az webapp create“ beim Erstellen von Windows-Apps mit „--runtime dotnetcore“</span><span class="sxs-lookup"><span data-stu-id="018bf-343">Fix #14758: az webapp create errors when creating windows app with --runtime dotnetcore</span></span>
* <span data-ttu-id="018bf-344">Fehlerbehebung Nr. 14701: „functionapp create --assign-identity“ implementiert</span><span class="sxs-lookup"><span data-stu-id="018bf-344">Fix #14701: Implement functionapp create --assign-identity</span></span>
* <span data-ttu-id="018bf-345">Fehlerbehebung Nr. 11244: `az webapp auth update`: Optionaler Parameter zum Aktualisieren von „client-secret-certificate-thumbprint“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-345">Fix #11244: `az webapp auth update`: Add optional parameter to update client-secret-certificate-thumbprint</span></span>
* <span data-ttu-id="018bf-346">`az functionapp keys`: Befehle hinzugefügt, mit denen Benutzer die Funktions-App-Schlüssel verwalten können</span><span class="sxs-lookup"><span data-stu-id="018bf-346">`az functionapp keys`: Added commands that allow users to manage their function app keys</span></span>
* <span data-ttu-id="018bf-347">`az functionapp function`: Befehle hinzugefügt, mit denen Benutzer die einzelnen Funktionen verwalten können</span><span class="sxs-lookup"><span data-stu-id="018bf-347">`az functionapp function`: Added commands that allow users to manage their individual functions</span></span>
* <span data-ttu-id="018bf-348">`az functionapp function keys`: Befehle hinzugefügt, mit denen Benutzer die Funktionsschlüssel verwalten können</span><span class="sxs-lookup"><span data-stu-id="018bf-348">`az functionapp function keys`: Added commands that allow users to manage their function keys</span></span>
* <span data-ttu-id="018bf-349">Fehlerbehebung Nr. 14788: Mit „az webapp create“ kann nicht die richtige Web-App abgerufen werden, wenn es sich bei den Namen um Teilzeichenfolgen handelt.</span><span class="sxs-lookup"><span data-stu-id="018bf-349">Fix #14788: az webapp create not getting correct webapp when names are substrings</span></span>
* <span data-ttu-id="018bf-350">`az functionapp create`: Möglichkeit zum Erstellen von 2.x-Funktionen in Regionen entfernt, in denen sie nicht unterstützt werden</span><span class="sxs-lookup"><span data-stu-id="018bf-350">`az functionapp create`: Removed ability to create 2.x Functions in regions that don't support it</span></span>

### <a name="arm"></a><span data-ttu-id="018bf-351">ARM</span><span class="sxs-lookup"><span data-stu-id="018bf-351">ARM</span></span>

* <span data-ttu-id="018bf-352">`az resource list`: Rückgabedaten von `createdTime`, `changedTime` und `provisioningState` erweitert</span><span class="sxs-lookup"><span data-stu-id="018bf-352">`az resource list`: Extend the return data of `createdTime`, `changedTime` and `provisioningState`</span></span>
* <span data-ttu-id="018bf-353">`az resource`: Parameter `--latest-include-preview` hinzugefügt, um die Verwendung der neuesten API-Version zu unterstützen, unabhängig davon, ob es sich dabei um eine Vorschauversion handelt</span><span class="sxs-lookup"><span data-stu-id="018bf-353">`az resource`: Add parameter `--latest-include-preview` to support using the latest api-version whether this version is preview</span></span>

### <a name="aro"></a><span data-ttu-id="018bf-354">ARO</span><span class="sxs-lookup"><span data-stu-id="018bf-354">ARO</span></span>

* <span data-ttu-id="018bf-355">CLI-Erweiterungen, einschließlich Berechtigungen für die Überprüfung von Routingtabellen</span><span class="sxs-lookup"><span data-stu-id="018bf-355">CLI enhancements, including route table checking permissions</span></span>

### <a name="cloud"></a><span data-ttu-id="018bf-356">Cloud</span><span class="sxs-lookup"><span data-stu-id="018bf-356">Cloud</span></span>

* <span data-ttu-id="018bf-357">`az cloud register`: Registrierung von Clouds mit einer Konfigurationsdatei korrigiert</span><span class="sxs-lookup"><span data-stu-id="018bf-357">`az cloud register`: Fix registering clouds with a config file</span></span>

### <a name="compute"></a><span data-ttu-id="018bf-358">Compute</span><span class="sxs-lookup"><span data-stu-id="018bf-358">Compute</span></span>

* <span data-ttu-id="018bf-359">VM-SKUs aktualisiert, die den beschleunigten Netzwerkbetrieb unterstützen</span><span class="sxs-lookup"><span data-stu-id="018bf-359">Update VM SKUs that support accelerated networking</span></span>
* <span data-ttu-id="018bf-360">`az vm create`: Automatische Patches auf Gastsystemen</span><span class="sxs-lookup"><span data-stu-id="018bf-360">`az vm create`: Automatic in-guest patching</span></span>
* <span data-ttu-id="018bf-361">`az image builder create`: „--vm-size“, „--os-disk-size“, „--vnet“ und „--subnet“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-361">`az image builder create`: Add --vm-size, --os-disk-size, --vnet, --subnet</span></span>
* <span data-ttu-id="018bf-362">Neuer Befehl „az vm assess-patches“</span><span class="sxs-lookup"><span data-stu-id="018bf-362">New command az vm assess-patches</span></span>

### <a name="container"></a><span data-ttu-id="018bf-363">Container</span><span class="sxs-lookup"><span data-stu-id="018bf-363">Container</span></span>

* <span data-ttu-id="018bf-364">Fehlerbehebung Nr. 6235: Hilfetext für ports-Parameter bei der Containererstellung aktualisiert</span><span class="sxs-lookup"><span data-stu-id="018bf-364">Fix #6235: Update help text for ports parameter in container create</span></span>

### <a name="datalake-store"></a><span data-ttu-id="018bf-365">Data Lake-Speicher</span><span class="sxs-lookup"><span data-stu-id="018bf-365">Datalake Store</span></span>

* <span data-ttu-id="018bf-366">Fehlerbehebung Nr. 14545 für Data Lake-Verknüpfungsvorgang</span><span class="sxs-lookup"><span data-stu-id="018bf-366">Fix issue #14545 for data lake join operation</span></span>

### <a name="eventhub"></a><span data-ttu-id="018bf-367">EventHub</span><span class="sxs-lookup"><span data-stu-id="018bf-367">EventHub</span></span>

* <span data-ttu-id="018bf-368">`az eventhubs eventhub create/update`: Dokumentation zu „destination_name“ geändert</span><span class="sxs-lookup"><span data-stu-id="018bf-368">`az eventhubs eventhub create/update`: Change documentation of destination_name</span></span>

### <a name="extension"></a><span data-ttu-id="018bf-369">Erweiterung</span><span class="sxs-lookup"><span data-stu-id="018bf-369">Extension</span></span>

* <span data-ttu-id="018bf-370">Befehl `az extension list-versions` hinzugefügt, um alle verfügbaren Versionen einer Erweiterung aufzulisten</span><span class="sxs-lookup"><span data-stu-id="018bf-370">Add `az extension list-versions` command to list all available versions of an extension</span></span>

### <a name="hdinsight"></a><span data-ttu-id="018bf-371">HDInsight</span><span class="sxs-lookup"><span data-stu-id="018bf-371">HDInsight</span></span>

* <span data-ttu-id="018bf-372">Unterstützung für das Erstellen von Clustern mit Autoskalierungskonfiguration und Unterstützung für die Verwaltung der Autoskalierungskonfiguration</span><span class="sxs-lookup"><span data-stu-id="018bf-372">Support creating cluster with autoscale configuration and Support managing autoscale configuration</span></span>
* <span data-ttu-id="018bf-373">Unterstützung für das Erstellen eines Clusters mit Verschlüsselung auf dem Host</span><span class="sxs-lookup"><span data-stu-id="018bf-373">Support creating cluster with encryption at host</span></span>

### <a name="iotcentral"></a><span data-ttu-id="018bf-374">IoTCentral</span><span class="sxs-lookup"><span data-stu-id="018bf-374">IoTCentral</span></span>

* <span data-ttu-id="018bf-375">Verbesserungen bei der CLI-Dokumentation</span><span class="sxs-lookup"><span data-stu-id="018bf-375">CLI documentation improvements</span></span>

### <a name="monitor"></a><span data-ttu-id="018bf-376">Überwachen</span><span class="sxs-lookup"><span data-stu-id="018bf-376">Monitor</span></span>

* <span data-ttu-id="018bf-377">`az monitor metrics alert create`: Unterstützung von „RG“ und „Sub“ als Bereichswerte</span><span class="sxs-lookup"><span data-stu-id="018bf-377">`az monitor metrics alert create`: support RG and Sub as the scope values</span></span>

### <a name="netappfiles"></a><span data-ttu-id="018bf-378">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="018bf-378">NetAppFiles</span></span>

* <span data-ttu-id="018bf-379">[BREAKING CHANGE] az netappfiles snapshot create: „file-system-id“ aus Parametern entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-379">[BREAKING CHANGE] az netappfiles snapshot create: Removed file-system-id from parameters</span></span>
* <span data-ttu-id="018bf-380">[BREAKING CHANGE] az netappfiles snapshot show: Die Momentaufnahme enthält nicht länger den Parameter „file-system-id“.</span><span class="sxs-lookup"><span data-stu-id="018bf-380">[BREAKING CHANGE] az netappfiles snapshot show: Snapshot no longer has parameter file-system-id</span></span>
* <span data-ttu-id="018bf-381">`az netappfiles account`: Das Modell „ActiveDirectory“ verfügt nun über den neuen Parameter „backup_operators“.</span><span class="sxs-lookup"><span data-stu-id="018bf-381">`az netappfiles account`: Model ActiveDirectory has a new parameter backup_operators</span></span>
* <span data-ttu-id="018bf-382">`az netappfiles volume show`: Das Modell „dataProtection“ verfügt nun über den neuen Parameter „snapshot“.</span><span class="sxs-lookup"><span data-stu-id="018bf-382">`az netappfiles volume show`: Model dataProtection has a new parameter snapshot</span></span>
* <span data-ttu-id="018bf-383">`az netappfiles volume show`: Das Modell „Volume“ verfügt nun über den neuen Parameter „snapshot_directory_visible“.</span><span class="sxs-lookup"><span data-stu-id="018bf-383">`az netappfiles volume show`: Model Volume has a new parameter snapshot_directory_visible</span></span>

### <a name="network"></a><span data-ttu-id="018bf-384">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="018bf-384">Network</span></span>

* <span data-ttu-id="018bf-385">`az network dns export`: Für MX, PTR, NS und SRV wird nun der FQDN anstelle des relativen Pfads exportiert.</span><span class="sxs-lookup"><span data-stu-id="018bf-385">`az network dns export`: export FQDN for MX, PTR, NS and SRV type instead of relative path</span></span>
* <span data-ttu-id="018bf-386">Unterstützung privater Links für verwaltete Datenträger</span><span class="sxs-lookup"><span data-stu-id="018bf-386">Support private link for managed disks</span></span>
* <span data-ttu-id="018bf-387">`az network application-gateway auth-cert show`: Beispiel zur Veranschaulichung des Zertifikatformats hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-387">`az network application-gateway auth-cert show`: Add example to demonstrate certificate format</span></span>
* <span data-ttu-id="018bf-388">`az network private-endpoint-connection`: Unterstützung der App-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="018bf-388">`az network private-endpoint-connection`: support app configuration</span></span>

### <a name="rbac"></a><span data-ttu-id="018bf-389">RBAC</span><span class="sxs-lookup"><span data-stu-id="018bf-389">RBAC</span></span>

* <span data-ttu-id="018bf-390">`az ad group create`: Unterstützung der Angabe einer Beschreibung beim Erstellen einer Gruppe</span><span class="sxs-lookup"><span data-stu-id="018bf-390">`az ad group create`: support specify description when creating a group</span></span>
* <span data-ttu-id="018bf-391">`az role definition create`: Ausgabe einer lesbaren Nachricht anstelle einer Ausnahme, wenn „assignableScope“ ein leeres Array ist</span><span class="sxs-lookup"><span data-stu-id="018bf-391">`az role definition create`: print human readable message instead of exception when assignableScope is an empty array</span></span>
* <span data-ttu-id="018bf-392">[BREAKING CHANGE] `az ad sp create-for-rbac`: Standardberechtigung des erstellten Zertifikats geändert</span><span class="sxs-lookup"><span data-stu-id="018bf-392">[BREAKING CHANGE] `az ad sp create-for-rbac`: change default permission of created certificate</span></span>

### <a name="sql"></a><span data-ttu-id="018bf-393">SQL</span><span class="sxs-lookup"><span data-stu-id="018bf-393">SQL</span></span>

* <span data-ttu-id="018bf-394">`az sql server audit-policy`: Unterstützung für SQL Server-Überwachung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-394">`az sql server audit-policy`: Add sql server auditing support</span></span>

### <a name="storage"></a><span data-ttu-id="018bf-395">Storage</span><span class="sxs-lookup"><span data-stu-id="018bf-395">Storage</span></span>

* <span data-ttu-id="018bf-396">`az storage blob copy start-batch`: Fehlerbehebung Nr. 6018 für „--source-sas“</span><span class="sxs-lookup"><span data-stu-id="018bf-396">`az storage blob copy start-batch`: Fix #6018 for --source-sas</span></span>
* <span data-ttu-id="018bf-397">`az storage account or-policy`: Unterstützung für die Objektreplikationsrichtlinie für Speicherkonten</span><span class="sxs-lookup"><span data-stu-id="018bf-397">`az storage account or-policy`: Support storage account object replication policy</span></span>
* <span data-ttu-id="018bf-398">Fehlerbehebung Nr. 14083, um die Version des Pakets „azure-multiapi-storage“ aufgrund eines Paketproblems zu aktualisieren und neue API-Versionen zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="018bf-398">Fix issue #14083 to upgrade azure-multiapi-storage package version for package issue and new api version support</span></span>
* <span data-ttu-id="018bf-399">`az storage blob generate-sas`: Beispiele für „--ip“ hinzugefügt und Fehlermeldung optimiert</span><span class="sxs-lookup"><span data-stu-id="018bf-399">`az storage blob generate-sas`: add examples for --ip  and refine error message</span></span>
* <span data-ttu-id="018bf-400">`az storage blob list`: Problem bei „next_marker“ behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-400">`az storage blob list`: Fix next_marker issue</span></span>

### <a name="synapse"></a><span data-ttu-id="018bf-401">Synapse</span><span class="sxs-lookup"><span data-stu-id="018bf-401">Synapse</span></span>

* <span data-ttu-id="018bf-402">Cmdlets für Arbeitsbereich, Spark-Pool und SQL-Pool hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-402">Add workspace, sparkpool, sqlpool related cmdlets</span></span>
* <span data-ttu-id="018bf-403">Befehle im Zusammenhang mit Spark-Aufträgen basierend auf track2 SDK hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-403">Add spark job releated commands based on track2 sdk</span></span>
* <span data-ttu-id="018bf-404">Befehle im Zusammenhang mit accesscontrol-Feature basierend auf track2 SDK hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-404">Add accesscontrol feature related commands based on track2 sdk</span></span>

### <a name="upgrade"></a><span data-ttu-id="018bf-405">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="018bf-405">Upgrade</span></span>

* <span data-ttu-id="018bf-406">Befehl `az upgrade` zum Aktualisieren der Azure CLI und von Erweiterungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-406">Add `az upgrade` command to upgrade azure cli and extensions</span></span>

## <a name="august-11-2020"></a><span data-ttu-id="018bf-407">11. August 2020</span><span class="sxs-lookup"><span data-stu-id="018bf-407">August 11, 2020</span></span>

<span data-ttu-id="018bf-408">Version 2.10.1</span><span class="sxs-lookup"><span data-stu-id="018bf-408">Version 2.10.1</span></span>

### <a name="app-service"></a><span data-ttu-id="018bf-409">App Service</span><span class="sxs-lookup"><span data-stu-id="018bf-409">App Service</span></span>

* <span data-ttu-id="018bf-410">Behebung Nr. 9887: webapp und functionapp, Unterstützung für das Zuweisen/Entfernen einer benutzerseitig verwalteten Identität</span><span class="sxs-lookup"><span data-stu-id="018bf-410">Fix #9887 webapp and functionapp, support assigning/removing user managed identity</span></span>
* <span data-ttu-id="018bf-411">Behebung Nr. 1382, Nr. 14055: Fehlermeldungen für „az webapp create“ und „az webapp config container set“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="018bf-411">Fix #1382, #14055: Update error messages for az webapp create and az webapp config container set</span></span>
* <span data-ttu-id="018bf-412">`az webapp up`: Standardmäßige ASP-Auswahllogik korrigiert, wenn der Parameter „--plan“ nicht angegeben wird</span><span class="sxs-lookup"><span data-stu-id="018bf-412">`az webapp up`: Fix default ASP selection logic when --plan parameter is not provided</span></span>

### <a name="appconfig"></a><span data-ttu-id="018bf-413">AppConfig</span><span class="sxs-lookup"><span data-stu-id="018bf-413">AppConfig</span></span>

* <span data-ttu-id="018bf-414">Unterstützung für die Aktivierung/Deaktivierung von PublicNetworkAccess während der Speichererstellung</span><span class="sxs-lookup"><span data-stu-id="018bf-414">Support enabling/disabling PublicNetworkAccess during store creation</span></span>

### <a name="compute"></a><span data-ttu-id="018bf-415">Compute</span><span class="sxs-lookup"><span data-stu-id="018bf-415">Compute</span></span>

* <span data-ttu-id="018bf-416">Unterstützung für das Zuordnen einer Datenträgerzugriffsressource für Datenträger und Momentaufnahmen</span><span class="sxs-lookup"><span data-stu-id="018bf-416">Support associating disk and snapshot with a disk-access resource</span></span>

### <a name="lab"></a><span data-ttu-id="018bf-417">Labor</span><span class="sxs-lookup"><span data-stu-id="018bf-417">Lab</span></span>

* <span data-ttu-id="018bf-418">Fehlerbehebung Nr. 7904: Fehler bei der Datumsüberprüfung bei der Lab-VM-Erstellung</span><span class="sxs-lookup"><span data-stu-id="018bf-418">Fix for issue #7904 date validation bug in lab vm creation</span></span>

### <a name="storage"></a><span data-ttu-id="018bf-419">Storage</span><span class="sxs-lookup"><span data-stu-id="018bf-419">Storage</span></span>

* <span data-ttu-id="018bf-420">`az storage blob upload-batch`: Problembehebung Nr. 14660 mit nicht positionellen Argumenten</span><span class="sxs-lookup"><span data-stu-id="018bf-420">`az storage blob upload-batch`: Fix issue #14660 with unpositional arguments</span></span>

## <a name="august-04-2020"></a><span data-ttu-id="018bf-421">04. August 2020</span><span class="sxs-lookup"><span data-stu-id="018bf-421">August 04, 2020</span></span>

<span data-ttu-id="018bf-422">Version 2.10.0</span><span class="sxs-lookup"><span data-stu-id="018bf-422">Version 2.10.0</span></span>

### <a name="aks"></a><span data-ttu-id="018bf-423">AKS</span><span class="sxs-lookup"><span data-stu-id="018bf-423">AKS</span></span>

* <span data-ttu-id="018bf-424">`az aks update`: Argument „--enable-aad“ geändert, um einen RBAC-fähigen AAD-fremden Cluster zu einem von AKS-verwalteten AAD-Cluster zu migrieren</span><span class="sxs-lookup"><span data-stu-id="018bf-424">`az aks update`: Change --enable-aad argument to migrate a RBAC-enabled non-AAD cluster to a AKS-managed AAD cluster</span></span>
* <span data-ttu-id="018bf-425">`az aks install-cli`: Argumente „--kubelogin-version“ und „--kubelogin-install-location“ zum Installieren von kubelogin hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-425">`az aks install-cli`: Add --kubelogin-version and --kubelogin-install-location arguments to install kubelogin</span></span>
* <span data-ttu-id="018bf-426">Befehl „az aks nodepool get-upgrades“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-426">Add az aks nodepool get-upgrades command</span></span>

### <a name="ams"></a><span data-ttu-id="018bf-427">AMS</span><span class="sxs-lookup"><span data-stu-id="018bf-427">AMS</span></span>

* <span data-ttu-id="018bf-428">Korrektur 14021: „az ams account sp“ ist nicht idempotent.</span><span class="sxs-lookup"><span data-stu-id="018bf-428">Fix #14021: az ams account sp is not idempotent</span></span>

### <a name="apim"></a><span data-ttu-id="018bf-429">APIM</span><span class="sxs-lookup"><span data-stu-id="018bf-429">APIM</span></span>

* <span data-ttu-id="018bf-430">APIM-API-Import: API-Importunterstützung und Erweiterung anderer CLI-Befehle auf der API-Ebene</span><span class="sxs-lookup"><span data-stu-id="018bf-430">apim api import: support API import and enchance other api level cli commands</span></span>

### <a name="app-service"></a><span data-ttu-id="018bf-431">App Service</span><span class="sxs-lookup"><span data-stu-id="018bf-431">App Service</span></span>

* <span data-ttu-id="018bf-432">Korrektur 13035: Zugriffsbeschränkungsüberprüfung für „az webapp config“ hinzugefügt, um Duplikate zu vermeiden</span><span class="sxs-lookup"><span data-stu-id="018bf-432">Fix #13035: Add validation for az webapp config access-restriction to avoid adding duplicates</span></span>

### <a name="appconfig"></a><span data-ttu-id="018bf-433">AppConfig</span><span class="sxs-lookup"><span data-stu-id="018bf-433">AppConfig</span></span>

* <span data-ttu-id="018bf-434">Bei fehlender Angabe wird die Standard-SKU verwendet.</span><span class="sxs-lookup"><span data-stu-id="018bf-434">Default to standard sku if not specified</span></span>
* <span data-ttu-id="018bf-435">[BREAKING CHANGE] Einstellungen mit JSON-Inhaltstyp werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="018bf-435">[BREAKING CHANGE] Support settings with JSON content type</span></span>

### <a name="arm"></a><span data-ttu-id="018bf-436">ARM</span><span class="sxs-lookup"><span data-stu-id="018bf-436">ARM</span></span>

* <span data-ttu-id="018bf-437">`az resource tag`: Fehler im Zusammenhang mit managedApp-Kennzeichnung sowie einige damit zusammenhängende Testprobleme behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-437">`az resource tag`: Fix the bug of managedApp tagging and some related test issues</span></span>
* <span data-ttu-id="018bf-438">`az deployment mg/tenant what-if`: Unterstützung für die Bereitstellung auf Verwaltungsgruppen- und Mandantenebene hinzugefügt (Was-wäre-wenn)</span><span class="sxs-lookup"><span data-stu-id="018bf-438">`az deployment mg/tenant what-if`: Add support to management group and tenant level deployment What-If</span></span>
* <span data-ttu-id="018bf-439">`az deployment mg/tenant create`: Parameter „--confirm-with-what-if/-c“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-439">`az deployment mg/tenant create`: Add --confirm-with-what-if/-c parameter.</span></span>
* <span data-ttu-id="018bf-440">`az deployment mg/tenant create`: Parameter „--what-if-result-format/-r“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-440">`az deployment mg/tenant create`: Add --what-if-result-format/-r parameter.</span></span>
* <span data-ttu-id="018bf-441">`az deployment mg/tenant create`: Parameter „--what-if-exclude-change-types/-x“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-441">`az deployment mg/tenant create`: Add --what-if-exclude-change-types/-x parameter.</span></span>
* <span data-ttu-id="018bf-442">`az tag`: Unterstützung von „az tag“ für Ressourcen-ID-Parameter</span><span class="sxs-lookup"><span data-stu-id="018bf-442">`az tag`: az tag support for resource id parameter</span></span>

### <a name="backup"></a><span data-ttu-id="018bf-443">Backup</span><span class="sxs-lookup"><span data-stu-id="018bf-443">Backup</span></span>

* <span data-ttu-id="018bf-444">Auslösung von AFS-Container-/Elementerkennung nur bei Bedarf</span><span class="sxs-lookup"><span data-stu-id="018bf-444">Trigger AFS container/item discovery only when needed</span></span>

### <a name="cdn"></a><span data-ttu-id="018bf-445">CDN</span><span class="sxs-lookup"><span data-stu-id="018bf-445">CDN</span></span>

* <span data-ttu-id="018bf-446">Private Link-Felder zu Ursprung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-446">Add private link fields to origin</span></span>

### <a name="compute"></a><span data-ttu-id="018bf-447">Compute</span><span class="sxs-lookup"><span data-stu-id="018bf-447">Compute</span></span>

* <span data-ttu-id="018bf-448">`az vm/vmss create`: Wahl eines gültigen Benutzernamens für den Benutzer bei ungültigem Standardbenutzernamen</span><span class="sxs-lookup"><span data-stu-id="018bf-448">`az vm/vmss create`: Select a valid username for user if the default username is invalid</span></span>
* <span data-ttu-id="018bf-449">`az vm update`: Unterstützung mandantenübergreifender Images</span><span class="sxs-lookup"><span data-stu-id="018bf-449">`az vm update`: support cross tenant image</span></span>
* <span data-ttu-id="018bf-450">`az disk-access`: Neue Befehlsgruppe für die Verwendung der Datenträgerzugriffsressource hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-450">`az disk-access`: Add new command group to operate disk access resource</span></span>
* <span data-ttu-id="018bf-451">Unterstützung der automatischen Platzierung dedizierter Hostgruppen</span><span class="sxs-lookup"><span data-stu-id="018bf-451">Support dedicated host group automatic placement</span></span>
* <span data-ttu-id="018bf-452">Unterstützung von PPG und SPG im VMSS-Orchestrierungsmodus</span><span class="sxs-lookup"><span data-stu-id="018bf-452">Support ppg and spg in VMSS orchestration mode</span></span>

### <a name="config"></a><span data-ttu-id="018bf-453">Config</span><span class="sxs-lookup"><span data-stu-id="018bf-453">Config</span></span>

* <span data-ttu-id="018bf-454">`az config`: Neuer Befehl (`config`) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-454">`az config`: Add new `config` command module</span></span>

### <a name="extension"></a><span data-ttu-id="018bf-455">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="018bf-455">Extension</span></span>

* <span data-ttu-id="018bf-456">Unterstützung der automatischen Installation einer Erweiterung, wenn die Erweiterung eines Befehls nicht installiert ist</span><span class="sxs-lookup"><span data-stu-id="018bf-456">Support automatically installing an extension if the extension of a command is not installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="018bf-457">HDInsight</span><span class="sxs-lookup"><span data-stu-id="018bf-457">HDInsight</span></span>

* <span data-ttu-id="018bf-458">Drei Parameter zum Befehl `az hdinsight create` hinzugefügt, um Private Link und Verschlüsselung während der Übertragung zu unterstützen:</span><span class="sxs-lookup"><span data-stu-id="018bf-458">Add 3 parameters to the command `az hdinsight create` to support private link and encryption in transit feature:</span></span>

### <a name="iot-hub"></a><span data-ttu-id="018bf-459">IoT Hub</span><span class="sxs-lookup"><span data-stu-id="018bf-459">Iot Hub</span></span>

* <span data-ttu-id="018bf-460">Korrektur 7792: „iot hub create“ ist nicht idempotent.</span><span class="sxs-lookup"><span data-stu-id="018bf-460">Fix #7792: IoT Hub Create is not idempotent</span></span>

### <a name="iot-central"></a><span data-ttu-id="018bf-461">IoT Central</span><span class="sxs-lookup"><span data-stu-id="018bf-461">IoT Central</span></span>

* <span data-ttu-id="018bf-462">Parameteroptionenliste für IoT Central hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-462">Add paramater option list for iot central</span></span>

### <a name="keyvault"></a><span data-ttu-id="018bf-463">KeyVault</span><span class="sxs-lookup"><span data-stu-id="018bf-463">KeyVault</span></span>

* <span data-ttu-id="018bf-464">`az keyvault key encrypt/decrypt`: Parameter `--data-type` zum expliziten Angeben der Art von Originaldaten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-464">`az keyvault key encrypt/decrypt`: add parameter `--data-type` for explicitly specifing the type of original data</span></span>

### <a name="monitor"></a><span data-ttu-id="018bf-465">Überwachen</span><span class="sxs-lookup"><span data-stu-id="018bf-465">Monitor</span></span>

* <span data-ttu-id="018bf-466">`az monitor log-analytics workspace data-export`: Unterstützung des Event Hub-Namespace als Ziel</span><span class="sxs-lookup"><span data-stu-id="018bf-466">`az monitor log-analytics workspace data-export`: support event hub namespace as the destination.</span></span>
* <span data-ttu-id="018bf-467">`az monitor autoscale`: Unterstützung von Namespace und Dimensionen für „--condition“</span><span class="sxs-lookup"><span data-stu-id="018bf-467">`az monitor autoscale`: support namespace and dimensions for --condition</span></span>

### <a name="netappfiles"></a><span data-ttu-id="018bf-468">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="018bf-468">NetAppFiles</span></span>

* <span data-ttu-id="018bf-469">`az volume revert`:  Volumewiederherstellung hinzugefügt, um ein Volume auf eine der zugehörigen Momentaufnahmen zurückzusetzen</span><span class="sxs-lookup"><span data-stu-id="018bf-469">`az volume revert`:  Add Volume Revert to revert a volume to one of its snapshots.</span></span>
* <span data-ttu-id="018bf-470">[BREAKING CHANGE] `az netappfiles mount-target` entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-470">[BREAKING CHANGE] Remove `az netappfiles mount-target`.</span></span>
* <span data-ttu-id="018bf-471">`az volume show`: Standort zu Active Directory-Eigenschaften hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-471">`az volume show`: Add site to Active Directory Properties</span></span>

### <a name="network"></a><span data-ttu-id="018bf-472">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="018bf-472">Network</span></span>

* <span data-ttu-id="018bf-473">`az application-gateway private-link add`: Unterstützung der Angabe eines vorhandenen Subnetzes nach ID</span><span class="sxs-lookup"><span data-stu-id="018bf-473">`az application-gateway private-link add`: support to specify an existing subnet by ID</span></span>
* <span data-ttu-id="018bf-474">`az network application-gateway waf-policy create`: Unterstützung von Version und Typ</span><span class="sxs-lookup"><span data-stu-id="018bf-474">`az network application-gateway waf-policy create`: support version and type</span></span>

### <a name="storage"></a><span data-ttu-id="018bf-475">Storage</span><span class="sxs-lookup"><span data-stu-id="018bf-475">Storage</span></span>

* <span data-ttu-id="018bf-476">Korrektur 10302: Unterstützung der Ermittlung des wahrscheinlichen Inhaltstyps beim Synchronisieren von Dateien</span><span class="sxs-lookup"><span data-stu-id="018bf-476">Fix #10302: Support guess content-type when synchronizing files</span></span>
* <span data-ttu-id="018bf-477">`az storage blob lease`: Neue API-Version für Blobleasevorgänge angewendet</span><span class="sxs-lookup"><span data-stu-id="018bf-477">`az storage blob lease`: Apply new api version for blob lease operations</span></span>
* <span data-ttu-id="018bf-478">`az storage fs access`: Unterstützung von AAD-Anmeldeinformationen bei der Verwaltung der Zugriffssteuerung für das ADLS Gen2-Konto</span><span class="sxs-lookup"><span data-stu-id="018bf-478">`az storage fs access`: Support AAD credential in managing access control for ADLS Gen2 account</span></span>
* <span data-ttu-id="018bf-479">`az storage share-rm create/update`: „--access-tier“ hinzugefügt, um die Zugriffsebene zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="018bf-479">`az storage share-rm create/update`: add --access-tier to support access tier</span></span>

## <a name="july-16-2020"></a><span data-ttu-id="018bf-480">16. Juli 2020</span><span class="sxs-lookup"><span data-stu-id="018bf-480">July 16, 2020</span></span>

<span data-ttu-id="018bf-481">Version 2.9.1</span><span class="sxs-lookup"><span data-stu-id="018bf-481">Version 2.9.1</span></span>

### <a name="aks"></a><span data-ttu-id="018bf-482">AKS</span><span class="sxs-lookup"><span data-stu-id="018bf-482">AKS</span></span>

* <span data-ttu-id="018bf-483">Explizite Einstellung von VMSS im Windows-Beispielbefehl entfernt, da dies jetzt die Standardeinstellung ist</span><span class="sxs-lookup"><span data-stu-id="018bf-483">Remove explicit setting of VMSS in Windows example command since it is now default</span></span>

### <a name="iot"></a><span data-ttu-id="018bf-484">IoT</span><span class="sxs-lookup"><span data-stu-id="018bf-484">IoT</span></span>

* <span data-ttu-id="018bf-485">[BREAKING CHANGE] `az iot pnp`: IoT-PNP-Vorschaubefehle aus Core-CLI entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-485">[BREAKING CHANGE] `az iot pnp`: Remove IoT PNP preview commands from core CLI</span></span>

### <a name="rest"></a><span data-ttu-id="018bf-486">REST</span><span class="sxs-lookup"><span data-stu-id="018bf-486">REST</span></span>

* <span data-ttu-id="018bf-487">Behebung Nr. 14152: `az rest`: ARM-URLs ohne Abonnement-ID werden nun akzeptiert.</span><span class="sxs-lookup"><span data-stu-id="018bf-487">Fix #14152: `az rest`: Accept ARM URLs without subscription ID</span></span>

### <a name="storage"></a><span data-ttu-id="018bf-488">Storage</span><span class="sxs-lookup"><span data-stu-id="018bf-488">Storage</span></span>

* <span data-ttu-id="018bf-489">Behebung Nr. 14138: Einige Berechtigungen sind nun optional.</span><span class="sxs-lookup"><span data-stu-id="018bf-489">Fix #14138: Make some permissions optional</span></span>

## <a name="july-14-2020"></a><span data-ttu-id="018bf-490">14. Juli 2020</span><span class="sxs-lookup"><span data-stu-id="018bf-490">July 14, 2020</span></span>

<span data-ttu-id="018bf-491">Version 2.9.0</span><span class="sxs-lookup"><span data-stu-id="018bf-491">Version 2.9.0</span></span>

### <a name="acr"></a><span data-ttu-id="018bf-492">ACR</span><span class="sxs-lookup"><span data-stu-id="018bf-492">ACR</span></span>

* <span data-ttu-id="018bf-493">Verarbeiten des Protokollartefaktlinks aus der Registrierung zum Streamen von Protokollen</span><span class="sxs-lookup"><span data-stu-id="018bf-493">Handle log artifact link from Registry to stream logs</span></span>
* <span data-ttu-id="018bf-494">Helm2-Befehle als veraltet kennzeichnen</span><span class="sxs-lookup"><span data-stu-id="018bf-494">Deprecate helm2 commands</span></span>

### <a name="aks"></a><span data-ttu-id="018bf-495">AKS</span><span class="sxs-lookup"><span data-stu-id="018bf-495">AKS</span></span>

* <span data-ttu-id="018bf-496">`az aks create`: Argument „--enable-aad“ hinzufügen</span><span class="sxs-lookup"><span data-stu-id="018bf-496">`az aks create`: add --enable-aad argument</span></span>
* <span data-ttu-id="018bf-497">`az aks update`: Argument „--enable-aad“ hinzufügen</span><span class="sxs-lookup"><span data-stu-id="018bf-497">`az aks update`: add --enable-aad argument</span></span>

### <a name="apim"></a><span data-ttu-id="018bf-498">APIM</span><span class="sxs-lookup"><span data-stu-id="018bf-498">APIM</span></span>

* <span data-ttu-id="018bf-499">Allgemeine Befehle vom Typ „az apim api“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-499">Added general az apim api commands</span></span>

### <a name="appconfig"></a><span data-ttu-id="018bf-500">AppConfig</span><span class="sxs-lookup"><span data-stu-id="018bf-500">AppConfig</span></span>

* <span data-ttu-id="018bf-501">Beispiel für die Verwendung von „--fields“ in AppConfig-Revision hinzufügen</span><span class="sxs-lookup"><span data-stu-id="018bf-501">Add example for using --fields in appconfig revision</span></span>

### <a name="appservice"></a><span data-ttu-id="018bf-502">AppService</span><span class="sxs-lookup"><span data-stu-id="018bf-502">AppService</span></span>

* <span data-ttu-id="018bf-503">`az functionapp create`: Unterstützung für Java 11 und PowerShell 7 hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-503">`az functionapp create`: Added support for Java 11 and Powershell 7.</span></span> <span data-ttu-id="018bf-504">Unterstützung für Stapel-API hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-504">Added Stacks API Support.</span></span>
* <span data-ttu-id="018bf-505">Behebung von Nr. 14208: Erstellen einer App mit mehreren Containern erzeugt einen Fehler</span><span class="sxs-lookup"><span data-stu-id="018bf-505">Fix #14208 multi-container app creation fails</span></span>
* <span data-ttu-id="018bf-506">Korrektur von „az webapp create“ – hartcodierte Laufzeitstapel verwenden</span><span class="sxs-lookup"><span data-stu-id="018bf-506">Fix az webapp create - use hardcoded runtime stacks</span></span>

### <a name="arm"></a><span data-ttu-id="018bf-507">ARM</span><span class="sxs-lookup"><span data-stu-id="018bf-507">ARM</span></span>

* <span data-ttu-id="018bf-508">`az resource tag`: Behebung des Problems beim Taggen von Ressourcen mit dem Ressourcentyp `Microsoft.ContainerInstance/containerGroups`</span><span class="sxs-lookup"><span data-stu-id="018bf-508">`az resource tag`: Fix the problem of tagging resources with resource type `Microsoft.ContainerInstance/containerGroups`</span></span>

### <a name="compute"></a><span data-ttu-id="018bf-509">Compute</span><span class="sxs-lookup"><span data-stu-id="018bf-509">Compute</span></span>

* <span data-ttu-id="018bf-510">Datenträgerversion aktualisieren 2020-05-01, Compute 2020-06-01</span><span class="sxs-lookup"><span data-stu-id="018bf-510">Bump version disks 2020-05-01, compute 2020-06-01</span></span>
* <span data-ttu-id="018bf-511">Doppelte Verschlüsselung des Datenträgerverschlüsselungssatzes</span><span class="sxs-lookup"><span data-stu-id="018bf-511">Double encryption of disk encryption set</span></span>
* <span data-ttu-id="018bf-512">`az vmss update`: Unterstützung für das Angeben eines mandantenübergreifendes Image.</span><span class="sxs-lookup"><span data-stu-id="018bf-512">`az vmss update`: support specify cross tenant image.</span></span>
* <span data-ttu-id="018bf-513">`az sig image-version create`: Unterstützung für das Angeben eines mandantenübergreifendes Image.</span><span class="sxs-lookup"><span data-stu-id="018bf-513">`az sig image-version create`: support specify cross tenant image.</span></span>
* <span data-ttu-id="018bf-514">vm/vmss create: Verschlüsselung von Cache und Daten während der Übertragung für (Betriebssystem-)Datenträger und temporäre Datenträger für VM und VMSS</span><span class="sxs-lookup"><span data-stu-id="018bf-514">vm/vmss create: Encryption of cache & data-in-transit for OS/Data disks and temp disks for VM & VMSS</span></span>
* <span data-ttu-id="018bf-515">Vorgang „simulate-eviction“ für VM und VMSS hinzufügen</span><span class="sxs-lookup"><span data-stu-id="018bf-515">Add simulate-eviction operation for VM and VMSS</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="018bf-516">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="018bf-516">CosmosDB</span></span>

* <span data-ttu-id="018bf-517">Aktuelle Features: Autoscale, IpRules, EnableFreeTier und EnableAnalyticalStorage</span><span class="sxs-lookup"><span data-stu-id="018bf-517">Recent features: Autoscale, IpRules, EnableFreeTier and EnableAnalyticalStorage</span></span>

### <a name="eventgrid"></a><span data-ttu-id="018bf-518">EventGrid</span><span class="sxs-lookup"><span data-stu-id="018bf-518">EventGrid</span></span>

* <span data-ttu-id="018bf-519">CLI-Unterstützung für 2020-04-01-preview hinzufügen und Previewfunktionen mit „is_Preview=True“ kennzeichnen</span><span class="sxs-lookup"><span data-stu-id="018bf-519">Add CLI support for 2020-04-01-preview and mark preview features with is_Preview=True</span></span>

### <a name="find"></a><span data-ttu-id="018bf-520">Suchen</span><span class="sxs-lookup"><span data-stu-id="018bf-520">Find</span></span>

* <span data-ttu-id="018bf-521">Behebung von Nr. 14094 „az find“: Abfragen schlagen fehl, wenn nicht angemeldet und Telemetrie deaktiviert</span><span class="sxs-lookup"><span data-stu-id="018bf-521">Fix #14094 az find Fix Queries failing when not logged in and when telemetry is disabled</span></span>

### <a name="hdinsight"></a><span data-ttu-id="018bf-522">HDInsight</span><span class="sxs-lookup"><span data-stu-id="018bf-522">HDInsight</span></span>

* <span data-ttu-id="018bf-523">Zwei Befehle zur Unterstützung der Neustartfunktion für HDInsight-Knoten hinzufügen</span><span class="sxs-lookup"><span data-stu-id="018bf-523">Add two commands to support hdinsight node reboot feature</span></span>

### <a name="monitor"></a><span data-ttu-id="018bf-524">Überwachen</span><span class="sxs-lookup"><span data-stu-id="018bf-524">Monitor</span></span>

* <span data-ttu-id="018bf-525">Vorschaukennzeichnung für Befehle unter Log Analytics-Arbeitsbereich entfernen</span><span class="sxs-lookup"><span data-stu-id="018bf-525">Remove preview flag for commands under Log Analytics workspace</span></span>
* <span data-ttu-id="018bf-526">`az monitor diagnostic-settings subscription`: Diagnoseeinstellungen für Abonnement unterstützen</span><span class="sxs-lookup"><span data-stu-id="018bf-526">`az monitor diagnostic-settings subscription`: Support diagnositc settings for subscription</span></span>
* <span data-ttu-id="018bf-527">`az monitor metrics`: „,“ und „|“ in Metrikname unterstützen</span><span class="sxs-lookup"><span data-stu-id="018bf-527">`az monitor metrics`: support ',' and '|' in metric name</span></span>
* <span data-ttu-id="018bf-528">`az monitor log-analytics workspace data-export`: Log Analytics-Datenexport unterstützen</span><span class="sxs-lookup"><span data-stu-id="018bf-528">`az monitor log-analytics workspace data-export`: support log analytics data export</span></span>

### <a name="network"></a><span data-ttu-id="018bf-529">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="018bf-529">Network</span></span>

* <span data-ttu-id="018bf-530">`az network application-gateway frontend-ip update`: Parameter „--public-ip-address“ als veraltet markieren</span><span class="sxs-lookup"><span data-stu-id="018bf-530">`az network application-gateway frontend-ip update`: Deprecating the --public-ip-address parameter</span></span>
* <span data-ttu-id="018bf-531">„azure-mgmt-network“ auf 11.0.0 aktualisieren</span><span class="sxs-lookup"><span data-stu-id="018bf-531">Bump azure-mgmt-network to 11.0.0</span></span>
* <span data-ttu-id="018bf-532">`az network express-route gateway connection`: Routingkonfiguration unterstützen</span><span class="sxs-lookup"><span data-stu-id="018bf-532">`az network express-route gateway connection`: support routing configuration</span></span>
* <span data-ttu-id="018bf-533">`az network virtual-appliance`: Virtuelle Azure-Netzwerkgerät unterstützen.</span><span class="sxs-lookup"><span data-stu-id="018bf-533">`az network virtual-appliance`: Support Azure network virtual appliance.</span></span>
* <span data-ttu-id="018bf-534">Application Gateway-Unterstützung der Funktion für private Links</span><span class="sxs-lookup"><span data-stu-id="018bf-534">Application Gateway support private link feature</span></span>

### <a name="policyinsights"></a><span data-ttu-id="018bf-535">PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="018bf-535">PolicyInsights</span></span>

* <span data-ttu-id="018bf-536">`az policy state`: Befehl „trigger-scan“ zu Auswertungen der Compliance von Auslöserrichtinien hinzufügen</span><span class="sxs-lookup"><span data-stu-id="018bf-536">`az policy state`: add trigger-scan command to trigger policy compliance evaluations</span></span>
* <span data-ttu-id="018bf-537">`az policy state list`: Versionen von Richtlinienentitäten in jedem Compliancedatensatz verfügbar machen</span><span class="sxs-lookup"><span data-stu-id="018bf-537">`az policy state list`: expose versions of policy entities in each compliance record</span></span>

### <a name="profile"></a><span data-ttu-id="018bf-538">Profil</span><span class="sxs-lookup"><span data-stu-id="018bf-538">Profile</span></span>

* <span data-ttu-id="018bf-539">`az account get-access-token`: „expiresOn“ für verwaltete Identität anzeigen</span><span class="sxs-lookup"><span data-stu-id="018bf-539">`az account get-access-token`: Show expiresOn for Managed Identity</span></span>

### <a name="rdbms"></a><span data-ttu-id="018bf-540">RDBMS</span><span class="sxs-lookup"><span data-stu-id="018bf-540">RDBMS</span></span>

* <span data-ttu-id="018bf-541">TLS-Mindestversion unterstützen</span><span class="sxs-lookup"><span data-stu-id="018bf-541">Support Minimum TLS version</span></span>
* <span data-ttu-id="018bf-542">Infrastrukturverschlüsselung für Azure Postgres und MySQL hinzufügen</span><span class="sxs-lookup"><span data-stu-id="018bf-542">Add Infrastructure Encryption for Azure Postgres and MySQL</span></span>

### <a name="security"></a><span data-ttu-id="018bf-543">Sicherheit</span><span class="sxs-lookup"><span data-stu-id="018bf-543">Security</span></span>

* <span data-ttu-id="018bf-544">Befehl „allowed_connections“ hinzufügen</span><span class="sxs-lookup"><span data-stu-id="018bf-544">Add allowed_connections commands</span></span>
* <span data-ttu-id="018bf-545">Befehle für adaptive Netzwerkhärtung hinzufügen</span><span class="sxs-lookup"><span data-stu-id="018bf-545">Add Adaptive network hardeningss commands</span></span>
* <span data-ttu-id="018bf-546">Befehle vom Typ „adaptive_application_controls“ hinzufügen</span><span class="sxs-lookup"><span data-stu-id="018bf-546">Add adaptive_application_controls commands</span></span>
* <span data-ttu-id="018bf-547">Hinzufügen von „az security iot-solution“/„iot-alerts“/„iot-recommendations“/„iot-analytics“ REST zu Azure CLI</span><span class="sxs-lookup"><span data-stu-id="018bf-547">Addition of az security iot-solution/ iot-alerts/iot-recommendations/iot-analytics REST to Azure CLI</span></span>
* <span data-ttu-id="018bf-548">CLI für Einhaltung gesetzlicher Bestimmungen hinzufügen</span><span class="sxs-lookup"><span data-stu-id="018bf-548">Add regulatory compliance CLI</span></span>

### <a name="signalr"></a><span data-ttu-id="018bf-549">SignalR</span><span class="sxs-lookup"><span data-stu-id="018bf-549">SignalR</span></span>

* <span data-ttu-id="018bf-550">Features einschließlich der Verwaltung privater Endpunktverbindungen, Netzwerkregeln und Upstream hinzufügen</span><span class="sxs-lookup"><span data-stu-id="018bf-550">Add features including managing private endpoint connections, network rules and upstream</span></span>

### <a name="sql"></a><span data-ttu-id="018bf-551">SQL</span><span class="sxs-lookup"><span data-stu-id="018bf-551">SQL</span></span>

* <span data-ttu-id="018bf-552">`az sql mi create`, `az sql mi update`: Parameter `--tags` zur Unterstützung von Ressourcenkennzeichnung hinzufügen</span><span class="sxs-lookup"><span data-stu-id="018bf-552">`az sql mi create`, `az sql mi update`: Add `--tags` parameter to support resource tagging</span></span>
* <span data-ttu-id="018bf-553">`az sql mi failover`: Failover vom primären oder sekundären Punkt unterstützen</span><span class="sxs-lookup"><span data-stu-id="018bf-553">`az sql mi failover`: Support failover from primary or secondary point</span></span>

### <a name="storage"></a><span data-ttu-id="018bf-554">Storage</span><span class="sxs-lookup"><span data-stu-id="018bf-554">Storage</span></span>

* <span data-ttu-id="018bf-555">`az storage account create/update`: „--allow-blob-public-access“ hinzufügen, um den öffentlichen Zugriff für Blob und Container zuzulassen oder zu unterbinden</span><span class="sxs-lookup"><span data-stu-id="018bf-555">`az storage account create/update`: Add --allow-blob-public-access to allow or disallow public access for blob and containers</span></span>
* <span data-ttu-id="018bf-556">`az storage account create/update`: `--min-tls-version` hinzufügen, um das Festlegen der TLS-Mindestversion für Anforderungen an den Speicher zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="018bf-556">`az storage account create/update`: Add `--min-tls-version` to support setting the minimum TLS version to be permitted on requests to storage.</span></span>
* <span data-ttu-id="018bf-557">Token-Anmeldeinformationen zum Einchecken entfernen</span><span class="sxs-lookup"><span data-stu-id="018bf-557">Remove check in token credential</span></span>
* <span data-ttu-id="018bf-558">Namen des Speicherkontos in Beispielen korrigieren</span><span class="sxs-lookup"><span data-stu-id="018bf-558">Fix the storage account name in examples</span></span>

### <a name="webapp"></a><span data-ttu-id="018bf-559">Webapp</span><span class="sxs-lookup"><span data-stu-id="018bf-559">Webapp</span></span>

* <span data-ttu-id="018bf-560">Fehlerbehebung: „az webapp log deployment show -“ gibt Bereitstellungsprotokolle anstatt von Protokollmetadaten zurück</span><span class="sxs-lookup"><span data-stu-id="018bf-560">Bugfix: az webapp log deployment show - return deployment logs instead of log metadata</span></span>
* <span data-ttu-id="018bf-561">Fehlerbehebung: „az webapp vnet-integration“ hinzufügen – Fehlerbehandlung korrigieren bei ungültigem VNET-Namen, VNET-Ressourcen-ID unterstützen</span><span class="sxs-lookup"><span data-stu-id="018bf-561">Bugfix: az webapp vnet-integration add - fix error handling if bad vnet name, support vnet resource ID</span></span>

## <a name="june-23-2020"></a><span data-ttu-id="018bf-562">23. Juni 2020</span><span class="sxs-lookup"><span data-stu-id="018bf-562">June 23, 2020</span></span>

<span data-ttu-id="018bf-563">Version 2.8.0</span><span class="sxs-lookup"><span data-stu-id="018bf-563">Version 2.8.0</span></span>

### <a name="acr"></a><span data-ttu-id="018bf-564">ACR</span><span class="sxs-lookup"><span data-stu-id="018bf-564">ACR</span></span>

* <span data-ttu-id="018bf-565">Unterstützung für Deaktivierung des Regionsendpunkts/Routings hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-565">Add support for region endpoint disable / routing disable</span></span>
* <span data-ttu-id="018bf-566">[BREAKING CHANGE] `az acr login --expose-token` akzeptiert Benutzername und Kennwort nicht.</span><span class="sxs-lookup"><span data-stu-id="018bf-566">[BREAKING CHANGE] `az acr login --expose-token` does not accept username and password</span></span>

### <a name="acs"></a><span data-ttu-id="018bf-567">ACS</span><span class="sxs-lookup"><span data-stu-id="018bf-567">ACS</span></span>

* <span data-ttu-id="018bf-568">Privater Cluster und API „2019-10-27-preview“ entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-568">Remove private cluster and 2019-10-27-preview API</span></span>

### <a name="aks"></a><span data-ttu-id="018bf-569">AKS</span><span class="sxs-lookup"><span data-stu-id="018bf-569">AKS</span></span>

* <span data-ttu-id="018bf-570">Unterstützung: Ja, für „az aks upgrade“</span><span class="sxs-lookup"><span data-stu-id="018bf-570">Support --yes for az aks upgrade</span></span>
* <span data-ttu-id="018bf-571">„Änderung der Standard-VM-SKU in Standard_D2s_v3 (Nr. 13541)“ wiederhergestellt</span><span class="sxs-lookup"><span data-stu-id="018bf-571">Revert "change default vm sku to Standard_D2s_v3 (#13541)"</span></span>
* <span data-ttu-id="018bf-572">„az aks update --uptime-sla“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-572">Add "az aks update --uptime-sla"</span></span>
* <span data-ttu-id="018bf-573">Tippfehler im Befehl „az aks update“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="018bf-573">Fix typo in az aks update command</span></span>
* <span data-ttu-id="018bf-574">Änderung, um einen Agentpool mit 0 Knoten zu unterstützen und die manuelle Skalierung für einen Pool mit CAS-Aktivierung zu blockieren</span><span class="sxs-lookup"><span data-stu-id="018bf-574">Change to support 0 node agent pool and block manual scale for CAS enabled pool</span></span>
* <span data-ttu-id="018bf-575">Tippfehler in VirtualMachineScaleSets korrigiert und Verweise auf Kubernetes-Versionen aktualisiert</span><span class="sxs-lookup"><span data-stu-id="018bf-575">Fix typo on VirtualMachineScaleSets and update references to Kubernetes versions</span></span>

### <a name="ams"></a><span data-ttu-id="018bf-576">AMS</span><span class="sxs-lookup"><span data-stu-id="018bf-576">AMS</span></span>

* <span data-ttu-id="018bf-577">ÄNDERUNG: Hilfetext für Parameter „--expiry“</span><span class="sxs-lookup"><span data-stu-id="018bf-577">CHANGE help text for "--expiry" parameter.</span></span>

### <a name="appservice"></a><span data-ttu-id="018bf-578">AppService</span><span class="sxs-lookup"><span data-stu-id="018bf-578">AppService</span></span>

* <span data-ttu-id="018bf-579">`az webapp log deployment show`: Anzeigen des aktuellen Bereitstellungsprotokolls oder der Bereitstellungsprotokolle einer bestimmten Bereitstellung, wenn die Bereitstellungs-ID angegeben ist</span><span class="sxs-lookup"><span data-stu-id="018bf-579">`az webapp log deployment show`: Show the latest deployment log, or the deployment logs of a specific deployment if deployment-id is specified</span></span>
* <span data-ttu-id="018bf-580">`az webapp log deployment list`: Liste der verfügbaren Bereitstellungsprotokolle</span><span class="sxs-lookup"><span data-stu-id="018bf-580">`az webapp log deployment list`: List of deployment logs available</span></span>
* <span data-ttu-id="018bf-581">Behebung: Oberflächenfehler bei Angabe eines ungültigen Web-App-Namens</span><span class="sxs-lookup"><span data-stu-id="018bf-581">Fix: Surface error when invalid webapp name provided</span></span>
* <span data-ttu-id="018bf-582">Nr. 13261 korrigiert: „az webapp list-runtimes“ nutzt eine statische Liste, bis die neue API für verfügbare Stapel zur Verfügung steht</span><span class="sxs-lookup"><span data-stu-id="018bf-582">Fix #13261 az webapp list-runtimes use static list until new Available Stacks API is available</span></span>
* <span data-ttu-id="018bf-583">`az appservice ase create`: Erstellungsproblem behoben (Nr. 13361)</span><span class="sxs-lookup"><span data-stu-id="018bf-583">`az appservice ase create`: Fix create issue #13361</span></span>
* <span data-ttu-id="018bf-584">`az appservice ase list-addresses`: SDK-Änderung korrigiert (Nr. 13140)</span><span class="sxs-lookup"><span data-stu-id="018bf-584">`az appservice ase list-addresses`: Fix change of SDK #13140.</span></span>
* <span data-ttu-id="018bf-585">Web-App-/Sloterstellung für Windows-Container korrigiert</span><span class="sxs-lookup"><span data-stu-id="018bf-585">Fix webapp/slot creation for Windows Containers</span></span>
* <span data-ttu-id="018bf-586">`az webapp auth update`: Optionaler Parameter zum Aktualisieren der Laufzeitversion hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-586">`az webapp auth update`: Add optional parameter to update runtime-version</span></span>
* <span data-ttu-id="018bf-587">Unterstützung für das Auflisten, Löschen, Genehmigen und Ablehnen der Verbindung mit privatem Endpunkt für eine Web-App in der CLI</span><span class="sxs-lookup"><span data-stu-id="018bf-587">Support list, delete, approve and reject private endpoint connection for webapp in CLI</span></span>
* <span data-ttu-id="018bf-588">Behebung Nr. 13888: Unterstützung für Static Web Apps hinzugefügt: Befehle zum Abrufen, Auflisten und Erstellen</span><span class="sxs-lookup"><span data-stu-id="018bf-588">Fix #13888 : Add support for Static WebApps: get, list, create commands</span></span>
* <span data-ttu-id="018bf-589">Fehlermeldungen für die SSH-Tunnelverbindung verbessert</span><span class="sxs-lookup"><span data-stu-id="018bf-589">Improved error messages for SSH Tunnel Connection</span></span>

### <a name="arm"></a><span data-ttu-id="018bf-590">ARM</span><span class="sxs-lookup"><span data-stu-id="018bf-590">ARM</span></span>

* <span data-ttu-id="018bf-591">`az tag`: Beispiele für „-h“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-591">`az tag`: Add examples for -h</span></span>
* <span data-ttu-id="018bf-592">`az deployment group/sub what-if`: Parameter „--exclude-change-types/-x“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-592">`az deployment group/sub what-if`: Add --exclude-change-types/-x parameter.</span></span>
* <span data-ttu-id="018bf-593">`az deployment group/sub/mg/tenant create`: Parameter „--what-if-exclude-change-types/-x“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-593">`az deployment group/sub/mg/tenant create`: Add --what-if-exclude-change-types/-x parameter.</span></span>
* <span data-ttu-id="018bf-594">`az deployment group/sub/mg/tenant validate`: Anzeigen von Fehlermeldungen in einem besseren Format</span><span class="sxs-lookup"><span data-stu-id="018bf-594">`az deployment group/sub/mg/tenant validate`: Show error messages in a better format.</span></span>
* <span data-ttu-id="018bf-595">`az group export`: Neue Parameter `--skip-resource-name-params` und `--skip-all-params` hinzugefügt, um das Überspringen der Parametrisierung zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="018bf-595">`az group export`: Add new parameters `--skip-resource-name-params` and `--skip-all-params` to support skip parameterization</span></span>
* <span data-ttu-id="018bf-596">API „az feature unregister“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-596">Add az feature unregister api</span></span>

### <a name="aro"></a><span data-ttu-id="018bf-597">ARO</span><span class="sxs-lookup"><span data-stu-id="018bf-597">ARO</span></span>

* <span data-ttu-id="018bf-598">„Public“/„Private“ zu Parametern zur Unterstützung bei Eingangs-/APIServer-Sichtbarkeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-598">Add Public, Private to params for help with ingress/apiserver visibility</span></span>

### <a name="batch"></a><span data-ttu-id="018bf-599">Batch</span><span class="sxs-lookup"><span data-stu-id="018bf-599">Batch</span></span>

* <span data-ttu-id="018bf-600">`az batch account create`: Neuer Parameter `--public-network-access` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-600">`az batch account create`: Add new parameter `--public-network-access`</span></span>
* <span data-ttu-id="018bf-601">`az batch account create`: Neuer Parameter `--identity-type` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-601">`az batch account create`: Add new parameter `--identity-type`</span></span>
* <span data-ttu-id="018bf-602">`az batch account set`: Neuer Parameter `--identity-type` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-602">`az batch account set`: Add new parameter `--identity-type`</span></span>
* <span data-ttu-id="018bf-603">[BREAKING CHANGE] az batch pool create: Bei der Erstellung eines Pools mithilfe eines benutzerdefinierten Images kann die Eigenschaft „--image“ nun ausschließlich auf ein Shared Image Gallery-Image verweisen.</span><span class="sxs-lookup"><span data-stu-id="018bf-603">[BREAKING CHANGE] az batch pool create: When creating a pool using a custom image, the --image property of can now only refer to a Shared Image Gallery image.</span></span>
* <span data-ttu-id="018bf-604">[BREAKING CHANGE] az batch pool create: Bei der Erstellung eines Pools mit der Option „--json-file“ und Angabe einer Netzwerkkonfiguration (networkConfiguration) wurde die Eigenschaft „publicIPs“ in die neue Eigenschaft „publicIPAddressConfiguration“ verschoben.</span><span class="sxs-lookup"><span data-stu-id="018bf-604">[BREAKING CHANGE] az batch pool create: When creating a pool with --json-file option and specifying a networkConfiguration, the publicIPs property has moved in to a new property publicIPAddressConfiguration.</span></span> <span data-ttu-id="018bf-605">Diese neue Eigenschaft unterstützt außerdem die neue Eigenschaft „ipAddressProvisioningType“. Diese gibt an, wie der Pool IP-Adressen und die Eigenschaft „publicIPs“ zuordnen muss, um die Konfiguration einer Liste mit PublicIP-Ressourcen zu ermöglichen, die bei der Festlegung von „ipAddressProvisioningType“ auf „UserManaged“ verwendet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="018bf-605">This new property also supports a new ipAddressProvisioningType property which specifies how the pool should allocate IP's and a publicIPs property which allows for configuration of a list of PublicIP resources to use in the case ipAddressProvisioningType is set to UserManaged</span></span>
* <span data-ttu-id="018bf-606">`az network private-link-resource`: Unterstützung für die Microsoft.Batch-Ressource „batchAccount“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-606">`az network private-link-resource`: Add support for the Microsoft.Batch batchAccount resource</span></span>
* <span data-ttu-id="018bf-607">`az network private-endpoint-connection`: Unterstützung für die Microsoft.Batch-Ressource „batchAccount“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-607">`az network private-endpoint-connection`: Add support for the Microsoft.Batch batchAccount resource</span></span>

### <a name="cdn"></a><span data-ttu-id="018bf-608">CDN</span><span class="sxs-lookup"><span data-stu-id="018bf-608">CDN</span></span>

* <span data-ttu-id="018bf-609">`az cdn custom-domain enable-https`: Unterstützung für BYOC hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-609">`az cdn custom-domain enable-https`: Add BYOC support.</span></span>
* <span data-ttu-id="018bf-610">`az cdn custom-domain enable-https`: Aktivierung von benutzerdefiniertem HTTPS mit CDN-verwalteten Zertifikaten für die SKUs Standard_Verizon und Standard_Microsoft korrigiert</span><span class="sxs-lookup"><span data-stu-id="018bf-610">`az cdn custom-domain enable-https`: Fix enabling custom HTTPS with CDN managed certificates for Standard_Verizon and Standard_Microsoft SKUs.</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="018bf-611">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="018bf-611">Cognitive Services</span></span>

* <span data-ttu-id="018bf-612">[BREAKING CHANGE] `az cognitiveservices account` besitzt nun eine einheitliche Struktur für alle Befehle.</span><span class="sxs-lookup"><span data-stu-id="018bf-612">[BREAKING CHANGE] `az cognitiveservices account` now have a unified structure for all commands.</span></span>
* <span data-ttu-id="018bf-613">`az cognitiveservices account identity`: Identitätsverwaltung für Cognitive Services hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-613">`az cognitiveservices account identity`: Add identity management for Cognitive Services.</span></span>

### <a name="compute"></a><span data-ttu-id="018bf-614">Compute</span><span class="sxs-lookup"><span data-stu-id="018bf-614">Compute</span></span>

* <span data-ttu-id="018bf-615">`az image builder`: API-Version auf 2020-02-14 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="018bf-615">`az image builder`: Upgrade API version to 2020-02-14</span></span>
* <span data-ttu-id="018bf-616">`az image builder create`: `--identity` zur Unterstützung der Identitätskonfiguration hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-616">`az image builder create`: Add `--identity` to support identity configuration</span></span>
* <span data-ttu-id="018bf-617">`az image builder customizer add`: Unterstützung für Windows Update-Anpassung</span><span class="sxs-lookup"><span data-stu-id="018bf-617">`az image builder customizer add`: Support Windows update customizer</span></span>
* <span data-ttu-id="018bf-618">Neuer Befehl `az image builder cancel`</span><span class="sxs-lookup"><span data-stu-id="018bf-618">New command `az image builder cancel`</span></span>
* <span data-ttu-id="018bf-619">Anzeigen einer Warnung, wenn ein Benutzer eine VMSS bereitstellt, die an eine bestimmte (und nicht an die neueste) Imageversion angeheftet ist</span><span class="sxs-lookup"><span data-stu-id="018bf-619">Show a warning when a user deploys a VMSS pinned to a specific image version rather than latest</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="018bf-620">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="018bf-620">Cosmos DB</span></span>

* <span data-ttu-id="018bf-621">`az cosmosdb`: Befehl „exists“ zu Datenbank- und Containergruppen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-621">`az cosmosdb`: Add exists command to database and container groups</span></span>
* <span data-ttu-id="018bf-622">Zulassen der Erstellung fester Sammlungen</span><span class="sxs-lookup"><span data-stu-id="018bf-622">Allow creating fixed collections</span></span>

### <a name="eventhub"></a><span data-ttu-id="018bf-623">EventHub</span><span class="sxs-lookup"><span data-stu-id="018bf-623">EventHub</span></span>

* <span data-ttu-id="018bf-624">`az eventhubs namespace create` : Parameter für verwaltete Identität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-624">`az eventhubs namespace create` : Add managed identity parameters</span></span>

### <a name="extension"></a><span data-ttu-id="018bf-625">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="018bf-625">Extension</span></span>

* <span data-ttu-id="018bf-626">„--version“ hinzugefügt, um die Installation über eine bestimmte Version zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="018bf-626">Add --version to support to install from a specific version</span></span>
* <span data-ttu-id="018bf-627">CLI-Erweiterungen dürfen nun Pakete im Namespace „azure“ enthalten.</span><span class="sxs-lookup"><span data-stu-id="018bf-627">Enable CLI extensions to include packages in the 'azure' namespace</span></span>

### <a name="iot-hub"></a><span data-ttu-id="018bf-628">IoT Hub</span><span class="sxs-lookup"><span data-stu-id="018bf-628">Iot Hub</span></span>

* <span data-ttu-id="018bf-629">[BREAKING CHANGE] az iot hub job: Veraltete job-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-629">[BREAKING CHANGE] az iot hub job: Remove deprecated job commands</span></span>

### <a name="keyvault"></a><span data-ttu-id="018bf-630">KeyVault</span><span class="sxs-lookup"><span data-stu-id="018bf-630">KeyVault</span></span>

* <span data-ttu-id="018bf-631">`az keyvault key import`: Unterstützt das Importieren aus Zeichenfolgen über zwei neue Parameter.</span><span class="sxs-lookup"><span data-stu-id="018bf-631">`az keyvault key import`: Supports importing from strings via two new parameters.</span></span>
* <span data-ttu-id="018bf-632">Unterstützung der Ver- und Entschlüsselung von Zeichenfolgen/Bytes mit gespeicherten Schlüsseln</span><span class="sxs-lookup"><span data-stu-id="018bf-632">Support string/bytes encryption and decryption with stored keys</span></span>

### <a name="monitor"></a><span data-ttu-id="018bf-633">Überwachen</span><span class="sxs-lookup"><span data-stu-id="018bf-633">Monitor</span></span>

* <span data-ttu-id="018bf-634">Unterstützung für „no wait“ bei der Clustererstellung</span><span class="sxs-lookup"><span data-stu-id="018bf-634">Support no wait for cluster creation</span></span>
* <span data-ttu-id="018bf-635">`az monitor log-analytics workspace saved-search`: Unterstützung neuer Befehle für gespeicherte Suche</span><span class="sxs-lookup"><span data-stu-id="018bf-635">`az monitor log-analytics workspace saved-search`: Support new commands for saved search</span></span>

### <a name="network"></a><span data-ttu-id="018bf-636">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="018bf-636">Network</span></span>

* <span data-ttu-id="018bf-637">`az network application-gateway address-pool update`: Hilfenachricht optimiert und Beispiele hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-637">`az network application-gateway address-pool update`: Refine help message and add examples.</span></span>
* <span data-ttu-id="018bf-638">`az network vnet create`: Unterstützung für das Argument „--nsg“</span><span class="sxs-lookup"><span data-stu-id="018bf-638">`az network vnet create`: Support --nsg argument</span></span>
* <span data-ttu-id="018bf-639">`az network lb address-pool`: Unterstützung für das Erstellen eines Back-End-Pools des Lastenausgleichs mit Back-End-Adresse</span><span class="sxs-lookup"><span data-stu-id="018bf-639">`az network lb address-pool`: Support create lb backend pool with backend address.</span></span>
* <span data-ttu-id="018bf-640">`az network application-gateway address-pool`: Korrektur für das Argument „--add“</span><span class="sxs-lookup"><span data-stu-id="018bf-640">`az network application-gateway address-pool`: Fix for --add argument</span></span>

### <a name="rbac"></a><span data-ttu-id="018bf-641">RBAC</span><span class="sxs-lookup"><span data-stu-id="018bf-641">RBAC</span></span>

* <span data-ttu-id="018bf-642">`az ad sp create-for-rabc`: Unterstützung von Namen mit Leerzeichen, Schrägstrich und umgekehrtem Schrägstrich</span><span class="sxs-lookup"><span data-stu-id="018bf-642">`az ad sp create-for-rabc`: Support name with space, slash and back slash</span></span>
* <span data-ttu-id="018bf-643">`az ad sp create-for-rbac`: Fehlermeldung optimiert, die angezeigt wird, wenn Benutzer einen ungültigen Bereich angeben</span><span class="sxs-lookup"><span data-stu-id="018bf-643">`az ad sp create-for-rbac`: Refine error message when user specify an invalid scope</span></span>

### <a name="security"></a><span data-ttu-id="018bf-644">Sicherheit</span><span class="sxs-lookup"><span data-stu-id="018bf-644">Security</span></span>

* <span data-ttu-id="018bf-645">Befehle für Sicherheitsbewertungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-645">Add security assessment commands</span></span>

### <a name="sql"></a><span data-ttu-id="018bf-646">SQL</span><span class="sxs-lookup"><span data-stu-id="018bf-646">SQL</span></span>

* <span data-ttu-id="018bf-647">`az sql db ltr-policy/ltr-backup`: Aktualisieren/Anzeigen der Richtlinie zur langfristigen Aufbewahrung, Anzeigen/Löschen von Sicherungen zur langfristigen Aufbewahrung, Wiederherstellen von Sicherungen zur langfristigen Aufbewahrung</span><span class="sxs-lookup"><span data-stu-id="018bf-647">`az sql db ltr-policy/ltr-backup`: update/show long term retention policy, show/delete long term retention backups, restore long term retention backup</span></span>

### <a name="storage"></a><span data-ttu-id="018bf-648">Storage</span><span class="sxs-lookup"><span data-stu-id="018bf-648">Storage</span></span>

* <span data-ttu-id="018bf-649">Authentifizierungsproblem behoben, um das Abrufen eines Tokens für „--subscription“ zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="018bf-649">Fix authentication issue to support get token for --subscription</span></span>
* <span data-ttu-id="018bf-650">`az storage remove`: Problem Nr. 13459 behoben, um eine Ausnahme bei einem Vorgangsfehler auszulösen</span><span class="sxs-lookup"><span data-stu-id="018bf-650">`az storage remove`: Fix issue #13459 to raise exception for operation failure</span></span>
* <span data-ttu-id="018bf-651">Probleme Nr. 13012, 13632 und 13657 behoben, um nicht verwendete Argumente für Befehle im Zusammenhang mit „generate-sas“ zu entfernen</span><span class="sxs-lookup"><span data-stu-id="018bf-651">Fix issues #13012, #13632 and #13657 to remove unused arguments for generate-sas related commands</span></span>
* <span data-ttu-id="018bf-652">`az storage logging update`: Überprüfung für Protokollierungsversion hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-652">`az storage logging update`: Add check for logging version</span></span>
* <span data-ttu-id="018bf-653">`az storage blob show`: Weitere Eigenschaften für Blob mit Track 2 SDK hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-653">`az storage blob show`: Add more properties for blob with track 2 SDK</span></span>
* <span data-ttu-id="018bf-654">Behebung Nr. 13708: Warnmeldung für Anmeldeinformationen optimiert</span><span class="sxs-lookup"><span data-stu-id="018bf-654">Fix #13708: Refine warning message for credential</span></span>
* <span data-ttu-id="018bf-655">`az storage share-rm create/update`: Unterstützung für NFS-Protokoll und Root-Squash hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-655">`az storage share-rm create/update`: Add NFS protocol and root squash support</span></span>
* <span data-ttu-id="018bf-656">`az storage account create`: Unterstützung für doppelte Verschlüsselung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-656">`az storage account create`: Add support for double encryption</span></span>
* <span data-ttu-id="018bf-657">[BREAKING CHANGE] `az storage blob/container/file/share/table/queue generate-sas`: „--expiry“ und „--permissions“ als erforderlich festgelegt</span><span class="sxs-lookup"><span data-stu-id="018bf-657">[BREAKING CHANGE] `az storage blob/container/file/share/table/queue generate-sas`: make --expiry and --permissions required</span></span>
* <span data-ttu-id="018bf-658">`az storage blob set-tier`: Migration zu Track 2, um das Festlegen der Aktivierungspriorität zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="018bf-658">`az storage blob set-tier`: Migrate to Track 2 to support setting rehydrate priority</span></span>

## <a name="june-02-2020"></a><span data-ttu-id="018bf-659">2\. Juni 2020</span><span class="sxs-lookup"><span data-stu-id="018bf-659">June 02, 2020</span></span>

<span data-ttu-id="018bf-660">Version 2.7.0</span><span class="sxs-lookup"><span data-stu-id="018bf-660">Version 2.7.0</span></span>

### <a name="acr"></a><span data-ttu-id="018bf-661">ACR</span><span class="sxs-lookup"><span data-stu-id="018bf-661">ACR</span></span>

* <span data-ttu-id="018bf-662">Tippfehler in einer Fehlermeldung der Tokenerstellung korrigiert</span><span class="sxs-lookup"><span data-stu-id="018bf-662">Fix a typo in an error message of token creation</span></span>

### <a name="aks"></a><span data-ttu-id="018bf-663">AKS</span><span class="sxs-lookup"><span data-stu-id="018bf-663">AKS</span></span>

* <span data-ttu-id="018bf-664">Standard-VM-SKU in „Standard_D2s_v3“ geändert</span><span class="sxs-lookup"><span data-stu-id="018bf-664">Change default vm sku to Standard_D2s_v3</span></span>
* <span data-ttu-id="018bf-665">Erstellung der Rollenzuweisung für MSI-Cluster plus benutzerdefiniertes Subnetz korrigiert</span><span class="sxs-lookup"><span data-stu-id="018bf-665">Fix creating role assignment for MSI clsuter plus custom subnet</span></span>

### <a name="appservice"></a><span data-ttu-id="018bf-666">AppService</span><span class="sxs-lookup"><span data-stu-id="018bf-666">AppService</span></span>

* <span data-ttu-id="018bf-667">Fehlerbehebung Nr. 12739: Von „az appservice list-locations“ werden einige ungültige Standorte zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="018bf-667">Fix #12739 az appservice list-locations returns some invalid locations</span></span>

### <a name="arm"></a><span data-ttu-id="018bf-668">ARM</span><span class="sxs-lookup"><span data-stu-id="018bf-668">ARM</span></span>

* <span data-ttu-id="018bf-669">`az deployment`: Fehlerbehebung Nr. 13159 der fehlerhaften JSON-Meldung nach dem Entfernen von Kommentaren und nach dem Komprimieren</span><span class="sxs-lookup"><span data-stu-id="018bf-669">`az deployment`: Fix issue #13159 of incorrect message of JSON after removing comments and compressing</span></span>
* <span data-ttu-id="018bf-670">`az resource tag`: Fehlerbehebung Nr. 13255 für das Markieren von Ressourcen mit dem Ressourcentyp `Microsoft.ContainerRegistry/registries/webhooks`</span><span class="sxs-lookup"><span data-stu-id="018bf-670">`az resource tag`: Fix issue #13255 of tagging resources with resource type `Microsoft.ContainerRegistry/registries/webhooks`</span></span>
* <span data-ttu-id="018bf-671">Beispiele für das Ressourcenmodul verbessert</span><span class="sxs-lookup"><span data-stu-id="018bf-671">Improve the examples for the resource module</span></span>

### <a name="aro"></a><span data-ttu-id="018bf-672">ARO</span><span class="sxs-lookup"><span data-stu-id="018bf-672">ARO</span></span>

* <span data-ttu-id="018bf-673">CLIError in das richtige Flag für „--worker-vm-disk-size-gb“ geändert</span><span class="sxs-lookup"><span data-stu-id="018bf-673">Change CLIError to correct flag for --worker-vm-disk-size-gb</span></span>

### <a name="eventhub"></a><span data-ttu-id="018bf-674">EventHub</span><span class="sxs-lookup"><span data-stu-id="018bf-674">EventHub</span></span>

* <span data-ttu-id="018bf-675">Fehlerbehebung Nr. 12406: „intervalInSeconds“ wird von Argument „--capture-interval“ nicht aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="018bf-675">Fix for issue #12406 Argument --capture-interval does not update the "intervalInSeconds"</span></span>

### <a name="hdinsight"></a><span data-ttu-id="018bf-676">HDInsight</span><span class="sxs-lookup"><span data-stu-id="018bf-676">HDInsight</span></span>

* <span data-ttu-id="018bf-677">„get_json_object“ in „shell_safe_json_parse“ geändert</span><span class="sxs-lookup"><span data-stu-id="018bf-677">Change get_json_object to shell_safe_json_parse</span></span>

### <a name="monitor"></a><span data-ttu-id="018bf-678">Überwachen</span><span class="sxs-lookup"><span data-stu-id="018bf-678">Monitor</span></span>

* <span data-ttu-id="018bf-679">`az monitor metrics alert`: Verschiedene Hilfemeldungen optimiert</span><span class="sxs-lookup"><span data-stu-id="018bf-679">`az monitor metrics alert`: refine several help messages</span></span>
* <span data-ttu-id="018bf-680">`az monitor diagnostic-settings create`: Unterstützung für das Argument „--export-to-resource-specific“</span><span class="sxs-lookup"><span data-stu-id="018bf-680">`az monitor diagnostic-settings create`: support --export-to-resource-specific argument</span></span>
* <span data-ttu-id="018bf-681">Unterstützung für die Wiederherstellung von LA-Arbeitsbereichen</span><span class="sxs-lookup"><span data-stu-id="018bf-681">Support LA workspace recover</span></span>

### <a name="network"></a><span data-ttu-id="018bf-682">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="018bf-682">Network</span></span>

* <span data-ttu-id="018bf-683">`az network dns zone`: Unterstützung des Bindestrichs (-)</span><span class="sxs-lookup"><span data-stu-id="018bf-683">`az network dns zone`: support - character</span></span>
* <span data-ttu-id="018bf-684">`az network vpn-connection ipsec-policy`: „--sa-lifetime“ und „--sa-max-size“ im Beispiel in höhere Werte geändert</span><span class="sxs-lookup"><span data-stu-id="018bf-684">`az network vpn-connection ipsec-policy`: change the --sa-lifetime and --sa-max-size to larger values in example</span></span>
* <span data-ttu-id="018bf-685">Netzwerk auf 2020-04-01 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="018bf-685">Bump network to 2020-04-01</span></span>
* <span data-ttu-id="018bf-686">`az network private-endpoint-connection`: Unterstützung von Event Grid</span><span class="sxs-lookup"><span data-stu-id="018bf-686">`az network private-endpoint-connection`: support event grid</span></span>
* <span data-ttu-id="018bf-687">`az network express-route list-route-tables`: Fehler behoben, der dazu führte, dass Routen nicht als Tabelle aufgeführt werden konnten</span><span class="sxs-lookup"><span data-stu-id="018bf-687">`az network express-route list-route-tables`: fix bug that cannot list routes as table</span></span>

### <a name="packaging"></a><span data-ttu-id="018bf-688">Verpackung</span><span class="sxs-lookup"><span data-stu-id="018bf-688">Packaging</span></span>

* <span data-ttu-id="018bf-689">Ubuntu-Paket (Focal) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-689">Add Ubuntu Focal Package</span></span>

### <a name="rbac"></a><span data-ttu-id="018bf-690">RBAC</span><span class="sxs-lookup"><span data-stu-id="018bf-690">RBAC</span></span>

* <span data-ttu-id="018bf-691">`az ad sp credential reset`: Erstellung von Anmeldeinformationen geändert, um problematische Sonderzeichen zu vermeiden</span><span class="sxs-lookup"><span data-stu-id="018bf-691">`az ad sp credential reset`: modify credential generation to avoid troublesome special characters</span></span>

### <a name="redis"></a><span data-ttu-id="018bf-692">Redis</span><span class="sxs-lookup"><span data-stu-id="018bf-692">Redis</span></span>

* <span data-ttu-id="018bf-693">Fehlerbehebung Nr. 13529: Dokumentation des Parameters „enable_non_ssl_port“ geändert</span><span class="sxs-lookup"><span data-stu-id="018bf-693">Fix #13529: Change documentation of parameter enable_non_ssl_port</span></span>

### <a name="storage"></a><span data-ttu-id="018bf-694">Storage</span><span class="sxs-lookup"><span data-stu-id="018bf-694">Storage</span></span>

* <span data-ttu-id="018bf-695">`az storage copy`: Parameter `--follow-symlinks` zur Unterstützung von symbolischen Verknüpfungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-695">`az storage copy`: Add parameter `--follow-symlinks` to support symlinks</span></span>
* <span data-ttu-id="018bf-696">Lokaler Kontext für Speicherkonto aktiviert</span><span class="sxs-lookup"><span data-stu-id="018bf-696">Enable local context for storage account</span></span>
* <span data-ttu-id="018bf-697">`az storage logging`: Fehlerbehebung Nr. 11969: Fehlermeldung optimiert</span><span class="sxs-lookup"><span data-stu-id="018bf-697">`az storage logging`: Fix issue #11969 to refine error message</span></span>

## <a name="may-19-2020"></a><span data-ttu-id="018bf-698">19. Mai 2020</span><span class="sxs-lookup"><span data-stu-id="018bf-698">May 19, 2020</span></span>

<span data-ttu-id="018bf-699">Version 2.6.0</span><span class="sxs-lookup"><span data-stu-id="018bf-699">Version 2.6.0</span></span>

### <a name="acr"></a><span data-ttu-id="018bf-700">ACR</span><span class="sxs-lookup"><span data-stu-id="018bf-700">ACR</span></span>

* <span data-ttu-id="018bf-701">Standardtimeout von fünf Minuten für jede an ACR gesendete Anforderung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-701">Add default timeout of 5 minutes for any requests to ACR</span></span>
* <span data-ttu-id="018bf-702">Unterstützung für das Deaktivieren des Zugriffs auf das öffentliche Netzwerk</span><span class="sxs-lookup"><span data-stu-id="018bf-702">Support disable public network access</span></span>
* <span data-ttu-id="018bf-703">`az acr token create`: Argument „--days“ verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="018bf-703">`az acr token create`: expose --days argument</span></span>
* <span data-ttu-id="018bf-704">`az acr import`: Akzeptiert Werte für das Argument „--source“, bei denen der Servername einen Anmeldenamen enthält (mittels clientseitiger Korrektur)</span><span class="sxs-lookup"><span data-stu-id="018bf-704">`az acr import`: accept --source argument values which contain login in server name through client end correction</span></span>

### <a name="acs"></a><span data-ttu-id="018bf-705">ACS</span><span class="sxs-lookup"><span data-stu-id="018bf-705">ACS</span></span>

* <span data-ttu-id="018bf-706">Fehlerbehebung: Felderbereinigung für Felder entfernt, die nicht mehr vorhanden sind</span><span class="sxs-lookup"><span data-stu-id="018bf-706">Bug fix: remove fields cleanup for fields that no longer exist</span></span>

### <a name="aks"></a><span data-ttu-id="018bf-707">AKS</span><span class="sxs-lookup"><span data-stu-id="018bf-707">AKS</span></span>

* <span data-ttu-id="018bf-708">Hilfekontext des Befehls „uptime-sla“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="018bf-708">Update uptime-sla command help context</span></span>
* <span data-ttu-id="018bf-709">Bereichsüberprüfung für die Aktualisierung der Mindestanzahl für die Autoskalierung entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-709">Remove range check for updating min count for autoscaler</span></span>
* <span data-ttu-id="018bf-710">Hotfix, der bewirkt, dass bei der CLI kein Fehler auftritt, wenn der Benutzer nur das Windows-Kennwort angibt</span><span class="sxs-lookup"><span data-stu-id="018bf-710">Fix that cli doe not fail when user only specifies Windows password</span></span>

### <a name="ams"></a><span data-ttu-id="018bf-711">AMS</span><span class="sxs-lookup"><span data-stu-id="018bf-711">AMS</span></span>

* <span data-ttu-id="018bf-712">`az ams transform create`: Funktion zum Erstellen einer Transformation mit einer FaceDetector-Voreinstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-712">`az ams transform create`: Add ability to create a transform with a FaceDetector preset</span></span>
* <span data-ttu-id="018bf-713">`az ams content-key-policy create` : Funktion zum Erstellen einer FairPlay-Inhaltsschlüsselrichtlinie mit einer Konfiguration für die Offlinemiete hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-713">`az ams content-key-policy create` : Add ability to create a FairPlay content key policy with an offline rental configuration</span></span>

### <a name="appconfig"></a><span data-ttu-id="018bf-714">AppConfig</span><span class="sxs-lookup"><span data-stu-id="018bf-714">AppConfig</span></span>

* <span data-ttu-id="018bf-715">Fehlerbehebung für die Schlüsselauflistungswerte mit Feldern</span><span class="sxs-lookup"><span data-stu-id="018bf-715">Bug fix for list key values with fields</span></span>

### <a name="appservice"></a><span data-ttu-id="018bf-716">AppService</span><span class="sxs-lookup"><span data-stu-id="018bf-716">AppService</span></span>

* <span data-ttu-id="018bf-717">`az functionapp create`: AzureWebJobsDashboard wird nur festgelegt, wenn AppInsights deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="018bf-717">`az functionapp create`: AzureWebJobsDashboard will only be set if AppInsights is disabled</span></span>
* <span data-ttu-id="018bf-718">Fehlerbehebung Nr. 10664: VNET-Integration – Standortüberprüfungsfehler und Fehlerbehebung Nr. 13257: Fehler bei „az webapp up“, wenn eine Ressourcengruppe erstellt werden muss</span><span class="sxs-lookup"><span data-stu-id="018bf-718">Fix #10664- VNet Integration - Location Check Issue & fix #13257- az webapp up failing when RG needs to be created</span></span>
* <span data-ttu-id="018bf-719">`az webapp|functionapp config ssl import`: Ressourcengruppenübergreifende Suche des Schlüsseltresors im Abonnement und verbesserte Hilfe und Beispiele</span><span class="sxs-lookup"><span data-stu-id="018bf-719">`az webapp|functionapp config ssl import`: Lookup key vault across resources groups in subscription and improve help and examples.</span></span>
* <span data-ttu-id="018bf-720">Lokaler Kontext für App Service integriert</span><span class="sxs-lookup"><span data-stu-id="018bf-720">Onboard local context for app service</span></span>

### <a name="arm"></a><span data-ttu-id="018bf-721">ARM</span><span class="sxs-lookup"><span data-stu-id="018bf-721">ARM</span></span>

* <span data-ttu-id="018bf-722">`az deployment`: Problem behoben, das dazu führte, dass templateLink beim Bereitstellen oder Überprüfen von „template-uri“ nicht zurückgegeben wurde</span><span class="sxs-lookup"><span data-stu-id="018bf-722">`az deployment`: Fix the problem that the templateLink will not be returned when deploying or validating template-uri</span></span>
* <span data-ttu-id="018bf-723">`az deployment`: Problem behoben, das dazu führte, dass speziell codierte Zeichen von der Bereitstellung/Überprüfung nicht unterstützt wurden</span><span class="sxs-lookup"><span data-stu-id="018bf-723">`az deployment`: Fix the problem that deployment/validate does not support specially encoded character</span></span>
* <span data-ttu-id="018bf-724">`az deployment sub/group what-if`: Arrayausrichtung und Fehlerbehandlung korrigiert</span><span class="sxs-lookup"><span data-stu-id="018bf-724">`az deployment sub/group what-if`: Fix array alignment and error handling</span></span>
* <span data-ttu-id="018bf-725">`az deployment operation`: Veraltete Informationen angepasst</span><span class="sxs-lookup"><span data-stu-id="018bf-725">`az deployment operation`: Modify the deprecate information</span></span>

### <a name="aro"></a><span data-ttu-id="018bf-726">ARO</span><span class="sxs-lookup"><span data-stu-id="018bf-726">ARO</span></span>

* <span data-ttu-id="018bf-727">Beispiele zu folgenden Befehlen hinzugefügt: az aro create, list, list-credentials, show, delete</span><span class="sxs-lookup"><span data-stu-id="018bf-727">Add examples to az aro create, list, list-credentials, show, delete</span></span>
* <span data-ttu-id="018bf-728">Funktion „generate_random_id“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-728">Add generate_random_id function</span></span>

### <a name="backup"></a><span data-ttu-id="018bf-729">Backup</span><span class="sxs-lookup"><span data-stu-id="018bf-729">Backup</span></span>

* <span data-ttu-id="018bf-730">FriendlyName im Befehl zum Aktivieren des Schutzes für AzureFileShare zulässig</span><span class="sxs-lookup"><span data-stu-id="018bf-730">Allow FriendlyName in enable protection for AzureFileShare command</span></span>
* <span data-ttu-id="018bf-731">Korrektur im IaasVM-Befehl „restore-disks“</span><span class="sxs-lookup"><span data-stu-id="018bf-731">Fix in IaasVM restore-disks Command</span></span>
* <span data-ttu-id="018bf-732">BackupManagementType „MAB“ zum Befehl zum Auflisten der Elemente hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-732">Add "MAB" BackupManagementType to item list command</span></span>
* <span data-ttu-id="018bf-733">Unterstützung für die Wiederholung des Richtlinienupdates für fehlerhafte Elemente hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-733">Add support for retrying policy update for failed items.</span></span>
* <span data-ttu-id="018bf-734">Funktion zum Fortsetzen des Schutzes für virtuelle Azure-Computer hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-734">Add Resume Protection functionality for Azure Virtual Machine</span></span>
* <span data-ttu-id="018bf-735">Unterstützung zum Angeben der Ressourcengruppe zum Speichern von instantRP beim Erstellen oder Ändern der Richtlinie hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-735">Add support to specify ResourceGroup for storing instantRP during Create or Modify Policy</span></span>

### <a name="ci"></a><span data-ttu-id="018bf-736">CI</span><span class="sxs-lookup"><span data-stu-id="018bf-736">CI</span></span>

* <span data-ttu-id="018bf-737">Unterstützung für flake8 3.8.0</span><span class="sxs-lookup"><span data-stu-id="018bf-737">Support flake8 3.8.0</span></span>

### <a name="compute"></a><span data-ttu-id="018bf-738">Compute</span><span class="sxs-lookup"><span data-stu-id="018bf-738">Compute</span></span>

* <span data-ttu-id="018bf-739">Neuer Befehl: az vm auto-shutdown</span><span class="sxs-lookup"><span data-stu-id="018bf-739">New command az vm auto-shutdown</span></span>
* <span data-ttu-id="018bf-740">`az vm list-skus`: Verhalten von „--zone“aktualisiert. Jetzt werden alle SKU-Typen zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="018bf-740">`az vm list-skus`: Update --zone behavior, return all type skus now</span></span>

### <a name="core"></a><span data-ttu-id="018bf-741">Core</span><span class="sxs-lookup"><span data-stu-id="018bf-741">Core</span></span>

* <span data-ttu-id="018bf-742">Aktivierungsstatus aus dem lokalen Kontext für globale Benutzerebene aktualisiert</span><span class="sxs-lookup"><span data-stu-id="018bf-742">Update local context on/off status to global user level</span></span>

### <a name="extension"></a><span data-ttu-id="018bf-743">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="018bf-743">Extension</span></span>

* <span data-ttu-id="018bf-744">`az extension add`: „--system“ hinzugefügt, um die Installation von Erweiterungen in einem Systempfad zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="018bf-744">`az extension add`: Add --system to enable installing extensions in a system path</span></span>
* <span data-ttu-id="018bf-745">Unterstützung für „.egg-info“ zum Speichern der Metadaten für die Radtyperweiterung</span><span class="sxs-lookup"><span data-stu-id="018bf-745">Support .egg-info to store wheel type extension metadata</span></span>

### <a name="iot"></a><span data-ttu-id="018bf-746">IoT</span><span class="sxs-lookup"><span data-stu-id="018bf-746">IoT</span></span>

* <span data-ttu-id="018bf-747">`az iot`: Nachricht des IoT-Befehlsmoduls mit dem Hinweis auf die Erweiterung für die erste Ausführung aktualisiert, sodass sie anstelle der veralteten ID die korrekte moderne ID (`azure-iot`) enthält</span><span class="sxs-lookup"><span data-stu-id="018bf-747">`az iot`: Update the IoT command module first run extension awareness message to the accurate, non-deprecated modern Id `azure-iot`.</span></span>

### <a name="iot-hub"></a><span data-ttu-id="018bf-748">IoT Hub</span><span class="sxs-lookup"><span data-stu-id="018bf-748">IoT Hub</span></span>

* <span data-ttu-id="018bf-749">Unterstützung für API- und Netzwerkisolationsbefehle für 2020-03-01</span><span class="sxs-lookup"><span data-stu-id="018bf-749">Support for 2020-03-01 API and Network Isolation commands</span></span>

### <a name="netappfiles"></a><span data-ttu-id="018bf-750">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="018bf-750">NetAppFiles</span></span>

* <span data-ttu-id="018bf-751">`az volume create`: „snapshot-id“ als Parameter zum Erstellen eines Volumes hinzugefügt. Ermöglicht Benutzern das Erstellen eines Volumes auf der Grundlage einer vorhandenen Momentaufnahme.</span><span class="sxs-lookup"><span data-stu-id="018bf-751">`az volume create`: Adds snapshot-id as a parameter to create volume this will allow users to create a volume from existing snapshot.</span></span>

### <a name="network"></a><span data-ttu-id="018bf-752">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="018bf-752">Network</span></span>

* <span data-ttu-id="018bf-753">TTL-Wert korrigiert, der für „dns add-record“ unbeabsichtigt geändert wurde</span><span class="sxs-lookup"><span data-stu-id="018bf-753">Fix ttl value changed unintended for dns add-record</span></span>
* <span data-ttu-id="018bf-754">`az network public-ip create`: Kunden über einen bevorstehenden Breaking Change informiert</span><span class="sxs-lookup"><span data-stu-id="018bf-754">`az network public-ip create`: Inform customers of a coming breaking change</span></span>
* <span data-ttu-id="018bf-755">Unterstützung von generischen Befehlen für Private Link-Szenario</span><span class="sxs-lookup"><span data-stu-id="018bf-755">Support generic commands for private link scenario</span></span>
* <span data-ttu-id="018bf-756">`az network private-endpoint-connection`: Unterstützung für MySQL-, Postgre- und MariaDB-Typen</span><span class="sxs-lookup"><span data-stu-id="018bf-756">`az network private-endpoint-connection`: Support mysql, postgre and mariadb types</span></span>
* <span data-ttu-id="018bf-757">`az network private-endpoint-connection`: Unterstützung von CosmosDB-Typen</span><span class="sxs-lookup"><span data-stu-id="018bf-757">`az network private-endpoint-connection`: Support cosmosdb types</span></span>
* <span data-ttu-id="018bf-758">`az network private-endpoint`: „--group-ids“ und Umleitung an „--group-id“ als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="018bf-758">`az network private-endpoint`: deprecate --group-ids and redirect to --group-id</span></span>

### <a name="output"></a><span data-ttu-id="018bf-759">Output</span><span class="sxs-lookup"><span data-stu-id="018bf-759">Output</span></span>

* <span data-ttu-id="018bf-760">Anzeigen der Updateanweisung bei der Suche, beim Feedback und in „--help“</span><span class="sxs-lookup"><span data-stu-id="018bf-760">Show update instruction in find, feedback and --help</span></span>

### <a name="packaging"></a><span data-ttu-id="018bf-761">Verpackung</span><span class="sxs-lookup"><span data-stu-id="018bf-761">Packaging</span></span>

* <span data-ttu-id="018bf-762">Erstellen von MSI-/Homebrew-Paketen mit Abhängigkeiten, die aus „requirements.txt“ aufgelöst werden</span><span class="sxs-lookup"><span data-stu-id="018bf-762">Build MSI/Homebrew packages with dependecies resolved from requirements.txt</span></span>

### <a name="rbac"></a><span data-ttu-id="018bf-763">RBAC</span><span class="sxs-lookup"><span data-stu-id="018bf-763">RBAC</span></span>

* <span data-ttu-id="018bf-764">`az ad sp credential reset`: Erstellung unsicherer Anmeldeinformationen korrigiert</span><span class="sxs-lookup"><span data-stu-id="018bf-764">`az ad sp credential reset`: fix weak credential generation</span></span>

### <a name="storage"></a><span data-ttu-id="018bf-765">Storage</span><span class="sxs-lookup"><span data-stu-id="018bf-765">Storage</span></span>

* <span data-ttu-id="018bf-766">`az storage account file-service-properties update/show`: Unterstützung für Dateieigenschaften für Speicherkonto hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-766">`az storage account file-service-properties update/show`: Add File Properties Support for Storage Account</span></span>
* <span data-ttu-id="018bf-767">`az storage container create`: Fehlerbehebung Nr. 13373 durch Hinzufügen eines Validierungssteuerelements für öffentlichen Zugriff</span><span class="sxs-lookup"><span data-stu-id="018bf-767">`az storage container create`: Fix #13373 by adding validator for public access</span></span>
* <span data-ttu-id="018bf-768">Unterstützung für ADLS Gen2 (track2) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-768">Add ADLS Gen2 track2 support</span></span>
* <span data-ttu-id="018bf-769">`az storage blob sync`: Unterstützung für `--connection-string`</span><span class="sxs-lookup"><span data-stu-id="018bf-769">`az storage blob sync`: Support `--connection-string`</span></span>
* <span data-ttu-id="018bf-770">`az storage blob sync`: Falsche Fehlermeldung korrigiert, die angezeigt wird, wenn der Installationsspeicherort von „azcopy“ nicht gefunden wird</span><span class="sxs-lookup"><span data-stu-id="018bf-770">`az storage blob sync`: Fix the incorrect error message when azcopy cannot find the installation location</span></span>

## <a name="april-30-2020"></a><span data-ttu-id="018bf-771">30. April 2020</span><span class="sxs-lookup"><span data-stu-id="018bf-771">April 30, 2020</span></span>

<span data-ttu-id="018bf-772">Version 2.5.1</span><span class="sxs-lookup"><span data-stu-id="018bf-772">Version 2.5.1</span></span>

### <a name="acr"></a><span data-ttu-id="018bf-773">ACR</span><span class="sxs-lookup"><span data-stu-id="018bf-773">ACR</span></span>

* <span data-ttu-id="018bf-774">`az acr check-health`: „DOCKER_PULL_ERROR“ unter Windows behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-774">`az acr check-health`: Fix "DOCKER_PULL_ERROR" on Windows</span></span>

### <a name="compute"></a><span data-ttu-id="018bf-775">Compute</span><span class="sxs-lookup"><span data-stu-id="018bf-775">Compute</span></span>

* <span data-ttu-id="018bf-776">`az vm list-ip-addresses`: Fehlerbehandlung</span><span class="sxs-lookup"><span data-stu-id="018bf-776">`az vm list-ip-addresses`: Error handling</span></span>
* <span data-ttu-id="018bf-777">Fehler behoben, der bei der VM-Erstellung auftrat, wenn „endpoint_vm_image_alias_doc“ im Cloudprofil nicht festgelegt war</span><span class="sxs-lookup"><span data-stu-id="018bf-777">Fix a bug of vm create if endpoint_vm_image_alias_doc is not set in cloud profile</span></span>
* <span data-ttu-id="018bf-778">`az vmss create`: „--os-disk-size-gb“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-778">`az vmss create`: Add --os-disk-size-gb</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="018bf-779">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="018bf-779">Cosmos DB</span></span>

* <span data-ttu-id="018bf-780">`az cosmosdb create/update`: Unterstützung für „--enable-public-network“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-780">`az cosmosdb create/update`: add --enable-public-network support</span></span>

### <a name="extension"></a><span data-ttu-id="018bf-781">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="018bf-781">Extension</span></span>

* <span data-ttu-id="018bf-782">Laden der falschen Metadaten für die Radtyperweiterung korrigiert</span><span class="sxs-lookup"><span data-stu-id="018bf-782">Fix loading wrong metadata for wheel type extension</span></span>

### <a name="packaging"></a><span data-ttu-id="018bf-783">Verpackung</span><span class="sxs-lookup"><span data-stu-id="018bf-783">Packaging</span></span>

* <span data-ttu-id="018bf-784">Az-Skript für Git Bash/Cygwin unter Windows hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-784">Add az script for Git Bash/Cygwin on Windows</span></span>

### <a name="sql"></a><span data-ttu-id="018bf-785">SQL</span><span class="sxs-lookup"><span data-stu-id="018bf-785">SQL</span></span>

* <span data-ttu-id="018bf-786">`az sql instance-pool`: Befehlsgruppe für Instanzpools hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-786">`az sql instance-pool`: Add instance pools command group</span></span>

### <a name="storage"></a><span data-ttu-id="018bf-787">Storage</span><span class="sxs-lookup"><span data-stu-id="018bf-787">Storage</span></span>

* <span data-ttu-id="018bf-788">Paket „azure-multiapi-storage“ auf 0.3.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="018bf-788">Upgrade package azure-multiapi-storage to 0.3.0</span></span>
* <span data-ttu-id="018bf-789">Unterstützung von GZRS für Speicherkontoerstellung und -aktualisierung</span><span class="sxs-lookup"><span data-stu-id="018bf-789">Support GZRS for storage account creation and update</span></span>
* <span data-ttu-id="018bf-790">`az storage account failover`: Unterstützung für das Failover von GRS/GZRS-Speicherkonten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-790">`az storage account failover`: Add support for grs/gzrs storage account failover</span></span>
* <span data-ttu-id="018bf-791">`az storage blob upload`: Parameter „--encryption-scope“ hinzugefügt, um die Angabe von Informationen zum Verschlüsselungsbereich zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="018bf-791">`az storage blob upload`: Add --encryption-scope parameter to support specifying encryption scope information</span></span>

## <a name="april-28-2020"></a><span data-ttu-id="018bf-792">28. April 2020</span><span class="sxs-lookup"><span data-stu-id="018bf-792">April 28, 2020</span></span>

<span data-ttu-id="018bf-793">Version 2.5.0</span><span class="sxs-lookup"><span data-stu-id="018bf-793">Version 2.5.0</span></span>

### <a name="acs"></a><span data-ttu-id="018bf-794">ACS</span><span class="sxs-lookup"><span data-stu-id="018bf-794">ACS</span></span>

* <span data-ttu-id="018bf-795">[BREAKING CHANGE] az openshift create: Parameter „--vnet-peer“ entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-795">[BREAKING CHANGE] az openshift create: remove --vnet-peer parameter.</span></span>
* <span data-ttu-id="018bf-796">`az openshift create`: Flags zur Unterstützung des privaten Clusters hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-796">`az openshift create`: add flags to support private cluster.</span></span>
* <span data-ttu-id="018bf-797">`az openshift`: Upgrade auf API-Version `2019-10-27-preview`</span><span class="sxs-lookup"><span data-stu-id="018bf-797">`az openshift`: upgrade to `2019-10-27-preview` API version.</span></span>
* <span data-ttu-id="018bf-798">`az openshift`: Befehl `update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-798">`az openshift`: add `update` command.</span></span>

### <a name="aks"></a><span data-ttu-id="018bf-799">AKS</span><span class="sxs-lookup"><span data-stu-id="018bf-799">AKS</span></span>

* <span data-ttu-id="018bf-800">`az aks create`: Unterstützung für Windows hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-800">`az aks create`: Add support for Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="018bf-801">AppService</span><span class="sxs-lookup"><span data-stu-id="018bf-801">AppService</span></span>

* <span data-ttu-id="018bf-802">`az webapp deployment source config-zip`: Energiesparmodus nach „request.get()“ entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-802">`az webapp deployment source config-zip`: remove sleep after request.get()</span></span>

### <a name="arm"></a><span data-ttu-id="018bf-803">ARM</span><span class="sxs-lookup"><span data-stu-id="018bf-803">ARM</span></span>

* <span data-ttu-id="018bf-804">Was-wäre-wenn-Befehle für Vorlagenbereitstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-804">Add template deployment What-If commands</span></span>

### <a name="aro"></a><span data-ttu-id="018bf-805">ARO</span><span class="sxs-lookup"><span data-stu-id="018bf-805">ARO</span></span>

* <span data-ttu-id="018bf-806">`az aro`: Tabellenausgabe korrigiert</span><span class="sxs-lookup"><span data-stu-id="018bf-806">`az aro`: Fix table output</span></span>

### <a name="ci"></a><span data-ttu-id="018bf-807">CI</span><span class="sxs-lookup"><span data-stu-id="018bf-807">CI</span></span>

* <span data-ttu-id="018bf-808">pytest integriert und nose für Automatisierungstest als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="018bf-808">Onboard pytest and deprecate nose for Automation Test</span></span>

### <a name="compute"></a><span data-ttu-id="018bf-809">Compute</span><span class="sxs-lookup"><span data-stu-id="018bf-809">Compute</span></span>

* <span data-ttu-id="018bf-810">`az vmss disk detach`: Datenträgerfehler „NoneType“ behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-810">`az vmss disk detach`: fix data disk NoneType issue</span></span>
* <span data-ttu-id="018bf-811">`az vm availability-set list`: Unterstützung zum Anzeigen der VM-Liste</span><span class="sxs-lookup"><span data-stu-id="018bf-811">`az vm availability-set list`: Support showing VM list</span></span>
* <span data-ttu-id="018bf-812">`az vm list-skus`: Anzeigeproblem des Tabellenformats behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-812">`az vm list-skus`: Fix display problem of table format</span></span>

### <a name="keyvault"></a><span data-ttu-id="018bf-813">KeyVault</span><span class="sxs-lookup"><span data-stu-id="018bf-813">KeyVault</span></span>

* <span data-ttu-id="018bf-814">Neuer Parameter `--enable-rbac-authorization` bei Erstellung oder Aktualisierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-814">Add new parameter `--enable-rbac-authorization` during creating or updating</span></span>

### <a name="monitor"></a><span data-ttu-id="018bf-815">Überwachen</span><span class="sxs-lookup"><span data-stu-id="018bf-815">Monitor</span></span>

* <span data-ttu-id="018bf-816">Unterstützung der CMK-Features für LA-Cluster</span><span class="sxs-lookup"><span data-stu-id="018bf-816">Support LA cluster CMK features</span></span>
* <span data-ttu-id="018bf-817">`az monitor log-analytics workspace linked-storage`: Unterstützung für BYOS-Features</span><span class="sxs-lookup"><span data-stu-id="018bf-817">`az monitor log-analytics workspace linked-storage`: supports BYOS features</span></span>

### <a name="network"></a><span data-ttu-id="018bf-818">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="018bf-818">Network</span></span>

* <span data-ttu-id="018bf-819">`az network security-partner`: Unterstützung des Sicherheitspartneranbieters</span><span class="sxs-lookup"><span data-stu-id="018bf-819">`az network security-partner`: support security partner provider</span></span>

### <a name="privatedns"></a><span data-ttu-id="018bf-820">PrivateDNS</span><span class="sxs-lookup"><span data-stu-id="018bf-820">Privatedns</span></span>

* <span data-ttu-id="018bf-821">Funktion in privater DNS-Zone zum Importieren der Exportzonendatei hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-821">Add feature in private DNS zone to import export zone file</span></span>

## <a name="april-21-2020"></a><span data-ttu-id="018bf-822">21. April 2020</span><span class="sxs-lookup"><span data-stu-id="018bf-822">April 21, 2020</span></span>

<span data-ttu-id="018bf-823">Version 2.4.0</span><span class="sxs-lookup"><span data-stu-id="018bf-823">Version 2.4.0</span></span>

### <a name="acr"></a><span data-ttu-id="018bf-824">ACR</span><span class="sxs-lookup"><span data-stu-id="018bf-824">ACR</span></span>

* <span data-ttu-id="018bf-825">`az acr run --cmd`: Deaktivieren der Arbeitsverzeichnisaußerkraftsetzung</span><span class="sxs-lookup"><span data-stu-id="018bf-825">`az acr run --cmd`: disable working directory override</span></span>
* <span data-ttu-id="018bf-826">Unterstützung dedizierter Datenendpunkte</span><span class="sxs-lookup"><span data-stu-id="018bf-826">Support dedicated data endpoint</span></span>

### <a name="aks"></a><span data-ttu-id="018bf-827">AKS</span><span class="sxs-lookup"><span data-stu-id="018bf-827">AKS</span></span>

* <span data-ttu-id="018bf-828">`az aks list -o table` sollte „privateFqdn“ als FQDN für private Cluster anzeigen</span><span class="sxs-lookup"><span data-stu-id="018bf-828">`az aks list -o table` should show privateFqdn as fqdn for private clusters</span></span>
* <span data-ttu-id="018bf-829">„--uptime-sla“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-829">Add --uptime-sla</span></span>
* <span data-ttu-id="018bf-830">containerservice-Paket aktualisiert</span><span class="sxs-lookup"><span data-stu-id="018bf-830">Update containerservice package</span></span>
* <span data-ttu-id="018bf-831">Unterstützung für öffentliche IP-Adressen für Knoten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-831">Add node public IP support</span></span>
* <span data-ttu-id="018bf-832">Tippfehler im help-Befehl korrigiert</span><span class="sxs-lookup"><span data-stu-id="018bf-832">Fix typo in the help command</span></span>

### <a name="appconfig"></a><span data-ttu-id="018bf-833">AppConfig</span><span class="sxs-lookup"><span data-stu-id="018bf-833">AppConfig</span></span>

* <span data-ttu-id="018bf-834">Schlüsseltresorverweis für die Befehle „kv list“ und „kv export“ aufgelöst</span><span class="sxs-lookup"><span data-stu-id="018bf-834">Resolve key vault reference for kv list and export commands</span></span>
* <span data-ttu-id="018bf-835">Fehlerbehebung für die Werte für das Auflisten von Schlüsseln</span><span class="sxs-lookup"><span data-stu-id="018bf-835">Bug fix for list key values</span></span>

### <a name="appservice"></a><span data-ttu-id="018bf-836">AppService</span><span class="sxs-lookup"><span data-stu-id="018bf-836">AppService</span></span>

* <span data-ttu-id="018bf-837">`az functionapp create`: Vorgehensweise zum Festlegen von „linuxFxVersion“ für Linux-Funktions-Apps (.NET) geändert.</span><span class="sxs-lookup"><span data-stu-id="018bf-837">`az functionapp create`: Changed the way linuxFxVersion was being set for dotnet linux function apps.</span></span> <span data-ttu-id="018bf-838">Dadurch sollte der Fehler behoben sein, der die Erstellung von Linux-Verbrauchs-Apps (.NET) verhindert hat.</span><span class="sxs-lookup"><span data-stu-id="018bf-838">This should fix a bug that was preventing dotnet linux consumption apps from being created</span></span>
* <span data-ttu-id="018bf-839">[BREAKING CHANGE] `az webapp create`: Korrektur vorgenommen, um vorhandene App-Einstellungen (AppSettings) für „az webapp create“ beizubehalten</span><span class="sxs-lookup"><span data-stu-id="018bf-839">[BREAKING CHANGE] `az webapp create`: fix to keep existing AppSettings with az webapp create</span></span>
* <span data-ttu-id="018bf-840">[BREAKING CHANGE] `az webapp up`: Korrektur vorgenommen, um bei Verwendung des Flags „-g“ eine RG für den Befehl „az webapp up“ zu erstellen</span><span class="sxs-lookup"><span data-stu-id="018bf-840">[BREAKING CHANGE] `az webapp up`: fix to create RG for az webapp up command when using -g flag</span></span>
* <span data-ttu-id="018bf-841">[BREAKING CHANGE] `az webapp config`: Korrektur vorgenommen, um Werte für Nicht-JSON-Ausgaben mit „az webapp config connection-string list“ anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="018bf-841">[BREAKING CHANGE] `az webapp config`: fix to show values for non-JSON output with az webapp config connection-string list</span></span>

### <a name="arm"></a><span data-ttu-id="018bf-842">ARM</span><span class="sxs-lookup"><span data-stu-id="018bf-842">ARM</span></span>

* <span data-ttu-id="018bf-843">`az deployment create/validate`: Parameter `--no-prompt` hinzugefügt, um das Überspringen der Eingabeaufforderung für fehlende Parameter für die ARM-Vorlage zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="018bf-843">`az deployment create/validate`: Add parameter `--no-prompt` to support skipping the prompt of missing parameters for ARM template</span></span>
* <span data-ttu-id="018bf-844">`az deployment group/mg/sub/tenant validate`: Unterstützung von Kommentaren in der Bereitstellungsparameterdatei</span><span class="sxs-lookup"><span data-stu-id="018bf-844">`az deployment group/mg/sub/tenant validate`: Support comments in deployment parameter file</span></span>
* <span data-ttu-id="018bf-845">`az deployment`: `is_preview` für Parameter `--handle-extended-json-format` entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-845">`az deployment`: Remove `is_preview` for parameter `--handle-extended-json-format`</span></span>
* <span data-ttu-id="018bf-846">`az deployment group/mg/sub/tenant cancel`: Unterstützung für den Abbruch der Bereitstellung für ARM-Vorlagen</span><span class="sxs-lookup"><span data-stu-id="018bf-846">`az deployment group/mg/sub/tenant cancel`: Support cancel deployment for ARM template</span></span>
* <span data-ttu-id="018bf-847">`az deployment group/mg/sub/tenant validate`: Fehlermeldung bei einem Fehler der Bereitstellungsüberprüfung verbessert</span><span class="sxs-lookup"><span data-stu-id="018bf-847">`az deployment group/mg/sub/tenant validate`: Improve the error message when deployment verification fails</span></span>
* <span data-ttu-id="018bf-848">`az deployment-scripts`: Neue Befehle für DeploymentScripts hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-848">`az deployment-scripts`: Add new commands for DeploymentScripts</span></span>
* <span data-ttu-id="018bf-849">`az resource tag`: Parameter `--is-incremental` hinzugefügt, um das inkrementelle Hinzufügen von Tags zur Ressource zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="018bf-849">`az resource tag`: Add parameter `--is-incremental` to support adding tags to resource incrementally</span></span>

### <a name="aro"></a><span data-ttu-id="018bf-850">ARO</span><span class="sxs-lookup"><span data-stu-id="018bf-850">ARO</span></span>

* <span data-ttu-id="018bf-851">`az aro`:  ARO-Befehlsmodul von Azure RedHat OpenShift V4 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-851">`az aro`:  Add Azure RedHat OpenShift V4 aro command module</span></span>

### <a name="batch"></a><span data-ttu-id="018bf-852">Batch</span><span class="sxs-lookup"><span data-stu-id="018bf-852">Batch</span></span>

* <span data-ttu-id="018bf-853">Batch-API aktualisiert</span><span class="sxs-lookup"><span data-stu-id="018bf-853">Update Batch API</span></span>

### <a name="compute"></a><span data-ttu-id="018bf-854">Compute</span><span class="sxs-lookup"><span data-stu-id="018bf-854">Compute</span></span>

* <span data-ttu-id="018bf-855">`az sig image-version create`: Speicherkontotyp „Premium_LRS“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-855">`az sig image-version create`: Add storage account type Premium_LRS</span></span>
* <span data-ttu-id="018bf-856">`az vmss update`: Problem behoben, das beim Aktualisieren der Beendigungsbenachrichtigung auftrat</span><span class="sxs-lookup"><span data-stu-id="018bf-856">`az vmss update`: Fix terminate notification update issue</span></span>
* <span data-ttu-id="018bf-857">`az vm/vmss create`: Unterstützung für spezialisierte Imageversion hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-857">`az vm/vmss create`: Add support for specialized image version</span></span>
* <span data-ttu-id="018bf-858">SIG-API-Version 2019-12-01</span><span class="sxs-lookup"><span data-stu-id="018bf-858">SIG API Version 2019-12-01</span></span>
* <span data-ttu-id="018bf-859">`az sig image-version create`: „--target-region-encryption“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-859">`az sig image-version create`: Add --target-region-encryption</span></span>
* <span data-ttu-id="018bf-860">Fehler bei Serientestausführung behoben, der auf die Duplizierung des Schlüsseltresornamens im globalen In-Memory-Cache zurückzuführen war.</span><span class="sxs-lookup"><span data-stu-id="018bf-860">Fix tests fail when running in serial due to keyvault name is duplicated in global in-momery cache</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="018bf-861">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="018bf-861">CosmosDB</span></span>

* <span data-ttu-id="018bf-862">Unterstützung für `az cosmosdb private-link-resource/private-endpoint-connection`</span><span class="sxs-lookup"><span data-stu-id="018bf-862">Support `az cosmosdb private-link-resource/private-endpoint-connection`</span></span>

### <a name="iot-central"></a><span data-ttu-id="018bf-863">IoT Central</span><span class="sxs-lookup"><span data-stu-id="018bf-863">IoT Central</span></span>

* <span data-ttu-id="018bf-864">`az iotcentral` als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="018bf-864">Deprecate `az iotcentral`</span></span>
* <span data-ttu-id="018bf-865">Befehlsmodul `az iot central` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-865">Add `az iot central` command module</span></span>

### <a name="monitor"></a><span data-ttu-id="018bf-866">Überwachen</span><span class="sxs-lookup"><span data-stu-id="018bf-866">Monitor</span></span>

* <span data-ttu-id="018bf-867">Unterstützung eines Private Link-Szenarios für die Überwachung</span><span class="sxs-lookup"><span data-stu-id="018bf-867">Support private link scenario for monitor</span></span>
* <span data-ttu-id="018bf-868">Falsche Simulationsmethode in „test_monitor_general_operations.py“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="018bf-868">Fix wrong mocking way in test_monitor_general_operations.py</span></span>

### <a name="network"></a><span data-ttu-id="018bf-869">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="018bf-869">Network</span></span>

* <span data-ttu-id="018bf-870">SKU für den Befehl zur Aktualisierung der öffentlichen IP-Adresse als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="018bf-870">Deprecate sku for public ip update command</span></span>
* <span data-ttu-id="018bf-871">`az network private-endpoint`: Unterstützung für private DNS-Zonengruppe</span><span class="sxs-lookup"><span data-stu-id="018bf-871">`az network private-endpoint`: Support private dns zone group</span></span>
* <span data-ttu-id="018bf-872">Feature für lokalen Kontext für VNET-/Subnetzparameter aktiviert</span><span class="sxs-lookup"><span data-stu-id="018bf-872">Enable local context feature for vnet/subnet parameter</span></span>
* <span data-ttu-id="018bf-873">Falsches Verwendungsbeispiel in „test_nw_flow_log_delete“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="018bf-873">Fix wrong usage example in test_nw_flow_log_delete</span></span>

### <a name="packaging"></a><span data-ttu-id="018bf-874">Verpackung</span><span class="sxs-lookup"><span data-stu-id="018bf-874">Packaging</span></span>

* <span data-ttu-id="018bf-875">Unterstützung für Ubuntu-/Disco-Paket eingestellt</span><span class="sxs-lookup"><span data-stu-id="018bf-875">Drop support for Ubuntu/Disco package</span></span>

### <a name="rbac"></a><span data-ttu-id="018bf-876">RBAC</span><span class="sxs-lookup"><span data-stu-id="018bf-876">RBAC</span></span>

* <span data-ttu-id="018bf-877">`az ad app create/update`: Unterstützung von „--optional-claims“ als Parameter</span><span class="sxs-lookup"><span data-stu-id="018bf-877">`az ad app create/update`: support --optional-claims as a parameter</span></span>

### <a name="rdbms"></a><span data-ttu-id="018bf-878">RDBMS</span><span class="sxs-lookup"><span data-stu-id="018bf-878">RDBMS</span></span>

* <span data-ttu-id="018bf-879">Azure Active Directory-Administratorbefehle für PostgreSQL und MySQL hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-879">Add Azure active directory administrator commands for PostgreSQL and MySQL</span></span>

### <a name="service-fabric"></a><span data-ttu-id="018bf-880">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="018bf-880">Service Fabric</span></span>

* <span data-ttu-id="018bf-881">Fehlerbehebung Nr. 12891: `az sf application update --application-parameters` entfernt alte Parameter, die nicht in der Anforderung enthalten sind.</span><span class="sxs-lookup"><span data-stu-id="018bf-881">Fix #12891: `az sf application update --application-parameters` removes old parameters that are not in the request</span></span>
* <span data-ttu-id="018bf-882">Fehlerbehebung Nr. 12470: az sf create cluster: Fehler im Zusammenhang mit der Dauerhaftigkeit und Zuverlässigkeit von Updates sowie im Zusammenhang mit der codebasierten Suche der VMSS unter Angabe eines bestimmten Knotentypnamens behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-882">Fix #12470 az sf create cluster, fix bugs in update durability and reliability and find vmss correctly through the code given a node type name</span></span>

### <a name="sql"></a><span data-ttu-id="018bf-883">SQL</span><span class="sxs-lookup"><span data-stu-id="018bf-883">SQL</span></span>

* <span data-ttu-id="018bf-884">`az sql mi op list`, `az sql mi op get`, `az sql mi op cancel` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-884">Add `az sql mi op list`, `az sql mi op get`, `az sql mi op cancel`</span></span>
* <span data-ttu-id="018bf-885">`az sql midb`: Aktualisieren/Anzeigen der Richtlinie zur langfristigen Aufbewahrung, Anzeigen/Löschen von Sicherungen zur langfristigen Aufbewahrung, Wiederherstellen von Sicherungen zur langfristigen Aufbewahrung</span><span class="sxs-lookup"><span data-stu-id="018bf-885">`az sql midb`: update/show long term retention policy,  show/delete long term retention backups, restore long term retention backup</span></span>

### <a name="storage"></a><span data-ttu-id="018bf-886">Storage</span><span class="sxs-lookup"><span data-stu-id="018bf-886">Storage</span></span>

* <span data-ttu-id="018bf-887">„azure-mgmt-storage“ auf 9.0.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="018bf-887">Upgrade azure-mgmt-storage to 9.0.0</span></span>
* <span data-ttu-id="018bf-888">`az storage logging off`: Unterstützung für das Ausschalten der Protokollierung für ein Speicherkonto</span><span class="sxs-lookup"><span data-stu-id="018bf-888">`az storage logging off`: Support turning off logging for a storage account</span></span>
* <span data-ttu-id="018bf-889">`az storage account update`: Automatische Rotation von Schlüsseln für CMK aktiviert</span><span class="sxs-lookup"><span data-stu-id="018bf-889">`az storage account update`: Enable key auto-rotated for CMK</span></span>
* <span data-ttu-id="018bf-890">`az storage account encryption-scope create/update/list/show`: Unterstützung zum Anpassen des Verschlüsselungsbereichs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-890">`az storage account encryption-scope create/update/list/show`: Add support to customize encryption scope</span></span>
* <span data-ttu-id="018bf-891">`az storage container create`: „--default-encryption-scope“ und „--deny-encryption-scope-override“ hinzugefügt, um den Verschlüsselungsbereich für die Containerebene festzulegen</span><span class="sxs-lookup"><span data-stu-id="018bf-891">`az storage container create`: Add --default-encryption-scope and --deny-encryption-scope-override to set encryption scope for container level</span></span>

### <a name="survey"></a><span data-ttu-id="018bf-892">Umfrage</span><span class="sxs-lookup"><span data-stu-id="018bf-892">Survey</span></span>

* <span data-ttu-id="018bf-893">Switch zum Deaktivieren des Umfragelinks hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-893">Add switch to turn off survey link</span></span>

## <a name="april-01-2020"></a><span data-ttu-id="018bf-894">01. April 2020</span><span class="sxs-lookup"><span data-stu-id="018bf-894">April 01, 2020</span></span>

<span data-ttu-id="018bf-895">Version 2.3.1</span><span class="sxs-lookup"><span data-stu-id="018bf-895">Version 2.3.1</span></span>

### <a name="acr"></a><span data-ttu-id="018bf-896">ACR</span><span class="sxs-lookup"><span data-stu-id="018bf-896">ACR</span></span>

* <span data-ttu-id="018bf-897">Falsche Version von „azure-mgmt-containerregistry“ für Linux korrigiert</span><span class="sxs-lookup"><span data-stu-id="018bf-897">Fix wrong version of azure-mgmt-containerregistry for Linux</span></span>

### <a name="profile"></a><span data-ttu-id="018bf-898">Profil</span><span class="sxs-lookup"><span data-stu-id="018bf-898">Profile</span></span>

* <span data-ttu-id="018bf-899">az login: Anmeldefehler behoben, der auftrat, wenn nicht das Cloudprofil `latest` verwendet wurde</span><span class="sxs-lookup"><span data-stu-id="018bf-899">az login: Fix login failure with cloud profiles other than `latest`</span></span>

## <a name="march-31-2020"></a><span data-ttu-id="018bf-900">31. März 2020</span><span class="sxs-lookup"><span data-stu-id="018bf-900">March 31, 2020</span></span>

<span data-ttu-id="018bf-901">Version 2.3.0</span><span class="sxs-lookup"><span data-stu-id="018bf-901">Version 2.3.0</span></span>

### <a name="acr"></a><span data-ttu-id="018bf-902">ACR</span><span class="sxs-lookup"><span data-stu-id="018bf-902">ACR</span></span>

* <span data-ttu-id="018bf-903">„az acr task update“: NULL-Zeiger-Ausnahme</span><span class="sxs-lookup"><span data-stu-id="018bf-903">'az acr task update': null pointer exception</span></span>
* <span data-ttu-id="018bf-904">`az acr import`: Hilfe und Fehlermeldung geändert, um die Verwendung von „--source“ und „--registry“ zu verdeutlichen</span><span class="sxs-lookup"><span data-stu-id="018bf-904">`az acr import`: Modify help and error message to clarify the usage of --source and --registry</span></span>
* <span data-ttu-id="018bf-905">Überprüfung für das Argument „registry_name“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-905">Add a validator for argument 'registry_name'</span></span>
* <span data-ttu-id="018bf-906">`az acr login`: Vorschauflag für „--expose-token“ entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-906">`az acr login`:Remove the preview flag on '--expose-token'</span></span>
* <span data-ttu-id="018bf-907">[BREAKING CHANGE] Branch-Parameter „az acr task create/update“ entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-907">[BREAKING CHANGE] 'az acr task create/update' Branch parameter is removed</span></span>
* <span data-ttu-id="018bf-908">„az acr task update“: Kunde kann nun Kontext, Git-Token und/oder Trigger einzeln aktualisieren</span><span class="sxs-lookup"><span data-stu-id="018bf-908">'az acr task update' Customer now can update context, git-token, and or triggers individually</span></span>
* <span data-ttu-id="018bf-909">„az acr agentpool“: Neues Feature</span><span class="sxs-lookup"><span data-stu-id="018bf-909">'az acr agentpool': new feature</span></span>

### <a name="aks"></a><span data-ttu-id="018bf-910">AKS</span><span class="sxs-lookup"><span data-stu-id="018bf-910">AKS</span></span>

* <span data-ttu-id="018bf-911">„apiServerAccessProfile“ bei der Aktualisierung von „--api-server-authorized-ip-ranges“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="018bf-911">Fix apiServerAccessProfile when updating --api-server-authorized-ip-ranges</span></span>
* <span data-ttu-id="018bf-912">aks update: Überschreibung ausgehender IP-Adressen mit Eingabewerten bei der Aktualisierung</span><span class="sxs-lookup"><span data-stu-id="018bf-912">aks update: Override outbound IPs with input values when update</span></span>
* <span data-ttu-id="018bf-913">Keine SPN-Erstellung für MSI-Cluster sowie Unterstützung der Anfügung von ACR an MSI-Cluster</span><span class="sxs-lookup"><span data-stu-id="018bf-913">Do not create SPN for MSI clusters and support attach acr to MSI clusters</span></span>

### <a name="ams"></a><span data-ttu-id="018bf-914">AMS</span><span class="sxs-lookup"><span data-stu-id="018bf-914">AMS</span></span>

* <span data-ttu-id="018bf-915">Fix 12469: Hinzufügen von „content-key-policy“ für Fairplay aufgrund von Problemen mit dem Parameter „ask“ nicht erfolgreich</span><span class="sxs-lookup"><span data-stu-id="018bf-915">Fix #12469: adding Fairplay content-key-policy fails due to problems with 'ask' parameter</span></span>

### <a name="appconfig"></a><span data-ttu-id="018bf-916">AppConfig</span><span class="sxs-lookup"><span data-stu-id="018bf-916">AppConfig</span></span>

* <span data-ttu-id="018bf-917">„--skip-keyvault“ für „kv export“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-917">Add --skip-keyvault for kv export</span></span>

### <a name="appservice"></a><span data-ttu-id="018bf-918">AppService</span><span class="sxs-lookup"><span data-stu-id="018bf-918">AppService</span></span>

* <span data-ttu-id="018bf-919">Fix 12509: Tag für „az webapp up“ standardmäßig entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-919">Fix #12509: Remove the tag to az webapp up by default</span></span>
* <span data-ttu-id="018bf-920">az functionapp create: Hilfemenü für „--runtime-version“ aktualisiert und Warnung hinzugefügt, wenn der Benutzer „--runtime-version“ für .NET angibt</span><span class="sxs-lookup"><span data-stu-id="018bf-920">az functionapp create: Updated --runtime-version help menu and added warning when user specifies --runtime-version for dotnet</span></span>
* <span data-ttu-id="018bf-921">az functionapp create: Methode zum Festlegen von „javaVersion“ für Windows-Funktions-Apps aktualisiert</span><span class="sxs-lookup"><span data-stu-id="018bf-921">az functionapp create: Updated the way javaVersion was being set for Windows function apps</span></span>

### <a name="arm"></a><span data-ttu-id="018bf-922">ARM</span><span class="sxs-lookup"><span data-stu-id="018bf-922">ARM</span></span>

* <span data-ttu-id="018bf-923">az deployment create/validate: Standardmäßige Verwendung von „--handle-extended-json-format“</span><span class="sxs-lookup"><span data-stu-id="018bf-923">az deployment create/validate: Use --handle-extended-json-format by default</span></span>
* <span data-ttu-id="018bf-924">az lock create: Beispiele für die Erstellung einer Unterressource in der Hilfedokumentation hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-924">az lock create: Add examples of creating subresource in the help documentation</span></span>
* <span data-ttu-id="018bf-925">az deployment {group/mg/sub/tenant} list: Unterstützung der provisioningState-Filterung</span><span class="sxs-lookup"><span data-stu-id="018bf-925">az deployment {group/mg/sub/tenant} list: Support provisioningState filtering</span></span>
* <span data-ttu-id="018bf-926">az deployment: Analysefehler für Kommentar unter letztem Argument behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-926">az deployment: Fix the parse bug for comment under the last argument</span></span>

### <a name="backup"></a><span data-ttu-id="018bf-927">Backup</span><span class="sxs-lookup"><span data-stu-id="018bf-927">Backup</span></span>

* <span data-ttu-id="018bf-928">Mehrere Dateiwiederherstellungsfunktionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-928">Added multiple files restore capabilities</span></span>
* <span data-ttu-id="018bf-929">Unterstützung der ausschließlichen Sicherung von Betriebssystemdatenträgern hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-929">Added support for Backing up OS Disks only</span></span>
* <span data-ttu-id="018bf-930">Parameter „restore-as-unmanaged-disk“ für die Angabe einer nicht verwalteten Wiederherstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-930">Added restore-as-unmanaged-disk parameter to specify unmanaged restore</span></span>

### <a name="compute"></a><span data-ttu-id="018bf-931">Compute</span><span class="sxs-lookup"><span data-stu-id="018bf-931">Compute</span></span>

* <span data-ttu-id="018bf-932">az vm create: Option „NONE“ von „--nsg-rule“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-932">az vm create: Add NONE option of --nsg-rule</span></span>
* <span data-ttu-id="018bf-933">az vmss create/update: Vorschautag für automatische VMSS-Reparaturen entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-933">az vmss create/update: remove vmss automatic repairs preview tag</span></span>
* <span data-ttu-id="018bf-934">az vm update: Unterstützung von „--workspace“</span><span class="sxs-lookup"><span data-stu-id="018bf-934">az vm update: Support --workspace</span></span>
* <span data-ttu-id="018bf-935">Fehler im VirtualMachineScaleSetExtension-Initialisierungscode behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-935">Fix a bug in VirtualMachineScaleSetExtension initialization code</span></span>
* <span data-ttu-id="018bf-936">Upgrade der VMAccessAgent-Version auf 2.4 durchgeführt</span><span class="sxs-lookup"><span data-stu-id="018bf-936">Upgrade VMAccessAgent version to 2.4</span></span>
* <span data-ttu-id="018bf-937">az vmss set-orchestration-service-state: Unterstützung zum Festlegen des Orchestrierungdienstzustands für VMSS</span><span class="sxs-lookup"><span data-stu-id="018bf-937">az vmss set-orchestration-service-state: support vmss set orchestration service state</span></span>
* <span data-ttu-id="018bf-938">Upgrade der Datenträger-API-Version auf 2019-11-01 durchgeführt</span><span class="sxs-lookup"><span data-stu-id="018bf-938">Upgrade disk API version to 2019-11-01</span></span>
* <span data-ttu-id="018bf-939">az disk create: add --disk-iops-read-only, --disk-mbps-read-only, --max-shares, --image-reference, --image-reference-lun, --gallery-image-reference, --gallery-image-reference-lun</span><span class="sxs-lookup"><span data-stu-id="018bf-939">az disk create: add --disk-iops-read-only, --disk-mbps-read-only, --max-shares, --image-reference, --image-reference-lun, --gallery-image-reference, --gallery-image-reference-lun</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="018bf-940">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="018bf-940">Cosmos DB</span></span>

* <span data-ttu-id="018bf-941">Fehlende Option „--type“ für Veraltungsumleitungen korrigiert</span><span class="sxs-lookup"><span data-stu-id="018bf-941">Fix missing --type option for deprecation redirections</span></span>

### <a name="docker"></a><span data-ttu-id="018bf-942">Docker</span><span class="sxs-lookup"><span data-stu-id="018bf-942">Docker</span></span>

* <span data-ttu-id="018bf-943">Update auf Alpine 3.11 und Python 3.6.10 durchgeführt</span><span class="sxs-lookup"><span data-stu-id="018bf-943">Update to Alpine 3.11 and Python 3.6.10</span></span>

### <a name="extension"></a><span data-ttu-id="018bf-944">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="018bf-944">Extension</span></span>

* <span data-ttu-id="018bf-945">Laden von Erweiterungen im Systempfad mittels Paketen ermöglicht</span><span class="sxs-lookup"><span data-stu-id="018bf-945">Allow to load extensions in the system path via packages</span></span>

### <a name="hdinsight"></a><span data-ttu-id="018bf-946">HDInsight</span><span class="sxs-lookup"><span data-stu-id="018bf-946">HDInsight</span></span>

* <span data-ttu-id="018bf-947">(az hdinsight create:) Unterstützung der Angabe der unterstützten TLS-Mindestversion durch Kunden unter Verwendung des Parameters `--minimal-tls-version`.</span><span class="sxs-lookup"><span data-stu-id="018bf-947">(az hdinsight create:) Support customers specify minimal supported tls version by using parameter `--minimal-tls-version`.</span></span> <span data-ttu-id="018bf-948">Zulässiger Wert: 1.0,1.1,1.2</span><span class="sxs-lookup"><span data-stu-id="018bf-948">The allowed value is 1.0,1.1,1.2</span></span>

### <a name="iot"></a><span data-ttu-id="018bf-949">IoT</span><span class="sxs-lookup"><span data-stu-id="018bf-949">IoT</span></span>

* <span data-ttu-id="018bf-950">Codebesitzer hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-950">Add codeowner</span></span>
* <span data-ttu-id="018bf-951">az iot hub create: Standard-SKU von F1 in S1 geändert</span><span class="sxs-lookup"><span data-stu-id="018bf-951">az iot hub create : Change default sku to S1 from F1</span></span>
* <span data-ttu-id="018bf-952">iot hub: Unterstützung von „IotHub“ im Profil „2019-03-01-hybrid“</span><span class="sxs-lookup"><span data-stu-id="018bf-952">iot hub: Support IotHub in the profile of 2019-03-01-hybrid</span></span>

### <a name="iotcentral"></a><span data-ttu-id="018bf-953">IoTCentral</span><span class="sxs-lookup"><span data-stu-id="018bf-953">IoTCentral</span></span>

* <span data-ttu-id="018bf-954">Fehlerdetails sowie Standardanwendungsvorlage und Aufforderungsmeldung aktualisiert</span><span class="sxs-lookup"><span data-stu-id="018bf-954">Update error details, update default application template and prompt message</span></span>

### <a name="keyvault"></a><span data-ttu-id="018bf-955">KeyVault</span><span class="sxs-lookup"><span data-stu-id="018bf-955">KeyVault</span></span>

* <span data-ttu-id="018bf-956">Unterstützung von Zertifikatsicherung/-wiederherstellung</span><span class="sxs-lookup"><span data-stu-id="018bf-956">Support certificate backup/restore</span></span>
* <span data-ttu-id="018bf-957">keyvault create/update: Unterstützung von „--retention-days“</span><span class="sxs-lookup"><span data-stu-id="018bf-957">keyvault create/update: Support --retention-days</span></span>
* <span data-ttu-id="018bf-958">Keine Anzeige von verwalteten Schlüsseln/Geheimnissen bei der Auflistung mehr</span><span class="sxs-lookup"><span data-stu-id="018bf-958">No longer display managed keys/secrets while listing</span></span>
* <span data-ttu-id="018bf-959">az keyvault create: Unterstützung von `--network-acls`, `--network-acls-ips` und `--network-acls-vnets` zur Angabe von Netzwerkregeln bei der Tresorerstellung</span><span class="sxs-lookup"><span data-stu-id="018bf-959">az keyvault create: support `--network-acls`, `--network-acls-ips` and `--network-acls-vnets` for specifying network rules while creating vault</span></span>

### <a name="lock"></a><span data-ttu-id="018bf-960">Sperre</span><span class="sxs-lookup"><span data-stu-id="018bf-960">Lock</span></span>

* <span data-ttu-id="018bf-961">Fehlerbehebung für „az lock delete“: „az lock delete“ funktioniert für „Microsoft.DocumentDB“ nicht.</span><span class="sxs-lookup"><span data-stu-id="018bf-961">az lock delete fix bug: az lock delete does not work on Microsoft.DocumentDB</span></span>

### <a name="monitor"></a><span data-ttu-id="018bf-962">Überwachen</span><span class="sxs-lookup"><span data-stu-id="018bf-962">Monitor</span></span>

* <span data-ttu-id="018bf-963">az monitor clone: Unterstützung des Klonens von Metrikregeln zwischen Ressourcen</span><span class="sxs-lookup"><span data-stu-id="018bf-963">az monitor clone: support clone metric rules from one resource to another</span></span>
* <span data-ttu-id="018bf-964">Fix IcM179210086: Erstellung einer benutzerdefinierten Metrikwarnung für die Application Insights-Metrik nicht möglich</span><span class="sxs-lookup"><span data-stu-id="018bf-964">Fix IcM179210086: unable to create custom metric alert for their Application Insights metric</span></span>

### <a name="netappfiles"></a><span data-ttu-id="018bf-965">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="018bf-965">NetAppFiles</span></span>

* <span data-ttu-id="018bf-966">az volume create: Datenschutzvolumes zum Hinzufügen von Replikationsvorgängen zugelassen: Genehmigen, Aussetzen, Fortsetzen, Status, Entfernen</span><span class="sxs-lookup"><span data-stu-id="018bf-966">az volume create: Allow data protection volumes adding replication operations: approve, suspend, resume, status, remove</span></span>

### <a name="network"></a><span data-ttu-id="018bf-967">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="018bf-967">Network</span></span>

* <span data-ttu-id="018bf-968">az network application-gateway waf-policy managed-rule rule-set add: Unterstützung von „ Microsoft_BotManagerRuleSet“</span><span class="sxs-lookup"><span data-stu-id="018bf-968">az network application-gateway waf-policy managed-rule rule-set add: support Microsoft_BotManagerRuleSet</span></span>
* <span data-ttu-id="018bf-969">network watcher flow-log show: Falsche Veraltungsinformationen behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-969">network watcher flow-log show: fix wrong deprecating info</span></span>
* <span data-ttu-id="018bf-970">Unterstützung von Hostnamen im Application Gateway-Listener</span><span class="sxs-lookup"><span data-stu-id="018bf-970">support host names in application gateway listener</span></span>
* <span data-ttu-id="018bf-971">az network nat gateway: Unterstützung der Erstellung einer leeren Ressource ohne öffentliche IP-Adresse oder Präfix für öffentliche IP-Adressen</span><span class="sxs-lookup"><span data-stu-id="018bf-971">az network nat gateway: support create empty resource without public ip or public ip prefix</span></span>
* <span data-ttu-id="018bf-972">Unterstützung der VPN-Gateway-Generierung</span><span class="sxs-lookup"><span data-stu-id="018bf-972">Support vpn gateway generation</span></span>
* <span data-ttu-id="018bf-973">Unterstützung von `--if-none-match` in `az network dns record-set {} add-record`</span><span class="sxs-lookup"><span data-stu-id="018bf-973">Support `--if-none-match` in `az network dns record-set {} add-record`</span></span>

### <a name="packaging"></a><span data-ttu-id="018bf-974">Verpackung</span><span class="sxs-lookup"><span data-stu-id="018bf-974">Packaging</span></span>

* <span data-ttu-id="018bf-975">Unterstützung von Python 3.5 eingestellt</span><span class="sxs-lookup"><span data-stu-id="018bf-975">Drop support for python 3.5</span></span>

### <a name="profile"></a><span data-ttu-id="018bf-976">Profil</span><span class="sxs-lookup"><span data-stu-id="018bf-976">Profile</span></span>

* <span data-ttu-id="018bf-977">az login: Warnung für MFA-Fehler</span><span class="sxs-lookup"><span data-stu-id="018bf-977">az login: Show warning for MFA error</span></span>

### <a name="rdbms"></a><span data-ttu-id="018bf-978">RDBMS</span><span class="sxs-lookup"><span data-stu-id="018bf-978">RDBMS</span></span>

* <span data-ttu-id="018bf-979">Befehle zur Verwaltung von Verschlüsselungsschlüsseln für Serverdaten für PostgreSQL und MySQL hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-979">Add server data encryption key management commands for PostgreSQL and MySQL</span></span>

## <a name="march-10-2020"></a><span data-ttu-id="018bf-980">10. März 2020</span><span class="sxs-lookup"><span data-stu-id="018bf-980">March 10, 2020</span></span>

<span data-ttu-id="018bf-981">Version 2.2.0</span><span class="sxs-lookup"><span data-stu-id="018bf-981">Version 2.2.0</span></span>

### <a name="acr"></a><span data-ttu-id="018bf-982">ACR</span><span class="sxs-lookup"><span data-stu-id="018bf-982">ACR</span></span>

* <span data-ttu-id="018bf-983">Fix: `az acr login` löst fälschlicherweise Fehler aus</span><span class="sxs-lookup"><span data-stu-id="018bf-983">Fix: `az acr login` wrongly raise error</span></span>
* <span data-ttu-id="018bf-984">Neuer Befehl `az acr helm install-cli` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-984">Add new command `az acr helm install-cli`</span></span>
* <span data-ttu-id="018bf-985">Privater Link und CMK-Unterstützung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-985">Add private link and CMK support</span></span>
* <span data-ttu-id="018bf-986">Befehl „private-link-resource list“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-986">add 'private-link-resource list' command</span></span>

### <a name="aks"></a><span data-ttu-id="018bf-987">AKS</span><span class="sxs-lookup"><span data-stu-id="018bf-987">AKS</span></span>

* <span data-ttu-id="018bf-988">Durchsuchen von AKS in Cloud-Shell korrigiert</span><span class="sxs-lookup"><span data-stu-id="018bf-988">fix the aks browse in cloud shell</span></span>
* <span data-ttu-id="018bf-989">az aks: NoneType-Fehler beim Überwachen von „addon“ und „agentpool“ behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-989">az aks: Fix monitoring addon and agentpool NoneType errors</span></span>
* <span data-ttu-id="018bf-990">„--nodepool-tags“ zum Knotenpool beim Erstellen von Azure-Kubernetes-Clustern hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-990">Add --nodepool-tags to node pool when creating azure kubernetes cluster</span></span>
* <span data-ttu-id="018bf-991">„--tags“ beim Hinzufügen oder Aktualisieren eines Knotenpool in einem Cluster hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-991">Add --tags when adding or updating a nodepool to cluster</span></span>
* <span data-ttu-id="018bf-992">aks create: `--enable-private-cluster` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-992">aks create: add `--enable-private-cluster`</span></span>
* <span data-ttu-id="018bf-993">„--nodepool-labels“ beim Erstellen von Azure-Kubernetes-Clustern hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-993">add --nodepool-labels when creating azure kubernetes cluster</span></span>
* <span data-ttu-id="018bf-994">„--labels“ beim Hinzufügen eines neuen Knotenpools zu einem Azure-Kubernetes-Cluster hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-994">add --labels when adding a new nodepool to azure kubernetes cluster</span></span>
* <span data-ttu-id="018bf-995">Fehlender Schrägstrich (/) in der Dashboard-URL hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-995">add missing / in the dashboard url</span></span>
* <span data-ttu-id="018bf-996">Unterstützung der Erstellung von AKS-Clustern, sodass verwaltete Identitäten möglich sind</span><span class="sxs-lookup"><span data-stu-id="018bf-996">Support create aks clusters enabling managed identity</span></span>
* <span data-ttu-id="018bf-997">az aks: Überprüfen, ob das Netzwerk-Plug-In entweder „azure“ oder „kubenet“ ist</span><span class="sxs-lookup"><span data-stu-id="018bf-997">az aks: Validate network plugin to be either "azure" or "kubenet"</span></span>
* <span data-ttu-id="018bf-998">az aks: Unterstützung für AAD-Sitzungsschlüssel hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-998">az aks: Add aad session key support</span></span>
* <span data-ttu-id="018bf-999">[BREAKING CHANGE] az aks: Unterstützung von MSI-Änderungen für GF und BF für omsagent (Containerüberwachung)(#1)</span><span class="sxs-lookup"><span data-stu-id="018bf-999">[BREAKING CHANGE] az aks: support msi changes for GF and BF for omsagent (Container monitoring)(#1)</span></span>
* <span data-ttu-id="018bf-1000">az aks use-dev-spaces: Endpunkt-Typoption zum Befehl „use-dev-spaces“, hinzugefügt, um den auf einem Azure Dev Spaces-Controller erstellten Endpunkt anzupassen</span><span class="sxs-lookup"><span data-stu-id="018bf-1000">az aks use-dev-spaces: Adding endpoint type option to the use-dev-spaces command to customize the endpoint created on an Azure Dev Spaces controller</span></span>

### <a name="appconfig"></a><span data-ttu-id="018bf-1001">AppConfig</span><span class="sxs-lookup"><span data-stu-id="018bf-1001">AppConfig</span></span>

* <span data-ttu-id="018bf-1002">Verwendung von „kv set“ entsperrt, um Schlüsseltresorverweis und -funktion hinzuzufügen …</span><span class="sxs-lookup"><span data-stu-id="018bf-1002">Unblock using "kv set" to add keyvault reference and feature …</span></span>

### <a name="appservice"></a><span data-ttu-id="018bf-1003">AppService</span><span class="sxs-lookup"><span data-stu-id="018bf-1003">AppService</span></span>

* <span data-ttu-id="018bf-1004">az webapp create : Beheben eines Problems beim Ausführen des Befehls mit „--runtime“</span><span class="sxs-lookup"><span data-stu-id="018bf-1004">az webapp create : Fix issue when running the command with --runtime</span></span>
* <span data-ttu-id="018bf-1005">az functionapp deployment source config-zip: Fehlermeldung hinzugefügt, wenn der Ressourcengruppen- oder Funktionsname ungültig oder nicht vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="018bf-1005">az functionapp deployment source config-zip: Add an error message if resource group or function name are invalid/don't exist</span></span>
* <span data-ttu-id="018bf-1006">functionapp create: Warnmeldung korrigiert, die derzeit mit `functionapp create` angezeigt wird und ein `--functions_version`-Flag angibt, aber irrtümlich ein `_` anstelle eines `-` im Flagnamen verwendet</span><span class="sxs-lookup"><span data-stu-id="018bf-1006">functionapp create: Fix the warning message that appears with `functionapp create` today which cites a `--functions_version` flag but erroneously uses a `_` instead of a `-` in the flag name</span></span>
* <span data-ttu-id="018bf-1007">az functionapp create: Es wurde aktualisiert, wie linuxFxVersion und der Containerimagename für Linux-Funktions-Apps festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="018bf-1007">az functionapp create: Updated the way linuxFxVersion and container image name were being set for linux function apps</span></span>
* <span data-ttu-id="018bf-1008">az functionapp deployment source config-zip: Problems behoben, das durch die Racebedingung für die Änderung von App-Einstellungen während der ZIP-Bereitstellung verursacht wird und während der Bereitstellung 5xx-Fehler ausgibt</span><span class="sxs-lookup"><span data-stu-id="018bf-1008">az functionapp deployment source config-zip: Fix an issue caused by app settings change racing condition during zip deploy, giving 5xx errors during deployment</span></span>
* <span data-ttu-id="018bf-1009">Fix #5720946: „az webapp backup“ legt Namen nicht fest</span><span class="sxs-lookup"><span data-stu-id="018bf-1009">Fix #5720946: az webapp backup fails to set name</span></span>

### <a name="arm"></a><span data-ttu-id="018bf-1010">ARM</span><span class="sxs-lookup"><span data-stu-id="018bf-1010">ARM</span></span>

* <span data-ttu-id="018bf-1011">az resource: Beispiele für das Ressourcenmodul verbessert</span><span class="sxs-lookup"><span data-stu-id="018bf-1011">az resource: Improve the examples of the resource module</span></span>
* <span data-ttu-id="018bf-1012">az policy assignment list: Unterstützung für das Auflisten von Richtlinienzuweisungen im Verwaltungsgruppenbereich</span><span class="sxs-lookup"><span data-stu-id="018bf-1012">az policy assignment list: Support listing policy assignments at Management Group scope</span></span>
* <span data-ttu-id="018bf-1013">`az deployment group` und `az deployment operation group` für Vorlagenbereitstellung in Ressourcengruppen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1013">Add `az deployment group` and `az deployment operation group` for template deployment at resource groups.</span></span> <span data-ttu-id="018bf-1014">Dies ist ein Duplikat von `az group deployment` und `az group deployment operation`.</span><span class="sxs-lookup"><span data-stu-id="018bf-1014">This is a duplicate of `az group deployment` and `az group deployment operation`</span></span>
* <span data-ttu-id="018bf-1015">`az deployment sub` und `az deployment operation sub` für Vorlagenbereitstellung im Abonnementbereich hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1015">Add `az deployment sub` and `az deployment operation sub` for template deployment at subscription scope.</span></span> <span data-ttu-id="018bf-1016">Dies ist ein Duplikat von `az deployment` und `az deployment operation`.</span><span class="sxs-lookup"><span data-stu-id="018bf-1016">This is a duplicate of `az deployment` and `az deployment operation`</span></span>
* <span data-ttu-id="018bf-1017">`az deployment mg` und `az deployment operation mg` für Vorlagenbereitstellung in Verwaltungsgruppen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1017">Add `az deployment mg` and `az deployment operation mg` for template deployment at management groups</span></span>
* <span data-ttu-id="018bf-1018">`az deployment tenant` und `az deployment operation tenant` für Vorlagenbereitstellung im Mandantenbereich hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1018">Add `az deployment tenant` and `az deployment operation tenant` for template deployment at tenant scope</span></span>
* <span data-ttu-id="018bf-1019">az policy assignment create: Beschreibung zu Parameter `--location` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1019">az policy assignment create: Add a description to the `--location` parameter</span></span>
* <span data-ttu-id="018bf-1020">az group deployment create: Parameter `--aux-tenants` zur mandantenübergreifenden Unterstützung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1020">az group deployment create: Add parameter `--aux-tenants` to support cross tenants</span></span>

### <a name="cdn"></a><span data-ttu-id="018bf-1021">CDN</span><span class="sxs-lookup"><span data-stu-id="018bf-1021">CDN</span></span>

* <span data-ttu-id="018bf-1022">CDN-WAF-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1022">Add CDN WAF commands</span></span>

### <a name="compute"></a><span data-ttu-id="018bf-1023">Compute</span><span class="sxs-lookup"><span data-stu-id="018bf-1023">Compute</span></span>

* <span data-ttu-id="018bf-1024">az sig image-version: „--data-snapshot-luns“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1024">az sig image-version: add --data-snapshot-luns</span></span>
* <span data-ttu-id="018bf-1025">az ppg show: „--colocation-status“ hinzugefügt, um das Abrufen des Zusammenstellungsstatus aller Ressourcen in der Näherungsplatzierungsgruppe zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="018bf-1025">az ppg show: add --colocation-status to enable fetching the colocation status of all the resources in the proximity placement group</span></span>
* <span data-ttu-id="018bf-1026">az vmss create/update: Unterstützung automatischer Reparaturen</span><span class="sxs-lookup"><span data-stu-id="018bf-1026">az vmss create/update: support automatic repairs</span></span>
* <span data-ttu-id="018bf-1027">[BREAKING CHANGE] az image template: „template“ in „builder“ umbenannt</span><span class="sxs-lookup"><span data-stu-id="018bf-1027">[BREAKING CHANGE] az image template: rename template to builder</span></span>
* <span data-ttu-id="018bf-1028">az image builder create: „--image-template“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1028">az image builder create: add --image-template</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="018bf-1029">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="018bf-1029">Cosmos DB</span></span>

* <span data-ttu-id="018bf-1030">Gespeicherte Prozedur „Add Sql“, udf- und trigger-Cmdlets hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1030">Add Sql stored procedure, udf and trigger cmdlets</span></span>
* <span data-ttu-id="018bf-1031">az cosmosdb create: „--key-uri“ hinzugefügt, um das Hinzufügen von Schlüsseltresor-Verschlüsselungsinformationen zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="018bf-1031">az cosmosdb create: add --key-uri to support adding key vault encryption information</span></span>

### <a name="keyvault"></a><span data-ttu-id="018bf-1032">KeyVault</span><span class="sxs-lookup"><span data-stu-id="018bf-1032">KeyVault</span></span>

* <span data-ttu-id="018bf-1033">keyvault create: „soft-delete“ standardmäßig aktiviert</span><span class="sxs-lookup"><span data-stu-id="018bf-1033">keyvault create: enable soft-delete by default</span></span>

### <a name="monitor"></a><span data-ttu-id="018bf-1034">Überwachen</span><span class="sxs-lookup"><span data-stu-id="018bf-1034">Monitor</span></span>

* <span data-ttu-id="018bf-1035">az monitor metrics alert create: Unterstützung von `~` in `--condition`</span><span class="sxs-lookup"><span data-stu-id="018bf-1035">az monitor metrics alert create: support `~` in `--condition`</span></span>

### <a name="network"></a><span data-ttu-id="018bf-1036">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="018bf-1036">Network</span></span>

* <span data-ttu-id="018bf-1037">az network application-gateway rewrite-rule create: Unterstützung der URL-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="018bf-1037">az network application-gateway rewrite-rule create: support url configuration</span></span>
* <span data-ttu-id="018bf-1038">az network dns zone import: Bei „--zone-name“ wird die Groß-/Kleinschreibung künftig nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="018bf-1038">az network dns zone import: --zone-name will be case insensitive in the future</span></span>
* <span data-ttu-id="018bf-1039">az network private-endpoint/private-link-service: Vorschaubezeichnung entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-1039">az network private-endpoint/private-link-service: remove preview label</span></span>
* <span data-ttu-id="018bf-1040">az network bastion: Unterstützung von „bastion“</span><span class="sxs-lookup"><span data-stu-id="018bf-1040">az network bastion: support bastion</span></span>
* <span data-ttu-id="018bf-1041">az network vnet list-available-ips: Unterstützung für das Auflisten verfügbarer IPs in einem VNET</span><span class="sxs-lookup"><span data-stu-id="018bf-1041">az network vnet list-available-ips: support list available ips in a vnet</span></span>
* <span data-ttu-id="018bf-1042">az network watcher flow-log create/list/delete/update: neue Befehle hinzugefügt, um Watcher-Datenflussprotokolle zu verwalten und „--location“ zur expliziten Identifizierung von Watcher verfügbar zu machen</span><span class="sxs-lookup"><span data-stu-id="018bf-1042">az network watcher flow-log create/list/delete/update: add new commands to manage watcher flow log and exposing --location to identify watcher explicitly</span></span>
* <span data-ttu-id="018bf-1043">az network watcher flow-log configure: veraltet</span><span class="sxs-lookup"><span data-stu-id="018bf-1043">az network watcher flow-log configure: deprecated</span></span>
* <span data-ttu-id="018bf-1044">az network watcher flow-log show: Unterstützung von „--location“ und „--name“, um ein ARM-formatiertes Ergebnis zu erhalten; alte formatierte Ausgabe als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="018bf-1044">az network watcher flow-log show: support --location and --name to get ARM-formatted result, deprecated old formatted output</span></span>

### <a name="policy"></a><span data-ttu-id="018bf-1045">Richtlinie</span><span class="sxs-lookup"><span data-stu-id="018bf-1045">Policy</span></span>

* <span data-ttu-id="018bf-1046">az policy assignment create: Fehler behoben, dass automatisch generierter Name der Richtlinienzuweisung den Grenzwert überschreitet</span><span class="sxs-lookup"><span data-stu-id="018bf-1046">az policy assignment create: Fix the bug that automatically generated name of policy assignment exceeds the limit</span></span>

### <a name="rbac"></a><span data-ttu-id="018bf-1047">RBAC</span><span class="sxs-lookup"><span data-stu-id="018bf-1047">RBAC</span></span>

* <span data-ttu-id="018bf-1048">az ad group show: Problem behoben, dass „--group“-Wert als regulärer Ausdruck behandelt wurde</span><span class="sxs-lookup"><span data-stu-id="018bf-1048">az ad group show: fix --group value treated as regex problem</span></span>

### <a name="rdbms"></a><span data-ttu-id="018bf-1049">RDBMS</span><span class="sxs-lookup"><span data-stu-id="018bf-1049">RDBMS</span></span>

* <span data-ttu-id="018bf-1050">SDK-Version von „azure-mgmt-rdbms“ auf 2.0.0 festgelegt</span><span class="sxs-lookup"><span data-stu-id="018bf-1050">Bump the azure-mgmt-rdbms SDK version to 2.0.0</span></span>
* <span data-ttu-id="018bf-1051">az postgres private-endpoint-connection: Verwalten von Verbindungen mit privatem Postgres-Endpunkt</span><span class="sxs-lookup"><span data-stu-id="018bf-1051">az postgres private-endpoint-connection: manage postgres private endpoint connections</span></span>
* <span data-ttu-id="018bf-1052">az postgres private-link-resource: Verwalten von privaten Postgres-Linkressourcen</span><span class="sxs-lookup"><span data-stu-id="018bf-1052">az postgres private-link-resource: manage postgres private link resources</span></span>
* <span data-ttu-id="018bf-1053">az mysql private-endpoint-connection: Verwalten von Verbindungen mit privatem MySQL-Endpunkt</span><span class="sxs-lookup"><span data-stu-id="018bf-1053">az mysql private-endpoint-connection: manage mysql private endpoint connections</span></span>
* <span data-ttu-id="018bf-1054">az mysql private-link-resource: Verwalten von privaten MySQL-Linkressourcen</span><span class="sxs-lookup"><span data-stu-id="018bf-1054">az mysql private-link-resource: manage mysql private link resources</span></span>
* <span data-ttu-id="018bf-1055">az mariadb private-endpoint-connection: Verwalten von Verbindungen mit privatem MariaDB-Endpunkt</span><span class="sxs-lookup"><span data-stu-id="018bf-1055">az mariadb private-endpoint-connection: manage mariadb private endpoint connections</span></span>
* <span data-ttu-id="018bf-1056">az mariadb private-link-resource: Verwalten von privaten MariaDB-Linkressourcen</span><span class="sxs-lookup"><span data-stu-id="018bf-1056">az mariadb private-link-resource: manage mariadb private link resources</span></span>
* <span data-ttu-id="018bf-1057">Aktualisieren von Tests von privaten RDBMS-Endpunkten</span><span class="sxs-lookup"><span data-stu-id="018bf-1057">Updating RDBMS Private Endpoint Tests</span></span>

### <a name="sql"></a><span data-ttu-id="018bf-1058">SQL</span><span class="sxs-lookup"><span data-stu-id="018bf-1058">SQL</span></span>

* <span data-ttu-id="018bf-1059">Sql midb: list-deleted, show-deleted, update-retention, show-retention hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1059">Sql midb Add: list-deleted, show-deleted, update-retention, show-retention</span></span>
* <span data-ttu-id="018bf-1060">(sql server create:) Optionales Flag „Enable“/„Disable“ für public-network-access zu „sql server create“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1060">(sql server create:) Add optional public-network-access 'Enable'/'Disable' flag to sql server create</span></span>
* <span data-ttu-id="018bf-1061">(sql server update): kundenorientierte Änderung vorgenommen</span><span class="sxs-lookup"><span data-stu-id="018bf-1061">(sql server update:) make some customer-facing change</span></span>
* <span data-ttu-id="018bf-1062">Eigenschaft „minimal_tls_version“ für MI und SQL-Datenbank hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1062">Add minimal_tls_version property for MI and SQL DB</span></span>

### <a name="storage"></a><span data-ttu-id="018bf-1063">Storage</span><span class="sxs-lookup"><span data-stu-id="018bf-1063">Storage</span></span>

* <span data-ttu-id="018bf-1064">az storage blob delete-batch: Flag `--dryrun` mit Fehlverhalten</span><span class="sxs-lookup"><span data-stu-id="018bf-1064">az storage blob delete-batch: Misbehaving `--dryrun` flag</span></span>
* <span data-ttu-id="018bf-1065">az storage account network-rule hinzugefügt (Fehlerbehebung): Hinzufügen von Vorgängen muss idempotent sein</span><span class="sxs-lookup"><span data-stu-id="018bf-1065">az storage account network-rule add (bug fix): add operation should be idempotent</span></span>
* <span data-ttu-id="018bf-1066">az storage account create/update: Unterstützung für Routingpräferenz hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1066">az storage account create/update: Add Routing Preference support</span></span>
* <span data-ttu-id="018bf-1067">„azure-mgmt-storage“ auf Version 8.0.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="018bf-1067">Upgrade azure-mgmt-storage version to 8.0.0</span></span>
* <span data-ttu-id="018bf-1068">az storage container immutability create: Parameter „--allow-protected-append-write“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1068">az storage container immutability create: add --allow-protected-append-write parameter</span></span>
* <span data-ttu-id="018bf-1069">az storage account private-link-resource list: Unterstützung zum Auflisten privater Linkressourcen für Speicherkonto hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1069">az storage account private-link-resource list: Add support to list private link resources for storage account</span></span>
* <span data-ttu-id="018bf-1070">az storage account private-endpoint-connection approve/reject/show/delete: Unterstützung der Verwaltung von Verbindungen mit privaten Endpunkten</span><span class="sxs-lookup"><span data-stu-id="018bf-1070">az storage account private-endpoint-connection approve/reject/show/delete: Support to manage private endpoint connections</span></span>
* <span data-ttu-id="018bf-1071">az storage account blob-service-properties update: „--enable-restore-policy“ und „--restore-days“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1071">az storage account blob-service-properties update: add --enable-restore-policy and --restore-days</span></span>
* <span data-ttu-id="018bf-1072">az storage blob restore: Unterstützung für die Wiederherstellung von Blobbereichen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1072">az storage blob restore: Add support to restore blob ranges</span></span>

## <a name="february-18-2020"></a><span data-ttu-id="018bf-1073">18. Februar 2020</span><span class="sxs-lookup"><span data-stu-id="018bf-1073">February 18, 2020</span></span>

<span data-ttu-id="018bf-1074">Version 2.1.0</span><span class="sxs-lookup"><span data-stu-id="018bf-1074">Version 2.1.0</span></span>

### <a name="acr"></a><span data-ttu-id="018bf-1075">ACR</span><span class="sxs-lookup"><span data-stu-id="018bf-1075">ACR</span></span>

* <span data-ttu-id="018bf-1076">Neues Argument `--expose-token` für `az acr login` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1076">Add a new argument `--expose-token` for `az acr login`</span></span>
* <span data-ttu-id="018bf-1077">Falsche Ausgabe für `az acr task identity show -n Name -r Registry -o table` korrigiert</span><span class="sxs-lookup"><span data-stu-id="018bf-1077">Fix the incorrect output of `az acr task identity show -n Name -r Registry -o table`</span></span>
* <span data-ttu-id="018bf-1078">az acr login: Auslösen von „CLIError“, wenn vom Docker-Befehl Fehler zurückgegeben werden</span><span class="sxs-lookup"><span data-stu-id="018bf-1078">az acr login: Throw a CLIError if there are errors returned by docker command</span></span>

### <a name="acs"></a><span data-ttu-id="018bf-1079">ACS</span><span class="sxs-lookup"><span data-stu-id="018bf-1079">ACS</span></span>

* <span data-ttu-id="018bf-1080">aks create/update: Validierung für `--vnet-subnet-id` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1080">aks create/update: add `--vnet-subnet-id` validation</span></span>

### <a name="aladdin"></a><span data-ttu-id="018bf-1081">Aladdin</span><span class="sxs-lookup"><span data-stu-id="018bf-1081">Aladdin</span></span>

* <span data-ttu-id="018bf-1082">Analysieren der generierten Beispiele in „_help.py“ der Befehle</span><span class="sxs-lookup"><span data-stu-id="018bf-1082">Parse generated examples into commands' _help.py</span></span>

### <a name="ams"></a><span data-ttu-id="018bf-1083">AMS</span><span class="sxs-lookup"><span data-stu-id="018bf-1083">AMS</span></span>

* <span data-ttu-id="018bf-1084">az ams ist jetzt allgemein verfügbar.</span><span class="sxs-lookup"><span data-stu-id="018bf-1084">az ams is GA now</span></span>

### <a name="appconfig"></a><span data-ttu-id="018bf-1085">AppConfig</span><span class="sxs-lookup"><span data-stu-id="018bf-1085">AppConfig</span></span>

* <span data-ttu-id="018bf-1086">Hilfenachricht überarbeitet, um nicht unterstützte Schlüssel-/Bezeichnungsfilter auszuschließen</span><span class="sxs-lookup"><span data-stu-id="018bf-1086">Revise help message to exclude unsupported key/label filter</span></span>
* <span data-ttu-id="018bf-1087">Vorschautag für die meisten Befehle entfernt (mit Ausnahme der Flags für verwaltete Identitäten und Features)</span><span class="sxs-lookup"><span data-stu-id="018bf-1087">Remove preview tag for most commands excluding managed identity and feature flags</span></span>
* <span data-ttu-id="018bf-1088">Kundenseitig verwalteter Schlüssel beim Aktualisieren der Speicher hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1088">Add customer managed key when updating stores</span></span>

### <a name="appservice"></a><span data-ttu-id="018bf-1089">AppService</span><span class="sxs-lookup"><span data-stu-id="018bf-1089">AppService</span></span>

* <span data-ttu-id="018bf-1090">az webapp list-runtimes: Fehler bei „list-runtimes“ behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-1090">az webapp list-runtimes: Fix the bug for list-runtimes</span></span>
* <span data-ttu-id="018bf-1091">„az webapp|functionapp config ssl create“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1091">Add az webapp|functionapp config ssl create</span></span>
* <span data-ttu-id="018bf-1092">Unterstützung für v3-Funktions-Apps und Node 12</span><span class="sxs-lookup"><span data-stu-id="018bf-1092">Add support for v3 function apps and node 12</span></span>

### <a name="arm"></a><span data-ttu-id="018bf-1093">ARM</span><span class="sxs-lookup"><span data-stu-id="018bf-1093">ARM</span></span>

* <span data-ttu-id="018bf-1094">az policy assignment create: Fehlermeldung korrigiert, die angezeigt wird, wenn der Parameter `--policy` ungültig ist</span><span class="sxs-lookup"><span data-stu-id="018bf-1094">az policy assignment create: Fix the error message when the `--policy` parameter is invalid</span></span>
* <span data-ttu-id="018bf-1095">az group deployment create: Fehler „stat: path too long for Windows" korrigiert, der angezeigt wird, wenn eine zu große Datei vom Typ „parameters.json“ verwendet wird</span><span class="sxs-lookup"><span data-stu-id="018bf-1095">az group deployment create: Fix "stat: path too long for Windows" error when using large parameters.json file</span></span>

### <a name="backup"></a><span data-ttu-id="018bf-1096">Backup</span><span class="sxs-lookup"><span data-stu-id="018bf-1096">Backup</span></span>

* <span data-ttu-id="018bf-1097">Korrektur des Wiederherstellungsflows auf Elementebene am ursprünglichen Speicherort</span><span class="sxs-lookup"><span data-stu-id="018bf-1097">Fix for item level recovery flow in OLR</span></span>
* <span data-ttu-id="018bf-1098">Unterstützung von „Als Dateien wiederherstellen“ für SQL- und SAP-Datenbanken hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1098">Add restore as files support for SQL and SAP Databases</span></span>

### <a name="compute"></a><span data-ttu-id="018bf-1099">Compute</span><span class="sxs-lookup"><span data-stu-id="018bf-1099">Compute</span></span>

* <span data-ttu-id="018bf-1100">vm/vmss/availability-set update: „--ppg“ hinzugefügt, um die Aktualisierung von „ProximityPlacementGroup“ zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="018bf-1100">vm/vmss/availability-set update: add --ppg to allowing updating ProximityPlacementGroup</span></span>
* <span data-ttu-id="018bf-1101">vmss create: „--data-disk-iops“ und „--data-disk-mbps“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1101">vmss create: add --data-disk-iops and --data-disk-mbps</span></span>
* <span data-ttu-id="018bf-1102">az vm host: Vorschautag für `vm host` und `vm host group` entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-1102">az vm host: remove preview tag for `vm host` and `vm host group`</span></span>
* <span data-ttu-id="018bf-1103">[BREAKING CHANGE] Behebung Nr. 10728: `az vm create`: Automatisches Erstellen des Subnetzes, wenn das VNET angegeben wird und das Subnetz nicht vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="018bf-1103">[BREAKING CHANGE] Fix #10728: `az vm create`: create subnet automatically if vnet is specified and subnet not exists</span></span>
* <span data-ttu-id="018bf-1104">Erhöhen der Stabilität von „vm image list“</span><span class="sxs-lookup"><span data-stu-id="018bf-1104">Increase robustness of vm image list</span></span>

### <a name="eventhub"></a><span data-ttu-id="018bf-1105">Eventhub</span><span class="sxs-lookup"><span data-stu-id="018bf-1105">Eventhub</span></span>

* <span data-ttu-id="018bf-1106">Azure Stack-Unterstützung für Profil „2019-03-01-hybrid“</span><span class="sxs-lookup"><span data-stu-id="018bf-1106">Azure Stack support for 2019-03-01-hybrid profile</span></span>

### <a name="keyvault"></a><span data-ttu-id="018bf-1107">KeyVault</span><span class="sxs-lookup"><span data-stu-id="018bf-1107">KeyVault</span></span>

* <span data-ttu-id="018bf-1108">az keyvault key create: neuer Wert `import` für Parameter `--ops` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1108">az keyvault key create: add a new value `import` for parameter `--ops`</span></span>
* <span data-ttu-id="018bf-1109">az keyvault key list-versions: Unterstützung des Parameters `--id` für die Angabe von Schlüsseln</span><span class="sxs-lookup"><span data-stu-id="018bf-1109">az keyvault key list-versions: support parameter `--id` for specifying keys</span></span>
* <span data-ttu-id="018bf-1110">Unterstützung für Verbindungen mit privaten Endpunkten</span><span class="sxs-lookup"><span data-stu-id="018bf-1110">Support private endpoint connections</span></span>

### <a name="network"></a><span data-ttu-id="018bf-1111">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="018bf-1111">Network</span></span>

* <span data-ttu-id="018bf-1112">Geändert in „azure-mgmt-network 9.0.0“</span><span class="sxs-lookup"><span data-stu-id="018bf-1112">Bump to azure-mgmt-network 9.0.0</span></span>
* <span data-ttu-id="018bf-1113">az network private-link-service update/create: Unterstützung von „--enable-proxy-protocol“</span><span class="sxs-lookup"><span data-stu-id="018bf-1113">az network private-link-service update/create: support --enable-proxy-protocol</span></span>
* <span data-ttu-id="018bf-1114">Feature für Version 2 von Verbindungsmonitor hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1114">Add connection Monitor V2 feature</span></span>

### <a name="packaging"></a><span data-ttu-id="018bf-1115">Verpackung</span><span class="sxs-lookup"><span data-stu-id="018bf-1115">Packaging</span></span>

* <span data-ttu-id="018bf-1116">[BREAKING CHANGE] Unterstützung für Python 2.7 eingestellt</span><span class="sxs-lookup"><span data-stu-id="018bf-1116">[BREAKING CHANGE] Drop support for Python 2.7</span></span>

### <a name="profile"></a><span data-ttu-id="018bf-1117">Profil</span><span class="sxs-lookup"><span data-stu-id="018bf-1117">Profile</span></span>

* <span data-ttu-id="018bf-1118">Vorschau: Neue Attribute `homeTenantId` und `managedByTenants` zu Abonnementkonten hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-1118">Preview: Add new attributes `homeTenantId` and `managedByTenants` to subscription accounts.</span></span> <span data-ttu-id="018bf-1119">Führen Sie `az login` erneut aus, damit die Änderungen wirksam werden.</span><span class="sxs-lookup"><span data-stu-id="018bf-1119">Please re-run `az login` for the changes to take effect</span></span>
* <span data-ttu-id="018bf-1120">az login: Eine Warnung wird angezeigt, wenn ein Abonnement von mehren Mandanten aufgeführt wird und der erste als Standard festgelegt wird.</span><span class="sxs-lookup"><span data-stu-id="018bf-1120">az login: Show a warning when a subscription is listed from more than one tenants and default to the first one.</span></span> <span data-ttu-id="018bf-1121">Fügen Sie `--tenant` in `az login` ein, um beim Zugreifen auf dieses Abonnement einen bestimmten Mandanten auszuwählen.</span><span class="sxs-lookup"><span data-stu-id="018bf-1121">To select a specific tenant when accessing this subscription, please include `--tenant` in `az login`</span></span>

### <a name="role"></a><span data-ttu-id="018bf-1122">Role</span><span class="sxs-lookup"><span data-stu-id="018bf-1122">Role</span></span>

* <span data-ttu-id="018bf-1123">az role assignment create: Problem behoben, das beim Zuweisen einer Rolle zu einem Dienstprinzipal nach Anzeigename einen Fehler vom Typ „HTTP 400“ verursachte</span><span class="sxs-lookup"><span data-stu-id="018bf-1123">az role assignment create: Fix the error that assigning a role to a service principal by display name yields a HTTP 400</span></span>

### <a name="sql"></a><span data-ttu-id="018bf-1124">SQL</span><span class="sxs-lookup"><span data-stu-id="018bf-1124">SQL</span></span>

* <span data-ttu-id="018bf-1125">Cmdlet `az sql mi update` der verwalteten SQL-Instanz mit zwei neuen Parametern aktualisiert: tier und family</span><span class="sxs-lookup"><span data-stu-id="018bf-1125">Update SQL Managed Instance cmdlet `az sql mi update` with two new parameters: tier and family</span></span>

### <a name="storage"></a><span data-ttu-id="018bf-1126">Storage</span><span class="sxs-lookup"><span data-stu-id="018bf-1126">Storage</span></span>

* <span data-ttu-id="018bf-1127">[BREAKING CHANGE] `az storage account create`: Art des Standardspeicherkontos in StorageV2 geändert</span><span class="sxs-lookup"><span data-stu-id="018bf-1127">[BREAKING CHANGE] `az storage account create`: Change default storage account kind to StorageV2</span></span>

## <a name="february-04-2020"></a><span data-ttu-id="018bf-1128">04. Februar 2020</span><span class="sxs-lookup"><span data-stu-id="018bf-1128">February 04, 2020</span></span>

<span data-ttu-id="018bf-1129">Version 2.0.81</span><span class="sxs-lookup"><span data-stu-id="018bf-1129">Version 2.0.81</span></span>

### <a name="acs"></a><span data-ttu-id="018bf-1130">ACS</span><span class="sxs-lookup"><span data-stu-id="018bf-1130">ACS</span></span>

* <span data-ttu-id="018bf-1131">Unterstützung für das Festlegen zugeordneter Ausgangsports und Leerlauftimeouts für Load Balancer Standard hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1131">Add support to set outbound allocated ports and idle timeouts on standard load balancer</span></span>
* <span data-ttu-id="018bf-1132">Aktualisierung auf API-Version 2019-11-01</span><span class="sxs-lookup"><span data-stu-id="018bf-1132">Update to API Version 2019-11-01</span></span>

### <a name="acr"></a><span data-ttu-id="018bf-1133">ACR</span><span class="sxs-lookup"><span data-stu-id="018bf-1133">ACR</span></span>

* <span data-ttu-id="018bf-1134">[BREAKING CHANGE] `az acr delete` löst eine Eingabeaufforderung aus.</span><span class="sxs-lookup"><span data-stu-id="018bf-1134">[BREAKING CHANGE] `az acr delete` will prompt</span></span>
* <span data-ttu-id="018bf-1135">[BREAKING CHANGE] „az acr task delete“ löst eine Eingabeaufforderung aus.</span><span class="sxs-lookup"><span data-stu-id="018bf-1135">[BREAKING CHANGE] 'az acr task delete' will prompt</span></span>
* <span data-ttu-id="018bf-1136">Neue Befehlsgruppe „az acr taskrun show/list/delete“ für die Aufgabenausführungsverwaltung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1136">Add a new command group 'az acr taskrun show/list/delete' for taskrun management</span></span>

### <a name="aks"></a><span data-ttu-id="018bf-1137">AKS</span><span class="sxs-lookup"><span data-stu-id="018bf-1137">AKS</span></span>

* <span data-ttu-id="018bf-1138">Jeder Cluster erhält einen separaten Dienstprinzipal zur Verbesserung der Isolation.</span><span class="sxs-lookup"><span data-stu-id="018bf-1138">Each cluster gets a separate service principal to improve isolation</span></span>

### <a name="appconfig"></a><span data-ttu-id="018bf-1139">AppConfig</span><span class="sxs-lookup"><span data-stu-id="018bf-1139">AppConfig</span></span>

* <span data-ttu-id="018bf-1140">Unterstützung für den Import/Export von KeyVault-Verweisen in/aus AppService</span><span class="sxs-lookup"><span data-stu-id="018bf-1140">Support import/export of keyvault references from/to appservice</span></span>
* <span data-ttu-id="018bf-1141">Unterstützung für den Import/Export aller Bezeichnungen in appconfig und aus appconfig</span><span class="sxs-lookup"><span data-stu-id="018bf-1141">Support import/export of all labels from appconfig to appconfig</span></span>
* <span data-ttu-id="018bf-1142">Überprüfen der Schlüssel- und Featurenamen vor dem Festlegen und Importieren</span><span class="sxs-lookup"><span data-stu-id="018bf-1142">Validate key and feature names before setting and importing</span></span>
* <span data-ttu-id="018bf-1143">Verfügbarmachen der SKU-Änderung für den Konfigurationsspeicher</span><span class="sxs-lookup"><span data-stu-id="018bf-1143">Expose sku modification for configuration store.</span></span>
* <span data-ttu-id="018bf-1144">Befehlsgruppe für die verwaltete Identität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1144">Add command group for managed identity.</span></span>

### <a name="appservice"></a><span data-ttu-id="018bf-1145">AppService</span><span class="sxs-lookup"><span data-stu-id="018bf-1145">AppService</span></span>

* <span data-ttu-id="018bf-1146">Azure Stack: Oberflächenbefehle im Profil „2019-03-01-hybrid“</span><span class="sxs-lookup"><span data-stu-id="018bf-1146">Azure Stack: surface commands under the profile of 2019-03-01-hybrid</span></span>
* <span data-ttu-id="018bf-1147">functionapp: Funktion zum Erstellen von Java-Funktions-Apps in Linux hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1147">functionapp: Add ability to create Java function apps in Linux</span></span>

### <a name="arm"></a><span data-ttu-id="018bf-1148">ARM</span><span class="sxs-lookup"><span data-stu-id="018bf-1148">ARM</span></span>

* <span data-ttu-id="018bf-1149">Behebung von Problem Nr. 10246: `az resource tag` stürzt ab, wenn der übergebene Parameter `--ids` der Ressourcengruppen-ID entspricht.</span><span class="sxs-lookup"><span data-stu-id="018bf-1149">Fix issue #10246: `az resource tag` crashes when the parameter `--ids` passed in is resource group ID</span></span>
* <span data-ttu-id="018bf-1150">Behebung von Problem Nr. 11658: Der Befehl `az group export` unterstützt die Parameter `--query` und `--output` nicht.</span><span class="sxs-lookup"><span data-stu-id="018bf-1150">Fix issue #11658: `az group export` command does not support `--query` and `--output` parameters</span></span>
* <span data-ttu-id="018bf-1151">Behebung von Problem Nr. 10279: Der Exitcode von `az group deployment validate` ist 0, wenn bei der Überprüfung ein Fehler auftritt.</span><span class="sxs-lookup"><span data-stu-id="018bf-1151">Fix issue #10279: The exit code of `az group deployment validate` is 0 when the verification fails</span></span>
* <span data-ttu-id="018bf-1152">Behebung von Problem Nr. 9916: Fehlermeldung des Konflikts zwischen Tag und anderen Filterbedingungen für Befehl `az resource list` verbessert</span><span class="sxs-lookup"><span data-stu-id="018bf-1152">Fix issue #9916: Improve the error message of the conflict between tag and other filter conditions for `az resource list` command</span></span>
* <span data-ttu-id="018bf-1153">Neuer Parameter `--managed-by` hinzugefügt, um das Hinzufügen der Informationen vom Typ „managedBy“ für Befehl `az group create` zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="018bf-1153">Add new parameter `--managed-by` to support adding managedBy information for command `az group create`</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="018bf-1154">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="018bf-1154">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="018bf-1155">Untergruppe `monitor` hinzugefügt, um Log Analytics-Überwachung im Azure Red Hat OpenShift-Cluster zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="018bf-1155">Add `monitor` subgroup to manage Log Analytics monitoring in Azure Red Hat OpensShift cluster</span></span>

### <a name="botservice"></a><span data-ttu-id="018bf-1156">BotService</span><span class="sxs-lookup"><span data-stu-id="018bf-1156">BotService</span></span>

* <span data-ttu-id="018bf-1157">Behebung von Problem Nr. 11697: `az bot create` ist nicht idempotent.</span><span class="sxs-lookup"><span data-stu-id="018bf-1157">Fix issue #11697: `az bot create` is not idempotent</span></span>
* <span data-ttu-id="018bf-1158">Tests zur Namenskorrektur geändert, sodass sie nur im Livemodus ausgeführt werden</span><span class="sxs-lookup"><span data-stu-id="018bf-1158">Change name-correcting tests to run in Live-mode only</span></span>

### <a name="cdn"></a><span data-ttu-id="018bf-1159">CDN</span><span class="sxs-lookup"><span data-stu-id="018bf-1159">CDN</span></span>

* <span data-ttu-id="018bf-1160">Unterstützung für das rulesEngine-Feature hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1160">Add support for rulesEngine feature</span></span>
* <span data-ttu-id="018bf-1161">Neue Befehlsgruppe „cdn endpoint rule“ zum Verwalten von Regeln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1161">Add new commands group 'cdn endpoint rule' to manage rules</span></span>
* <span data-ttu-id="018bf-1162">azure-mgmt-cdn-Version auf 4.0.0 aktualisiert, um API-Version 2019-04-15 zu verwenden</span><span class="sxs-lookup"><span data-stu-id="018bf-1162">Update azure-mgmt-cdn version to 4.0.0 to use api version 2019-04-15</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="018bf-1163">Bereitstellungs-Manager</span><span class="sxs-lookup"><span data-stu-id="018bf-1163">Deployment Manager</span></span>

* <span data-ttu-id="018bf-1164">Auflistungsvorgang für alle Ressourcen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1164">Add list operation for all resources.</span></span>
* <span data-ttu-id="018bf-1165">Schrittressource für neuen Schritttyp optimiert</span><span class="sxs-lookup"><span data-stu-id="018bf-1165">Enhance step resource for new step type.</span></span>
* <span data-ttu-id="018bf-1166">Paket „azure-mgmt-deploymentmanager“ zur Verwendung von Version 0.2.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="018bf-1166">Update azure-mgmt-deploymentmanager package to use version 0.2.0.</span></span>

### <a name="iot"></a><span data-ttu-id="018bf-1167">IoT</span><span class="sxs-lookup"><span data-stu-id="018bf-1167">IoT</span></span>

* <span data-ttu-id="018bf-1168">Befehle vom Typ „IoT hub Job“ als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="018bf-1168">Deprecate 'IoT hub Job' commands.</span></span>

### <a name="iot-central"></a><span data-ttu-id="018bf-1169">IoT Central</span><span class="sxs-lookup"><span data-stu-id="018bf-1169">IoT Central</span></span>

* <span data-ttu-id="018bf-1170">Unterstützung der App-Erstellung/-Aktualisierung mit neuem SKU-Namen ST0, ST1, ST2</span><span class="sxs-lookup"><span data-stu-id="018bf-1170">Support app creation/update with the new sku name ST0, ST1, ST2.</span></span>

### <a name="key-vault"></a><span data-ttu-id="018bf-1171">Key Vault</span><span class="sxs-lookup"><span data-stu-id="018bf-1171">Key Vault</span></span>

* <span data-ttu-id="018bf-1172">Neuer Befehl `az keyvault key download` zum Herunterladen von Schlüsseln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1172">Add a new command `az keyvault key download` for downloading keys.</span></span>

### <a name="misc"></a><span data-ttu-id="018bf-1173">Sonstiges</span><span class="sxs-lookup"><span data-stu-id="018bf-1173">Misc</span></span>

* <span data-ttu-id="018bf-1174">Behebung Nr. 6371: Unterstützung für die Vervollständigung von Dateinamen und Umgebungsvariablen in Bash</span><span class="sxs-lookup"><span data-stu-id="018bf-1174">Fix #6371: Support filename and environment variable completion in Bash</span></span>

### <a name="network"></a><span data-ttu-id="018bf-1175">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="018bf-1175">Network</span></span>

* <span data-ttu-id="018bf-1176">Behebung Nr. 2092: az network dns record-set add/remove: Warnung hinzugefügt, wenn Datensatzgruppe nicht gefunden wurde.</span><span class="sxs-lookup"><span data-stu-id="018bf-1176">Fix #2092: az network dns record-set add/remove: add warning when record-set is not found.</span></span> <span data-ttu-id="018bf-1177">In Zukunft wird ein zusätzliches Argument unterstützt, um diese automatische Erstellung zu bestätigen.</span><span class="sxs-lookup"><span data-stu-id="018bf-1177">In the future, an extra argument will be supported to confirm this auto creation.</span></span>

### <a name="policy"></a><span data-ttu-id="018bf-1178">Richtlinie</span><span class="sxs-lookup"><span data-stu-id="018bf-1178">Policy</span></span>

* <span data-ttu-id="018bf-1179">Neuer Befehl `az policy metadata` hinzugefügt, um umfangreiche Richtlinienmetadatenressourcen abzurufen</span><span class="sxs-lookup"><span data-stu-id="018bf-1179">Add new command `az policy metadata` to retrieve rich policy metadata resources</span></span>
* <span data-ttu-id="018bf-1180">`az policy remediation create`: Geben Sie mit dem Parameter `--resource-discovery-mode` an, ob die Konformität vor der Wartung neu bewertet werden soll.</span><span class="sxs-lookup"><span data-stu-id="018bf-1180">`az policy remediation create`: Specify whether compliance should be re-evaluated prior to remediation with the `--resource-discovery-mode` parameter</span></span>

### <a name="profile"></a><span data-ttu-id="018bf-1181">Profil</span><span class="sxs-lookup"><span data-stu-id="018bf-1181">Profile</span></span>

* <span data-ttu-id="018bf-1182">`az account get-access-token`: Parameter `--tenant` hinzugefügt, um das Token für den Mandanten direkt abzurufen. Es muss kein Abonnement angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="018bf-1182">`az account get-access-token`: Add `--tenant` parameter to acquire token for the tenant directly, needless to specify a subscription</span></span>

### <a name="rbac"></a><span data-ttu-id="018bf-1183">RBAC</span><span class="sxs-lookup"><span data-stu-id="018bf-1183">RBAC</span></span>

* <span data-ttu-id="018bf-1184">[BREAKING CHANGE] Behebung Nr. 11883: `az role assignment create`: Bei leerem Bereich wird ein Fehler ausgegeben.</span><span class="sxs-lookup"><span data-stu-id="018bf-1184">[BREAKING CHANGE] Fix #11883: `az role assignment create`: empty scope will prompt error</span></span>

### <a name="security"></a><span data-ttu-id="018bf-1185">Sicherheit</span><span class="sxs-lookup"><span data-stu-id="018bf-1185">Security</span></span>

* <span data-ttu-id="018bf-1186">Neue Befehle `az atp show` und `az atp update` hinzugefügt, um erweiterte Einstellungen für den Bedrohungsschutz für Speicherkonten anzuzeigen und zu verwalten</span><span class="sxs-lookup"><span data-stu-id="018bf-1186">Add new commands `az atp show` and `az atp update` to view and manage advanced threat protection settings for storage accounts.</span></span>

### <a name="sql"></a><span data-ttu-id="018bf-1187">SQL</span><span class="sxs-lookup"><span data-stu-id="018bf-1187">SQL</span></span>

* <span data-ttu-id="018bf-1188">`sql dw create`: Parameter `--zone-redundant` und `--read-replica-count` als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="018bf-1188">`sql dw create`: deprecate `--zone-redundant` and `--read-replica-count` parameters.</span></span> <span data-ttu-id="018bf-1189">Diese Parameter gelten nicht für Datawarehouse.</span><span class="sxs-lookup"><span data-stu-id="018bf-1189">These parameters do not apply to DataWarehouse.</span></span>
* <span data-ttu-id="018bf-1190">[BREAKING CHANGE] `az sql db create`: „WideWorldImportersStd“ und „WideWorldImportersFull“ als dokumentierte zulässige Werte für „az sql db create --sample-name“ entfernt.</span><span class="sxs-lookup"><span data-stu-id="018bf-1190">[BREAKING CHANGE] `az sql db create`: Remove "WideWorldImportersStd" and "WideWorldImportersFull" as documented allowed values for "az sql db create --sample-name".</span></span> <span data-ttu-id="018bf-1191">Diese Beispieldatenbanken führen immer zu einem Fehler bei der Erstellung.</span><span class="sxs-lookup"><span data-stu-id="018bf-1191">These sample databases would always cause creation to fail.</span></span>
* <span data-ttu-id="018bf-1192">Neue Befehle `sql db classification show/list/update/delete` und `sql db classification recommendation list/enable/disable` zur Verwaltung von Vertraulichkeitsklassifizierungen für SQL-Datenbanken hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1192">Add New commands `sql db classification show/list/update/delete` and `sql db classification recommendation list/enable/disable` to manage sensitivity classifications for SQL databases.</span></span>
* <span data-ttu-id="018bf-1193">`az sql db audit-policy`: Behebung für leere Überwachungsaktionen und -gruppen</span><span class="sxs-lookup"><span data-stu-id="018bf-1193">`az sql db audit-policy`: Fix for empty audit actions and groups</span></span>

### <a name="storage"></a><span data-ttu-id="018bf-1194">Storage</span><span class="sxs-lookup"><span data-stu-id="018bf-1194">Storage</span></span>

* <span data-ttu-id="018bf-1195">Neue Befehlsgruppe `az storage share-rm` hinzugefügt, um den Ressourcenanbieter „Microsoft.Storage“ für Verwaltungsvorgänge der Azure-Dateifreigabe zu verwenden</span><span class="sxs-lookup"><span data-stu-id="018bf-1195">Add a new command group `az storage share-rm` to use the Microsoft.Storage resource provider for Azure file share management operations.</span></span>
* <span data-ttu-id="018bf-1196">Behebung für Problem Nr. 11415: Berechtigungsfehler für `az storage blob update`</span><span class="sxs-lookup"><span data-stu-id="018bf-1196">Fix issue #11415: permission error for `az storage blob update`</span></span>
* <span data-ttu-id="018bf-1197">Integration von Azcopy 10.3.3 und Unterstützung von Win32</span><span class="sxs-lookup"><span data-stu-id="018bf-1197">Integrate Azcopy 10.3.3 and support Win32.</span></span>
* <span data-ttu-id="018bf-1198">`az storage copy`: Parameter `--include-path`, `--include-pattern`, `--exclude-path` und`--exclude-pattern` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1198">`az storage copy`: Add `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="018bf-1199">`az storage remove`: Parameter `--inlcude` und `--exclude` in Parameter `--include-path`, `--include-pattern`, `--exclude-path` und`--exclude-pattern` geändert</span><span class="sxs-lookup"><span data-stu-id="018bf-1199">`az storage remove`: Change `--inlcude` and `--exclude` parameters to `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="018bf-1200">`az storage sync`: Parameter `--include-pattern`, `--exclude-path` und`--exclude-pattern` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1200">`az storage sync`: Add `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>

### <a name="servicefabric"></a><span data-ttu-id="018bf-1201">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="018bf-1201">ServiceFabric</span></span>

* <span data-ttu-id="018bf-1202">Neue Befehle zum Verwalten von Anwendung und Diensten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1202">Add new commands to manage appliaction and services.</span></span>

## <a name="january-13-2020"></a><span data-ttu-id="018bf-1203">13. Januar 2020</span><span class="sxs-lookup"><span data-stu-id="018bf-1203">January 13, 2020</span></span>

<span data-ttu-id="018bf-1204">Version 2.0.80</span><span class="sxs-lookup"><span data-stu-id="018bf-1204">Version 2.0.80</span></span>

### <a name="compute"></a><span data-ttu-id="018bf-1205">Compute</span><span class="sxs-lookup"><span data-stu-id="018bf-1205">Compute</span></span>

* <span data-ttu-id="018bf-1206">Datenträgeraktualisierung: „--disk-encryption-set“ und „--encryption-type“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1206">disk update: Add --disk-encryption-set and --encryption-type</span></span>
* <span data-ttu-id="018bf-1207">Momentaufnahmeerstellung/-aktualisierung: „--disk-encryption-set“ und „--encryption-type“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1207">snapshot create/update: Add --disk-encryption-set and --encryption-type</span></span>

### <a name="storage"></a><span data-ttu-id="018bf-1208">Storage</span><span class="sxs-lookup"><span data-stu-id="018bf-1208">Storage</span></span>

* <span data-ttu-id="018bf-1209">„azure-mgmt-storage“ auf Version 7.1.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="018bf-1209">Upgrade azure-mgmt-storage version to 7.1.0</span></span>
* <span data-ttu-id="018bf-1210">`az storage account create`: `--encryption-key-type-for-table` und `--encryption-key-type-for-queue` zur Unterstützung des Tabellen- und Warteschlangenverschlüsselungsdiensts hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1210">`az storage account create`: Add `--encryption-key-type-for-table` and `--encryption-key-type-for-queue` to support Table and Queue Encryption Service</span></span>

## <a name="january-07-2020"></a><span data-ttu-id="018bf-1211">7\. Januar 2020</span><span class="sxs-lookup"><span data-stu-id="018bf-1211">January 07, 2020</span></span>

<span data-ttu-id="018bf-1212">Version 2.0.79</span><span class="sxs-lookup"><span data-stu-id="018bf-1212">Version 2.0.79</span></span>

### <a name="acr"></a><span data-ttu-id="018bf-1213">ACR</span><span class="sxs-lookup"><span data-stu-id="018bf-1213">ACR</span></span>

* <span data-ttu-id="018bf-1214">[BREAKING CHANGE] Parameter „--os“ für „acr build“, „acr task create/update“, „acr run“ und „acr pack“ wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="018bf-1214">[BREAKING CHANGE] Remove '--os' parameter for 'acr build', 'acr task create/update', 'acr run', and 'acr pack'.</span></span> <span data-ttu-id="018bf-1215">Verwenden Sie stattdessen „--platform“.</span><span class="sxs-lookup"><span data-stu-id="018bf-1215">Use '--platform' instead.</span></span>

### <a name="appconfig"></a><span data-ttu-id="018bf-1216">AppConfig</span><span class="sxs-lookup"><span data-stu-id="018bf-1216">AppConfig</span></span>

* <span data-ttu-id="018bf-1217">Unterstützung für das Importieren/Exportieren von Featureflags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1217">Add support for importing/exporting feature flags</span></span>
* <span data-ttu-id="018bf-1218">Neuer Befehl „az appconfig kv set-keyvault“ für das Erstellen einer KeyVault-Referenz hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1218">Add new command 'az appconfig kv set-keyvault' for creating keyvault reference</span></span>
* <span data-ttu-id="018bf-1219">Unterstützung verschiedener Benennungskonventionen beim Exportieren von Featureflags in eine Datei</span><span class="sxs-lookup"><span data-stu-id="018bf-1219">Support various naming conventions when exporting feature flags to file</span></span>

### <a name="appservice"></a><span data-ttu-id="018bf-1220">AppService</span><span class="sxs-lookup"><span data-stu-id="018bf-1220">AppService</span></span>

* <span data-ttu-id="018bf-1221">Behebung von Problem Nr. 7154: Aktualisierung der Dokumentation für Befehl „<>“, sodass Backticks anstelle von einfachen Anführungszeichen verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="018bf-1221">Fix issue #7154: Updating documentation for command <> to use back ticks instead of single quotes</span></span>
* <span data-ttu-id="018bf-1222">Behebung von Problem Nr. 11287: „webapp up“: Für die mit „up“ erstellte App muss standardmäßig SSL aktiviert sein.</span><span class="sxs-lookup"><span data-stu-id="018bf-1222">Fix issue #11287: webapp up: By default make the app created using up 'should be 'SSL enabled'</span></span>
* <span data-ttu-id="018bf-1223">Behebung von Problem Nr. 11592: Flag „az webapp up“ für statische HTML-Websites hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1223">Fix issue #11592: Add az webapp up flag for html static sites</span></span>

### <a name="arm"></a><span data-ttu-id="018bf-1224">ARM</span><span class="sxs-lookup"><span data-stu-id="018bf-1224">ARM</span></span>

* <span data-ttu-id="018bf-1225">Behebung `az resource tag`: Recovery Services-Tresor-Tags können nicht aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="018bf-1225">Fix `az resource tag`: Recovery Services Vault tags cannot be updated</span></span>

### <a name="backup"></a><span data-ttu-id="018bf-1226">Backup</span><span class="sxs-lookup"><span data-stu-id="018bf-1226">Backup</span></span>

* <span data-ttu-id="018bf-1227">Neuer Befehl „backup protection undelete“ hinzugefügt, um die Funktion zum vorläufigen Löschen für IaasVM-Workloads zu aktivieren</span><span class="sxs-lookup"><span data-stu-id="018bf-1227">Added new command 'backup protection undelete' to enable soft-delete feature for IaasVM workload</span></span>
* <span data-ttu-id="018bf-1228">Neuer Parameter „--soft-delete-feature-state“ hinzugefügt, um den Befehl „backup-properties“ festzulegen</span><span class="sxs-lookup"><span data-stu-id="018bf-1228">Added new parameter '--soft-delete-feature-state' to set backup-properties command</span></span>
* <span data-ttu-id="018bf-1229">Unterstützung für den Ausschluss von Datenträgern für IaasVM-Workload hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1229">Added disk exclusion support for IaasVM workload</span></span>

### <a name="compute"></a><span data-ttu-id="018bf-1230">Compute</span><span class="sxs-lookup"><span data-stu-id="018bf-1230">Compute</span></span>

* <span data-ttu-id="018bf-1231">Fehler `vm create` in Azure Stack-Profil behoben.</span><span class="sxs-lookup"><span data-stu-id="018bf-1231">Fix `vm create` failure in Azure Stack profile.</span></span>
* <span data-ttu-id="018bf-1232">vm monitor metrics tail/list-definitions: Unterstützung einer Abfragemetrik und von Listendefinitionen für eine VM.</span><span class="sxs-lookup"><span data-stu-id="018bf-1232">vm monitor metrics tail/list-definitions: support query metric and list definitions for a vm.</span></span>
* <span data-ttu-id="018bf-1233">Neue Aktion des Befehls zum erneuten Anwenden für „az vm“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1233">Add new reapply command action for az vm</span></span>

### <a name="hdinsight"></a><span data-ttu-id="018bf-1234">HDInsight</span><span class="sxs-lookup"><span data-stu-id="018bf-1234">HDInsight</span></span>

* <span data-ttu-id="018bf-1235">Unterstützung für das Erstellen eines Kafka-Clusters mit Kafka-REST-Proxy</span><span class="sxs-lookup"><span data-stu-id="018bf-1235">Support for creating a Kafka cluster with Kafka Rest Proxy</span></span>
* <span data-ttu-id="018bf-1236">„azure-mgmt-hdinsight“ auf 1.3.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="018bf-1236">Upgrade azure-mgmt-hdinsight to 1.3.0</span></span>

### <a name="misc"></a><span data-ttu-id="018bf-1237">Verschiedenes:</span><span class="sxs-lookup"><span data-stu-id="018bf-1237">Misc.</span></span>

* <span data-ttu-id="018bf-1238">Vorschaubefehl `az version show` hinzugefügt, um die Versionen der Azure CLI-Module und Erweiterungen standardmäßig im JSON-Format oder im mit „--output“ konfigurierten Format anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="018bf-1238">Add preview command `az version show` to show the versions of Azure CLI modules and extensions in JSON format by default or format configured by --output</span></span>

### <a name="event-hubs"></a><span data-ttu-id="018bf-1239">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="018bf-1239">Event Hubs</span></span>

* <span data-ttu-id="018bf-1240">[BREAKING CHANGE] Statusoption „ReceiveDisabled“ aus „az eventhubs eventhub update“ und „az eventhubs eventhub create“ entfernt.</span><span class="sxs-lookup"><span data-stu-id="018bf-1240">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az eventhubs eventhub update' and 'az eventhubs eventhub create'.</span></span> <span data-ttu-id="018bf-1241">Diese Option ist für Event Hub-Entitäten nicht gültig.</span><span class="sxs-lookup"><span data-stu-id="018bf-1241">This option is not valid for Event Hub entities.</span></span>

### <a name="service-bus"></a><span data-ttu-id="018bf-1242">Service Bus</span><span class="sxs-lookup"><span data-stu-id="018bf-1242">Service Bus</span></span>

* <span data-ttu-id="018bf-1243">[BREAKING CHANGE] Statusoption „ReceiveDisabled“ aus Befehlen „az servicebus topic create“, „az servicebus topic update“, „az servicebus queue create“ und „az servicebus queue update“ entfernt.</span><span class="sxs-lookup"><span data-stu-id="018bf-1243">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az servicebus topic create', 'az servicebus topic update', 'az servicebus queue create', and 'az servicebus queue update'.</span></span> <span data-ttu-id="018bf-1244">Diese Option ist für Service Bus-Themen und -Warteschlangen nicht gültig.</span><span class="sxs-lookup"><span data-stu-id="018bf-1244">This option is not valid for Service Bus topics and queues.</span></span>

### <a name="rbac"></a><span data-ttu-id="018bf-1245">RBAC</span><span class="sxs-lookup"><span data-stu-id="018bf-1245">RBAC</span></span>

* <span data-ttu-id="018bf-1246">Behebung Nr. 11712: `az ad app/sp show` gibt nicht den Exitcode 3 zurück, wenn die Anwendung oder der Dienstprinzipal nicht vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="018bf-1246">Fix #11712: `az ad app/sp show` does not return exit code 3 when the application or service principal does not exist</span></span>

### <a name="storage"></a><span data-ttu-id="018bf-1247">Storage</span><span class="sxs-lookup"><span data-stu-id="018bf-1247">Storage</span></span>

* <span data-ttu-id="018bf-1248">`az storage account create`: Vorschaukennzeichnung für Parameter „--enable-hierarchical-namespace“ entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-1248">`az storage account create`: Remove preview flag for --enable-hierarchical-namespace parameter</span></span>
* <span data-ttu-id="018bf-1249">azure-mgmt-storage-Version auf 7.0.0 aktualisiert, um API-Version 2019-06-01 zu verwenden</span><span class="sxs-lookup"><span data-stu-id="018bf-1249">Update azure-mgmt-storage version to 7.0.0 to use api version 2019-06-01</span></span>
* <span data-ttu-id="018bf-1250">Neue Parameter `--enable-delete-retention` und `--delete-retention-days` hinzugefügt, um die Verwaltung der Aufbewahrungsrichtlinie für Löschen für „blob-service-properties“ von Speicherkonten zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="018bf-1250">Add new parameters `--enable-delete-retention` and `--delete-retention-days` to support managing delete retention policy for storage account blob-service-properties.</span></span>

## <a name="december-17-2019"></a><span data-ttu-id="018bf-1251">17. Dezember 2019</span><span class="sxs-lookup"><span data-stu-id="018bf-1251">December 17, 2019</span></span>

<span data-ttu-id="018bf-1252">2.0.78</span><span class="sxs-lookup"><span data-stu-id="018bf-1252">2.0.78</span></span>

### <a name="acr"></a><span data-ttu-id="018bf-1253">ACR</span><span class="sxs-lookup"><span data-stu-id="018bf-1253">ACR</span></span>

* <span data-ttu-id="018bf-1254">Unterstützung für lokalen Kontext in „acr task run“</span><span class="sxs-lookup"><span data-stu-id="018bf-1254">Added support Local context in acr task run</span></span>

### <a name="acs"></a><span data-ttu-id="018bf-1255">ACS</span><span class="sxs-lookup"><span data-stu-id="018bf-1255">ACS</span></span>

* <span data-ttu-id="018bf-1256">[BREAKING CHANGE] az openshift create: `--workspace-resource-id` in `--workspace-id` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="018bf-1256">[BREAKING CHANGE]az openshift create: rename `--workspace-resource-id` to `--workspace-id`.</span></span>

### <a name="ams"></a><span data-ttu-id="018bf-1257">AMS</span><span class="sxs-lookup"><span data-stu-id="018bf-1257">AMS</span></span>

* <span data-ttu-id="018bf-1258">Befehle zum Anzeigen aktualisiert, sodass 3 zurückgegeben wird, wenn die Ressource nicht gefunden wurde</span><span class="sxs-lookup"><span data-stu-id="018bf-1258">Updated show commands to return 3 when resource not found</span></span>

### <a name="appconfig"></a><span data-ttu-id="018bf-1259">AppConfig</span><span class="sxs-lookup"><span data-stu-id="018bf-1259">AppConfig</span></span>

* <span data-ttu-id="018bf-1260">Fehler beim Anhängen der API-Version an die Anforderungs-URL korrigiert.</span><span class="sxs-lookup"><span data-stu-id="018bf-1260">Fixed bug when appending api-version to request url.</span></span> <span data-ttu-id="018bf-1261">Die vorhandene Lösung funktioniert nicht mit Paginierung.</span><span class="sxs-lookup"><span data-stu-id="018bf-1261">The existing solution doesn't work with pagination.</span></span>
* <span data-ttu-id="018bf-1262">Unterstützung für die Anzeige von weiteren Sprachen neben Englisch hinzugefügt, da der Back-End-Dienst Unicode für die Globalisierung unterstützt.</span><span class="sxs-lookup"><span data-stu-id="018bf-1262">Added support for showing languages besides English as our backend service support unicode for globalization.</span></span>

### <a name="appservice"></a><span data-ttu-id="018bf-1263">AppService</span><span class="sxs-lookup"><span data-stu-id="018bf-1263">AppService</span></span>

* <span data-ttu-id="018bf-1264">Problem Nr. 11217 behoben: Web-App: „az webapp config ssl upload“ muss Slot-Parameter unterstützen.</span><span class="sxs-lookup"><span data-stu-id="018bf-1264">Fixed issue #11217: webapp: az webapp config ssl upload should support slot parameter</span></span>
* <span data-ttu-id="018bf-1265">Problem Nr. 10965 behoben: Error: Der Name darf nicht leer sein.</span><span class="sxs-lookup"><span data-stu-id="018bf-1265">Fixed issue #10965: Error: Name cannot be empty.</span></span> <span data-ttu-id="018bf-1266">Entfernen anhand von „ip_address“ und „subnet“ zulassen</span><span class="sxs-lookup"><span data-stu-id="018bf-1266">Allow remove by ip_address and subnet</span></span>
* <span data-ttu-id="018bf-1267">Unterstützung des Imports von Zertifikaten aus Key Vault hinzugefügt `az webapp config ssl import`</span><span class="sxs-lookup"><span data-stu-id="018bf-1267">Added support for importing certificates from Key Vault `az webapp config ssl import`</span></span>

### <a name="arm"></a><span data-ttu-id="018bf-1268">ARM</span><span class="sxs-lookup"><span data-stu-id="018bf-1268">ARM</span></span>

* <span data-ttu-id="018bf-1269">Paket „azure-mgmt-resource“ auf die Verwendung von 6.0.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="018bf-1269">Updated azure-mgmt-resource package to use 6.0.0</span></span>
* <span data-ttu-id="018bf-1270">Mandantenübergreifende Unterstützung für Befehl `az group deployment create` durch Hinzufügen des neuen Parameters `--aux-subs`</span><span class="sxs-lookup"><span data-stu-id="018bf-1270">Cross Tenant Support for `az group deployment create` command by adding new parameter `--aux-subs`</span></span>
* <span data-ttu-id="018bf-1271">Neuer Parameter `--metadata` hinzugefügt, um das Hinzufügen von Metadateninformationen für Richtliniensatzdefinitionen zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="018bf-1271">Added new parameter `--metadata` to support adding metadata information for policy set definitions.</span></span>

### <a name="backup"></a><span data-ttu-id="018bf-1272">Backup</span><span class="sxs-lookup"><span data-stu-id="018bf-1272">Backup</span></span>

* <span data-ttu-id="018bf-1273">Unterstützung der Sicherung für SQL- und SAP Hana-Workloads hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-1273">Added Backup support for SQL and SAP Hana workload.</span></span>

### <a name="botservice"></a><span data-ttu-id="018bf-1274">BotService</span><span class="sxs-lookup"><span data-stu-id="018bf-1274">BotService</span></span>

* <span data-ttu-id="018bf-1275">[Breaking Change] Flag „--version“ aus Vorschaubefehl „az bot create“ entfernt.</span><span class="sxs-lookup"><span data-stu-id="018bf-1275">[Breaking change] Remove '--version' flag from preview command 'az bot create'.</span></span> <span data-ttu-id="018bf-1276">Nur v4-SDK-Bots werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="018bf-1276">Only v4 SDK bots are supported.</span></span>
* <span data-ttu-id="018bf-1277">Überprüfung der Namensverfügbarkeit für „az bot create“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-1277">Added name availability check for 'az bot create'.</span></span>
* <span data-ttu-id="018bf-1278">Unterstützung für das Aktualisieren der Symbol-URL für einen Bot über „az bot update“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-1278">Added support for updating the icon URL for a bot via 'az bot update'.</span></span>
* <span data-ttu-id="018bf-1279">Unterstützung für das Aktualisieren eines Direct Line-Kanals über „az bot directline update“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-1279">Added support for updating a Direct Line channel via 'az bot directline update'.</span></span>
* <span data-ttu-id="018bf-1280">Unterstützung für Flag „--enable-enhanced-auth“ zu „az bot directline create“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-1280">Added '--enable-enhanced-auth' flag support to 'az bot directline create'.</span></span>
* <span data-ttu-id="018bf-1281">Die folgenden Befehlsgruppen sind allgemein verfügbar und befinden sich nicht in der Vorschau: „az bot authsetting“.</span><span class="sxs-lookup"><span data-stu-id="018bf-1281">The following command groups are GA and not in preview: 'az bot authsetting'.</span></span>
* <span data-ttu-id="018bf-1282">Die folgenden Befehle in „az bot“ sind allgemein verfügbar und befinden sich nicht in der Vorschau: „create“, „prepare-deploy“, „show“, „delete“, „update“.</span><span class="sxs-lookup"><span data-stu-id="018bf-1282">The following commands in 'az bot' are GA and not in preview: 'create', 'prepare-deploy', 'show', 'delete', 'update'.</span></span>
* <span data-ttu-id="018bf-1283">„az bot prepare-deploy“ korrigiert, indem der Wert voon „--proj-file-path“ in Kleinschreibung geändert wurde (z. B. „Test.csproj“ in „test.csproj“).</span><span class="sxs-lookup"><span data-stu-id="018bf-1283">Fixed 'az bot prepare-deploy' changing '--proj-file-path' value to lower case (e.g. "Test.csproj" to "test.csproj").</span></span>

### <a name="compute"></a><span data-ttu-id="018bf-1284">Compute</span><span class="sxs-lookup"><span data-stu-id="018bf-1284">Compute</span></span>

* <span data-ttu-id="018bf-1285">vmss create/update: „--scale-in-policy“ hinzugefügt, womit entschieden wird, welche virtuellen Computer beim horizontalen Herunterskalieren einer VM-Skalierungsgruppe zum Entfernen ausgewählt werden.</span><span class="sxs-lookup"><span data-stu-id="018bf-1285">vmss create/update: Added --scale-in-policy, which decides which virtual machines are chosen for removal when a VMSS is scaled-in.</span></span>
* <span data-ttu-id="018bf-1286">vm/vmss update: „--priority“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-1286">vm/vmss update: Added --priority.</span></span>
* <span data-ttu-id="018bf-1287">vm/vmss update: „--max-price“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-1287">vm/vmss update: Added --max-price.</span></span>
* <span data-ttu-id="018bf-1288">Befehlsgruppe „disk-encryption-set“ hinzugefügt (create, show, update, delete, list).</span><span class="sxs-lookup"><span data-stu-id="018bf-1288">Added disk-encryption-set command group (create, show, update, delete, list).</span></span>
* <span data-ttu-id="018bf-1289">disk create: „--encryption-type“ und „--disk-encryption-set“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-1289">disk create: Added --encryption-type and --disk-encryption-set.</span></span>
* <span data-ttu-id="018bf-1290">vm/vmss create: „--os-disk-encryption-set“ und „--data-disk-encryption-sets“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-1290">vm/vmss create: Added --os-disk-encryption-set and --data-disk-encryption-sets.</span></span>

### <a name="core"></a><span data-ttu-id="018bf-1291">Core</span><span class="sxs-lookup"><span data-stu-id="018bf-1291">Core</span></span>

* <span data-ttu-id="018bf-1292">Unterstützung für Python 3.4 entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-1292">Removed support for Python 3.4</span></span>
* <span data-ttu-id="018bf-1293">Plug-In für HaTS-Umfrage in mehreren Befehlen</span><span class="sxs-lookup"><span data-stu-id="018bf-1293">Plug in HaTS survey in multiple commands</span></span>

### <a name="dls"></a><span data-ttu-id="018bf-1294">DLS</span><span class="sxs-lookup"><span data-stu-id="018bf-1294">DLS</span></span>

* <span data-ttu-id="018bf-1295">ADLS-SDK-Version aktualisiert (0.0.48).</span><span class="sxs-lookup"><span data-stu-id="018bf-1295">Updated ADLS sdk version (0.0.48).</span></span>

### <a name="install"></a><span data-ttu-id="018bf-1296">Installieren</span><span class="sxs-lookup"><span data-stu-id="018bf-1296">Install</span></span>

* <span data-ttu-id="018bf-1297">Installationsskript unterstützt Python 3.8</span><span class="sxs-lookup"><span data-stu-id="018bf-1297">Install script support python 3.8</span></span>

### <a name="iot"></a><span data-ttu-id="018bf-1298">IoT</span><span class="sxs-lookup"><span data-stu-id="018bf-1298">IOT</span></span>

* <span data-ttu-id="018bf-1299">[BREAKING CHANGE] Parameter „--failover-region“ aus „manual-failover“ entfernt.</span><span class="sxs-lookup"><span data-stu-id="018bf-1299">[BREAKING CHANGE] Removed --failover-region parameter from manual-failover.</span></span> <span data-ttu-id="018bf-1300">Das Failover erfolgt jetzt in eine zugewiesene, geografisch gekoppelte sekundäre Region.</span><span class="sxs-lookup"><span data-stu-id="018bf-1300">Now it will failover to assigned geo-paired secondary region.</span></span>

### <a name="key-vault"></a><span data-ttu-id="018bf-1301">Key Vault</span><span class="sxs-lookup"><span data-stu-id="018bf-1301">Key Vault</span></span>

* <span data-ttu-id="018bf-1302">Nr. 8095 behoben: `az keyvault storage remove`: Hilfemeldung verbessert</span><span class="sxs-lookup"><span data-stu-id="018bf-1302">Fixed #8095: `az keyvault storage remove`: improve the help message</span></span>
* <span data-ttu-id="018bf-1303">Nr. 8921 behoben: `az keyvault key/secret/certificate list/list-deleted/list-versions`: Validierungsfehler in Parameter `--maxresults` behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-1303">Fixed #8921: `az keyvault key/secret/certificate list/list-deleted/list-versions`: fix the validation bug on parameter `--maxresults`</span></span>
* <span data-ttu-id="018bf-1304">Nr. 10512 behoben: `az keyvault set-policy`: Fehlermeldung verbessert, wenn weder `--object-id`, `--spn` noch `--upn` angegeben ist</span><span class="sxs-lookup"><span data-stu-id="018bf-1304">Fixed #10512: `az keyvault set-policy`: improve the error message when none of `--object-id`, `--spn` or `--upn` is specified</span></span>
* <span data-ttu-id="018bf-1305">Nr. 10846 behoben: `az keyvault secret show-deleted`: Wenn `--id` angegeben ist, ist `--name/-n` nicht erforderlich.</span><span class="sxs-lookup"><span data-stu-id="018bf-1305">Fixed #10846: `az keyvault secret show-deleted`: when `--id` is specified, `--name/-n` is not required</span></span>
* <span data-ttu-id="018bf-1306">Nr. 11084 behoben: `az keyvault secret download`: Hilfemeldung von Parameter `--encoding` verbessert</span><span class="sxs-lookup"><span data-stu-id="018bf-1306">Fixed #11084: `az keyvault secret download`: improve the help message of parameter `--encoding`</span></span>

### <a name="network"></a><span data-ttu-id="018bf-1307">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="018bf-1307">Network</span></span>

* <span data-ttu-id="018bf-1308">az network application-gateway probe: Unterstützung für Option „--port“ hinzugefügt, um einen Port zum Prüfen von Back-End-Servern beim Erstellen und Aktualisieren anzugeben</span><span class="sxs-lookup"><span data-stu-id="018bf-1308">az network application-gateway probe: Added support --port option to specify a port for probing backend servers when create and update</span></span>
* <span data-ttu-id="018bf-1309">az network application-gateway url-path-map create/update: Fehlerbehebung für `--waf-policy`</span><span class="sxs-lookup"><span data-stu-id="018bf-1309">az network application-gateway url-path-map create/update: bug fix for `--waf-policy`</span></span>
* <span data-ttu-id="018bf-1310">az network application-gateway: Unterstützung für `--rewrite-rule-set` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1310">az network application-gateway: Added support `--rewrite-rule-set`</span></span>
* <span data-ttu-id="018bf-1311">az network list-service-aliases: Unterstützung für Listendienstaliase hinzugefügt, die für Dienstendpunktrichtlinien verwendet werden können</span><span class="sxs-lookup"><span data-stu-id="018bf-1311">az network list-service-aliases: Added support list service aliases which can be used for Service Endpoint Policies</span></span>
* <span data-ttu-id="018bf-1312">az network dns zone import: Unterstützung für „.@“ in Datensatzname hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1312">az network dns zone import: Added support .@ in record name</span></span>

### <a name="packaging"></a><span data-ttu-id="018bf-1313">Verpackung</span><span class="sxs-lookup"><span data-stu-id="018bf-1313">Packaging</span></span>

* <span data-ttu-id="018bf-1314">Back-Edge-Builds für PIP-Installation hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1314">Added back edge builds for pip install</span></span>
* <span data-ttu-id="018bf-1315">Ubuntu-Eoan-Paket hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1315">Added Ubuntu eoan package</span></span>

### <a name="policy"></a><span data-ttu-id="018bf-1316">Richtlinie</span><span class="sxs-lookup"><span data-stu-id="018bf-1316">Policy</span></span>

* <span data-ttu-id="018bf-1317">Unterstützung für Version 2019-09-01 der Richtlinien-API hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1317">Added support for Policy API version 2019-09-01.</span></span>
* <span data-ttu-id="018bf-1318">az policy set-definition: Unterstützung der Gruppierung innerhalb von Richtliniensatzdefinitionen mit `--definition-groups`-Parameter hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1318">az policy set-definition: Added support grouping within policy set definitions with `--definition-groups` parameter</span></span>

### <a name="redis"></a><span data-ttu-id="018bf-1319">Redis</span><span class="sxs-lookup"><span data-stu-id="018bf-1319">Redis</span></span>

* <span data-ttu-id="018bf-1320">Vorschauparameter `--replicas-per-master` zu Befehl `az redis create`hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1320">Added preview param `--replicas-per-master` to `az redis create` command</span></span>
* <span data-ttu-id="018bf-1321">„azure-mgmt-redis“ von 6.0.0 auf 7.0.0rc1 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="018bf-1321">Updated azure-mgmt-redis from 6.0.0 to 7.0.0rc1</span></span>

### <a name="servicefabric"></a><span data-ttu-id="018bf-1322">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="018bf-1322">ServiceFabric</span></span>

* <span data-ttu-id="018bf-1323">Hinzufügen von Logik in Knotentyp korrigiert, einschließlich Nr. 10963: Beim Hinzufügen eines neuen Knotentyps mit Dauerhaftigkeitsstufe „Gold“ wird immer ein CLI-Fehler ausgegeben.</span><span class="sxs-lookup"><span data-stu-id="018bf-1323">Fixed in node-type add logic including #10963: Adding new node type with durability level Gold will always throw CLI error</span></span>
* <span data-ttu-id="018bf-1324">ServiceFabricNodeVmExt-Version in Erstellungsvorlage auf 1.1 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="018bf-1324">Updated ServiceFabricNodeVmExt version to 1.1 in creation template</span></span>

### <a name="sql"></a><span data-ttu-id="018bf-1325">SQL</span><span class="sxs-lookup"><span data-stu-id="018bf-1325">SQL</span></span>

* <span data-ttu-id="018bf-1326">Parameter „--read-scale“ und „--read-replicas“ zu Befehlen „sql db create“ und „sql db update“ hinzugefügt, um Leseskalierungsverwaltung zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="018bf-1326">Added "--read-scale" and "--read-replicas" parameters to sql db create and update commands, to support read scale management.</span></span>

### <a name="storage"></a><span data-ttu-id="018bf-1327">Storage</span><span class="sxs-lookup"><span data-stu-id="018bf-1327">Storage</span></span>

* <span data-ttu-id="018bf-1328">Allgemein verfügbares Release – Eigenschaft „Large File Shares“ für Befehle „storage account create“ und „storage account update“</span><span class="sxs-lookup"><span data-stu-id="018bf-1328">GA Release Large File Shares property for storage account create and update command</span></span>
* <span data-ttu-id="018bf-1329">Allgemein verfügbares Release – Unterstützung von SAS-Token für die Benutzerdelegierung</span><span class="sxs-lookup"><span data-stu-id="018bf-1329">GA Release User Delegation SAS token Support</span></span>
* <span data-ttu-id="018bf-1330">Neue Befehle `az storage account blob-service-properties show` und `az storage account blob-service-properties update --enable-change-feed` hinzugefügt, um Blob-Diensteigenschaften für das Speicherkonto zu verwalten.</span><span class="sxs-lookup"><span data-stu-id="018bf-1330">Added new commands `az storage account blob-service-properties show` and `az storage account blob-service-properties update --enable-change-feed` to manage blob service properties for storage account.</span></span>
* <span data-ttu-id="018bf-1331">[BEVORSTEHENDER BREAKING CHANGE] `az storage copy`: Das Zeichen `*` wird nicht mehr als Platzhalter in der URL, es werden jedoch die neuen Parameter „--include-pattern“ und „--exclude-pattern“ mit Unterstützung des Platzhalters `*` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-1331">[COMING BREAKING CHANGE] `az storage copy`: `*` character is no longer supported as a wildcard in URL, but new parameters --include-pattern and --exclude-pattern will be added with `*` wildcard support.</span></span>
* <span data-ttu-id="018bf-1332">Problem Nr. 11043 behoben: Unterstützung für das Entfernen des gesamten Containers/der gesamten Freigabe in `az storage remove` Befehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1332">Fixed issue #11043: Added support to remove whole container/share in `az storage remove` command</span></span>

## <a name="november-26-2019"></a><span data-ttu-id="018bf-1333">26. November 2019</span><span class="sxs-lookup"><span data-stu-id="018bf-1333">November 26, 2019</span></span>

<span data-ttu-id="018bf-1334">Version 2.0.77</span><span class="sxs-lookup"><span data-stu-id="018bf-1334">Version 2.0.77</span></span>

### <a name="acr"></a><span data-ttu-id="018bf-1335">ACR</span><span class="sxs-lookup"><span data-stu-id="018bf-1335">ACR</span></span>

* <span data-ttu-id="018bf-1336">Parameter `--branch` in „acr task create/update“ als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="018bf-1336">Deprecated parameter `--branch` from acr task create/update</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="018bf-1337">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="018bf-1337">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="018bf-1338">`--workspace-resource-id`-Flag hinzugefügt, um die Erstellung eines Azure Red Hat OpenShift-Clusters mit Überwachung zuzulassen</span><span class="sxs-lookup"><span data-stu-id="018bf-1338">Added `--workspace-resource-id` flag to allow creation of Azure Red Hat Openshift cluster with monitoring</span></span>
* <span data-ttu-id="018bf-1339">`monitor_profile`-Flag hinzugefügt, um einen Azure Red Hat OpenShift-Clusters mit Überwachung zu erstellen</span><span class="sxs-lookup"><span data-stu-id="018bf-1339">Added `monitor_profile` to create Azure Red Hat OpenShift cluster with monitoring</span></span>

### <a name="aks"></a><span data-ttu-id="018bf-1340">AKS</span><span class="sxs-lookup"><span data-stu-id="018bf-1340">AKS</span></span>

* <span data-ttu-id="018bf-1341">Unterstützung des Rotationsvorgangs für Clusterzertifikate mithilfe von für Cluster Zertifikat Rotation mit „az aks rotate-certs“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-1341">Added support cluster certificate rotation operation using "az aks rotate-certs".</span></span>

### <a name="appconfig"></a><span data-ttu-id="018bf-1342">AppConfig</span><span class="sxs-lookup"><span data-stu-id="018bf-1342">AppConfig</span></span>

* <span data-ttu-id="018bf-1343">Unterstützung für die Verwendung von „:“ für `as az appconfig kv import`-Trennzeichen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1343">Added support for using ":" for `as az appconfig kv import` separator</span></span>
* <span data-ttu-id="018bf-1344">Problem beim Auflisten von Schlüsselwerten mit mehreren Bezeichnungen, einschließlich NULL-Bezeichnung, behoben.</span><span class="sxs-lookup"><span data-stu-id="018bf-1344">Fixed issue for listing key values with multiple labels including null label.</span></span> 
* <span data-ttu-id="018bf-1345">Verwaltungsebenen-SDK, „azure-mgmt-appconfiguration“, auf Version 0.3.0 aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="018bf-1345">Updated management plane sdk, azure-mgmt-appconfiguration, to version 0.3.0.</span></span> 

### <a name="appservice"></a><span data-ttu-id="018bf-1346">AppService</span><span class="sxs-lookup"><span data-stu-id="018bf-1346">AppService</span></span>

* <span data-ttu-id="018bf-1347">Problem Nr. 11100 behoben AttributeError für „az webapp up“ beim Erstellen eines Dienstplans</span><span class="sxs-lookup"><span data-stu-id="018bf-1347">Fixed issue #11100: AttributeError for az webapp up when create service plan</span></span>
* <span data-ttu-id="018bf-1348">az webapp up: Erzwingen der Erstellung oder Bereitstellung auf einer Website für unterstützte Sprachen, es werden keine Standardeinstellungen verwendet.</span><span class="sxs-lookup"><span data-stu-id="018bf-1348">az webapp up: Forcing the creation or deployment to a site for supported languages, no defaults used.</span></span>
* <span data-ttu-id="018bf-1349">Unterstützung für App Service-Umgebung hinzugefügt: az appservice ase show | list | list-addresses | list-plans | create | update | delete</span><span class="sxs-lookup"><span data-stu-id="018bf-1349">Added support for App Service Environment: az appservice ase show | list | list-addresses | list-plans | create | update | delete</span></span>

### <a name="backup"></a><span data-ttu-id="018bf-1350">Backup</span><span class="sxs-lookup"><span data-stu-id="018bf-1350">Backup</span></span>

* <span data-ttu-id="018bf-1351">Problem in Az-Sicherungsrichtlinie „list-associated-items“ behoben.</span><span class="sxs-lookup"><span data-stu-id="018bf-1351">Fixed issue in az backup policy list-associated-items.</span></span> <span data-ttu-id="018bf-1352">Optionaler Parameter „BackupManagementType“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-1352">Added optional BackupManagementType parameter.</span></span>

### <a name="compute"></a><span data-ttu-id="018bf-1353">Compute</span><span class="sxs-lookup"><span data-stu-id="018bf-1353">Compute</span></span>

* <span data-ttu-id="018bf-1354">API-Version von Compute, Datenträger, Momentaufnahmen auf 2019-07-01 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="018bf-1354">Upgraded API version of compute, disks, snapshots to 2019-07-01</span></span>
* <span data-ttu-id="018bf-1355">vmss create: Verbesserung für – Orchestrierungsmodus</span><span class="sxs-lookup"><span data-stu-id="018bf-1355">vmss create: Improvement for --orchestration-mode</span></span>
* <span data-ttu-id="018bf-1356">sig image-definition create: „--os-state“ hinzugefügt, um die Angabe zu ermöglichen, ob die unter diesem Image erstellten virtuellen Computer „generalisiert“ oder „spezialisiert“ sind</span><span class="sxs-lookup"><span data-stu-id="018bf-1356">sig image-definition create: Added --os-state to allow specifying whether the virtual machines created under this image are 'Generalized' or 'Specialized'</span></span>
* <span data-ttu-id="018bf-1357">sig image-definition create: „--hyper-v-generation“ hinzugefügt, um die Angabe der Hypervisorgeneration zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="018bf-1357">sig image-definition create: Added --hyper-v-generation to allow specifying the hypervisor generation</span></span>
* <span data-ttu-id="018bf-1358">sig image-version create: Unterstützung für „--os-snapshot“ und „--data-snapshots“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1358">sig image-version create: Added support --os-snapshot and --data-snapshots</span></span>
* <span data-ttu-id="018bf-1359">image create: „--data-disk-caching“ hinzugefügt, um die Angabe der Zwischenspeicherungseinstellung von Datenträger zu ermöflichen</span><span class="sxs-lookup"><span data-stu-id="018bf-1359">image create: Added --data-disk-caching to allow specifying caching setting of data disks</span></span>
* <span data-ttu-id="018bf-1360">Upgrade des Python-Compute-SDK auf 10.0.0</span><span class="sxs-lookup"><span data-stu-id="018bf-1360">Upgraded Python Compute SDK to 10.0.0</span></span>
* <span data-ttu-id="018bf-1361">vm/vmss create: „Spot“ zu Aufzählungseigenschaft „Priority“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1361">vm/vmss create: Added 'Spot' to 'Priority' enum property</span></span>
* <span data-ttu-id="018bf-1362">[Breaking Change] Parameter „--max-billing“ für sowohl VM als auch VMSS in „--max-price“ umbenannt, um die Konsistenz mit Swagger- und PowerShell-Cmdlets sicherzustellen</span><span class="sxs-lookup"><span data-stu-id="018bf-1362">[Breaking change] Renamed '--max-billing' parameter to '--max-price', for both VM and VMSS, to be consistent with Swagger and Powershell cmdlets</span></span>
* <span data-ttu-id="018bf-1363">vm monitor log show: Unterstützung für das Abfragen von Protokollen über verknüpften Protokollanalyse-Arbeitsbereich hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-1363">vm monitor log show: Added support for querying log over linked log analytics workspace.</span></span>

### <a name="iot"></a><span data-ttu-id="018bf-1364">IoT</span><span class="sxs-lookup"><span data-stu-id="018bf-1364">IOT</span></span>

* <span data-ttu-id="018bf-1365">Behebung Nr. 2531: Argumente für Benutzerfreundlichkeit für Hub-Update hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-1365">Fix #2531: Added convenience arguments for hub update.</span></span>
* <span data-ttu-id="018bf-1366">Behebung Nr. 8323: Fehlende Parameter zum Erstellen eines benutzerdefinierten Speicherendpunkts hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-1366">Fix #8323: Added missing parameters to create storage custom endpoint.</span></span>
* <span data-ttu-id="018bf-1367">Regressionsfehler behoben: Die Änderungen wurden rückgängig gemacht, sodass der standardmäßige Speicherendpunkt überschrieben wurde.</span><span class="sxs-lookup"><span data-stu-id="018bf-1367">Fix regression bug: Reverted the changes which overrides the default storage endpoint.</span></span>

### <a name="key-vault"></a><span data-ttu-id="018bf-1368">Key Vault</span><span class="sxs-lookup"><span data-stu-id="018bf-1368">Key Vault</span></span>

* <span data-ttu-id="018bf-1369">Nr. 11121 behoben: Bei der Verwendung von `az keyvault certificate list` erfordert die Übergabe von `--include-pending` jetzt nicht mehr den Wert `true` oder `false`.</span><span class="sxs-lookup"><span data-stu-id="018bf-1369">Fixed #11121: When using `az keyvault certificate list`, passing `--include-pending` now doesn't require a value of `true` or `false`</span></span>

### <a name="netappfiles"></a><span data-ttu-id="018bf-1370">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="018bf-1370">NetAppFiles</span></span>

* <span data-ttu-id="018bf-1371">Upgrade von „azure-mgmt-netapp“ auf Version 0.7.0, die einige zusätzliche Volumeeigenschaften enthält, die bevorstehenden Replikationsvorgängen zugeordnet sind</span><span class="sxs-lookup"><span data-stu-id="018bf-1371">Upgraded azure-mgmt-netapp to 0.7.0 which includes some additional volume properties associated with upcoming replication operations</span></span>

### <a name="network"></a><span data-ttu-id="018bf-1372">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="018bf-1372">Network</span></span>

* <span data-ttu-id="018bf-1373">application-gateway waf-config: veraltet</span><span class="sxs-lookup"><span data-stu-id="018bf-1373">application-gateway waf-config: deprecated</span></span>
* <span data-ttu-id="018bf-1374">application-gateway waf-policy: Untergruppe „managed-rules“ zur Verwaltung von verwalteten Regelsätzen und Ausschlussregeln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1374">application-gateway waf-policy: Added subgroup managed-rules to manage managed rule sets and exclusion rules</span></span>
* <span data-ttu-id="018bf-1375">application-gateway waf-policy: Untergruppe „policy-setting“ zur Verwaltung der globalen Konfiguration von „waf-policy“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1375">application-gateway waf-policy: Added subgroup policy-setting to manage global configuration of a waf-policy</span></span>
* <span data-ttu-id="018bf-1376">[BREAKING CHANGE] application-gateway waf-policy: Untergruppenregel in „custom-rule“ umbenannt</span><span class="sxs-lookup"><span data-stu-id="018bf-1376">[BREAKING CHANGE] application-gateway waf-policy: Renamed subgroup rule to custom-rule</span></span>
* <span data-ttu-id="018bf-1377">application-gateway http-listener: „--firewall-policy“ beim Erstellen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1377">application-gateway http-listener: Added --firewall-policy when create</span></span>
* <span data-ttu-id="018bf-1378">application-gateway url-path-map rule: „--firewall-policy“ beim Erstellen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1378">application-gateway url-path-map rule: Added --firewall-policy when create</span></span>

### <a name="packaging"></a><span data-ttu-id="018bf-1379">Verpackung</span><span class="sxs-lookup"><span data-stu-id="018bf-1379">Packaging</span></span>

* <span data-ttu-id="018bf-1380">Az-Wrapper in Python neu geschrieben</span><span class="sxs-lookup"><span data-stu-id="018bf-1380">Rewrote the az wrapper in Python</span></span>
* <span data-ttu-id="018bf-1381">Unterstützung für Python 3.8 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1381">Added support for Python 3.8</span></span>
* <span data-ttu-id="018bf-1382">Für RPM-Paket in Python 3 geändert</span><span class="sxs-lookup"><span data-stu-id="018bf-1382">Changed to Python 3 for RPM package</span></span>

### <a name="profile"></a><span data-ttu-id="018bf-1383">Profil</span><span class="sxs-lookup"><span data-stu-id="018bf-1383">Profile</span></span>

* <span data-ttu-id="018bf-1384">Fehler beim Ausführen von `az login -u {} -p {}` mit Microsoft-Konto entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-1384">Polished error when running `az login -u {} -p {}` with Microsoft account</span></span>
* <span data-ttu-id="018bf-1385">`SSLError` beim Ausführen von `az login` hinter einem Proxy mit einem selbstsignierten Stammzertifikat entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-1385">Polished `SSLError` when running `az login` behind a proxy with self-signed root certificate</span></span>
* <span data-ttu-id="018bf-1386">Nr. 10578 behoben: `az login` hängt, wenn mehrere Instanzen gleichzeitig unter Windows oder WSL gestartet werden.</span><span class="sxs-lookup"><span data-stu-id="018bf-1386">Fixed #10578: `az login` hangs when more than one instances are launched at the same time on Windows or WSL</span></span>
* <span data-ttu-id="018bf-1387">Nr. 11059 behoben: `az login --allow-no-subscriptions` schlägt fehl, wenn Abonnements im Mandanten vorhanden sind.</span><span class="sxs-lookup"><span data-stu-id="018bf-1387">Fixed #11059: `az login --allow-no-subscriptions` fails if there are subscriptions in the tenant</span></span>
* <span data-ttu-id="018bf-1388">Nr. 11238 behoben: Nach dem Umbenennen eines Abonnements führt die Anmeldung mit MSI dazu, dass das gleiche Abonnement zweimal angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="018bf-1388">Fixed #11238: After renaming a subscription, logging in with MSI will result in the same subscription appearing twice</span></span>

### <a name="rbac"></a><span data-ttu-id="018bf-1389">RBAC</span><span class="sxs-lookup"><span data-stu-id="018bf-1389">RBAC</span></span>

* <span data-ttu-id="018bf-1390">Nr. 10996 behoben: Fehler für `--force-change-password-next-login` in `az ad user update` entfernt, wenn `--password` nicht angegeben ist</span><span class="sxs-lookup"><span data-stu-id="018bf-1390">Fixed #10996: Polish error for `--force-change-password-next-login` in `az ad user update` when `--password` is not specified</span></span>

### <a name="redis"></a><span data-ttu-id="018bf-1391">Redis</span><span class="sxs-lookup"><span data-stu-id="018bf-1391">Redis</span></span>

* <span data-ttu-id="018bf-1392">Nr. 2902 behoben: Festlegen von Speicherkonfigurationen beim Aktualisieren des Basic-SKU-Cache vermeiden</span><span class="sxs-lookup"><span data-stu-id="018bf-1392">Fixed #2902: Avoid setting memory configs while updating Basic SKU cache</span></span>

### <a name="reservations"></a><span data-ttu-id="018bf-1393">Reservations</span><span class="sxs-lookup"><span data-stu-id="018bf-1393">Reservations</span></span>

* <span data-ttu-id="018bf-1394">SDK-Version auf 0.6.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="018bf-1394">Upgraded SDK Version to 0.6.0</span></span>
* <span data-ttu-id="018bf-1395">Abrechnungsplandetails nach dem Aufrufen von „Get-Gatalogs“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1395">Added billingplan details info after calling Get-Gatalogs</span></span>
* <span data-ttu-id="018bf-1396">Neuer Befehl `az reservations reservation-order calculate` zum Berechnen des Preises für eine Reservierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1396">Added new command `az reservations reservation-order calculate` to calculate the price for a reservation</span></span>
* <span data-ttu-id="018bf-1397">Neuer Befehl `az reservations reservation-order purchase` zum Erwerb einer neuen Reservierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1397">Added new command `az reservations reservation-order purchase` to purchase a new reservation</span></span>

### <a name="rest"></a><span data-ttu-id="018bf-1398">REST</span><span class="sxs-lookup"><span data-stu-id="018bf-1398">Rest</span></span>
* <span data-ttu-id="018bf-1399">`az rest` in allgemeine Verfügbarkeit geändert</span><span class="sxs-lookup"><span data-stu-id="018bf-1399">Changed `az rest` to GA</span></span>

### <a name="sql"></a><span data-ttu-id="018bf-1400">SQL</span><span class="sxs-lookup"><span data-stu-id="018bf-1400">SQL</span></span>

* <span data-ttu-id="018bf-1401">„azure-mgmt-sql“ auf Version 0.15.0 aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="018bf-1401">Updated azure-mgmt-sql to version 0.15.0.</span></span>

### <a name="storage"></a><span data-ttu-id="018bf-1402">Storage</span><span class="sxs-lookup"><span data-stu-id="018bf-1402">Storage</span></span>

* <span data-ttu-id="018bf-1403">storage account create: „--enable-hierarchical-namespace“ hinzugefügt, um Dateisystemsemantik in Blobdienst zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="018bf-1403">storage account create: Added --enable-hierarchical-namespace to support filesystem semantics in blob service.</span></span>
* <span data-ttu-id="018bf-1404">Ausnahme ohne Zusammenhang aus Fehlermeldung entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-1404">Removed unrelated exception from error message</span></span>
* <span data-ttu-id="018bf-1405">Probleme mit falscher Fehlermeldung „Sie verfügen nicht über die erforderlichen Berechtigungen zum Ausführen dieses Vorgangs“ behoben.</span><span class="sxs-lookup"><span data-stu-id="018bf-1405">Fixed issues with incorrect error message "You do not have the required permissions needed to perform this operation."</span></span> <span data-ttu-id="018bf-1406">bei Blockierung durch Netzwerkregeln oder bei „AuthenticationFailed“.</span><span class="sxs-lookup"><span data-stu-id="018bf-1406">when blocked by network rules or AuthenticationFailed.</span></span>

## <a name="november-4-2019"></a><span data-ttu-id="018bf-1407">4\. November 2019</span><span class="sxs-lookup"><span data-stu-id="018bf-1407">November 4, 2019</span></span>

<span data-ttu-id="018bf-1408">Version 2.0.76</span><span class="sxs-lookup"><span data-stu-id="018bf-1408">Version 2.0.76</span></span>

### <a name="acr"></a><span data-ttu-id="018bf-1409">ACR</span><span class="sxs-lookup"><span data-stu-id="018bf-1409">ACR</span></span>

* <span data-ttu-id="018bf-1410">Vorschauparameter `--pack-image-tag` wurde dem Befehl `az acr pack build` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-1410">Added a preview parameter `--pack-image-tag` to command `az acr pack build`.</span></span>
* <span data-ttu-id="018bf-1411">Unterstützung der Aktivierung der Überwachung beim Erstellen einer Registrierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1411">Added support for enabling auditing on creating a registry</span></span>
* <span data-ttu-id="018bf-1412">Unterstützung von RBAC mit Repositoryumfang hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1412">Added support for Repository-scoped RBAC</span></span>

### <a name="aks"></a><span data-ttu-id="018bf-1413">AKS</span><span class="sxs-lookup"><span data-stu-id="018bf-1413">AKS</span></span>

* <span data-ttu-id="018bf-1414">`--enable-cluster-autoscaler`, `--min-count` und `--max-count` wurden dem Befehl `az aks create` hinzugefügt, sodass die automatische Clusterskalierung für den Knotenpool aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="018bf-1414">Added `--enable-cluster-autoscaler`, `--min-count` and `--max-count` to the `az aks create` command, which enables cluster autoscaler for the node pool.</span></span>
* <span data-ttu-id="018bf-1415">Die obigen Flags sowie `--update-cluster-autoscaler` und `--disable-cluster-autoscaler` wurden dem Befehl `az aks update` hinzugefügt, sodass Updates der automatischen Clusterskalierung zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="018bf-1415">Added the above flags as well as `--update-cluster-autoscaler` and `--disable-cluster-autoscaler` to the `az aks update` command, allowing updates to cluster autoscaler.</span></span>

### <a name="appconfig"></a><span data-ttu-id="018bf-1416">AppConfig</span><span class="sxs-lookup"><span data-stu-id="018bf-1416">AppConfig</span></span>

* <span data-ttu-id="018bf-1417">Befehlsgruppe der AppConfig-Funktion zum Verwalten von in einer App Configuration-Instanz gespeicherten Featureflags wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-1417">Added appconfig feature command group to manage feature flags stored in an App Configuration.</span></span>
* <span data-ttu-id="018bf-1418">Geringfügiger Programmfehler für Befehl „appconfig kv export to file“ wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="018bf-1418">Fixed minor bug for appconfig kv export to file command.</span></span> <span data-ttu-id="018bf-1419">Das Lesen der Zieldateiinhalte wird während des Exports angehalten.</span><span class="sxs-lookup"><span data-stu-id="018bf-1419">Stop reading dest file contents during export.</span></span>

### <a name="appservice"></a><span data-ttu-id="018bf-1420">AppService</span><span class="sxs-lookup"><span data-stu-id="018bf-1420">AppService</span></span>

* <span data-ttu-id="018bf-1421">`az appservice plan create`: Unterstützung für das Festlegen von „persitescalung“ beim Erstellen eines App-Serviceplans wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-1421">`az appservice plan create`: Added support to set 'persitescaling' on appservice plan create.</span></span>
* <span data-ttu-id="018bf-1422">Ein Problem wurde behoben, aufgrund dessen der Vorgang „webapp config ssl bind“ vorhandene Tags aus der Ressource entfernt hat.</span><span class="sxs-lookup"><span data-stu-id="018bf-1422">Fixed an issue where webapp config ssl bind operation was removing existing tags from the resource</span></span>
* <span data-ttu-id="018bf-1423">Flag `--build-remote` wurde für `az functionapp deployment source config-zip` hinzugefügt, um die Remotebuildaktion während der Funktions-App-Bereitstellung zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="018bf-1423">Added `--build-remote` flag for `az functionapp deployment source config-zip` to support remote build action during function app deployment.</span></span>
* <span data-ttu-id="018bf-1424">Die Standardknotenversion in Funktions-Apps wurde für Windows in ~ 10 geändert.</span><span class="sxs-lookup"><span data-stu-id="018bf-1424">Changed default node version on function apps to ~10 for Windows</span></span>
* <span data-ttu-id="018bf-1425">`--runtime-version`-Eigenschaft zu `az functionapp create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1425">Added `--runtime-version` property to `az functionapp create`</span></span>

### <a name="arm"></a><span data-ttu-id="018bf-1426">ARM</span><span class="sxs-lookup"><span data-stu-id="018bf-1426">ARM</span></span>

* <span data-ttu-id="018bf-1427">`az deployment/group deployment validate`: Parameter `--handle-extended-json-format` wurde hinzugefügt, um bei der Bereitstellung mehrere Zeilen und Kommentare in der JSON-Vorlage zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="018bf-1427">`az deployment/group deployment validate`: Added `--handle-extended-json-format` parameter to support multiline and comments in json template when deployment.</span></span>
* <span data-ttu-id="018bf-1428">„azure-mgmt-resource“ auf „2019-07-01“ festgelegt</span><span class="sxs-lookup"><span data-stu-id="018bf-1428">Bumped azure-mgmt-resource to 2019-07-01</span></span>

### <a name="backup"></a><span data-ttu-id="018bf-1429">Backup</span><span class="sxs-lookup"><span data-stu-id="018bf-1429">Backup</span></span>

* <span data-ttu-id="018bf-1430">Unterstützung für AzureFiles-Sicherung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1430">Added AzureFiles backup support</span></span>

### <a name="compute"></a><span data-ttu-id="018bf-1431">Compute</span><span class="sxs-lookup"><span data-stu-id="018bf-1431">Compute</span></span>

* <span data-ttu-id="018bf-1432">`az vm create`: Beim gleichzeitigen Festlegen von beschleunigtem Netzwerkbetrieb und einer vorhandenen NIC wurde eine Warnung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-1432">`az vm create`: Added warning when specifying accelerated networking and an existing NIC together.</span></span>
* <span data-ttu-id="018bf-1433">`az vm create`: `--vmss` hinzugefügt, um eine vorhandene VM-Skalierungsgruppe anzugeben, welcher der virtuelle Computer zugewiesen werden soll.</span><span class="sxs-lookup"><span data-stu-id="018bf-1433">`az vm create`: Added `--vmss` to specify an existing virtual machine scale set that the virtual machine should be assigned to.</span></span>
* <span data-ttu-id="018bf-1434">`az vm/vmss create`: Eine lokale Kopie der Imagealiasdatei wurde hinzugefügt, sodass in einer eingeschränkten Netzwerkumgebung darauf zugegriffen werden kann.</span><span class="sxs-lookup"><span data-stu-id="018bf-1434">`az vm/vmss create`: Added a local copy of image alias file so that it can be accessed in a restricted network environment.</span></span>
* <span data-ttu-id="018bf-1435">`az vmss create`: `--orchestration-mode` hinzugefügt, um anzugeben, wie virtuelle Computer von der Skalierungsgruppe verwaltet werden.</span><span class="sxs-lookup"><span data-stu-id="018bf-1435">`az vmss create`: Added `--orchestration-mode` to specify how virtual machines are managed by the scale set.</span></span>
* <span data-ttu-id="018bf-1436">`az vm/vmss update`: `--ultra-ssd-enabled` hinzugefügt, um das Aktualisieren der SSD-Einstellung zuzulassen.</span><span class="sxs-lookup"><span data-stu-id="018bf-1436">`az vm/vmss update`: Added `--ultra-ssd-enabled` to allow updating ultra SSD setting.</span></span>
* <span data-ttu-id="018bf-1437">[BREAKING CHANGE] `az vm extension set`: Ein Fehler wurde behoben, aufgrund dessen Benutzer mit `--ids` keine Erweiterung auf einem virtuellen Computer festlegen konnten.</span><span class="sxs-lookup"><span data-stu-id="018bf-1437">[BREAKING CHANGE] `az vm extension set`: Fixed bug where users could not set an extension on a VM with `--ids`.</span></span>
* <span data-ttu-id="018bf-1438">Neue Befehle wurden zu `az vm image terms accept/cancel/show` hinzugefügt , um Azure Marketplace-Imagebedingungen zu verwalten.</span><span class="sxs-lookup"><span data-stu-id="018bf-1438">Added new commands `az vm image terms accept/cancel/show` to manage Azure Marketplace image terms.</span></span>
* <span data-ttu-id="018bf-1439">VMAccessForLinux auf Version 1.5 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="018bf-1439">Updated VMAccessForLinux to version 1.5</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="018bf-1440">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="018bf-1440">CosmosDB</span></span>

* <span data-ttu-id="018bf-1441">[BREAKING CHANGE] `az sql container create`: `--partition-key-path` in erforderlichen Parameter geändert</span><span class="sxs-lookup"><span data-stu-id="018bf-1441">[BREAKING CHANGE] `az sql container create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="018bf-1442">[BREAKING CHANGE] `az gremlin graph create`: `--partition-key-path` in erforderlichen Parameter geändert</span><span class="sxs-lookup"><span data-stu-id="018bf-1442">[BREAKING CHANGE] `az gremlin graph create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="018bf-1443">`az sql container create`: `--unique-key-policy` und `--conflict-resolution-policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1443">`az sql container create`: Added `--unique-key-policy` and `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="018bf-1444">`az sql container create/update`: Aktualisierung des `--idx`-Standardschemas</span><span class="sxs-lookup"><span data-stu-id="018bf-1444">`az sql container create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="018bf-1445">`gremlin graph create`: `--conflict-resolution-policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1445">`gremlin graph create`: Added `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="018bf-1446">`gremlin graph create/update`: Aktualisierung des `--idx`-Standardschemas</span><span class="sxs-lookup"><span data-stu-id="018bf-1446">`gremlin graph create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="018bf-1447">Tippfehler in Hilfemeldung korrigiert</span><span class="sxs-lookup"><span data-stu-id="018bf-1447">Fixed typo in help message</span></span>
* <span data-ttu-id="018bf-1448">Datenbank: Informationen zur eingestellten Unterstützung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1448">database: Added deprecation information</span></span>
* <span data-ttu-id="018bf-1449">Auflistung: Informationen zur eingestellten Unterstützung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1449">collection: Added deprecation information</span></span>

### <a name="iot"></a><span data-ttu-id="018bf-1450">IoT</span><span class="sxs-lookup"><span data-stu-id="018bf-1450">IoT</span></span>

* <span data-ttu-id="018bf-1451">Neuer Routingquelltyp hinzugefügt: DigitalTwinChangeEvents</span><span class="sxs-lookup"><span data-stu-id="018bf-1451">Added new routing source type: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="018bf-1452">Fehlende Features in `az iot hub create` behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-1452">Fixed missing features in `az iot hub create`</span></span>

### <a name="key-vault"></a><span data-ttu-id="018bf-1453">Key Vault</span><span class="sxs-lookup"><span data-stu-id="018bf-1453">Key Vault</span></span>

* <span data-ttu-id="018bf-1454">Ein unerwarteter Fehler wurde behoben, bei dem keine Zertifikatdatei vorhanden war.</span><span class="sxs-lookup"><span data-stu-id="018bf-1454">Fixed an unexpected error when certificate file does not exist</span></span>
* <span data-ttu-id="018bf-1455">Funktionsunfähigkeit von `az keyvault recover/purge` behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-1455">Fixed `az keyvault recover/purge` not working</span></span>

### <a name="netappfiles"></a><span data-ttu-id="018bf-1456">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="018bf-1456">NetAppFiles</span></span>

* <span data-ttu-id="018bf-1457">„azure-mgmt-netapp“ wurde auf 0.6.0 aktualisiert, um API-Version 2019-07-01 zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="018bf-1457">Upgraded azure-mgmt-netapp to 0.6.0 to use API version 2019-07-01.</span></span> <span data-ttu-id="018bf-1458">Diese neue API-Version umfasst:</span><span class="sxs-lookup"><span data-stu-id="018bf-1458">This new API version includes:</span></span>

    - <span data-ttu-id="018bf-1459">Volumeerstellung `--protocol-types` akzeptiert jetzt „NFSv4.1“ anstelle von „NFSv4“.</span><span class="sxs-lookup"><span data-stu-id="018bf-1459">Volume creation `--protocol-types` accepts now "NFSv4.1" not "NFSv4"</span></span>
    - <span data-ttu-id="018bf-1460">Die Richtlinie der Volumeexportrichtlinie heißt jetzt „nfsv41“ anstelle von „nfsv4“.</span><span class="sxs-lookup"><span data-stu-id="018bf-1460">Volume export policy property now named 'nfsv41' not 'nfsv4'</span></span>
    - <span data-ttu-id="018bf-1461">Volume `--creation-token` wurde in `--file-path` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="018bf-1461">Volume `--creation-token` renamed to `--file-path`</span></span>
    - <span data-ttu-id="018bf-1462">Das Erstellungsdatum einer Momentaufnahme heißt jetzt einfach „erstellt“.</span><span class="sxs-lookup"><span data-stu-id="018bf-1462">Snapshot creation date now named just 'created'</span></span>

### <a name="network"></a><span data-ttu-id="018bf-1463">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="018bf-1463">Network</span></span>

* <span data-ttu-id="018bf-1464">`az network private-dns link vnet create/update`: Unterstützung für mandantenübergreifende Verknüpfung virtueller Netzwerke.</span><span class="sxs-lookup"><span data-stu-id="018bf-1464">`az network private-dns link vnet create/update`: Support cross-tenant virtual network linking.</span></span>
* <span data-ttu-id="018bf-1465">[BREAKING CHANGE] `az network vnet subnet list`: `--resource-group` und `--vnet-name` wurden geändert und sind jetzt erforderlich.</span><span class="sxs-lookup"><span data-stu-id="018bf-1465">[BREAKING CHANGE] `az network vnet subnet list`: Changed `--resource-group` and `--vnet-name` to be required now.</span></span>
* <span data-ttu-id="018bf-1466">`az network public-ip prefix create`: Unterstützung der Angabe der IP-Adressversion (IPv4, IPv6) bei der Erstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1466">`az network public-ip prefix create`: Added support to specify IP address version (IPv4, IPv6) when creation</span></span>
* <span data-ttu-id="018bf-1467">„azure-mgmt-network“ auf 7.0.0 und „api-version“ auf 2019-09-01 festgelegt</span><span class="sxs-lookup"><span data-stu-id="018bf-1467">Bumped azure-mgmt-network to 7.0.0 and api-version to 2019-09-01</span></span>
* <span data-ttu-id="018bf-1468">`az network vrouter`: Unterstützung für neuen virtuellen Dienstrouter und virtuelles Routerpeering hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1468">`az network vrouter`: Added support for new service virtual router and virtual router peering</span></span>
* <span data-ttu-id="018bf-1469">`az network express-route gateway connection`: Unterstützung für `--internet-security` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-1469">`az network express-route gateway connection`: Added support for `--internet-security`</span></span>

### <a name="profile"></a><span data-ttu-id="018bf-1470">Profil</span><span class="sxs-lookup"><span data-stu-id="018bf-1470">Profile</span></span>

* <span data-ttu-id="018bf-1471">Funktionsunfähigkeit von `az account get-access-token --resource-type ms-graph` behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-1471">Fixed `az account get-access-token --resource-type ms-graph` not working</span></span>
* <span data-ttu-id="018bf-1472">Warnung aus `az login` entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-1472">Removed warning from `az login`</span></span>

### <a name="rbac"></a><span data-ttu-id="018bf-1473">RBAC</span><span class="sxs-lookup"><span data-stu-id="018bf-1473">RBAC</span></span>

* <span data-ttu-id="018bf-1474">Funktionsunfähigkeit von `az ad app update --id {} --display-name {}` behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-1474">Fixed `az ad app update --id {} --display-name {}` doesn't work</span></span>

### <a name="servicefabric"></a><span data-ttu-id="018bf-1475">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="018bf-1475">ServiceFabric</span></span>

* <span data-ttu-id="018bf-1476">`az sf cluster create`: Ein Problem wurde behoben, indem die Compute-VMSS von „template.json“ für Service Fabric unter Linux und Windows von Standarddatenträgern auf verwaltete Datenträger umgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="018bf-1476">`az sf cluster create`: Fixed an issue by modifying service fabric linux and windows template.json compute vmss from standard to managed disks</span></span>

### <a name="sql"></a><span data-ttu-id="018bf-1477">SQL</span><span class="sxs-lookup"><span data-stu-id="018bf-1477">SQL</span></span>

* <span data-ttu-id="018bf-1478">Die Parameter `--compute-model`, `--auto-pause-delay` und `--min-capacity` wurden hinzugefügt, um CRUD-Vorgänge für das neue SQL-Datenbank-Angebot zu unterstützen: Serverloses Computemodell.</span><span class="sxs-lookup"><span data-stu-id="018bf-1478">Added `--compute-model`, `--auto-pause-delay`, and `--min-capacity` parameters to support CRUD operations for new SQL Database offering: Serverless compute model.</span></span>

### <a name="storage"></a><span data-ttu-id="018bf-1479">Storage</span><span class="sxs-lookup"><span data-stu-id="018bf-1479">Storage</span></span>

* <span data-ttu-id="018bf-1480">`az storage account create/update`: Parameter „--enable-files-adds“ und Azure Active Directory-Eigenschaftenargumentgruppe hinzugefügt, um Active Directory Domain-Dienstauthentifizierung für Azure Files zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="018bf-1480">`az storage account create/update`: Added --enable-files-adds parameter and Azure Active Directory Properties Argument group to support Azure Files Active Directory Domain Service Authentication</span></span>
* <span data-ttu-id="018bf-1481">`az storage account keys list/renew` wurde erweitert, um die Auflistung oder erneute Generierung von Kerberos-Schlüsseln des Speicherkontos zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="018bf-1481">Expanded `az storage account keys list/renew` to support listing or regenerating Kerberos keys of storage account.</span></span>

## <a name="october-15-2019"></a><span data-ttu-id="018bf-1482">15. Oktober 2019</span><span class="sxs-lookup"><span data-stu-id="018bf-1482">October 15, 2019</span></span>

<span data-ttu-id="018bf-1483">Version 2.0.75</span><span class="sxs-lookup"><span data-stu-id="018bf-1483">Version 2.0.75</span></span>

### <a name="aks"></a><span data-ttu-id="018bf-1484">AKS</span><span class="sxs-lookup"><span data-stu-id="018bf-1484">AKS</span></span>

* <span data-ttu-id="018bf-1485">Standardwert `--load-balancer-sku` in `standard` geändert, sofern von der Kubernetes-Version unterstützt</span><span class="sxs-lookup"><span data-stu-id="018bf-1485">Changed `--load-balancer-sku` default value to `standard` if supported by the kubernetes version</span></span>
* <span data-ttu-id="018bf-1486">Standardwert `--vm-set-type` in `virtualmachinescalesets` geändert, sofern von der Kubernetes-Version unterstützt</span><span class="sxs-lookup"><span data-stu-id="018bf-1486">Changed `--vm-set-type` default value to `virtualmachinescalesets` if supported by the kubernetes version</span></span>

### <a name="ams"></a><span data-ttu-id="018bf-1487">AMS</span><span class="sxs-lookup"><span data-stu-id="018bf-1487">AMS</span></span>

* <span data-ttu-id="018bf-1488">[BREAKING CHANGE] Name von `job start` in `job create` geändert</span><span class="sxs-lookup"><span data-stu-id="018bf-1488">[BREAKING CHANGE] Changed the name of `job start` to `job create`</span></span>
* <span data-ttu-id="018bf-1489">[BREAKING CHANGE] Parameter `--ask` von `content-key-policy create` geändert, sodass eine hexadezimale Zeichenfolge mit 32 Zeichen anstelle von UTF8 verwendet wird</span><span class="sxs-lookup"><span data-stu-id="018bf-1489">[BREAKING CHANGE] Changed the `--ask` parameter of `content-key-policy create` to use a 32-character hex string instead of UTF8</span></span>

### <a name="appservice"></a><span data-ttu-id="018bf-1490">AppService</span><span class="sxs-lookup"><span data-stu-id="018bf-1490">AppService</span></span>

* <span data-ttu-id="018bf-1491">Befehle vom Typ `webapp config access-restriction show|set|add|remove` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1491">Added commands `webapp config access-restriction show|set|add|remove`</span></span>
* <span data-ttu-id="018bf-1492">Bessere Fehlerbehandlung zu `webapp up` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1492">Added better error handling to `webapp up`</span></span>
* <span data-ttu-id="018bf-1493">Unterstützung für SKU `Isolated` zu `appservice plan update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1493">Added support for `Isolated` SKU to `appservice plan update`</span></span>

### <a name="arm"></a><span data-ttu-id="018bf-1494">ARM</span><span class="sxs-lookup"><span data-stu-id="018bf-1494">ARM</span></span>

* <span data-ttu-id="018bf-1495">Parameter `--handle-extended-json-format` zu `deployment create` hinzugefügt, um mehrere Zeilen und Kommentare in der JSON-Vorlage zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="018bf-1495">Added `--handle-extended-json-format` parameter `deployment create` to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="018bf-1496">Compute</span><span class="sxs-lookup"><span data-stu-id="018bf-1496">Compute</span></span>

* <span data-ttu-id="018bf-1497">Parameter `--enable-agent` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1497">Added `--enable-agent` parameter to `vm create`</span></span>
* <span data-ttu-id="018bf-1498">`vm create` geändert, um bei der Verwendung von Zonen die SKU „Standard“ für die öffentliche IP-Adresse zu verwenden</span><span class="sxs-lookup"><span data-stu-id="018bf-1498">Changed `vm create` to use standard public IP SKU automatically when using zones</span></span>
* <span data-ttu-id="018bf-1499">`vm create` geändert, um automatisch einen gültigen Computernamen für eine VM zu erstellen, falls keiner angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="018bf-1499">Changed `vm create` to automatically create a valid computer name for a VM if none is provided</span></span>
* <span data-ttu-id="018bf-1500">Parameter `--computer-name-prefix` zu `vmss create` hinzugefügt, um das benutzerdefinierte Computernamenspräfix virtueller Computer in VMSS zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="018bf-1500">Added `--computer-name-prefix` parameter to `vmss create` to support custom computer name prefix of virtual machines in the VMSS</span></span>
* <span data-ttu-id="018bf-1501">Parameter `--workspace` zu `vm create` hinzugefügt, um automatisch einen Log Analytics-Arbeitsbereich zu aktivieren</span><span class="sxs-lookup"><span data-stu-id="018bf-1501">Add `--workspace` parameter to `vm create` to enable log analytics workspace automatically</span></span>
* <span data-ttu-id="018bf-1502">API-Version für Kataloge auf 2019-07-01 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="018bf-1502">Updated galleries API version to 2019-07-01</span></span>

### <a name="core"></a><span data-ttu-id="018bf-1503">Core</span><span class="sxs-lookup"><span data-stu-id="018bf-1503">Core</span></span>

* <span data-ttu-id="018bf-1504">Syntaxprüfung für Parameter `--set` im generischen Updatebefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1504">Added syntax check for `--set` parameter in generic update command</span></span>

### <a name="iot"></a><span data-ttu-id="018bf-1505">IoT</span><span class="sxs-lookup"><span data-stu-id="018bf-1505">IoT</span></span>

* <span data-ttu-id="018bf-1506">Problem behoben, bei dem für `iot hub show` der Fehler „Ressource nicht gefunden.“ zurückgegeben wurde</span><span class="sxs-lookup"><span data-stu-id="018bf-1506">Fixed an issue where `iot hub show` would incorrectly error with "resource not found"</span></span>

### <a name="monitor"></a><span data-ttu-id="018bf-1507">Überwachen</span><span class="sxs-lookup"><span data-stu-id="018bf-1507">Monitor</span></span>

* <span data-ttu-id="018bf-1508">Unterstützung für CRUD zu `monitor log-analytics workspace` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1508">Added support for CRUD to `monitor log-analytics workspace`</span></span>

### <a name="network"></a><span data-ttu-id="018bf-1509">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="018bf-1509">Network</span></span>

* <span data-ttu-id="018bf-1510">Unterstützung für mandantenübergreifende virtuelle Verbindung zu `network private-dns link vnet [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1510">Added support for cross-tenant virtual linking to `network private-dns link vnet [create|update]`</span></span>
* <span data-ttu-id="018bf-1511">[BREAKING CHANGE]`network vnet subnet list` geändert, um Parameter `--resource-group` und `--vnet-name` vorauszusetzen</span><span class="sxs-lookup"><span data-stu-id="018bf-1511">[BREAKING CHANGE] Changed `network vnet subnet list` to require `--resource-group` and `--vnet-name` parameters</span></span>

### <a name="sql"></a><span data-ttu-id="018bf-1512">SQL</span><span class="sxs-lookup"><span data-stu-id="018bf-1512">SQL</span></span>

* <span data-ttu-id="018bf-1513">Befehle zu `sql mi ad-admin` hinzugefügt, die das Festlegen eines AAD-Administrators für verwaltete Instanzen unterstützen</span><span class="sxs-lookup"><span data-stu-id="018bf-1513">Added commands to `sql mi ad-admin` that support setting an AAD administrator on managed instances</span></span>

### <a name="storage"></a><span data-ttu-id="018bf-1514">Storage</span><span class="sxs-lookup"><span data-stu-id="018bf-1514">Storage</span></span>

* <span data-ttu-id="018bf-1515">Parameter `--preserve-s2s-access-tier` zu `storage copy` hinzugefügt, um die Zugriffsebene beim Kopieren von Dienst zu Dienst beizubehalten</span><span class="sxs-lookup"><span data-stu-id="018bf-1515">Added `--preserve-s2s-access-tier` parameter `storage copy` to preserve access tier during service to service copy</span></span>
* <span data-ttu-id="018bf-1516">Parameter `--enable-large-file-share` zu `storage account [create|update]` hinzugefügt, um große Dateifreigaben für ein Speicherkonto zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="018bf-1516">Added `--enable-large-file-share` parameter to `storage account [create|update]` to support large file shares for storage account</span></span>

## <a name="september-24-2019"></a><span data-ttu-id="018bf-1517">24. September 2019</span><span class="sxs-lookup"><span data-stu-id="018bf-1517">September 24, 2019</span></span>

<span data-ttu-id="018bf-1518">Version 2.0.74</span><span class="sxs-lookup"><span data-stu-id="018bf-1518">Version 2.0.74</span></span>

### <a name="acr"></a><span data-ttu-id="018bf-1519">ACR</span><span class="sxs-lookup"><span data-stu-id="018bf-1519">ACR</span></span>

* <span data-ttu-id="018bf-1520">Erforderlicher Parameter `--type` zu `acr config retention update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1520">Added a required `--type` parameter to `acr config retention update`</span></span>
* <span data-ttu-id="018bf-1521">[BREAKING CHANGE] Umbenannter Parameter `--name -n` in `--registry -r ` für Befehlsgruppe `acr config` geändert</span><span class="sxs-lookup"><span data-stu-id="018bf-1521">[BREAKING CHANGE] Renamed parameter `--name -n` changed to `--registry -r ` for `acr config` command group</span></span>

### <a name="aks"></a><span data-ttu-id="018bf-1522">AKS</span><span class="sxs-lookup"><span data-stu-id="018bf-1522">AKS</span></span>

* <span data-ttu-id="018bf-1523">Parameter `--load-balancer-sku` zum Befehl `aks create` hinzugefügt, um die Erstellung von AKS-Clustern mit SLB zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="018bf-1523">Added `--load-balancer-sku` parameter to `aks create` command, which allows for creating AKS cluster with SLB</span></span>
* <span data-ttu-id="018bf-1524">Parameter `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` und `--load-balancer-outbound-ip-prefixes` zu den Befehlen `aks [create|update]` hinzugefügt,um die Aktualisierung des Lastenausgleichsprofils eines AKS-Clusters mit SLB zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="018bf-1524">Added `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` and `--load-balancer-outbound-ip-prefixes` parameters to `aks [create|update]` commands, which allow for updating load balancer profile of an AKS cluster with SLB</span></span>
* <span data-ttu-id="018bf-1525">Parameter `--vm-set-type` zum Befehl `aks create` hinzugefügt, um die Angabe von VM-Typen eines AKS-Clusters (vmas oder vmss) zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="018bf-1525">Added `--vm-set-type` parameter to `aks create` command, which allows to specify vm types of an AKS Cluster (vmas or vmss)</span></span>

### <a name="arm"></a><span data-ttu-id="018bf-1526">ARM</span><span class="sxs-lookup"><span data-stu-id="018bf-1526">ARM</span></span>

* <span data-ttu-id="018bf-1527">Parameter `--handle-extended-json-format` zum Befehl `group deployment create` hinzugefügt, um mehrere Zeilen und Kommentare in der JSON-Vorlage zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="018bf-1527">Added `--handle-extended-json-format` parameter to `group deployment create` command to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="018bf-1528">Compute</span><span class="sxs-lookup"><span data-stu-id="018bf-1528">Compute</span></span>

* <span data-ttu-id="018bf-1529">Parameter `--terminate-notification-time` zu den Befehlen `vmss [create|update]` hinzugefügt, um die Konfigurierbarkeit der Beendigung geplanter Ereignisse zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="018bf-1529">Added `--terminate-notification-time` parameter to `vmss [create|update]` commands to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="018bf-1530">Parameter `--enable-terminate-notification` zu den Befehlen `vmss update` hinzugefügt, um die Konfigurierbarkeit der Beendigung geplanter Ereignisse zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="018bf-1530">Added `--enable-terminate-notification` parameter to `vmss update` command to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="018bf-1531">Parameter `--priority,` `--eviction-policy,` `--max-billing` zu `[vm|vmss] create`-Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1531">Added `--priority,` `--eviction-policy,` `--max-billing` parameters to `[vm|vmss] create` commands</span></span>
* <span data-ttu-id="018bf-1532">`disk create` geändert, um die Angabe der genauen Größe des Datenträgeruploads zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="018bf-1532">Changed `disk create` to allow specifying the exact size of the disk upload</span></span>
* <span data-ttu-id="018bf-1533">Unterstützung für inkrementelle Momentaufnahmen für verwaltete Datenträger zu `snapshot create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1533">Added support for incremental snapshots for managed disks to `snapshot create`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="018bf-1534">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="018bf-1534">Cosmos DB</span></span>

* <span data-ttu-id="018bf-1535">Parameter `--type <key-type>` zum Befehl `cosmosdb keys list` hinzugefügt, um Schlüssel, schreibgeschützte Schlüssel oder Verbindungszeichenfolgen anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="018bf-1535">Added `--type <key-type>` parameter to `cosmosdb keys list` command to show key, read only keys or connection strings</span></span>
* <span data-ttu-id="018bf-1536">Befehl `cosmosdb keys regenerate` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1536">Added `cosmosdb keys regenerate` command</span></span>
* <span data-ttu-id="018bf-1537">[VERALTET] Befehle `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` und `cosmosdb list-read-only-keys` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="018bf-1537">[DEPRECATED] Deprecated `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` and `cosmosdb list-read-only-keys` commands</span></span>

### <a name="eventgrid"></a><span data-ttu-id="018bf-1538">EventGrid</span><span class="sxs-lookup"><span data-stu-id="018bf-1538">EventGrid</span></span>

* <span data-ttu-id="018bf-1539">Endpunkthilfetext korrigiert, um auf den richtigen Parameter zu verweisen</span><span class="sxs-lookup"><span data-stu-id="018bf-1539">Fixed the endpoint help text to refer to the right parameter</span></span>

### <a name="key-vault"></a><span data-ttu-id="018bf-1540">Key Vault</span><span class="sxs-lookup"><span data-stu-id="018bf-1540">Key Vault</span></span>

* <span data-ttu-id="018bf-1541">Problem behoben, aufgrund dessen die Anmeldung mit einem Mandanten (`login -t`) unter Umständen zu einem Fehler von `keyvault create` führte</span><span class="sxs-lookup"><span data-stu-id="018bf-1541">Fixed issue where logging in with a tenant (`login -t`) could cause `keyvault create` to fail</span></span>

### <a name="monitor"></a><span data-ttu-id="018bf-1542">Überwachen</span><span class="sxs-lookup"><span data-stu-id="018bf-1542">Monitor</span></span>

* <span data-ttu-id="018bf-1543">Problem behoben, aufgrund dessen das Zeichen `:` in `--condition` für `monitor metrics alert create` nicht zulässig war</span><span class="sxs-lookup"><span data-stu-id="018bf-1543">Fixed issue where `:` character was not allowed in `--condition` argument to `monitor metrics alert create`</span></span>

### <a name="policy"></a><span data-ttu-id="018bf-1544">Richtlinie</span><span class="sxs-lookup"><span data-stu-id="018bf-1544">Policy</span></span>

* <span data-ttu-id="018bf-1545">Unterstützung für Policy-API-Version 2019-06-01 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1545">Added support for Policy API version 2019-06-01</span></span>
* <span data-ttu-id="018bf-1546">Parameter `--enforcement-mode` zum Befehl `policy assignment create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1546">Added `--enforcement-mode` parameter to `policy assignment create` command</span></span>

### <a name="storage"></a><span data-ttu-id="018bf-1547">Storage</span><span class="sxs-lookup"><span data-stu-id="018bf-1547">Storage</span></span>

* <span data-ttu-id="018bf-1548">Parameter `--blob-type` zum Befehl `az storage copy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1548">Added `--blob-type` parameter to `az storage copy` command</span></span>

## <a name="september-10-2019"></a><span data-ttu-id="018bf-1549">10. September 2019</span><span class="sxs-lookup"><span data-stu-id="018bf-1549">September 10, 2019</span></span>

### <a name="acr"></a><span data-ttu-id="018bf-1550">ACR</span><span class="sxs-lookup"><span data-stu-id="018bf-1550">ACR</span></span>

* <span data-ttu-id="018bf-1551">Befehlsgruppe `acr config retention` zum Konfigurieren der Aufbewahrungsrichtlinie hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1551">Added command group `acr config retention` to configure retention policy</span></span>

### <a name="aks"></a><span data-ttu-id="018bf-1552">AKS</span><span class="sxs-lookup"><span data-stu-id="018bf-1552">AKS</span></span>

* <span data-ttu-id="018bf-1553">Unterstützung für die ACR-Integration mit den folgenden Befehlen hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="018bf-1553">Added support for ACR integration with the following commands:</span></span>
  * <span data-ttu-id="018bf-1554">Parameter `--attach-acr` zu `aks [create|update]` hinzugefügt, um einen ACR an einen AKS-Cluster anzufügen</span><span class="sxs-lookup"><span data-stu-id="018bf-1554">Added `--attach-acr` parameter to `aks [create|update]` to attach an ACR to an AKS cluster</span></span>
  * <span data-ttu-id="018bf-1555">Parameter `--detach-acr` zu `aks update` hinzugefügt, um den ACR von einem AKS-Cluster zu trennen</span><span class="sxs-lookup"><span data-stu-id="018bf-1555">Added `--detach-acr` parameter to `aks update` to detach the ACR from an AKS cluster</span></span>

### <a name="arm"></a><span data-ttu-id="018bf-1556">ARM</span><span class="sxs-lookup"><span data-stu-id="018bf-1556">ARM</span></span>

* <span data-ttu-id="018bf-1557">Zur Verwendung der API-Version 2019-05-10 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="018bf-1557">Updated to use API version 2019-05-10</span></span>

### <a name="batch"></a><span data-ttu-id="018bf-1558">Batch</span><span class="sxs-lookup"><span data-stu-id="018bf-1558">Batch</span></span>

* <span data-ttu-id="018bf-1559">Neue JSON-Konfigurationseinstellungen für `batch pool create` zu `--json-file` hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="018bf-1559">Added new JSON configuration settings to `--json-file` for `batch pool create`:</span></span>
  * <span data-ttu-id="018bf-1560">`MountConfigurations` für Dateisystemeinbindungen hinzugefügt (Details siehe https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body )</span><span class="sxs-lookup"><span data-stu-id="018bf-1560">Added `MountConfigurations` for file system mounts (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
  * <span data-ttu-id="018bf-1561">Optionale Eigenschaft `publicIPs` in `NetworkConfiguration` für öffentliche IP-Adressen für Pools hinzugefügt (Details siehe https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body )</span><span class="sxs-lookup"><span data-stu-id="018bf-1561">Added optional property `publicIPs` on `NetworkConfiguration` for public IPs on pools (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
* <span data-ttu-id="018bf-1562">Unterstützung für Kataloge mit freigegebenen Images zu `--image` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1562">Added support for shared image galleries to `--image`</span></span>
* <span data-ttu-id="018bf-1563">[BREAKING CHANGE] Standardwert von `--start-task-wait-for-success` für `batch pool create` in `true` geändert</span><span class="sxs-lookup"><span data-stu-id="018bf-1563">[BREAKING CHANGE] Changed default value of `--start-task-wait-for-success` on `batch pool create` to be `true`</span></span>
* <span data-ttu-id="018bf-1564">[BREAKING CHANGE] Standardwert von `Scope` für `AutoUserSpecification` geändert, damit immer „Pool“ verwendet wird (vormals `Task` für Windows-Knoten bzw. `Pool` für Linux-Knoten)</span><span class="sxs-lookup"><span data-stu-id="018bf-1564">[BREAKING CHANGE] Changed default value for `Scope` on `AutoUserSpecification` to always be Pool (was `Task` on Windows nodes, `Pool` on Linux nodes)</span></span>
  * <span data-ttu-id="018bf-1565">Dieses Argument kann nur über eine JSON-Konfiguration mit `--json-file` festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="018bf-1565">This argument can only be set from a JSON configuration with `--json-file`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="018bf-1566">HDInsight</span><span class="sxs-lookup"><span data-stu-id="018bf-1566">HDInsight</span></span>

* <span data-ttu-id="018bf-1567">Allgemein verfügbares Release</span><span class="sxs-lookup"><span data-stu-id="018bf-1567">GA release</span></span>
* <span data-ttu-id="018bf-1568">[BREAKING CHANGE] Parameter `--workernode-count/-c` von `az hdinsight resize` in erforderlich geändert</span><span class="sxs-lookup"><span data-stu-id="018bf-1568">[BREAKING CHANGE] Changed parameter `--workernode-count/-c` of `az hdinsight resize` to be required.</span></span>

### <a name="key-vault"></a><span data-ttu-id="018bf-1569">Key Vault</span><span class="sxs-lookup"><span data-stu-id="018bf-1569">Key Vault</span></span>

* <span data-ttu-id="018bf-1570">Problem behoben, aufgrund dessen Subnetze nicht aus Netzwerkregeln gelöscht werden konnten</span><span class="sxs-lookup"><span data-stu-id="018bf-1570">Fixed issue where subnets couldn't be deleted from network rules</span></span>
* <span data-ttu-id="018bf-1571">Problem behoben, aufgrund dessen doppelte Subnetze und IP-Adressen zu Netzwerkregeln hinzugefügt werden konnten</span><span class="sxs-lookup"><span data-stu-id="018bf-1571">Fixed issue where duplicated subnets and IP addresses could be added to network rules</span></span>

### <a name="network"></a><span data-ttu-id="018bf-1572">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="018bf-1572">Network</span></span>

* <span data-ttu-id="018bf-1573">Parameter `--interval` zu `network watcher flow-log` hinzugefügt, um den Wert für das Intervall der Datenverkehrsanalyse festzulegen</span><span class="sxs-lookup"><span data-stu-id="018bf-1573">Added `--interval` parameter to `network watcher flow-log` to set traffic analysis interval value</span></span>
* <span data-ttu-id="018bf-1574">`network application-gateway identity` zum Verwalten der Gatewayidentität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1574">Added `network application-gateway identity` to manage gateway identity</span></span>
* <span data-ttu-id="018bf-1575">Unterstützung zum Festlegen der Key Vault-ID zu `network application-gateway ssl-cert` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1575">Added support for setting Key Vault ID to `network application-gateway ssl-cert`</span></span>
* <span data-ttu-id="018bf-1576">`network express-route peering peer-connection [show|list]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1576">Added `network express-route peering peer-connection [show|list]`</span></span>

### <a name="policy"></a><span data-ttu-id="018bf-1577">Richtlinie</span><span class="sxs-lookup"><span data-stu-id="018bf-1577">Policy</span></span>

* <span data-ttu-id="018bf-1578">Zur Verwendung der API-Version 2019-01-01 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="018bf-1578">Updated to use API version 2019-01-01</span></span>

## <a name="august-27-2019"></a><span data-ttu-id="018bf-1579">27. August 2019</span><span class="sxs-lookup"><span data-stu-id="018bf-1579">August 27, 2019</span></span>

<span data-ttu-id="018bf-1580">Version 2.0.72</span><span class="sxs-lookup"><span data-stu-id="018bf-1580">Version 2.0.72</span></span>

### <a name="acr"></a><span data-ttu-id="018bf-1581">ACR</span><span class="sxs-lookup"><span data-stu-id="018bf-1581">ACR</span></span>

* <span data-ttu-id="018bf-1582">[BREAKING CHANGE] Unterstützung für SKU `classic` entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-1582">[BREAKING CHANGE] Removed support for the `classic` SKU</span></span>

### <a name="api-management"></a><span data-ttu-id="018bf-1583">API Management</span><span class="sxs-lookup"><span data-stu-id="018bf-1583">API Management</span></span>

* <span data-ttu-id="018bf-1584">[VORSCHAU] Befehlsgruppe `apim` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1584">[PREVIEW] Added `apim` command group</span></span>

### <a name="appservice"></a><span data-ttu-id="018bf-1585">AppService</span><span class="sxs-lookup"><span data-stu-id="018bf-1585">AppService</span></span>

* <span data-ttu-id="018bf-1586">Problem mit dem Befehl `webapp webjob continuous start` bei Angabe eines Slots behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-1586">Fixed issue with `webapp webjob continuous start` command when specifying a slot</span></span>
* <span data-ttu-id="018bf-1587">`webapp up` geändert, um den Ordner `env` zu erkennen und aus der für die Bereitstellung verwendeten Datei zu entfernen</span><span class="sxs-lookup"><span data-stu-id="018bf-1587">Changed `webapp up` to detect `env` folder and remove it from the file used for deployment</span></span>

### <a name="keyvault"></a><span data-ttu-id="018bf-1588">KeyVault</span><span class="sxs-lookup"><span data-stu-id="018bf-1588">Keyvault</span></span>

* <span data-ttu-id="018bf-1589">Fehler in `keyvault secret set` behoben, aufgrund dessen das Argument `--expires` ignoriert wurde</span><span class="sxs-lookup"><span data-stu-id="018bf-1589">Fixed a bug in `keyvault secret set` that igored the `--expires` argument</span></span>

### <a name="network"></a><span data-ttu-id="018bf-1590">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="018bf-1590">Network</span></span>

* <span data-ttu-id="018bf-1591">Unterstützung für IPv6-Adressen zu Argumenten vom Typ `--private-ip-address-version` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1591">Added support for IPv6 addresses to `--private-ip-address-version` arguments</span></span>
* <span data-ttu-id="018bf-1592">Neue Befehle vom Typ `network private-endpoint [create|update|list-types]` für die Verwaltung privater Endpunkte hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1592">Added new commands `network private-endpoint [create|update|list-types]` for private endpoint management</span></span>
* <span data-ttu-id="018bf-1593">Befehlsgruppe `network private-link-service` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1593">Added command group `network private-link-service`</span></span>
* <span data-ttu-id="018bf-1594">Argumente `--private-endpoint-network-policies` und `--private-link-service-network-policies` zu `network vnet subnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1594">Added `--private-endpoint-network-policies` and `--private-link-service-network-policies` arguments to `network vnet subnet update`</span></span>

### <a name="rbac"></a><span data-ttu-id="018bf-1595">RBAC</span><span class="sxs-lookup"><span data-stu-id="018bf-1595">RBAC</span></span>

* <span data-ttu-id="018bf-1596">Problem mit `ad app update --homepage` behoben, aufgrund dessen die Startseite nicht aktualisiert wurde</span><span class="sxs-lookup"><span data-stu-id="018bf-1596">Fixed issue with `ad app update --homepage` where homepage would not be updated</span></span>

### <a name="servicefabric"></a><span data-ttu-id="018bf-1597">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="018bf-1597">ServiceFabric</span></span>

* <span data-ttu-id="018bf-1598">Unterstützung für Key Vault-Namen mit Groß- und Kleinschreibung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1598">Added support for mixed-case Key Vault names</span></span>
* <span data-ttu-id="018bf-1599">Problem bei der Verwendung von Zertifikaten in Key Vault behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-1599">Fixed issue when using certificates in Key Vault</span></span>
* <span data-ttu-id="018bf-1600">Problem bei der Verwendung von PFX-Zertifikatdateien behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-1600">Fixed issue with using PFX certificate files</span></span>
* <span data-ttu-id="018bf-1601">Problem mit `sf cluster certificate add` behoben, wenn keine Key Vault-Ressourcengruppe angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="018bf-1601">Fixed issue with `sf cluster certificate add` when Key Vault resource group wasn't specified</span></span>
* <span data-ttu-id="018bf-1602">Problem behoben, aufgrund dessen `sf cluster set` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="018bf-1602">Fixed issue with `sf cluster set` not working</span></span>

### <a name="signalr"></a><span data-ttu-id="018bf-1603">SignalR</span><span class="sxs-lookup"><span data-stu-id="018bf-1603">SignalR</span></span>

* <span data-ttu-id="018bf-1604">Neue Befehle hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="018bf-1604">Added new commands:</span></span>
  * <span data-ttu-id="018bf-1605">`signalr cors`: Verwalten von CORS für SignalR</span><span class="sxs-lookup"><span data-stu-id="018bf-1605">`signalr cors`: Manage SignalR CORS</span></span>
  * <span data-ttu-id="018bf-1606">`signalr restart`: Starten eines SignalR-Diensts</span><span class="sxs-lookup"><span data-stu-id="018bf-1606">`signalr restart`: Restart a SignalR service</span></span>
  * <span data-ttu-id="018bf-1607">`signalr update`: Aktualisieren eines SignalR-Diensts</span><span class="sxs-lookup"><span data-stu-id="018bf-1607">`signalr update`: Update a SignalR service</span></span>
* <span data-ttu-id="018bf-1608">Argument `--service-mode` zu `signalr create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1608">Added `--service-mode` argument to `signalr create`</span></span>

### <a name="storage"></a><span data-ttu-id="018bf-1609">Storage</span><span class="sxs-lookup"><span data-stu-id="018bf-1609">Storage</span></span>

* <span data-ttu-id="018bf-1610">Befehl `storage account revoke-delegation-keys` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1610">Added `storage account revoke-delegation-keys` command</span></span>

## <a name="august-13-2019"></a><span data-ttu-id="018bf-1611">13. August 2019</span><span class="sxs-lookup"><span data-stu-id="018bf-1611">August 13, 2019</span></span>

<span data-ttu-id="018bf-1612">Version 2.0.71</span><span class="sxs-lookup"><span data-stu-id="018bf-1612">Version 2.0.71</span></span>

### <a name="appservice"></a><span data-ttu-id="018bf-1613">AppService</span><span class="sxs-lookup"><span data-stu-id="018bf-1613">AppService</span></span>

* <span data-ttu-id="018bf-1614">Problem behoben, aufgrund dessen bei Befehlen vom Typ `webapp webjob continuous` für Slots Fehler auftraten</span><span class="sxs-lookup"><span data-stu-id="018bf-1614">Fixed issue where `webapp webjob continuous` commands were failing for slots</span></span>

### <a name="botservice"></a><span data-ttu-id="018bf-1615">BotService</span><span class="sxs-lookup"><span data-stu-id="018bf-1615">BotService</span></span>

* <span data-ttu-id="018bf-1616">[BREAKING CHANGE] Unterstützung für die Erstellung von Bots der Version 3 entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-1616">[BREAKING CHANGE] Removed support for creating v3 SDK bots</span></span>

### <a name="cognitiveservices"></a><span data-ttu-id="018bf-1617">CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="018bf-1617">CognitiveServices</span></span>

* <span data-ttu-id="018bf-1618">Befehle vom Typ `cognitiveservices account network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1618">Added `cognitiveservices account network-rule` commands</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="018bf-1619">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="018bf-1619">Cosmos DB</span></span>

* <span data-ttu-id="018bf-1620">Beim Aktualisieren mehrerer Schreibstandorte wurde eine Warnung entfernt.</span><span class="sxs-lookup"><span data-stu-id="018bf-1620">Removed warning when updating multiple write locations</span></span>
* <span data-ttu-id="018bf-1621">CRUD-Befehle für CosmosDB SQL-, MongoDB-, Cassandra-, Gremlin- und Tabellenressourcen sowie den Ressourcendurchsatz hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1621">Added CRUD commands for CosmosDB SQL, MongoDB, Cassandra, Gremlin and Table resources and resource's throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="018bf-1622">HDInsight</span><span class="sxs-lookup"><span data-stu-id="018bf-1622">HDInsight</span></span>

<span data-ttu-id="018bf-1623">Dieses Release enthält zahlreiche wichtige Änderungen.</span><span class="sxs-lookup"><span data-stu-id="018bf-1623">This release contains a large number of breaking changes.</span></span>

* <span data-ttu-id="018bf-1624">[BREAKING CHANGE] Parameter für `hdinsight create` umbenannt:</span><span class="sxs-lookup"><span data-stu-id="018bf-1624">[BREAKING CHANGE] Renamed parameters for `hdinsight create`:</span></span>
  * <span data-ttu-id="018bf-1625">`--storage-default-container` in `--storage-container` umbenannt</span><span class="sxs-lookup"><span data-stu-id="018bf-1625">Renamed `--storage-default-container` to `--storage-container`</span></span>
  * <span data-ttu-id="018bf-1626">`--storage-default-filesystem` in `--storage-filesystem` umbenannt</span><span class="sxs-lookup"><span data-stu-id="018bf-1626">Renamed `--storage-default-filesystem` to `--storage-filesystem`</span></span>
* <span data-ttu-id="018bf-1627">[BREAKING CHANGE] Das Argument `--name` von `application create` wurde so geändert, dass es den Anwendungsnamen anstelle des Clusternamens darstellt.</span><span class="sxs-lookup"><span data-stu-id="018bf-1627">[BREAKING CHANGE] Changed the `--name` argument of `application create` to represent the application name instead of the cluster name</span></span>
* <span data-ttu-id="018bf-1628">Argument `--cluster-name` zu `application create` hinzugefügt, um die alte Funktion `--name` zu ersetzen</span><span class="sxs-lookup"><span data-stu-id="018bf-1628">Added `--cluster-name` argument to `application create` to replace old `--name` functionality</span></span>
* <span data-ttu-id="018bf-1629">[BREAKING CHANGE] Parameter für `application create` umbenannt:</span><span class="sxs-lookup"><span data-stu-id="018bf-1629">[BREAKING CHANGE] Renamed parameters for `application create`:</span></span>
  * <span data-ttu-id="018bf-1630">`--application-type` in `--type` umbenannt</span><span class="sxs-lookup"><span data-stu-id="018bf-1630">Renamed `--application-type` to `--type`</span></span>
  * <span data-ttu-id="018bf-1631">`--marketplace-identifier` in `--marketplace-id` umbenannt</span><span class="sxs-lookup"><span data-stu-id="018bf-1631">Renamed `--marketplace-identifier` to `--marketplace-id`</span></span>
  * <span data-ttu-id="018bf-1632">`--https-endpoint-access-mode` in `--access-mode` umbenannt</span><span class="sxs-lookup"><span data-stu-id="018bf-1632">Renamed `--https-endpoint-access-mode` to `--access-mode`</span></span>
  * <span data-ttu-id="018bf-1633">`--https-endpoint-destination-port` in `--destination-port` umbenannt</span><span class="sxs-lookup"><span data-stu-id="018bf-1633">Renamed  `--https-endpoint-destination-port` to `--destination-port`</span></span>
* <span data-ttu-id="018bf-1634">[BREAKING CHANGE] Parameter für `application create` entfernt:</span><span class="sxs-lookup"><span data-stu-id="018bf-1634">[BREAKING CHANGE] Removed parameters for `application create`:</span></span>
  * `--https-endpoint-location`
  * `--https-endpoint-public-port`
  * `--ssh-endpoint-destination-port`
  * `--ssh-endpoint-location`
  * `--ssh-endpoint-public-port`
* <span data-ttu-id="018bf-1635">[WICHTIGE ÄNDERUNG] `--target-instance-count` für `hdinsight resize` in `--workernode-count` umbenannt</span><span class="sxs-lookup"><span data-stu-id="018bf-1635">[BREAKING CHNAGE] Renamed `--target-instance-count` to `--workernode-count` for `hdinsight resize`</span></span>
* <span data-ttu-id="018bf-1636">[BREAKING CHANGE] Alle Befehle in der Gruppe `hdinsight script-action` wurden so geändert, dass sie den Parameter `--name` als Namen der Skriptaktion verwenden.</span><span class="sxs-lookup"><span data-stu-id="018bf-1636">[BREAKING CHANGE] Changed all commands in the `hdinsight script-action` group to use the `--name` parameter as the name of the script action.</span></span>
* <span data-ttu-id="018bf-1637">Argument `--cluster-name` zu allen Befehlen vom Typ `hdinsight script-action` hinzugefügt, um die alte Funktion `--name` zu ersetzen</span><span class="sxs-lookup"><span data-stu-id="018bf-1637">Added `--cluster-name` argument to all `hdinsight script-action` commands to replace old `--name` functionality</span></span>
* <span data-ttu-id="018bf-1638">[BREAKING CHANGE]`--script-execution-id` für alle Befehle vom Typ `hdinsight script-action` in `--execution-id` umbenannt</span><span class="sxs-lookup"><span data-stu-id="018bf-1638">[BREAKING CHANGE] Renamed `--script-execution-id` to `--execution-id` for all `hdinsight script-action` commands</span></span>
* <span data-ttu-id="018bf-1639">[BREAKING CHANGE]`hdinsight script-action show` in `hdinsight script-action show-execution-details` umbenannt</span><span class="sxs-lookup"><span data-stu-id="018bf-1639">[BREAKING CHANGE] Renamed `hdinsight script-action show` to `hdinsight script-action show-execution-details`</span></span>
* <span data-ttu-id="018bf-1640">[WICHTIGE ÄNDERUNG] Parameter in `hdinsight script-action execute --roles` geändert, sodass sie durch Leerzeichen anstelle von Kommas getrennt sind</span><span class="sxs-lookup"><span data-stu-id="018bf-1640">[BREAKING CHNAGE] Changed parameters to `hdinsight script-action execute --roles` to be space-separated instead of comma-separated</span></span>
* <span data-ttu-id="018bf-1641">[BREAKING CHANGE] Parameter `--persisted` für `hdinsight script-action list` entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-1641">[BREAKING CHANGE] Removed the `--persisted` parameter of `hdinsight script-action list`</span></span>
* <span data-ttu-id="018bf-1642">Der Parameter `hdinsight create --cluster-configurations` wurde so geändert, dass er einen Pfad zu einer lokalen JSON-Datei oder JSON-Zeichenfolge akzeptiert.</span><span class="sxs-lookup"><span data-stu-id="018bf-1642">Changed the `hdinsight create --cluster-configurations` parameter to accept a path to a local JSON file or a JSON string</span></span>
* <span data-ttu-id="018bf-1643">Befehl `hdinsight script-action list-execution-history` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1643">Added command `hdinsight script-action list-execution-history`</span></span>
* <span data-ttu-id="018bf-1644">`hdinsight monitor enable --workspace` geändert, um die ID oder den Namen eines Log Analytics-Arbeitsbereichs zu akzeptieren</span><span class="sxs-lookup"><span data-stu-id="018bf-1644">Changed `hdinsight monitor enable --workspace` to accept a Log Analytics workspace ID or workspace name</span></span>
* <span data-ttu-id="018bf-1645">Argument `hdinsight monitor enable --primary-key` hinzugefügt. Dieses Argument wird benötigt, wenn eine Arbeitsbereichs-ID als Parameter angegeben wird.</span><span class="sxs-lookup"><span data-stu-id="018bf-1645">Added the `hdinsight monitor enable --primary-key` argument, which is needed if a workspace ID is provided as the parameter</span></span>
* <span data-ttu-id="018bf-1646">Weitere Beispiele und aktualisierte Beschreibungen für Hilfemeldungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1646">Added more examples and updated descriptions for help messages</span></span>

### <a name="interactive"></a><span data-ttu-id="018bf-1647">Interactive</span><span class="sxs-lookup"><span data-stu-id="018bf-1647">Interactive</span></span>

* <span data-ttu-id="018bf-1648">Ladefehler behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-1648">Fixed a loading error</span></span>

### <a name="kubernetes"></a><span data-ttu-id="018bf-1649">Kubernetes</span><span class="sxs-lookup"><span data-stu-id="018bf-1649">Kubernetes</span></span>

* <span data-ttu-id="018bf-1650">Änderung, um `https` zu verwenden, wenn der Dashboardcontainerport `https` verwendet</span><span class="sxs-lookup"><span data-stu-id="018bf-1650">Changed to use `https` if dashboard container port is using `https`</span></span>

### <a name="network"></a><span data-ttu-id="018bf-1651">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="018bf-1651">Network</span></span>

* <span data-ttu-id="018bf-1652">Argument `--yes` hinzugefügt zu `network dns record-set cname delete`</span><span class="sxs-lookup"><span data-stu-id="018bf-1652">Added `--yes` argument `network dns record-set cname delete`</span></span>

### <a name="profile"></a><span data-ttu-id="018bf-1653">Profil</span><span class="sxs-lookup"><span data-stu-id="018bf-1653">Profile</span></span>

* <span data-ttu-id="018bf-1654">Argument `--resource-type` zu `account get-access-token` zum Abrufen von Ressourcenzugriffstoken hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1654">Added `--resource-type` argument to `account get-access-token` to get resource access tokens</span></span>

### <a name="servicefabric"></a><span data-ttu-id="018bf-1655">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="018bf-1655">ServiceFabric</span></span>

* <span data-ttu-id="018bf-1656">Alle unterstützten Betriebssystemversionen für „sf cluster create“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1656">Added all supported os version for sf cluster create</span></span>
* <span data-ttu-id="018bf-1657">Fehler beim Überprüfen des primären Zertifikats behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-1657">Fixed primary certificate validation bug</span></span>

### <a name="storage"></a><span data-ttu-id="018bf-1658">Storage</span><span class="sxs-lookup"><span data-stu-id="018bf-1658">Storage</span></span>

* <span data-ttu-id="018bf-1659">Befehl `storage copy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1659">Added command `storage copy`</span></span>

## <a name="july-30-2019"></a><span data-ttu-id="018bf-1660">30. Juli 2019</span><span class="sxs-lookup"><span data-stu-id="018bf-1660">July 30, 2019</span></span>

<span data-ttu-id="018bf-1661">Version 2.0.70</span><span class="sxs-lookup"><span data-stu-id="018bf-1661">Version 2.0.70</span></span>

### <a name="acr"></a><span data-ttu-id="018bf-1662">ACR</span><span class="sxs-lookup"><span data-stu-id="018bf-1662">ACR</span></span>

* <span data-ttu-id="018bf-1663">Problem #9952 behoben (Regression im Befehl `acr pack build`)</span><span class="sxs-lookup"><span data-stu-id="018bf-1663">Fixed issue #9952 (a regression in the `acr pack build` command)</span></span>
* <span data-ttu-id="018bf-1664">Standardname des Generatorimages in `acr pack build` entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-1664">Removed the default builder image name in `acr pack build`</span></span>

### <a name="appservice"></a><span data-ttu-id="018bf-1665">AppService</span><span class="sxs-lookup"><span data-stu-id="018bf-1665">Appservice</span></span>

* <span data-ttu-id="018bf-1666">`webapp config ssl` geändert, um eine Meldung anzuzeigen, wenn eine Ressource nicht gefunden wurde</span><span class="sxs-lookup"><span data-stu-id="018bf-1666">Changed `webapp config ssl` to show a message if a resource is not found</span></span>
* <span data-ttu-id="018bf-1667">Problem behoben, aufgrund dessen `functionapp create` den Speicherkontotypen `Standard_RAGRS` nicht akzeptiert hat</span><span class="sxs-lookup"><span data-stu-id="018bf-1667">Fixed issue where `functionapp create` does not accept `Standard_RAGRS` storage account type</span></span>
* <span data-ttu-id="018bf-1668">Problem behoben, aufgrund dessen für `webapp up` ein Fehler auftrat, wenn für die Ausführung ältere Python-Versionen verwendet wurden</span><span class="sxs-lookup"><span data-stu-id="018bf-1668">Fixed an issue where `webapp up` would fail if run using older versions of python</span></span>

### <a name="network"></a><span data-ttu-id="018bf-1669">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="018bf-1669">Network</span></span>

* <span data-ttu-id="018bf-1670">Ungültiger Parameter `--ids` aus `network nic ip-config add` entfernt (Fehlerbehebungen #9861)</span><span class="sxs-lookup"><span data-stu-id="018bf-1670">Removed invalid parameter `--ids` from `network nic ip-config add` (fixes #9861)</span></span>
* <span data-ttu-id="018bf-1671">Fehlerbehebungen #9604.</span><span class="sxs-lookup"><span data-stu-id="018bf-1671">Fixes #9604.</span></span> <span data-ttu-id="018bf-1672">Parameter `--root-certs` zu `network application-gateway http-settings [create|update]` hinzugefügt, um vom Benutzer zugewiesene vertrauenswürdige Stammzertifikate zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="018bf-1672">Added `--root-certs` parameter to `network application-gateway http-settings [create|update]` to support user associate trusted root certificates.</span></span>
* <span data-ttu-id="018bf-1673">Argument `--subscription` für `network dns record-set ns create` korrigiert (#9965)</span><span class="sxs-lookup"><span data-stu-id="018bf-1673">Fixed arguent `--subscription` for `network dns record-set ns create` (#9965)</span></span>

### <a name="rbac"></a><span data-ttu-id="018bf-1674">RBAC</span><span class="sxs-lookup"><span data-stu-id="018bf-1674">RBAC</span></span>

* <span data-ttu-id="018bf-1675">Befehl `user update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1675">Added `user update` command</span></span>
* <span data-ttu-id="018bf-1676">[VERALTET]`--upn-or-object-id` in benutzerbezogenen Befehlen als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="018bf-1676">[DEPRECATED] Deprecated `--upn-or-object-id` from user-related commands</span></span>
    * <span data-ttu-id="018bf-1677">Verwenden Sie das Ersatzargument `--id`.</span><span class="sxs-lookup"><span data-stu-id="018bf-1677">Use replacement argument `--id`</span></span>
* <span data-ttu-id="018bf-1678">Argument `--id` zu benutzerbezogenen Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1678">Added `--id` argument to user-related commands</span></span>

### <a name="sql"></a><span data-ttu-id="018bf-1679">SQL</span><span class="sxs-lookup"><span data-stu-id="018bf-1679">SQL</span></span>

* <span data-ttu-id="018bf-1680">Verwaltungsbefehle für Schlüssel verwalteter Instanzen und TDE-Schutzvorrichtung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1680">Added management commands for managed instance keys and TDE protector</span></span>

### <a name="storage"></a><span data-ttu-id="018bf-1681">Storage</span><span class="sxs-lookup"><span data-stu-id="018bf-1681">Storage</span></span>

* <span data-ttu-id="018bf-1682">Befehl `storage remove` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1682">Added `storage remove` command</span></span>
* <span data-ttu-id="018bf-1683">Problem mit `storage blob update` behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-1683">Fixed an issue with `storage blob update`</span></span>

### <a name="vm"></a><span data-ttu-id="018bf-1684">VM</span><span class="sxs-lookup"><span data-stu-id="018bf-1684">VM</span></span>

* <span data-ttu-id="018bf-1685">`list-skus` wurde geändert, um eine neuere API-Version für die Ausgabe von Zonendetails zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="018bf-1685">Changed `list-skus` to use newer api-version to output zone details</span></span>
* <span data-ttu-id="018bf-1686">Standardwert `--single-placement-group` für `vmss create` in `false` geändert</span><span class="sxs-lookup"><span data-stu-id="018bf-1686">Changed default of `--single-placement-group` to `false` for `vmss create`</span></span>
* <span data-ttu-id="018bf-1687">Möglichkeit zum Auswählen von ZRS-Speicher-SKUs für `[snapshot|disk] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1687">Added ability to select ZRS storage SKUs for `[snapshot|disk] create`</span></span>
* <span data-ttu-id="018bf-1688">Neue Befehlsgruppe `vm host` zur Unterstützung dedizierter Hosts hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1688">Added new command group `vm host` to support dedicated hosts</span></span>
* <span data-ttu-id="018bf-1689">Parameter `--host` und `--host-group` für `vm create` hinzugefügt, um den dedizierten VM-Host festzulegen</span><span class="sxs-lookup"><span data-stu-id="018bf-1689">Added parameters `--host` and `--host-group` on `vm create` to set VM dedicated host</span></span>

## <a name="july-16-2019"></a><span data-ttu-id="018bf-1690">16. Juli 2019</span><span class="sxs-lookup"><span data-stu-id="018bf-1690">July 16, 2019</span></span>

<span data-ttu-id="018bf-1691">Version 2.0.69</span><span class="sxs-lookup"><span data-stu-id="018bf-1691">Version 2.0.69</span></span>

### <a name="appservice"></a><span data-ttu-id="018bf-1692">AppService</span><span class="sxs-lookup"><span data-stu-id="018bf-1692">Appservice</span></span>

* <span data-ttu-id="018bf-1693">`webapp identity`-Befehle geändert, um eine korrekte Fehlermeldung zurückzugeben, wenn „ResourceGroupName“ oder der App-Name ungültig sind</span><span class="sxs-lookup"><span data-stu-id="018bf-1693">Changed `webapp identity` commands to return a proper error message if ResourceGroupName or App name are invalid</span></span>
* <span data-ttu-id="018bf-1694">`webapp list` korrigiert, sodass der korrekte Wert für „numberOfSites“ zurückgegeben wird, wenn „ResourceGroup“ nicht angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="018bf-1694">Fixed `webapp list` to return the correct value for numberOfSites if no ResourceGroup was provided</span></span>
* <span data-ttu-id="018bf-1695">Nebeneffekte von `appservice plan create` und `webapp create` behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-1695">Fixed side-effects of `appservice plan create` and `webapp create`</span></span>

### <a name="core"></a><span data-ttu-id="018bf-1696">Core</span><span class="sxs-lookup"><span data-stu-id="018bf-1696">Core</span></span>

* <span data-ttu-id="018bf-1697">Problem behoben, aufgrund dessen `--subscription` angezeigt wurde, obwohl nicht anwendbar</span><span class="sxs-lookup"><span data-stu-id="018bf-1697">Fixed issue where `--subscription` would appear despite being not applicable</span></span>

### <a name="batch"></a><span data-ttu-id="018bf-1698">Batch</span><span class="sxs-lookup"><span data-stu-id="018bf-1698">Batch</span></span>

* <span data-ttu-id="018bf-1699">[BREAKING CHANGE]`batch pool node-agent-skus list` durch `batch pool supported-images list` ersetzt</span><span class="sxs-lookup"><span data-stu-id="018bf-1699">[BREAKING CHANGE] Replaced `batch pool node-agent-skus list` with `batch pool supported-images list`</span></span>
* <span data-ttu-id="018bf-1700">Unterstützung für Sicherheitsregeln hinzugefügt, die den Netzwerkzugriff auf einen Pool basierend auf dem Quellport des Datenverkehrs blockieren, wenn die Option `--json-file` von `batch pool create network` verwendet wird</span><span class="sxs-lookup"><span data-stu-id="018bf-1700">Added support for security rules blocking network access to a pool based on the source port of the traffic when using the `--json-file` option of `batch pool create network`</span></span>
* <span data-ttu-id="018bf-1701">Unterstützung für die Ausführung der Aufgabe im Arbeitsverzeichnis des Containers oder der Batch-Aufgabe hinzugefügt, wenn die Option `--json-file` von `batch task create` verwendet wird</span><span class="sxs-lookup"><span data-stu-id="018bf-1701">Added support for executing the task in the container working directory or in the Batch task working directory when using the `--json-file` option of `batch task create`</span></span>
* <span data-ttu-id="018bf-1702">Fehler in Option `--application-package-references` von `batch pool create` behoben, aufgrund dessen nur Standardeinstellungen möglich waren</span><span class="sxs-lookup"><span data-stu-id="018bf-1702">Fixed error in `--application-package-references` option of `batch pool create` where it would only work with defaults</span></span>

### <a name="eventhubs"></a><span data-ttu-id="018bf-1703">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="018bf-1703">Eventhubs</span></span>

* <span data-ttu-id="018bf-1704">Validierung für Parameter `--rights` von `authorizationrule`-Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1704">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="rdbms"></a><span data-ttu-id="018bf-1705">RDBMS</span><span class="sxs-lookup"><span data-stu-id="018bf-1705">RDBMS</span></span>

* <span data-ttu-id="018bf-1706">Optionaler Parameter zum Angeben der Replikat-SKU für den Befehl zum Erstellen von Replikaten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1706">Added optional parameter to specify replica SKU for create replica command</span></span>
* <span data-ttu-id="018bf-1707">Problem mit CI-Testfehler bei der Erstellung von MySQL-Replikaten behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-1707">Fixed the issue with CI test failure with creating MySQL replica</span></span>

### <a name="relay"></a><span data-ttu-id="018bf-1708">Relay</span><span class="sxs-lookup"><span data-stu-id="018bf-1708">Relay</span></span>

* <span data-ttu-id="018bf-1709">Problem mit Hybridverbindung behoben, wenn die Client-Autorisierung deaktiviert ist [#8775](https://github.com/azure/azure-cli/issues/8775)</span><span class="sxs-lookup"><span data-stu-id="018bf-1709">Fixed issue with hybrid connection when client authroization disabled [#8775](https://github.com/azure/azure-cli/issues/8775)</span></span>
* <span data-ttu-id="018bf-1710">Parameter `--requires-transport-security` zu `relay wcfrelay create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1710">Added parameter `--requires-transport-security` to `relay wcfrelay create`</span></span>

### <a name="servicebus"></a><span data-ttu-id="018bf-1711">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="018bf-1711">Servicebus</span></span>

* <span data-ttu-id="018bf-1712">Validierung für Parameter `--rights` von `authorizationrule`-Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1712">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="storage"></a><span data-ttu-id="018bf-1713">Storage</span><span class="sxs-lookup"><span data-stu-id="018bf-1713">Storage</span></span>

* <span data-ttu-id="018bf-1714">AADDS für Files für Speicherkontoaktualisierung aktiviert</span><span class="sxs-lookup"><span data-stu-id="018bf-1714">Enable Files AADDS for storage account update</span></span>
* <span data-ttu-id="018bf-1715">Problem `storage blob service-properties update --set` behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-1715">Fixed issue `storage blob service-properties update --set`</span></span>

## <a name="july-2-2019"></a><span data-ttu-id="018bf-1716">2\. Juli 2019</span><span class="sxs-lookup"><span data-stu-id="018bf-1716">July 2, 2019</span></span>

<span data-ttu-id="018bf-1717">Version 2.0.68</span><span class="sxs-lookup"><span data-stu-id="018bf-1717">Version 2.0.68</span></span>

### <a name="core"></a><span data-ttu-id="018bf-1718">Core</span><span class="sxs-lookup"><span data-stu-id="018bf-1718">Core</span></span>

* <span data-ttu-id="018bf-1719">Befehlsmodule sind jetzt in einer einzelnen verteilbaren Python-Komponente zusammengefasst.</span><span class="sxs-lookup"><span data-stu-id="018bf-1719">Command modules are now consolidated into a single Python distributable.</span></span> <span data-ttu-id="018bf-1720">Die direkte Verwendung zahlreicher Pakete vom Typ `azure-cli-` in PyPI ist daher veraltet.</span><span class="sxs-lookup"><span data-stu-id="018bf-1720">This deprecates direct use of many `azure-cli-` packages on PyPI.</span></span>
  <span data-ttu-id="018bf-1721">Dadurch sollte sich die Installationsgröße reduzieren. Darüber hinaus sollte es nur Benutzer betreffen, die eine direkte Installation über `pip` ausgeführt haben.</span><span class="sxs-lookup"><span data-stu-id="018bf-1721">This should reduce install size and only affect users who have directly installed via `pip`.</span></span>

### <a name="acr"></a><span data-ttu-id="018bf-1722">ACR</span><span class="sxs-lookup"><span data-stu-id="018bf-1722">ACR</span></span>

* <span data-ttu-id="018bf-1723">Unterstützung für Trigger mit Timer zu Aufgabe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1723">Added support for Timer Triggers to Task</span></span>

### <a name="appservice"></a><span data-ttu-id="018bf-1724">AppService</span><span class="sxs-lookup"><span data-stu-id="018bf-1724">Appservice</span></span>

* <span data-ttu-id="018bf-1725">`functionapp create` wurde so geändert, das Application Insights standardmäßig aktiviert wird.</span><span class="sxs-lookup"><span data-stu-id="018bf-1725">Changed `functionapp create` to enable application insights by default</span></span>
* <span data-ttu-id="018bf-1726">[BREAKING CHANGE] Veralteter Befehl `functionapp devops-build` entfernt.</span><span class="sxs-lookup"><span data-stu-id="018bf-1726">[BREAKING CHANGE] Removed deprecated `functionapp devops-build` command.</span></span>
  *  <span data-ttu-id="018bf-1727">Verwenden Sie stattdessen den neuen Befehl `az functionapp devops-pipeline`.</span><span class="sxs-lookup"><span data-stu-id="018bf-1727">Use the new command `az functionapp devops-pipeline` instead</span></span>
* <span data-ttu-id="018bf-1728">Unterstützung des Funktions-App-Plans für Linux-Verbrauch zu `functionapp deployment config-zip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1728">Added Linux Consumption function app plan support to `functionapp deployment config-zip`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="018bf-1729">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="018bf-1729">Cosmos DB</span></span>

* <span data-ttu-id="018bf-1730">Unterstützung für das Deaktivieren von TTL hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1730">Added support for disabling TTL</span></span>

### <a name="dls"></a><span data-ttu-id="018bf-1731">DLS</span><span class="sxs-lookup"><span data-stu-id="018bf-1731">DLS</span></span>

* <span data-ttu-id="018bf-1732">Aktualisierte ADLS-Version (0.0.45)</span><span class="sxs-lookup"><span data-stu-id="018bf-1732">Updated ADLS version (0.0.45)</span></span>

### <a name="feedback"></a><span data-ttu-id="018bf-1733">Feedback</span><span class="sxs-lookup"><span data-stu-id="018bf-1733">Feedback</span></span>

* <span data-ttu-id="018bf-1734">Wird ein fehlgeschlagener Erweiterungsbefehl gemeldet, versucht `az feedback` nun, über den Index die Projekt-/Repository-URL der Erweiterung im Browser zu öffnen.</span><span class="sxs-lookup"><span data-stu-id="018bf-1734">When reporting a failed extension command, `az feedback` now attempts to open the browser to the project/repo url of the extension from the index</span></span>

### <a name="hdinsight"></a><span data-ttu-id="018bf-1735">HDInsight</span><span class="sxs-lookup"><span data-stu-id="018bf-1735">HDInsight</span></span>

* <span data-ttu-id="018bf-1736">[BREAKING CHANGE] Der Befehlsgruppenname `oms` wurde in `monitor` geändert.</span><span class="sxs-lookup"><span data-stu-id="018bf-1736">[BREAKING CHANGE] Changed `oms` command group name to `monitor`</span></span>
* <span data-ttu-id="018bf-1737">[BREAKING CHANGE]`--http-password/-p` als erforderlicher Parameter festgelegt</span><span class="sxs-lookup"><span data-stu-id="018bf-1737">[BREAKING CHANGE] Made `--http-password/-p` a required parameter</span></span> 
* <span data-ttu-id="018bf-1738">Vervollständigungen für `--cluster-admin-account` und `cluster-users-group-dns` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1738">Added completers for `--cluster-admin-account` and `cluster-users-group-dns` parameters completer</span></span> 
* <span data-ttu-id="018bf-1739">Parameter `cluster-users-group-dns` so geändert, dass er erforderlich ist, wenn `—esp` vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="018bf-1739">Changed `cluster-users-group-dns` parameter to be required when `—esp` is present</span></span>
* <span data-ttu-id="018bf-1740">Timeout für alle vorhandenen automatischen Argumentvervollständigungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1740">Added a timeout for all existing argument auto-completers</span></span>
* <span data-ttu-id="018bf-1741">Timeout für das Transformieren des Ressourcennamens in eine Ressourcen-ID hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1741">Added a timeout for transforming resource name to resource id</span></span>
* <span data-ttu-id="018bf-1742">Die automatischen Vervollständigungen wurden so geändert, dass Ressourcen aus einer beliebigen Ressourcengruppe ausgewählt werden.</span><span class="sxs-lookup"><span data-stu-id="018bf-1742">Changed Auto-completers to select resources from any resource group.</span></span> <span data-ttu-id="018bf-1743">Dabei kann es sich um eine andere Ressourcengruppe als die mit `-g` angegebene Gruppe handeln.</span><span class="sxs-lookup"><span data-stu-id="018bf-1743">It can be a different resource group than the one specified with `-g`</span></span>
* <span data-ttu-id="018bf-1744">Unterstützung für die Parameter `--sub-domain-suffix` und `--disable_gateway_auth` im Befehl `hdinsight application create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1744">Added support for `--sub-domain-suffix` and `--disable_gateway_auth` parameters in the `hdinsight application create` command</span></span>

### <a name="managed-services"></a><span data-ttu-id="018bf-1745">Verwaltete Dienste</span><span class="sxs-lookup"><span data-stu-id="018bf-1745">Managed Services</span></span>

* <span data-ttu-id="018bf-1746">Befehlsmodul für verwaltete Dienste als Vorschau eingeführt</span><span class="sxs-lookup"><span data-stu-id="018bf-1746">Introducing managed service command module in preview</span></span>

### <a name="profile"></a><span data-ttu-id="018bf-1747">Profil</span><span class="sxs-lookup"><span data-stu-id="018bf-1747">Profile</span></span>
* <span data-ttu-id="018bf-1748">Argument `--subscription` für Abmeldebefehl unterdrückt</span><span class="sxs-lookup"><span data-stu-id="018bf-1748">Suppress `--subscription` argument for logout command</span></span>

### <a name="rbac"></a><span data-ttu-id="018bf-1749">RBAC</span><span class="sxs-lookup"><span data-stu-id="018bf-1749">RBAC</span></span>

* <span data-ttu-id="018bf-1750">[BREAKING CHANGE] Argument `--password` für `create-for-rbac` entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-1750">[BREAKING CHANGE] Removed `--password` argument for `create-for-rbac`</span></span>
* <span data-ttu-id="018bf-1751">Parameter `--assignee-principal-type` zum Befehl `create` hinzugefügt, um zeitweilige Fehler zu vermeiden, die durch die Replikationswartezeit des AAD-Graph-Servers verursacht werden</span><span class="sxs-lookup"><span data-stu-id="018bf-1751">Added `--assignee-principal-type` parameter to `create` command to avoid intermittent failures caused by AAD graph server replication latency</span></span>
* <span data-ttu-id="018bf-1752">Absturz in `ad signed-in-user` beim Auflisten von in Besitz befindlichen Objekten behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-1752">Fixed a crash in `ad signed-in-user` when listing owned objects</span></span>
* <span data-ttu-id="018bf-1753">Problem behoben, aufgrund dessen `ad sp` nicht die richtige Anwendung über einen Dienstprinzipal fand</span><span class="sxs-lookup"><span data-stu-id="018bf-1753">Fixed issue where `ad sp` would not find the right application from a service principal</span></span>

### <a name="rdbms"></a><span data-ttu-id="018bf-1754">RDBMS</span><span class="sxs-lookup"><span data-stu-id="018bf-1754">RDBMS</span></span>

* <span data-ttu-id="018bf-1755">Unterstützung für die Replikation für MariaDB hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1755">Added support for replication for MariaDB</span></span>

### <a name="sql"></a><span data-ttu-id="018bf-1756">SQL</span><span class="sxs-lookup"><span data-stu-id="018bf-1756">SQL</span></span>

* <span data-ttu-id="018bf-1757">Zulässige Werte für `sql db create --sample-name` dokumentiert</span><span class="sxs-lookup"><span data-stu-id="018bf-1757">Documented allowed values for `sql db create --sample-name`</span></span>

### <a name="storage"></a><span data-ttu-id="018bf-1758">Storage</span><span class="sxs-lookup"><span data-stu-id="018bf-1758">Storage</span></span>

* <span data-ttu-id="018bf-1759">Unterstützung von SAS-Token für die Benutzerdelegierung mit `--as-user` zu `storage blob generate-sas` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1759">Added user delegation SAS token support with `--as-user` to `storage blob generate-sas`</span></span> 
* <span data-ttu-id="018bf-1760">Unterstützung von SAS-Token für die Benutzerdelegierung mit `--as-user` zu `storage container generate-sas` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1760">Added user delegation SAS token support with `--as-user` to `storage container generate-sas`</span></span> 

### <a name="vm"></a><span data-ttu-id="018bf-1761">VM</span><span class="sxs-lookup"><span data-stu-id="018bf-1761">VM</span></span>

* <span data-ttu-id="018bf-1762">Fehler behoben, aufgrund dessen `vmss create` bei der Ausführung mit `--no-wait` eine Fehlermeldung zurückgab</span><span class="sxs-lookup"><span data-stu-id="018bf-1762">Fixed bug where `vmss create` returns an error message when run with `--no-wait`</span></span>
* <span data-ttu-id="018bf-1763">Die clientseitige Validierung für `vmss create --single-placement-group` wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="018bf-1763">Removed client-side validation for `vmss create --single-placement-group`.</span></span> <span data-ttu-id="018bf-1764">Es tritt kein Fehler auf, wenn `--single-placement-group` auf `true` und für `--instance-count` ein größerer Wert als 100 festgelegt wird oder wenn Verfügbarkeitszonen angegeben werden. Diese Validierung wird jedoch dem Computedienst überlassen.</span><span class="sxs-lookup"><span data-stu-id="018bf-1764">Does not fail if `--single-placement-group` is set to `true` and`--instance-count` is greater than 100 or availability zones are specified, but leaves this validation to the compute service</span></span>
* <span data-ttu-id="018bf-1765">Problem behoben, aufgrund dessen bei der Verwendung von `--latest` für `[vm|vmss] extension image list` ein Fehler auftrat</span><span class="sxs-lookup"><span data-stu-id="018bf-1765">Fixed bug where `[vm|vmss] extension image list` fails when used with `--latest`</span></span>


## <a name="june-18-2019"></a><span data-ttu-id="018bf-1766">18. Juni 2019</span><span class="sxs-lookup"><span data-stu-id="018bf-1766">June 18, 2019</span></span>

<span data-ttu-id="018bf-1767">Version 2.0.67</span><span class="sxs-lookup"><span data-stu-id="018bf-1767">Version 2.0.67</span></span>

### <a name="core"></a><span data-ttu-id="018bf-1768">Core</span><span class="sxs-lookup"><span data-stu-id="018bf-1768">Core</span></span>

<span data-ttu-id="018bf-1769">In diesem Release wird das neue [Preview]-Tag eingeführt, um Kunden gegenüber deutlich zu machen, dass sich eine Befehlsgruppe, ein Befehl oder ein Argument in der Vorschauphase befindet.</span><span class="sxs-lookup"><span data-stu-id="018bf-1769">This release introduces a new [Preview] tag to more clearly communicate to customers when a command group, command or argument is in preview status.</span></span> <span data-ttu-id="018bf-1770">Diese Information war zuvor im Hilfetext oder implizit durch die Versionsnummer des Befehlsmoduls angegeben.</span><span class="sxs-lookup"><span data-stu-id="018bf-1770">This was previously called out in help text or communicated implicitly by the command module version number.</span></span>
<span data-ttu-id="018bf-1771">Die Befehlszeilenschnittstelle wird künftig Versionsnummern für einzelne Pakete entfernen.</span><span class="sxs-lookup"><span data-stu-id="018bf-1771">The CLI will be removing version numbers for individual packages in the future.</span></span> <span data-ttu-id="018bf-1772">Wenn sich ein Befehl in der Vorschauphase befindet, gilt dies auch für alle seine Argumente.</span><span class="sxs-lookup"><span data-stu-id="018bf-1772">If a command is in preview, all of its arguments are as well.</span></span> <span data-ttu-id="018bf-1773">Wenn eine Befehlsgruppe als Vorschau gekennzeichnet ist, befinden sich auch alle Befehle und Argumente in der Vorschauphase.</span><span class="sxs-lookup"><span data-stu-id="018bf-1773">If a command group is labeled as being in preview, then all commands and arguments are considered to be in preview as well.</span></span>

<span data-ttu-id="018bf-1774">Infolge dieser Änderung befinden sich in diesem Release verschiedene Befehlsgruppen anscheinend „plötzlich“ in der Vorschauphase.</span><span class="sxs-lookup"><span data-stu-id="018bf-1774">As a result of this change, several command groups may seem to "suddenly" appear to be in a preview status with this release.</span></span> <span data-ttu-id="018bf-1775">Tatsächlich ist es jedoch so, dass sich die meisten Pakete in der Vorschauphase befanden, in diesem Release jedoch als allgemein verfügbar gelten.</span><span class="sxs-lookup"><span data-stu-id="018bf-1775">What actually happened is that most packages were in a preview status, but are being deemed GA with this release</span></span>

### <a name="acr"></a><span data-ttu-id="018bf-1776">ACR</span><span class="sxs-lookup"><span data-stu-id="018bf-1776">ACR</span></span>
* <span data-ttu-id="018bf-1777">Befehl „acr check-health“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1777">Added 'acr check-health' command</span></span>
* <span data-ttu-id="018bf-1778">Verbesserte Fehlerbehandlung für AAD-Token und für das Abrufen externer Befehle</span><span class="sxs-lookup"><span data-stu-id="018bf-1778">Improved error handling for AAD tokens and for retrieving external commands</span></span>

### <a name="acs"></a><span data-ttu-id="018bf-1779">ACS</span><span class="sxs-lookup"><span data-stu-id="018bf-1779">ACS</span></span>
* <span data-ttu-id="018bf-1780">Veraltete ACS-Befehle werden jetzt in der Hilfeansicht ausgeblendet.</span><span class="sxs-lookup"><span data-stu-id="018bf-1780">Deprecated ACS commands are now hidden from help view</span></span>

### <a name="ams"></a><span data-ttu-id="018bf-1781">AMS</span><span class="sxs-lookup"><span data-stu-id="018bf-1781">AMS</span></span>
* <span data-ttu-id="018bf-1782">[BREAKING CHANGE] Änderung, damit ISO 8601-Zeitzeichenfolgen für „archive-window-length“ und „key-frame-interval-duration“ zurückgegeben werden</span><span class="sxs-lookup"><span data-stu-id="018bf-1782">[BREAKING CHANGE] Changed to return ISO 8601 time strings for archive-window-length and key-frame-interval-duration</span></span>

### <a name="appservice"></a><span data-ttu-id="018bf-1783">AppService</span><span class="sxs-lookup"><span data-stu-id="018bf-1783">AppService</span></span>
* <span data-ttu-id="018bf-1784">Standortbasiertes Routing für `webapp deleted list` und `webapp deleted restore` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1784">Added location based routing for `webapp deleted list` and `webapp deleted restore`</span></span>
* <span data-ttu-id="018bf-1785">Problem behoben, aufgrund dessen in Azure Cloud Shell nicht auf die von einer Web-App protokollierte Ziel-URL („Sie können die App starten unter...“) geklickt werden konnte</span><span class="sxs-lookup"><span data-stu-id="018bf-1785">Fixed issue where webapp up logged target URL ("You can launch the app at...") was not clickable in Azure Cloud Shell</span></span>
* <span data-ttu-id="018bf-1786">Problem behoben, aufgrund dessen beim Erstellen von Apps bei einigen SKUs ein AlwaysOn-Fehler auftrat</span><span class="sxs-lookup"><span data-stu-id="018bf-1786">Fixed an issue where creating apps with the some SKUs was failing with an AlwaysOn error</span></span>
* <span data-ttu-id="018bf-1787">Vorabüberprüfung zu `[appservice|webapp] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1787">Added pre-validation to `[appservice|webapp] create`</span></span>
* <span data-ttu-id="018bf-1788">`[webapp|functionapp] traffic-routing` korrigiert, damit der richtige actionHostName-Wert verwendet wird</span><span class="sxs-lookup"><span data-stu-id="018bf-1788">Fixed `[webapp|functionapp] traffic-routing` to use the correct actionHostName</span></span>
* <span data-ttu-id="018bf-1789">Slotunterstützung zu `functionapp`-Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1789">Added slot support to `functionapp` commands</span></span>

### <a name="batch"></a><span data-ttu-id="018bf-1790">Batch</span><span class="sxs-lookup"><span data-stu-id="018bf-1790">Batch</span></span>
* <span data-ttu-id="018bf-1791">AAD-Authentifizierungsregression korrigiert, die von übermäßiger Berichterstellung für Authentifizierung mit gemeinsam verwendetem Schlüssel verursacht wurde</span><span class="sxs-lookup"><span data-stu-id="018bf-1791">Fixed AAD auth regression caused by over-aggressive error reporting for Shared Key Auth</span></span>

### <a name="batchai"></a><span data-ttu-id="018bf-1792">Batch AI</span><span class="sxs-lookup"><span data-stu-id="018bf-1792">BatchAI</span></span>
* <span data-ttu-id="018bf-1793">BatchAI-Befehle sind jetzt veraltet und ausgeblendet.</span><span class="sxs-lookup"><span data-stu-id="018bf-1793">BatchAI commands are now deprecated and hidden</span></span>

### <a name="botservice"></a><span data-ttu-id="018bf-1794">BotService</span><span class="sxs-lookup"><span data-stu-id="018bf-1794">BotService</span></span>
* <span data-ttu-id="018bf-1795">Für Befehle, die Version 3 des SDK unterstützen, wurden die Warnmeldungen „Support eingestellt“/„Wartungsmodus“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1795">Added "discontinued support"/"maintenance mode" warning messages for commands that support the v3 SDK</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="018bf-1796">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="018bf-1796">CosmosDB</span></span>
* <span data-ttu-id="018bf-1797">[VERALTET] Der Befehl `cosmosdb list-keys` wurde als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="018bf-1797">[DEPRECATED] Deprecated the `cosmosdb list-keys` command</span></span>
* <span data-ttu-id="018bf-1798">Befehl `cosmosdb keys list` hinzugefügt, er ersetzt `cosmosdb list-keys`.</span><span class="sxs-lookup"><span data-stu-id="018bf-1798">Added the `cosmosdb keys list` command - replaces `cosmosdb list-keys`</span></span>
* <span data-ttu-id="018bf-1799">`cosmsodb create/update`: Neues Format für „--location“ hinzugefügt, um das Festlegen der Eigenschaft „isZoneRedundant“ zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="018bf-1799">`cosmsodb create/update`: Added new format for --location to allow setting "isZoneRedundant" property.</span></span> <span data-ttu-id="018bf-1800">Das alte Format wurde als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="018bf-1800">Deprecated old format</span></span>

### <a name="eventgrid"></a><span data-ttu-id="018bf-1801">EventGrid</span><span class="sxs-lookup"><span data-stu-id="018bf-1801">EventGrid</span></span>
* <span data-ttu-id="018bf-1802">`eventgrid domain`-Befehle für CRUD-Vorgänge für Domänen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1802">Added `eventgrid domain` commands for domain CRUD operations</span></span>
* <span data-ttu-id="018bf-1803">`eventgrid domain topic`-Befehle für CRUD-Vorgänge für Domänenthemen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1803">Added `eventgrid domain topic` commands for domain topics CRUD operations</span></span>
* <span data-ttu-id="018bf-1804">Argument `--odata-query` zu `eventgrid [topic|event-subscription] list` zum Filtern der Ergebnisse mithilfe von OData-Syntax hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1804">Added `--odata-query` argument to `eventgrid [topic|event-subscription] list` for filtering results using OData syntax</span></span>
* <span data-ttu-id="018bf-1805">`event-subscription create/update`: „servicebusqueue“ als neue Werte für den Parameter `--endpoint-type` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1805">`event-subscription create/update`: Added servicebusqueue as new values for the `--endpoint-type` parameter</span></span>
* <span data-ttu-id="018bf-1806">[BREAKING CHANGE] Unterstützung für `--included-event-types All` mit `eventgrid event-subscription [create|update]` entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-1806">[BREAKING CHANGE] Removed support for `--included-event-types All` with `eventgrid event-subscription [create|update]`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="018bf-1807">HDInsight</span><span class="sxs-lookup"><span data-stu-id="018bf-1807">HDInsight</span></span>
* <span data-ttu-id="018bf-1808">Unterstützung für den Parameter `--ssh-public-key` im Befehl vom Typ `hdinsight create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1808">Added support for `--ssh-public-key` parameter in `hdinsight create` command</span></span>

### <a name="iot"></a><span data-ttu-id="018bf-1809">IoT</span><span class="sxs-lookup"><span data-stu-id="018bf-1809">IoT</span></span>
* <span data-ttu-id="018bf-1810">Unterstützung für das erneute Generieren von Autorisierungsrichtlinienschlüsseln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1810">Added support to regenerate authorization policy keys</span></span>
* <span data-ttu-id="018bf-1811">SDK und Unterstützung für den Bereitstellungsdienst des DigitalTwin-Repositorys hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1811">Added SDK and support for DigitalTwin Repository Provisioning Service</span></span>

### <a name="network"></a><span data-ttu-id="018bf-1812">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="018bf-1812">Network</span></span>
* <span data-ttu-id="018bf-1813">Zonenunterstützung für NAT Gateway hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1813">Added Zone support for Nat Gateway</span></span>
* <span data-ttu-id="018bf-1814">Befehl `network list-service-tags` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1814">Added command `network list-service-tags`</span></span>
* <span data-ttu-id="018bf-1815">Problem mit `dns zone import` behoben, aufgrund dessen Benutzer keine A-Platzhaltereinträge importieren konnten</span><span class="sxs-lookup"><span data-stu-id="018bf-1815">Fixed issue with `dns zone import` where users could not import wildcard A records</span></span>
* <span data-ttu-id="018bf-1816">Problem mit `watcher flow-log configure` behoben, aufgrund dessen die Flowprotokollierung in bestimmten Regionen nicht aktiviert werden konnte</span><span class="sxs-lookup"><span data-stu-id="018bf-1816">Fixed issue with `watcher flow-log configure` where flow logging could not be enabled in certain regions</span></span>

### <a name="resource"></a><span data-ttu-id="018bf-1817">Resource</span><span class="sxs-lookup"><span data-stu-id="018bf-1817">Resource</span></span>
* <span data-ttu-id="018bf-1818">Befehl `az rest` zum Ausführen von REST-Aufrufen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1818">Added `az rest` command for making REST calls</span></span>
* <span data-ttu-id="018bf-1819">Fehler behoben, der bei Verwendung von `policy assignment list` mit `--scope` auf Ressourcengruppen- oder Abonnementebene auftrat</span><span class="sxs-lookup"><span data-stu-id="018bf-1819">Fixed error when using `policy assignment list` with a resource group or subscription level `--scope`</span></span>

### <a name="servicebus"></a><span data-ttu-id="018bf-1820">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="018bf-1820">ServiceBus</span></span>
* <span data-ttu-id="018bf-1821">Problem mit `servicebus topic create --max-size` behoben [Nr. 9319](https://github.com/azure/azure-cli/issues/9319)</span><span class="sxs-lookup"><span data-stu-id="018bf-1821">Fixed issue with `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span></span>

### <a name="sql"></a><span data-ttu-id="018bf-1822">SQL</span><span class="sxs-lookup"><span data-stu-id="018bf-1822">SQL</span></span>
* <span data-ttu-id="018bf-1823">`--location` wurde geändert und ist nun für `sql [server|mi] create` optional. Ohne Angabe wird der Ressourcengruppenstandort verwendet.</span><span class="sxs-lookup"><span data-stu-id="018bf-1823">Changed `--location` to be optional for `sql [server|mi] create` - uses resource group location if not specified</span></span>
* <span data-ttu-id="018bf-1824">Der Fehler, dass das Objekt „NoneType“ nicht wiederholbar ist, wurde für `sql db list-editions --available` behoben.</span><span class="sxs-lookup"><span data-stu-id="018bf-1824">Fixed "'NoneType' object is not iterable" error for `sql db list-editions --available`</span></span>

### <a name="sqlvm"></a><span data-ttu-id="018bf-1825">SQLVm</span><span class="sxs-lookup"><span data-stu-id="018bf-1825">SQLVm</span></span>
* <span data-ttu-id="018bf-1826">[WICHTIGE ÄNDERUNG] `sql vm create` wurde geändert und erfordert nun den Parameter `--license-type`.</span><span class="sxs-lookup"><span data-stu-id="018bf-1826">[BREAKING CHNAGE] Changed `sql vm create` to require `--license-type` parameter</span></span>
* <span data-ttu-id="018bf-1827">Änderung, um beim Erstellen oder Aktualisieren einer SQL-VM das Festlegen der SQL-Image-SKU zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="018bf-1827">Changed to allow setting SQL image SKU when creating or updating a sql vm</span></span>

### <a name="storage"></a><span data-ttu-id="018bf-1828">Storage</span><span class="sxs-lookup"><span data-stu-id="018bf-1828">Storage</span></span>
* <span data-ttu-id="018bf-1829">Problem mit fehlendem Kontoschlüssel für `storage container generate-sas` behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-1829">Fixed issue with missing account key for `storage container generate-sas`</span></span>
* <span data-ttu-id="018bf-1830">Problem mit `storage blob sync` unter Linux behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-1830">Fixed issue with `storage blob sync` on Linux</span></span>

### <a name="vm"></a><span data-ttu-id="018bf-1831">VM</span><span class="sxs-lookup"><span data-stu-id="018bf-1831">VM</span></span>
* <span data-ttu-id="018bf-1832">[VORSCHAU] Befehle vom Typ `vm image template` zum Erstellen von VM-Images hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1832">[PREVIEW] Added `vm image template` commands to build VM images</span></span>

## <a name="june-4-2019"></a><span data-ttu-id="018bf-1833">4\. Juni 2019</span><span class="sxs-lookup"><span data-stu-id="018bf-1833">June 4, 2019</span></span>

<span data-ttu-id="018bf-1834">Version 2.0.66</span><span class="sxs-lookup"><span data-stu-id="018bf-1834">Version 2.0.66</span></span>

### <a name="core"></a><span data-ttu-id="018bf-1835">Core</span><span class="sxs-lookup"><span data-stu-id="018bf-1835">Core</span></span>
* <span data-ttu-id="018bf-1836">Fehler behoben, aufgrund dessen bei Befehlen ein Fehler auftrat, wenn `--output yaml` mit `--query` verwendet wurde</span><span class="sxs-lookup"><span data-stu-id="018bf-1836">Fixed bug where commands fail if `--output yaml` is used with `--query`</span></span>

### <a name="acr"></a><span data-ttu-id="018bf-1837">ACR</span><span class="sxs-lookup"><span data-stu-id="018bf-1837">ACR</span></span>
* <span data-ttu-id="018bf-1838">Befehlsgruppe „acr pack“ zum Erstellen von Aufgaben zur Schnellerstellung mit Buildpacks hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1838">Added 'acr pack' command group for creating quick build Tasks using Buildpacks.</span></span>

### <a name="acs"></a><span data-ttu-id="018bf-1839">ACS</span><span class="sxs-lookup"><span data-stu-id="018bf-1839">ACS</span></span>
* <span data-ttu-id="018bf-1840">Zulassen der Aktivierung/Deaktivierung des AKS-Add-Ons für das Kube-Dashboard</span><span class="sxs-lookup"><span data-stu-id="018bf-1840">Allow enabling/disabling AKS kube-dashboard addon</span></span>
* <span data-ttu-id="018bf-1841">Ausgeben einer benutzerfreundlichen Nachricht, wenn das Abonnement nicht in der Whitelist zur Verwendung von Azure Red Hat OpenShift enthalten ist</span><span class="sxs-lookup"><span data-stu-id="018bf-1841">Print a friendly message when the subscription is not whitelisted to use Azure Red Hat OpenShift</span></span>

### <a name="batch"></a><span data-ttu-id="018bf-1842">Batch</span><span class="sxs-lookup"><span data-stu-id="018bf-1842">Batch</span></span>
* <span data-ttu-id="018bf-1843">Bessere Fehlerbehandlung, wenn der Benutzer nicht bei einem Konto angemeldet ist \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span><span class="sxs-lookup"><span data-stu-id="018bf-1843">Improved error handling when not logged in to an account \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span></span>

### <a name="iot"></a><span data-ttu-id="018bf-1844">IoT</span><span class="sxs-lookup"><span data-stu-id="018bf-1844">IoT</span></span>
* <span data-ttu-id="018bf-1845">Unterstützung für manuelles Failover hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1845">Added support for manual failover</span></span>

### <a name="network"></a><span data-ttu-id="018bf-1846">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="018bf-1846">Network</span></span>
* <span data-ttu-id="018bf-1847">Befehle vom Typ `network application-gateway waf-policy` hinzugefügt, um benutzerdefinierte WAF-Regeln zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="018bf-1847">Added `network application-gateway waf-policy` commands to support custom WAF rules.</span></span>
* <span data-ttu-id="018bf-1848">Argumente `--waf-policy` und `--max-capacity` zu `network application-gateway [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1848">Added `--waf-policy` and `--max-capacity` arguments to `network application-gateway [create|update]`</span></span> 

### <a name="resource"></a><span data-ttu-id="018bf-1849">Resource</span><span class="sxs-lookup"><span data-stu-id="018bf-1849">Resource</span></span>
* <span data-ttu-id="018bf-1850">Verbesserte Fehlermeldungen aus `deployment create`, wenn TTY nicht verfügbar ist</span><span class="sxs-lookup"><span data-stu-id="018bf-1850">Improved error message from `deployment create` when there is no TTY available</span></span>

### <a name="role"></a><span data-ttu-id="018bf-1851">Role</span><span class="sxs-lookup"><span data-stu-id="018bf-1851">Role</span></span>
* <span data-ttu-id="018bf-1852">Hilfetext aktualisiert</span><span class="sxs-lookup"><span data-stu-id="018bf-1852">Updated help text.</span></span>

### <a name="compute"></a><span data-ttu-id="018bf-1853">Compute</span><span class="sxs-lookup"><span data-stu-id="018bf-1853">Compute</span></span>
* <span data-ttu-id="018bf-1854">Unterstützung zu `vm create` für virtuelle Computer aus einem verwalteten Image mit Datenträger-LUNs hinzugefügt, die nicht bei 0 beginnen oder die Nummern überspringen</span><span class="sxs-lookup"><span data-stu-id="018bf-1854">Added support to `vm create` for VMs from a managed image with data-disk luns that do not start from 0 or that skip numbers</span></span>

## <a name="may-21-2019"></a><span data-ttu-id="018bf-1855">21. Mai 2019</span><span class="sxs-lookup"><span data-stu-id="018bf-1855">May 21, 2019</span></span>

<span data-ttu-id="018bf-1856">Version 2.0.65</span><span class="sxs-lookup"><span data-stu-id="018bf-1856">Version 2.0.65</span></span>

### <a name="core"></a><span data-ttu-id="018bf-1857">Core</span><span class="sxs-lookup"><span data-stu-id="018bf-1857">Core</span></span>
* <span data-ttu-id="018bf-1858">Besseres Feedback für Authentifizierungsfehler hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1858">Added better feedback for authentication errors</span></span>
* <span data-ttu-id="018bf-1859">Problem behoben, aufgrund dessen die CLI Erweiterungen lädt, die nicht mit der Core-Version kompatibel waren</span><span class="sxs-lookup"><span data-stu-id="018bf-1859">Fixed issue where the CLI would load extensions that were not compatible with its core version</span></span>
* <span data-ttu-id="018bf-1860">Problem beim Starten behoben, wenn `clouds.config` beschädigt ist</span><span class="sxs-lookup"><span data-stu-id="018bf-1860">Fixed issue with launching when `clouds.config` is corrupted</span></span>

### <a name="acr"></a><span data-ttu-id="018bf-1861">ACR</span><span class="sxs-lookup"><span data-stu-id="018bf-1861">ACR</span></span>
* <span data-ttu-id="018bf-1862">Unterstützung für verwaltete Identitäten zu Aufgaben hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1862">Added support for Managed Identities to Tasks</span></span>

### <a name="acs"></a><span data-ttu-id="018bf-1863">ACS</span><span class="sxs-lookup"><span data-stu-id="018bf-1863">ACS</span></span>
* <span data-ttu-id="018bf-1864">`openshift create`-Befehl bei der Verwendung mit dem AAD-Kundenclient korrigiert</span><span class="sxs-lookup"><span data-stu-id="018bf-1864">Fixed `openshift create` command when used with customer AAD client</span></span>

### <a name="appservice"></a><span data-ttu-id="018bf-1865">AppService</span><span class="sxs-lookup"><span data-stu-id="018bf-1865">AppService</span></span>
* <span data-ttu-id="018bf-1866">[VERALTET] Befehl `functionapp devops-build` als veraltet gekennzeichnet – wird in der nächsten Version entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-1866">[DEPRECATED] Deprecated `functionapp devops-build` command - will be removed in next release</span></span>
* <span data-ttu-id="018bf-1867">`functionapp devops-pipeline` geändert, um das Buildprotokoll von Azure DevOps im ausführlichen Modus abzurufen</span><span class="sxs-lookup"><span data-stu-id="018bf-1867">Changed `functionapp devops-pipeline` to fetch build log from Azure DevOps in verbose mode</span></span>
* <span data-ttu-id="018bf-1868">[BREAKING CHANGE] Flag `--use_local_settings` aus dem Befehl `functionapp devops-pipeline` entfernt – kein Vorgang wurde ausgeführt</span><span class="sxs-lookup"><span data-stu-id="018bf-1868">[BREAKING CHANGE] Removed `--use_local_settings` flag from `functionapp devops-pipeline` command - was a no-op</span></span>
* <span data-ttu-id="018bf-1869">`webapp up` geändert, sodass die JSON-Ausgabe zurückgegeben wird, wenn `--logs` nicht verwendet wird</span><span class="sxs-lookup"><span data-stu-id="018bf-1869">Changed `webapp up` to return JSON output if `--logs` is not used</span></span>
* <span data-ttu-id="018bf-1870">Unterstützung hinzugefügt zum Schreiben von Standardressourcen in die lokale Konfiguration für `webapp up`</span><span class="sxs-lookup"><span data-stu-id="018bf-1870">Added support for writing default resources to local config for `webapp up`</span></span>
* <span data-ttu-id="018bf-1871">Unterstützung zu `webapp up` hinzugefügt für die erneute Bereitstellung einer App ohne Verwendung des `--location`-Arguments</span><span class="sxs-lookup"><span data-stu-id="018bf-1871">Added support to `webapp up` for redeploying an app without using the `--location` argument</span></span>
* <span data-ttu-id="018bf-1872">Problem behoben, bei dem für die ASP-Erstellung der Linux-SKU „Free“ der SKU-Wert „Free“ nicht funktioniert hat</span><span class="sxs-lookup"><span data-stu-id="018bf-1872">Fixed an issue where for Linux Free SKU ASP creation use Free as SKU value was not working</span></span>

### <a name="botservice"></a><span data-ttu-id="018bf-1873">BotService</span><span class="sxs-lookup"><span data-stu-id="018bf-1873">BotService</span></span>
* <span data-ttu-id="018bf-1874">Geändert, sodass Groß-/Kleinschreibung für `--lang`-Parameter für Befehle zulässig ist</span><span class="sxs-lookup"><span data-stu-id="018bf-1874">Changed to allow all casing for `--lang` parameters for commands</span></span>
* <span data-ttu-id="018bf-1875">Beschreibung für das Befehlsmodul aktualisiert</span><span class="sxs-lookup"><span data-stu-id="018bf-1875">Updated description for command module</span></span>

### <a name="consumption"></a><span data-ttu-id="018bf-1876">Nutzung</span><span class="sxs-lookup"><span data-stu-id="018bf-1876">Consumption</span></span>
* <span data-ttu-id="018bf-1877">Fehlende erforderliche Parameter bei der Ausführung von `consumption usage list --billing-period-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1877">Added missing required parameter when running `consumption usage list --billing-period-name`</span></span>

### <a name="iot"></a><span data-ttu-id="018bf-1878">IoT</span><span class="sxs-lookup"><span data-stu-id="018bf-1878">IoT</span></span>
* <span data-ttu-id="018bf-1879">Unterstützung für das Auflisten aller Schlüssel hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1879">Added support to list all keys</span></span>

### <a name="network"></a><span data-ttu-id="018bf-1880">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="018bf-1880">Network</span></span>
* [BREAKING CHANGE]: Removed `network interface-endpoints` command group - use `network private-endpoints` 
* <span data-ttu-id="018bf-1882">`--nat-gateway`-Argument zu `network vnet subnet [create|update]` für das Anfügen an ein NAT-Gateway hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1882">Added `--nat-gateway` argument to `network vnet subnet [create|update]` for attaching to a NAT gateway</span></span>
* <span data-ttu-id="018bf-1883">Problem mit `dns zone import` behoben, aufgrund dessen Eintragsnamen keinem Datensatztyp entsprochen haben</span><span class="sxs-lookup"><span data-stu-id="018bf-1883">Fixed issue with `dns zone import` where record names could not match a record type</span></span>

### <a name="rdbms"></a><span data-ttu-id="018bf-1884">RDBMS</span><span class="sxs-lookup"><span data-stu-id="018bf-1884">RDBMS</span></span>
* <span data-ttu-id="018bf-1885">Postgres- und MySLQ-Unterstützung für die Georeplikation hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1885">Added postgres and mysql support for geo replication</span></span>

### <a name="rbac"></a><span data-ttu-id="018bf-1886">RBAC</span><span class="sxs-lookup"><span data-stu-id="018bf-1886">RBAC</span></span>
* <span data-ttu-id="018bf-1887">Unterstützung für den Verwaltungsgruppenumfang zu `role assignment` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1887">Added support for management group scope to `role assignment`</span></span>

### <a name="storage"></a><span data-ttu-id="018bf-1888">Storage</span><span class="sxs-lookup"><span data-stu-id="018bf-1888">Storage</span></span>
* <span data-ttu-id="018bf-1889">`storage blob sync`: Synchronisierungsbefehl für Speicherblob hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1889">`storage blob sync`: add sync command for storage blob</span></span>

### <a name="compute"></a><span data-ttu-id="018bf-1890">Compute</span><span class="sxs-lookup"><span data-stu-id="018bf-1890">Compute</span></span>
* <span data-ttu-id="018bf-1891">`--computer-name` zu `vm create` zum Festlegen des Computernamens eines virtuellen Computers hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1891">Added `--computer-name` to `vm create` for setting a VM's computer name</span></span>
* <span data-ttu-id="018bf-1892">`--ssh-key-value` umbenannt in `--ssh-key-values` für `[vm|vmss] create`: Jetzt können mehrere öffentliche SSH-Schlüsselwerte oder -pfade akzeptiert werden.</span><span class="sxs-lookup"><span data-stu-id="018bf-1892">Renamed `--ssh-key-value` renamed to `--ssh-key-values` for `[vm|vmss] create` - can now accept multiple ssh public key values or paths</span></span>
  * <span data-ttu-id="018bf-1893">__Hinweis__ : Dies ist **kein** Breaking Change: `--ssh-key-value` wird korrekt analysiert, da nur eine Übereinstimmung mit `--ssh-key-values` besteht.</span><span class="sxs-lookup"><span data-stu-id="018bf-1893">__Note__ : This is **not** a breaking change - `--ssh-key-value` will be parsed correctly as it matches only `--ssh-key-values`</span></span>
* <span data-ttu-id="018bf-1894">`--type`-Argument von `ppg create` in optionales Argument geändert</span><span class="sxs-lookup"><span data-stu-id="018bf-1894">Changed the `--type` argument of `ppg create` to be optional</span></span>

## <a name="may-6-2019"></a><span data-ttu-id="018bf-1895">6\. Mai 2019</span><span class="sxs-lookup"><span data-stu-id="018bf-1895">May 6, 2019</span></span>

<span data-ttu-id="018bf-1896">Version 2.0.64</span><span class="sxs-lookup"><span data-stu-id="018bf-1896">Version 2.0.64</span></span>

### <a name="acs"></a><span data-ttu-id="018bf-1897">ACS</span><span class="sxs-lookup"><span data-stu-id="018bf-1897">ACS</span></span>
* <span data-ttu-id="018bf-1898">[BREAKING CHANGE] Flag `--fqdn` aus den `openshift`-Befehlen entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-1898">[BREAKING CHANGE] Removed `--fqdn` flag on `openshift` commands</span></span>
* <span data-ttu-id="018bf-1899">Geändert, sodass die allgemein verfügbare Azure Red Hat Openshift-API-Version verwendet wird</span><span class="sxs-lookup"><span data-stu-id="018bf-1899">Changed to use Azure Red Hat Openshift GA API Version</span></span>
* <span data-ttu-id="018bf-1900">Flag `customer-admin-group-id` wurde zu `openshift create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-1900">Added `customer-admin-group-id` flag to `openshift create`</span></span>
* <span data-ttu-id="018bf-1901">[ALLGEMEIN VERFÜGBAR] `(PREVIEW)` aus der `aks create`-Option `--network-policy` entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-1901">[GA] Removed `(PREVIEW)` from `aks create` option `--network-policy`</span></span>

### <a name="appservice"></a><span data-ttu-id="018bf-1902">AppService</span><span class="sxs-lookup"><span data-stu-id="018bf-1902">Appservice</span></span>
* <span data-ttu-id="018bf-1903">[VERALTET] Befehl `functionapp devops-build` als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="018bf-1903">[DEPRECATED] Deprecated `functionapp devops-build` command</span></span>
  * <span data-ttu-id="018bf-1904">Umbenannt in `functionapp devops-pipeline`</span><span class="sxs-lookup"><span data-stu-id="018bf-1904">Renamed to `functionapp devops-pipeline`</span></span>
* <span data-ttu-id="018bf-1905">Fehler beim Abrufen des richtigen Benutzernamens für Cloud Shell behoben, der einen Fehler von `webapp up` verursachte</span><span class="sxs-lookup"><span data-stu-id="018bf-1905">Fixed getting the correct username for cloudshell which was causing `webapp up` to fail</span></span>
* <span data-ttu-id="018bf-1906">Dokumentation von `appservice plan --sku` mit den unterstützten App Service-Plänen aktualisiert</span><span class="sxs-lookup"><span data-stu-id="018bf-1906">Updated `appservice plan --sku` documentation updated to reflect the supported appserviceplans</span></span>
* <span data-ttu-id="018bf-1907">Optionale Argumente für Ressourcengruppe und Plan zu `webapp up` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1907">Added optional arguments for resource group and plan to `webapp up`</span></span>
* <span data-ttu-id="018bf-1908">Unterstützung zur Berücksichtigung der Umgebungsvariablen `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` zu `webapp ssh` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1908">Added support to `webapp ssh` to respect `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>
* <span data-ttu-id="018bf-1909">Unterstützung für `appserviceplan create` für die kostenlose Linux-SKU hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1909">Added `appserviceplan create` support for Linux Free SKU</span></span>
* <span data-ttu-id="018bf-1910">`webapp up` geändert, um nach dem Festlegen der App-Einstellung `SCM_DO_BUILD_DURING_DEPLOYMENT=true` zum Verarbeiten des Kudu-Kaltstarts für 30 Sekunden in den Energiesparmodus zu wechseln</span><span class="sxs-lookup"><span data-stu-id="018bf-1910">Changed `webapp up` to have a 30s sleep after setting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` appsetting to handle kudu cold start</span></span>
* <span data-ttu-id="018bf-1911">Unterstützung für die `powershell`-Runtime zu `functionapp create` unter Windows hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1911">Added support for `powershell` runtime to `functionapp create` on Windows</span></span>
* <span data-ttu-id="018bf-1912">Befehl `create-remote-connection` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1912">Added `create-remote-connection` command</span></span>

### <a name="batch"></a><span data-ttu-id="018bf-1913">Batch</span><span class="sxs-lookup"><span data-stu-id="018bf-1913">Batch</span></span>
* <span data-ttu-id="018bf-1914">Fehler im Validierungssteuerelement für `--application-package-references`-Optionen korrigiert</span><span class="sxs-lookup"><span data-stu-id="018bf-1914">Fixed bug in validator for `--application-package-references` options</span></span>

### <a name="botservice"></a><span data-ttu-id="018bf-1915">Botservice</span><span class="sxs-lookup"><span data-stu-id="018bf-1915">Botservice</span></span>
* <span data-ttu-id="018bf-1916">[BREAKING CHANGE]`bot create -v v4 -k webapp` geändert, sodass standardmäßig eine leerer Web-App-Bot erstellt wird (d. h. kein Bot wird in App Service bereitgestellt)</span><span class="sxs-lookup"><span data-stu-id="018bf-1916">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to create an empty Web App Bot by default (i.e. no bot is deployed to the App Service)</span></span>
* <span data-ttu-id="018bf-1917">`--echo`-Flag zu `bot create` hinzugefügt, sodass das alte Verhalten mit `-v v4` verwendet wird</span><span class="sxs-lookup"><span data-stu-id="018bf-1917">Added `--echo` flag to `bot create` to use the old behavior with `-v v4`</span></span>
* <span data-ttu-id="018bf-1918">[BREAKING CHANGE] Standardwert von `--version` in `v4` geändert</span><span class="sxs-lookup"><span data-stu-id="018bf-1918">[BREAKING CHANGE] Changed the default value of  `--version` to `v4`</span></span>
  * <span data-ttu-id="018bf-1919">__HINWEIS:__ `bot prepare-publish` verwendet weiterhin den alten Standard.</span><span class="sxs-lookup"><span data-stu-id="018bf-1919">__NOTE:__ `bot prepare-publish` still uses the its old default</span></span>
* <span data-ttu-id="018bf-1920">[BREAKING CHANGE]`--lang` geändert, sodass der Standard nicht mehr `Csharp` ist.</span><span class="sxs-lookup"><span data-stu-id="018bf-1920">[BREAKING CHANGE] Changed `--lang` to no longer default to `Csharp`.</span></span> <span data-ttu-id="018bf-1921">Wenn der Befehl `--lang` erfordert und dies nicht angegeben ist, wird der Befehl nun mit Fehler beendet.</span><span class="sxs-lookup"><span data-stu-id="018bf-1921">If the command requires `--lang` and it is not provided, the command will now error out</span></span>
* <span data-ttu-id="018bf-1922">[BREAKING CHANGE]`--appid`- und `--password`-Argumente für `bot create` in erforderlich geändert, sie können jetzt über `ad app create` erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="018bf-1922">[BREAKING CHANGE] Changed the `--appid` and `--password` args for `bot create` to be required and can now be created via `ad app create`</span></span>
* <span data-ttu-id="018bf-1923">`--appid`- und `--password`-Validierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1923">Added `--appid` and `--password` validation</span></span>
* <span data-ttu-id="018bf-1924">[BREAKING CHANGE]`bot create -v v4` geändert, sodass kein Speicherkonto bzw. keine Application Insights-Instanz erstellt oder verwendet wird</span><span class="sxs-lookup"><span data-stu-id="018bf-1924">[BREAKING CHANGE] Changed `bot create -v v4` to not create or use a Storage Account or Application Insights</span></span>
* <span data-ttu-id="018bf-1925">[BREAKING CHANGE]`bot create -v v3` geändert, sodass eine Region erforderlich ist, in der Application Insights verfügbar ist</span><span class="sxs-lookup"><span data-stu-id="018bf-1925">[BREAKING CHANGE] Changed `bot create -v v3` to require a region where Application Insights is available</span></span>
* <span data-ttu-id="018bf-1926">[BREAKING CHANGE]`bot update` geändert, sodass es sich jetzt nur auf spezifische Eigenschaften eines Bots auswirkt</span><span class="sxs-lookup"><span data-stu-id="018bf-1926">[BREAKING CHANGE] Changed `bot update` to now affect only specific properties of a bot</span></span>
* <span data-ttu-id="018bf-1927">[BREAKING CHANGE]`--lang`-Flags geändert, sodass `Javascript` anstelle von `Node` akzeptiert wird</span><span class="sxs-lookup"><span data-stu-id="018bf-1927">[BREAKING CHANGE] Changed `--lang` flags to accept `Javascript` instead of `Node`</span></span>
* <span data-ttu-id="018bf-1928">[BREAKING CHANGE]`Node` als zulässiger `--lang`-Wert entfernt.</span><span class="sxs-lookup"><span data-stu-id="018bf-1928">[BREAKING CHANGE] Removed `Node` as an allowed `--lang` value</span></span>
* <span data-ttu-id="018bf-1929">[BREAKING CHANGE]`bot create -v v4 -k webapp` geändert, sodass `SCM_DO_BUILD_DURING_DEPLOYMENT` nicht mehr auf TRUE festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="018bf-1929">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to no longer set `SCM_DO_BUILD_DURING_DEPLOYMENT` to true.</span></span> <span data-ttu-id="018bf-1930">Alle Bereitstellungen über Kudu fungieren ihrem Standardverhalten entsprechend.</span><span class="sxs-lookup"><span data-stu-id="018bf-1930">All deployments through Kudu will act according to their default behavior</span></span>
* <span data-ttu-id="018bf-1931">`bot download` für Bots ohne `.bot`-Dateien geändert, sodass die sprachspezifische Konfigurationsdatei mit Werten aus den Anwendungseinstellungen für den Bot erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="018bf-1931">Changed `bot download` for bots without `.bot` files to create the language-specific configuration file with values from the Application Settings for the bot</span></span>
* <span data-ttu-id="018bf-1932">Unterstützung für `Typescript` zu `bot prepare-deploy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1932">Added `Typescript` support to `bot prepare-deploy`</span></span>
* <span data-ttu-id="018bf-1933">Warnmeldung zu `bot prepare-deploy` für `Javascript`- und `Typescript`-Bots hinzugefügt, wenn `package.json` in `--code-dir` nicht enthalten ist</span><span class="sxs-lookup"><span data-stu-id="018bf-1933">Added warning message to `bot prepare-deploy` for `Javascript` and `Typescript` bots for when `--code-dir` does not contain `package.json`</span></span>
* <span data-ttu-id="018bf-1934">`bot prepare-deploy` geändert, sodass bei Erfolg `true` zurückgegeben wird</span><span class="sxs-lookup"><span data-stu-id="018bf-1934">Changed `bot prepare-deploy` to return `true` if successful</span></span>
* <span data-ttu-id="018bf-1935">Ausführliche Protokollierung zu `bot prepare-deploy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1935">Added verbose logging to `bot prepare-deploy`</span></span>
* <span data-ttu-id="018bf-1936">Mehr verfügbare Application Insights-Regionen zu `az bot create -v v3` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1936">Added more available Application Insights regions to `az bot create -v v3`</span></span>

### <a name="configure"></a><span data-ttu-id="018bf-1937">Konfigurieren</span><span class="sxs-lookup"><span data-stu-id="018bf-1937">Configure</span></span>
* <span data-ttu-id="018bf-1938">Unterstützung für die ordnerbasierte Argument-Standardwertkonfigurationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1938">Added support for folder based argument default value configurations</span></span>

### <a name="eventhubs"></a><span data-ttu-id="018bf-1939">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="018bf-1939">Eventhubs</span></span>
* <span data-ttu-id="018bf-1940">Befehle vom Typ `namespace network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1940">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="018bf-1941">`--default-action`-Argument für Netzwerkregeln zu `namespace [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1941">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="018bf-1942">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="018bf-1942">Network</span></span>
* <span data-ttu-id="018bf-1943">[BREAKING CHANGE]`--cache`-Argument mit `--defer` für `vnet [create|update]` ersetzt</span><span class="sxs-lookup"><span data-stu-id="018bf-1943">[BREAKING CHANGE] Replaced `--cache` arugment with `--defer` for `vnet [create|update]`</span></span> 

### <a name="policy-insights"></a><span data-ttu-id="018bf-1944">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="018bf-1944">Policy Insights</span></span>
* <span data-ttu-id="018bf-1945">Unterstützung für `--expand PolicyEvaluationDetails` hinzugefügt, sodass Richtlinienauswertungsdetails von der Ressource abgefragt werden</span><span class="sxs-lookup"><span data-stu-id="018bf-1945">Added support for `--expand PolicyEvaluationDetails` to query policy evaluation details on the resource</span></span>

### <a name="role"></a><span data-ttu-id="018bf-1946">Role</span><span class="sxs-lookup"><span data-stu-id="018bf-1946">Role</span></span>
* <span data-ttu-id="018bf-1947">[VERALTET]: Ausblenden des „--password"-Arguments von `create-for-rbac` geändert; Unterstützung wird im Mai 2019 entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-1947">[DEPRECATED] Changed `create-for-rbac` hide '--password' argument - support will be removed in May 2019</span></span>

### <a name="service-bus"></a><span data-ttu-id="018bf-1948">Service Bus</span><span class="sxs-lookup"><span data-stu-id="018bf-1948">Service Bus</span></span>
* <span data-ttu-id="018bf-1949">Befehle vom Typ `namespace network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1949">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="018bf-1950">`--default-action`-Argument für Netzwerkregeln zu `namespace [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1950">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>
* <span data-ttu-id="018bf-1951">`topic [create|update]` korrigiert, sodass `--max-size`-Unterstützung für 10-, 20-, 40- und 80-GB-Werte mit Premium-SKU zulässig ist</span><span class="sxs-lookup"><span data-stu-id="018bf-1951">Fixed `topic [create|update]` to allow `--max-size` support for 10, 20, 40 and 80GB values with premium SKU</span></span>

### <a name="sql"></a><span data-ttu-id="018bf-1952">SQL</span><span class="sxs-lookup"><span data-stu-id="018bf-1952">SQL</span></span>
* <span data-ttu-id="018bf-1953">Befehle vom Typ `sql virtual-cluster [list|show|delete]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1953">Added `sql virtual-cluster [list|show|delete]` commands</span></span>

### <a name="vm"></a><span data-ttu-id="018bf-1954">VM</span><span class="sxs-lookup"><span data-stu-id="018bf-1954">VM</span></span>
* <span data-ttu-id="018bf-1955">`--protect-from-scale-in` und `--protect-from-scale-set-actions` zu `vmss update` hinzugefügt, sodass Aktualisierungen der Schutzrichtlinie von VMSS-VM-Instanzen aktiviert sind</span><span class="sxs-lookup"><span data-stu-id="018bf-1955">Added `--protect-from-scale-in` and `--protect-from-scale-set-actions` to `vmss update` to enable updates to the protection policy of VMSS VM instances</span></span>
* <span data-ttu-id="018bf-1956">`--instance-id` zu `vmss update` hinzugefügt, sodass allgemeine Aktualisierungen von VMSS-VM-Instanzen aktiviert sind</span><span class="sxs-lookup"><span data-stu-id="018bf-1956">Added `--instance-id` to `vmss update` to enable generic update of VMSS VM instances</span></span>
* <span data-ttu-id="018bf-1957">`--instance-id` zu `vmss wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1957">Added `--instance-id` to `vmss wait`</span></span>
* <span data-ttu-id="018bf-1958">Neue `ppg`-Befehlsgruppe für die Verwaltung von Näherungsplatzierungsgruppen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1958">Added new `ppg` command group for managing Proximity Placement Groups</span></span>
* <span data-ttu-id="018bf-1959">`--ppg` zu `[vm|vmss] create` und `vm availability-set create` für die Verwaltung von PPGs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1959">Added `--ppg` to `[vm|vmss] create` and `vm availability-set create` for managing PPGs</span></span>
* <span data-ttu-id="018bf-1960">Parameter `--hyper-v-generation` zu `image create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1960">Added `--hyper-v-generation` parameter to `image create`</span></span>

## <a name="april-23-2019"></a><span data-ttu-id="018bf-1961">23. April 2019</span><span class="sxs-lookup"><span data-stu-id="018bf-1961">April 23, 2019</span></span>

<span data-ttu-id="018bf-1962">Version 2.0.63</span><span class="sxs-lookup"><span data-stu-id="018bf-1962">Version 2.0.63</span></span>

### <a name="acs"></a><span data-ttu-id="018bf-1963">ACS</span><span class="sxs-lookup"><span data-stu-id="018bf-1963">ACS</span></span>
* <span data-ttu-id="018bf-1964">`aks get-credentials` zur Anzeige einer Eingabeaufforderung zum Überschreiben doppelter Werte geändert</span><span class="sxs-lookup"><span data-stu-id="018bf-1964">Changed `aks get-credentials` to prompt to overwrite duplicated values</span></span>
* <span data-ttu-id="018bf-1965">`(PREVIEW)` aus Dev Spaces-Befehlen „aks use-dev-spaces“ und „aks remove-dev-spaces“ entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-1965">Removed `(PREVIEW)` from Dev Spaces commands "aks use-dev-spaces" and "aks remove-dev-spaces"</span></span>

### <a name="ams"></a><span data-ttu-id="018bf-1966">AMS</span><span class="sxs-lookup"><span data-stu-id="018bf-1966">AMS</span></span>
* <span data-ttu-id="018bf-1967">Fehler bei der Objekt- und Kontofilteraktualisierung behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-1967">Fixed bug with asset and account filters update</span></span>

### <a name="appservice"></a><span data-ttu-id="018bf-1968">AppService</span><span class="sxs-lookup"><span data-stu-id="018bf-1968">AppService</span></span>
* <span data-ttu-id="018bf-1969">Unterstützung für die App Service-Umgebung (App Service Environment, ASE) und Zeitlimit zu `webapp ssh` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1969">Added support for ASE and timeout to `webapp ssh`</span></span>
* <span data-ttu-id="018bf-1970">Unterstützung für die Einrichtung von CI/CD für eine Azure DevOps-Pipeline aus einem GitHub-Repository zu Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1970">Added support for establishing CI CD to an Azure DevOps pipeline from a Github repository to Function apps</span></span>
* <span data-ttu-id="018bf-1971">`--github-pat`-Argument zu `functionapp devops-build create` hinzugefügt, um persönliche GitHub-Zugriffstoken zu akzeptieren</span><span class="sxs-lookup"><span data-stu-id="018bf-1971">Added `--github-pat` argument to `functionapp devops-build create` to accept Github personal access token</span></span>
* <span data-ttu-id="018bf-1972">`--github-repository`-Argument zu `functionapp devops-build create` hinzugefügt, um das GitHub-Repository mit dem Quellcode einer Funktions-App zu akzeptieren</span><span class="sxs-lookup"><span data-stu-id="018bf-1972">Added `--github-repository` argument to `functionapp devops-build create` to accept Github repository that contains a functionapp source code</span></span>
* <span data-ttu-id="018bf-1973">Problem behoben, aufgrund dessen bei `az webapp up --logs` ein Fehler auftrat und die .NET Core-Standardversion auf 2.1 aktualisiert wurde</span><span class="sxs-lookup"><span data-stu-id="018bf-1973">Fixed issue where `az webapp up --logs` was failing with a error and updating default .NETCORE version to 2.1</span></span>
* <span data-ttu-id="018bf-1974">Unnötige Funktions-App-Einstellungen beim Erstellen einer Funktions-App mit Verbrauchsplan entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-1974">Removed unnecessary functionapp settings when creating a function app with consumption plan</span></span>
* <span data-ttu-id="018bf-1975">`webapp up` geändert, sodass die ASP-Standardzeichenfolge jetzt eine Zahl am Ende anfügt, um einen neuen ASP basierend auf SKU-Optionen zu erstellen</span><span class="sxs-lookup"><span data-stu-id="018bf-1975">Changed `webapp up` so the default asp string now appends number at the end to create a new ASP based on SKU options</span></span>
* <span data-ttu-id="018bf-1976">`-b` als Option für `webapp up` hinzugefügt, um die App im Browser zu starten</span><span class="sxs-lookup"><span data-stu-id="018bf-1976">Added `-b` as an option to `webapp up` to launch the app in the browser</span></span>
* <span data-ttu-id="018bf-1977">`webapp deployment source config zip` geändert, um die `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`-Umgebungsvariable zu behandeln</span><span class="sxs-lookup"><span data-stu-id="018bf-1977">Changed `webapp deployment source config zip` to handle `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="018bf-1978">Bereitstellungs-Manager</span><span class="sxs-lookup"><span data-stu-id="018bf-1978">Deployment Manager</span></span>
* <span data-ttu-id="018bf-1979">[VORSCHAUVERSIPN] Erstellen und Verwalten von Artefakten, die Rollouts unterstützen</span><span class="sxs-lookup"><span data-stu-id="018bf-1979">[PREVIEW] Create and manage artifacts that support rollouts</span></span>

### <a name="lab"></a><span data-ttu-id="018bf-1980">Labor</span><span class="sxs-lookup"><span data-stu-id="018bf-1980">Lab</span></span>
* <span data-ttu-id="018bf-1981">Fehler behoben, der zu einer vorzeitigen Beendigung führen würde</span><span class="sxs-lookup"><span data-stu-id="018bf-1981">Fixed bug which would cause an early exit</span></span>

### <a name="network"></a><span data-ttu-id="018bf-1982">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="018bf-1982">Network</span></span>
* <span data-ttu-id="018bf-1983">Automatische Delegierung des Namenservers im übergeordneten Element während der Erstellung der untergeordneten Zone zu `dns zone create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1983">Added auto name server delegation to `dns zone create` in parent during child zone creation</span></span>

### <a name="resource"></a><span data-ttu-id="018bf-1984">Resource</span><span class="sxs-lookup"><span data-stu-id="018bf-1984">Resource</span></span>
* <span data-ttu-id="018bf-1985">[VERALTET]: Argumente `--link-id`, `--target-id` und `--filter-string` von `resource link` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="018bf-1985">[DEPRECATED] Deprecated `--link-id`, `--target-id` and `--filter-string` arguments of `resource link`</span></span>
  * <span data-ttu-id="018bf-1986">Verwenden Sie stattdessen die Argumente `--link`, `--target` und `--filter`.</span><span class="sxs-lookup"><span data-stu-id="018bf-1986">Use the arguments `--link`, `--target`, and `--filter` instead</span></span>
* <span data-ttu-id="018bf-1987">Problem behoben, aufgrund dessen `resource link [create|update]`-Befehle nicht verwendet werden konnten</span><span class="sxs-lookup"><span data-stu-id="018bf-1987">Fixed issue where `resource link [create|update]` commands would not work</span></span>
* <span data-ttu-id="018bf-1988">Problem behoben, aufgrund dessen das Löschen anhand einer Ressourcen-ID bei einem Fehler zu einem Absturz führen konnte</span><span class="sxs-lookup"><span data-stu-id="018bf-1988">Fixed an issue where deleting using a resource ID could crash on error</span></span>

### <a name="sql"></a><span data-ttu-id="018bf-1989">SQL</span><span class="sxs-lookup"><span data-stu-id="018bf-1989">SQL</span></span>
* <span data-ttu-id="018bf-1990">Unterstützung für benutzerdefinierte Zeitzonen auf verwalteten Instanzen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1990">Added support for custom time zone on managed instances</span></span>
* <span data-ttu-id="018bf-1991">Geändert, um die Verwendung des Namens eines Pools für elastische Datenbanken mit `sql db update` zuzulassen</span><span class="sxs-lookup"><span data-stu-id="018bf-1991">Changed to allow elastic pool name to be used with `sql db update`</span></span>
* <span data-ttu-id="018bf-1992">Unterstützung für `--no-wait` zu `sql server [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1992">Added `--no-wait` support to `sql server [create|update]`</span></span>
* <span data-ttu-id="018bf-1993">Befehl `sql server wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1993">Added command `sql server wait`</span></span>

### <a name="storage"></a><span data-ttu-id="018bf-1994">Storage</span><span class="sxs-lookup"><span data-stu-id="018bf-1994">Storage</span></span>
* <span data-ttu-id="018bf-1995">Problem mit doppelt codierten SAS-Token in `storage blob generate-sas` behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-1995">Fixed issue with double-encoded SAS tokens in `storage blob generate-sas`</span></span>

### <a name="vm"></a><span data-ttu-id="018bf-1996">VM</span><span class="sxs-lookup"><span data-stu-id="018bf-1996">VM</span></span>
* <span data-ttu-id="018bf-1997">`--skip-shutdown`-Flag zum Ausschalten von VMs ohne Herunterfahren zu `vm|vmss stop` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1997">Added `--skip-shutdown` flag to `vm|vmss stop` to power-off VMs without shutdown</span></span>
* <span data-ttu-id="018bf-1998">`--storage-account-type`-Argument zum Festlegen des Kontotyps des Veröffentlichungsprofils zu `sig image-version create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-1998">Added `--storage-account-type` argument to `sig image-version create` to set the publishing profile's account type</span></span>
* <span data-ttu-id="018bf-1999">`--target-regions`-Argument zu `sig image-version create` hinzugefügt, um das Festlegen von regionsspezifischen Speicherkontotypen zuzulassen</span><span class="sxs-lookup"><span data-stu-id="018bf-1999">Added `--target-regions` argument to `sig image-version create` to allow setting region-specific storage account types</span></span>

## <a name="april-9-2019"></a><span data-ttu-id="018bf-2000">9\. April 2019</span><span class="sxs-lookup"><span data-stu-id="018bf-2000">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="018bf-2001">Core</span><span class="sxs-lookup"><span data-stu-id="018bf-2001">Core</span></span>
* <span data-ttu-id="018bf-2002">Problem behoben, aufgrund dessen einige Erweiterungen mit der Version `Unknown` angezeigt wurden und nicht aktualisiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="018bf-2002">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="018bf-2003">ACR</span><span class="sxs-lookup"><span data-stu-id="018bf-2003">ACR</span></span>
* <span data-ttu-id="018bf-2004">Unterstützung für die kontextlose Ausführung eines Images hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2004">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="018bf-2005">AMS</span><span class="sxs-lookup"><span data-stu-id="018bf-2005">AMS</span></span>
* [VERALTET]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
[DEPRECATED]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [BREAKING CHANGE]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="018bf-2008">Unterstützung für neue Verschlüsselungsparameter in `ams streaming-policy create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2008">Added new encryption parameters support in `ams streaming-policy create`</span></span>
* <span data-ttu-id="018bf-2009">Neuer Parameter `--filters` zu `ams streaming-locator create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2009">Added new paramter `--filters` to `ams streaming-locator create`</span></span>

### <a name="appservice"></a><span data-ttu-id="018bf-2010">AppService</span><span class="sxs-lookup"><span data-stu-id="018bf-2010">AppService</span></span>
* <span data-ttu-id="018bf-2011">Unterstützung für `--logs` zu `webapp up` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2011">Added `--logs` support to `webapp up`</span></span>
* <span data-ttu-id="018bf-2012">Probleme bei der Generierung von `azure-pipelines.yml` beim Befehl `functionapp devops-build create` behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-2012">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="018bf-2013">Fehlerbehandlung und Indikatoren für `unctionapp devops-build create` verbessert</span><span class="sxs-lookup"><span data-stu-id="018bf-2013">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="018bf-2014">[BREAKING CHANGE] Flag `--local-git` für den Befehl `devops-build` entfernt; lokale Git-Erkennung und -Verarbeitung sind zum Erstellen von Azure DevOps-Pipelines obligatorisch</span><span class="sxs-lookup"><span data-stu-id="018bf-2014">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="018bf-2015">Unterstützung für das Erstellen von Linux-Functions-Plänen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2015">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="018bf-2016">Möglichkeit zum Wechseln eines Plans unter einer Funktions-App mit `functionapp update --plan` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2016">Added ability to switch a plan underneath a function app using `functionapp update --plan`</span></span>
* <span data-ttu-id="018bf-2017">Unterstützung für Einstellungen zum Aufskalieren für den Azure Functions-Premium-Plan hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2017">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="018bf-2018">CDN</span><span class="sxs-lookup"><span data-stu-id="018bf-2018">CDN</span></span>
* <span data-ttu-id="018bf-2019">Unterstützung hinzugefügt für `Microsoft_Standard` und `Standard_ChinaCdn`</span><span class="sxs-lookup"><span data-stu-id="018bf-2019">Added support for `Microsoft_Standard` and `Standard_ChinaCdn`</span></span>

### <a name="feedback"></a><span data-ttu-id="018bf-2020">Feedback</span><span class="sxs-lookup"><span data-stu-id="018bf-2020">Feedback</span></span>
* <span data-ttu-id="018bf-2021">`feedback` zur Anzeige von Metadaten zu den zuletzt ausgeführten Befehlen geändert</span><span class="sxs-lookup"><span data-stu-id="018bf-2021">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="018bf-2022">`feedback` geändert, um den Benutzer zur Unterstützung beim Issueerstellungsprozess aufzufordern (durch Öffnen eines Browsers und Verwenden einer Issuevorlage)</span><span class="sxs-lookup"><span data-stu-id="018bf-2022">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="018bf-2023">`feedback` geändert, um den Issuetext bei der Ausführung mit „--verbose“ auszugeben</span><span class="sxs-lookup"><span data-stu-id="018bf-2023">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="018bf-2024">Überwachen</span><span class="sxs-lookup"><span data-stu-id="018bf-2024">Monitor</span></span>
* <span data-ttu-id="018bf-2025">Problem behoben, aufgrund dessen „Count“ kein zulässiger Wert für `metrics alert [create|update]` war</span><span class="sxs-lookup"><span data-stu-id="018bf-2025">Fixed issue where "count" was not a permitted value with `metrics alert [create|update]`</span></span> 

### <a name="network"></a><span data-ttu-id="018bf-2026">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="018bf-2026">Network</span></span>
* <span data-ttu-id="018bf-2027">Problem behoben, aufgrund dessen das Tabellenformat mit `vnet-gateway list-bgp-peer-status` nicht angezeigt wurde</span><span class="sxs-lookup"><span data-stu-id="018bf-2027">Fixed table format not displaying with `vnet-gateway list-bgp-peer-status`</span></span>
* <span data-ttu-id="018bf-2028">Befehle `list-request-headers` und `list-response-headers` zu `application-gateway rewrite-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2028">Added `list-request-headers` and `list-response-headers` commands to `application-gateway rewrite-rule`</span></span>
* <span data-ttu-id="018bf-2029">Befehl `list-server-variables` zu `application-gateway rewrite-rule condition` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2029">Added `list-server-variables` command to `application-gateway rewrite-rule condition`</span></span>
* <span data-ttu-id="018bf-2030">Problem behoben, aufgrund dessen durch das Aktualisieren des Linkstatus für einen ExpressRoute-Port eine Ausnahme vom Typ „unbekanntes Attribut“ ausgelöst wurde: `express-route port update`</span><span class="sxs-lookup"><span data-stu-id="018bf-2030">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception `express-route port update`</span></span>

### <a name="privatedns"></a><span data-ttu-id="018bf-2031">PrivateDNS</span><span class="sxs-lookup"><span data-stu-id="018bf-2031">PrivateDNS</span></span>
* <span data-ttu-id="018bf-2032">`network private-dns` für private DNS-Zonen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2032">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="018bf-2033">Resource</span><span class="sxs-lookup"><span data-stu-id="018bf-2033">Resource</span></span>
* <span data-ttu-id="018bf-2034">Problem mit `deployment create` und `group deployment create` behoben, aufgrund dessen eine Parameterdatei mit leerem Parametersatz nicht verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="018bf-2034">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="018bf-2035">Role</span><span class="sxs-lookup"><span data-stu-id="018bf-2035">Role</span></span>
* <span data-ttu-id="018bf-2036">`create-for-rbac` korrigiert, um `--years` korrekt zu verarbeiten</span><span class="sxs-lookup"><span data-stu-id="018bf-2036">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="018bf-2037">[BREAKING CHANGE]`role assignment delete` geändert, um eine Eingabeaufforderung anzuzeigen, wenn alle Zuweisungen im Abonnement ohne Bedingungen gelöscht werden</span><span class="sxs-lookup"><span data-stu-id="018bf-2037">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="018bf-2038">SQL</span><span class="sxs-lookup"><span data-stu-id="018bf-2038">SQL</span></span>
* <span data-ttu-id="018bf-2039">`sql mi [create|update]` mit den Eigenschaften „proxyOverride“ und „publicDataEndpointEnabled“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="018bf-2039">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="018bf-2040">Storage</span><span class="sxs-lookup"><span data-stu-id="018bf-2040">Storage</span></span>
* <span data-ttu-id="018bf-2041">[BREAKING CHANGE] Ergebnis von `storage blob delete` entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-2041">[BREAKING CHANGE] Removed result of `storage blob delete`</span></span>
* <span data-ttu-id="018bf-2042">`--full-uri` zu `storage blob generate-sas` hinzugefügt, um den vollständigen URI für das Blob mit SAS zu erstellen</span><span class="sxs-lookup"><span data-stu-id="018bf-2042">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="018bf-2043">`--file-snapshot` zu `storage file copy start` hinzugefügt, um die Datei aus der Momentaufnahme zu kopieren</span><span class="sxs-lookup"><span data-stu-id="018bf-2043">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="018bf-2044">`storage blob copy cancel` geändert, um anstelle der Ausnahme für „NoPendingCopyOperation“ nur den Fehler anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="018bf-2044">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="018bf-2045">26. März 2019</span><span class="sxs-lookup"><span data-stu-id="018bf-2045">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="018bf-2046">Core</span><span class="sxs-lookup"><span data-stu-id="018bf-2046">Core</span></span>
* <span data-ttu-id="018bf-2047">Probleme mit der Inkompatibilität der Entwicklungserweiterung behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-2047">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="018bf-2048">Die Fehlerbehandlung verweist Kunden jetzt auf die Problemseite.</span><span class="sxs-lookup"><span data-stu-id="018bf-2048">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="018bf-2049">Cloud</span><span class="sxs-lookup"><span data-stu-id="018bf-2049">Cloud</span></span>
* <span data-ttu-id="018bf-2050">Fehler „Abonnement nicht gefunden“ in `cloud set` behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-2050">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="018bf-2051">ACR</span><span class="sxs-lookup"><span data-stu-id="018bf-2051">ACR</span></span>
* <span data-ttu-id="018bf-2052">Redundante Quellen im Imageimport korrigiert</span><span class="sxs-lookup"><span data-stu-id="018bf-2052">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="018bf-2053">`--auth-mode` wurde den Befehlen `acr build`, `acr run`, `acr task create` und `acr task update` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-2053">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="018bf-2054">Befehlsgruppe „acr task credential“ zum Verwalten von Anmeldeinformationen für eine Aufgabe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2054">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="018bf-2055">„--no-wait“ zum Befehl `acr build` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2055">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="018bf-2056">AppService</span><span class="sxs-lookup"><span data-stu-id="018bf-2056">AppService</span></span>
* <span data-ttu-id="018bf-2057">Problem behoben, das dazu führte, dass die Ausführung aus einem leeren Verzeichnis oder ein Szenario mit unbekannten Code von `webapp up` nicht korrekt behandelt wurde</span><span class="sxs-lookup"><span data-stu-id="018bf-2057">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="018bf-2058">Problem behoben, aufgrund dessen Slots für `[webapp|functionapp] config ssl bind` nicht verwendet werden konnten</span><span class="sxs-lookup"><span data-stu-id="018bf-2058">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="018bf-2059">Bot Service</span><span class="sxs-lookup"><span data-stu-id="018bf-2059">BOT Service</span></span>
* <span data-ttu-id="018bf-2060">`bot prepare-deploy` hinzugefügt, um die Bereitstellung von Bots über `webapp` vorzubereiten</span><span class="sxs-lookup"><span data-stu-id="018bf-2060">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="018bf-2061">`bot create --kind registration` geändert, um das Kennwort anzuzeigen, falls kein Kennwort angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="018bf-2061">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="018bf-2062">[BREAKING CHANGE]`--endpoint` wurde in `bot create --kind registration` geändert, sodass nun standardmäßig eine leere Zeichenfolge verwendet wird, anstatt eine Angabe zu erfordern.</span><span class="sxs-lookup"><span data-stu-id="018bf-2062">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="018bf-2063">`SCM_DO_BUILD_DURING_DEPLOYMENT` zu den Anwendungseinstellungen der ARM-Vorlage für Web-App-Bot (v4) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2063">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="018bf-2064">CDN</span><span class="sxs-lookup"><span data-stu-id="018bf-2064">CDN</span></span>
* <span data-ttu-id="018bf-2065">Unterstützung für `--no-wait` zu `cdn endpoint [create|update|start|stop|delete|load|purge]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2065">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* <span data-ttu-id="018bf-2066">[BREAKING CHANGE] Das standardmäßige Zwischenspeicherverhalten für Abfragezeichenfolgen von `cdn endpoint create` wurde geändert.</span><span class="sxs-lookup"><span data-stu-id="018bf-2066">[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour.</span></span> <span data-ttu-id="018bf-2067">Es wird nicht mehr standardmäßig „IgnoreQueryString“ festgelegt.</span><span class="sxs-lookup"><span data-stu-id="018bf-2067">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="018bf-2068">Er wird jetzt vom Dienst festgelegt.</span><span class="sxs-lookup"><span data-stu-id="018bf-2068">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="018bf-2069">Cosmosdb</span><span class="sxs-lookup"><span data-stu-id="018bf-2069">Cosmosdb</span></span>
* <span data-ttu-id="018bf-2070">Unterstützung für `--enable-multiple-write-locations` bei Kontoaktualisierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2070">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="018bf-2071">Untergruppe `network-rule` mit Befehlen `add`, `remove` und `list` zum Verwalten von VNET-Regeln eines Cosmos DB-Kontos hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2071">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="018bf-2072">Interactive</span><span class="sxs-lookup"><span data-stu-id="018bf-2072">Interactive</span></span>
* <span data-ttu-id="018bf-2073">Inkompatibilität mit der über azdev installierten interaktiven Erweiterung korrigiert</span><span class="sxs-lookup"><span data-stu-id="018bf-2073">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="018bf-2074">Überwachen</span><span class="sxs-lookup"><span data-stu-id="018bf-2074">Monitor</span></span>
* <span data-ttu-id="018bf-2075">Geändert, sodass der Dimensionswert `*` für `monitor metrics alert [create|update]` zulässig ist</span><span class="sxs-lookup"><span data-stu-id="018bf-2075">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="018bf-2076">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="018bf-2076">Network</span></span>
* <span data-ttu-id="018bf-2077">Befehlsgruppe `rewrite-rule` zu `application-gateway` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2077">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="018bf-2078">Profil</span><span class="sxs-lookup"><span data-stu-id="018bf-2078">Profile</span></span>
* <span data-ttu-id="018bf-2079">Kontounterstützung auf Mandantenebene für verwaltete Dienstidentität zu `login` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2079">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="018bf-2080">Postgres</span><span class="sxs-lookup"><span data-stu-id="018bf-2080">Postgres</span></span> 
* <span data-ttu-id="018bf-2081">postgresql-Befehle vom Typ `replica` und Befehl `restart server` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2081">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="018bf-2082">Änderungen vorgenommen, um den Standardspeicherort aus der Ressourcengruppe abzurufen, wenn er für die Erstellung von Servern nicht angegeben wurde, und um eine Überprüfung für die Aufbewahrungstage hinzuzufügen</span><span class="sxs-lookup"><span data-stu-id="018bf-2082">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="018bf-2083">Resource</span><span class="sxs-lookup"><span data-stu-id="018bf-2083">Resource</span></span>
* <span data-ttu-id="018bf-2084">Verbesserte Tabellenausgabe für `deployment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="018bf-2084">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="018bf-2085">Problem mit `deployment [create|validate]` behoben, aufgrund dessen der Typ „secureObject“ nicht erkannt wurde</span><span class="sxs-lookup"><span data-stu-id="018bf-2085">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="018bf-2086">Graph</span><span class="sxs-lookup"><span data-stu-id="018bf-2086">Graph</span></span>
* <span data-ttu-id="018bf-2087">Unterstützung für `--end-date` zu `ad [app|sp] credential reset` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2087">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="018bf-2088">Unterstützung für das Hinzufügen von Berechtigungen mit `ad app permission add` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2088">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="018bf-2089">Fehler mit `ad app permission list` behoben, wenn keine Berechtigungen vorlagen</span><span class="sxs-lookup"><span data-stu-id="018bf-2089">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="018bf-2090">Änderung an `ad sp delete` vorgenommen, um das Entfernen einer Rollenzuweisung zu überspringen, wenn das aktuelle Konto kein Abonnement enthält</span><span class="sxs-lookup"><span data-stu-id="018bf-2090">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="018bf-2091">`ad app create` geändert, sodass ohne Angabe für `--identifier-uris` standardmäßig eine leere Liste verwendet wird</span><span class="sxs-lookup"><span data-stu-id="018bf-2091">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="018bf-2092">storage</span><span class="sxs-lookup"><span data-stu-id="018bf-2092">storage</span></span>
* <span data-ttu-id="018bf-2093">`--snapshot` zu `storage file download-batch` für den Download von einer Freigabemomentaufnahme hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2093">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="018bf-2094">Statusanzeige für `storage blob [download-batch|upload-batch]` geändert, damit sie weniger ausführlich dargestellt wird und das aktuelle Blob angibt</span><span class="sxs-lookup"><span data-stu-id="018bf-2094">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="018bf-2095">Problem mit `storage account update` behoben, das beim Aktualisieren von Verschlüsselungsparametern auftrat</span><span class="sxs-lookup"><span data-stu-id="018bf-2095">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="018bf-2096">Problem behoben, bei dem für `storage blob show` ein Fehler auftrat, wenn oauth (`--auth-mode=login`) verwendet wurde</span><span class="sxs-lookup"><span data-stu-id="018bf-2096">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="018bf-2097">VM</span><span class="sxs-lookup"><span data-stu-id="018bf-2097">VM</span></span>
* <span data-ttu-id="018bf-2098">Befehl `image update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2098">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="018bf-2099">12. März 2019</span><span class="sxs-lookup"><span data-stu-id="018bf-2099">March 12, 2019</span></span>

<span data-ttu-id="018bf-2100">Version 2.0.60</span><span class="sxs-lookup"><span data-stu-id="018bf-2100">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="018bf-2101">Core</span><span class="sxs-lookup"><span data-stu-id="018bf-2101">Core</span></span>

* <span data-ttu-id="018bf-2102">Falsche Fehlermeldung in `cloud set` zu nicht gefundenem Abonnement korrigiert</span><span class="sxs-lookup"><span data-stu-id="018bf-2102">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="018bf-2103">ACR</span><span class="sxs-lookup"><span data-stu-id="018bf-2103">ACR</span></span>

* <span data-ttu-id="018bf-2104">Redundante Quellen im Imageimport korrigiert</span><span class="sxs-lookup"><span data-stu-id="018bf-2104">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="018bf-2105">ACS</span><span class="sxs-lookup"><span data-stu-id="018bf-2105">ACS</span></span>

* <span data-ttu-id="018bf-2106">Änderung vorgenommen, um den Parameter `--listen-address` für `aks browse` zu ignorieren, wenn er nicht von kubectl unterstützt wird</span><span class="sxs-lookup"><span data-stu-id="018bf-2106">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="018bf-2107">AppService</span><span class="sxs-lookup"><span data-stu-id="018bf-2107">AppService</span></span>

* <span data-ttu-id="018bf-2108">`[webapp|functionapp] deployment list-publishing-credentials` hinzugefügt, um die Kudu-Veröffentlichungs-URL und die entsprechenden Anmeldeinformationen abzurufen</span><span class="sxs-lookup"><span data-stu-id="018bf-2108">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="018bf-2109">Fehlerhafte Ausgabeanweisung für `webapp auth update` entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-2109">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="018bf-2110">`functionapp` korrigiert, um das korrekte Image für die Runtime in App Service-Plänen unter Linux festzulegen</span><span class="sxs-lookup"><span data-stu-id="018bf-2110">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="018bf-2111">Vorschau-Tag für `webapp up` entfernt und Verbesserungen am Befehl implementiert</span><span class="sxs-lookup"><span data-stu-id="018bf-2111">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="018bf-2112">Botservice</span><span class="sxs-lookup"><span data-stu-id="018bf-2112">Botservice</span></span>

* <span data-ttu-id="018bf-2113">`SCM_DO_BUILD_DURING_DEPLOYMENT` zu den Anwendungseinstellungen der ARM-Vorlage für Web-App-Bot (v4) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2113">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="018bf-2114">`Microsoft-BotFramework-AppId` und `Microsoft-BotFramework-AppPassword` zu den Anwendungseinstellungen der ARM-Vorlage für Web-App-Bot (v4) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2114">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="018bf-2115">Einfache Anführungszeichen aus der Befehlsausgabe von `bot publish` am Ende von `bot create` entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-2115">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="018bf-2116">`bot publish` wurde geändert und ist jetzt asynchron.</span><span class="sxs-lookup"><span data-stu-id="018bf-2116">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="018bf-2117">Container</span><span class="sxs-lookup"><span data-stu-id="018bf-2117">Container</span></span>

* <span data-ttu-id="018bf-2118">Argument `--no-wait` zu `container [start|restart]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2118">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="018bf-2119">EventHub</span><span class="sxs-lookup"><span data-stu-id="018bf-2119">EventHub</span></span>

* <span data-ttu-id="018bf-2120">Flag `--skip-empty-archives` zu `eventhub create|update` hinzugefügt, um leere Archive in der Aufzeichnung zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="018bf-2120">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="018bf-2121">Suchen</span><span class="sxs-lookup"><span data-stu-id="018bf-2121">Find</span></span>

* <span data-ttu-id="018bf-2122">Umfangreiches Funktionsupdate</span><span class="sxs-lookup"><span data-stu-id="018bf-2122">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="018bf-2123">HDInsight</span><span class="sxs-lookup"><span data-stu-id="018bf-2123">HDInsight</span></span>

* <span data-ttu-id="018bf-2124">Parameter `--storage-account-managed-identity` zu `hdinsight create` hinzugefügt, um MSI in ADLS Gen2 zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="018bf-2124">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="018bf-2125">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="018bf-2125">Network</span></span>

* <span data-ttu-id="018bf-2126">Problem mit `vpn-connection update` behoben, aufgrund dessen die Aktualisierung einer VPN-Verbindung zwischen Gateways in verschiedenen Abonnements fehlschlug</span><span class="sxs-lookup"><span data-stu-id="018bf-2126">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="018bf-2127">Rdbms</span><span class="sxs-lookup"><span data-stu-id="018bf-2127">Rdbms</span></span>

* <span data-ttu-id="018bf-2128">Kleinere Korrekturen, um den Standardspeicherort aus der Ressourcengruppe abzurufen, wenn er für die Erstellung von Servern nicht angegeben wurde, und um eine Überprüfung für die Aufbewahrungstage hinzuzufügen</span><span class="sxs-lookup"><span data-stu-id="018bf-2128">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="018bf-2129">Role</span><span class="sxs-lookup"><span data-stu-id="018bf-2129">Role</span></span>

* <span data-ttu-id="018bf-2130">`role definition update` wurde korrigiert und nutzt nun die ID, um die Definition korrekt aufzulösen.</span><span class="sxs-lookup"><span data-stu-id="018bf-2130">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="018bf-2131">`ad app credential reset` geändert, um die Annahme zu entfernen, dass der Dienstprinzipal der App stets vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="018bf-2131">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="018bf-2132">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="018bf-2132">Service Fabric</span></span>

* <span data-ttu-id="018bf-2133">Das Problem, dass `sf cluster list` nicht wiederholbar war, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="018bf-2133">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="018bf-2134">26. Februar 2019</span><span class="sxs-lookup"><span data-stu-id="018bf-2134">February 26, 2019</span></span>

<span data-ttu-id="018bf-2135">Version 2.0.59</span><span class="sxs-lookup"><span data-stu-id="018bf-2135">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="018bf-2136">Core</span><span class="sxs-lookup"><span data-stu-id="018bf-2136">Core</span></span>

* <span data-ttu-id="018bf-2137">Problem behoben, aufgrund dessen die Verwendung von `--subscription NAME` in einigen Instanzen eine Ausnahme ausgelöst hat</span><span class="sxs-lookup"><span data-stu-id="018bf-2137">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="018bf-2138">ACR</span><span class="sxs-lookup"><span data-stu-id="018bf-2138">ACR</span></span>

* <span data-ttu-id="018bf-2139">Parameter `--target` für die Befehle `acr build`, `acr task create` und `acr task update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2139">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="018bf-2140">Verbesserte Fehlerbehandlung für Runtimebefehle, wenn keine Anmeldung bei Azure besteht</span><span class="sxs-lookup"><span data-stu-id="018bf-2140">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="018bf-2141">ACS</span><span class="sxs-lookup"><span data-stu-id="018bf-2141">ACS</span></span>

* <span data-ttu-id="018bf-2142">Option `--listen-address` zu `aks port-forward` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2142">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="018bf-2143">AppService</span><span class="sxs-lookup"><span data-stu-id="018bf-2143">AppService</span></span>

* <span data-ttu-id="018bf-2144">Befehl `functionapp devops-build` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2144">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="018bf-2145">Batch</span><span class="sxs-lookup"><span data-stu-id="018bf-2145">Batch</span></span>
* <span data-ttu-id="018bf-2146">[BREAKING CHANGE] Befehl `batch pool upgrade os` entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-2146">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="018bf-2147">[BREAKING CHANGE]`Pacakges`-Eigenschaft aus `Application`-Antworten entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-2147">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="018bf-2148">Befehl `batch application package list` zum Auflisten von Paketen einer Anwendung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2148">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="018bf-2149">[BREAKING CHANGE]`--application-id` in allen `batch application`-Befehlen in `--application-name` geändert</span><span class="sxs-lookup"><span data-stu-id="018bf-2149">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="018bf-2150">Argument `--json-file` für Befehle zum Anfordern der unformatierten API-Antwort hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2150">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="018bf-2151">Validierung aktualisiert, sodass das `https://`-Element automatisch in alle Endpunkte aufgenommen wird, wenn es fehlt</span><span class="sxs-lookup"><span data-stu-id="018bf-2151">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="018bf-2152">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="018bf-2152">CosmosDB</span></span>

* <span data-ttu-id="018bf-2153">Untergruppe `network-rule` mit Befehlen `add`, `remove` und `list` zum Verwalten von VNET-Regeln eines Cosmos DB-Kontos hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2153">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="018bf-2154">Kusto</span><span class="sxs-lookup"><span data-stu-id="018bf-2154">Kusto</span></span>

* <span data-ttu-id="018bf-2155">[BREAKING CHANGE] Typen `hot_cache_period` und `soft_delete_period` für Datenbank in Format der Zeitspanne nach ISO8601 geändert</span><span class="sxs-lookup"><span data-stu-id="018bf-2155">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="018bf-2156">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="018bf-2156">Network</span></span>

* <span data-ttu-id="018bf-2157">Argument `--express-route-gateway-bypass` zu `vpn-connection [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2157">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="018bf-2158">Befehlsgruppen aus `express-route`-Erweiterungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2158">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="018bf-2159">Befehlsgruppen `express-route gateway` und `express-route port` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2159">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="018bf-2160">Argument `--legacy-mode` zu `express-route peering [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2160">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="018bf-2161">Argumente `--allow-classic-operations` und `--express-route-port` zu `express-route [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2161">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="018bf-2162">Argument `--gateway-default-site` zu `vnet-gateway [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2162">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="018bf-2163">Befehle vom Typ `ipsec-policy` zu `vnet-gateway` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2163">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="018bf-2164">Resource</span><span class="sxs-lookup"><span data-stu-id="018bf-2164">Resource</span></span>

* <span data-ttu-id="018bf-2165">Problem mit `deployment create` behoben, aufgrund dessen beim Feld „Typ“ die Groß-/Kleinschreibung beachtet wurde</span><span class="sxs-lookup"><span data-stu-id="018bf-2165">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="018bf-2166">Unterstützung für URI-basierte Parameterdatei zu `policy assignment create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2166">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="018bf-2167">Unterstützung für URI-basierte Parameter und Definitionen zu `policy set-definition update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2167">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="018bf-2168">Verarbeitung von Parametern und Regeln für `policy definition update` korrigiert</span><span class="sxs-lookup"><span data-stu-id="018bf-2168">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="018bf-2169">Problem mit `resource show/update/delete/tag/invoke-action` behoben, aufgrund dessen bei abonnementübergreifenden IDs die Abonnement-ID nicht ordnungsgemäß berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="018bf-2169">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="018bf-2170">Role</span><span class="sxs-lookup"><span data-stu-id="018bf-2170">Role</span></span>

* <span data-ttu-id="018bf-2171">Unterstützung für App-Rollen zu `ad app [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2171">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="018bf-2172">VM</span><span class="sxs-lookup"><span data-stu-id="018bf-2172">VM</span></span>

* <span data-ttu-id="018bf-2173">Problem mit `vm create where ` behoben, aufgrund dessen der beschleunigte Netzwerkbetrieb für Ubuntu 18.0 nicht standardmäßig aktiviert war</span><span class="sxs-lookup"><span data-stu-id="018bf-2173">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="018bf-2174">12. Februar 2019</span><span class="sxs-lookup"><span data-stu-id="018bf-2174">February 12, 2019</span></span>

<span data-ttu-id="018bf-2175">Version 2.0.58</span><span class="sxs-lookup"><span data-stu-id="018bf-2175">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="018bf-2176">Core</span><span class="sxs-lookup"><span data-stu-id="018bf-2176">Core</span></span>

* <span data-ttu-id="018bf-2177">`az --version` zeigt jetzt eine Benachrichtigung an, wenn Sie Pakete haben, für die ein Update verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="018bf-2177">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="018bf-2178">Die Regression, dass `--ids` nicht mehr mit JSON-Ausgaben verwendet werden konnte, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="018bf-2178">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="018bf-2179">ACR</span><span class="sxs-lookup"><span data-stu-id="018bf-2179">ACR</span></span>
* <span data-ttu-id="018bf-2180">[BREAKING CHANGE] Die Befehlsgruppe `acr build-task` wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="018bf-2180">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="018bf-2181">[BREAKING CHANGE] Die Optionen `--tag` und `--manifest` wurden aus `acr repository delete` entfernt.</span><span class="sxs-lookup"><span data-stu-id="018bf-2181">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="018bf-2182">ACS</span><span class="sxs-lookup"><span data-stu-id="018bf-2182">ACS</span></span>
* <span data-ttu-id="018bf-2183">Unterstützung für Namen ohne Berücksichtigung von Groß-/Kleinschreibung wurde zu `aks [enable-addons|disable-addons]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-2183">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="018bf-2184">Unterstützung für Azure Active Directory-Aktualisierungsvorgang mithilfe von `aks update-credentials --reset-aad` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-2184">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="018bf-2185">Die Information, dass `--output` für `aks get-credentials` ignoriert wird, wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-2185">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="018bf-2186">AMS</span><span class="sxs-lookup"><span data-stu-id="018bf-2186">AMS</span></span>
* <span data-ttu-id="018bf-2187">Befehle vom Typ `ams streaming-endpoint [start | stop | create | update] wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2187">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="018bf-2188">Befehle vom Typ `ams live-event [create | start | stop | reset] wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2188">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="018bf-2189">AppService</span><span class="sxs-lookup"><span data-stu-id="018bf-2189">Appservice</span></span>
* <span data-ttu-id="018bf-2190">Die Möglichkeit zum Erstellen und Konfigurieren von Funktionen mithilfe von ACR-Containern wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-2190">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="018bf-2191">Unterstützung für das Aktualisieren von Web-App-Konfigurationen über JSON wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-2191">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="018bf-2192">Die Hilfe für `appservice-plan-update` wurde verbessert.</span><span class="sxs-lookup"><span data-stu-id="018bf-2192">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="018bf-2193">Unterstützung für App-Erkenntnisse beim Erstellen von Funktions-Apps wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-2193">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="018bf-2194">Probleme mit der Web-App SSH wurden behoben.</span><span class="sxs-lookup"><span data-stu-id="018bf-2194">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="018bf-2195">Botservice</span><span class="sxs-lookup"><span data-stu-id="018bf-2195">Botservice</span></span>
* <span data-ttu-id="018bf-2196">Die Benutzeroberfläche für `bot publish` wurde verbessert.</span><span class="sxs-lookup"><span data-stu-id="018bf-2196">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="018bf-2197">Eine Warnung für Zeitlimit bei der Ausführung von `npm install` während `az bot publish` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-2197">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="018bf-2198">Ungültiges char-Element wurde `.` aus `--name` in `az bot create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="018bf-2198">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="018bf-2199">Eine Änderung wurde vorgenommen, um die zufällige Zuordnung von Ressourcennamen beim Erstellen von Azure Storage-Instanzen, App Service-Plänen, Funktions-/Web-Apps und Application Insights-Instanzen zu verhindern.</span><span class="sxs-lookup"><span data-stu-id="018bf-2199">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="018bf-2200">[VERALTET] Argument `--proj-name` zugunsten von `--proj-file-path` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="018bf-2200">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="018bf-2201">`az bot publish` wurde geändert, um abgerufene IIS-Bereitstellungsdateien vom Typ „Node.js“ zu entfernen, wenn sie nicht bereits vorhanden waren.</span><span class="sxs-lookup"><span data-stu-id="018bf-2201">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="018bf-2202">Das `--keep-node-modules` Argument wurde zu `az bot publish` hinzugefügt, damit der Ordner `node_modules` in App Service nicht gelöscht wird.</span><span class="sxs-lookup"><span data-stu-id="018bf-2202">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="018bf-2203">Das Schlüssel-Wert-Paar `"publishCommand"` wurde der Ausgabe von `az bot create` beim Erstellen einer Funktions-App oder eines Web-App-Bots hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-2203">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="018bf-2204">Der Wert von `"publishCommand"` ist ein `az bot publish`-Befehl, der bereits die erforderlichen Parameter zum Veröffentlichen des neu erstellten Bots enthält.</span><span class="sxs-lookup"><span data-stu-id="018bf-2204">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="018bf-2205">`"WEBSITE_NODE_DEFAULT_VERSION"` in der ARM-Vorlage wurde so aktualisiert, dass v4-SDK-Bots 10.14.1 anstelle von 8.9.4 verwenden.</span><span class="sxs-lookup"><span data-stu-id="018bf-2205">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="018bf-2206">Key Vault</span><span class="sxs-lookup"><span data-stu-id="018bf-2206">Key Vault</span></span>
* <span data-ttu-id="018bf-2207">Ein Problem mit `keyvault secret backup` wurde behoben, aufgrund dessen einige Benutzer bei Verwendung von `--id` einen `unexpected_keyword`-Fehler erhielten.</span><span class="sxs-lookup"><span data-stu-id="018bf-2207">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="018bf-2208">Überwachen</span><span class="sxs-lookup"><span data-stu-id="018bf-2208">Monitor</span></span>
* <span data-ttu-id="018bf-2209">`monitor metrics alert [create|update]` wurde so geändert, dass der Dimensionswert `*` zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="018bf-2209">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="018bf-2210">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="018bf-2210">Network</span></span>
* <span data-ttu-id="018bf-2211">`dns zone export` wurde geändert, um sicherzustellen, dass es sich bei exportierten CNAMEs um FQDNs handelt.</span><span class="sxs-lookup"><span data-stu-id="018bf-2211">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="018bf-2212">Parameter `--gateway-name` wurde zu `nic ip-config address-pool [add|remove]` hinzugefügt, um Back-End-Adresspools von Anwendungsgateways zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="018bf-2212">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="018bf-2213">Argumente `--traffic-analytics` und `--workspace` wurden zu `network watcher flow-log configure` hinzugefügt, um Datenverkehrsanalysen über einen Log Analytics-Arbeitsbereich zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="018bf-2213">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="018bf-2214">`--idle-timeout` und `--floating-ip` wurden zu `lb inbound-nat-pool [create|update]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-2214">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="018bf-2215">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="018bf-2215">Policy Insights</span></span>
* <span data-ttu-id="018bf-2216">`policy remediation`-Befehle wurden hinzugefügt, um Korrekturfunktionen der Ressourcenrichtlinie zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="018bf-2216">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="018bf-2217">RDBMS</span><span class="sxs-lookup"><span data-stu-id="018bf-2217">RDBMS</span></span>
* <span data-ttu-id="018bf-2218">Hilfemeldung und Befehlsparameter wurden verbessert.</span><span class="sxs-lookup"><span data-stu-id="018bf-2218">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="018bf-2219">Redis</span><span class="sxs-lookup"><span data-stu-id="018bf-2219">Redis</span></span>
* <span data-ttu-id="018bf-2220">Befehle zum Verwalten von „firewall-rules“ (erstellen, aktualisieren, löschen, anzeigen, auflisten) wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-2220">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="018bf-2221">Befehle zum Verwalten von „server-link“ (erstellen, aktualisieren, löschen, anzeigen, auflisten) wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-2221">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="018bf-2222">Befehle zum Verwalten von „patch-schedule“ (erstellen, aktualisieren, löschen, anzeigen, auflisten) wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-2222">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="018bf-2223">Unterstützung für Verfügbarkeitszonen und TLS-Mindestversion wurden zu „redis create“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-2223">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="018bf-2224">[BREAKING CHANGE] Befehle `redis update-settings` und `redis list-all` wurden entfernt.</span><span class="sxs-lookup"><span data-stu-id="018bf-2224">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="018bf-2225">[BREAKING CHANGE] Parameter für `redis create`: „Mandanteneinstellungen“ werden im Format „Schlüssel[=Wert] nicht akzeptiert.</span><span class="sxs-lookup"><span data-stu-id="018bf-2225">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="018bf-2226">[VERALTET] Warnmeldung zur Markierung des Befehls `redis import-method` als veraltet hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2226">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="018bf-2227">Role</span><span class="sxs-lookup"><span data-stu-id="018bf-2227">Role</span></span>
* <span data-ttu-id="018bf-2228">[BREAKING CHANGE] Befehl `az identity` wurde aus den `vm`-Befehlen hierher verschoben.</span><span class="sxs-lookup"><span data-stu-id="018bf-2228">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="018bf-2229">SQL-VM</span><span class="sxs-lookup"><span data-stu-id="018bf-2229">SQL VM</span></span>
* <span data-ttu-id="018bf-2230">[VERALTET] Argument `--boostrap-acc-pwd` aufgrund eines Tippfehlers als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="018bf-2230">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="018bf-2231">VM</span><span class="sxs-lookup"><span data-stu-id="018bf-2231">VM</span></span>
* <span data-ttu-id="018bf-2232">`vm list-skus` wurde so geändert, dass `--all` anstelle von `--all true` verwendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="018bf-2232">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="018bf-2233">`vmss run-command [invoke | list | show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2233">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="018bf-2234">Ein Fehler wurde behoben, aufgrund dessen bei der Ausführung von `vmss encryption enable` bisher ein Fehler auftrat.</span><span class="sxs-lookup"><span data-stu-id="018bf-2234">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="018bf-2235">[BREAKING CHANGE] Die Befehle vom Typ `az identity` wurden zu `role`-Befehlen verschoben.</span><span class="sxs-lookup"><span data-stu-id="018bf-2235">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="018bf-2236">31. Januar 2019</span><span class="sxs-lookup"><span data-stu-id="018bf-2236">January 31, 2019</span></span>

<span data-ttu-id="018bf-2237">Version 2.0.57</span><span class="sxs-lookup"><span data-stu-id="018bf-2237">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="018bf-2238">Core</span><span class="sxs-lookup"><span data-stu-id="018bf-2238">Core</span></span>

* <span data-ttu-id="018bf-2239">Hotfix für [Problem 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="018bf-2239">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="018bf-2240">28. Januar 2019</span><span class="sxs-lookup"><span data-stu-id="018bf-2240">January 28, 2019</span></span>

<span data-ttu-id="018bf-2241">Version 2.0.56</span><span class="sxs-lookup"><span data-stu-id="018bf-2241">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="018bf-2242">ACR</span><span class="sxs-lookup"><span data-stu-id="018bf-2242">ACR</span></span>
* <span data-ttu-id="018bf-2243">Unterstützung für VNet/IP-Regeln wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-2243">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="018bf-2244">ACS</span><span class="sxs-lookup"><span data-stu-id="018bf-2244">ACS</span></span>
* <span data-ttu-id="018bf-2245">Virtuelle Knoten (Vorschau) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2245">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="018bf-2246">Verwaltete OpenShift-Befehle wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-2246">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="018bf-2247">Unterstützung für den Dienstprinzipal-Updatevorgang mit `aks update-credentials -reset-service-principal` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-2247">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="018bf-2248">AMS</span><span class="sxs-lookup"><span data-stu-id="018bf-2248">AMS</span></span>
* <span data-ttu-id="018bf-2249">[BREAKING CHANGE]`ams asset get-streaming-locators` in `ams asset list-streaming-locators` umbenannt</span><span class="sxs-lookup"><span data-stu-id="018bf-2249">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="018bf-2250">[BREAKING CHANGE]`ams streaming-locator get-content-keys` in `ams streaming-locator list-content-keys` umbenannt</span><span class="sxs-lookup"><span data-stu-id="018bf-2250">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="018bf-2251">AppService</span><span class="sxs-lookup"><span data-stu-id="018bf-2251">Appservice</span></span>
* <span data-ttu-id="018bf-2252">Unterstützung für App-Erkenntnisse in `functionapp create` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-2252">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="018bf-2253">Unterstützung für die Erstellung von App Service-Plänen (einschließlich Elastic Premium) wurde zu Funktions-Apps hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-2253">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="018bf-2254">Probleme bei einer App-Einstellung mit Elastic Premium-Plänen wurden behoben.</span><span class="sxs-lookup"><span data-stu-id="018bf-2254">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="018bf-2255">Container</span><span class="sxs-lookup"><span data-stu-id="018bf-2255">Container</span></span>
* <span data-ttu-id="018bf-2256">Befehl `container start` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2256">Added `container start` command</span></span>
* <span data-ttu-id="018bf-2257">Eine Änderung wurde vorgenommen, um bei der Containererstellung die Verwendung von Dezimalwerten für die CPU zuzulassen.</span><span class="sxs-lookup"><span data-stu-id="018bf-2257">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="018bf-2258">EventGrid</span><span class="sxs-lookup"><span data-stu-id="018bf-2258">EventGrid</span></span>
* <span data-ttu-id="018bf-2259">Parameter `--deadletter-endpoint` zu `event-subscription [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2259">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="018bf-2260">„storagequeue“ und „hybridconnection“ wurden als neue Werte für „event-subscription [create|update] --endpoint-type“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-2260">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="018bf-2261">Parameter `--max-delivery-attempts` und `--event-ttl` wurden zu `event-subscription create` hinzugefügt, um die Wiederholungsrichtlinie für Ereignisse anzugeben.</span><span class="sxs-lookup"><span data-stu-id="018bf-2261">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="018bf-2262">Eine Warnmeldung wurde zu `event-subscription [create|update]` hinzugefügt, wenn Webhook als Ziel für ein Ereignisabonnement verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="018bf-2262">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="018bf-2263">Parameter „source-resource-id“ wurde für alle Befehle im Zusammenhang mit Ereignisabonnements hinzugefügt, und alle anderen Parameter im Zusammenhang mit Quellressourcen wurden als veraltet markiert.</span><span class="sxs-lookup"><span data-stu-id="018bf-2263">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="018bf-2264">HDInsight</span><span class="sxs-lookup"><span data-stu-id="018bf-2264">HDInsight</span></span>
* <span data-ttu-id="018bf-2265">[BREAKING CHANGE] Die Parameter `--virtual-network` und `--subnet-name` wurden aus `hdinsight [application] create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="018bf-2265">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="018bf-2266">[BREAKING CHANGE]`hdinsight create --storage-account` wurde so geändert, dass der Name oder die ID eines Speicherkontos anstellen von Blobendpunkten akzeptiert wird.</span><span class="sxs-lookup"><span data-stu-id="018bf-2266">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="018bf-2267">Parameter `--vnet-name` und `--subnet-name` zu `hdinsight create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2267">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="018bf-2268">Unterstützung für das Enterprise-Sicherheitspaket und Datenträgerverschlüsselung wurde zu `hdinsight create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-2268">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="018bf-2269">Befehl `hdinsight rotate-disk-encryption-key` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2269">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="018bf-2270">Befehl `hdinsight update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2270">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="018bf-2271">IoT</span><span class="sxs-lookup"><span data-stu-id="018bf-2271">IoT</span></span>
* <span data-ttu-id="018bf-2272">Codierungsformat wurde zu Befehl „routing-endpoint“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-2272">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="018bf-2273">Kusto</span><span class="sxs-lookup"><span data-stu-id="018bf-2273">Kusto</span></span>
* <span data-ttu-id="018bf-2274">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="018bf-2274">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="018bf-2275">Überwachen</span><span class="sxs-lookup"><span data-stu-id="018bf-2275">Monitor</span></span>
* <span data-ttu-id="018bf-2276">ID-Vergleich wurde so geändert, dass Groß-/Kleinschreibung nicht mehr beachtet wird.</span><span class="sxs-lookup"><span data-stu-id="018bf-2276">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="018bf-2277">Profil</span><span class="sxs-lookup"><span data-stu-id="018bf-2277">Profile</span></span>
* <span data-ttu-id="018bf-2278">Konto auf Mandantenebene für verwaltete Dienstidentität für `login` wird aktiviert.</span><span class="sxs-lookup"><span data-stu-id="018bf-2278">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="018bf-2279">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="018bf-2279">Network</span></span>
* <span data-ttu-id="018bf-2280">Ein Problem mit `express-route update` wurde behoben, aufgrund dessen das Argument `--bandwidth` ignoriert wurde.</span><span class="sxs-lookup"><span data-stu-id="018bf-2280">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="018bf-2281">Ein Problem mit `ddos-protection update` wurde behoben, aufgrund dessen das festgelegte Verständnis zu einer Stapelüberwachung führte.</span><span class="sxs-lookup"><span data-stu-id="018bf-2281">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="018bf-2282">Resource</span><span class="sxs-lookup"><span data-stu-id="018bf-2282">Resource</span></span>
* <span data-ttu-id="018bf-2283">Unterstützung für die URI-Parameterdatei wurde zu `group deployment create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-2283">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="018bf-2284">Unterstützung für verwaltete Identitäten wurde zu `policy assignment [create|list|show]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-2284">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="018bf-2285">Virtueller SQL-Computer</span><span class="sxs-lookup"><span data-stu-id="018bf-2285">SQL Virtual Machine</span></span>
* <span data-ttu-id="018bf-2286">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="018bf-2286">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="018bf-2287">Storage</span><span class="sxs-lookup"><span data-stu-id="018bf-2287">Storage</span></span>
* <span data-ttu-id="018bf-2288">Eine Lösung wurde so geändert, dass nur Eigenschaften aktualisiert werden, die im selben Objekt geändert werden.</span><span class="sxs-lookup"><span data-stu-id="018bf-2288">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="018bf-2289">Nr. 8021 wurde korrigiert, Binärdaten werden bei der Rückgabe in Base64 codiert.</span><span class="sxs-lookup"><span data-stu-id="018bf-2289">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="018bf-2290">VM</span><span class="sxs-lookup"><span data-stu-id="018bf-2290">VM</span></span>
* <span data-ttu-id="018bf-2291">`vm encryption enable` wurde geändert, um den Schlüsseltresor für die Datenträgerverschlüsselung zu überprüfen und sicherzustellen, dass der Schlüsseltresor für die Schlüsselverschlüsselung vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="018bf-2291">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="018bf-2292">Flag `--force` wurde zu `vm encryption enable` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-2292">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="018bf-2293">15. Januar 2019</span><span class="sxs-lookup"><span data-stu-id="018bf-2293">January 15, 2019</span></span>

<span data-ttu-id="018bf-2294">Version 2.0.55</span><span class="sxs-lookup"><span data-stu-id="018bf-2294">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="018bf-2295">ACR</span><span class="sxs-lookup"><span data-stu-id="018bf-2295">ACR</span></span>
* <span data-ttu-id="018bf-2296">Wurde geändert, um den Push eines nicht vorhandenen Helm-Diagramms zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="018bf-2296">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="018bf-2297">Wurde geändert, um Laufzeitvorgänge ohne ARM-Anforderungen zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="018bf-2297">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="018bf-2298">[VERALTET] Parameter `--resource-group` in folgenden Befehlen als veraltet markiert:</span><span class="sxs-lookup"><span data-stu-id="018bf-2298">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="018bf-2299">ACS</span><span class="sxs-lookup"><span data-stu-id="018bf-2299">ACS</span></span>
* <span data-ttu-id="018bf-2300">Unterstützung für neue ACI-Regionen wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-2300">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="018bf-2301">AppService</span><span class="sxs-lookup"><span data-stu-id="018bf-2301">Appservice</span></span>
* <span data-ttu-id="018bf-2302">Ein Problem beim Hochladen von Zertifikaten für in einer ASE gehostete Apps wurde behoben, aufgrund dessen die AS-RG und die App-RG nicht übereinstimmten.</span><span class="sxs-lookup"><span data-stu-id="018bf-2302">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="018bf-2303">`webapp up` wurde geändert, sodass SKU P1V1 als Standard für Linux verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="018bf-2303">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="018bf-2304">`[webapp|functionapp] deployment source config-zip` wurde korrigiert, sodass beim Fehlschlagen einer Bereitstellung die richtige Fehlermeldung angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="018bf-2304">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="018bf-2305">Befehl `webapp ssh` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2305">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="018bf-2306">Botservice</span><span class="sxs-lookup"><span data-stu-id="018bf-2306">Botservice</span></span>
* <span data-ttu-id="018bf-2307">Aktualisierungen des Bereitstellungsstatus wurden zu `bot create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-2307">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="018bf-2308">Konfigurieren</span><span class="sxs-lookup"><span data-stu-id="018bf-2308">Configure</span></span>
* <span data-ttu-id="018bf-2309">`none` wurde als konfigurierbares Ausgabeformat hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-2309">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="018bf-2310">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="018bf-2310">CosmosDB</span></span>
* <span data-ttu-id="018bf-2311">Unterstützung für das Erstellen einer Datenbank mit gemeinsam genutztem Durchsatz wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-2311">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="018bf-2312">HDInsight</span><span class="sxs-lookup"><span data-stu-id="018bf-2312">HDInsight</span></span>
* <span data-ttu-id="018bf-2313">Befehle zum Verwalten von Anwendungen wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-2313">Added commands for managing applications</span></span>
* <span data-ttu-id="018bf-2314">Befehle zum Verwalten von Skriptaktionen wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-2314">Added commands for managing script actions</span></span>
* <span data-ttu-id="018bf-2315">Befehle zum Verwalten von der Operations Management Suite (OMS) wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-2315">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="018bf-2316">Unterstützung zum Auflisten der regionalen Nutzung wurde zu `hdinsight list-usage` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-2316">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="018bf-2317">[BREAKING CHANGE] Standardclustertyp wurde aus `hdinsight create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="018bf-2317">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="018bf-2318">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="018bf-2318">Network</span></span>
* <span data-ttu-id="018bf-2319">Argumente `--custom-headers` und `--status-code-ranges` zu `traffic-manager profile [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2319">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="018bf-2320">Neue Routingtypen wurden hinzugefügt: Subnetz und MultiValue</span><span class="sxs-lookup"><span data-stu-id="018bf-2320">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="018bf-2321">Argumente `--custom-headers` und `--subnets` zu `traffic-manager endpoint [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2321">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="018bf-2322">Eine Problem wurde behoben, aufgrund dessen die Angabe von `--vnets ""` für `ddos-protection update` einen Fehler verursacht hat.</span><span class="sxs-lookup"><span data-stu-id="018bf-2322">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="018bf-2323">Role</span><span class="sxs-lookup"><span data-stu-id="018bf-2323">Role</span></span>
* <span data-ttu-id="018bf-2324">[VERALTET] Argument `--password` als veraltet markiert für `create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="018bf-2324">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="018bf-2325">Verwenden Sie stattdessen sichere, von der CLI generierte Kennwörter.</span><span class="sxs-lookup"><span data-stu-id="018bf-2325">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="018bf-2326">Sicherheit</span><span class="sxs-lookup"><span data-stu-id="018bf-2326">Security</span></span>
* <span data-ttu-id="018bf-2327">Erstrelease</span><span class="sxs-lookup"><span data-stu-id="018bf-2327">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="018bf-2328">Storage</span><span class="sxs-lookup"><span data-stu-id="018bf-2328">Storage</span></span>
* <span data-ttu-id="018bf-2329">[BREAKING CHANGE] Die Standardanzahl von Ergebnissen wurde für `storage [blob|file|container|share] list` in 5.000 geändert.</span><span class="sxs-lookup"><span data-stu-id="018bf-2329">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="018bf-2330">Verwenden Sie `--num-results *` für das ursprüngliche Verhalten, alle Ergebnisse zurückzugeben.</span><span class="sxs-lookup"><span data-stu-id="018bf-2330">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="018bf-2331">Parameter `--marker` zu `storage [blob|file|container|share] list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2331">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="018bf-2332">Ein Protokollmarker für die nächste Seite wurde zur STDERR für `storage [blob|file|container|share] list` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-2332">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="018bf-2333">Der Befehl `storage blob service-properties update` mit Unterstützung für statische Websites wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-2333">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="018bf-2334">VM</span><span class="sxs-lookup"><span data-stu-id="018bf-2334">VM</span></span>
* <span data-ttu-id="018bf-2335">`vm [disk|unmanaged-disk]` und `vmss disk` wurden geändert, sodass sie konsistentere Parameter enthalten.</span><span class="sxs-lookup"><span data-stu-id="018bf-2335">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="018bf-2336">Unterstützung für mandantenübergreifende Imageverweise wurden zu `[vm|vmss] create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-2336">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="018bf-2337">Fehler bei Standardkonfiguration in `vm diagnostics get-default-config --windows-os` wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="018bf-2337">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="018bf-2338">Argument `--provision-after-extensions` wurde zu `vmss extension set` hinzugefügt, um zu definieren, welche Erweiterungen vor dem Festlegen der Erweiterung bereitgestellt werden müssen.</span><span class="sxs-lookup"><span data-stu-id="018bf-2338">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="018bf-2339">Argument `--replica-count` wurde zu `sig image-version update` hinzugefügt, um die Standardanzahl für die Replikation festzulegen.</span><span class="sxs-lookup"><span data-stu-id="018bf-2339">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="018bf-2340">Fehler bei `image create --source` wurde behoben, aufgrund dessen, der Quellbetriebssystem-Datenträger für einen virtuellen Computer mit dem gleichen Namen gehalten wurde, selbst wenn die vollständige Ressourcen-ID angegeben war.</span><span class="sxs-lookup"><span data-stu-id="018bf-2340">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="018bf-2341">20. Dezember 2018</span><span class="sxs-lookup"><span data-stu-id="018bf-2341">December 20, 2018</span></span>

<span data-ttu-id="018bf-2342">Version 2.0.54</span><span class="sxs-lookup"><span data-stu-id="018bf-2342">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="018bf-2343">AppService</span><span class="sxs-lookup"><span data-stu-id="018bf-2343">Appservice</span></span>
* <span data-ttu-id="018bf-2344">Problem behoben, bei dem `webapp up` nicht erneut bereitgestellt werden konnte</span><span class="sxs-lookup"><span data-stu-id="018bf-2344">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="018bf-2345">Unterstützung für das Auflisten und Wiederherstellen von Web-App-Momentaufnahmen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2345">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="018bf-2346">Unterstützung für das Flag `--runtime` zu Windows-Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2346">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="018bf-2347">IoTCentral</span><span class="sxs-lookup"><span data-stu-id="018bf-2347">IoTCentral</span></span>
* <span data-ttu-id="018bf-2348">Fehler bei API-Aufruf für update-Befehl behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-2348">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="018bf-2349">Role</span><span class="sxs-lookup"><span data-stu-id="018bf-2349">Role</span></span>
* <span data-ttu-id="018bf-2350">[BREAKING CHANGE]`ad [app|sp] list` geändert, damit standardmäßig nur die ersten 100 Objekte aufgelistet werden</span><span class="sxs-lookup"><span data-stu-id="018bf-2350">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="018bf-2351">SQL</span><span class="sxs-lookup"><span data-stu-id="018bf-2351">SQL</span></span>
* <span data-ttu-id="018bf-2352">Unterstützung für die benutzerdefinierte Sortierung auf verwalteten Instanzen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2352">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="018bf-2353">VM</span><span class="sxs-lookup"><span data-stu-id="018bf-2353">VM</span></span>
* <span data-ttu-id="018bf-2354">Parameter `---os-type` zu `disk create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2354">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="018bf-2355">18. Dezember 2018</span><span class="sxs-lookup"><span data-stu-id="018bf-2355">December 18, 2018</span></span>

<span data-ttu-id="018bf-2356">Version 2.0.53</span><span class="sxs-lookup"><span data-stu-id="018bf-2356">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="018bf-2357">ACR</span><span class="sxs-lookup"><span data-stu-id="018bf-2357">ACR</span></span>
* <span data-ttu-id="018bf-2358">Unterstützung für Imageimport aus externen Containerregistrierungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2358">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="018bf-2359">Tabellenlayout für Aufgabenliste komprimiert</span><span class="sxs-lookup"><span data-stu-id="018bf-2359">Condensed the table layout for task list</span></span>
* <span data-ttu-id="018bf-2360">Unterstützung für Azure DevOps-URLs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2360">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="018bf-2361">ACS</span><span class="sxs-lookup"><span data-stu-id="018bf-2361">ACS</span></span>
* <span data-ttu-id="018bf-2362">Virtuelle Knoten (Vorschau) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2362">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="018bf-2363">„(PREVIEW)“ aus AAD-Argumenten für `aks create` entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-2363">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="018bf-2364">[VERALTET]`az acs`-Befehle als veraltet markiert.</span><span class="sxs-lookup"><span data-stu-id="018bf-2364">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="018bf-2365">ACS wird am 31. Januar 2020 eingestellt</span><span class="sxs-lookup"><span data-stu-id="018bf-2365">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="018bf-2366">Unterstützung für Netzwerkrichtlinie bei der Erstellung neuer AKS-Cluster hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2366">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="018bf-2367">Anforderung des Arguments `--nodepool-name` bei nur einem Knotenpool für `aks scale` entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-2367">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="018bf-2368">AppService</span><span class="sxs-lookup"><span data-stu-id="018bf-2368">Appservice</span></span>
* <span data-ttu-id="018bf-2369">Problem behoben, bei dem für `webapp config container` der Parameter `--slot` nicht berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="018bf-2369">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="018bf-2370">Botservice</span><span class="sxs-lookup"><span data-stu-id="018bf-2370">Botservice</span></span>
* <span data-ttu-id="018bf-2371">Unterstützung für Analyse von `.bot`-Dateien beim Aufrufen von `bot show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2371">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="018bf-2372">Fehler bei der AppInsights-Bereitstellung behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-2372">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="018bf-2373">Leerzeichenfehler bei Dateipfaden behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-2373">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="018bf-2374">Kudu-Netzwerkaufrufe reduziert</span><span class="sxs-lookup"><span data-stu-id="018bf-2374">Reduced Kudu network calls</span></span>
* <span data-ttu-id="018bf-2375">Allgemeine Verbesserungen bei Befehlen der Benutzeroberfläche durchgeführt</span><span class="sxs-lookup"><span data-stu-id="018bf-2375">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="018bf-2376">Nutzung</span><span class="sxs-lookup"><span data-stu-id="018bf-2376">Consumption</span></span>
* <span data-ttu-id="018bf-2377">Fehler für Budget-API zum Anzeigen von Benachrichtigungen behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-2377">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="018bf-2378">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="018bf-2378">CosmosDB</span></span>
* <span data-ttu-id="018bf-2379">Unterstützung für die Aktualisierung des Kontos von „Singlemaster“ auf „Multimaster“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2379">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="018bf-2380">Karten</span><span class="sxs-lookup"><span data-stu-id="018bf-2380">Maps</span></span>
* <span data-ttu-id="018bf-2381">Unterstützung für SKU „S1“ für `maps account [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2381">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="018bf-2382">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="018bf-2382">Network</span></span>
* <span data-ttu-id="018bf-2383">Unterstützung für `--format` und `--log-version` für `watcher flow-log configure` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2383">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="018bf-2384">Problem mit `dns zone update` behoben, bei dem die Verwendung von "" zum Löschen von Auflösungs- und Registrierungs-VNETs nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="018bf-2384">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="018bf-2385">Resource</span><span class="sxs-lookup"><span data-stu-id="018bf-2385">Resource</span></span>
* <span data-ttu-id="018bf-2386">Verarbeitung des Bereichsparameters für Verwaltungsgruppen in `policy assignment [create|list|delete|show|update]` behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-2386">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="018bf-2387">Neuen Befehl `resource wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2387">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="018bf-2388">Storage</span><span class="sxs-lookup"><span data-stu-id="018bf-2388">Storage</span></span>
*  <span data-ttu-id="018bf-2389">Möglichkeit zum Aktualisieren der Protokollschemaversion für Speicherdienste in `storage logging update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2389">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="018bf-2390">VM</span><span class="sxs-lookup"><span data-stu-id="018bf-2390">VM</span></span>
* <span data-ttu-id="018bf-2391">Absturz in `vm identity remove` behoben, der aufgetreten ist, wenn der angegebenen VM keine verwalteten Dienstidentitäten zugewiesen waren</span><span class="sxs-lookup"><span data-stu-id="018bf-2391">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="018bf-2392">4\. Dezember 2018</span><span class="sxs-lookup"><span data-stu-id="018bf-2392">December 4, 2018</span></span>

<span data-ttu-id="018bf-2393">Version 2.0.52</span><span class="sxs-lookup"><span data-stu-id="018bf-2393">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="018bf-2394">Core</span><span class="sxs-lookup"><span data-stu-id="018bf-2394">Core</span></span>
* <span data-ttu-id="018bf-2395">Unterstützung für mandantenübergreifende Ressourcenbereitstellung für mehrinstanzenfähigen Dienstprinzipal hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2395">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="018bf-2396">Behebung eines Fehlers, aufgrund dessen IDs, die von einem Befehl mit Ausgabe im TSV-Format weitergeleitet wurden, nicht ordnungsgemäß analysiert wurden</span><span class="sxs-lookup"><span data-stu-id="018bf-2396">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="018bf-2397">AppService</span><span class="sxs-lookup"><span data-stu-id="018bf-2397">Appservice</span></span>
* <span data-ttu-id="018bf-2398">[VORSCHAU] Befehl `webapp up` hinzugefügt, der Benutzer beim Erstellen und Bereitstellen von Inhalten in Apps unterstützt</span><span class="sxs-lookup"><span data-stu-id="018bf-2398">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="018bf-2399">Behebung eines Fehlers in einer containerbasierten Windows-App, der aufgrund einer Back-End-Änderung auftrat</span><span class="sxs-lookup"><span data-stu-id="018bf-2399">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="018bf-2400">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="018bf-2400">Network</span></span>
* <span data-ttu-id="018bf-2401">Argument `--exclusion` zu `application-gateway waf-config set` hinzugefügt, um WAF-Ausschlüsse zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="018bf-2401">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="018bf-2402">Role</span><span class="sxs-lookup"><span data-stu-id="018bf-2402">Role</span></span>
* <span data-ttu-id="018bf-2403">Unterstützung für benutzerdefinierte Bezeichner für Kennwortanmeldeinformation hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2403">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="018bf-2404">VM</span><span class="sxs-lookup"><span data-stu-id="018bf-2404">VM</span></span>
* <span data-ttu-id="018bf-2405">[VERALTET] Parameter `vm extension [show|wait] --expand` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="018bf-2405">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="018bf-2406">Parameter `--force` zu `vm restart` hinzugefügt, um nicht reagierende virtuelle Computer erneut bereitzustellen</span><span class="sxs-lookup"><span data-stu-id="018bf-2406">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="018bf-2407">`[vm|vmss] create --authentication-type` geändert, um „all“ zu akzeptieren und einen virtuellen Computer mit Kennwort- und SSH-Authentifizierung zu erstellen</span><span class="sxs-lookup"><span data-stu-id="018bf-2407">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="018bf-2408">Parameter `image create --os-disk-caching` hinzugefügt, um die Zwischenspeicherung von Betriebssystemdatenträgern für ein Image festzulegen</span><span class="sxs-lookup"><span data-stu-id="018bf-2408">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="018bf-2409">20. November 2018</span><span class="sxs-lookup"><span data-stu-id="018bf-2409">November 20, 2018</span></span>

<span data-ttu-id="018bf-2410">Version 2.0.51</span><span class="sxs-lookup"><span data-stu-id="018bf-2410">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="018bf-2411">Core</span><span class="sxs-lookup"><span data-stu-id="018bf-2411">Core</span></span>
* <span data-ttu-id="018bf-2412">MSI-Anmeldung geändert, sodass der Abonnementname nicht in der Identität wiederverwendet wird</span><span class="sxs-lookup"><span data-stu-id="018bf-2412">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="018bf-2413">ACR</span><span class="sxs-lookup"><span data-stu-id="018bf-2413">ACR</span></span>
* <span data-ttu-id="018bf-2414">Kontexttoken zum Aufgabenschritt hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2414">Added context token to task step</span></span>
* <span data-ttu-id="018bf-2415">Unterstützung für das Festlegen von Geheimnissen in „acr run“ zum Spiegeln der ACR-Aufgabe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2415">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="018bf-2416">Unterstützung für `--top` und `--orderby` für die Befehle `show-tags` und `show-manifests` verbessert</span><span class="sxs-lookup"><span data-stu-id="018bf-2416">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="018bf-2417">AppService</span><span class="sxs-lookup"><span data-stu-id="018bf-2417">Appservice</span></span>
* <span data-ttu-id="018bf-2418">Standardtimeout der ZIP-Bereitstellung für das Abrufen des Status auf fünf Minuten erhöht und Timeout-Eigenschaft zum Anpassen dieses Werts hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2418">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="018bf-2419">Aktualisierung der standardmäßigen `node_version`.</span><span class="sxs-lookup"><span data-stu-id="018bf-2419">Updated the default `node_version`.</span></span> <span data-ttu-id="018bf-2420">Während eines Austauschvorgangs mit zwei Phasen werden bei der Austauschaktion zum Zurücksetzen des Slots alle App-Einstellungen und Verbindungszeichenfolgen beibehalten.</span><span class="sxs-lookup"><span data-stu-id="018bf-2420">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="018bf-2421">Clientseitige SKU-Überprüfung für die Erstellung eines Linux-App Service-Plans entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-2421">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="018bf-2422">Behebung eines Fehlers beim Abrufen des ZipDeploy-Status</span><span class="sxs-lookup"><span data-stu-id="018bf-2422">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="018bf-2423">IotCentral</span><span class="sxs-lookup"><span data-stu-id="018bf-2423">IotCentral</span></span>
* <span data-ttu-id="018bf-2424">Verfügbarkeitsprüfung für Unterdomänen beim Erstellen einer IoT Central-Anwendung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2424">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="018bf-2425">KeyVault</span><span class="sxs-lookup"><span data-stu-id="018bf-2425">KeyVault</span></span>
* <span data-ttu-id="018bf-2426">Behebung eines Fehlers, aufgrund dessen Fehler mitunter ignoriert wurden</span><span class="sxs-lookup"><span data-stu-id="018bf-2426">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="018bf-2427">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="018bf-2427">Network</span></span>
* <span data-ttu-id="018bf-2428">`root-cert`-Unterbefehle zum Behandeln von vertrauenswürdigen Stammzertifikaten zu `application-gateway` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2428">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="018bf-2429">Optionen `--min-capacity` und `--custom-error-pages` zu `application-gateway [create|update]` hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="018bf-2429">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="018bf-2430">`--zones` zur Unterstützung von Verfügbarkeitszonen zu `application-gateway create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2430">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="018bf-2431">Argumente `--file-upload-limit`, `--max-request-body-size` und `--request-body-check` zu `application-gateway waf-config set` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2431">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="018bf-2432">Rdbms</span><span class="sxs-lookup"><span data-stu-id="018bf-2432">Rdbms</span></span>
* <span data-ttu-id="018bf-2433">MariaDB-VNET-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2433">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="018bf-2434">RBAC</span><span class="sxs-lookup"><span data-stu-id="018bf-2434">Rbac</span></span>
* <span data-ttu-id="018bf-2435">Problem beim Aktualisieren unveränderlicher Anmeldeinformationen in `ad app update` behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-2435">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="018bf-2436">Ausgabewarnungen zur Ankündigung bevorstehender Breaking Changes für `ad [app|sp] list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2436">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="018bf-2437">Storage</span><span class="sxs-lookup"><span data-stu-id="018bf-2437">Storage</span></span>
* <span data-ttu-id="018bf-2438">Behandlung von Ausnahmefällen für Speicherkopierbefehle verbessert</span><span class="sxs-lookup"><span data-stu-id="018bf-2438">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="018bf-2439">Problem behoben, aufgrund dessen `storage blob copy start-batch` bei identischen Ziel- und Quellkonten keine Anmeldeinformationen verwendete</span><span class="sxs-lookup"><span data-stu-id="018bf-2439">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="018bf-2440">Fehler bei `storage [blob|file] url` behoben, aufgrund dessen `sas_token` nicht in die URL eingebunden wurde</span><span class="sxs-lookup"><span data-stu-id="018bf-2440">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="018bf-2441">Breaking Change-Warnung zu `[blob|container] list` hinzugefügt: In Kürze werden standardmäßig nur die ersten 5.000 Ergebnisse ausgegeben.</span><span class="sxs-lookup"><span data-stu-id="018bf-2441">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="018bf-2442">VM</span><span class="sxs-lookup"><span data-stu-id="018bf-2442">VM</span></span>
* <span data-ttu-id="018bf-2443">Unterstützung für die separate Angabe einer Speicherkonto-SKU für verwaltete Betriebssystemdatenträger und Datenträger zu `[vm|vmss] create --storage-sku` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2443">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="018bf-2444">Parameter für den Versionsnamen von `sig image-version` in `--image-version -e` geändert</span><span class="sxs-lookup"><span data-stu-id="018bf-2444">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="018bf-2445">`sig image-version`-Argument `--image-version-name` als veraltet markiert und durch `--image-version` ersetzt</span><span class="sxs-lookup"><span data-stu-id="018bf-2445">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="018bf-2446">Unterstützung für die Verwendung des lokalen Betriebssystemdatenträgers für `[vm|vmss] create --ephemeral-os-disk` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2446">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="018bf-2447">Unterstützung für `--no-wait` zu `snapshot create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2447">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="018bf-2448">Befehl `snapshot wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2448">Added `snapshot wait` command</span></span>
* <span data-ttu-id="018bf-2449">Unterstützung für die Verwendung von Instanznamen mit `[vm|vmss] extension set --extension-instance-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2449">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="018bf-2450">6\. November 2018</span><span class="sxs-lookup"><span data-stu-id="018bf-2450">November 6, 2018</span></span>

<span data-ttu-id="018bf-2451">Version 2.0.50</span><span class="sxs-lookup"><span data-stu-id="018bf-2451">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="018bf-2452">Core</span><span class="sxs-lookup"><span data-stu-id="018bf-2452">Core</span></span>
* <span data-ttu-id="018bf-2453">Unterstützung für die Dienstprinzipalauthentifizierung (SN und Aussteller) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2453">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="018bf-2454">ACR</span><span class="sxs-lookup"><span data-stu-id="018bf-2454">ACR</span></span>
* <span data-ttu-id="018bf-2455">Unterstützung für Commit- und Pull Request-Git-Ereignisse für Aufgabenquellentrigger hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2455">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="018bf-2456">Auf Verwendung des Standard-Dockerfiles umgestellt, falls im Erstellungsbefehl kein Dockerfile angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="018bf-2456">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="018bf-2457">ACS</span><span class="sxs-lookup"><span data-stu-id="018bf-2457">ACS</span></span>
* <span data-ttu-id="018bf-2458">[BREAKING CHANGE]`enable_cloud_console_aks_browse` entfernt, um standardmäßig „az aks browse“ zu aktivieren</span><span class="sxs-lookup"><span data-stu-id="018bf-2458">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="018bf-2459">Advisor</span><span class="sxs-lookup"><span data-stu-id="018bf-2459">Advisor</span></span>
* <span data-ttu-id="018bf-2460">Allgemein verfügbares Release</span><span class="sxs-lookup"><span data-stu-id="018bf-2460">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="018bf-2461">AMS</span><span class="sxs-lookup"><span data-stu-id="018bf-2461">AMS</span></span>
* <span data-ttu-id="018bf-2462">Neue Befehlsgruppen hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="018bf-2462">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="018bf-2463">Neue Befehle hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="018bf-2463">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="018bf-2464">Unterstützung von Verschlüsselungsparametern für `ams streaming-policy create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2464">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="018bf-2465">Für `ams transform output remove` kann jetzt der zu entfernende Ausgabeindex angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="018bf-2465">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="018bf-2466">Argumente `--correlation-data` und `--label` zur Befehlsgruppe `ams job` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2466">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="018bf-2467">Argumente `--storage-account` und `--container` zur Befehlsgruppe `ams asset` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2467">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="018bf-2468">Standardwerte für Ablaufzeit (aktueller Zeitpunkt + 23 Std.) und Berechtigungen (Lesen) im Befehl `ams asset get-sas-url` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2468">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="018bf-2469">[BREAKING CHANGE] Befehl `ams streaming locator` durch `ams streaming-locator` ersetzt</span><span class="sxs-lookup"><span data-stu-id="018bf-2469">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="018bf-2470">[BREAKING CHANGE] Argument `--content-keys` von `ams streaming locator` aktualisiert</span><span class="sxs-lookup"><span data-stu-id="018bf-2470">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="018bf-2471">[BREAKING CHANGE]`--content-policy-name` im Befehl `ams streaming locator` in `--content-key-policy-name` umbenannt</span><span class="sxs-lookup"><span data-stu-id="018bf-2471">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="018bf-2472">[BREAKING CHANGE] Befehl `ams streaming policy` durch `ams streaming-policy` ersetzt</span><span class="sxs-lookup"><span data-stu-id="018bf-2472">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="018bf-2473">[BREAKING CHANGE] Das Argument `--preset-names` wurde in der Befehlsgruppe `--preset` durch `ams transform` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="018bf-2473">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="018bf-2474">Ab sofort kann nur noch eine einzelne Ausgabe/Voreinstellung festgelegt werden. (Wenn Sie weitere hinzufügen möchten, müssen Sie `ams transform output add` ausführen.)</span><span class="sxs-lookup"><span data-stu-id="018bf-2474">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="018bf-2475">Darüber hinaus können Sie eine benutzerdefinierte Voreinstellung für den Standard-Encoder (StandardEncoderPreset) festlegen, indem Sie den Pfad an Ihr benutzerdefiniertes JSON-Objekt übergeben.</span><span class="sxs-lookup"><span data-stu-id="018bf-2475">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="018bf-2476">[BREAKING CHANGE]`--output-asset-names ` wurde im Befehl `ams job start` in `--output-assets` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="018bf-2476">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="018bf-2477">Ab sofort wird eine durch Leerzeichen getrennte Ressourcenliste im Format „assetName=Bezeichnung“ akzeptiert.</span><span class="sxs-lookup"><span data-stu-id="018bf-2477">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="018bf-2478">Ressourcen ohne Bezeichnung können wie folgt gesendet werden: „assetName=“.</span><span class="sxs-lookup"><span data-stu-id="018bf-2478">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="018bf-2479">AppService</span><span class="sxs-lookup"><span data-stu-id="018bf-2479">AppService</span></span>
* <span data-ttu-id="018bf-2480">Fehler in `az webapp config backup update` behoben, der dazu führte, dass kein Sicherungszeitplan festgelegt werden konnte, wenn noch keiner festgelegt war</span><span class="sxs-lookup"><span data-stu-id="018bf-2480">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="018bf-2481">Konfigurieren</span><span class="sxs-lookup"><span data-stu-id="018bf-2481">Configure</span></span>
* <span data-ttu-id="018bf-2482">YAML zu Ausgabeformatoptionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2482">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="018bf-2483">Container</span><span class="sxs-lookup"><span data-stu-id="018bf-2483">Container</span></span>
* <span data-ttu-id="018bf-2484">Auf Anzeige der Identität umgestellt, wenn eine Containergruppe nach YAML exportiert wird</span><span class="sxs-lookup"><span data-stu-id="018bf-2484">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="018bf-2485">EventHub</span><span class="sxs-lookup"><span data-stu-id="018bf-2485">EventHub</span></span>
* <span data-ttu-id="018bf-2486">Flag `--enable-kafka` hinzugefügt, um Kafka in `eventhub namespace [create|update]` zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="018bf-2486">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="018bf-2487">Interactive</span><span class="sxs-lookup"><span data-stu-id="018bf-2487">Interactive</span></span>
* <span data-ttu-id="018bf-2488">Interactive installiert nun die Erweiterung `interactive`, um schnellere Updates und schnelleren Support zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="018bf-2488">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="018bf-2489">Überwachen</span><span class="sxs-lookup"><span data-stu-id="018bf-2489">Monitor</span></span>
* <span data-ttu-id="018bf-2490">Unterstützung für Metriknamen mit Schrägstrichen und Punkten zu `--condition` in `monitor metrics alert [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2490">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="018bf-2491">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="018bf-2491">Network</span></span>
* <span data-ttu-id="018bf-2492">Befehlsnamen vom Typ `network interface-endpoint` zugunsten von `network private-endpoint` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="018bf-2492">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="018bf-2493">Problem behoben, das dazu führte, dass das Argument `--peer-circuit` in `express-route peering connection create` keine ID akzeptiert</span><span class="sxs-lookup"><span data-stu-id="018bf-2493">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="018bf-2494">Problem behoben, das dazu führte, dass `--ip-tags` mit `public-ip create` nicht ordnungsgemäß funktioniert</span><span class="sxs-lookup"><span data-stu-id="018bf-2494">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="018bf-2495">Profil</span><span class="sxs-lookup"><span data-stu-id="018bf-2495">Profile</span></span>
* <span data-ttu-id="018bf-2496">`--use-cert-sn-issuer` zu `az login` hinzugefügt, um Dienstprinzipalanmeldungen mit automatischem Zertifikatrollover zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="018bf-2496">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="018bf-2497">RDBMS</span><span class="sxs-lookup"><span data-stu-id="018bf-2497">RDBMS</span></span>
* <span data-ttu-id="018bf-2498">MySQL-Replikatbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2498">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="018bf-2499">Resource</span><span class="sxs-lookup"><span data-stu-id="018bf-2499">Resource</span></span>
* <span data-ttu-id="018bf-2500">Unterstützung für Verwaltungsgruppen und Abonnements zu Befehlen vom Typ `policy definition|set-definition` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2500">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="018bf-2501">Role</span><span class="sxs-lookup"><span data-stu-id="018bf-2501">Role</span></span>
* <span data-ttu-id="018bf-2502">Unterstützung für die API-Berechtigungsverwaltung, den angemeldeten Benutzer und die Verwaltung von Anwendungskennwörtern und Zertifikatanmeldeinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2502">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="018bf-2503">`ad sp create-for-rbac` geändert, um „displayName“ und Dienstprinzipalname besser unterscheiden zu können</span><span class="sxs-lookup"><span data-stu-id="018bf-2503">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="018bf-2504">Unterstützung der Gewährung von Berechtigungen für AAD-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2504">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="018bf-2505">Storage</span><span class="sxs-lookup"><span data-stu-id="018bf-2505">Storage</span></span>
* <span data-ttu-id="018bf-2506">Möglichkeit hinzugefügt, allein mit SAS und Endpunkten (ohne Kontoname oder Schlüssel) eine Verbindung mit Speicherdiensten herzustellen, wie unter `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>` beschrieben</span><span class="sxs-lookup"><span data-stu-id="018bf-2506">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="018bf-2507">VM</span><span class="sxs-lookup"><span data-stu-id="018bf-2507">VM</span></span>
* <span data-ttu-id="018bf-2508">Argument `storage-sku` zu `image create` hinzugefügt, um das Festlegen des standardmäßigen Speicherkontotyps für das Image zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="018bf-2508">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="018bf-2509">Fehler für `vm resize` behoben, durch den die Option `--no-wait` einen Absturz des Befehls verursachte</span><span class="sxs-lookup"><span data-stu-id="018bf-2509">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="018bf-2510">Tabellenausgabeformat für `vm encryption show` geändert, um den Status anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="018bf-2510">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="018bf-2511">`vm secret format` geändert, um JSON/JSONC-Ausgabe erforderlich zu machen.</span><span class="sxs-lookup"><span data-stu-id="018bf-2511">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="018bf-2512">Der Benutzer wird gewarnt, und es wird standardmäßig die JSON-Ausgabe verwendet, wenn ein unzulässiges Ausgabeformat ausgewählt wird.</span><span class="sxs-lookup"><span data-stu-id="018bf-2512">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="018bf-2513">Argumentüberprüfung für `vm create --image` verbessert</span><span class="sxs-lookup"><span data-stu-id="018bf-2513">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="018bf-2514">23. Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="018bf-2514">October 23, 2018</span></span>

<span data-ttu-id="018bf-2515">Version 2.0.49</span><span class="sxs-lookup"><span data-stu-id="018bf-2515">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="018bf-2516">Core</span><span class="sxs-lookup"><span data-stu-id="018bf-2516">Core</span></span>
* <span data-ttu-id="018bf-2517">Problem mit `--ids` behoben, aufgrund dessen `--subscription` Vorrang vor dem Abonnement in `--ids` hatte</span><span class="sxs-lookup"><span data-stu-id="018bf-2517">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="018bf-2518">Ausdrückliche Warnungen hinzugefügt, wenn Parameter durch die Verwendung von `--ids` ignoriert würden</span><span class="sxs-lookup"><span data-stu-id="018bf-2518">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="018bf-2519">ACR</span><span class="sxs-lookup"><span data-stu-id="018bf-2519">ACR</span></span>
* <span data-ttu-id="018bf-2520">Problem mit der ACR Build-Codierung in Python2 behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-2520">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="018bf-2521">CDN</span><span class="sxs-lookup"><span data-stu-id="018bf-2521">CDN</span></span>
* <span data-ttu-id="018bf-2522">[BREAKING CHANGE] Standardverhalten beim Zwischenspeichern der Abfragezeichenfolge von `cdn endpoint create` so geändert, dass der Standardwert nicht mehr „IgnoreQueryString“ ist.</span><span class="sxs-lookup"><span data-stu-id="018bf-2522">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="018bf-2523">Er wird jetzt vom Dienst festgelegt.</span><span class="sxs-lookup"><span data-stu-id="018bf-2523">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="018bf-2524">Container</span><span class="sxs-lookup"><span data-stu-id="018bf-2524">Container</span></span>
* <span data-ttu-id="018bf-2525">`Private` als gültiger Typ für die Übergabe an „--ip-address“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2525">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="018bf-2526">Geändert, sodass nur eine Subnetz-ID für das Einrichten eines virtuellen Netzwerks für die Containergruppe zulässig ist</span><span class="sxs-lookup"><span data-stu-id="018bf-2526">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="018bf-2527">Geändert, sodass das Verwenden eines VNET-Namens oder einer Ressourcen-ID zulässig ist, um die Verwendung von VNETs aus verschiedenen Ressourcengruppen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="018bf-2527">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="018bf-2528">`--assign-identity` hinzugefügt, um einer Containergruppe eine MSI-Identität hinzuzufügen</span><span class="sxs-lookup"><span data-stu-id="018bf-2528">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="018bf-2529">`--scope` hinzugefügt, um eine Rollenzuweisung für die vom System zugewiesene MSI-Identität zu erstellen</span><span class="sxs-lookup"><span data-stu-id="018bf-2529">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="018bf-2530">Warnung hinzugefügt, wenn eine Containergruppe mit einem Image ohne Prozess mit langer Ausführungszeit erstellt wird</span><span class="sxs-lookup"><span data-stu-id="018bf-2530">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="018bf-2531">Probleme mit der Tabellenausgabe für Befehle `list` und `show` behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-2531">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="018bf-2532">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="018bf-2532">CosmosDB</span></span>
* <span data-ttu-id="018bf-2533">Unterstützung für `--enable-multiple-write-locations` zu `cosmosdb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2533">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="018bf-2534">Interactive</span><span class="sxs-lookup"><span data-stu-id="018bf-2534">Interactive</span></span>
* <span data-ttu-id="018bf-2535">Geändert, um sicherzustellen, dass der Parameter für globales Abonnement in Parametern angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="018bf-2535">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="018bf-2536">IoT Central</span><span class="sxs-lookup"><span data-stu-id="018bf-2536">IoT Central</span></span>
* <span data-ttu-id="018bf-2537">Optionen für Vorlagen und Anzeigenamen für die Erstellung von IoT Central-Anwendungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2537">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="018bf-2538">[BREAKING CHANGE] Unterstützung für F1-SKU entfernt; stattdessen ist die S1-SKU zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="018bf-2538">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="018bf-2539">Überwachen</span><span class="sxs-lookup"><span data-stu-id="018bf-2539">Monitor</span></span>
* <span data-ttu-id="018bf-2540">Änderungen an `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="018bf-2540">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="018bf-2541">Unterstützung für das Auflisten aller Ereignisse auf Abonnementebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2541">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="018bf-2542">`--offset`-Parameter für das einfachere Erstellen von Zeitabfragen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2542">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="018bf-2543">Validierung für `--start-time` und `--end-time` verbessert, um die Verwendung von mehr ISO8601-Formate und benutzerfreundlicheren datetime-Formaten zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="018bf-2543">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="018bf-2544">`--namespace` als Alias für veraltete Option `--resource-provider` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2544">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="018bf-2545">`--filters` als veraltet markiert, da vom Dienst ausschließlich Werte mit stark typisierten Optionen unterstützt werden</span><span class="sxs-lookup"><span data-stu-id="018bf-2545">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="018bf-2546">Änderungen an `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="018bf-2546">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="018bf-2547">`--offset`-Parameter für das einfachere Erstellen von Zeitabfragen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2547">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="018bf-2548">Validierung für `--start-time` und `--end-time` verbessert, um die Verwendung von mehr ISO8601-Formate und benutzerfreundlicheren datetime-Formaten zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="018bf-2548">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="018bf-2549">Validierung für `--event-hub`- und `--event-hub-rule`-Argumente an `monitor diagnostic-settings create` verbessert</span><span class="sxs-lookup"><span data-stu-id="018bf-2549">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="018bf-2550">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="018bf-2550">Network</span></span>
* <span data-ttu-id="018bf-2551">`--app-gateway-address-pools`- und `--gateway-name`-Argumente zu `nic create` hinzugefügt, um das Hinzufügen von Back-End-Adresspools für Anwendungsgateways zu einer NIC zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="018bf-2551">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="018bf-2552">`--app-gateway-address-pools`- und `--gateway-name`-Argumente zu `nic ip-config create/update` hinzugefügt, um das Hinzufügen von Back-End-Adresspools für Anwendungsgateways zu einer NIC zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="018bf-2552">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="018bf-2553">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="018bf-2553">ServiceBus</span></span>
* <span data-ttu-id="018bf-2554">Schreibgeschütztes `migration_state`-Element zu „MigrationConfigProperties“ hinzugefügt, um den aktuellen Status der Migration von Service Bus Standard- zu Premium-Namespace anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="018bf-2554">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="018bf-2555">SQL</span><span class="sxs-lookup"><span data-stu-id="018bf-2555">SQL</span></span>
* <span data-ttu-id="018bf-2556">`sql failover-group create` und `sql failover-group update` korrigiert, damit die Verwendung einer Richtlinie für manuelles Failover möglich ist</span><span class="sxs-lookup"><span data-stu-id="018bf-2556">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="018bf-2557">Storage</span><span class="sxs-lookup"><span data-stu-id="018bf-2557">Storage</span></span>
* <span data-ttu-id="018bf-2558">Formatierung der `az storage cors list`-Ausgabe korrigiert, sodass alle Elemente den richtigen Dienstschlüssel anzeigen</span><span class="sxs-lookup"><span data-stu-id="018bf-2558">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="018bf-2559">`--bypass-immutability-policy`-Parameter für das Löschen von durch Unveränderlichkeitsrichtlinien blockierten Containern hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2559">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="018bf-2560">VM</span><span class="sxs-lookup"><span data-stu-id="018bf-2560">VM</span></span>
* <span data-ttu-id="018bf-2561">Datenträger-Zwischenspeicherungsmodus `None` für Lv/Lv2-Computerserine in `[vm|vmss] create` erzwungen</span><span class="sxs-lookup"><span data-stu-id="018bf-2561">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="018bf-2562">Liste der unterstützten Größen für unterstützenden Netzwerkbeschleuniger für `vm create` aktualisiert</span><span class="sxs-lookup"><span data-stu-id="018bf-2562">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="018bf-2563">Stark typisierte Argumente für UltraSSD-IOPS und MBit/s-Konfigurationen für `disk create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2563">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="018bf-2564">16. Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="018bf-2564">October 16, 2018</span></span>

<span data-ttu-id="018bf-2565">Version 2.0.48</span><span class="sxs-lookup"><span data-stu-id="018bf-2565">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="018bf-2566">VM</span><span class="sxs-lookup"><span data-stu-id="018bf-2566">VM</span></span>
* <span data-ttu-id="018bf-2567">SDK-Problem behoben, das ein Fehlschlagen der Homebrew-Installation verursacht hat</span><span class="sxs-lookup"><span data-stu-id="018bf-2567">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="018bf-2568">9\. Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="018bf-2568">October 9, 2018</span></span>

<span data-ttu-id="018bf-2569">Version 2.0.47</span><span class="sxs-lookup"><span data-stu-id="018bf-2569">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="018bf-2570">Core</span><span class="sxs-lookup"><span data-stu-id="018bf-2570">Core</span></span>
* <span data-ttu-id="018bf-2571">Verbesserte Fehlerbehandlung für Fehler vom Typ „Ungültige Anforderung“</span><span class="sxs-lookup"><span data-stu-id="018bf-2571">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="018bf-2572">ACR</span><span class="sxs-lookup"><span data-stu-id="018bf-2572">ACR</span></span>
* <span data-ttu-id="018bf-2573">Unterstützung für ähnliches Tabellenformat wie Helm-Client hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2573">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="018bf-2574">ACS</span><span class="sxs-lookup"><span data-stu-id="018bf-2574">ACS</span></span>
* <span data-ttu-id="018bf-2575">`aks [create|scale] --nodepool-name` zum Konfigurieren des Knotenpoolnamens hinzugefügt, auf 12 Zeichen gekürzt, Standard: nodepool1</span><span class="sxs-lookup"><span data-stu-id="018bf-2575">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="018bf-2576">Korrektur, bei der auf „scp“ zurückgegriffen wird, wenn Parimiko nicht funktioniert</span><span class="sxs-lookup"><span data-stu-id="018bf-2576">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="018bf-2577">`aks create` geändert, sodass `--aad-tenant-id` nicht mehr erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="018bf-2577">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="018bf-2578">Verbesserte Zusammenführung von Kubernetes-Anmeldeinformationen, wenn doppelte Einträge vorhanden sind</span><span class="sxs-lookup"><span data-stu-id="018bf-2578">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="018bf-2579">Container</span><span class="sxs-lookup"><span data-stu-id="018bf-2579">Container</span></span>
* <span data-ttu-id="018bf-2580">`functionapp create` geändert, sodass das Erstellen eines Linux-Nutzungsplans mit einer bestimmten Runtime unterstützt wird</span><span class="sxs-lookup"><span data-stu-id="018bf-2580">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="018bf-2581">[VORSCHAUVERSION] Unterstützung für das Hosten von Web-Apps in Windows-Containern hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2581">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="018bf-2582">Event Hub</span><span class="sxs-lookup"><span data-stu-id="018bf-2582">Event Hub</span></span>
* <span data-ttu-id="018bf-2583">Befehl `eventhub update` korrigiert</span><span class="sxs-lookup"><span data-stu-id="018bf-2583">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="018bf-2584">[BREAKING CHANGE]`list`-Befehle geändert, sodass Fehler von Typ „NotFound(404)“ für Ressourcen mit der typische Vorgehensweise behandelt werden, anstatt eine leere Liste anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="018bf-2584">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="018bf-2585">Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="018bf-2585">Extensions</span></span>
* <span data-ttu-id="018bf-2586">Problem beim Hinzufügen einer Erweiterung behoben, die bereits installiert ist</span><span class="sxs-lookup"><span data-stu-id="018bf-2586">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="018bf-2587">HDInsight</span><span class="sxs-lookup"><span data-stu-id="018bf-2587">HDInsight</span></span>
* <span data-ttu-id="018bf-2588">Erste Veröffentlichung</span><span class="sxs-lookup"><span data-stu-id="018bf-2588">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="018bf-2589">IoT</span><span class="sxs-lookup"><span data-stu-id="018bf-2589">IoT</span></span>
* <span data-ttu-id="018bf-2590">Befehl zur Erweiterungsinstallation zu Banner bei der ersten Ausführung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2590">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="018bf-2591">KeyVault</span><span class="sxs-lookup"><span data-stu-id="018bf-2591">KeyVault</span></span>
* <span data-ttu-id="018bf-2592">Geändert, sodass Key Vault-Speicherbefehle auf das aktuelle API-Profil beschränkt sind</span><span class="sxs-lookup"><span data-stu-id="018bf-2592">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="018bf-2593">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="018bf-2593">Network</span></span>
* <span data-ttu-id="018bf-2594">`network dns zone create` korrigiert: Befehl ist auch erfolgreich, wenn der Benutzer einen Standardspeicherort konfiguriert hat.</span><span class="sxs-lookup"><span data-stu-id="018bf-2594">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="018bf-2595">Siehe Nr. 6052</span><span class="sxs-lookup"><span data-stu-id="018bf-2595">See #6052</span></span>
* <span data-ttu-id="018bf-2596">`--remote-vnet-id` für `network vnet peering create` eingestellt</span><span class="sxs-lookup"><span data-stu-id="018bf-2596">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="018bf-2597">`--remote-vnet` zum `network vnet peering create`-Element hinzugefügt, das einen Namen oder eine ID akzeptiert</span><span class="sxs-lookup"><span data-stu-id="018bf-2597">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="018bf-2598">Unterstützung für mehrere Subnetzpräfixe zu `network vnet create` in `--subnet-prefixes` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2598">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="018bf-2599">Unterstützung für mehrere Subnetzpräfixe zu `network vnet subnet [create|update]` in `--address-prefixes` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2599">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="018bf-2600">Problem mit `network application-gateway create` behoben, das die Erstellung von Gateways mit der SKU `WAF_v2` oder `Standard_v2` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="018bf-2600">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="018bf-2601">`--service-endpoint-policy`-Argument für Benutzerfreundlichkeit zu `network vnet subnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2601">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="018bf-2602">Role</span><span class="sxs-lookup"><span data-stu-id="018bf-2602">Role</span></span>
* <span data-ttu-id="018bf-2603">Unterstützung für das Auflisten von Azure AD-App-Besitzern in `ad app owner` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2603">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="018bf-2604">Unterstützung für das Auflisten von Azure AD-Dienstprinzipalbesitzern in `ad sp owner` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2604">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="018bf-2605">Geändert, um sicherzustellen, dass die Erstellungs- und Aktualisierungsbefehle für die Rollendefinition Konfigurationen mit mehreren Berechtigungen akzeptieren</span><span class="sxs-lookup"><span data-stu-id="018bf-2605">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="018bf-2606">`ad sp create-for-rbac` geändert, um sicherzustellen, dass der Homepage-URI immer „https“ ist</span><span class="sxs-lookup"><span data-stu-id="018bf-2606">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="018bf-2607">Service Bus</span><span class="sxs-lookup"><span data-stu-id="018bf-2607">Service Bus</span></span>
* <span data-ttu-id="018bf-2608">[BREAKING CHANGE]`list`-Befehle geändert, sodass Fehler von Typ „NotFound(404)“ für Ressourcen mit der typische Vorgehensweise behandelt werden, anstatt eine leere Liste anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="018bf-2608">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="018bf-2609">VM</span><span class="sxs-lookup"><span data-stu-id="018bf-2609">VM</span></span>
* <span data-ttu-id="018bf-2610">Leeres `accessSas`-Feld in `disk grant-access` korrigiert</span><span class="sxs-lookup"><span data-stu-id="018bf-2610">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="018bf-2611">`vmss create` geändert, sodass ein ausreichend großer Front-End-Portbereich zur Verarbeitung von Überbereitstellung reserviert ist</span><span class="sxs-lookup"><span data-stu-id="018bf-2611">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="018bf-2612">Aktualisierungsbefehle für `sig` korrigiert</span><span class="sxs-lookup"><span data-stu-id="018bf-2612">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="018bf-2613">`--no-wait`-Unterstützung für die Verwaltung von Imageversionen in `sig` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2613">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="018bf-2614">`vm list-ip-addresses` geändert, sodass die Verfügbarkeitszone von öffentlichen IP-Adressen angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="018bf-2614">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="018bf-2615">`[vm|vmss] disk attach` geändert, sodass die Standard-LUN eines Datenträgers standardmäßig auf die erste verfügbare Stelle festgelegt wird</span><span class="sxs-lookup"><span data-stu-id="018bf-2615">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="018bf-2616">21. September 2018</span><span class="sxs-lookup"><span data-stu-id="018bf-2616">September 21, 2018</span></span>

<span data-ttu-id="018bf-2617">Version 2.0.46</span><span class="sxs-lookup"><span data-stu-id="018bf-2617">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="018bf-2618">ACR</span><span class="sxs-lookup"><span data-stu-id="018bf-2618">ACR</span></span>
* <span data-ttu-id="018bf-2619">ACR-Aufgabenbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2619">Added ACR Task commands</span></span>
* <span data-ttu-id="018bf-2620">Befehl für die Schnellausführung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2620">Added quick run command</span></span>
* <span data-ttu-id="018bf-2621">`build-task`-Befehlsgruppe als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="018bf-2621">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="018bf-2622">`helm`-Befehlsgruppe hinzugefügt, um die Verwaltung von Helm-Diagrammen mit ACR zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="018bf-2622">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="018bf-2623">Unterstützung für idempotentes Erstellen für die verwaltete Registrierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2623">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="018bf-2624">Formatfreies Flag für die Anzeige von Buildprotokollen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2624">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="018bf-2625">ACS</span><span class="sxs-lookup"><span data-stu-id="018bf-2625">ACS</span></span>
* <span data-ttu-id="018bf-2626">Befehl `install-connector` zum Festlegen des AKS-Master-FQDN geändert</span><span class="sxs-lookup"><span data-stu-id="018bf-2626">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="018bf-2627">Erstellen der Rollenzuweisung für „vnet-subnet-id“ (wenn kein Dienstprinzipal angegeben wurde) und „skip-role-assignment“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="018bf-2627">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="018bf-2628">AppService</span><span class="sxs-lookup"><span data-stu-id="018bf-2628">AppService</span></span>

* <span data-ttu-id="018bf-2629">Unterstützung für WebJobs-Vorgangsverwaltung hinzugefügt (kontinuierlich/ausgelöst)</span><span class="sxs-lookup"><span data-stu-id="018bf-2629">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="018bf-2630">„az webapp config set“ unterstützt die Eigenschaft „--fts-state“; Unterstützung für „az functionapp config set/show“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2630">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="018bf-2631">Unterstützung für Bring Your Own Storage für Web-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2631">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="018bf-2632">Unterstützung für das Auflisten und Wiederherstellen gelöschter Web-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2632">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="018bf-2633">Batch</span><span class="sxs-lookup"><span data-stu-id="018bf-2633">Batch</span></span>
* <span data-ttu-id="018bf-2634">Hinzufügen von Aufgaben über `--json-file` geändert, um die AddTaskCollectionParameter-Syntax zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="018bf-2634">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="018bf-2635">Dokumentation akzeptierter `--json-file`-Formate aktualisiert</span><span class="sxs-lookup"><span data-stu-id="018bf-2635">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="018bf-2636">`--max-tasks-per-node-option` zu `batch pool create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2636">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="018bf-2637">Verhalten von `batch account` geändert, um das aktuell angemeldete Konto anzuzeigen, wenn keine Optionen angegeben wurden</span><span class="sxs-lookup"><span data-stu-id="018bf-2637">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="018bf-2638">Batch KI</span><span class="sxs-lookup"><span data-stu-id="018bf-2638">Batch AI</span></span> 
* <span data-ttu-id="018bf-2639">Fehler bei der automatischen Speicherkontoerstellung im Befehl `batchai cluster create` behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-2639">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="018bf-2640">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="018bf-2640">Cognitive Services</span></span>
* <span data-ttu-id="018bf-2641">Vervollständigung für die Argumente `--sku`, `--kind` und `--location` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2641">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="018bf-2642">Befehl `cognitiveservices account list-usage` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2642">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="018bf-2643">Befehl `cognitiveservices account list-kinds` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2643">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="018bf-2644">Befehl `cognitiveservices account list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2644">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="018bf-2645">`cognitiveservices list` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="018bf-2645">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="018bf-2646">`--name` geändert (ist jetzt optional für `cognitiveservices account list-skus`)</span><span class="sxs-lookup"><span data-stu-id="018bf-2646">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="018bf-2647">Container</span><span class="sxs-lookup"><span data-stu-id="018bf-2647">Container</span></span>
* <span data-ttu-id="018bf-2648">Möglichkeit zum Neustarten und Beenden einer ausgeführten Containergruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2648">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="018bf-2649">`--network-profile` zum Übergeben eines Netzwerkprofils hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2649">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="018bf-2650">`--subnet` und `--vnet_name` hinzugefügt, um das Erstellen von Containergruppen in einem VNET zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="018bf-2650">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="018bf-2651">Tabellenausgabe geändert, sodass der Status der Containergruppe angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="018bf-2651">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="018bf-2652">Data Lake</span><span class="sxs-lookup"><span data-stu-id="018bf-2652">Datalake</span></span>
* <span data-ttu-id="018bf-2653">Befehle für VNET-Regeln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2653">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="018bf-2654">Interaktive Shell</span><span class="sxs-lookup"><span data-stu-id="018bf-2654">Interactive Shell</span></span>
* <span data-ttu-id="018bf-2655">Fehler in Windows behoben, durch den Befehle nicht ordnungsgemäß ausgeführt wurden</span><span class="sxs-lookup"><span data-stu-id="018bf-2655">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="018bf-2656">Durch veraltete Objekte verursachtes Problem beim Laden von Befehlen im interaktiven Modus behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-2656">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="018bf-2657">IoT</span><span class="sxs-lookup"><span data-stu-id="018bf-2657">IoT</span></span>
* <span data-ttu-id="018bf-2658">Routingunterstützung für IoT Hubs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2658">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="018bf-2659">Key Vault</span><span class="sxs-lookup"><span data-stu-id="018bf-2659">Key Vault</span></span>
* <span data-ttu-id="018bf-2660">Key Vault-Schlüsselimport für RSA-Schlüssel korrigiert</span><span class="sxs-lookup"><span data-stu-id="018bf-2660">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="018bf-2661">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="018bf-2661">Network</span></span>
* <span data-ttu-id="018bf-2662">Befehle vom Typ `network public-ip prefix` hinzugefügt, um Präfixe von öffentlichen IP-Adressen zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="018bf-2662">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="018bf-2663">Befehle vom Typ `network service-endpoint` hinzugefügt, um Dienstendpunktrichtlinien-Features zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="018bf-2663">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="018bf-2664">Befehle vom Typ `network lb outbound-rule` hinzugefügt, um die Erstellung von Ausgangsregeln für Load Balancer Standard zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="018bf-2664">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="018bf-2665">`--public-ip-prefix` zu `network lb frontend-ip create/update` hinzugefügt, um Front-End-IP-Konfigurationen mit Präfixen von öffentlichen IP-Adressen zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="018bf-2665">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="018bf-2666">`--enable-tcp-reset` zu `network lb rule/inbound-nat-rule/inbound-nat-pool create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2666">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="018bf-2667">`--disable-outbound-snat` zu `network lb rule create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2667">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="018bf-2668">Verwendung von `network watcher flow-log show/configure` mit klassischen NSGs ermöglicht</span><span class="sxs-lookup"><span data-stu-id="018bf-2668">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="018bf-2669">Hinzufügen des `network watcher run-configuration-diagnostic`-Befehls</span><span class="sxs-lookup"><span data-stu-id="018bf-2669">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="018bf-2670">Befehl `network watcher test-connectivity` korrigiert und Eigenschaften `--method`, `--valid-status-codes` und `--headers` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2670">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="018bf-2671">`network express-route create/update`: Flag `--allow-global-reach` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2671">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="018bf-2672">`network vnet subnet create/update`: Unterstützung für `--delegation` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2672">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="018bf-2673">Befehl `network vnet subnet list-available-delegations` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2673">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="018bf-2674">`network traffic-manager profile create/update`: Unterstützung für `--interval`, `--timeout` und `--max-failures` für die Überwachungskonfiguration hinzugefügt; Optionen `--monitor-path`, `--monitor-port` und `--monitor-protocol` zugunsten von `--path`, `--port` und `--protocol` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="018bf-2674">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="018bf-2675">`network lb frontend-ip create/update`: Logik für das Festlegen der Zuweisungsmethode für private IP-Adressen korrigiert. Bei Angabe einer privaten IP-Adresse ist die Zuweisung statisch. Wird keine private IP-Adresse (oder eine leere Zeichenfolge für die private IP-Adresse) angegeben, erfolgt eine dynamische Zuweisung.</span><span class="sxs-lookup"><span data-stu-id="018bf-2675">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="018bf-2676">`dns record-set * create/update`: Unterstützung für `--target-resource` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2676">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="018bf-2677">Befehle vom Typ `network interface-endpoint` hinzugefügt, um Schnittstellenendpunkt-Objekte abzufragen</span><span class="sxs-lookup"><span data-stu-id="018bf-2677">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="018bf-2678">`network profile show/list/delete` für die partielle Verwaltung von Netzwerkprofilen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2678">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="018bf-2679">Befehle vom Typ `network express-route peering connection` für die Verwaltung von Peeringverbindungen zwischen ExpressRoute-Instanzen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2679">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="018bf-2680">RDBMS</span><span class="sxs-lookup"><span data-stu-id="018bf-2680">RDBMS</span></span>
* <span data-ttu-id="018bf-2681">Unterstützung für den MariaDB-Dienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2681">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="018bf-2682">Reservierung</span><span class="sxs-lookup"><span data-stu-id="018bf-2682">Reservation</span></span>
* <span data-ttu-id="018bf-2683">Cosmos DB im Enumerationstyp für reservierte Ressourcen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2683">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="018bf-2684">Namenseigenschaft im Patchmodell hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2684">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="018bf-2685">App-Verwaltung</span><span class="sxs-lookup"><span data-stu-id="018bf-2685">Manage App</span></span>
* <span data-ttu-id="018bf-2686">Fehler in `managedapp create --kind MarketPlace` korrigiert, der zum Absturz der Instanzerstellung einer verwalteten Marketplace-App führte</span><span class="sxs-lookup"><span data-stu-id="018bf-2686">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="018bf-2687">Befehle vom Typ `feature` geändert, um sie auf unterstützte Profile zu beschränken</span><span class="sxs-lookup"><span data-stu-id="018bf-2687">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="018bf-2688">Role</span><span class="sxs-lookup"><span data-stu-id="018bf-2688">Role</span></span>
* <span data-ttu-id="018bf-2689">Unterstützung für das Auflisten der Gruppenmitgliedschaften des Benutzers hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2689">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="018bf-2690">SignalR</span><span class="sxs-lookup"><span data-stu-id="018bf-2690">SignalR</span></span>
* <span data-ttu-id="018bf-2691">Erste Version</span><span class="sxs-lookup"><span data-stu-id="018bf-2691">First release</span></span>

### <a name="storage"></a><span data-ttu-id="018bf-2692">Storage</span><span class="sxs-lookup"><span data-stu-id="018bf-2692">Storage</span></span>
* <span data-ttu-id="018bf-2693">Parameter `--auth-mode login` für die Verwendung der Anmeldeinformationen des Benutzers für die Blob- und Warteschlangenautorisierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2693">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="018bf-2694">`storage container immutability-policy/legal-hold` für die Verwaltung von unveränderlichem Speicher hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2694">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="018bf-2695">VM</span><span class="sxs-lookup"><span data-stu-id="018bf-2695">VM</span></span>
* <span data-ttu-id="018bf-2696">Problem behoben, das dazu führte, dass die Datei mit dem privaten Schlüssel durch `vm create --generate-ssh-keys` überschrieben wird, wenn die Datei mit dem privaten Schlüssel fehlt (Nr. 4725, 6780)</span><span class="sxs-lookup"><span data-stu-id="018bf-2696">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="018bf-2697">Unterstützung für den gemeinsamen Image-Katalog über `az sig` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2697">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="018bf-2698">28. August 2018</span><span class="sxs-lookup"><span data-stu-id="018bf-2698">August 28, 2018</span></span>

<span data-ttu-id="018bf-2699">Version 2.0.45</span><span class="sxs-lookup"><span data-stu-id="018bf-2699">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="018bf-2700">Core</span><span class="sxs-lookup"><span data-stu-id="018bf-2700">Core</span></span>

* <span data-ttu-id="018bf-2701">Das Problem, aufgrund dessen eine leere Konfigurationsdatei geladen wurde, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="018bf-2701">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="018bf-2702">Unterstützung für Profil `2018-03-01-hybrid` für Azure Stack hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2702">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="018bf-2703">ACR</span><span class="sxs-lookup"><span data-stu-id="018bf-2703">ACR</span></span>

* <span data-ttu-id="018bf-2704">Problemumgehung für Laufzeitvorgänge ohne ARM-Anforderungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2704">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="018bf-2705">Änderung vorgenommen, um im Befehl `build` Versionskontrolldateien (etwa „.git“ und „.gitignore“) standardmäßig aus der TAR-Datei auszuschließen</span><span class="sxs-lookup"><span data-stu-id="018bf-2705">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="018bf-2706">ACS</span><span class="sxs-lookup"><span data-stu-id="018bf-2706">ACS</span></span>

* <span data-ttu-id="018bf-2707">`aks create` geändert, dass standardmäßig virtuelle Computer vom Typ `Standard_DS2_v2` erstellt werden</span><span class="sxs-lookup"><span data-stu-id="018bf-2707">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="018bf-2708">`aks get-credentials` geändert, um nun neue APIs zum Abrufen der Clusteranmeldeinformationen aufzurufen</span><span class="sxs-lookup"><span data-stu-id="018bf-2708">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="018bf-2709">AppService</span><span class="sxs-lookup"><span data-stu-id="018bf-2709">AppService</span></span>

* <span data-ttu-id="018bf-2710">Unterstützung für CORS in „functionapp“ und „webapp“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2710">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="018bf-2711">ARM-Tagunterstützung in Erstellungsbefehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2711">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="018bf-2712">`[webapp|functionapp] identity show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="018bf-2712">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="018bf-2713">Backup</span><span class="sxs-lookup"><span data-stu-id="018bf-2713">Backup</span></span>

* <span data-ttu-id="018bf-2714">`backup vault backup-properties show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="018bf-2714">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="018bf-2715">Botdienst</span><span class="sxs-lookup"><span data-stu-id="018bf-2715">Bot Service</span></span>

* <span data-ttu-id="018bf-2716">Anfängliches Release der Botdienst-CLI</span><span class="sxs-lookup"><span data-stu-id="018bf-2716">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="018bf-2717">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="018bf-2717">Cognitive Services</span></span>

* <span data-ttu-id="018bf-2718">Neuer Parameter `--api-properties,` hinzugefügt, der zum Erstellen einiger Dienste erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="018bf-2718">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="018bf-2719">IoT</span><span class="sxs-lookup"><span data-stu-id="018bf-2719">IoT</span></span>

* <span data-ttu-id="018bf-2720">Problem mit dem Zuweisen verknüpfter Hubs behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-2720">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="018bf-2721">Überwachen</span><span class="sxs-lookup"><span data-stu-id="018bf-2721">Monitor</span></span>

* <span data-ttu-id="018bf-2722">`monitor metrics alert`-Befehle für Metrikwarnungen nahezu in Echtzeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2722">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="018bf-2723">`monitor alert`-Befehle als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="018bf-2723">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="018bf-2724">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="018bf-2724">Network</span></span>

* <span data-ttu-id="018bf-2725">`network application-gateway ssl-policy predefined show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="018bf-2725">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="018bf-2726">Resource</span><span class="sxs-lookup"><span data-stu-id="018bf-2726">Resource</span></span>

* <span data-ttu-id="018bf-2727">`provider operation show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="018bf-2727">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="018bf-2728">Storage</span><span class="sxs-lookup"><span data-stu-id="018bf-2728">Storage</span></span>

* <span data-ttu-id="018bf-2729">`storage share policy show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="018bf-2729">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="018bf-2730">VM</span><span class="sxs-lookup"><span data-stu-id="018bf-2730">VM</span></span>

* <span data-ttu-id="018bf-2731">`vm/vmss identity show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="018bf-2731">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="018bf-2732">`--storage-caching` für `vm create` eingestellt</span><span class="sxs-lookup"><span data-stu-id="018bf-2732">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="018bf-2733">14. August 2018</span><span class="sxs-lookup"><span data-stu-id="018bf-2733">Auguest 14, 2018</span></span>

<span data-ttu-id="018bf-2734">Version 2.0.44</span><span class="sxs-lookup"><span data-stu-id="018bf-2734">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="018bf-2735">Core</span><span class="sxs-lookup"><span data-stu-id="018bf-2735">Core</span></span>

* <span data-ttu-id="018bf-2736">Numerische Anzeige in `table`-Ausgabe korrigiert</span><span class="sxs-lookup"><span data-stu-id="018bf-2736">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="018bf-2737">YAML-Ausgabeformat hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2737">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="018bf-2738">Telemetrie</span><span class="sxs-lookup"><span data-stu-id="018bf-2738">Telemetry</span></span>

* <span data-ttu-id="018bf-2739">Verbesserte Berichterstellung für Telemetriedaten</span><span class="sxs-lookup"><span data-stu-id="018bf-2739">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="018bf-2740">ACR</span><span class="sxs-lookup"><span data-stu-id="018bf-2740">ACR</span></span>

* <span data-ttu-id="018bf-2741">Befehle vom Typ `content-trust policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2741">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="018bf-2742">Problem behoben, aufgrund dessen `.dockerignore` nicht richtig verarbeitet wurde</span><span class="sxs-lookup"><span data-stu-id="018bf-2742">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="018bf-2743">ACS</span><span class="sxs-lookup"><span data-stu-id="018bf-2743">ACS</span></span>

* <span data-ttu-id="018bf-2744">`az acs/aks install-cli` für die Installation in `%USERPROFILE%\.azure-kubectl` unter Windows geändert</span><span class="sxs-lookup"><span data-stu-id="018bf-2744">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="018bf-2745">`az aks install-connector` geändert, um zu ermitteln, ob der Cluster über RBAC verfügt, und um den ACI-Connector entsprechend zu konfigurieren</span><span class="sxs-lookup"><span data-stu-id="018bf-2745">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="018bf-2746">Geändert in Rollenzuweisung zum Subnetz bei entsprechender Angabe</span><span class="sxs-lookup"><span data-stu-id="018bf-2746">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="018bf-2747">Neue Option zum Überspringen der Rollenzuweisung für Subnetz hinzugefügt, wenn dieses angegeben ist</span><span class="sxs-lookup"><span data-stu-id="018bf-2747">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="018bf-2748">Geändert, um Rollenzuweisung zum Subnetz zu überspringen, wenn bereits eine Zuweisung vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="018bf-2748">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="018bf-2749">AppService</span><span class="sxs-lookup"><span data-stu-id="018bf-2749">AppService</span></span>

* <span data-ttu-id="018bf-2750">Fehler behoben, der das Erstellen einer Funktions-App mithilfe von Speicherkonten in externen Ressourcengruppen verhinderte</span><span class="sxs-lookup"><span data-stu-id="018bf-2750">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="018bf-2751">Absturz bei ZIP-Bereitstellung behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-2751">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="018bf-2752">Batch AI</span><span class="sxs-lookup"><span data-stu-id="018bf-2752">BatchAI</span></span>

* <span data-ttu-id="018bf-2753">Protokollierungsausgabe für die automatische Speicherkontoerstellung geändert, sodass nun „Ressourcen *gruppe* “ angegeben wird</span><span class="sxs-lookup"><span data-stu-id="018bf-2753">Changed logger output for auto-storage account creation to specifies "resource *group* ".</span></span>        

### <a name="container"></a><span data-ttu-id="018bf-2754">Container</span><span class="sxs-lookup"><span data-stu-id="018bf-2754">Container</span></span>

* <span data-ttu-id="018bf-2755">`--secure-environment-variables` zum Übergeben sicherer Umgebungsvariablen an einen Container hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2755">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="018bf-2756">IoT</span><span class="sxs-lookup"><span data-stu-id="018bf-2756">IoT</span></span>

* <span data-ttu-id="018bf-2757">[BREAKING CHANGE] Veraltete Befehle entfernt, die in die IoT-Erweiterung verschoben wurden</span><span class="sxs-lookup"><span data-stu-id="018bf-2757">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="018bf-2758">Elemente aktualisiert, um nicht die Domäne `azure-devices.net` anzunehmen</span><span class="sxs-lookup"><span data-stu-id="018bf-2758">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="018bf-2759">Iot Central</span><span class="sxs-lookup"><span data-stu-id="018bf-2759">Iot Central</span></span>

* <span data-ttu-id="018bf-2760">Erstes Release des IoT Central-Moduls</span><span class="sxs-lookup"><span data-stu-id="018bf-2760">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="018bf-2761">KeyVault</span><span class="sxs-lookup"><span data-stu-id="018bf-2761">KeyVault</span></span>


* <span data-ttu-id="018bf-2762">Befehle zum Verwalten von Speicherkonten und SAS-Definitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2762">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="018bf-2763">Befehle für Netzwerkregeln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2763">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="018bf-2764">Parameter `--id` zu Geheimnis-, Schlüssel- und Zertifikatvorgängen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2764">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="018bf-2765">Unterstützung für Version mit mehreren APIs zur Schlüsseltresorverwaltung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2765">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="018bf-2766">Unterstützung für Version mit mehreren APIs zur Schlüsseltresordatenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2766">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="018bf-2767">Relay</span><span class="sxs-lookup"><span data-stu-id="018bf-2767">Relay</span></span>

* <span data-ttu-id="018bf-2768">Erste Veröffentlichung</span><span class="sxs-lookup"><span data-stu-id="018bf-2768">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="018bf-2769">Sql</span><span class="sxs-lookup"><span data-stu-id="018bf-2769">Sql</span></span>

* <span data-ttu-id="018bf-2770">Befehle vom Typ `sql failover-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2770">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="018bf-2771">Storage</span><span class="sxs-lookup"><span data-stu-id="018bf-2771">Storage</span></span>

* <span data-ttu-id="018bf-2772">[BREAKING CHANGE]`storage account show-usage` geändert, um Parameter `--location` erforderlich zu machen. Auflistung nach Region</span><span class="sxs-lookup"><span data-stu-id="018bf-2772">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="018bf-2773">Parameter `--resource-group` geändert, sodass er für `storage account`-Befehle optional ist</span><span class="sxs-lookup"><span data-stu-id="018bf-2773">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="018bf-2774">Warnungen vom Typ „Fehler bei Vorbedingung“ für einzelne Fehler in Batch-Befehlen für eine aggregiert Nachricht entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-2774">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="018bf-2775">`[blob|file] delete-batch`-Befehle geändert, sodass kein Array mit Null-Werten mehr ausgegeben wird</span><span class="sxs-lookup"><span data-stu-id="018bf-2775">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="018bf-2776">`blob [download|upload|delete-batch]`-Befehle geändert, um SAS-Token aus Container-URL zu lesen</span><span class="sxs-lookup"><span data-stu-id="018bf-2776">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="018bf-2777">VM</span><span class="sxs-lookup"><span data-stu-id="018bf-2777">VM</span></span>

* <span data-ttu-id="018bf-2778">Allgemeine Filter zu `vm list-skus` für höhere Benutzerfreundlichkeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2778">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="018bf-2779">31. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="018bf-2779">July 31, 2018</span></span>

<span data-ttu-id="018bf-2780">Version 2.0.43</span><span class="sxs-lookup"><span data-stu-id="018bf-2780">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="018bf-2781">ACR</span><span class="sxs-lookup"><span data-stu-id="018bf-2781">ACR</span></span>

* <span data-ttu-id="018bf-2782">Flag `--with-secure-properties` zum Befehl `acr build-task show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2782">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="018bf-2783">Befehl `acr build-task update-build` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2783">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="018bf-2784">ACS</span><span class="sxs-lookup"><span data-stu-id="018bf-2784">ACS</span></span>

* <span data-ttu-id="018bf-2785">Änderung, um 0 (Erfolg) zurückzugeben, wenn `az aks browse` durch Drücken von [STRG+C] beendet wird</span><span class="sxs-lookup"><span data-stu-id="018bf-2785">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="018bf-2786">Batch</span><span class="sxs-lookup"><span data-stu-id="018bf-2786">Batch</span></span>

* <span data-ttu-id="018bf-2787">Korrektur eines Fehlers bei der Anzeige des AAD-Tokens in Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="018bf-2787">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="018bf-2788">Container</span><span class="sxs-lookup"><span data-stu-id="018bf-2788">Container</span></span>

* <span data-ttu-id="018bf-2789">Voraussetzung von `--log-analytics-workspace-key` für Name oder ID im festgelegten Abonnement entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-2789">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="018bf-2790">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="018bf-2790">Network</span></span>

* <span data-ttu-id="018bf-2791">DNS-Unterstützung zu „2017-03-09-profile“ für Azure Stack hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2791">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="018bf-2792">Resource</span><span class="sxs-lookup"><span data-stu-id="018bf-2792">Resource</span></span>

* <span data-ttu-id="018bf-2793">`--rollback-on-error` zu `group deployment create` hinzugefügt, um bei einem Fehler eine als funktionierend bekannte Bereitstellung auszuführen</span><span class="sxs-lookup"><span data-stu-id="018bf-2793">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="018bf-2794">Problem behoben, aufgrund dessen `--parameters {}` mit `group deployment create` zu einem Fehler führte</span><span class="sxs-lookup"><span data-stu-id="018bf-2794">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="018bf-2795">Role</span><span class="sxs-lookup"><span data-stu-id="018bf-2795">Role</span></span>

* <span data-ttu-id="018bf-2796">Unterstützung für das Stack-Profil „2017-03-09-profile“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2796">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="018bf-2797">Problem behoben, aufgrund dessen das generische Update von Parametern auf `app update` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="018bf-2797">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="018bf-2798">Suchen,</span><span class="sxs-lookup"><span data-stu-id="018bf-2798">Search</span></span>

* <span data-ttu-id="018bf-2799">Befehle für Azure Search-Dienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2799">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="018bf-2800">Service Bus</span><span class="sxs-lookup"><span data-stu-id="018bf-2800">Service Bus</span></span>

* <span data-ttu-id="018bf-2801">Migrationsbefehlsgruppe hinzugefügt, um einen Namespace von Service Bus Standard zu Premium zu migrieren</span><span class="sxs-lookup"><span data-stu-id="018bf-2801">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="018bf-2802">Neue optionale Eigenschaften zu Service Bus-Warteschlange und -Abonnement hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2802">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="018bf-2803">`--enable-batched-operations` und `--enable-dead-lettering-on-message-expiration` in `queue`</span><span class="sxs-lookup"><span data-stu-id="018bf-2803">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="018bf-2804">`--dead-letter-on-filter-exceptions` in `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="018bf-2804">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="018bf-2805">Storage</span><span class="sxs-lookup"><span data-stu-id="018bf-2805">Storage</span></span>

* <span data-ttu-id="018bf-2806">Unterstützung für den Download großer Dateien über eine einzelne Verbindung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2806">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="018bf-2807">`show`-Befehle konvertiert, bei denen im Falle einer fehlenden Ressource kein Fehler mit dem Exitcode 3 ausgelöst wurde</span><span class="sxs-lookup"><span data-stu-id="018bf-2807">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="018bf-2808">VM</span><span class="sxs-lookup"><span data-stu-id="018bf-2808">VM</span></span>

* <span data-ttu-id="018bf-2809">Unterstützung zum Auflisten von Verfügbarkeitsgruppen nach Abonnement hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2809">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="018bf-2810">Unterstützung für `StandardSSD_LRS` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-2810">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="018bf-2811">Unterstützung für Anwendungssicherheitsgruppe beim Erstellen einer VM-Skalierungsgruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2811">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="018bf-2812">[BREAKING CHANGE]`[vm|vmss] create`, `[vm|vmss] identity assign` und `[vm|vmss] identity remove` wurden geändert, um vom Benutzer zugewiesene Identitäten im Wörterbuchformat auszugeben.</span><span class="sxs-lookup"><span data-stu-id="018bf-2812">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="018bf-2813">18. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="018bf-2813">July 18, 2018</span></span>

<span data-ttu-id="018bf-2814">Version 2.0.42</span><span class="sxs-lookup"><span data-stu-id="018bf-2814">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="018bf-2815">Core</span><span class="sxs-lookup"><span data-stu-id="018bf-2815">Core</span></span>

* <span data-ttu-id="018bf-2816">Unterstützung für browserbasierte Anmeldung WSL-Bash-Fenster hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2816">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="018bf-2817">`--force-string`-Flag für alle generischen Updatebefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2817">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="018bf-2818">[BREAKING CHANGE] Befehle vom Typ „show“ so geändert, dass die Fehlermeldung protokolliert wird und der Vorgang bei einer fehlenden Ressource mit dem Exitcode 3 fehlschlägt</span><span class="sxs-lookup"><span data-stu-id="018bf-2818">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="018bf-2819">ACR</span><span class="sxs-lookup"><span data-stu-id="018bf-2819">ACR</span></span>

* <span data-ttu-id="018bf-2820">[BREAKING CHANGE] „--no-push“ in Befehl „acr build“ in reines Flag geändert</span><span class="sxs-lookup"><span data-stu-id="018bf-2820">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="018bf-2821">Befehle `show` und `update` unter Gruppe `acr repository` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2821">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="018bf-2822">`--detail`-Flag für `show-manifests` und `show-tags` hinzugefügt, um ausführlichere Informationen anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="018bf-2822">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="018bf-2823">Parameter `--image` zur Unterstützung des Abrufs von Builddetails oder Protokollen anhand eines Images hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2823">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="018bf-2824">ACS</span><span class="sxs-lookup"><span data-stu-id="018bf-2824">ACS</span></span>

* <span data-ttu-id="018bf-2825">`az aks create` so geändert, dass mit Fehler beendet wird, wenn `--max-pods` kleiner als 5 ist</span><span class="sxs-lookup"><span data-stu-id="018bf-2825">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="018bf-2826">AppService</span><span class="sxs-lookup"><span data-stu-id="018bf-2826">AppService</span></span>

* <span data-ttu-id="018bf-2827">Unterstützung für PremiumV2-SKUs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2827">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="018bf-2828">Batch</span><span class="sxs-lookup"><span data-stu-id="018bf-2828">Batch</span></span>

* <span data-ttu-id="018bf-2829">Korrektur eines Fehlers bei der Verwendung von Anmeldeinformationen im Cloud Shell-Modus</span><span class="sxs-lookup"><span data-stu-id="018bf-2829">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="018bf-2830">JSON-Eingabe so geändert, dass Groß-/Kleinschreibung nicht beachtet wird</span><span class="sxs-lookup"><span data-stu-id="018bf-2830">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="018bf-2831">Batch KI</span><span class="sxs-lookup"><span data-stu-id="018bf-2831">Batch AI</span></span>

* <span data-ttu-id="018bf-2832">Befehl `az batchai job exec` korrigiert</span><span class="sxs-lookup"><span data-stu-id="018bf-2832">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="018bf-2833">Container</span><span class="sxs-lookup"><span data-stu-id="018bf-2833">Container</span></span>

* <span data-ttu-id="018bf-2834">Anforderung von Benutzername und Kennwort für Nicht-DockerHub-Registrierungen entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-2834">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="018bf-2835">Fehler beim Erstellen von Containergruppen aus YAML-Datei behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-2835">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="018bf-2836">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="018bf-2836">Network</span></span>

* <span data-ttu-id="018bf-2837">Unterstützung für `--no-wait` zu `network nic [create|update|delete]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2837">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="018bf-2838">`network nic wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2838">Added `network nic wait`</span></span>
* <span data-ttu-id="018bf-2839">`--ids`-Argument für `network vnet [subnet|peering] list` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="018bf-2839">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="018bf-2840">`--include-default`-Flag hinzugefügt, um Standardsicherheitsregeln in die Ausgabe von `network nsg rule list` aufzunehmen</span><span class="sxs-lookup"><span data-stu-id="018bf-2840">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="018bf-2841">Resource</span><span class="sxs-lookup"><span data-stu-id="018bf-2841">Resource</span></span>

* <span data-ttu-id="018bf-2842">Unterstützung für `--no-wait` zu `group deployment delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2842">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="018bf-2843">Unterstützung für `--no-wait` zu `deployment delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2843">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="018bf-2844">Befehl `deployment wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2844">Added `deployment wait` command</span></span>
* <span data-ttu-id="018bf-2845">Problem behoben, aufgrund dessen die `az deployment`-Befehle auf Abonnementebene fälschlicherweise für Profil „2017-03-09-profile“ angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="018bf-2845">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="018bf-2846">SQL</span><span class="sxs-lookup"><span data-stu-id="018bf-2846">SQL</span></span>

* <span data-ttu-id="018bf-2847">Fehler „Der angegebene Ressourcengruppenname ... entsprach nicht dem Namen in der URL“ beim Angeben des Namens des Pools für elastische Datenbanken für `sql db copy`-und `sql db replica create`-Befehle behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-2847">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="018bf-2848">Konfigurieren des Standard-SQL Servers durch Ausführen von `az configure --defaults sql-server=<name>` zulässig</span><span class="sxs-lookup"><span data-stu-id="018bf-2848">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="018bf-2849">Tabellenformatierer für Befehle `sql server`, `sql server firewall-rule`, `sql list-usages` und `sql show-usage` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2849">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="018bf-2850">Storage</span><span class="sxs-lookup"><span data-stu-id="018bf-2850">Storage</span></span>

* <span data-ttu-id="018bf-2851">`pageRanges`-Eigenschaft zu `storage blob show`-Ausgabe hinzugefügt, die für Seitenblobs ausgefüllt wird</span><span class="sxs-lookup"><span data-stu-id="018bf-2851">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="018bf-2852">VM</span><span class="sxs-lookup"><span data-stu-id="018bf-2852">VM</span></span>

* <span data-ttu-id="018bf-2853">[BREAKING CHANGE]`vmss create` so geändert, dass `Standard_DS1_v2` als standardmäßige Instanzgröße verwendet wird</span><span class="sxs-lookup"><span data-stu-id="018bf-2853">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="018bf-2854">Unterstützung für `--no-wait` zu `vm extension [set|delete]` und `vmss extension [set|delete]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2854">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="018bf-2855">`vm extension wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2855">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="018bf-2856">3\. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="018bf-2856">July 3, 2018</span></span>

<span data-ttu-id="018bf-2857">Version 2.0.41</span><span class="sxs-lookup"><span data-stu-id="018bf-2857">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="018bf-2858">AKS</span><span class="sxs-lookup"><span data-stu-id="018bf-2858">AKS</span></span>

* <span data-ttu-id="018bf-2859">Überwachung geändert, sodass Abonnement-ID verwendet wird</span><span class="sxs-lookup"><span data-stu-id="018bf-2859">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="018bf-2860">3\. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="018bf-2860">July 3, 2018</span></span>

<span data-ttu-id="018bf-2861">Version 2.0.40</span><span class="sxs-lookup"><span data-stu-id="018bf-2861">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="018bf-2862">Core</span><span class="sxs-lookup"><span data-stu-id="018bf-2862">Core</span></span>

* <span data-ttu-id="018bf-2863">Neuer Autorisierungscode-Flow für interaktive Anmeldung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2863">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="018bf-2864">ACR</span><span class="sxs-lookup"><span data-stu-id="018bf-2864">ACR</span></span>

* <span data-ttu-id="018bf-2865">Abruf-Buildstatus hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2865">Added polling build status</span></span>
* <span data-ttu-id="018bf-2866">Unterstützung für Enumerationswerte ohne Berücksichtigung von Groß-/Kleinschreibung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2866">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="018bf-2867">Parameter `--top` und `--orderby` für `show-manifests` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2867">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="018bf-2868">ACS</span><span class="sxs-lookup"><span data-stu-id="018bf-2868">ACS</span></span>

* <span data-ttu-id="018bf-2869">[BREAKING CHANGE] Standardmäßiges Aktivieren der rollenbasierten Zugriffssteuerung für Kubernetes</span><span class="sxs-lookup"><span data-stu-id="018bf-2869">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="018bf-2870">Argument `--disable-rbac` hinzugefügt und `--enable-rbac` als veraltet festgelegt, da es nun der Standard ist</span><span class="sxs-lookup"><span data-stu-id="018bf-2870">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="018bf-2871">Optionen für Befehl `aks browse` wurden aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="018bf-2871">Updated options for `aks browse` command.</span></span> <span data-ttu-id="018bf-2872">Unterstützung für `--listen-port` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2872">Added `--listen-port` support</span></span>
* <span data-ttu-id="018bf-2873">Standardmäßiges Helm-Diagrammpaket für Befehl `aks install-connector` wurde aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="018bf-2873">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="018bf-2874">Verwenden von „virtual-kubelet-for-aks-latest.tgz“</span><span class="sxs-lookup"><span data-stu-id="018bf-2874">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="018bf-2875">Befehle `aks enable-addons` und `aks disable-addons` zum Aktualisieren eines vorhandenen Clusters hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2875">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="018bf-2876">AppService</span><span class="sxs-lookup"><span data-stu-id="018bf-2876">AppService</span></span>

* <span data-ttu-id="018bf-2877">Unterstützung für das Deaktivieren der Identität über `webapp identity remove` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2877">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="018bf-2878">`preview`-Tag für Identitätsfunktion entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-2878">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="018bf-2879">Backup</span><span class="sxs-lookup"><span data-stu-id="018bf-2879">Backup</span></span>

* <span data-ttu-id="018bf-2880">Moduldefinition aktualisiert</span><span class="sxs-lookup"><span data-stu-id="018bf-2880">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="018bf-2881">Batch AI</span><span class="sxs-lookup"><span data-stu-id="018bf-2881">BatchAI</span></span>

* <span data-ttu-id="018bf-2882">Tabellenausgabe für Befehle `batchai cluster node list` und `batchai job node list` korrigiert</span><span class="sxs-lookup"><span data-stu-id="018bf-2882">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="018bf-2883">Cloud</span><span class="sxs-lookup"><span data-stu-id="018bf-2883">Cloud</span></span>

* <span data-ttu-id="018bf-2884">Serversuffix `acr login` zu Cloudkonfiguration hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2884">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="018bf-2885">Container</span><span class="sxs-lookup"><span data-stu-id="018bf-2885">Container</span></span>

* <span data-ttu-id="018bf-2886">`container create` zu Standard für Vorgang mit langer Ausführungsdauer geändert</span><span class="sxs-lookup"><span data-stu-id="018bf-2886">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="018bf-2887">Log Analytics-Parameter `--log-analytics-workspace` und `--log-analytics-workspace-key` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2887">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="018bf-2888">Parameter `--protocol` zum Festlegen des zu verwendenden Netzwerkprotokolls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2888">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="018bf-2889">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="018bf-2889">Extension</span></span>

* <span data-ttu-id="018bf-2890">`extension list-available` geändert, sodass nur mit der CLI-Version kompatible Erweiterungen angezeigt werden</span><span class="sxs-lookup"><span data-stu-id="018bf-2890">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="018bf-2891">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="018bf-2891">Network</span></span>

* <span data-ttu-id="018bf-2892">Problem behoben, aufgrund dessen bei Datensatztypen die Groß-/Kleinschreibung beachtet werden musste ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="018bf-2892">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="018bf-2893">Rdbms</span><span class="sxs-lookup"><span data-stu-id="018bf-2893">Rdbms</span></span>

* <span data-ttu-id="018bf-2894">Befehle vom Typ `[postgres|myql] server vnet-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2894">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="018bf-2895">Resource</span><span class="sxs-lookup"><span data-stu-id="018bf-2895">Resource</span></span>

* <span data-ttu-id="018bf-2896">Neue Vorgangsgruppe `deployment` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2896">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="018bf-2897">VM</span><span class="sxs-lookup"><span data-stu-id="018bf-2897">VM</span></span>

* <span data-ttu-id="018bf-2898">Unterstützung für das Entfernen der vom System zugewiesenen Identität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2898">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="018bf-2899">25. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="018bf-2899">June 25, 2018</span></span>

<span data-ttu-id="018bf-2900">Version 2.0.39</span><span class="sxs-lookup"><span data-stu-id="018bf-2900">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="018bf-2901">Befehlszeilenschnittstelle (CLI)</span><span class="sxs-lookup"><span data-stu-id="018bf-2901">CLI</span></span>

* <span data-ttu-id="018bf-2902">Dateieinschränkung in MSI-Installer aktualisiert, um Problem mit der Erweiterungsinstallation zu beheben</span><span class="sxs-lookup"><span data-stu-id="018bf-2902">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="018bf-2903">19. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="018bf-2903">June 19, 2018</span></span>

<span data-ttu-id="018bf-2904">Version 2.0.38</span><span class="sxs-lookup"><span data-stu-id="018bf-2904">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="018bf-2905">Core</span><span class="sxs-lookup"><span data-stu-id="018bf-2905">Core</span></span>

* <span data-ttu-id="018bf-2906">Globale Unterstützung für `--subscription` zu den meisten Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2906">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="018bf-2907">ACR</span><span class="sxs-lookup"><span data-stu-id="018bf-2907">ACR</span></span>

* <span data-ttu-id="018bf-2908">`azure-storage-blob` als Abhängigkeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2908">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="018bf-2909">CPU-Standardkonfiguration für `acr build-task create` geändert, sodass zwei Kerne verwendet werden</span><span class="sxs-lookup"><span data-stu-id="018bf-2909">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="018bf-2910">ACS</span><span class="sxs-lookup"><span data-stu-id="018bf-2910">ACS</span></span>

* <span data-ttu-id="018bf-2911">Optionen des Befehls `aks use-dev-spaces` wurden aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="018bf-2911">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="018bf-2912">Unterstützung für `--update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2912">Added `--update` support</span></span>
* <span data-ttu-id="018bf-2913">`aks get-credentials --admin` geändert, sodass der Benutzerkontext in `$HOME/.kube/config` ersetzt wird</span><span class="sxs-lookup"><span data-stu-id="018bf-2913">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="018bf-2914">Schreibgeschützte `nodeResourceGroup`-Eigenschaft in verwalteten Clustern verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="018bf-2914">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="018bf-2915">Befehlsfehler `acs browse` korrigiert</span><span class="sxs-lookup"><span data-stu-id="018bf-2915">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="018bf-2916">`--connector-name` für `aks install-connector`, `aks upgrade-connector` und `aks remove-connector` als optional festgelegt</span><span class="sxs-lookup"><span data-stu-id="018bf-2916">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="018bf-2917">Neue Azure Container Instances-Regionen für `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2917">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="018bf-2918">Normalisierter Speicherort im Helm-Versionsnamen und Knotenname zu `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2918">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="018bf-2919">AppService</span><span class="sxs-lookup"><span data-stu-id="018bf-2919">AppService</span></span>

* <span data-ttu-id="018bf-2920">Unterstützung für neuere Versionen von „urllib“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2920">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="018bf-2921">Unterstützung der Verwendung eines App Service-Plans aus externen Ressourcengruppen zu `functionapp create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2921">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="018bf-2922">Batch</span><span class="sxs-lookup"><span data-stu-id="018bf-2922">Batch</span></span>

* <span data-ttu-id="018bf-2923">`azure-batch-extensions`-Abhängigkeit entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-2923">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="018bf-2924">Batch KI</span><span class="sxs-lookup"><span data-stu-id="018bf-2924">Batch AI</span></span>

* <span data-ttu-id="018bf-2925">Unterstützung für Arbeitsbereiche wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-2925">Added support for workspaces.</span></span> <span data-ttu-id="018bf-2926">Arbeitsbereiche ermöglichen das Zusammenfassen von Clustern, Dateiservern und Experimenten in Gruppen ohne Beschränkung der Anzahl von Ressourcen, die erstellt werden können.</span><span class="sxs-lookup"><span data-stu-id="018bf-2926">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="018bf-2927">Unterstützung für Experimente wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-2927">Added support for experiments.</span></span> <span data-ttu-id="018bf-2928">Experimente ermöglichen das Zusammenfassen von Aufträgen in Sammlungen ohne Beschränkung der Anzahl von erstellten Aufträgen.</span><span class="sxs-lookup"><span data-stu-id="018bf-2928">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="018bf-2929">Unterstützung für das Konfigurieren von `/dev/shm` für Aufträge hinzugefügt, die in einem Docker-Container ausgeführt werden</span><span class="sxs-lookup"><span data-stu-id="018bf-2929">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="018bf-2930">Die Befehle `batchai cluster node exec` und `batchai job node exec` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-2930">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="018bf-2931">Diese Befehle ermöglichen die Ausführung aller Befehle direkt auf Knoten und bieten Funktionen zur Portweiterleitung.</span><span class="sxs-lookup"><span data-stu-id="018bf-2931">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="018bf-2932">Unterstützung für `--ids` zu `batchai`-Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2932">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="018bf-2933">[BREAKING CHANGE] Alle Cluster und Dateiserver müssen unter Arbeitsbereichen erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="018bf-2933">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="018bf-2934">[BREAKING CHANGE] Aufträge müssen unter Experimenten erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="018bf-2934">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="018bf-2935">[BREAKING CHANGE]`--nfs-resource-group` wurde aus den Befehlen `cluster create` und `job create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="018bf-2935">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="018bf-2936">Geben Sie zum Bereitstellen eines NFS, das einem anderen Arbeitsbereich/einer anderen Ressourcengruppe angehört, die ARM-ID des Dateiservers über die Option `--nfs` an.</span><span class="sxs-lookup"><span data-stu-id="018bf-2936">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="018bf-2937">[BREAKING CHANGE]`--cluster-resource-group` wurde aus dem Befehl `job create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="018bf-2937">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="018bf-2938">Geben Sie zum Übermitteln eines Auftrags, der einem anderen Arbeitsbereich/einer anderen Ressourcengruppe angehört, die ARM-ID des Clusters über die Option `--cluster` an.</span><span class="sxs-lookup"><span data-stu-id="018bf-2938">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="018bf-2939">[BREAKING CHANGE] Attribut `location` wurde aus Aufträgen, Clustern und Dateiservern entfernt.</span><span class="sxs-lookup"><span data-stu-id="018bf-2939">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="018bf-2940">„Location“ ist jetzt ein Attribut eines Arbeitsbereichs.</span><span class="sxs-lookup"><span data-stu-id="018bf-2940">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="018bf-2941">[BREAKING CHANGE]`--location` wurde aus den Befehlen `job create`, `cluster create` und `file-server create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="018bf-2941">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="018bf-2942">[BREAKING CHANGE] Namen von Kurzoptionen wurden geändert, um die Schnittstelle konsistenter zu machen:</span><span class="sxs-lookup"><span data-stu-id="018bf-2942">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="018bf-2943">[`--config`, `-c`] in [`--config-file`, `-f`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="018bf-2943">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="018bf-2944">[`--cluster`, `-r`] in [`--cluster`, `-c`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="018bf-2944">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="018bf-2945">[`--cluster`, `-n`] in [`--cluster`, `-c`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="018bf-2945">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="018bf-2946">[`--job`, `-n`] in [`--job`, `-j`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="018bf-2946">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="018bf-2947">Karten</span><span class="sxs-lookup"><span data-stu-id="018bf-2947">Maps</span></span>

* <span data-ttu-id="018bf-2948">[BREAKING CHANGE]`maps account create` wurde so geändert, dass Nutzungsbedingungen entweder durch interaktive Eingabeaufforderung oder `--accept-tos`-Flag akzeptiert werden müssen.</span><span class="sxs-lookup"><span data-stu-id="018bf-2948">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="018bf-2949">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="018bf-2949">Network</span></span>

* <span data-ttu-id="018bf-2950">Unterstützung für `https` zu `network lb probe create` hinzugefügt [Nr. 6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="018bf-2950">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="018bf-2951">Problem behoben, aufgrund dessen die Groß-/Kleinschreibung von `--endpoint-status` berücksichtigt wurde.</span><span class="sxs-lookup"><span data-stu-id="018bf-2951">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="018bf-2952">#6502</span><span class="sxs-lookup"><span data-stu-id="018bf-2952">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="018bf-2953">Reservations</span><span class="sxs-lookup"><span data-stu-id="018bf-2953">Reservations</span></span>

* <span data-ttu-id="018bf-2954">[BREAKING CHANGE] Erforderlicher Parameter `ReservedResourceType` zu `reservations catalog show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2954">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="018bf-2955">Parameter `Location` zu `reservations catalog show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2955">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="018bf-2956">[BREAKING CHANGE]`kind` aus `ReservationProperties` entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-2956">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="018bf-2957">[BREAKING CHANGE]`capabilities` wurde in `Catalog` in `sku_properties` umbenannt</span><span class="sxs-lookup"><span data-stu-id="018bf-2957">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="018bf-2958">[BREAKING CHANGE] Eigenschaften `size` und `tier` aus `Catalog` entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-2958">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="018bf-2959">Parameter `InstanceFlexibility` zu `reservations reservation update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2959">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="018bf-2960">Role</span><span class="sxs-lookup"><span data-stu-id="018bf-2960">Role</span></span>

* <span data-ttu-id="018bf-2961">Fehlerbehandlung verbessert</span><span class="sxs-lookup"><span data-stu-id="018bf-2961">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="018bf-2962">SQL</span><span class="sxs-lookup"><span data-stu-id="018bf-2962">SQL</span></span>

* <span data-ttu-id="018bf-2963">Verwirrender Fehler behoben, der beim Ausführen von `az sql db list-editions` für einen Ort auftrat, der für Ihr Abonnement nicht verfügbar ist</span><span class="sxs-lookup"><span data-stu-id="018bf-2963">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="018bf-2964">Storage</span><span class="sxs-lookup"><span data-stu-id="018bf-2964">Storage</span></span>

* <span data-ttu-id="018bf-2965">Lesbarkeit der Tabellenausgabe für `storage blob download` verbessert</span><span class="sxs-lookup"><span data-stu-id="018bf-2965">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="018bf-2966">VM</span><span class="sxs-lookup"><span data-stu-id="018bf-2966">VM</span></span>

* <span data-ttu-id="018bf-2967">Verbesserte Einschränkung der VM-Größenüberprüfung für Unterstützung von beschleunigten Netzwerken in `vm create`</span><span class="sxs-lookup"><span data-stu-id="018bf-2967">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="018bf-2968">Warnung für `vmss create` hinzugefügt, dass die VM-Standardgröße von `Standard_D1_v2` auf `Standard_DS1_v2` umgestellt wird</span><span class="sxs-lookup"><span data-stu-id="018bf-2968">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="018bf-2969">`--force-update` zu `[vm|vmss] extension set` hinzugefügt, um die Erweiterung auch dann zu aktualisieren, wenn die Konfiguration nicht geändert wurde</span><span class="sxs-lookup"><span data-stu-id="018bf-2969">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="018bf-2970">13. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="018bf-2970">June 13, 2018</span></span>

<span data-ttu-id="018bf-2971">Version 2.0.37</span><span class="sxs-lookup"><span data-stu-id="018bf-2971">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="018bf-2972">Core</span><span class="sxs-lookup"><span data-stu-id="018bf-2972">Core</span></span>

* <span data-ttu-id="018bf-2973">Verbesserte interaktive Telemetrie</span><span class="sxs-lookup"><span data-stu-id="018bf-2973">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="018bf-2974">13. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="018bf-2974">June 13, 2018</span></span>

<span data-ttu-id="018bf-2975">Version 2.0.36</span><span class="sxs-lookup"><span data-stu-id="018bf-2975">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="018bf-2976">AKS</span><span class="sxs-lookup"><span data-stu-id="018bf-2976">AKS</span></span>

* <span data-ttu-id="018bf-2977">Zusätzliche erweiterte Netzwerkoptionen zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2977">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="018bf-2978">Argumente zu `aks create` zum Aktivieren der Überwachung und HTTP-Routing hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2978">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="018bf-2979">Argument `--no-ssh-key` zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2979">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="018bf-2980">Argument `--enable-rbac` zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2980">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="018bf-2981">[VORSCHAUVERSION] Unterstützung für Azure Active Directory-Authentifizierung zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2981">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="018bf-2982">AppService</span><span class="sxs-lookup"><span data-stu-id="018bf-2982">AppService</span></span>

* <span data-ttu-id="018bf-2983">Problem mit inkompatiblen urllib-Versionen behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-2983">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="018bf-2984">5\. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="018bf-2984">June 5, 2018</span></span>

<span data-ttu-id="018bf-2985">Version 2.0.35</span><span class="sxs-lookup"><span data-stu-id="018bf-2985">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="018bf-2986">Interactive</span><span class="sxs-lookup"><span data-stu-id="018bf-2986">Interactive</span></span>

* <span data-ttu-id="018bf-2987">Grenzwerte für die Abhängigkeiten des interaktiven Modus hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2987">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="018bf-2988">5\. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="018bf-2988">June 5, 2018</span></span>

<span data-ttu-id="018bf-2989">Version 2.0.34</span><span class="sxs-lookup"><span data-stu-id="018bf-2989">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="018bf-2990">Core</span><span class="sxs-lookup"><span data-stu-id="018bf-2990">Core</span></span>

* <span data-ttu-id="018bf-2991">Unterstützung für mandantenübergreifende Ressourcenverweise hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2991">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="018bf-2992">Verbesserte Zuverlässigkeit bei Telemetrieuploads</span><span class="sxs-lookup"><span data-stu-id="018bf-2992">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="018bf-2993">ACR</span><span class="sxs-lookup"><span data-stu-id="018bf-2993">ACR</span></span>

* <span data-ttu-id="018bf-2994">Unterstützung für VSTS als Remotequellort hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2994">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="018bf-2995">Befehl `acr import` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-2995">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="018bf-2996">AKS</span><span class="sxs-lookup"><span data-stu-id="018bf-2996">AKS</span></span>

* <span data-ttu-id="018bf-2997">`aks get-credentials` wurde geändert, um die Kube-Konfigurationsdatei mit sichereren Dateisystemberechtigungen zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="018bf-2997">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="018bf-2998">Batch</span><span class="sxs-lookup"><span data-stu-id="018bf-2998">Batch</span></span>

* <span data-ttu-id="018bf-2999">Fehler bei der Formatierung der Poollistentabelle behoben [[Problem 4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="018bf-2999">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="018bf-3000">IoT</span><span class="sxs-lookup"><span data-stu-id="018bf-3000">IOT</span></span>

* <span data-ttu-id="018bf-3001">Unterstützung für das Erstellen von IoT Hub-Instanzen im Tarif „Basic“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3001">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="018bf-3002">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="018bf-3002">Network</span></span>

* <span data-ttu-id="018bf-3003">`network vnet peering` wurde verbessert.</span><span class="sxs-lookup"><span data-stu-id="018bf-3003">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="018bf-3004">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="018bf-3004">Policy Insights</span></span>

* <span data-ttu-id="018bf-3005">Erstrelease</span><span class="sxs-lookup"><span data-stu-id="018bf-3005">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="018bf-3006">ARM</span><span class="sxs-lookup"><span data-stu-id="018bf-3006">ARM</span></span>

* <span data-ttu-id="018bf-3007">Befehle vom Typ `account management-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3007">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="018bf-3008">SQL</span><span class="sxs-lookup"><span data-stu-id="018bf-3008">SQL</span></span>

* <span data-ttu-id="018bf-3009">Neue Befehle für verwaltete Instanzen hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="018bf-3009">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="018bf-3010">Neue Befehle für verwaltete Datenbanken hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="018bf-3010">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="018bf-3011">Storage</span><span class="sxs-lookup"><span data-stu-id="018bf-3011">Storage</span></span>

* <span data-ttu-id="018bf-3012">Zusätzliche MimeTypes für JSON und JavaScript hinzugefügt (abzuleiten aus Dateierweiterungen)</span><span class="sxs-lookup"><span data-stu-id="018bf-3012">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="018bf-3013">VM</span><span class="sxs-lookup"><span data-stu-id="018bf-3013">VM</span></span>

* <span data-ttu-id="018bf-3014">`vm list-skus` wurde geändert, um feste Spalten zu verwenden und eine Warnung hinzuzufügen, dass `Tier` und `Size` entfernt werden.</span><span class="sxs-lookup"><span data-stu-id="018bf-3014">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="018bf-3015">Option `--accelerated-networking` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3015">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="018bf-3016">`--tags` zu `identity create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3016">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="018bf-3017">22. Mai 2018</span><span class="sxs-lookup"><span data-stu-id="018bf-3017">May 22, 2018</span></span>

<span data-ttu-id="018bf-3018">Version 2.0.33</span><span class="sxs-lookup"><span data-stu-id="018bf-3018">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="018bf-3019">Core</span><span class="sxs-lookup"><span data-stu-id="018bf-3019">Core</span></span>

* <span data-ttu-id="018bf-3020">Unterstützung für das Erweitern von `@` in Dateinamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3020">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="018bf-3021">ACS</span><span class="sxs-lookup"><span data-stu-id="018bf-3021">ACS</span></span>

* <span data-ttu-id="018bf-3022">Neue Dev Spaces-Befehle `aks use-dev-spaces` und `aks remove-dev-spaces` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3022">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="018bf-3023">Tippfehler in Hilfemeldung korrigiert</span><span class="sxs-lookup"><span data-stu-id="018bf-3023">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="018bf-3024">AppService</span><span class="sxs-lookup"><span data-stu-id="018bf-3024">AppService</span></span>

* <span data-ttu-id="018bf-3025">Verbesserte generische Aktualisierungsbefehle</span><span class="sxs-lookup"><span data-stu-id="018bf-3025">Improved generic update commands</span></span>
* <span data-ttu-id="018bf-3026">Asynchrone Unterstützung für `webapp deployment source config-zip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3026">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="018bf-3027">Container</span><span class="sxs-lookup"><span data-stu-id="018bf-3027">Container</span></span>

* <span data-ttu-id="018bf-3028">Unterstützung für das Exportieren einer Containergruppe im YAML-Format hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3028">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="018bf-3029">Unterstützung für die Verwendung einer YAML-Datei zum Erstellen/Aktualisieren einer Containergruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3029">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="018bf-3030">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="018bf-3030">Extension</span></span>

* <span data-ttu-id="018bf-3031">Verbesserte Entfernung von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="018bf-3031">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="018bf-3032">Interactive</span><span class="sxs-lookup"><span data-stu-id="018bf-3032">Interactive</span></span>

* <span data-ttu-id="018bf-3033">Protokollierung geändert, um Parser für Abschlüsse zu deaktivieren</span><span class="sxs-lookup"><span data-stu-id="018bf-3033">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="018bf-3034">Verbesserte Verarbeitung beschädigter Hilfscaches</span><span class="sxs-lookup"><span data-stu-id="018bf-3034">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="018bf-3035">KeyVault</span><span class="sxs-lookup"><span data-stu-id="018bf-3035">KeyVault</span></span>

* <span data-ttu-id="018bf-3036">keyvault-Befehle wurden korrigiert, damit sie in Cloud Shell oder auf virtuellen Computern mit Identität verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="018bf-3036">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="018bf-3037">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="018bf-3037">Network</span></span>

* <span data-ttu-id="018bf-3038">Problem behoben, aufgrund dessen `network watcher show-topology` nicht mit einem VNET und/oder Subnetznamen verwendet werden konnte ([#6326](https://github.com/Azure/azure-cli/issues/6326))</span><span class="sxs-lookup"><span data-stu-id="018bf-3038">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="018bf-3039">Problem behoben, aufgrund dessen einige `network watcher`-Befehle fälschlicherweise angaben, dass Network Watcher nicht für bestimmte Regionen aktiviert ist ([#6264](https://github.com/Azure/azure-cli/issues/6264))</span><span class="sxs-lookup"><span data-stu-id="018bf-3039">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="018bf-3040">SQL</span><span class="sxs-lookup"><span data-stu-id="018bf-3040">SQL</span></span>

* <span data-ttu-id="018bf-3041">[BREAKING CHANGE] Von den Befehlen `db` und `dw` zurückgegebene Antwortobjekte geändert:</span><span class="sxs-lookup"><span data-stu-id="018bf-3041">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="018bf-3042">Eigenschaft `serviceLevelObjective` in `currentServiceObjectiveName` umbenannt</span><span class="sxs-lookup"><span data-stu-id="018bf-3042">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="018bf-3043">Eigenschaften `currentServiceObjectiveId` und `requestedServiceObjectiveId` entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-3043">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="018bf-3044">Eigenschaft `maxSizeBytes` geändert (ist nun keine Zeichenfolge mehr, sondern ein Ganzzahlwert)</span><span class="sxs-lookup"><span data-stu-id="018bf-3044">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="018bf-3045">[BREAKING CHANGE] Die folgenden `db`- und `dw`-Eigenschaften wurden geändert und sind jetzt schreibgeschützt:</span><span class="sxs-lookup"><span data-stu-id="018bf-3045">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="018bf-3046">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="018bf-3046">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="018bf-3047">Verwenden Sie zum Aktualisieren den Parameter `--service-objective`, oder legen Sie die Eigenschaft `sku.name` fest.</span><span class="sxs-lookup"><span data-stu-id="018bf-3047">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="018bf-3048">`edition`.</span><span class="sxs-lookup"><span data-stu-id="018bf-3048">`edition`.</span></span> <span data-ttu-id="018bf-3049">Verwenden Sie zum Aktualisieren den Parameter `--edition`, oder legen Sie die Eigenschaft `sku.tier` fest.</span><span class="sxs-lookup"><span data-stu-id="018bf-3049">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="018bf-3050">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="018bf-3050">`elasticPoolName`.</span></span> <span data-ttu-id="018bf-3051">Verwenden Sie zum Aktualisieren den Parameter `--elastic-pool`, oder legen Sie die Eigenschaft `elasticPoolId` fest.</span><span class="sxs-lookup"><span data-stu-id="018bf-3051">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="018bf-3052">[BREAKING CHANGE] Die folgenden `elastic-pool`-Eigenschaften wurden geändert und sind jetzt schreibgeschützt:</span><span class="sxs-lookup"><span data-stu-id="018bf-3052">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="018bf-3053">`edition`.</span><span class="sxs-lookup"><span data-stu-id="018bf-3053">`edition`.</span></span> <span data-ttu-id="018bf-3054">Verwenden Sie zum Aktualisieren den Parameter `--edition`.</span><span class="sxs-lookup"><span data-stu-id="018bf-3054">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="018bf-3055">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="018bf-3055">`dtu`.</span></span> <span data-ttu-id="018bf-3056">Verwenden Sie zum Aktualisieren den Parameter `--capacity`.</span><span class="sxs-lookup"><span data-stu-id="018bf-3056">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="018bf-3057">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="018bf-3057">`databaseDtuMin`.</span></span> <span data-ttu-id="018bf-3058">Verwenden Sie zum Aktualisieren den Parameter `--db-min-capacity`.</span><span class="sxs-lookup"><span data-stu-id="018bf-3058">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="018bf-3059">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="018bf-3059">`databaseDtuMax`.</span></span> <span data-ttu-id="018bf-3060">Verwenden Sie zum Aktualisieren den Parameter `--db-max-capacity`.</span><span class="sxs-lookup"><span data-stu-id="018bf-3060">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="018bf-3061">Die Parameter `--family` und `--capacity` wurden zu den `db`-, `dw`- und `elastic-pool`-Befehlen hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-3061">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="018bf-3062">Den `db`-, `dw`- und `elastic-pool`-Befehlen wurden Tabellenformatierer hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-3062">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="018bf-3063">Storage</span><span class="sxs-lookup"><span data-stu-id="018bf-3063">Storage</span></span>

* <span data-ttu-id="018bf-3064">Vervollständigung für das Argument `--account-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3064">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="018bf-3065">Problem mit `storage entity query` behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-3065">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="018bf-3066">VM</span><span class="sxs-lookup"><span data-stu-id="018bf-3066">VM</span></span>

* <span data-ttu-id="018bf-3067">[BREAKING CHANGE]`--write-accelerator` aus `vm create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="018bf-3067">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="018bf-3068">Die gleiche Unterstützung kann über `vm update` oder `vm disk attach` erzielt werden.</span><span class="sxs-lookup"><span data-stu-id="018bf-3068">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="018bf-3069">Erweiterungsimageabgleich in `[vm|vmss] extension` korrigiert</span><span class="sxs-lookup"><span data-stu-id="018bf-3069">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="018bf-3070">`--boot-diagnostics-storage` zu `vm create` zur Erfassung des Startprotokolls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3070">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="018bf-3071">`--license-type` zu `[vm|vmss] update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3071">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="018bf-3072">7\. Mai 2018</span><span class="sxs-lookup"><span data-stu-id="018bf-3072">May 7, 2018</span></span>

<span data-ttu-id="018bf-3073">Version 2.0.32</span><span class="sxs-lookup"><span data-stu-id="018bf-3073">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="018bf-3074">Core</span><span class="sxs-lookup"><span data-stu-id="018bf-3074">Core</span></span>

* <span data-ttu-id="018bf-3075">Ein Ausnahmefehler wurde behoben, der beim Abrufen von Geheimnissen aus einem Dienstprinzipalkonto mit Zertifikat auftrat.</span><span class="sxs-lookup"><span data-stu-id="018bf-3075">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="018bf-3076">Eingeschränkte Unterstützung für positionelle Argumente hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3076">Added limited support for positional arguments</span></span>
* <span data-ttu-id="018bf-3077">Problem behoben, aufgrund dessen `--query` nicht mit `--ids` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="018bf-3077">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="018bf-3078">#5591</span><span class="sxs-lookup"><span data-stu-id="018bf-3078">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="018bf-3079">Pipingszenarien von Befehlen bei Verwendung von `--ids` verbessert</span><span class="sxs-lookup"><span data-stu-id="018bf-3079">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="018bf-3080">Unterstützt `-o tsv` mit angegebener Abfrage bzw. `-o json` ohne angegeben Abfrage</span><span class="sxs-lookup"><span data-stu-id="018bf-3080">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="018bf-3081">Befehlsvorschläge bei Fehler hinzugefügt, wenn Befehle Tippfehler enthielten</span><span class="sxs-lookup"><span data-stu-id="018bf-3081">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="018bf-3082">Fehler bei der Eingabe von `az ''` behandelt</span><span class="sxs-lookup"><span data-stu-id="018bf-3082">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="018bf-3083">Unterstützung für benutzerdefinierte Ressourcentypen für Befehlsmodule und -erweiterungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3083">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="018bf-3084">ACR</span><span class="sxs-lookup"><span data-stu-id="018bf-3084">ACR</span></span>

* <span data-ttu-id="018bf-3085">ACR Build-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3085">Added ACR Build commands</span></span>
* <span data-ttu-id="018bf-3086">Fehlermeldungen vom Typ „Ressource nicht gefunden.“ verbessert</span><span class="sxs-lookup"><span data-stu-id="018bf-3086">Improved resource not found error messages</span></span>
* <span data-ttu-id="018bf-3087">Höhere Leistung bei der Ressourcenerstellung und optimierte Fehlerbehandlung</span><span class="sxs-lookup"><span data-stu-id="018bf-3087">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="018bf-3088">ACR-Anmeldung bei nicht standardmäßigen Konsolen und WSL optimiert</span><span class="sxs-lookup"><span data-stu-id="018bf-3088">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="018bf-3089">Fehlermeldungen zu Repositorybefehlen optimiert</span><span class="sxs-lookup"><span data-stu-id="018bf-3089">Improved repository commands error messages</span></span>
* <span data-ttu-id="018bf-3090">Tabellenspalten und -reihenfolge aktualisiert</span><span class="sxs-lookup"><span data-stu-id="018bf-3090">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="018bf-3091">ACS</span><span class="sxs-lookup"><span data-stu-id="018bf-3091">ACS</span></span>

* <span data-ttu-id="018bf-3092">Warnung hinzugefügt, dass `az aks` eine Vorschauversion des Diensts ist</span><span class="sxs-lookup"><span data-stu-id="018bf-3092">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="018bf-3093">Berechtigungsproblem in `aks install-connector` behoben, wenn `--aci-resource-group` nicht angegeben wird</span><span class="sxs-lookup"><span data-stu-id="018bf-3093">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="018bf-3094">AMS</span><span class="sxs-lookup"><span data-stu-id="018bf-3094">AMS</span></span>

* <span data-ttu-id="018bf-3095">Erste Version: Verwalten von Azure Media Services-Ressourcen</span><span class="sxs-lookup"><span data-stu-id="018bf-3095">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="018bf-3096">AppService</span><span class="sxs-lookup"><span data-stu-id="018bf-3096">Appservice</span></span>

* <span data-ttu-id="018bf-3097">Ein Problem in `webapp delete` wurde behoben, das bei Angabe von `--slot` auftrat.</span><span class="sxs-lookup"><span data-stu-id="018bf-3097">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="018bf-3098">`--runtime-version` aus `webapp auth update` entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-3098">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="018bf-3099">Unterstützung für „min\_tls\_version“ und „https2.0“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3099">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="018bf-3100">Unterstützung für mehrere Container hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3100">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="018bf-3101">Batch KI</span><span class="sxs-lookup"><span data-stu-id="018bf-3101">Batch AI</span></span>

* <span data-ttu-id="018bf-3102">`batchai create cluster` wurde geändert, um die in der Konfigurationsdatei des Clusters konfigurierte VM-Priorität zu berücksichtigen.</span><span class="sxs-lookup"><span data-stu-id="018bf-3102">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="018bf-3103">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="018bf-3103">Cognitive Services</span></span>

* <span data-ttu-id="018bf-3104">Tippfehler im Beispiel für `cognitiveservices account create` behoben [Nr. 5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="018bf-3104">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="018bf-3105">Nutzung</span><span class="sxs-lookup"><span data-stu-id="018bf-3105">Consumption</span></span>

* <span data-ttu-id="018bf-3106">Neue Befehle für Budget-API hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3106">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="018bf-3107">Container</span><span class="sxs-lookup"><span data-stu-id="018bf-3107">Container</span></span>

* <span data-ttu-id="018bf-3108">`--registry-server` muss nicht mehr für `container create` angegeben werden, wenn ein Registrierungsserver im Imagenamen enthalten ist.</span><span class="sxs-lookup"><span data-stu-id="018bf-3108">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="018bf-3109">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="018bf-3109">Cosmos DB</span></span>

* <span data-ttu-id="018bf-3110">VNET-Unterstützung für Azure CLI eingeführt: Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="018bf-3110">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="018bf-3111">DMS</span><span class="sxs-lookup"><span data-stu-id="018bf-3111">DMS</span></span>

* <span data-ttu-id="018bf-3112">Erste Version: Die Migration von SQL zu Azure SQL wird nun unterstützt.</span><span class="sxs-lookup"><span data-stu-id="018bf-3112">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="018bf-3113">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="018bf-3113">Extension</span></span>

* <span data-ttu-id="018bf-3114">Fehler behoben, aufgrund dessen Erweiterungsmetadaten nicht mehr angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="018bf-3114">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="018bf-3115">Interactive</span><span class="sxs-lookup"><span data-stu-id="018bf-3115">Interactive</span></span>

* <span data-ttu-id="018bf-3116">Interaktive Vervollständigung funktioniert nun auch mit positionellen Argumenten.</span><span class="sxs-lookup"><span data-stu-id="018bf-3116">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="018bf-3117">Benutzerfreundlichere Ausgabe bei der Eingabe von '\'</span><span class="sxs-lookup"><span data-stu-id="018bf-3117">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="018bf-3118">Abschlüsse für Parameter ohne Hilfe korrigiert</span><span class="sxs-lookup"><span data-stu-id="018bf-3118">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="018bf-3119">Beschreibungen für Befehlsgruppen korrigiert</span><span class="sxs-lookup"><span data-stu-id="018bf-3119">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="018bf-3120">Labor</span><span class="sxs-lookup"><span data-stu-id="018bf-3120">Lab</span></span>

* <span data-ttu-id="018bf-3121">Regressionen aus Knack-Umwandlung korrigiert</span><span class="sxs-lookup"><span data-stu-id="018bf-3121">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="018bf-3122">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="018bf-3122">Network</span></span>

* <span data-ttu-id="018bf-3123">[BREAKING CHANGE] Parameter `--ids` entfernt für:</span><span class="sxs-lookup"><span data-stu-id="018bf-3123">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="018bf-3124">Profil</span><span class="sxs-lookup"><span data-stu-id="018bf-3124">Profile</span></span>

* <span data-ttu-id="018bf-3125">Quellerkennung für `disk create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="018bf-3125">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="018bf-3126">[BREAKING CHANGE]`--msi-port` und `--identity-port` entfernt, da sie nicht mehr verwendet werden</span><span class="sxs-lookup"><span data-stu-id="018bf-3126">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="018bf-3127">Tippfehler in kurzer Zusammenfassung für `account get-access-token` korrigiert</span><span class="sxs-lookup"><span data-stu-id="018bf-3127">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="018bf-3128">Redis</span><span class="sxs-lookup"><span data-stu-id="018bf-3128">Redis</span></span>

* <span data-ttu-id="018bf-3129">`redis patch-schedule patch-schedule show` wurde durch `redis patch-schedule show` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="018bf-3129">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="018bf-3130">`redis list-all` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="018bf-3130">Deprecated `redis list-all`.</span></span> <span data-ttu-id="018bf-3131">Diese Funktion wurde in `redis list` integriert.</span><span class="sxs-lookup"><span data-stu-id="018bf-3131">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="018bf-3132">`redis import-method` wurde durch `redis import` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="018bf-3132">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="018bf-3133">Unterstützung für `--ids` zu verschiedenen Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3133">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="018bf-3134">Role</span><span class="sxs-lookup"><span data-stu-id="018bf-3134">Role</span></span>

* <span data-ttu-id="018bf-3135">[BREAKING CHANGE] Veralteter Befehl `ad sp reset-credentials` entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-3135">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="018bf-3136">Storage</span><span class="sxs-lookup"><span data-stu-id="018bf-3136">Storage</span></span>

* <span data-ttu-id="018bf-3137">Zulassen, dass das Ziel-SAS-Token für die Blobkopie auf die Quelle angewendet wird, wenn Quell-SAS und Kontoschlüssel nicht angegeben werden</span><span class="sxs-lookup"><span data-stu-id="018bf-3137">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="018bf-3138">Verfügbar gemacht: Socket-Timeout für Blobuploads und -downloads</span><span class="sxs-lookup"><span data-stu-id="018bf-3138">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="018bf-3139">Blobnamen, die mit Pfadtrennzeichen beginnen, als relative Pfade behandeln</span><span class="sxs-lookup"><span data-stu-id="018bf-3139">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="018bf-3140">Zulassen, dass `storage blob copy --source-sas` mit dem Abfragezeichen „?“ beginnt</span><span class="sxs-lookup"><span data-stu-id="018bf-3140">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="018bf-3141">`storage entity query --marker` korrigiert, um Liste von Schlüsselwerten zu akzeptieren</span><span class="sxs-lookup"><span data-stu-id="018bf-3141">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="018bf-3142">VM</span><span class="sxs-lookup"><span data-stu-id="018bf-3142">VM</span></span>

* <span data-ttu-id="018bf-3143">Ungültige Erkennungslogik für nicht verwalteten Blob-URI korrigiert</span><span class="sxs-lookup"><span data-stu-id="018bf-3143">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="018bf-3144">Unterstützung für Datenträgerverschlüsselung ohne vom Benutzer bereitgestellte Dienstprinzipale hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3144">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="018bf-3145">[BREAKING CHANGE] Verwenden Sie nicht „ManagedIdentityExtension“ des virtuellen Computers für MSI-Unterstützung.</span><span class="sxs-lookup"><span data-stu-id="018bf-3145">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="018bf-3146">Unterstützung für Entfernungsrichtlinie zu `vmss` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3146">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="018bf-3147">[BREAKING CHANGE]`--ids` entfernt aus:</span><span class="sxs-lookup"><span data-stu-id="018bf-3147">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="018bf-3148">Unterstützung für Schreibbeschleunigung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3148">Added write accelerator support</span></span>
* <span data-ttu-id="018bf-3149">`vmss perform-maintenance` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3149">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="018bf-3150">`vm diagnostics set` korrigiert, um zuverlässig den Betriebssystemtyp des virtuellen Computers zu erkennen</span><span class="sxs-lookup"><span data-stu-id="018bf-3150">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="018bf-3151">`vm resize` geändert, um zu überprüfen, ob die angeforderte Größe von der derzeit festgelegten Größe abweicht, und nur bei einer Änderung eine Aktualisierung auszuführen</span><span class="sxs-lookup"><span data-stu-id="018bf-3151">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="018bf-3152">10. April 2018</span><span class="sxs-lookup"><span data-stu-id="018bf-3152">April 10, 2018</span></span>

<span data-ttu-id="018bf-3153">Version 2.0.31</span><span class="sxs-lookup"><span data-stu-id="018bf-3153">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="018bf-3154">ACR</span><span class="sxs-lookup"><span data-stu-id="018bf-3154">ACR</span></span>

* <span data-ttu-id="018bf-3155">Verbesserte Fehlerbehandlung für wincred-Fallback</span><span class="sxs-lookup"><span data-stu-id="018bf-3155">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="018bf-3156">ACS</span><span class="sxs-lookup"><span data-stu-id="018bf-3156">ACS</span></span>

* <span data-ttu-id="018bf-3157">Gültigkeit von per AKS erstellten SPNs in fünf Jahre geändert</span><span class="sxs-lookup"><span data-stu-id="018bf-3157">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="018bf-3158">AppService</span><span class="sxs-lookup"><span data-stu-id="018bf-3158">Appservice</span></span>

* [BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="018bf-3160">Nicht abgefangene Ausnahme für nicht vorhandene Web-App-Pläne behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-3160">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="018bf-3161">Batch AI</span><span class="sxs-lookup"><span data-stu-id="018bf-3161">BatchAI</span></span>

* <span data-ttu-id="018bf-3162">Unterstützung für API 2018-03-01 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3162">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="018bf-3163">Bereitstellung auf Auftragsebene</span><span class="sxs-lookup"><span data-stu-id="018bf-3163">Job level mounting</span></span>
  - <span data-ttu-id="018bf-3164">Umgebungsvariablen mit Geheimniswerten</span><span class="sxs-lookup"><span data-stu-id="018bf-3164">Environment variables with secret values</span></span>
  - <span data-ttu-id="018bf-3165">Einstellungen von Leistungsindikatoren</span><span class="sxs-lookup"><span data-stu-id="018bf-3165">Performance counters settings</span></span>
  - <span data-ttu-id="018bf-3166">Berichtstellung für auftragsspezifisches Pfadsegment</span><span class="sxs-lookup"><span data-stu-id="018bf-3166">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="018bf-3167">Unterstützung für Unterordner in Listendateien-API</span><span class="sxs-lookup"><span data-stu-id="018bf-3167">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="018bf-3168">Berichterstellung zur Nutzung und zu Grenzwerten</span><span class="sxs-lookup"><span data-stu-id="018bf-3168">Usage and limits reporting</span></span>
  - <span data-ttu-id="018bf-3169">Zulassen der Angabe des Cachetyps für NFS-Server</span><span class="sxs-lookup"><span data-stu-id="018bf-3169">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="018bf-3170">Unterstützung für benutzerdefinierte Images</span><span class="sxs-lookup"><span data-stu-id="018bf-3170">Support for custom images</span></span>
  - <span data-ttu-id="018bf-3171">Unterstützung für pyTorch-Toolkit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3171">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="018bf-3172">Befehl `job wait` hinzugefügt, der das Warten auf die Auftragsfertigstellung ermöglicht und den Code für die Auftragsbeendigung meldet</span><span class="sxs-lookup"><span data-stu-id="018bf-3172">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="018bf-3173">Befehl `usage show` hinzugefügt, mit dem die aktuelle Nutzung von Batch KI-Ressourcen und die Grenzwerte für verschiedene Regionen aufgelistet werden</span><span class="sxs-lookup"><span data-stu-id="018bf-3173">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="018bf-3174">Nationale Clouds werden unterstützt</span><span class="sxs-lookup"><span data-stu-id="018bf-3174">National clouds are supported</span></span>
* <span data-ttu-id="018bf-3175">Befehlszeilenargumente für Aufträge hinzugefügt, um das Bereitstellen von Dateisystemen auf Auftragsebene zusätzlich zu Konfigurationsdateien zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="018bf-3175">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="018bf-3176">Weitere Optionen zum Anpassen von Clustern hinzugefügt – VM-Priorität, Subnetz, anfängliche Knotenanzahl für Cluster mit automatischer Skalierung, Angeben eines benutzerdefinierten Images</span><span class="sxs-lookup"><span data-stu-id="018bf-3176">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="018bf-3177">Befehlszeilenoption zum Angeben des Cachetyps für NFS mit Verwaltung per Batch KI hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3177">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="018bf-3178">Angeben der Bereitstellung von Dateisystemen in Konfigurationsdateien vereinfacht.</span><span class="sxs-lookup"><span data-stu-id="018bf-3178">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="018bf-3179">Weglassen von Anmeldeinformationen für Azure-Dateifreigaben und Azure-Blobcontainer ist jetzt möglich. Die CLI füllt fehlende Anmeldeinformationen auf, indem der Speicherkontoschlüssel verwendet wird, der über Befehlszeilenparameter oder per Umgebungsvariable angegeben wird, oder der Schlüssel wird über Azure Storage abgefragt (sofern das Speicherkonto zum aktuellen Abonnement gehört).</span><span class="sxs-lookup"><span data-stu-id="018bf-3179">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="018bf-3180">Der Befehl zum Streamen von Auftragsdateien wird jetzt automatisch abgeschlossen, nachdem der Auftrag beendet ist (Erfolg, Fehler, Beendigung oder Löschung)</span><span class="sxs-lookup"><span data-stu-id="018bf-3180">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="018bf-3181">Verbesserte `table`-Ausgabe für `show`-Vorgänge</span><span class="sxs-lookup"><span data-stu-id="018bf-3181">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="018bf-3182">Option `--use-auto-storage` für die Clustererstellung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-3182">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="018bf-3183">Diese Option erleichtert die Verwaltung von Speicherkonten und die Bereitstellung von Azure-Dateifreigaben und Azure-Blobcontainern in Clustern.</span><span class="sxs-lookup"><span data-stu-id="018bf-3183">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="018bf-3184">`--generate-ssh-keys` für `cluster create` und `file-server create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3184">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="018bf-3185">Möglichkeit zum Angeben der Knotensetupaufgabe über die Befehlszeile</span><span class="sxs-lookup"><span data-stu-id="018bf-3185">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="018bf-3186">[BREAKING CHANGE] Befehl `job stream-file` und `job list-files` in die Gruppe `job file` verschoben</span><span class="sxs-lookup"><span data-stu-id="018bf-3186">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="018bf-3187">[BREAKING CHANGE]`--admin-user-name` im Befehl `file-server create` in `--user-name` umbenannt, um Einheitlichkeit mit dem Befehl `cluster create` zu erzielen</span><span class="sxs-lookup"><span data-stu-id="018bf-3187">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="018bf-3188">Abrechnung</span><span class="sxs-lookup"><span data-stu-id="018bf-3188">Billing</span></span>

* <span data-ttu-id="018bf-3189">Registrierungskontobefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3189">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="018bf-3190">Nutzung</span><span class="sxs-lookup"><span data-stu-id="018bf-3190">Consumption</span></span>

* <span data-ttu-id="018bf-3191">Befehle vom Typ `marketplace` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3191">Added `marketplace` commands</span></span>
* <span data-ttu-id="018bf-3192">[BREAKING CHANGE]`reservations summaries` in `reservation summary` umbenannt</span><span class="sxs-lookup"><span data-stu-id="018bf-3192">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="018bf-3193">[BREAKING CHANGE]`reservations details` in `reservation detail` umbenannt</span><span class="sxs-lookup"><span data-stu-id="018bf-3193">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="018bf-3194">[BREAKING CHANGE] Kurzoptionen `--reservation-order-id` und `--reservation-id` für `reservation`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-3194">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="018bf-3195">[BREAKING CHANGE]`--grain`-Kurzoptionen für `reservation summary`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-3195">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="018bf-3196">[BREAKING CHANGE]`--include-meter-details`-Kurzoptionen für `pricesheet`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-3196">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="018bf-3197">Container</span><span class="sxs-lookup"><span data-stu-id="018bf-3197">Container</span></span>

* <span data-ttu-id="018bf-3198">Parameter für die Volumebereitstellung für das Git-Repository hinzugefügt: `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` und `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="018bf-3198">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="018bf-3199">[#5926](https://github.com/Azure/azure-cli/issues/5926) behoben: Fehler bei `az container exec`, wenn „--container-name“ angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="018bf-3199">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="018bf-3200">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="018bf-3200">Extension</span></span>

* <span data-ttu-id="018bf-3201">Meldung für Distributionsüberprüfung in Debugebene geändert</span><span class="sxs-lookup"><span data-stu-id="018bf-3201">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="018bf-3202">Interactive</span><span class="sxs-lookup"><span data-stu-id="018bf-3202">Interactive</span></span>

* <span data-ttu-id="018bf-3203">Geändert: Verhinderung des Abschlusses bei nicht erkannten Befehlen</span><span class="sxs-lookup"><span data-stu-id="018bf-3203">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="018bf-3204">Ereignishooks vor und nach der Erstellung der Teilstruktur von Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3204">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="018bf-3205">Abschluss für `--ids`-Parameter hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3205">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="018bf-3206">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="018bf-3206">Network</span></span>

* <span data-ttu-id="018bf-3207">[#5936](https://github.com/Azure/azure-cli/issues/5936) behoben: `application-gateway create`-Tags konnten nicht festgelegt werden</span><span class="sxs-lookup"><span data-stu-id="018bf-3207">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="018bf-3208">Argument `--auth-certs` zum Anfügen von Authentifizierungszertifikaten für `application-gateway http-settings [create|update]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-3208">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="018bf-3209">#4910</span><span class="sxs-lookup"><span data-stu-id="018bf-3209">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="018bf-3210">`ddos-protection`-Befehle zum Erstellen von DDoS-Schutzplänen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3210">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="018bf-3211">Unterstützung von `--ddos-protection-plan` für `vnet [create|update]` hinzugefügt, um das Zuordnen eines VNET zu einem DDoS-Schutzplan zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="018bf-3211">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="018bf-3212">Problem mit `--disable-bgp-route-propagation`-Flag in `network route-table [create|update]` behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-3212">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="018bf-3213">Dummy-Argumente `--public-ip-address-type` und `--subnet-type` für `network lb [create|update]` entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-3213">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="018bf-3214">Unterstützung für TXT-Datensätze mit RFC 1035-Escapesequenzen für `network dns zone [import|export]` und `network dns record-set txt add-record` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3214">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="018bf-3215">Profil</span><span class="sxs-lookup"><span data-stu-id="018bf-3215">Profile</span></span>

* <span data-ttu-id="018bf-3216">Unterstützung für klassische Azure-Konten in `account list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3216">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="018bf-3217">[BREAKING CHANGE]`--msi` & `--msi-port`-Argumente entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-3217">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="018bf-3218">RDBMS</span><span class="sxs-lookup"><span data-stu-id="018bf-3218">RDBMS</span></span>

* <span data-ttu-id="018bf-3219">Befehl `georestore` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3219">Added `georestore` command</span></span>
* <span data-ttu-id="018bf-3220">Speichergrößenbeschränkung aus Befehl `create` entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-3220">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="018bf-3221">Resource</span><span class="sxs-lookup"><span data-stu-id="018bf-3221">Resource</span></span>

* <span data-ttu-id="018bf-3222">Unterstützung für `--metadata` zu `policy definition create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3222">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="018bf-3223">Unterstützung von `--metadata`, `--set`, `--add`, `--remove` für `policy definition update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3223">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="018bf-3224">SQL</span><span class="sxs-lookup"><span data-stu-id="018bf-3224">SQL</span></span>

* <span data-ttu-id="018bf-3225">`sql elastic-pool op list` und `sql elastic-pool op cancel` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3225">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="018bf-3226">Storage</span><span class="sxs-lookup"><span data-stu-id="018bf-3226">Storage</span></span>

* <span data-ttu-id="018bf-3227">Fehlermeldungen für falsch formatierte Verbindungszeichenfolgen verbessert</span><span class="sxs-lookup"><span data-stu-id="018bf-3227">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="018bf-3228">VM</span><span class="sxs-lookup"><span data-stu-id="018bf-3228">VM</span></span>

* <span data-ttu-id="018bf-3229">Unterstützung für die Konfiguration der Plattform-Fehlerdomänenanzahl für `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3229">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="018bf-3230">`vmss create` geändert, damit standardmäßig „Standard LB“ für zonales, großes oder per einzelner Platzierungsgruppe deaktiviertes Scale Set festgelegt wird</span><span class="sxs-lookup"><span data-stu-id="018bf-3230">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret`
* <span data-ttu-id="018bf-3232">Unterstützung für SKU mit öffentlicher IP für `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3232">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="018bf-3233">Argumente `--keyvault` und `--resource-group` für `vm secret format` hinzugefügt, um Szenarien zu unterstützen, bei denen der Befehl die Tresor-ID nicht auflösen kann.</span><span class="sxs-lookup"><span data-stu-id="018bf-3233">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="018bf-3234">#5718</span><span class="sxs-lookup"><span data-stu-id="018bf-3234">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="018bf-3235">Bessere Fehler für `[vm|vmss create]`, wenn der Standort einer Ressourcengruppe keine Zonenunterstützung aufweist</span><span class="sxs-lookup"><span data-stu-id="018bf-3235">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="018bf-3236">27. März 2018</span><span class="sxs-lookup"><span data-stu-id="018bf-3236">March 27, 2018</span></span>

<span data-ttu-id="018bf-3237">Version 2.0.30</span><span class="sxs-lookup"><span data-stu-id="018bf-3237">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="018bf-3238">Core</span><span class="sxs-lookup"><span data-stu-id="018bf-3238">Core</span></span>

* <span data-ttu-id="018bf-3239">Anzeigen einer Meldung für Erweiterungen, die in der Hilfe als Vorschauversion gekennzeichnet sind</span><span class="sxs-lookup"><span data-stu-id="018bf-3239">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="018bf-3240">ACS</span><span class="sxs-lookup"><span data-stu-id="018bf-3240">ACS</span></span>

* <span data-ttu-id="018bf-3241">Behebung eines Fehlers bei der SSL-Zertifikatprüfung für `aks install-cli` in Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="018bf-3241">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="018bf-3242">AppService</span><span class="sxs-lookup"><span data-stu-id="018bf-3242">Appservice</span></span>

* <span data-ttu-id="018bf-3243">Unterstützung nur von HTTPS zu `webapp update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3243">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="018bf-3244">Unterstützung für Slots zu `az webapp identity [assign|show]` und `az functionapp identity [assign|show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3244">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="018bf-3245">Backup</span><span class="sxs-lookup"><span data-stu-id="018bf-3245">Backup</span></span>

* <span data-ttu-id="018bf-3246">Neuer Befehl `az backup protection isenabled-for-vm` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-3246">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="018bf-3247">Mit diesem Befehl kann überprüft werden, ob ein virtueller Computer von einem beliebigen Tresor im Abonnement gesichert wird.</span><span class="sxs-lookup"><span data-stu-id="018bf-3247">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="018bf-3248">Azure-Objekt-IDs für Parameter `--resource-group` und `--vault-name` für die folgenden Befehle aktiviert:</span><span class="sxs-lookup"><span data-stu-id="018bf-3248">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="018bf-3249">`--name`-Parameter wurden geändert, um das Ausgabeformat von `backup ... show`-Befehlen zu akzeptieren.</span><span class="sxs-lookup"><span data-stu-id="018bf-3249">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="018bf-3250">Container</span><span class="sxs-lookup"><span data-stu-id="018bf-3250">Container</span></span>

* <span data-ttu-id="018bf-3251">Befehl `container exec` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-3251">Added `container exec` command.</span></span> <span data-ttu-id="018bf-3252">Ausführung von Befehlen in einem Container für eine ausgeführte Containergruppe</span><span class="sxs-lookup"><span data-stu-id="018bf-3252">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="018bf-3253">Zulassen der Tabellenausgabe zum Erstellen und Aktualisieren einer Containergruppe</span><span class="sxs-lookup"><span data-stu-id="018bf-3253">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="018bf-3254">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="018bf-3254">Extension</span></span>

* <span data-ttu-id="018bf-3255">Meldung für `extension add` hinzugefügt, wenn sich die Erweiterung in der Vorschauphase befindet</span><span class="sxs-lookup"><span data-stu-id="018bf-3255">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="018bf-3256">`extension list-available` geändert, um vollständige Erweiterungsdaten mit `--show-details` anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="018bf-3256">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="018bf-3257">[BREAKING CHANGE]`extension list-available` geändert, um standardmäßig vereinfachte Erweiterungsdaten anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="018bf-3257">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="018bf-3258">Interactive</span><span class="sxs-lookup"><span data-stu-id="018bf-3258">Interactive</span></span>

* <span data-ttu-id="018bf-3259">Vervollständigungen wurden geändert und werden jetzt aktiviert, sobald das Laden der Befehlstabelle abgeschlossen ist.</span><span class="sxs-lookup"><span data-stu-id="018bf-3259">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="018bf-3260">Fehler bei der Verwendung des Parameters `--style` behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-3260">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="018bf-3261">Interaktiver Lexer nach Befehlstabellensicherung instanziiert (sofern nicht vorhanden)</span><span class="sxs-lookup"><span data-stu-id="018bf-3261">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="018bf-3262">Verbesserte Unterstützung der Vervollständigung</span><span class="sxs-lookup"><span data-stu-id="018bf-3262">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="018bf-3263">Labor</span><span class="sxs-lookup"><span data-stu-id="018bf-3263">Lab</span></span>

* <span data-ttu-id="018bf-3264">Probleme mit Befehl `create environment` behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-3264">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="018bf-3265">Überwachen</span><span class="sxs-lookup"><span data-stu-id="018bf-3265">Monitor</span></span>

* <span data-ttu-id="018bf-3266">Unterstützung für `--top`, `--orderby` und `--namespace` zu `metrics list` hinzugefügt [Nr. 5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="018bf-3266">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="018bf-3267">[#4529](https://github.com/Azure/azure-cli/issues/5785) behoben: `metrics list` akzeptiert eine durch Leerzeichen getrennte Liste von abzurufenden Metriken</span><span class="sxs-lookup"><span data-stu-id="018bf-3267">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="018bf-3268">Unterstützung für `--namespace` zu `metrics list-definitions` hinzugefügt [Nr. 5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="018bf-3268">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="018bf-3269">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="018bf-3269">Network</span></span>

* <span data-ttu-id="018bf-3270">Unterstützung für private DNS-Zonen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3270">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="018bf-3271">Profil</span><span class="sxs-lookup"><span data-stu-id="018bf-3271">Profile</span></span>

* <span data-ttu-id="018bf-3272">Warnung für `--identity-port` und `--msi-port` zu `login` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3272">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="018bf-3273">RDBMS</span><span class="sxs-lookup"><span data-stu-id="018bf-3273">RDBMS</span></span>

* <span data-ttu-id="018bf-3274">GA-API-Version 2017-12-01 (Geschäftsmodell) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3274">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="018bf-3275">Resource</span><span class="sxs-lookup"><span data-stu-id="018bf-3275">Resource</span></span>

* [BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="018bf-3277">Role</span><span class="sxs-lookup"><span data-stu-id="018bf-3277">Role</span></span>

* <span data-ttu-id="018bf-3278">Unterstützung für erforderliche Zugriffskonfigurationen und native Clients zu `az ad app create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3278">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="018bf-3279">`rbac`-Befehle geändert, um maximal 1.000 IDs für Objektauflösung zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="018bf-3279">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="018bf-3280">Befehle zur Verwaltung von Anmeldeinformationen (`ad sp credential [reset|list|delete]`) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3280">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="018bf-3281">[BREAKING CHANGE] „properties“ aus `az role assignment [list|show]`-Ausgabe entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-3281">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="018bf-3282">Unterstützung für `dataActions`- und `notDataActions`-Berechtigungen zu `role definition` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3282">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="018bf-3283">Storage</span><span class="sxs-lookup"><span data-stu-id="018bf-3283">Storage</span></span>

* <span data-ttu-id="018bf-3284">Problem beim Hochladen von Dateien mit einer Größe von 195 GB bis 200 GB behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-3284">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="018bf-3285">[#4049](https://github.com/Azure/azure-cli/issues/4049) behoben: Probleme bei Uploads von Anfügeblobs behoben, die ein Ignorieren der Bedingungsparameter verursacht haben</span><span class="sxs-lookup"><span data-stu-id="018bf-3285">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="018bf-3286">VM</span><span class="sxs-lookup"><span data-stu-id="018bf-3286">VM</span></span>

* <span data-ttu-id="018bf-3287">Warnung für anstehende BREAKING CHANGEen für Sätze mit mehr als 100 Instanzen zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3287">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="018bf-3288">Unterstützung der Zonenresilienz zu `vm [snapshot|image]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3288">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="018bf-3289">Datenträgerinstanzansicht geändert, um besseren Verschlüsselungsstatus zu melden</span><span class="sxs-lookup"><span data-stu-id="018bf-3289">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="018bf-3290">[BREAKING CHANGE]`vm extension delete` geändert, um keine Ausgabe mehr zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="018bf-3290">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="018bf-3291">13. März 2018</span><span class="sxs-lookup"><span data-stu-id="018bf-3291">March 13, 2018</span></span>

<span data-ttu-id="018bf-3292">Version 2.0.29</span><span class="sxs-lookup"><span data-stu-id="018bf-3292">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="018bf-3293">ACR</span><span class="sxs-lookup"><span data-stu-id="018bf-3293">ACR</span></span>

* <span data-ttu-id="018bf-3294">Unterstützung für den Parameter `--image` zu `repository delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3294">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="018bf-3295">Parameter `--manifest` und `--tag` des Befehls `repository delete` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="018bf-3295">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="018bf-3296">Befehl `repository untag` zum Entfernen eines Tags ohne das Löschen von Daten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3296">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="018bf-3297">ACS</span><span class="sxs-lookup"><span data-stu-id="018bf-3297">ACS</span></span>

* <span data-ttu-id="018bf-3298">Befehl `aks upgrade-connector` zum Aktualisieren eines vorhandenen Connectors hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3298">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="018bf-3299">`kubectl`-Konfigurationsdateien zur Verwendung von besser lesbarem YAML im Blockstil geändert</span><span class="sxs-lookup"><span data-stu-id="018bf-3299">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="018bf-3300">Advisor</span><span class="sxs-lookup"><span data-stu-id="018bf-3300">Advisor</span></span>

* <span data-ttu-id="018bf-3301">[BREAKING CHANGE]`advisor configuration get` in `advisor configuration list` umbenannt</span><span class="sxs-lookup"><span data-stu-id="018bf-3301">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="018bf-3302">[BREAKING CHANGE]`advisor configuration set` in `advisor configuration update` umbenannt</span><span class="sxs-lookup"><span data-stu-id="018bf-3302">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="018bf-3303">[BREAKING CHANGE]`advisor recommendation generate` entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-3303">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="018bf-3304">Parameter `--refresh` zu `advisor recommendation list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3304">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="018bf-3305">Befehl `advisor recommendation show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3305">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="018bf-3306">AppService</span><span class="sxs-lookup"><span data-stu-id="018bf-3306">Appservice</span></span>

* <span data-ttu-id="018bf-3307">`[webapp|functionapp] assign-identity` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="018bf-3307">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="018bf-3308">Befehle `webapp identity [assign|show]` und `functionapp identity [assign|show]` für verwaltete Identität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3308">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="018bf-3309">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="018bf-3309">Eventhubs</span></span>

* <span data-ttu-id="018bf-3310">Erste Veröffentlichung</span><span class="sxs-lookup"><span data-stu-id="018bf-3310">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="018bf-3311">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="018bf-3311">Extension</span></span>

* <span data-ttu-id="018bf-3312">Überprüfung zum Warnen von Benutzern hinzugefügt, wenn sich die verwendete Distribution von der in der Paketquelldatei gespeicherten Distribution unterscheidet, da dies Fehlern führen kann</span><span class="sxs-lookup"><span data-stu-id="018bf-3312">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="018bf-3313">Interactive</span><span class="sxs-lookup"><span data-stu-id="018bf-3313">Interactive</span></span>

* <span data-ttu-id="018bf-3314">[#5625](https://github.com/Azure/azure-cli/issues/5625) behoben: Verlauf über verschiedene Sitzungen hinweg beibehalten</span><span class="sxs-lookup"><span data-stu-id="018bf-3314">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="018bf-3315">[#3016](https://github.com/Azure/azure-cli/issues/3016) behoben: Verlauf nicht aufgezeichnet, obwohl er innerhalb des Bereichs liegt</span><span class="sxs-lookup"><span data-stu-id="018bf-3315">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="018bf-3316">[#5688](https://github.com/Azure/azure-cli/issues/5688) behoben: Abschlüsse wurden nicht angezeigt, wenn beim Laden der Befehlstabelle eine Ausnahme aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="018bf-3316">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="018bf-3317">Statusanzeige für lang ausgeführte Vorgänge korrigiert</span><span class="sxs-lookup"><span data-stu-id="018bf-3317">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="018bf-3318">Überwachen</span><span class="sxs-lookup"><span data-stu-id="018bf-3318">Monitor</span></span>

* <span data-ttu-id="018bf-3319">`monitor autoscale-settings`-Befehle als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="018bf-3319">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="018bf-3320">Befehle vom Typ `monitor autoscale` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3320">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="018bf-3321">Befehle vom Typ `monitor autoscale profile` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3321">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="018bf-3322">Befehle vom Typ `monitor autoscale rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3322">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="018bf-3323">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="018bf-3323">Network</span></span>

* <span data-ttu-id="018bf-3324">[BREAKING CHANGE] Parameter `--tags` aus `route-filter rule create` entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-3324">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="018bf-3325">Einige fehlerhafte Standardwerte für die folgenden Befehle entfernt:</span><span class="sxs-lookup"><span data-stu-id="018bf-3325">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="018bf-3326">`network watcher connection-monitor`-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3326">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="018bf-3327">Parameter `--vnet` und `--subnet` zu `network watcher show-topology` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3327">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="018bf-3328">Profil</span><span class="sxs-lookup"><span data-stu-id="018bf-3328">Profile</span></span>

* <span data-ttu-id="018bf-3329">Parameter `--msi` für `az login` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="018bf-3329">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="018bf-3330">Parameter `--identity` für `az login` als Ersatz vor `--msi` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3330">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="018bf-3331">RDBMS</span><span class="sxs-lookup"><span data-stu-id="018bf-3331">RDBMS</span></span>

* <span data-ttu-id="018bf-3332">[VORSCHAU] Geändert, sodass die API „2017-12-01-preview“ verwendet wird</span><span class="sxs-lookup"><span data-stu-id="018bf-3332">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="018bf-3333">Service Bus</span><span class="sxs-lookup"><span data-stu-id="018bf-3333">Service Bus</span></span>

* <span data-ttu-id="018bf-3334">Erste Veröffentlichung</span><span class="sxs-lookup"><span data-stu-id="018bf-3334">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="018bf-3335">Storage</span><span class="sxs-lookup"><span data-stu-id="018bf-3335">Storage</span></span>

* <span data-ttu-id="018bf-3336">[#4971](https://github.com/Azure/azure-cli/issues/4971) behoben: `storage blob copy` unterstützt jetzt andere Azure-Clouds.</span><span class="sxs-lookup"><span data-stu-id="018bf-3336">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="018bf-3337">[#5286](https://github.com/Azure/azure-cli/issues/5286) behoben: Batchbefehle `storage blob [delete-batch|download-batch|upload-batch]` lösen bei Vorbedingungsfehlern keinen Fehler mehr aus</span><span class="sxs-lookup"><span data-stu-id="018bf-3337">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="018bf-3338">VM</span><span class="sxs-lookup"><span data-stu-id="018bf-3338">VM</span></span>

* <span data-ttu-id="018bf-3339">`[vm|vmss] create` unterstützt jetzt das Anfügen nicht verwalteter Datenträger und das Konfigurieren der Zwischenspeicherung.</span><span class="sxs-lookup"><span data-stu-id="018bf-3339">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="018bf-3340">`[vm|vmss] assign-identity` und `[vm|vmss] remove-identity` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="018bf-3340">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="018bf-3341">Befehle `vm identity [assign|remove|show]` und `vmss identity [assign|remove|show]` als Ersatz für veraltete Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3341">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="018bf-3342">Standardpriorität in `vmss create` auf „Keine“ geändert</span><span class="sxs-lookup"><span data-stu-id="018bf-3342">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="018bf-3343">27. Februar 2018</span><span class="sxs-lookup"><span data-stu-id="018bf-3343">February 27, 2018</span></span>

<span data-ttu-id="018bf-3344">Version 2.0.28</span><span class="sxs-lookup"><span data-stu-id="018bf-3344">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="018bf-3345">Core</span><span class="sxs-lookup"><span data-stu-id="018bf-3345">Core</span></span>

* <span data-ttu-id="018bf-3346">[#5184](https://github.com/Azure/azure-cli/issues/5184) behoben: Problem beim Installieren von Homebrew</span><span class="sxs-lookup"><span data-stu-id="018bf-3346">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="018bf-3347">Unterstützung für Erweiterungstelemetrie mit benutzerdefinierten Schlüsseln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3347">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="018bf-3348">HTTP-Protokollierung zu `--debug` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3348">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="018bf-3349">ACS</span><span class="sxs-lookup"><span data-stu-id="018bf-3349">ACS</span></span>

* <span data-ttu-id="018bf-3350">Geändert, sodass für `aks install-connector` standardmäßig das Helm-Diagramm `virtual-kubelet-for-aks` verwendet wird</span><span class="sxs-lookup"><span data-stu-id="018bf-3350">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="018bf-3351">Problem behoben: Unzureichende Berechtigungen für Dienstprinzipale zum Erstellen einer ACI-Containergruppe</span><span class="sxs-lookup"><span data-stu-id="018bf-3351">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="018bf-3352">Parameter `--aci-container-group`, `--location` und `--image-tag` zu `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3352">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="018bf-3353">Veraltungshinweis aus `aks get-versions` entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-3353">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="018bf-3354">AppService</span><span class="sxs-lookup"><span data-stu-id="018bf-3354">Appservice</span></span>

* <span data-ttu-id="018bf-3355">Updates für die neue SDK-Version (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="018bf-3355">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="018bf-3356">[5538](https://github.com/Azure/azure-cli/issues/5538) behoben: `Free` wurde als ungültige SKU gemeldet.</span><span class="sxs-lookup"><span data-stu-id="018bf-3356">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="018bf-3357">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="018bf-3357">Cognitive Services</span></span>

* <span data-ttu-id="018bf-3358">Hinweis beim Erstellen eines neuen Cognitive Services-Kontos aktualisiert</span><span class="sxs-lookup"><span data-stu-id="018bf-3358">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="018bf-3359">Nutzung</span><span class="sxs-lookup"><span data-stu-id="018bf-3359">Consumption</span></span>

* <span data-ttu-id="018bf-3360">Neue Befehle für PriceSheet-API hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3360">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="018bf-3361">Vorhandene Formate für Nutzungsdetails und Reservierungsdetails aktualisiert</span><span class="sxs-lookup"><span data-stu-id="018bf-3361">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="018bf-3362">Container</span><span class="sxs-lookup"><span data-stu-id="018bf-3362">Container</span></span>

* <span data-ttu-id="018bf-3363">Argumente `--secrets` und `--secrets-mount-path` zu `container create` hinzugefügt, um Geheimnisse in ACI verwenden zu können</span><span class="sxs-lookup"><span data-stu-id="018bf-3363">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="018bf-3364">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="018bf-3364">Network</span></span>

* <span data-ttu-id="018bf-3365">[#5559](https://github.com/Azure/azure-cli/issues/5559) behoben: Fehlender Client in `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="018bf-3365">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="018bf-3366">Resource</span><span class="sxs-lookup"><span data-stu-id="018bf-3366">Resource</span></span>

* <span data-ttu-id="018bf-3367">`group deployment export` geändert, um eine partielle Vorlage und ggf. Fehler anzuzeigen, wenn der Vorgang nicht erfolgreich war</span><span class="sxs-lookup"><span data-stu-id="018bf-3367">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="018bf-3368">Role</span><span class="sxs-lookup"><span data-stu-id="018bf-3368">Role</span></span>

* <span data-ttu-id="018bf-3369">`role assignment list-changelogs` hinzugefügt, um die Überprüfung von Dienstprinzipalrollen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="018bf-3369">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="018bf-3370">SQL</span><span class="sxs-lookup"><span data-stu-id="018bf-3370">SQL</span></span>

* <span data-ttu-id="018bf-3371">Zonenredundanzunterstützung für Datenbanken und Pools für elastische Datenbanken hinzugefügt (bei Erstellung und Aktualisierung)</span><span class="sxs-lookup"><span data-stu-id="018bf-3371">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="018bf-3372">Storage</span><span class="sxs-lookup"><span data-stu-id="018bf-3372">Storage</span></span>

* <span data-ttu-id="018bf-3373">Angabe von Zielpfad/Präfix für `storage blob [upload-batch|download-batch]` ermöglicht</span><span class="sxs-lookup"><span data-stu-id="018bf-3373">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="018bf-3374">VM</span><span class="sxs-lookup"><span data-stu-id="018bf-3374">VM</span></span>

* <span data-ttu-id="018bf-3375">Unterstützung für das Anfügen/Trennen von Datenträgern für eine einzelne VMSS-Instanz hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3375">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="018bf-3376">13. Februar 2018</span><span class="sxs-lookup"><span data-stu-id="018bf-3376">February 13, 2018</span></span>

<span data-ttu-id="018bf-3377">Version 2.0.27</span><span class="sxs-lookup"><span data-stu-id="018bf-3377">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="018bf-3378">Core</span><span class="sxs-lookup"><span data-stu-id="018bf-3378">Core</span></span>

* <span data-ttu-id="018bf-3379">Authentifizierung für Abonnement-ID und Namen bei der MSI-Anmeldung in Authentifizierung mit Schlüssel geändert</span><span class="sxs-lookup"><span data-stu-id="018bf-3379">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="018bf-3380">ACS</span><span class="sxs-lookup"><span data-stu-id="018bf-3380">ACS</span></span>

* <span data-ttu-id="018bf-3381">[BREAKING CHANGE]`aks get-versions` aus Gründen der Genauigkeit in `aks get-upgrades` umbenannt</span><span class="sxs-lookup"><span data-stu-id="018bf-3381">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="018bf-3382">`aks get-versions` zur Anzeige der verfügbaren Kubernetes-Versionen für `aks create` geändert</span><span class="sxs-lookup"><span data-stu-id="018bf-3382">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="018bf-3383">Standardwerte von `aks create` in Auswahl der Kubernetes-Version durch den Server geändert</span><span class="sxs-lookup"><span data-stu-id="018bf-3383">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="018bf-3384">Hilfemeldungen zu dem von AKS generierten Dienstprinzipal aktualisiert</span><span class="sxs-lookup"><span data-stu-id="018bf-3384">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="018bf-3385">Standardknotengrößen für `aks create` von „Standard\_D1\_v2“ in „Standard\_DS1\_v2“ geändert</span><span class="sxs-lookup"><span data-stu-id="018bf-3385">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="018bf-3386">Zuverlässigkeit der Suche nach dem Dashboardpod für `az aks browse` verbessert</span><span class="sxs-lookup"><span data-stu-id="018bf-3386">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="018bf-3387">`aks get-credentials` korrigiert, um Unicode-Fehler beim Laden von Kubernetes-Konfigurationsdateien zu behandeln</span><span class="sxs-lookup"><span data-stu-id="018bf-3387">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="018bf-3388">Meldung zu `az aks install-cli` hinzugefügt, um das Abrufen von `kubectl` in `$PATH` zu erleichtern</span><span class="sxs-lookup"><span data-stu-id="018bf-3388">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="018bf-3389">AppService</span><span class="sxs-lookup"><span data-stu-id="018bf-3389">Appservice</span></span>

* <span data-ttu-id="018bf-3390">Problem behoben, das zu einem Fehler von `webapp [backup|restore]` aufgrund eines Nullverweises führte</span><span class="sxs-lookup"><span data-stu-id="018bf-3390">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="018bf-3391">Unterstützung für Standard-App Service-Pläne durch `az configure --defaults appserviceplan=my-asp` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3391">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="018bf-3392">CDN</span><span class="sxs-lookup"><span data-stu-id="018bf-3392">CDN</span></span>

* <span data-ttu-id="018bf-3393">Befehle vom Typ `cdn custom-domain [enable-https|disable-https]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3393">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="018bf-3394">Container</span><span class="sxs-lookup"><span data-stu-id="018bf-3394">Container</span></span>

* <span data-ttu-id="018bf-3395">Option `--follow` zu `az container logs` für Streamingprotokolle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3395">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="018bf-3396">Befehl `container attach` hinzugefügt, der die lokale Standardausgabe und Fehlerdatenströme an einen Container in einer Containergruppe angefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3396">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="018bf-3397">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="018bf-3397">CosmosDB</span></span>

* <span data-ttu-id="018bf-3398">Unterstützung für Einstellungsfunktionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3398">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="018bf-3399">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="018bf-3399">Extension</span></span>

* <span data-ttu-id="018bf-3400">Unterstützung für den Parameter `--pip-proxy` zu Befehlen vom Typ `az extension [add|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3400">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="018bf-3401">Unterstützung für das Argument `--pip-extra-index-urls` zu Befehlen vom Typ `az extension [add|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3401">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="018bf-3402">Feedback</span><span class="sxs-lookup"><span data-stu-id="018bf-3402">Feedback</span></span>

* <span data-ttu-id="018bf-3403">Erweiterungsinformationen zu Telemetriedaten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3403">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="018bf-3404">Interactive</span><span class="sxs-lookup"><span data-stu-id="018bf-3404">Interactive</span></span>

* <span data-ttu-id="018bf-3405">Problem behoben, aufgrund dessen der Benutzer bei Verwendung des interaktiven Modus in Cloud Shell zur Anmeldung aufgefordert wird</span><span class="sxs-lookup"><span data-stu-id="018bf-3405">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="018bf-3406">Regression mit fehlenden Parametervervollständigungen korrigiert</span><span class="sxs-lookup"><span data-stu-id="018bf-3406">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="018bf-3407">IoT</span><span class="sxs-lookup"><span data-stu-id="018bf-3407">IoT</span></span>

* <span data-ttu-id="018bf-3408">Problem behoben, aufgrund dessen `iot dps access policy [create|update]` bei erfolgreicher Ausführung einen Fehler „nicht gefunden“ zurückgibt</span><span class="sxs-lookup"><span data-stu-id="018bf-3408">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="018bf-3409">Problem behoben, aufgrund dessen `iot dps linked-hub [create|update]` bei erfolgreicher Ausführung einen Fehler „nicht gefunden“ zurückgibt</span><span class="sxs-lookup"><span data-stu-id="018bf-3409">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="018bf-3410">Unterstützung für `--no-wait` zu `iot dps access policy [create|update]` und `iot dps linked-hub [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3410">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="018bf-3411">`iot hub create` geändert, um die Angabe der Anzahl von Partitionen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="018bf-3411">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="018bf-3412">Überwachen</span><span class="sxs-lookup"><span data-stu-id="018bf-3412">Monitor</span></span>

* <span data-ttu-id="018bf-3413">Befehl `az monitor log-profiles create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="018bf-3413">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="018bf-3414">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="018bf-3414">Network</span></span>

* <span data-ttu-id="018bf-3415">Option `--tags` für folgende Befehle korrigiert:</span><span class="sxs-lookup"><span data-stu-id="018bf-3415">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="018bf-3416">Profil</span><span class="sxs-lookup"><span data-stu-id="018bf-3416">Profile</span></span>

* <span data-ttu-id="018bf-3417">`az login` im interaktiven Modus aktiviert</span><span class="sxs-lookup"><span data-stu-id="018bf-3417">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="018bf-3418">Resource</span><span class="sxs-lookup"><span data-stu-id="018bf-3418">Resource</span></span>

* <span data-ttu-id="018bf-3419">`feature show` wieder hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3419">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="018bf-3420">Role</span><span class="sxs-lookup"><span data-stu-id="018bf-3420">Role</span></span>

* <span data-ttu-id="018bf-3421">Argument `--available-to-other-tenants` zu `ad app update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3421">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="018bf-3422">SQL</span><span class="sxs-lookup"><span data-stu-id="018bf-3422">SQL</span></span>

* <span data-ttu-id="018bf-3423">Befehle vom Typ `sql server dns-alias` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3423">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="018bf-3424">`sql db rename` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3424">Added `sql db rename`</span></span>
* <span data-ttu-id="018bf-3425">Unterstützung für das Argument `--ids` für alle SQL-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3425">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="018bf-3426">Storage</span><span class="sxs-lookup"><span data-stu-id="018bf-3426">Storage</span></span>

* <span data-ttu-id="018bf-3427">Befehle `storage blob service-properties delete-policy` und `storage blob undelete` hinzugefügt, um vorläufiges Löschen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="018bf-3427">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="018bf-3428">VM</span><span class="sxs-lookup"><span data-stu-id="018bf-3428">VM</span></span>

* <span data-ttu-id="018bf-3429">Absturz bei unvollständiger Initialisierung der VM-Verschlüsselung behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-3429">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="018bf-3430">Prinzipal-ID-Ausgabe beim Aktivieren von MSI hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3430">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="018bf-3431">`vm boot-diagnostics get-boot-log` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="018bf-3431">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="018bf-3432">31. Januar 2018</span><span class="sxs-lookup"><span data-stu-id="018bf-3432">January 31, 2018</span></span>

<span data-ttu-id="018bf-3433">Version 2.0.26</span><span class="sxs-lookup"><span data-stu-id="018bf-3433">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="018bf-3434">Core</span><span class="sxs-lookup"><span data-stu-id="018bf-3434">Core</span></span>

* <span data-ttu-id="018bf-3435">Unterstützung für das Abrufen von unformatierten Token im MSI-Kontext hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3435">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="018bf-3436">Abrufindikator-Zeichenfolge nach Fertigstellung von LRO für die Windows-Datei „cmd.exe“ entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-3436">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="018bf-3437">Warnung hinzugefügt, die angezeigt wird, wenn ein konfigurierter Standardwert in einen Eintrag auf INFO-Ebene geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="018bf-3437">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="018bf-3438">`--verbose` zum Anzeigen verwenden.</span><span class="sxs-lookup"><span data-stu-id="018bf-3438">Use `--verbose` to see</span></span>
* <span data-ttu-id="018bf-3439">Statusanzeige für Wait-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3439">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="018bf-3440">ACS</span><span class="sxs-lookup"><span data-stu-id="018bf-3440">ACS</span></span>

* <span data-ttu-id="018bf-3441">Argument `--disable-browser` erläutert</span><span class="sxs-lookup"><span data-stu-id="018bf-3441">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="018bf-3442">Vervollständigung mit der TAB-TASTE für Argumente vom Typ `--vm-size` verbessert</span><span class="sxs-lookup"><span data-stu-id="018bf-3442">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="018bf-3443">AppService</span><span class="sxs-lookup"><span data-stu-id="018bf-3443">Appservice</span></span>

* <span data-ttu-id="018bf-3444">`webapp log [tail|download]` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="018bf-3444">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="018bf-3445">Überprüfung `kind` für Web-Apps und Funktionen entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-3445">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="018bf-3446">CDN</span><span class="sxs-lookup"><span data-stu-id="018bf-3446">CDN</span></span>

* <span data-ttu-id="018bf-3447">Problem mit fehlendem Client für `cdn custom-domain create` behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-3447">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="018bf-3448">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="018bf-3448">CosmosDB</span></span>

* <span data-ttu-id="018bf-3449">Parameterbeschreibung für Failoverrichtlinien korrigiert</span><span class="sxs-lookup"><span data-stu-id="018bf-3449">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="018bf-3450">Interactive</span><span class="sxs-lookup"><span data-stu-id="018bf-3450">Interactive</span></span>

* <span data-ttu-id="018bf-3451">Problem behoben, aufgrund dessen Vervollständigungen von Befehlsoptionen nicht mehr angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="018bf-3451">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="018bf-3452">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="018bf-3452">Network</span></span>

* <span data-ttu-id="018bf-3453">Schutz für `--cert-password` zu `application-gateway create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3453">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="018bf-3454">Problem mit `application-gateway update` behoben, aufgrund dessen `--sku` fälschlicherweise einen Standardwert anwendete</span><span class="sxs-lookup"><span data-stu-id="018bf-3454">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="018bf-3455">Schutz für `--shared-key` und `--authorization-key` zu `vpn-connection create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3455">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="018bf-3456">Problem mit fehlendem Client für `asg create` behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-3456">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="018bf-3457">Parameter `--file-name / -f` für exportierte Namen zu `dns zone export` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3457">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="018bf-3458">Folgende Probleme mit `dns zone export` behoben:</span><span class="sxs-lookup"><span data-stu-id="018bf-3458">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="018bf-3459">Problem behoben, aufgrund dessen lange TXT-Einträge nicht korrekt exportiert wurden</span><span class="sxs-lookup"><span data-stu-id="018bf-3459">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="018bf-3460">Problem behoben, aufgrund dessen TXT-Einträge in Anführungszeichen fälschlich ohne Anführungszeichen in Escapezeichen exportiert wurden</span><span class="sxs-lookup"><span data-stu-id="018bf-3460">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="018bf-3461">Problem behoben, aufgrund dessen bestimmte Datensätze zweimal mit `dns zone import` importiert wurden</span><span class="sxs-lookup"><span data-stu-id="018bf-3461">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="018bf-3462">Befehle `vnet-gateway root-cert` und `vnet-gateway revoked-cert` wiederhergestellt</span><span class="sxs-lookup"><span data-stu-id="018bf-3462">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="018bf-3463">Profil</span><span class="sxs-lookup"><span data-stu-id="018bf-3463">Profile</span></span>

* <span data-ttu-id="018bf-3464">`get-access-token` zur Verwendung auf einer VM mit Identität korrigiert</span><span class="sxs-lookup"><span data-stu-id="018bf-3464">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="018bf-3465">Resource</span><span class="sxs-lookup"><span data-stu-id="018bf-3465">Resource</span></span>

* <span data-ttu-id="018bf-3466">Fehler mit `deployment [create|validate]` korrigiert, aufgrund dessen fälschlich eine Warnung angezeigt wurde, wenn ein Vorlagenfeld „Typ“ Werte in Großbuchstaben enthielt</span><span class="sxs-lookup"><span data-stu-id="018bf-3466">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="018bf-3467">Storage</span><span class="sxs-lookup"><span data-stu-id="018bf-3467">Storage</span></span>

* <span data-ttu-id="018bf-3468">Problem mit der Migration von Storage V1-Konten zu Storage V2 behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-3468">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="018bf-3469">Statusberichterstellung für alle Upload-/Downloadbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3469">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="018bf-3470">Fehler korrigiert, der die Verwendung der arg-Option „-n“ mit `storage account check-name` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="018bf-3470">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="018bf-3471">Spalte „Momentaufnahme“ zur Tabellenausgabe für `blob [list|show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3471">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="018bf-3472">Fehler mit verschiedenen Parametern korrigiert, die als Int-Typen analysiert werden mussten</span><span class="sxs-lookup"><span data-stu-id="018bf-3472">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="018bf-3473">VM</span><span class="sxs-lookup"><span data-stu-id="018bf-3473">VM</span></span>

* <span data-ttu-id="018bf-3474">Befehl `vm image accept-terms` hinzugefügt, um die Erstellung von VMs aus Images mit zusätzlichen Gebühren zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="018bf-3474">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="018bf-3475">`[vm|vmss create]` korrigiert, um sicherzustellen, dass Befehle unter einem Proxy mit nicht signierten Zertifikaten ausgeführt werden können</span><span class="sxs-lookup"><span data-stu-id="018bf-3475">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="018bf-3476">[VORSCHAU] Unterstützung für „niedrige“ Priorität zu VMSS hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3476">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="018bf-3477">Schutz für `--admin-password` zu `[vm|vmss] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3477">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="018bf-3478">17. Januar 2018</span><span class="sxs-lookup"><span data-stu-id="018bf-3478">January 17, 2018</span></span>

<span data-ttu-id="018bf-3479">Version 2.0.25</span><span class="sxs-lookup"><span data-stu-id="018bf-3479">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="018bf-3480">ACR</span><span class="sxs-lookup"><span data-stu-id="018bf-3480">ACR</span></span>

* <span data-ttu-id="018bf-3481">Fallback auf ACR-Anmeldung bei Fehlern mit Windows-Anmeldeinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3481">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="018bf-3482">Registrierungsprotokolle aktiviert</span><span class="sxs-lookup"><span data-stu-id="018bf-3482">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="018bf-3483">ACS</span><span class="sxs-lookup"><span data-stu-id="018bf-3483">ACS</span></span>

* <span data-ttu-id="018bf-3484">Befehl `get-credentials` korrigiert</span><span class="sxs-lookup"><span data-stu-id="018bf-3484">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="018bf-3485">SPN-Rollenanforderung entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-3485">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="018bf-3486">AppService</span><span class="sxs-lookup"><span data-stu-id="018bf-3486">Appservice</span></span>

* <span data-ttu-id="018bf-3487">Fehler mit `config ssl upload` behoben, bei dem `hosting_environment_profile` NULL war</span><span class="sxs-lookup"><span data-stu-id="018bf-3487">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="018bf-3488">Unterstützung benutzerdefinierter URLs zu `browse` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3488">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="018bf-3489">Slotunterstützung für `log tail` korrigiert</span><span class="sxs-lookup"><span data-stu-id="018bf-3489">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="018bf-3490">Backup</span><span class="sxs-lookup"><span data-stu-id="018bf-3490">Backup</span></span>

* <span data-ttu-id="018bf-3491">Option `--container-name` von `backup item list` geändert (ist jetzt optional)</span><span class="sxs-lookup"><span data-stu-id="018bf-3491">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="018bf-3492">Speicherkontooptionen zu `backup restore restore-disks` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3492">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="018bf-3493">Standortüberprüfung in `backup protection enable-for-vm` korrigiert (Groß-/Kleinschreibung wird jetzt nicht mehr beachtet)</span><span class="sxs-lookup"><span data-stu-id="018bf-3493">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="018bf-3494">Problem behoben, durch das bei Befehlen mit ungültigem Containernamen ein Fehler auftrat</span><span class="sxs-lookup"><span data-stu-id="018bf-3494">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="018bf-3495">`backup item list` geändert (Integritätsstatus jetzt standardmäßig enthalten)</span><span class="sxs-lookup"><span data-stu-id="018bf-3495">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="018bf-3496">Batch</span><span class="sxs-lookup"><span data-stu-id="018bf-3496">Batch</span></span>

* <span data-ttu-id="018bf-3497">`batch login` geändert, um Authentifizierungsdetails zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="018bf-3497">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="018bf-3498">Cloud</span><span class="sxs-lookup"><span data-stu-id="018bf-3498">Cloud</span></span>

* <span data-ttu-id="018bf-3499">Beim Festlegen von `--profile` für eine Cloud werden nun keine Endpunkte mehr benötigt.</span><span class="sxs-lookup"><span data-stu-id="018bf-3499">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="018bf-3500">Nutzung</span><span class="sxs-lookup"><span data-stu-id="018bf-3500">Consumption</span></span>

* <span data-ttu-id="018bf-3501">Neue Befehle für Reservierungen hinzugefügt: `consumption reservations summaries` und `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="018bf-3501">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="018bf-3502">Event Grid</span><span class="sxs-lookup"><span data-stu-id="018bf-3502">Event Grid</span></span>

* <span data-ttu-id="018bf-3503">[BREAKING CHANGE] Die Befehle vom Typ `az eventgrid topic event-subscription` wurden in `eventgrid event-subscription` verschoben.</span><span class="sxs-lookup"><span data-stu-id="018bf-3503">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="018bf-3504">[BREAKING CHANGE] Die Befehle vom Typ `az eventgrid resource event-subscription` wurden in `eventgrid event-subscription` verschoben.</span><span class="sxs-lookup"><span data-stu-id="018bf-3504">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="018bf-3505">[BREAKING CHANGE] Der Befehl `eventgrid event-subscription show-endpoint-url` wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="018bf-3505">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="018bf-3506">Verwenden Sie stattdessen `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="018bf-3506">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="018bf-3507">Befehl `eventgrid topic update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3507">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="018bf-3508">Befehl `eventgrid event-subscription update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3508">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="018bf-3509">Parameter `--ids` für Befehle vom Typ `eventgrid topic` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3509">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="018bf-3510">Unterstützung der Vervollständigung mit der TAB-TASTE für Themennamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3510">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="018bf-3511">Interactive</span><span class="sxs-lookup"><span data-stu-id="018bf-3511">Interactive</span></span>

* <span data-ttu-id="018bf-3512">Problem behoben, das dazu führte, dass der interaktive Modus nicht mit Python 2.x verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="018bf-3512">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="018bf-3513">Fehler beim Start behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-3513">Fixed errors on startup</span></span>
* <span data-ttu-id="018bf-3514">Problem behoben, das dazu führte, dass einige Befehle nicht im interaktiven Modus ausgeführt werden konnten</span><span class="sxs-lookup"><span data-stu-id="018bf-3514">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="018bf-3515">IoT</span><span class="sxs-lookup"><span data-stu-id="018bf-3515">IoT</span></span>

* <span data-ttu-id="018bf-3516">Unterstützung für Gerätebereitstellungsdienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3516">Added support for device provisioning service</span></span>
* <span data-ttu-id="018bf-3517">Benachrichtigungen zu veralteten Elementen in Befehlen und in der Befehlshilfe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3517">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="018bf-3518">IoT-Überprüfung hinzugefügt, um Benutzer über die IoT-Erweiterung zu informieren</span><span class="sxs-lookup"><span data-stu-id="018bf-3518">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="018bf-3519">Überwachen</span><span class="sxs-lookup"><span data-stu-id="018bf-3519">Monitor</span></span>

* <span data-ttu-id="018bf-3520">Unterstützung mehrerer Diagnoseeinstellung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-3520">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="018bf-3521">Der Parameter `--name` ist nun für `az monitor diagnostic-settings create` erforderlich.</span><span class="sxs-lookup"><span data-stu-id="018bf-3521">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="018bf-3522">Befehl `monitor diagnostic-settings categories` zum Abrufen der Diagnoseeinstellungskategorie hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3522">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="018bf-3523">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="018bf-3523">Network</span></span>

* <span data-ttu-id="018bf-3524">Problem behoben, das beim Ändern des aktiven Standbymodus mit `vnet-gateway update` auftrat</span><span class="sxs-lookup"><span data-stu-id="018bf-3524">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="018bf-3525">Unterstützung für HTTP2 zu `application-gateway [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3525">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="018bf-3526">Profil</span><span class="sxs-lookup"><span data-stu-id="018bf-3526">Profile</span></span>

* <span data-ttu-id="018bf-3527">Unterstützung für die Anmeldung mit durch Benutzer zugewiesenen Identitäten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3527">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="018bf-3528">Role</span><span class="sxs-lookup"><span data-stu-id="018bf-3528">Role</span></span>

* <span data-ttu-id="018bf-3529">Argument `--assignee-object-id` zu `role assignment create` hinzugefügt, um Graph-Abfrage zu umgehen</span><span class="sxs-lookup"><span data-stu-id="018bf-3529">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="018bf-3530">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="018bf-3530">Service Fabric</span></span>

* <span data-ttu-id="018bf-3531">Ausführliche Fehler zur Überprüfungsantwort bei der Clustererstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3531">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="018bf-3532">Problem mit fehlendem Client für verschiedene Befehle behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-3532">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="018bf-3533">VM</span><span class="sxs-lookup"><span data-stu-id="018bf-3533">VM</span></span>

* <span data-ttu-id="018bf-3534">[VORSCHAUVERSION] Zonenübergreifende Unterstützung für `vmss`</span><span class="sxs-lookup"><span data-stu-id="018bf-3534">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="018bf-3535">[BREAKING CHANGE] Standard für Einzelzone (`vmss`) in Standardlastenausgleich geändert</span><span class="sxs-lookup"><span data-stu-id="018bf-3535">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="018bf-3536">[BREAKING CHANGE]`externalIdentities` in `userAssignedIdentities` geändert für EMSI</span><span class="sxs-lookup"><span data-stu-id="018bf-3536">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="018bf-3537">[VORSCHAUVERSION] Unterstützung für Austausch des Betriebssystemdatenträgers hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3537">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="018bf-3538">Unterstützung der Verwendung von VM-Images aus anderen Abonnements hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3538">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="018bf-3539">Argumente `--plan-name`, `--plan-product`, `--plan-promotion-code` und `--plan-publisher` zu `[vm|vmss] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3539">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="018bf-3540">Fehlerbedingte Probleme mit `[vm|vmss] create` behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-3540">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="018bf-3541">Übermäßige Ressourcenverwendung durch `vm image list --all` behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-3541">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="018bf-3542">19. Dezember 2017</span><span class="sxs-lookup"><span data-stu-id="018bf-3542">December 19, 2017</span></span>

<span data-ttu-id="018bf-3543">Version 2.0.23</span><span class="sxs-lookup"><span data-stu-id="018bf-3543">Version 2.0.23</span></span>

* <span data-ttu-id="018bf-3544">Unterstützung für die Anmeldung mit durch Benutzer zugewiesenen Identitäten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3544">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="018bf-3545">Container</span><span class="sxs-lookup"><span data-stu-id="018bf-3545">Container</span></span>

* <span data-ttu-id="018bf-3546">Falsche Reihenfolge der Parameter für Containerprotokolle behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-3546">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="018bf-3547">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="018bf-3547">Network</span></span>

* <span data-ttu-id="018bf-3548">Argument `--disable-bgp-route-propagation` zu `route-table [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3548">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="018bf-3549">Argument `--ip-tags` zu `public-ip [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3549">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="018bf-3550">Storage</span><span class="sxs-lookup"><span data-stu-id="018bf-3550">Storage</span></span>

* <span data-ttu-id="018bf-3551">Unterstützung für Storage V2 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3551">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="018bf-3552">VM</span><span class="sxs-lookup"><span data-stu-id="018bf-3552">VM</span></span>

* <span data-ttu-id="018bf-3553">[VORSCHAUVERSION] Unterstützung für durch Benutzer zugewiesene Identitäten für virtuelle Computer und VMSSs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3553">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="018bf-3554">5\. Dezember 2017</span><span class="sxs-lookup"><span data-stu-id="018bf-3554">December 5, 2017</span></span>

<span data-ttu-id="018bf-3555">Version 2.0.22</span><span class="sxs-lookup"><span data-stu-id="018bf-3555">Version 2.0.22</span></span>

* <span data-ttu-id="018bf-3556">`az component`-Befehle wurden entfernt.</span><span class="sxs-lookup"><span data-stu-id="018bf-3556">Removed `az component` commands.</span></span> <span data-ttu-id="018bf-3557">Verwenden Sie stattdessen `az extension`.</span><span class="sxs-lookup"><span data-stu-id="018bf-3557">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="018bf-3558">Core</span><span class="sxs-lookup"><span data-stu-id="018bf-3558">Core</span></span>
* <span data-ttu-id="018bf-3559">Der `AZURE_US_GOV_CLOUD`-Autoritätsendpunkt von AAD wurde von „login.microsoftonline.com“ in „login.microsoftonline.us“ geändert.</span><span class="sxs-lookup"><span data-stu-id="018bf-3559">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="018bf-3560">Problem behoben, aufgrund dessen Telemetriedaten fortlaufend neu gesendet wurden</span><span class="sxs-lookup"><span data-stu-id="018bf-3560">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="018bf-3561">ACS</span><span class="sxs-lookup"><span data-stu-id="018bf-3561">ACS</span></span>

* <span data-ttu-id="018bf-3562">Die Befehle `aks install-connector` und `aks remove-connector` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-3562">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="018bf-3563">Verbesserte Fehlerberichterstellung für `acs create`</span><span class="sxs-lookup"><span data-stu-id="018bf-3563">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="018bf-3564">Feste Verwendung von `aks get-credentials -f` ohne vollqualifizierten Pfad</span><span class="sxs-lookup"><span data-stu-id="018bf-3564">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="018bf-3565">Advisor</span><span class="sxs-lookup"><span data-stu-id="018bf-3565">Advisor</span></span>

* <span data-ttu-id="018bf-3566">Erste Veröffentlichung</span><span class="sxs-lookup"><span data-stu-id="018bf-3566">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="018bf-3567">AppService</span><span class="sxs-lookup"><span data-stu-id="018bf-3567">Appservice</span></span>

* <span data-ttu-id="018bf-3568">Erstellung feststehender Zertifikatnamen mit `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="018bf-3568">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="018bf-3569">`webapp [list|show]` und `functionapp [list|show]` wurden verbessert, um die richtigen Apps anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="018bf-3569">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="018bf-3570">Standardwert für `WEBSITE_NODE_DEFAULT_VERSION` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3570">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="018bf-3571">Nutzung</span><span class="sxs-lookup"><span data-stu-id="018bf-3571">Consumption</span></span>

* <span data-ttu-id="018bf-3572">Unterstützung für API-Version 2017-11-30 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3572">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="018bf-3573">Container</span><span class="sxs-lookup"><span data-stu-id="018bf-3573">Container</span></span>

* <span data-ttu-id="018bf-3574">Feste Regression für Standardports</span><span class="sxs-lookup"><span data-stu-id="018bf-3574">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="018bf-3575">Überwachen</span><span class="sxs-lookup"><span data-stu-id="018bf-3575">Monitor</span></span>

* <span data-ttu-id="018bf-3576">Unterstützung mehrerer Dimensionen zu Metrikbefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3576">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="018bf-3577">Resource</span><span class="sxs-lookup"><span data-stu-id="018bf-3577">Resource</span></span>

* <span data-ttu-id="018bf-3578">Argument `--include-response-body` zu `resource show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3578">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="018bf-3579">Role</span><span class="sxs-lookup"><span data-stu-id="018bf-3579">Role</span></span>

* <span data-ttu-id="018bf-3580">Anzeige von Standardzuweisungen für „klassische“ Administratoren zu `role assignment list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3580">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="018bf-3581">Unterstützung für das Hinzufügen (anstelle der Überschreibung) von Anmeldeinformationen zu `ad sp reset-credentials` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3581">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="018bf-3582">Verbesserte Fehlerberichterstellung für `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="018bf-3582">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="018bf-3583">SQL</span><span class="sxs-lookup"><span data-stu-id="018bf-3583">SQL</span></span>

* <span data-ttu-id="018bf-3584">Die Befehle `sql db list-usages` und `sql db show-usage` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-3584">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="018bf-3585">Die Befehle `sql server conn-policy show` und `sql server conn-policy update` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-3585">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="018bf-3586">VM</span><span class="sxs-lookup"><span data-stu-id="018bf-3586">VM</span></span>

* <span data-ttu-id="018bf-3587">Zoneninformationen zu `az vm list-skus` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3587">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="018bf-3588">14. November 2017</span><span class="sxs-lookup"><span data-stu-id="018bf-3588">November 14, 2017</span></span>

<span data-ttu-id="018bf-3589">Version 2.0.21</span><span class="sxs-lookup"><span data-stu-id="018bf-3589">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="018bf-3590">ACR</span><span class="sxs-lookup"><span data-stu-id="018bf-3590">ACR</span></span>

* <span data-ttu-id="018bf-3591">Unterstützung für das Erstellen von Webhooks in Replikationsregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3591">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="018bf-3592">ACS</span><span class="sxs-lookup"><span data-stu-id="018bf-3592">ACS</span></span>

* <span data-ttu-id="018bf-3593">Formulierung in AKS von „Agent“ in „Knoten“ geändert</span><span class="sxs-lookup"><span data-stu-id="018bf-3593">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="018bf-3594">Option `--orchestrator-release` für `acs create` als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="018bf-3594">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="018bf-3595">VM-Standardgröße für AKS in `Standard_D1_v2` geändert</span><span class="sxs-lookup"><span data-stu-id="018bf-3595">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="018bf-3596">`az aks browse` für Windows korrigiert</span><span class="sxs-lookup"><span data-stu-id="018bf-3596">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="018bf-3597">`az aks get-credentials` für Windows korrigiert</span><span class="sxs-lookup"><span data-stu-id="018bf-3597">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="018bf-3598">AppService</span><span class="sxs-lookup"><span data-stu-id="018bf-3598">Appservice</span></span>

* <span data-ttu-id="018bf-3599">Bereitstellungsquelle `config-zip` für Web-Apps und Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3599">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="018bf-3600">Option `--docker-container-logging` zu `az webapp log config` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3600">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="018bf-3601">Option `storage` aus dem Parameter `--web-server-logging` von `az webapp log config` entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-3601">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="018bf-3602">Fehlermeldungen für `deployment user set` verbessert</span><span class="sxs-lookup"><span data-stu-id="018bf-3602">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="018bf-3603">Unterstützung für das Erstellen von Linux-Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3603">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="018bf-3604">`list-locations` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="018bf-3604">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="018bf-3605">Batch</span><span class="sxs-lookup"><span data-stu-id="018bf-3605">Batch</span></span>

* <span data-ttu-id="018bf-3606">Fehler im Poolerstellungsbefehl korrigiert, der bei Verwendung einer Ressourcen-ID mit dem Flag `--image` aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="018bf-3606">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="018bf-3607">BatchAI</span><span class="sxs-lookup"><span data-stu-id="018bf-3607">Batchai</span></span>

* <span data-ttu-id="018bf-3608">Kurzoption (`-s`) für `--vm-size` zur Angabe der VM-Größe im Befehl `file-server create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3608">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="018bf-3609">Argumente für Speicherkontoname und -schlüssel zum Parameter `cluster create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3609">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="018bf-3610">Dokumentation für `job list-files` und `job stream-file` korrigiert</span><span class="sxs-lookup"><span data-stu-id="018bf-3610">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="018bf-3611">Kurzoption (`-r`) für `--cluster-name` zur Angabe des Clusternamens im Befehl `job create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3611">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="018bf-3612">Cloud</span><span class="sxs-lookup"><span data-stu-id="018bf-3612">Cloud</span></span>

* <span data-ttu-id="018bf-3613">`cloud [register|update]` geändert, um die Registrierung von Clouds ohne erforderliche Endpunkte zu verhindern</span><span class="sxs-lookup"><span data-stu-id="018bf-3613">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="018bf-3614">Container</span><span class="sxs-lookup"><span data-stu-id="018bf-3614">Container</span></span>

* <span data-ttu-id="018bf-3615">Unterstützung für das Öffnen mehrerer Ports hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3615">Added support to open multiple ports</span></span>
* <span data-ttu-id="018bf-3616">Neustartrichtlinie für Containergruppen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3616">Added container group restart policy</span></span>
* <span data-ttu-id="018bf-3617">Unterstützung zum Einbinden einer Azure-Dateifreigabe als Volume hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3617">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="018bf-3618">Hilfedokumente aktualisiert</span><span class="sxs-lookup"><span data-stu-id="018bf-3618">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="018bf-3619">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="018bf-3619">Data Lake Analytics</span></span>

* <span data-ttu-id="018bf-3620">`[job|account] list` geändert, um präzisere Informationen zu erhalten</span><span class="sxs-lookup"><span data-stu-id="018bf-3620">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="018bf-3621">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="018bf-3621">Data Lake Store</span></span>

* <span data-ttu-id="018bf-3622">`account list` geändert, um präzisere Informationen zu erhalten</span><span class="sxs-lookup"><span data-stu-id="018bf-3622">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="018bf-3623">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="018bf-3623">Extension</span></span>

* <span data-ttu-id="018bf-3624">`extension list-available` hinzugefügt, um das Auflisten offizieller Microsoft-Erweiterungen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="018bf-3624">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="018bf-3625">`--name` zu `extension [add|update]` hinzugefügt, um das Installieren von Erweiterungen nach Name zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="018bf-3625">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="018bf-3626">IoT</span><span class="sxs-lookup"><span data-stu-id="018bf-3626">IoT</span></span>

* <span data-ttu-id="018bf-3627">Unterstützung für Zertifizierungsstellen (CAs) und Zertifikatketten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3627">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="018bf-3628">Überwachen</span><span class="sxs-lookup"><span data-stu-id="018bf-3628">Monitor</span></span>

* <span data-ttu-id="018bf-3629">Befehle vom Typ `activity-log alert` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3629">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="018bf-3630">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="018bf-3630">Network</span></span>

* <span data-ttu-id="018bf-3631">Unterstützung für CAA-DNS-Einträge hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3631">Added support for CAA DNS records</span></span>
* <span data-ttu-id="018bf-3632">Problem behoben, durch das Endpunkte nicht mit `traffic-manager profile update` aktualisiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="018bf-3632">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="018bf-3633">Problem behoben, durch das `vnet update --dns-servers` je nach VNet-Erstellungsmethode nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="018bf-3633">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="018bf-3634">Problem behoben, durch das relative DNS-Namen durch `dns zone import` nicht korrekt importiert wurden</span><span class="sxs-lookup"><span data-stu-id="018bf-3634">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="018bf-3635">Reservations</span><span class="sxs-lookup"><span data-stu-id="018bf-3635">Reservations</span></span>

* <span data-ttu-id="018bf-3636">Erste Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="018bf-3636">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="018bf-3637">Resource</span><span class="sxs-lookup"><span data-stu-id="018bf-3637">Resource</span></span>

* <span data-ttu-id="018bf-3638">Unterstützung für Ressourcen-IDs zum Parameter `--resource` und Sperren auf Ressourcenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3638">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="018bf-3639">SQL</span><span class="sxs-lookup"><span data-stu-id="018bf-3639">SQL</span></span>

* <span data-ttu-id="018bf-3640">Parameter `--ignore-missing-vnet-service-endpoint` zu `sql server vnet-rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3640">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="018bf-3641">Storage</span><span class="sxs-lookup"><span data-stu-id="018bf-3641">Storage</span></span>

* <span data-ttu-id="018bf-3642">`storage account create` geändert, sodass die SKU `Standard_RAGRS` als Standard verwendet wird</span><span class="sxs-lookup"><span data-stu-id="018bf-3642">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="018bf-3643">Fehler im Zusammenhang mit Datei-/Blobnamen korrigiert, die ASCII-fremde Zeichen enthalten</span><span class="sxs-lookup"><span data-stu-id="018bf-3643">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="018bf-3644">Fehler korrigiert, der die Verwendung von `--source-uri` mit `storage [blob|file] copy start-batch` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="018bf-3644">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="018bf-3645">Befehle zum Globalisieren und Löschen mehrerer Objekte mit `storage [blob|file] delete-batch` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3645">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="018bf-3646">Problem beim Aktivieren von Metriken mit `storage metrics update` behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-3646">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="018bf-3647">Problem mit Dateien über 200 GB bei Verwendung von `storage blob upload-batch` behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-3647">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="018bf-3648">Problem behoben, durch das `--bypass` und `--default-action` von `storage account [create|update]` ignoriert wurden</span><span class="sxs-lookup"><span data-stu-id="018bf-3648">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="018bf-3649">VM</span><span class="sxs-lookup"><span data-stu-id="018bf-3649">VM</span></span>

* <span data-ttu-id="018bf-3650">Fehler mit `vmss create` korrigiert, der die Verwendung der Größenebene `Basic` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="018bf-3650">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="018bf-3651">`--plan`-Argumente zu `[vm|vmss] create` für benutzerdefinierte Images mit Abrechnungsinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3651">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="018bf-3652">Befehle hinzugefügt: `vm secret `[add|remove|list]</span><span class="sxs-lookup"><span data-stu-id="018bf-3652">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="018bf-3653">`vm format-secret` in `vm secret format` umbenannt</span><span class="sxs-lookup"><span data-stu-id="018bf-3653">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="018bf-3654">Argument `--encrypt format` zu `vm encryption enable` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3654">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="018bf-3655">24. Oktober 2017</span><span class="sxs-lookup"><span data-stu-id="018bf-3655">October 24, 2017</span></span>

<span data-ttu-id="018bf-3656">Version 2.0.20</span><span class="sxs-lookup"><span data-stu-id="018bf-3656">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="018bf-3657">Core</span><span class="sxs-lookup"><span data-stu-id="018bf-3657">Core</span></span>

* <span data-ttu-id="018bf-3658">Aktualisierung von `2017-03-09-profile` zur Verwendung von Version `2016-01-01` der `MGMT_STORAGE`-API</span><span class="sxs-lookup"><span data-stu-id="018bf-3658">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="018bf-3659">ACR</span><span class="sxs-lookup"><span data-stu-id="018bf-3659">ACR</span></span>

* <span data-ttu-id="018bf-3660">Die Ressourcenverwaltung wurde aktualisiert und verweist nun auf die API-Version `2017-10-01`.</span><span class="sxs-lookup"><span data-stu-id="018bf-3660">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="018bf-3661">SKU „Bring Your Own Storage“ wurde in „Klassisch“ geändert.</span><span class="sxs-lookup"><span data-stu-id="018bf-3661">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="018bf-3662">Die Registrierungs-SKUs wurden in „Basic“, „Standard“ und „Premium“ umbenannt.</span><span class="sxs-lookup"><span data-stu-id="018bf-3662">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="018bf-3663">ACS</span><span class="sxs-lookup"><span data-stu-id="018bf-3663">ACS</span></span>

* <span data-ttu-id="018bf-3664">[VORSCHAUVERSION] Befehle vom Typ `az aks` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3664">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="018bf-3665">Problem mit `get-credentials` in Kubernetes behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-3665">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="018bf-3666">AppService</span><span class="sxs-lookup"><span data-stu-id="018bf-3666">Appservice</span></span>

* <span data-ttu-id="018bf-3667">Problem behoben, aufgrund dessen heruntergeladene `webapp`-Protokolle unter Umständen ungültig waren</span><span class="sxs-lookup"><span data-stu-id="018bf-3667">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="018bf-3668">Komponente</span><span class="sxs-lookup"><span data-stu-id="018bf-3668">Component</span></span>

* <span data-ttu-id="018bf-3669">Deutlichere Meldung zur Einstellung für alle Installer und für Bestätigungsaufforderung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3669">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="018bf-3670">Überwachen</span><span class="sxs-lookup"><span data-stu-id="018bf-3670">Monitor</span></span>

* <span data-ttu-id="018bf-3671">Befehle vom Typ `action-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3671">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="018bf-3672">Resource</span><span class="sxs-lookup"><span data-stu-id="018bf-3672">Resource</span></span>

* <span data-ttu-id="018bf-3673">Inkompatibilität mit der aktuellen Version der msrest-Abhängigkeit in `group export` behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-3673">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="018bf-3674">Problem mit `policy assignment create` behoben, sodass der Befehl mit integrierten Richtliniendefinitionen und Richtliniensatzdefinitionen verwendet werden kann</span><span class="sxs-lookup"><span data-stu-id="018bf-3674">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="018bf-3675">VM</span><span class="sxs-lookup"><span data-stu-id="018bf-3675">VM</span></span>

* <span data-ttu-id="018bf-3676">Argument `--accelerated-networking` zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3676">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="018bf-3677">9\. Oktober 2017</span><span class="sxs-lookup"><span data-stu-id="018bf-3677">October 9, 2017</span></span>

<span data-ttu-id="018bf-3678">Version 2.0.19</span><span class="sxs-lookup"><span data-stu-id="018bf-3678">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="018bf-3679">Core</span><span class="sxs-lookup"><span data-stu-id="018bf-3679">Core</span></span>

* <span data-ttu-id="018bf-3680">Verarbeitung von ADFS-Autoritäts-URLs wurde mit einem nachgestellten Schrägstrich zu Azure Stack hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-3680">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="018bf-3681">AppService</span><span class="sxs-lookup"><span data-stu-id="018bf-3681">Appservice</span></span>

* <span data-ttu-id="018bf-3682">Mit dem neuen Befehl `webapp update` wurde ein allgemeines Update hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-3682">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="018bf-3683">Batch</span><span class="sxs-lookup"><span data-stu-id="018bf-3683">Batch</span></span>

* <span data-ttu-id="018bf-3684">Aktualisierung auf Batch SDK 4.0.0</span><span class="sxs-lookup"><span data-stu-id="018bf-3684">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="018bf-3685">Die Option `--image` von „VirtualMachineConfiguration“ wurde aktualisiert, um zusätzlich zu „publish:offer:sku:version“ ARM-Imageverweise zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="018bf-3685">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="018bf-3686">Unterstützung für das neue CLI-Erweiterungsmodell für Batch-Erweiterungsbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3686">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="018bf-3687">Batch-Unterstützung aus dem Komponentenmodell entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-3687">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="018bf-3688">BatchAI</span><span class="sxs-lookup"><span data-stu-id="018bf-3688">Batchai</span></span>

* <span data-ttu-id="018bf-3689">Erste Version des Batch KI-Moduls</span><span class="sxs-lookup"><span data-stu-id="018bf-3689">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="018bf-3690">KeyVault</span><span class="sxs-lookup"><span data-stu-id="018bf-3690">Keyvault</span></span>

* <span data-ttu-id="018bf-3691">Key Vault-Authentifizierungsproblem behoben, das bei Verwendung von ADFS in Azure Stack auftrat.</span><span class="sxs-lookup"><span data-stu-id="018bf-3691">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="018bf-3692">(#4448)</span><span class="sxs-lookup"><span data-stu-id="018bf-3692">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="018bf-3693">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="018bf-3693">Network</span></span>

* <span data-ttu-id="018bf-3694">Das Argument `--server` von `application-gateway address-pool create` ist nun optional, sodass leere Adresspools zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="018bf-3694">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="018bf-3695">`traffic-manager` wurde aktualisiert, um aktuelle Features zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="018bf-3695">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="018bf-3696">Resource</span><span class="sxs-lookup"><span data-stu-id="018bf-3696">Resource</span></span>

* <span data-ttu-id="018bf-3697">Zusätzliche Unterstützung für `--resource-group/-g`-Optionen für Ressourcengruppennamen zu `group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3697">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="018bf-3698">Befehle für `account lock` hinzugefügt, um die Verwendung mit Sperren auf Abonnementebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="018bf-3698">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="018bf-3699">Befehle für `group lock` hinzugefügt, um die Verwendung mit Sperren auf Gruppenebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="018bf-3699">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="018bf-3700">Befehle für `resource lock` hinzugefügt, um die Verwendung mit Sperren auf Ressourcenebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="018bf-3700">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="018bf-3701">Sql</span><span class="sxs-lookup"><span data-stu-id="018bf-3701">Sql</span></span>

* <span data-ttu-id="018bf-3702">Unterstützung für SQL Transparent Data Encryption (TDE) und TDE für Bring Your Own Key-Szenarien hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3702">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="018bf-3703">Der Befehl `db list-deleted` und der Parameter `db restore --deleted-time` wurden hinzugefügt, um die Ermittlung und Wiederherstellung gelöschter Datenbanken zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="018bf-3703">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="018bf-3704">`db op list` und `db op cancel` wurden hinzugefügt, um das Auflisten und Abbrechen ausgeführter Vorgänge für eine Datenbank zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="018bf-3704">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="018bf-3705">Storage</span><span class="sxs-lookup"><span data-stu-id="018bf-3705">Storage</span></span>

* <span data-ttu-id="018bf-3706">Unterstützung für Momentaufnahme von Dateifreigaben hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3706">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="018bf-3707">VM</span><span class="sxs-lookup"><span data-stu-id="018bf-3707">Vm</span></span>

* <span data-ttu-id="018bf-3708">Korrektur eines Fehlers in `vm show`, bei dem die Verwendung von `-d` in Verbindung mit fehlenden privaten IP-Adressen einen Absturz verursachte</span><span class="sxs-lookup"><span data-stu-id="018bf-3708">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="018bf-3709">[VORSCHAUVERSION] Unterstützung für paralleles Upgrade zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3709">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="018bf-3710">Unterstützung für das Aktualisieren der Verschlüsselungseinstellungen mit `vm encryption enable` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3710">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="018bf-3711">Parameter `--os-disk-size-gb` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3711">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="018bf-3712">Parameter `--license-type` für Windows zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3712">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="018bf-3713">22. September 2017</span><span class="sxs-lookup"><span data-stu-id="018bf-3713">September 22, 2017</span></span>

<span data-ttu-id="018bf-3714">Version 2.0.18</span><span class="sxs-lookup"><span data-stu-id="018bf-3714">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="018bf-3715">Resource</span><span class="sxs-lookup"><span data-stu-id="018bf-3715">Resource</span></span>

* <span data-ttu-id="018bf-3716">Unterstützung für das Anzeigen integrierter Richtliniendefinitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3716">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="018bf-3717">Unterstützungsmodusparameter zum Erstellen von Richtliniendefinitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3717">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="018bf-3718">Unterstützung für UI-Definitionen und -Vorlagen zu `managedapp definition create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3718">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="018bf-3719">[BREAKING CHANGE] Der Ressourcentyp `managedapp` wurde von `appliances` in `applications` und von `applianceDefinitions` in `applicationDefinitions` geändert.</span><span class="sxs-lookup"><span data-stu-id="018bf-3719">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="018bf-3720">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="018bf-3720">Network</span></span>

* <span data-ttu-id="018bf-3721">Unterstützung für Verfügbarkeitszone zu Unterbefehlen `network lb` und `network public-ip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3721">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="018bf-3722">Unterstützung für IPv6-Microsoft-Peering zu `express-route` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3722">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="018bf-3723">Befehle für Anwendungssicherheitsgruppe `asg` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3723">Added `asg` application security group commands</span></span>
* <span data-ttu-id="018bf-3724">Argument `--application-security-groups` zu `nic [create|ip-config create|ip-config update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3724">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="018bf-3725">Argumente `--source-asgs` und `--destination-asgs` zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3725">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="018bf-3726">Argumente `--ddos-protection` und `--vm-protection` zu `vnet [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3726">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="018bf-3727">Befehle vom Typ `network [vnet-gateway|vpn-client|show-url]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3727">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="018bf-3728">Storage</span><span class="sxs-lookup"><span data-stu-id="018bf-3728">Storage</span></span>

* <span data-ttu-id="018bf-3729">Problem behoben, das nach der Aktualisierung des SDK unter Umständen einen Fehler der `storage account network-rule`-Befehle zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="018bf-3729">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="018bf-3730">Eventgrid</span><span class="sxs-lookup"><span data-stu-id="018bf-3730">Eventgrid</span></span>

* <span data-ttu-id="018bf-3731">Azure Event Grid Python SDK für die Verwendung der neueren API-Version „2017-09-15-preview“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="018bf-3731">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="018bf-3732">SQL</span><span class="sxs-lookup"><span data-stu-id="018bf-3732">SQL</span></span>

* <span data-ttu-id="018bf-3733">`sql server list`-Argument `--resource-group` geändert, sodass es nun optional ist.</span><span class="sxs-lookup"><span data-stu-id="018bf-3733">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="018bf-3734">Wird es nicht angegeben, werden alle SQL Server-Instanzen im Abonnement zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="018bf-3734">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="018bf-3735">Parameter `--no-wait` zu `db [create|copy|restore|update|replica create|create|update]` und `dw [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3735">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="018bf-3736">KeyVault</span><span class="sxs-lookup"><span data-stu-id="018bf-3736">Keyvault</span></span>

* <span data-ttu-id="018bf-3737">Unterstützung für die Keyvault-Befehlsausführung hinter einem Proxy hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3737">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="018bf-3738">VM</span><span class="sxs-lookup"><span data-stu-id="018bf-3738">VM</span></span>

* <span data-ttu-id="018bf-3739">Unterstützung für Verfügbarkeitszone zu `[vm|vmss|disk] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3739">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="018bf-3740">Problem behoben, das bei Verwendung von `--app-gateway ID` mit `vmss create` einen Fehler zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="018bf-3740">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="018bf-3741">Argument `--asgs` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3741">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="018bf-3742">Unterstützung für die Ausführung von Befehlen auf virtuellen Computern mit `vm run-command` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3742">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="018bf-3743">[VORSCHAU] Unterstützung für VMSS-Datenträgerverschlüsselung mit `vmss encryption` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3743">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="018bf-3744">Unterstützung für die Durchführung der Wartung auf virtuellen Computern mit `vm perform-maintenance` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3744">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="018bf-3745">ACS</span><span class="sxs-lookup"><span data-stu-id="018bf-3745">ACS</span></span>

* <span data-ttu-id="018bf-3746">[VORSCHAU] Argument `--orchestrator-release` zu `acs create` für ACS-Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3746">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="018bf-3747">AppService</span><span class="sxs-lookup"><span data-stu-id="018bf-3747">Appservice</span></span>

* <span data-ttu-id="018bf-3748">Neue Möglichkeit zum Aktualisieren und Anzeigen der Authentifizierungseinstellungen mit `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="018bf-3748">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="018bf-3749">Backup</span><span class="sxs-lookup"><span data-stu-id="018bf-3749">Backup</span></span>

* <span data-ttu-id="018bf-3750">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="018bf-3750">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="018bf-3751">11. September 2017</span><span class="sxs-lookup"><span data-stu-id="018bf-3751">September 11, 2017</span></span>

<span data-ttu-id="018bf-3752">Version 2.0.17</span><span class="sxs-lookup"><span data-stu-id="018bf-3752">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="018bf-3753">Core</span><span class="sxs-lookup"><span data-stu-id="018bf-3753">Core</span></span>

* <span data-ttu-id="018bf-3754">Festlegung einer eigenen Korrelations-ID in Telemetrie durch das Befehlsmodul aktiviert</span><span class="sxs-lookup"><span data-stu-id="018bf-3754">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="018bf-3755">Ein Problem mit der JSON-Sicherungsdatei wurde behoben, das beim Festlegen des Diagnosemodus für Telemetrie auftrat</span><span class="sxs-lookup"><span data-stu-id="018bf-3755">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="018bf-3756">ACS</span><span class="sxs-lookup"><span data-stu-id="018bf-3756">Acs</span></span>

* <span data-ttu-id="018bf-3757">Befehl `acs list-locations` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3757">Added `acs list-locations` command</span></span>
* <span data-ttu-id="018bf-3758">`ssh-key-file` wird mit dem erwarteten Standardwert versehen.</span><span class="sxs-lookup"><span data-stu-id="018bf-3758">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="018bf-3759">AppService</span><span class="sxs-lookup"><span data-stu-id="018bf-3759">Appservice</span></span>

* <span data-ttu-id="018bf-3760">Neue Möglichkeit zum Erstellen einer Web-App in einer anderen Ressourcengruppe als der des aktiven Diensttarifs</span><span class="sxs-lookup"><span data-stu-id="018bf-3760">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="018bf-3761">CDN</span><span class="sxs-lookup"><span data-stu-id="018bf-3761">CDN</span></span>

* <span data-ttu-id="018bf-3762">Der Fehler bei `cdn custom-domain create`, dass „CustomDomain“ nicht wiederholbar ist, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="018bf-3762">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="018bf-3763">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="018bf-3763">Extension</span></span>

* <span data-ttu-id="018bf-3764">Erstrelease</span><span class="sxs-lookup"><span data-stu-id="018bf-3764">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="018bf-3765">KeyVault</span><span class="sxs-lookup"><span data-stu-id="018bf-3765">Keyvault</span></span>

* <span data-ttu-id="018bf-3766">Problem behoben, aufgrund dessen bei den Berechtigungen für `keyvault set-policy` die Groß-/Kleinschreibung beachtet werden musste</span><span class="sxs-lookup"><span data-stu-id="018bf-3766">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="018bf-3767">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="018bf-3767">Network</span></span>

* <span data-ttu-id="018bf-3768">`vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="018bf-3768">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="018bf-3769">Das Argument `--private-access-services` wurde für `vnet subnet create/update` in `--service-endpoints` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="018bf-3769">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="018bf-3770">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3770">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="018bf-3771">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3771">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="018bf-3772">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3772">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="018bf-3773">Resource</span><span class="sxs-lookup"><span data-stu-id="018bf-3773">Resource</span></span>

* <span data-ttu-id="018bf-3774">Übergabe von Parameterdefinitionen für Ressourcenrichtlinien in `policy definition create` und `policy definition update` zulassen</span><span class="sxs-lookup"><span data-stu-id="018bf-3774">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="018bf-3775">Übergabe von Parameterwerten für `policy assignment create` zulassen</span><span class="sxs-lookup"><span data-stu-id="018bf-3775">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="018bf-3776">Übergabe von JSON-Code oder einer Datei für alle Parameter zulassen</span><span class="sxs-lookup"><span data-stu-id="018bf-3776">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="018bf-3777">Inkrementierte API-Version</span><span class="sxs-lookup"><span data-stu-id="018bf-3777">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="018bf-3778">SQL</span><span class="sxs-lookup"><span data-stu-id="018bf-3778">SQL</span></span>

* <span data-ttu-id="018bf-3779">Befehle vom Typ `sql server vnet-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3779">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="018bf-3780">VM</span><span class="sxs-lookup"><span data-stu-id="018bf-3780">VM</span></span>

* <span data-ttu-id="018bf-3781">Behoben: Zugriff nur zuweisen, wenn `--scope` angegeben wird</span><span class="sxs-lookup"><span data-stu-id="018bf-3781">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="018bf-3782">Behoben: Gleiche Erweiterungsbenennung wie Portal verwenden</span><span class="sxs-lookup"><span data-stu-id="018bf-3782">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="018bf-3783">`subscription` aus der Ausgabe von `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-3783">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="018bf-3784">Behoben: Speicher-SKU vom Typ `[vm|vmss] create` wird nicht auf Datenträger mit einem Image angewendet.</span><span class="sxs-lookup"><span data-stu-id="018bf-3784">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="018bf-3785">Behoben: `vm format-secret --secrets` akzeptierte keine durch neue Zeilen getrennte IDs.</span><span class="sxs-lookup"><span data-stu-id="018bf-3785">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="018bf-3786">31. August 2017</span><span class="sxs-lookup"><span data-stu-id="018bf-3786">August 31, 2017</span></span>

<span data-ttu-id="018bf-3787">Version 2.0.16</span><span class="sxs-lookup"><span data-stu-id="018bf-3787">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="018bf-3788">KeyVault</span><span class="sxs-lookup"><span data-stu-id="018bf-3788">Keyvault</span></span>

* <span data-ttu-id="018bf-3789">Fehler behoben, der beim Versuch auftrat, die Geheimniscodierung mit `secret download` automatisch aufzulösen</span><span class="sxs-lookup"><span data-stu-id="018bf-3789">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="018bf-3790">Sf</span><span class="sxs-lookup"><span data-stu-id="018bf-3790">Sf</span></span>

* <span data-ttu-id="018bf-3791">Alle Befehle wurden durch die Service Fabric-Befehlszeilenschnittstelle (sfctl) ersetzt.</span><span class="sxs-lookup"><span data-stu-id="018bf-3791">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="018bf-3792">Storage</span><span class="sxs-lookup"><span data-stu-id="018bf-3792">Storage</span></span>

* <span data-ttu-id="018bf-3793">Problem behoben, aufgrund dessen Speicherkonten nicht in Regionen erstellt werden konnten, die die NetworkACLs-Funktion nicht unterstützen</span><span class="sxs-lookup"><span data-stu-id="018bf-3793">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="018bf-3794">Festlegen des Inhaltstyps und der Inhaltscodierung während Blob- und Dateiuploads, wenn weder Inhaltstyp noch Inhaltscodierung angegeben sind</span><span class="sxs-lookup"><span data-stu-id="018bf-3794">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="018bf-3795">28. August 2017</span><span class="sxs-lookup"><span data-stu-id="018bf-3795">August 28, 2017</span></span>

<span data-ttu-id="018bf-3796">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="018bf-3796">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="018bf-3797">Befehlszeilenschnittstelle (CLI)</span><span class="sxs-lookup"><span data-stu-id="018bf-3797">CLI</span></span>

* <span data-ttu-id="018bf-3798">Rechtlichen Hinweis zu `--version` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3798">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="018bf-3799">ACS</span><span class="sxs-lookup"><span data-stu-id="018bf-3799">ACS</span></span>

* <span data-ttu-id="018bf-3800">Vorschauregionen korrigiert</span><span class="sxs-lookup"><span data-stu-id="018bf-3800">Corrected preview regions</span></span>
* <span data-ttu-id="018bf-3801">Standardmäßiges DNS-Namenspräfix (`dns_name_prefix`) ordnungsgemäß formatiert</span><span class="sxs-lookup"><span data-stu-id="018bf-3801">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="018bf-3802">ACS-Befehlsausgabe optimiert</span><span class="sxs-lookup"><span data-stu-id="018bf-3802">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="018bf-3803">AppService</span><span class="sxs-lookup"><span data-stu-id="018bf-3803">Appservice</span></span>

* <span data-ttu-id="018bf-3804">[BREAKING CHANGE] Inkonsistenzen in der Ausgabe von `az webapp config appsettings [delete|set]` behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-3804">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="018bf-3805">Neuen Alias (`-i`) für `az webapp config container set --docker-custom-image-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3805">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="018bf-3806">`az webapp log show` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="018bf-3806">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="018bf-3807">Neue Argumente aus `az webapp delete` verfügbar gemacht, um App Service-Plan, Metriken oder DNS-Registrierung beizubehalten</span><span class="sxs-lookup"><span data-stu-id="018bf-3807">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="018bf-3808">Behoben: Korrekte Erkennung der Sloteinstellungen</span><span class="sxs-lookup"><span data-stu-id="018bf-3808">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="018bf-3809">IoT</span><span class="sxs-lookup"><span data-stu-id="018bf-3809">IoT</span></span>

* <span data-ttu-id="018bf-3810">#3934 behoben: Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="018bf-3810">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="018bf-3811">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="018bf-3811">Network</span></span>

* <span data-ttu-id="018bf-3812">[BREAKING CHANGE]`vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="018bf-3812">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="018bf-3813">[BREAKING CHANGE] Option `--private-access-services` für `--service-endpoints` in `vnet subnet [create|update]` umbenannt</span><span class="sxs-lookup"><span data-stu-id="018bf-3813">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="018bf-3814">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3814">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="018bf-3815">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3815">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="018bf-3816">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3816">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="018bf-3817">Profil</span><span class="sxs-lookup"><span data-stu-id="018bf-3817">Profile</span></span>

* <span data-ttu-id="018bf-3818">`--msi` und `--msi-port` für die Anmeldung mit der Identität eines virtuellen Computers verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="018bf-3818">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="018bf-3819">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="018bf-3819">Service Fabric</span></span>

* <span data-ttu-id="018bf-3820">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="018bf-3820">Preview release</span></span>
* <span data-ttu-id="018bf-3821">Registrierungsbenutzer-/-kennwortregeln für Befehl vereinfacht</span><span class="sxs-lookup"><span data-stu-id="018bf-3821">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="018bf-3822">Kennwortanforderung für Benutzer trotz Parameterübergabe behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-3822">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="018bf-3823">Unterstützung für leere Registrierungsanmeldeinformationen (`registry_cred`) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3823">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="018bf-3824">Storage</span><span class="sxs-lookup"><span data-stu-id="018bf-3824">Storage</span></span>

* <span data-ttu-id="018bf-3825">Festlegen des Blobtarifs ermöglicht</span><span class="sxs-lookup"><span data-stu-id="018bf-3825">Enabled setting blob tier</span></span>
* <span data-ttu-id="018bf-3826">Argumente `--bypass` und `--default-action` zur Unterstützung von Diensttunneling zu `storage account [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3826">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="018bf-3827">Befehle zum Hinzufügen von VNet-Regeln und IP-basierten Regeln zu `storage account network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3827">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="018bf-3828">Dienstverschlüsselung durch vom Kunden verwalteten Schlüssel ermöglicht</span><span class="sxs-lookup"><span data-stu-id="018bf-3828">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="018bf-3829">[BREAKING CHANGE] Option `--encryption` für Befehl `az storage account create and az storage account update` in `--encryption-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="018bf-3829">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="018bf-3830">Behoben (4220): `az storage account update encryption` – Syntaxkonflikt</span><span class="sxs-lookup"><span data-stu-id="018bf-3830">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="018bf-3831">VM</span><span class="sxs-lookup"><span data-stu-id="018bf-3831">VM</span></span>

* <span data-ttu-id="018bf-3832">Problem behoben, aufgrund dessen bei Verwendung von `--instance-id *` zusätzliche, fehlerhafte Informationen für `vmss get-instance-view` angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="018bf-3832">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="018bf-3833">Unterstützung für `--lb-sku` zu `vmss create` hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="018bf-3833">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="018bf-3834">Menschliche Namen aus der Administratornamen-Blacklist für `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-3834">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="018bf-3835">Problem behoben, aufgrund dessen `[vm|vmss] create` einen Fehler ausgelöst hat, wenn aus einem Image keine Tarifinformationen extrahiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="018bf-3835">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="018bf-3836">Absturzproblem beim Erstellen einer VMMS-Skalierungsgruppe mit einem internen Lastenausgleich behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-3836">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="018bf-3837">Problem behoben, aufgrund dessen das Argument `--no-wait` nicht mit `vm availability-set create` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="018bf-3837">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="018bf-3838">15. August 2017</span><span class="sxs-lookup"><span data-stu-id="018bf-3838">August 15, 2017</span></span>

<span data-ttu-id="018bf-3839">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="018bf-3839">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="018bf-3840">ACS</span><span class="sxs-lookup"><span data-stu-id="018bf-3840">ACS</span></span>

* <span data-ttu-id="018bf-3841">sshMaster0-Portnummer für Kubernetes korrigiert</span><span class="sxs-lookup"><span data-stu-id="018bf-3841">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="018bf-3842">AppService</span><span class="sxs-lookup"><span data-stu-id="018bf-3842">Appservice</span></span>

* <span data-ttu-id="018bf-3843">Ausnahme beim Erstellen einer neuen Git-basierten Linux-Web-App behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-3843">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="018bf-3844">Event Grid</span><span class="sxs-lookup"><span data-stu-id="018bf-3844">Event Grid</span></span>

* <span data-ttu-id="018bf-3845">SDK-Abhängigkeiten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3845">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="018bf-3846">11. August 2017</span><span class="sxs-lookup"><span data-stu-id="018bf-3846">August 11, 2017</span></span>

<span data-ttu-id="018bf-3847">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="018bf-3847">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="018bf-3848">ACS</span><span class="sxs-lookup"><span data-stu-id="018bf-3848">ACS</span></span>

* <span data-ttu-id="018bf-3849">Weitere Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3849">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="018bf-3850">Batch</span><span class="sxs-lookup"><span data-stu-id="018bf-3850">Batch</span></span>

* <span data-ttu-id="018bf-3851">Auf Batch SDK 3.1.0 und Batch Management SDK 4.1.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="018bf-3851">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="018bf-3852">Neuen Befehl zum Anzeigen der Aufgabenanzahl eines Auftrags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3852">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="018bf-3853">Fehler in der SAS-URL-Verarbeitung der Ressourcendatei behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-3853">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="018bf-3854">Batch-Kontoendpunkt unterstützt nun optionales Präfix „https://“</span><span class="sxs-lookup"><span data-stu-id="018bf-3854">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="018bf-3855">Unterstützung für das Hinzufügen von Listen mit mehr als 100 Aufgaben zu einem Auftrag</span><span class="sxs-lookup"><span data-stu-id="018bf-3855">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="018bf-3856">Debugprotokollierung für das Laden des Erweiterungsbefehlsmoduls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3856">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="018bf-3857">Komponente</span><span class="sxs-lookup"><span data-stu-id="018bf-3857">Component</span></span>

* <span data-ttu-id="018bf-3858">Warnung für veraltete Befehle vom Typ „az component“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3858">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="018bf-3859">Container</span><span class="sxs-lookup"><span data-stu-id="018bf-3859">Container</span></span>

* <span data-ttu-id="018bf-3860">`create`: Problem behoben, aufgrund dessen das Gleichheitszeichen innerhalb einer Umgebungsvariablen nicht zulässig war</span><span class="sxs-lookup"><span data-stu-id="018bf-3860">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="018bf-3861">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="018bf-3861">Data Lake Store</span></span>

* <span data-ttu-id="018bf-3862">Fortschrittsüberwachung ermöglicht</span><span class="sxs-lookup"><span data-stu-id="018bf-3862">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="018bf-3863">Event Grid</span><span class="sxs-lookup"><span data-stu-id="018bf-3863">Event Grid</span></span>

* <span data-ttu-id="018bf-3864">Erste Veröffentlichung</span><span class="sxs-lookup"><span data-stu-id="018bf-3864">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="018bf-3865">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="018bf-3865">Network</span></span>

* <span data-ttu-id="018bf-3866">`lb`: Problem behoben, aufgrund dessen bestimmte Namen untergeordneter Ressourcen bei Auslassung nicht richtig aufgelöst wurden</span><span class="sxs-lookup"><span data-stu-id="018bf-3866">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="018bf-3867">`application-gateway {subresource} delete`: Problem behoben, aufgrund dessen `--no-wait` nicht berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="018bf-3867">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="018bf-3868">`application-gateway http-settings update`: Problem behoben, aufgrund dessen `--connection-draining-timeout` nicht deaktiviert werden konnte</span><span class="sxs-lookup"><span data-stu-id="018bf-3868">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="018bf-3869">Fehler behoben: Unerwartetes Schlüsselwortargument `sa_data_size_kilobyes` bei `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="018bf-3869">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="018bf-3870">Profil</span><span class="sxs-lookup"><span data-stu-id="018bf-3870">Profile</span></span>

* <span data-ttu-id="018bf-3871">`account list`: `--refresh` hinzugefügt, um die neuesten Abonnements vom Server zu synchronisieren</span><span class="sxs-lookup"><span data-stu-id="018bf-3871">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="018bf-3872">Storage</span><span class="sxs-lookup"><span data-stu-id="018bf-3872">Storage</span></span>

* <span data-ttu-id="018bf-3873">Aktualisieren des Speicherkontos mit vom System zugewiesener Identität ermöglicht</span><span class="sxs-lookup"><span data-stu-id="018bf-3873">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="018bf-3874">VM</span><span class="sxs-lookup"><span data-stu-id="018bf-3874">VM</span></span>

* <span data-ttu-id="018bf-3875">`availability-set`: Fehlerdomänenanzahl bei Konvertierung verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="018bf-3875">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="018bf-3876">Befehl `list-skus` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="018bf-3876">Exposed `list-skus` command</span></span>
* <span data-ttu-id="018bf-3877">Unterstützung der Identitätszuweisung ohne Erstellung von Rollenzuweisungen</span><span class="sxs-lookup"><span data-stu-id="018bf-3877">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="018bf-3878">Anwenden von Speicher-SKU beim Anfügen von Datenträgern</span><span class="sxs-lookup"><span data-stu-id="018bf-3878">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="018bf-3879">Standardmäßiger Betriebssystemdatenträger-Name und Speicher-SKU bei Verwendung verwalteter Datenträger entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-3879">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="018bf-3880">28. Juli 2017</span><span class="sxs-lookup"><span data-stu-id="018bf-3880">July 28, 2017</span></span>

<span data-ttu-id="018bf-3881">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="018bf-3881">Version 2.0.12</span></span>

* <span data-ttu-id="018bf-3882">Containerbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3882">Added container commands</span></span>
* <span data-ttu-id="018bf-3883">Abrechnungs- und Nutzungsmodule hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3883">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="018bf-3884">Core</span><span class="sxs-lookup"><span data-stu-id="018bf-3884">Core</span></span>

* <span data-ttu-id="018bf-3885">Ausgabe von SDK-Authentifizierungsinformationen für Dienstprinzipale mit Zertifikaten</span><span class="sxs-lookup"><span data-stu-id="018bf-3885">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="018bf-3886">Ausnahmen beim Bereitstellungsfortschritt behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-3886">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="018bf-3887">Verwendung des ARM-Endpunkts aus der aktuellen Cloud für die Erstellung des Abonnementclients</span><span class="sxs-lookup"><span data-stu-id="018bf-3887">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="018bf-3888">Gleichzeitige Verarbeitung der Datei „clouds.config“ verbessert (3636)</span><span class="sxs-lookup"><span data-stu-id="018bf-3888">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="018bf-3889">Aktualisierung der Clientanforderungs-ID für jede Befehlsausführung</span><span class="sxs-lookup"><span data-stu-id="018bf-3889">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="018bf-3890">Erstellung von Abonnementclients mit richtigem SDK-Profil (3635)</span><span class="sxs-lookup"><span data-stu-id="018bf-3890">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="018bf-3891">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="018bf-3891">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="018bf-3892">Unterstützung für Auswahl von Tabellenausgabefeldern über jmespath Abfrage hinzugefügt (3581)</span><span class="sxs-lookup"><span data-stu-id="018bf-3892">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="018bf-3893">Stummschaltung von Analyseargumenten und Anfügeverlauf mit Gesten verbessert (3434)</span><span class="sxs-lookup"><span data-stu-id="018bf-3893">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="018bf-3894">Erstellung von Abonnementclients mit richtigem SDK-Profil</span><span class="sxs-lookup"><span data-stu-id="018bf-3894">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="018bf-3895">Verschiebung aller vorhandenen Erfassungsdateien in den neuesten Ordner</span><span class="sxs-lookup"><span data-stu-id="018bf-3895">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="018bf-3896">Idempotenz für VM-/VMSS-Erstellung behoben (3586)</span><span class="sxs-lookup"><span data-stu-id="018bf-3896">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="018bf-3897">Bei Befehlspfaden wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="018bf-3897">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="018bf-3898">Bei bestimmten booleschen Parametern wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="018bf-3898">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="018bf-3899">Unterstützung der Anmeldung bei lokalem AD FS-Server wie Azure Stack</span><span class="sxs-lookup"><span data-stu-id="018bf-3899">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="018bf-3900">Gleichzeitige Schreibvorgänge in „clouds.config“ behoben (3255)</span><span class="sxs-lookup"><span data-stu-id="018bf-3900">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="018bf-3901">ACR</span><span class="sxs-lookup"><span data-stu-id="018bf-3901">ACR</span></span>

* <span data-ttu-id="018bf-3902">Befehl `show-usage` für verwaltete Registrierungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3902">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="018bf-3903">Unterstützung der SKU-Aktualisierung für verwaltete Registrierungen</span><span class="sxs-lookup"><span data-stu-id="018bf-3903">Support SKU update for managed registries</span></span>
* <span data-ttu-id="018bf-3904">Verwaltete Registrierungen mit verwalteter SKU hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3904">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="018bf-3905">Webhooks für verwaltete Registrierungen mit ACR-Webhook-Befehlsmodul hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3905">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="018bf-3906">AAD-Authentifizierung mit ACR-Anmeldebefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3906">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="018bf-3907">Löschbefehl für Docker-Repositorys, Manifeste und Tags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3907">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="018bf-3908">ACS</span><span class="sxs-lookup"><span data-stu-id="018bf-3908">ACS</span></span>

* <span data-ttu-id="018bf-3909">Unterstützung der API-Version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="018bf-3909">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="018bf-3910">AppService</span><span class="sxs-lookup"><span data-stu-id="018bf-3910">Appservice</span></span>

* <span data-ttu-id="018bf-3911">Fehler behoben, aufgrund dessen die Auflistung der Linux-Web-App keine Werte zurückgegeben hat</span><span class="sxs-lookup"><span data-stu-id="018bf-3911">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="018bf-3912">Unterstützung für das Abrufen von Anmeldeinformationen aus dem ACR</span><span class="sxs-lookup"><span data-stu-id="018bf-3912">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="018bf-3913">Entfernung aller Befehle unter `appservice web`</span><span class="sxs-lookup"><span data-stu-id="018bf-3913">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="018bf-3914">Maskierung von Docker-Registrierungskennwörtern aus der Befehlsausgabe (3656)</span><span class="sxs-lookup"><span data-stu-id="018bf-3914">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="018bf-3915">Gewährleistung der fehlerfreien Verwendung des Standardbrowsers unter macOS (3623)</span><span class="sxs-lookup"><span data-stu-id="018bf-3915">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="018bf-3916">Verbesserung des Nutzens von `webapp log tail` und `webapp log download` (3624)</span><span class="sxs-lookup"><span data-stu-id="018bf-3916">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="018bf-3917">Befehl `traffic-routing` zum Konfigurieren des statischen Routings verfügbar gemacht (3566)</span><span class="sxs-lookup"><span data-stu-id="018bf-3917">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="018bf-3918">Zuverlässigkeit beim Konfigurieren der Quellcodeverwaltung verbessert (3245)</span><span class="sxs-lookup"><span data-stu-id="018bf-3918">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="018bf-3919">Nicht unterstütztes Argument `--node-version` aus `webapp config update` für Windows-Web-Apps entfernt.</span><span class="sxs-lookup"><span data-stu-id="018bf-3919">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="018bf-3920">Verwenden Sie stattdessen `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="018bf-3920">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="018bf-3921">Batch</span><span class="sxs-lookup"><span data-stu-id="018bf-3921">Batch</span></span>

* <span data-ttu-id="018bf-3922">Auf Batch SDK 3.0.0 mit Unterstützung virtueller Computer mit niedriger Priorität in Pools aktualisiert</span><span class="sxs-lookup"><span data-stu-id="018bf-3922">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="018bf-3923">`pool create`-Option `--target-dedicated` in `--target-dedicated-nodes` umbenannt</span><span class="sxs-lookup"><span data-stu-id="018bf-3923">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="018bf-3924">`pool create`-Optionen `--target-low-priority-nodes` und `--application-licenses` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3924">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="018bf-3925">CDN</span><span class="sxs-lookup"><span data-stu-id="018bf-3925">CDN</span></span>

* <span data-ttu-id="018bf-3926">Besser verständliche Fehlermeldung für `cdn endpoint list`, wenn das von `--profile-name` angegebene Profil nicht vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="018bf-3926">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="018bf-3927">Cloud</span><span class="sxs-lookup"><span data-stu-id="018bf-3927">Cloud</span></span>

* <span data-ttu-id="018bf-3928">API-Version des Cloudmetadaten-Endpunkts in das Format JJJJ-MM-TT umgewandelt</span><span class="sxs-lookup"><span data-stu-id="018bf-3928">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="018bf-3929">Katalogendpunkt nicht erforderlich</span><span class="sxs-lookup"><span data-stu-id="018bf-3929">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="018bf-3930">Unterstützung für die Cloudregistrierung nur mit ARM-Endpunkt</span><span class="sxs-lookup"><span data-stu-id="018bf-3930">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="018bf-3931">Option für `cloud set` bereitgestellt, um beim Auswählen der aktuellen Cloud das Profil auswählen zu können</span><span class="sxs-lookup"><span data-stu-id="018bf-3931">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="018bf-3932">`endpoint_vm_image_alias_doc` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="018bf-3932">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="018bf-3933">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="018bf-3933">CosmosDB</span></span>

* <span data-ttu-id="018bf-3934">Möglichkeit zum Erstellen einer Auflistung mit benutzerdefiniertem Partitionsschlüssel behoben</span><span class="sxs-lookup"><span data-stu-id="018bf-3934">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="018bf-3935">Unterstützung für Auflistungs-Standardgültigkeitsdauer hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3935">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="018bf-3936">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="018bf-3936">Data Lake Analytics</span></span>

* <span data-ttu-id="018bf-3937">Zusätzliche Befehle für Compute-Richtlinienverwaltung unter der Überschrift `dla account compute-policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3937">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="018bf-3938">`dla job pipeline show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3938">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="018bf-3939">`dla job recurrence list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3939">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="018bf-3940">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="018bf-3940">Data Lake Store</span></span>

* <span data-ttu-id="018bf-3941">Unterstützung für vom Benutzer verwaltete Schlüsseltresor-Schlüsselrotation in `dls account update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3941">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="018bf-3942">Zugrunde liegende SDK-Version des Data Lake Store-Dateisystems aktualisiert, um ein Leistungsproblem zu behandeln</span><span class="sxs-lookup"><span data-stu-id="018bf-3942">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="018bf-3943">Befehl `dls enable-key-vault` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="018bf-3943">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="018bf-3944">Dieser Befehl versucht, eine vom Benutzer angegebene Key Vault-Instanz zur Verschlüsselung der Daten in einem Data Lake Store-Konto zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="018bf-3944">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="018bf-3945">Interactive</span><span class="sxs-lookup"><span data-stu-id="018bf-3945">Interactive</span></span>

* <span data-ttu-id="018bf-3946">Startzeit durch Verwendung zwischengespeicherter Befehle verbessert</span><span class="sxs-lookup"><span data-stu-id="018bf-3946">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="018bf-3947">Testabdeckung verbessert</span><span class="sxs-lookup"><span data-stu-id="018bf-3947">Increased test coverage</span></span>
* <span data-ttu-id="018bf-3948">?-Geste erweitert, sodass sie auch in den nächsten Befehl eingefügt wird</span><span class="sxs-lookup"><span data-stu-id="018bf-3948">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="018bf-3949">Interaktive Fehler mit dem Profil „2017-03-09-profile-preview“ behoben (3587)</span><span class="sxs-lookup"><span data-stu-id="018bf-3949">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="018bf-3950">`--version` als Parameter für den interaktiven Modus zugelassen (3645)</span><span class="sxs-lookup"><span data-stu-id="018bf-3950">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="018bf-3951">Beseitigung von Fehlern im interaktiven Modus beim Abschluss von Überprüfungen (3570)</span><span class="sxs-lookup"><span data-stu-id="018bf-3951">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="018bf-3952">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="018bf-3952">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="018bf-3953">Flag `--progress` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3953">Added `--progress` flag</span></span>
* <span data-ttu-id="018bf-3954">`--debug` und `--verbose` aus Abschlüssen entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-3954">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="018bf-3955">`interactive` aus Abschlüssen entfernt (3324)</span><span class="sxs-lookup"><span data-stu-id="018bf-3955">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="018bf-3956">IoT</span><span class="sxs-lookup"><span data-stu-id="018bf-3956">IoT</span></span>

* <span data-ttu-id="018bf-3957">Behoben: Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="018bf-3957">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="018bf-3958">(3934)</span><span class="sxs-lookup"><span data-stu-id="018bf-3958">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="018bf-3959">Schlüsseltresor</span><span class="sxs-lookup"><span data-stu-id="018bf-3959">Key vault</span></span>

* <span data-ttu-id="018bf-3960">Befehle für Schlüsseltresor-Wiederherstellungsfeatures hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="018bf-3960">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="018bf-3961">`keyvault`-Unterbefehle: `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="018bf-3961">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="018bf-3962">`keyvault secret`-Unterbefehle: `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="018bf-3962">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="018bf-3963">`keyvault certificate`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="018bf-3963">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="018bf-3964">`keyvault key`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="018bf-3964">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="018bf-3965">Dienstprinzipal-Schlüsseltresorintegration hinzugefügt (3133)</span><span class="sxs-lookup"><span data-stu-id="018bf-3965">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="018bf-3966">Schlüsseltresor-Datenebene auf 0.3.2. aktualisiert</span><span class="sxs-lookup"><span data-stu-id="018bf-3966">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="018bf-3967">(3307)</span><span class="sxs-lookup"><span data-stu-id="018bf-3967">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="018bf-3968">Labor</span><span class="sxs-lookup"><span data-stu-id="018bf-3968">Lab</span></span>

* <span data-ttu-id="018bf-3969">Unterstützung für Übernahme eines beliebigen virtuellen Computers im Labor über `az lab vm claim` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3969">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="018bf-3970">Tabellenausgabeformatierer für `az lab vm list` und `az lab vm show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3970">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="018bf-3971">Überwachen</span><span class="sxs-lookup"><span data-stu-id="018bf-3971">Monitor</span></span>

* <span data-ttu-id="018bf-3972">Korrektur für Vorlagendatei mit Befehl `monitor autoscale-settings get-parameters-template` (3349)</span><span class="sxs-lookup"><span data-stu-id="018bf-3972">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="018bf-3973">`monitor alert-rule-incidents list` in `monitor alert list-incidents` umbenannt</span><span class="sxs-lookup"><span data-stu-id="018bf-3973">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="018bf-3974">`monitor alert-rule-incidents show` in `monitor alert show-incident` umbenannt</span><span class="sxs-lookup"><span data-stu-id="018bf-3974">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="018bf-3975">`monitor metric-defintions list` in `monitor metrics list-definitions` umbenannt</span><span class="sxs-lookup"><span data-stu-id="018bf-3975">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="018bf-3976">`monitor alert-rules` in `monitor alert` umbenannt</span><span class="sxs-lookup"><span data-stu-id="018bf-3976">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="018bf-3977">`monitor alert create` geändert:</span><span class="sxs-lookup"><span data-stu-id="018bf-3977">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="018bf-3978">Unterbefehle vom Typ `condition` und `action` akzeptieren keinen JSON-Code mehr.</span><span class="sxs-lookup"><span data-stu-id="018bf-3978">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="018bf-3979">Hinzufügung zahlreicher Parameter zur Vereinfachung der Regelerstellung</span><span class="sxs-lookup"><span data-stu-id="018bf-3979">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="018bf-3980">`location` nicht mehr erforderlich</span><span class="sxs-lookup"><span data-stu-id="018bf-3980">`location` no longer required</span></span>
  * <span data-ttu-id="018bf-3981">Hinzufügung von Namen- und ID-Unterstützung für Ziel</span><span class="sxs-lookup"><span data-stu-id="018bf-3981">Add name and ID support for target</span></span>
  * <span data-ttu-id="018bf-3982">Entfernung von `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="018bf-3982">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="018bf-3983">Umbenennung von `is-enabled` in `enabled` (nicht mehr erforderlich)</span><span class="sxs-lookup"><span data-stu-id="018bf-3983">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="018bf-3984">`description` wird nun abhängig von der angegebenen Bedingung auf einen Standardwert festgelegt.</span><span class="sxs-lookup"><span data-stu-id="018bf-3984">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="018bf-3985">Hinzufügung von Beispielen zur Verdeutlichung des neuen Formats</span><span class="sxs-lookup"><span data-stu-id="018bf-3985">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="018bf-3986">Unterstützung von Namen oder IDs für Befehle vom Typ `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="018bf-3986">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="018bf-3987">Komfortargumente und Beispiele zu `monitor alert rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3987">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="018bf-3988">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="018bf-3988">Network</span></span>

* <span data-ttu-id="018bf-3989">Befehl `list-private-access-services` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3989">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="018bf-3990">Argument `--private-access-services` zu `vnet subnet create` und `vnet subnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3990">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="018bf-3991">Problem behoben, das einen Fehler für `application-gateway redirect-config create` zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="018bf-3991">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="018bf-3992">Problem behoben, aufgrund dessen `application-gateway redirect-config update` nicht mit `--no-wait` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="018bf-3992">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="018bf-3993">Fehler behoben, der bei der Verwendung des Arguments `--servers` mit `application-gateway address-pool create` und `application-gateway address-pool update` aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="018bf-3993">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="018bf-3994">Befehle vom Typ `application-gateway redirect-config` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3994">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="018bf-3995">Befehle zu `application-gateway ssl-policy` hinzugefügt: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="018bf-3995">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="018bf-3996">Argumente zu `application-gateway ssl-policy set` hinzugefügt: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="018bf-3996">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="018bf-3997">Argumente zu `application-gateway http-settings create` und `application-gateway http-settings update` hinzugefügt: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="018bf-3997">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="018bf-3998">Argumente zu `application-gateway url-path-map create` und `application-gateway url-path-map update` hinzugefügt: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="018bf-3998">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="018bf-3999">Argument `--redirect-config` zu `application-gateway url-path-map rule create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-3999">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="018bf-4000">Unterstützung für `--no-wait` zu `application-gateway url-path-map rule delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-4000">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="018bf-4001">Argumente zu `application-gateway probe create` und `application-gateway probe update` hinzugefügt: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="018bf-4001">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="018bf-4002">Argument `--redirect-config` zu `application-gateway rule create` und `application-gateway rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-4002">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="018bf-4003">Unterstützung für `--accelerated-networking` zu `nic create` und `nic update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-4003">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="018bf-4004">Argument `--internal-dns-name-suffix` von `nic create` entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-4004">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="018bf-4005">Unterstützung für `--dns-servers` zu `nic update` und `nic create` hinzugefügt: Hinzufügung von Unterstützung für --dns-servers</span><span class="sxs-lookup"><span data-stu-id="018bf-4005">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="018bf-4006">Fehler korrigiert, aufgrund dessen `--local-address-prefixes` von `local-gateway create` ignoriert wurde</span><span class="sxs-lookup"><span data-stu-id="018bf-4006">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="018bf-4007">Unterstützung für `--dns-servers` zu `vnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-4007">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="018bf-4008">Fehler beim Erstellen eines Peerings ohne Routenfilterung mit `express-route peering create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="018bf-4008">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="018bf-4009">Fehler korrigiert, aufgrund dessen die Argumente `--provider` und `--bandwidth` nicht mit `express-route update` verwendet werden konnten</span><span class="sxs-lookup"><span data-stu-id="018bf-4009">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="018bf-4010">Fehler mit Standardlogik von `network watcher show-topology` korrigiert</span><span class="sxs-lookup"><span data-stu-id="018bf-4010">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="018bf-4011">Ausgabeformatierung für `network list-usages` verbessert</span><span class="sxs-lookup"><span data-stu-id="018bf-4011">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="018bf-4012">Verwendung der standardmäßigen Front-End-IP-Adresse für `application-gateway http-listener create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="018bf-4012">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="018bf-4013">Verwendung des Standardadresspools, der HTTP-Standardeinstellungen und des HTTP-Standardlisteners für `application-gateway rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="018bf-4013">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="018bf-4014">Verwendung der standardmäßigen Front-End-IP-Adresse und des standardmäßigen Back-End-Pools für `lb rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="018bf-4014">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="018bf-4015">Verwendung der standardmäßigen Front-End-IP-Adresse für `lb inbound-nat-rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="018bf-4015">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="018bf-4016">Profil</span><span class="sxs-lookup"><span data-stu-id="018bf-4016">Profile</span></span>

* <span data-ttu-id="018bf-4017">Unterstützung der Anmeldung innerhalb eines virtuellen Computers mit einer verwalteten Identität</span><span class="sxs-lookup"><span data-stu-id="018bf-4017">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="018bf-4018">Unterstützung der Ausgabe für `account show` im SDK-Authentifizierungsdateiformat</span><span class="sxs-lookup"><span data-stu-id="018bf-4018">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="018bf-4019">Anzeige von Warnungen für veraltete Befehle bei Verwendung von „--expanded-view“</span><span class="sxs-lookup"><span data-stu-id="018bf-4019">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="018bf-4020">Befehl `get-access-token` für die Bereitstellung eines unformatierten AAD-Tokens hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-4020">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="018bf-4021">Unterstützung der Anmeldung mit einem Benutzerkonto ohne zugeordnete Abonnements</span><span class="sxs-lookup"><span data-stu-id="018bf-4021">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="018bf-4022">RDBMS</span><span class="sxs-lookup"><span data-stu-id="018bf-4022">RDBMS</span></span>

* <span data-ttu-id="018bf-4023">Unterstützung der abonnementübergreifenden Auflistung von Servern (3417)</span><span class="sxs-lookup"><span data-stu-id="018bf-4023">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="018bf-4024">Behoben: `%s` wird aufgrund von fehlendem `% server_type` nicht verarbeitet (3393)</span><span class="sxs-lookup"><span data-stu-id="018bf-4024">Fixed `%s` not processed because of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="018bf-4025">Dokumentquellenzuordnung behoben und CI-Aufgabe zur Überprüfung hinzugefügt (3361)</span><span class="sxs-lookup"><span data-stu-id="018bf-4025">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="018bf-4026">MySQL- und PostgreSQL-Hilfe korrigiert (3369)</span><span class="sxs-lookup"><span data-stu-id="018bf-4026">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="018bf-4027">Resource</span><span class="sxs-lookup"><span data-stu-id="018bf-4027">Resource</span></span>

* <span data-ttu-id="018bf-4028">Eingabeaufforderungen bei fehlenden Parametern für `group deployment create` verbessert</span><span class="sxs-lookup"><span data-stu-id="018bf-4028">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="018bf-4029">Analyse der Syntax `--parameters KEY=VALUE` verbessert</span><span class="sxs-lookup"><span data-stu-id="018bf-4029">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="018bf-4030">Probleme behoben, durch die Parameterdateien von `group deployment create` bei Verwendung der Syntax `@<file>` nicht mehr erkannt wurden</span><span class="sxs-lookup"><span data-stu-id="018bf-4030">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="018bf-4031">Unterstützung des Arguments `--ids` für Befehle vom Typ `resource` und `managedapp`</span><span class="sxs-lookup"><span data-stu-id="018bf-4031">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="018bf-4032">Einige Analyse- und Fehlermeldungen korrigiert (3584)</span><span class="sxs-lookup"><span data-stu-id="018bf-4032">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="018bf-4033">Analyse vom Typ `--resource-type` für den Befehl `lock` korrigiert, sodass `<resource-namespace>` und `<resource-type>` akzeptiert werden</span><span class="sxs-lookup"><span data-stu-id="018bf-4033">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="018bf-4034">Parameterüberprüfung für Vorlagenlinkvorlagen hinzugefügt (3629)</span><span class="sxs-lookup"><span data-stu-id="018bf-4034">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="018bf-4035">Unterstützung für die Angabe von Bereitstellungsparametern mit der Syntax `KEY=VALUE` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-4035">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="018bf-4036">Role</span><span class="sxs-lookup"><span data-stu-id="018bf-4036">Role</span></span>

* <span data-ttu-id="018bf-4037">Unterstützung der Ausgabe im SDK-Authentifizierungsdateiformat für `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="018bf-4037">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="018bf-4038">Rollenzuweisungen und dazugehörige AAD-Anwendung beim Löschen eines Dienstprinzipals bereinigt (3610)</span><span class="sxs-lookup"><span data-stu-id="018bf-4038">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="018bf-4039">Einbeziehung des Zeitformats in Beschreibungen vom Typ `--start-date` und `--end-date` für `app create`-Argumente</span><span class="sxs-lookup"><span data-stu-id="018bf-4039">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="018bf-4040">Anzeige von Warnungen für veraltete Befehle bei Verwendung von `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="018bf-4040">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="018bf-4041">Schlüsseltresorintegration zu den Befehlen `create-for-rbac` und `reset-credentials` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-4041">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="018bf-4042">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="018bf-4042">Service Fabric</span></span>
* <span data-ttu-id="018bf-4043">Problem behoben, aufgrund dessen große Dateien in Anwendungen beim Hochladen gekürzt wurden (3666)</span><span class="sxs-lookup"><span data-stu-id="018bf-4043">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="018bf-4044">Tests für Service Fabric-Befehle hinzugefügt (3424)</span><span class="sxs-lookup"><span data-stu-id="018bf-4044">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="018bf-4045">Zahlreiche Service Fabric-Befehle korrigiert (3234)</span><span class="sxs-lookup"><span data-stu-id="018bf-4045">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="018bf-4046">SQL</span><span class="sxs-lookup"><span data-stu-id="018bf-4046">SQL</span></span>

* <span data-ttu-id="018bf-4047">Fehlerhafte1 Parameter `--identity` für `sql server create` entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-4047">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="018bf-4048">Kennwortwerte aus der Befehlsausgabe von `sql server create` und `sql server update` entfernt</span><span class="sxs-lookup"><span data-stu-id="018bf-4048">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="018bf-4049">Befehle `sql db list-editions` und `sql elastic-pool list-editions` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-4049">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="018bf-4050">Storage</span><span class="sxs-lookup"><span data-stu-id="018bf-4050">Storage</span></span>

* <span data-ttu-id="018bf-4051">Option `--marker` für die Befehle `storage blob list`, `storage container list` und `storage share list` entfernt (3745)</span><span class="sxs-lookup"><span data-stu-id="018bf-4051">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="018bf-4052">Erstellung eines reinen HTTPS-Speicherkontos ermöglicht</span><span class="sxs-lookup"><span data-stu-id="018bf-4052">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="018bf-4053">Speichermetriken, Protokollierung und CORS-Befehle aktualisiert (3495)</span><span class="sxs-lookup"><span data-stu-id="018bf-4053">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="018bf-4054">Ausnahmemeldung von „cors add“ umformuliert (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="018bf-4054">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="018bf-4055">Generator im Probelaufmodus des Downloadbatchbefehls in eine Liste konvertiert (3592)</span><span class="sxs-lookup"><span data-stu-id="018bf-4055">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="018bf-4056">Problem bei Probelauf des Blobdownloadbatchs behoben (3640) (3592)</span><span class="sxs-lookup"><span data-stu-id="018bf-4056">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="018bf-4057">VM</span><span class="sxs-lookup"><span data-stu-id="018bf-4057">VM</span></span>

* <span data-ttu-id="018bf-4058">Unterstützung der NSG-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="018bf-4058">Support configuring nsg</span></span>
* <span data-ttu-id="018bf-4059">Fehler behoben, aufgrund dessen der DNS-Server nicht ordnungsgemäß konfiguriert wurde</span><span class="sxs-lookup"><span data-stu-id="018bf-4059">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="018bf-4060">Unterstützung verwalteter Dienstidentitäten</span><span class="sxs-lookup"><span data-stu-id="018bf-4060">Support managed service identities</span></span>
* <span data-ttu-id="018bf-4061">Problem behoben, aufgrund dessen `cmss create` mit einem vorhandenen Lastenausgleich `--backend-pool-name` benötigte</span><span class="sxs-lookup"><span data-stu-id="018bf-4061">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="018bf-4062">Festlegung, dass die LUN von mit `vm image create` erstellten Datenträgern mit 0 beginnt</span><span class="sxs-lookup"><span data-stu-id="018bf-4062">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="018bf-4063">10. Mai 2017</span><span class="sxs-lookup"><span data-stu-id="018bf-4063">May 10, 2017</span></span>

<span data-ttu-id="018bf-4064">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="018bf-4064">Version 2.0.6</span></span>

* <span data-ttu-id="018bf-4065">Umbenennen von „documentdb“ in „cosmosdb“</span><span class="sxs-lookup"><span data-stu-id="018bf-4065">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="018bf-4066">Hinzufügen von rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="018bf-4066">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="018bf-4067">Einbeziehen der Data Lake Analytics- und Data Lake Store-Module</span><span class="sxs-lookup"><span data-stu-id="018bf-4067">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="018bf-4068">Einbeziehen des Cognitive Services-Moduls</span><span class="sxs-lookup"><span data-stu-id="018bf-4068">Include Cognitive Services module</span></span>
* <span data-ttu-id="018bf-4069">Einbeziehen des Service Fabric-Moduls</span><span class="sxs-lookup"><span data-stu-id="018bf-4069">Include Service Fabric module</span></span>
* <span data-ttu-id="018bf-4070">Einbeziehen des interaktiven Moduls (Umbenennen von „az-shell“)</span><span class="sxs-lookup"><span data-stu-id="018bf-4070">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="018bf-4071">Hinzufügen von Unterstützung für CDN-Befehle</span><span class="sxs-lookup"><span data-stu-id="018bf-4071">Add support for CDN commands</span></span>
* <span data-ttu-id="018bf-4072">Entfernen des Containermoduls</span><span class="sxs-lookup"><span data-stu-id="018bf-4072">Remove Container module</span></span>
* <span data-ttu-id="018bf-4073">Hinzufügen von „az -v“ als Verknüpfung für „az --version“ ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="018bf-4073">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="018bf-4074">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="018bf-4074">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="018bf-4075">Core</span><span class="sxs-lookup"><span data-stu-id="018bf-4075">Core</span></span>

* <span data-ttu-id="018bf-4076">Core: Erfassen von Ausnahmen, die durch einen nicht registrierten Anbieter verursacht werden, und automatische Registrierung</span><span class="sxs-lookup"><span data-stu-id="018bf-4076">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="018bf-4077">Leistung: Dauerhaftes Speichern des ADAL-Tokencaches im Arbeitsspeicher bis zum Prozessende ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="018bf-4077">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="018bf-4078">Korrigieren der vom hexadezimalen Fingerabdruck -o tsv zurückgegebenen Bytes ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="018bf-4078">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="018bf-4079">Verbessern des Downloads des Schlüsseltresorzertifikats und der AAD-SP-Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="018bf-4079">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="018bf-4080">Hinzufügen des Python-Speicherorts zu „az –version“ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="018bf-4080">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="018bf-4081">Anmeldung: Unterstützung der Anmeldung, wenn keine Abonnements vorhanden sind ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="018bf-4081">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="018bf-4082">Core: Beheben eines Fehlers bei zweimaliger Verwendung eines Dienstprinzipals bei der Anmeldung ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="018bf-4082">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="018bf-4083">Core: Ermöglichen der Konfiguration des Dateipfads von „accessTokens.json“ über eine Umgebungsvariable ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="018bf-4083">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="018bf-4084">Core: Zulassen der Anwendung konfigurierter Standardwerte auf optionale Argumente ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="018bf-4084">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="018bf-4085">Core: Verbesserte Leistung</span><span class="sxs-lookup"><span data-stu-id="018bf-4085">core: Improved performance</span></span>
* <span data-ttu-id="018bf-4086">Core: Zertifikate von benutzerdefinierter Zertifizierungsstelle – Unterstützung für das Festlegen der REQUESTS_CA_BUNDLE-Umgebungsvariablen</span><span class="sxs-lookup"><span data-stu-id="018bf-4086">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="018bf-4087">Core: Cloudkonfiguration – Verwenden des Endpunkts „resource manager“, wenn Endpunkt „management“ nicht festgelegt ist</span><span class="sxs-lookup"><span data-stu-id="018bf-4087">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="018bf-4088">ACS</span><span class="sxs-lookup"><span data-stu-id="018bf-4088">ACS</span></span>

* <span data-ttu-id="018bf-4089">Korrigieren der Master- und Agentanzahl als ganze Zahl statt Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="018bf-4089">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="018bf-4090">Verfügbarmachen von „az acs create --no-wait“ und „az acs wait“ für die asynchrone Erstellung</span><span class="sxs-lookup"><span data-stu-id="018bf-4090">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="018bf-4091">Verfügbarmachen von „az acs create --validate“ für Probelaufüberprüfungen</span><span class="sxs-lookup"><span data-stu-id="018bf-4091">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="018bf-4092">Entfernen von Windows-Profil vor PUT-Aufruf für Skalierungsbefehl ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="018bf-4092">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="018bf-4093">AppService</span><span class="sxs-lookup"><span data-stu-id="018bf-4093">AppService</span></span>

* <span data-ttu-id="018bf-4094">functionapp: Hinzufügen der vollständigen functionapp-Unterstützung, einschließlich Erstellen, Anzeigen, Auflisten, Löschen, Hostname, SSL usw.</span><span class="sxs-lookup"><span data-stu-id="018bf-4094">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="018bf-4095">Hinzufügen von Team Services (vsts) als Continuous Delivery-Option zu „appservice web source-control config“</span><span class="sxs-lookup"><span data-stu-id="018bf-4095">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="018bf-4096">Erstellen von „az webapp“ als Ersatz für „az appservice web“ (für Abwärtskompatibilität bleibt „az appservice web“ für 2 weitere Releases erhalten)</span><span class="sxs-lookup"><span data-stu-id="018bf-4096">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="018bf-4097">Verfügbarmachen von Argumenten zum Konfigurieren von Bereitstellung und Laufzeitstapeln beim Erstellen von Web-Apps</span><span class="sxs-lookup"><span data-stu-id="018bf-4097">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="018bf-4098">Verfügbarmachen von „webapp list-runtimes“</span><span class="sxs-lookup"><span data-stu-id="018bf-4098">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="018bf-4099">Unterstützen der Konfiguration von Verbindungszeichenfolgen ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="018bf-4099">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="018bf-4100">Unterstützen des Slottauschs mit Vorschau</span><span class="sxs-lookup"><span data-stu-id="018bf-4100">support slot swap with preview</span></span>
* <span data-ttu-id="018bf-4101">Beheben von Fehlern in appservice-Befehlen ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="018bf-4101">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="018bf-4102">Verwenden der Ressourcengruppe des App Service-Plans für Zertifizierungsvorgänge ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="018bf-4102">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="018bf-4103">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="018bf-4103">CosmosDB</span></span>

* <span data-ttu-id="018bf-4104">Umbenennen des documentdb-Moduls in cosmosdb</span><span class="sxs-lookup"><span data-stu-id="018bf-4104">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="018bf-4105">Zusätzliche Unterstützung für documentdb-APIs auf Datenebene: Datenbank- und Sammlungsverwaltung</span><span class="sxs-lookup"><span data-stu-id="018bf-4105">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="018bf-4106">Zusätzliche Unterstützung für das Aktivieren des automatischen Failovers für Datenbankkonten</span><span class="sxs-lookup"><span data-stu-id="018bf-4106">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="018bf-4107">Zusätzliche Unterstützung für die neue ConsistentPrefix-Konsistenzrichtlinie</span><span class="sxs-lookup"><span data-stu-id="018bf-4107">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="018bf-4108">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="018bf-4108">Data Lake Analytics</span></span>

* <span data-ttu-id="018bf-4109">Beheben eines Fehlers, bei dem das Filtern von Auftragslisten nach Ergebnis und Status einen Fehler auslöst</span><span class="sxs-lookup"><span data-stu-id="018bf-4109">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="018bf-4110">Hinzufügen von Unterstützung für den neuen Katalogelementtyp „Paket“</span><span class="sxs-lookup"><span data-stu-id="018bf-4110">Add support for new catalog item type: package.</span></span> <span data-ttu-id="018bf-4111">Zugriff über: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="018bf-4111">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="018bf-4112">Ermöglichen der Auflistung folgender Katalogelemente innerhalb einer Datenbank (keine Schemaspezifikation erforderlich):</span><span class="sxs-lookup"><span data-stu-id="018bf-4112">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="018bf-4113">Tabelle</span><span class="sxs-lookup"><span data-stu-id="018bf-4113">Table</span></span>
  * <span data-ttu-id="018bf-4114">Tabellenwertfunktion</span><span class="sxs-lookup"><span data-stu-id="018bf-4114">Table valued function</span></span>
  * <span data-ttu-id="018bf-4115">Sicht</span><span class="sxs-lookup"><span data-stu-id="018bf-4115">View</span></span>
  * <span data-ttu-id="018bf-4116">Tabellenstatistiken.</span><span class="sxs-lookup"><span data-stu-id="018bf-4116">Table Statistics.</span></span> <span data-ttu-id="018bf-4117">Können auch mit einem Schema, jedoch ohne Angabe eines Tabellennamens aufgelistet werden.</span><span class="sxs-lookup"><span data-stu-id="018bf-4117">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="018bf-4118">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="018bf-4118">Data Lake Store</span></span>

* <span data-ttu-id="018bf-4119">Aktualisieren der Version des zugrunde liegenden Dateisystem-SDK, wodurch eine bessere Unterstützung für die Verarbeitung von Drosselungsszenarien auf Serverseite gewährt wird</span><span class="sxs-lookup"><span data-stu-id="018bf-4119">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="018bf-4120">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="018bf-4120">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="018bf-4121">Fehlende Hilfe für Zugriffsanzeige</span><span class="sxs-lookup"><span data-stu-id="018bf-4121">missed help for access show.</span></span> <span data-ttu-id="018bf-4122">hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="018bf-4122">adding it.</span></span> <span data-ttu-id="018bf-4123">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="018bf-4123">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="018bf-4124">Suchen</span><span class="sxs-lookup"><span data-stu-id="018bf-4124">Find</span></span>

* <span data-ttu-id="018bf-4125">Verbessern von Suchergebnissen und Ermöglichen der Versionsverwaltung des Suchindex</span><span class="sxs-lookup"><span data-stu-id="018bf-4125">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="018bf-4126">KeyVault</span><span class="sxs-lookup"><span data-stu-id="018bf-4126">KeyVault</span></span>

* <span data-ttu-id="018bf-4127">BC:`az keyvault certificate download` Ändern von „-e“ von Zeichenfolge oder Binärdatentyp in PEM oder DER zur besseren Darstellung der Optionen</span><span class="sxs-lookup"><span data-stu-id="018bf-4127">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="018bf-4128">BC: Entfernen von „--expires“ und „--not-before“ aus `keyvault certificate create`, da diese Parameter nicht vom Dienst unterstützt werden</span><span class="sxs-lookup"><span data-stu-id="018bf-4128">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="018bf-4129">Hinzufügen des Parameters „--validity“ zu `keyvault certificate create`, um gezielt den Wert in „--policy“ zu überschreiben</span><span class="sxs-lookup"><span data-stu-id="018bf-4129">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="018bf-4130">Beheben des Problems in `keyvault certificate get-default-policy`, bei dem „expires“ und „not_before“ verfügbar gemacht wurden, „validity_in_months“ hingegen nicht</span><span class="sxs-lookup"><span data-stu-id="018bf-4130">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="018bf-4131">Keyvault-Korrektur für den Import von PEM und PFX ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="018bf-4131">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="018bf-4132">Labor</span><span class="sxs-lookup"><span data-stu-id="018bf-4132">Lab</span></span>

* <span data-ttu-id="018bf-4133">Hinzufügen der Befehle „create“, „show“, „delete“ und „list“ für die Laborumgebung</span><span class="sxs-lookup"><span data-stu-id="018bf-4133">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="018bf-4134">Hinzufügen der Befehle „show“ und „list“ zur Anzeige von ARM-Vorlagen im Labor</span><span class="sxs-lookup"><span data-stu-id="018bf-4134">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="018bf-4135">Hinzufügen des Kennzeichens „--environment“ in `az lab vm list`, um virtuelle Computer nach Umgebung im Labor zu filtern</span><span class="sxs-lookup"><span data-stu-id="018bf-4135">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="018bf-4136">Hinzufügen des benutzerfreundlichen Befehls `az lab formula export-artifacts` zum Exportieren des Artefaktgerüsts innerhalb der Formel eines Labors</span><span class="sxs-lookup"><span data-stu-id="018bf-4136">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="018bf-4137">Hinzufügen von Befehlen zum Verwalten von Geheimnissen in einem Labor</span><span class="sxs-lookup"><span data-stu-id="018bf-4137">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="018bf-4138">Überwachen</span><span class="sxs-lookup"><span data-stu-id="018bf-4138">Monitor</span></span>

* <span data-ttu-id="018bf-4139">Fehlerbehebung: Modellieren von `--actions` von `az alert-rules create` zum Verarbeiten von JSON-Zeichenfolgen ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="018bf-4139">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="018bf-4140">Programmfehlerbehebung: Beim Erstellen von Diagnoseeinstellungen werden Protokolle/Metriken aus Anzeigebefehlen nicht akzeptiert ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="018bf-4140">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="018bf-4141">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="018bf-4141">Network</span></span>

* <span data-ttu-id="018bf-4142">Hinzufügen des `network watcher test-connectivity`-Befehls</span><span class="sxs-lookup"><span data-stu-id="018bf-4142">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="018bf-4143">Hinzufügen von Unterstützung für den `--filters`-Parameter für `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="018bf-4143">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="018bf-4144">Hinzufügen von Unterstützung für den Application Gateway-Verbindungsausgleich</span><span class="sxs-lookup"><span data-stu-id="018bf-4144">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="018bf-4145">Hinzufügen von Unterstützung für die Konfiguration von Application Gateway-WAF-Regelsätzen</span><span class="sxs-lookup"><span data-stu-id="018bf-4145">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="018bf-4146">Hinzufügen von Unterstützung für ExpressRoute-Routenfilter und -Regeln</span><span class="sxs-lookup"><span data-stu-id="018bf-4146">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="018bf-4147">Hinzufügen von Unterstützung für geografisches TrafficManager-Routing</span><span class="sxs-lookup"><span data-stu-id="018bf-4147">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="018bf-4148">Hinzufügen von Unterstützung für richtlinienbasierte Datenverkehrsselektoren für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="018bf-4148">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="018bf-4149">Hinzufügen von Unterstützung für IPSec-Richtlinien für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="018bf-4149">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="018bf-4150">Korrektur eines Fehlers bei `vpn-connection create` bei Verwendung der Parameter `--no-wait` oder `--validate`</span><span class="sxs-lookup"><span data-stu-id="018bf-4150">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="018bf-4151">Hinzufügen von Unterstützung für Aktiv/Aktiv-VNET-Gateways</span><span class="sxs-lookup"><span data-stu-id="018bf-4151">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="018bf-4152">Entfernen von NULL-Werten aus der Ausgabe von `network vpn-connection list/show`-Befehlen</span><span class="sxs-lookup"><span data-stu-id="018bf-4152">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="018bf-4153">BC: Korrektur eines Fehlers in der Ausgabe von `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="018bf-4153">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="018bf-4154">Korrektur eines Fehlers, bei dem das Argument „--key-length“ von „vpn-connection create“ nicht ordnungsgemäß analysiert wurde</span><span class="sxs-lookup"><span data-stu-id="018bf-4154">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="018bf-4155">Korrektur eines Fehlers in `dns zone import`, bei dem Datensätze nicht ordnungsgemäß importiert wurden</span><span class="sxs-lookup"><span data-stu-id="018bf-4155">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="018bf-4156">Korrektur eines Fehlers, bei dem `traffic-manager endpoint update` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="018bf-4156">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="018bf-4157">Hinzufügen von Network Watcher-Vorschaubefehlen</span><span class="sxs-lookup"><span data-stu-id="018bf-4157">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="018bf-4158">Profil</span><span class="sxs-lookup"><span data-stu-id="018bf-4158">Profile</span></span>

* <span data-ttu-id="018bf-4159">Unterstützung der Anmeldung, wenn keine Abonnements gefunden werden ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="018bf-4159">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="018bf-4160">Unterstützung für kurze Parameternamen in „az account set --subscription“ ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="018bf-4160">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="018bf-4161">Redis</span><span class="sxs-lookup"><span data-stu-id="018bf-4161">Redis</span></span>

* <span data-ttu-id="018bf-4162">Hinzufügen des Updatebefehls, durch den auch die Möglichkeit zum Skalieren für Redis Cache hinzugefügt wird</span><span class="sxs-lookup"><span data-stu-id="018bf-4162">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="018bf-4163">Verwerfen des Befehls „update-settings“</span><span class="sxs-lookup"><span data-stu-id="018bf-4163">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="018bf-4164">Resource</span><span class="sxs-lookup"><span data-stu-id="018bf-4164">Resource</span></span>

* <span data-ttu-id="018bf-4165">Hinzufügen der Befehle „managedapp“ und „managedapp definition“ ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="018bf-4165">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="018bf-4166">Unterstützung für die „provider operation“-Befehle ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="018bf-4166">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="018bf-4167">Unterstützung für die Erstellung generischer Ressourcen ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="018bf-4167">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="018bf-4168">Korrigieren der Ressourcenanalyse und der API-Versionssuche</span><span class="sxs-lookup"><span data-stu-id="018bf-4168">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="018bf-4169">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="018bf-4169">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="018bf-4170">Hinzufügen von Dokumenten für „az lock update“</span><span class="sxs-lookup"><span data-stu-id="018bf-4170">Add docs for az lock update.</span></span> <span data-ttu-id="018bf-4171">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="018bf-4171">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="018bf-4172">Beenden mit Fehler bei dem Versuch, Ressourcen für eine nicht vorhandene Gruppe aufzulisten</span><span class="sxs-lookup"><span data-stu-id="018bf-4172">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="018bf-4173">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="018bf-4173">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="018bf-4174">[Compute] Beheben von Problemen mit dem Update von VMSS- und VM-Verfügbarkeitsgruppen</span><span class="sxs-lookup"><span data-stu-id="018bf-4174">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="018bf-4175">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="018bf-4175">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="018bf-4176">Korrigieren des Erstellungs- und Löschvorgangs für Sperren, wenn „parent-resource-path“ auf „None“ festgelegt ist ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="018bf-4176">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="018bf-4177">Role</span><span class="sxs-lookup"><span data-stu-id="018bf-4177">Role</span></span>

* <span data-ttu-id="018bf-4178">create-for-rbac: Sicherstellen, dass das SP-Enddatum nicht das Ablaufdatum des Zertifikats überschreitet ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="018bf-4178">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="018bf-4179">RBAC: Hinzufügen vollständiger Unterstützung für „ad group“ ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="018bf-4179">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="018bf-4180">Rolle: Beheben von Probleme beim Rollendefinitionsupdate ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="018bf-4180">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="018bf-4181">create-for-rbac: Sicherstellen, dass das angegebene Benutzerkennwort übernommen wird</span><span class="sxs-lookup"><span data-stu-id="018bf-4181">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="018bf-4182">SQL</span><span class="sxs-lookup"><span data-stu-id="018bf-4182">SQL</span></span>

* <span data-ttu-id="018bf-4183">Hinzufügen der Befehle „az sql server list-usages“ und „az sql db list-usages“</span><span class="sxs-lookup"><span data-stu-id="018bf-4183">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="018bf-4184">SQL: Möglichkeit zur direkten Verbindung mit Ressourcenanbieter ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="018bf-4184">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="018bf-4185">Storage</span><span class="sxs-lookup"><span data-stu-id="018bf-4185">Storage</span></span>

* <span data-ttu-id="018bf-4186">Festlegen des Ressourcengruppenstandorts als Standardstandort für `storage account create`</span><span class="sxs-lookup"><span data-stu-id="018bf-4186">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="018bf-4187">Hinzufügen von Unterstützung für das inkrementelle Kopieren von Blobs</span><span class="sxs-lookup"><span data-stu-id="018bf-4187">Add support for incremental blob copy</span></span>
* <span data-ttu-id="018bf-4188">Hinzufügen von Unterstützung für den Upload umfangreicher Blockblobs</span><span class="sxs-lookup"><span data-stu-id="018bf-4188">Add support for large block blob upload</span></span>
* <span data-ttu-id="018bf-4189">Ändern der Blockgröße auf 100 MB, wenn die hochzuladende Datei größer als 200 GB ist</span><span class="sxs-lookup"><span data-stu-id="018bf-4189">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="018bf-4190">VM</span><span class="sxs-lookup"><span data-stu-id="018bf-4190">VM</span></span>

* <span data-ttu-id="018bf-4191">avail-set: Festlegen der UD- und FD-Domänenanzahl als optional</span><span class="sxs-lookup"><span data-stu-id="018bf-4191">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="018bf-4192">Hinweis: VM-Befehle in unabhängigen Clouds: Vermeiden Sie Features im Zusammenhang mit verwalteten Datenträgern, einschließlich der folgenden:</span><span class="sxs-lookup"><span data-stu-id="018bf-4192">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="018bf-4193">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="018bf-4193">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="018bf-4194">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="018bf-4194">az vm/vmss disk</span></span>
  3. <span data-ttu-id="018bf-4195">Verwenden Sie in „az vm/vmss create“ den Befehl „—use-unmanaged-disk“, um verwaltete Datenträger zu vermeiden. Andere Befehle sollten funktionieren.</span><span class="sxs-lookup"><span data-stu-id="018bf-4195">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="018bf-4196">vm/vmss: Verbessern des Warnungstexts beim Generieren von SSH-Schlüsselpaaren</span><span class="sxs-lookup"><span data-stu-id="018bf-4196">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="018bf-4197">vm/vmss: Unterstützen der Erstellung über ein Marketplace-Image, für das Planinformationen erforderlich sind ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="018bf-4197">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="018bf-4198">3\. April 2017</span><span class="sxs-lookup"><span data-stu-id="018bf-4198">April 3, 2017</span></span>

<span data-ttu-id="018bf-4199">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="018bf-4199">Version 2.0.2</span></span>

<span data-ttu-id="018bf-4200">In dieser Version wurden die Komponenten ACR, Batch, KeyVault und SQL eingeführt.</span><span class="sxs-lookup"><span data-stu-id="018bf-4200">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="018bf-4201">Core</span><span class="sxs-lookup"><span data-stu-id="018bf-4201">Core</span></span>

* <span data-ttu-id="018bf-4202">Hinzufügen der Module „acr“, „lab“, „monitor“ und „find“ zur Standardliste</span><span class="sxs-lookup"><span data-stu-id="018bf-4202">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="018bf-4203">Anmeldung: Überspringen des fehlerhaften Mandanten ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="018bf-4203">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="018bf-4204">Anmeldung: Festlegen des Standardabonnements auf ein Abonnement mit dem Status „Enabled“ ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="018bf-4204">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="018bf-4205">Hinzufügen von wait-Befehlen und Unterstützung von „--no-wait“ für mehr Befehle ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="018bf-4205">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="018bf-4206">Core: Unterstützen der Anmeldung per Dienstprinzipal mit einem Zertifikat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="018bf-4206">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="018bf-4207">Hinzufügen der Meldung zu fehlenden Vorlagenparametern</span><span class="sxs-lookup"><span data-stu-id="018bf-4207">Add prompting for missing template parameters.</span></span> <span data-ttu-id="018bf-4208">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="018bf-4208">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="018bf-4209">Unterstützen des Festlegens von Standardwerten für häufig verwendete Argumente, z.B. Standardressourcengruppe, Standardweb und Standard-VM</span><span class="sxs-lookup"><span data-stu-id="018bf-4209">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="018bf-4210">Unterstützen der Anmeldung an einem bestimmten Mandanten</span><span class="sxs-lookup"><span data-stu-id="018bf-4210">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="018bf-4211">ACS</span><span class="sxs-lookup"><span data-stu-id="018bf-4211">ACS</span></span>

* <span data-ttu-id="018bf-4212">[ACS] Hinzufügen von Unterstützung für die Konfiguration eines ACS-Standardclusters ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="018bf-4212">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="018bf-4213">Hinzufügen von Unterstützung der Aufforderung zur Kennworteingabe für SSH-Schlüssel</span><span class="sxs-lookup"><span data-stu-id="018bf-4213">Add support for ssh key password prompting.</span></span> <span data-ttu-id="018bf-4214">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="018bf-4214">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="018bf-4215">Hinzufügen von Unterstützung für Windows-Cluster</span><span class="sxs-lookup"><span data-stu-id="018bf-4215">Add support for windows clusters.</span></span> <span data-ttu-id="018bf-4216">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="018bf-4216">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="018bf-4217">Wechseln von der Rolle „Besitzer“ zur Rolle „Mitwirkender“</span><span class="sxs-lookup"><span data-stu-id="018bf-4217">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="018bf-4218">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="018bf-4218">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="018bf-4219">AppService</span><span class="sxs-lookup"><span data-stu-id="018bf-4219">AppService</span></span>

* <span data-ttu-id="018bf-4220">appservice: Unterstützung für das Abrufen der externen IP-Adresse für DNS A-Einträge ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="018bf-4220">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="018bf-4221">appservice: Unterstützung der Bindung von Platzhalterzertifikaten ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="018bf-4221">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="018bf-4222">appservice: Unterstützung von Veröffentlichungsprofilen für Listen ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="018bf-4222">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="018bf-4223">AppService: Auslösen der Synchronisierung der Quellcodeverwaltung nach der Konfiguration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="018bf-4223">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="018bf-4224">DataLake</span><span class="sxs-lookup"><span data-stu-id="018bf-4224">DataLake</span></span>

* <span data-ttu-id="018bf-4225">Erste Version des Data Lake Analytics-Moduls</span><span class="sxs-lookup"><span data-stu-id="018bf-4225">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="018bf-4226">Erste Version des Data Lake Store-Moduls</span><span class="sxs-lookup"><span data-stu-id="018bf-4226">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="018bf-4227">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="018bf-4227">DocuemntDB</span></span>

* <span data-ttu-id="018bf-4228">DocumentDB: Hinzufügen von Unterstützung für das Auflisten von Verbindungszeichenfolgen ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="018bf-4228">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="018bf-4229">VM</span><span class="sxs-lookup"><span data-stu-id="018bf-4229">VM</span></span>

* <span data-ttu-id="018bf-4230">[Compute] Hinzufügen von AppGateway-Unterstützung für Erstellung von VM-Skalierungsgruppen ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="018bf-4230">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="018bf-4231">[VM/VMSS] Verbesserte Unterstützung für die Datenträgerzwischenspeicherung ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="018bf-4231">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="018bf-4232">VM/VMSS: Einbinden der vom Portal verwendeten Logik zur Überprüfung von Anmeldeinformationen ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="018bf-4232">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="018bf-4233">Hinzufügen von wait-Befehlen und Unterstützung für „--no-wait“ ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="018bf-4233">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="018bf-4234">VM-Skalierungsgruppe: Unterstützung von „\*“ zum Auflisten der übergreifenden Instanzansicht für VMs ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="018bf-4234">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="018bf-4235">Hinzufügen – Geheimnisse für virtuellen Computer und VM-Skalierungsgruppe ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="018bf-4235">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="018bf-4236">Zulassen der VM-Erstellung mit spezialisierter VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="018bf-4236">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="018bf-4237">27. Februar 2017</span><span class="sxs-lookup"><span data-stu-id="018bf-4237">February 27, 2017</span></span>

<span data-ttu-id="018bf-4238">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="018bf-4238">Version 2.0.0</span></span>

<span data-ttu-id="018bf-4239">Diese Version der Azure CLI 2.0 ist die erste „allgemein verfügbare“ Version. Die allgemeine Verfügbarkeit gilt für die folgenden Befehlsmodule:</span><span class="sxs-lookup"><span data-stu-id="018bf-4239">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="018bf-4240">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="018bf-4240">Container Service (acs)</span></span>
- <span data-ttu-id="018bf-4241">Compute (einschließlich Resource Manager, VM, VM-Skalierungsgruppen, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="018bf-4241">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="018bf-4242">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="018bf-4242">Networking</span></span>
- <span data-ttu-id="018bf-4243">Storage</span><span class="sxs-lookup"><span data-stu-id="018bf-4243">Storage</span></span>

<span data-ttu-id="018bf-4244">Diese Befehlsmodule können in der Produktion verwendet werden und verfügen über Unterstützung durch eine Standard-SLA von Microsoft. Sie können Anfragen zu Problemen direkt beim Microsoft-Support oder in der [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/) öffnen. Sie haben die Möglichkeit, Fragen in [StackOverflow mit dem Tag „azure-cli“](http://stackoverflow.com/questions/tagged/azure-cli) zu stellen oder sich unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) an das Produktteam zu wenden. Außerdem können Sie über die Befehlszeile mit dem Befehl `az feedback` Feedback senden.</span><span class="sxs-lookup"><span data-stu-id="018bf-4244">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="018bf-4245">Die Befehle in diesen Modulen sind stabil, und es ist nicht zu erwarten, dass sich die Syntax in den anstehenden Veröffentlichungen dieser Version der Azure CLI ändern.</span><span class="sxs-lookup"><span data-stu-id="018bf-4245">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="018bf-4246">Verwenden Sie zum Überprüfen der Version der CLI den Befehl `az --version`. In der Ausgabe werden die Version der CLI selbst (für diese Veröffentlichung 2.0.0), die einzelnen Befehlsmodule und die von Ihnen genutzten Versionen von Python und GCC aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="018bf-4246">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="018bf-4247">Einige Befehlsmodule verfügen über das Postfix „b *n* “ oder „rc *n* “. Diese Befehlsmodule befinden sich noch in der Vorschauphase und werden später die allgemeine Verfügbarkeit erlangen.</span><span class="sxs-lookup"><span data-stu-id="018bf-4247">Some of the command modules have a "b *n* " or "rc *n* " postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="018bf-4248">Außerdem werden jeden Abend Vorschaubuilds der CLI bereitgestellt. Informationen hierzu finden Sie in der [Anleitung zum Abrufen der abendlichen Builds](https://github.com/Azure/azure-cli#nightly-builds) und im Abschnitt zum [Setup für Entwickler und Beitragen von Code](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="018bf-4248">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="018bf-4249">Sie können für die abendlichen Vorschaubuilds wie folgt Probleme melden:</span><span class="sxs-lookup"><span data-stu-id="018bf-4249">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="018bf-4250">Über die [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="018bf-4250">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="018bf-4251">Per Kontaktaufnahme mit dem Produktteam unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="018bf-4251">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="018bf-4252">Senden von Feedback über die Befehlszeile mit dem Befehl `az feedback`</span><span class="sxs-lookup"><span data-stu-id="018bf-4252">Provide feedback from the command line with the `az feedback` command</span></span>

# <a name="beta-release-notes"></a>[<span data-ttu-id="018bf-4253">Versionshinweise zur Betaversion</span><span class="sxs-lookup"><span data-stu-id="018bf-4253">Beta release notes</span></span>](#tab/azure-cli-beta)

<span data-ttu-id="018bf-4254">Die Azure CLI-Betaversion ist eine Migration der Authentifizierungsmethode der AAD-Plattform (v1.0) zu [Microsoft Identity Platform (v2.0)](/azure/active-directory/develop/v2-overview).</span><span class="sxs-lookup"><span data-stu-id="018bf-4254">The Azure CLI beta release is a migration from the authentican method of AAD platform (v1.0) to [Microsoft Identity platform (v2.0)](/azure/active-directory/develop/v2-overview).</span></span>

## <a name="june-23-2020"></a><span data-ttu-id="018bf-4255">23. Juni 2020</span><span class="sxs-lookup"><span data-stu-id="018bf-4255">June 23, 2020</span></span>

### <a name="things-to-know-about-the-new-azure-cli-beta-release"></a><span data-ttu-id="018bf-4256">Wissenswertes über die neue Azure CLI-Betaversion</span><span class="sxs-lookup"><span data-stu-id="018bf-4256">Things to know about the new Azure CLI beta release</span></span>

-   <span data-ttu-id="018bf-4257">Die Betaversion der Azure CLI unterstützt alle CLI-Befehle, die in der aktuellen veröffentlichten Version verfügbar sind.</span><span class="sxs-lookup"><span data-stu-id="018bf-4257">The beta version of the Azure CLI supports all CLI commands that you will find in the current released version.</span></span>
-   <span data-ttu-id="018bf-4258">Nach der Installation der Betaversion ist eine erneute Anmeldung erforderlich.</span><span class="sxs-lookup"><span data-stu-id="018bf-4258">Relogin is required after install the beta version.</span></span>
-   <span data-ttu-id="018bf-4259">Die Betaversion unterstützt nur die Windows-Plattform.</span><span class="sxs-lookup"><span data-stu-id="018bf-4259">The beta release only supports the Windows platform.</span></span>
-   <span data-ttu-id="018bf-4260">Azure Stack wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="018bf-4260">The Azure Stack is not supported.</span></span>
-   <span data-ttu-id="018bf-4261">Parameter `--use-cert-sn-issuer` wird nicht unterstützt, wenn für die Authentifizierung ein Dienstprinzipalschlüssel verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="018bf-4261">`--use-cert-sn-issuer` parameter is not supported when using service principal key to authenticate.</span></span>
-   <span data-ttu-id="018bf-4262">Das Überspringen der SSL-Überprüfung über die Umgebung `ADAL_PYTHON_SSL_NO_VERIFY` wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="018bf-4262">Skip SSL verification via environment `ADAL_PYTHON_SSL_NO_VERIFY` is not supported.</span></span>

<span data-ttu-id="018bf-4263">Sollten Probleme in der Betaversion auftreten, können Sie auf [GitHub](https://github.com/Azure/azure-cli/issues/new/choose) gerne Kommentare für das Azure CLI-Entwicklungsteam hinterlassen.</span><span class="sxs-lookup"><span data-stu-id="018bf-4263">If you find any issues in the beta release, the Azure CLI engineering team welcomes your comments on [GitHub](https://github.com/Azure/azure-cli/issues/new/choose).</span></span>

---
